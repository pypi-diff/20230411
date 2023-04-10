# Comparing `tmp/basinmaker-3.0.1.tar.gz` & `tmp/basinmaker-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basinmaker-3.0.1.tar", last modified: Mon Nov  7 01:12:40 2022, max compression
+gzip compressed data, was "basinmaker-3.0.3.tar", last modified: Mon Apr 10 22:43:29 2023, max compression
```

## Comparing `basinmaker-3.0.1.tar` & `basinmaker-3.0.3.tar`

### file list

```diff
@@ -1,124 +1,141 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.884791 basinmaker-3.0.1/
--rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.0.1/LICENSE
--rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5505 2022-11-07 01:12:40.884791 basinmaker-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:39.742846 basinmaker-3.0.1/basinmaker/
--rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.0.1/basinmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:39.911406 basinmaker-3.0.1/basinmaker/addattributes/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/__init__.py
--rw-rw-rw-   0        0        0    12375 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/addattributestocatchments.py
--rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/addgaugeattributesqgis.py
--rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/addlakeattributesqgis.py
--rw-rw-rw-   0        0        0    12356 2022-10-05 15:00:15.000000 basinmaker-3.0.1/basinmaker/addattributes/calbkfwidthdepthqgis.py
--rw-rw-rw-   0        0        0    16556 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/calculatebasicattributesqgis.py
--rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/calfloodmanningnqgis.py
--rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/createattributestemplateqgis.py
--rw-rw-rw-   0        0        0     5657 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/exportoutputsqgis.py
--rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addattributes/joinpandastoattributesqgis.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.036061 basinmaker-3.0.1/basinmaker/addlakeandobs/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/__init__.py
--rw-rw-rw-   0        0        0    10182 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
--rw-rw-rw-   0        0        0     4401 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/addlakesarcgis.py
--rw-rw-rw-   0        0        0    13820 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/addlakesqgis.py
--rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/addobsqgis.py
--rw-rw-rw-   0        0        0     6295 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/definecatrivqgis.py
--rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/definelaketypeqgis.py
--rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/filterlakesqgis.py
--rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/modifyfdr.py
--rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/modifystr.py
--rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/addlakeandobs/pourpointsqgis.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.094903 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/__init__.py
--rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
--rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
--rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
--rw-rw-rw-   0        0        0    60438 2022-08-17 19:35:25.000000 basinmaker-3.0.1/basinmaker/basinmaker.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.195634 basinmaker-3.0.1/basinmaker/delineationnolake/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/__init__.py
--rw-rw-rw-   0        0        0     8666 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watdelineationwithoutlake.py
--rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingdemarcgis.py
--rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingdemqgis.py
--rw-rw-rw-   0        0        0     3008 2022-10-23 19:36:41.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingfacqgis.py
--rw-rw-rw-   0        0        0     3024 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingfdrarcgis.py
--rw-rw-rw-   0        0        0     2969 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingfdrqgis.py
--rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/delineationnolake/watusingsubregionddata.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.270435 basinmaker-3.0.1/basinmaker/extent/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/extent/__init__.py
--rw-rw-rw-   0        0        0     7487 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/extent/projectextent.py
--rw-rw-rw-   0        0        0     2997 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/extent/usingdemarcgis.py
--rw-rw-rw-   0        0        0     4681 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/extent/usingdemqgis.py
--rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.0.1/basinmaker/extent/usinghybasinplyarcgis.py
--rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/extent/usinghybasinplyqgis.py
--rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/extent/usinginputplyqgis.py
--rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/extent/usingoutletpointqgis.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.388121 basinmaker-3.0.1/basinmaker/func/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.415047 basinmaker-3.0.1/basinmaker/func/__pycache__/
--rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5911 2022-09-07 00:49:52.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
--rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
--rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    45502 2022-11-02 00:12:26.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
--rw-rw-rw-   0        0        0    10057 2022-10-19 23:52:13.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/purepy.cpython-39.pyc
--rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/qgis.cpython-39.pyc
--rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.0.1/basinmaker/func/__pycache__/rarray.cpython-39.pyc
--rw-rw-rw-   0        0        0     9482 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/arcgis.py
--rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/fgdal.py
--rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/grassgis.py
--rw-rw-rw-   0        0        0   133734 2022-11-02 00:12:18.000000 basinmaker-3.0.1/basinmaker/func/pdtable.py
--rw-rw-rw-   0        0        0    16723 2022-10-19 23:50:34.000000 basinmaker-3.0.1/basinmaker/func/purepy.py
--rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/qgis.py
--rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/func/rarray.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.438984 basinmaker-3.0.1/basinmaker/hymodin/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/hymodin/__init__.py
--rw-rw-rw-   0        0        0    92299 2022-09-07 14:28:11.000000 basinmaker-3.0.1/basinmaker/hymodin/raveninput.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.766108 basinmaker-3.0.1/basinmaker/postprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     6523 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/combine.py
--rw-rw-rw-   0        0        0     6633 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/combinearcgis.py
--rw-rw-rw-   0        0        0     5706 2022-10-30 21:03:14.000000 basinmaker-3.0.1/basinmaker/postprocessing/combinepurepy.py
--rw-rw-rw-   0        0        0     7406 2022-09-11 02:48:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/downloadpd.py
--rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/downloadpdptspurepy.py
--rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/gridweight.py
--rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/gridweightarcgis.py
--rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/hru.py
--rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.0.1/basinmaker/postprocessing/hruarcgis.py
--rw-rw-rw-   0        0        0    37449 2022-10-13 03:27:29.000000 basinmaker-3.0.1/basinmaker/postprocessing/hrupurepy.py
--rw-rw-rw-   0        0        0    11006 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/increaseda.py
--rw-rw-rw-   0        0        0     9110 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/increasedaarcgis.py
--rw-rw-rw-   0        0        0     8745 2022-11-01 02:14:40.000000 basinmaker-3.0.1/basinmaker/postprocessing/increasedapurepy.py
--rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.0.1/basinmaker/postprocessing/inversetopology.py
--rw-rw-rw-   0        0        0     7866 2022-08-17 20:39:07.000000 basinmaker-3.0.1/basinmaker/postprocessing/plotleaflet.py
--rw-rw-rw-   0        0        0    14174 2022-08-17 20:01:18.000000 basinmaker-3.0.1/basinmaker/postprocessing/postprocessingfunctions.py
--rw-rw-rw-   0        0        0    10928 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectlake.py
--rw-rw-rw-   0        0        0     8937 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectlakearcgis.py
--rw-rw-rw-   0        0        0     8133 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectlakepurepy.py
--rw-rw-rw-   0        0        0    11993 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectprod.py
--rw-rw-rw-   0        0        0    10886 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectprodarcgis.py
--rw-rw-rw-   0        0        0     7424 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/postprocessing/selectprodpurepy.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.846892 basinmaker-3.0.1/basinmaker/preprocessing/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/preinputpolygonqgis.py
--rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/preprocessinglakeply.py
--rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/preprocessingobs.py
--rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/preprocessrasterqgis.py
--rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
--rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.873820 basinmaker-3.0.1/basinmaker/subreg/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/subreg/__init__.py
--rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/subreg/defsubreg.py
--rw-rw-rw-   0        0        0    37889 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/subreg/generatesubregionqgis.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:40.882796 basinmaker-3.0.1/basinmaker/utilities/
--rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/utilities/__init__.py
--rw-rw-rw-   0        0        0     7265 2022-08-17 20:01:19.000000 basinmaker-3.0.1/basinmaker/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2022-11-07 01:12:39.760799 basinmaker-3.0.1/basinmaker.egg-info/
--rw-rw-rw-   0        0        0     5505 2022-11-07 01:12:39.000000 basinmaker-3.0.1/basinmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4430 2022-11-07 01:12:39.000000 basinmaker-3.0.1/basinmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 01:12:39.000000 basinmaker-3.0.1/basinmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-11-07 01:12:39.000000 basinmaker-3.0.1/basinmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-07 01:12:40.885788 basinmaker-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      828 2022-11-07 00:56:40.000000 basinmaker-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:29.030584 basinmaker-3.0.3/
+-rw-rw-rw-   0        0        0     8852 2022-07-20 16:58:36.000000 basinmaker-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-07-20 16:58:36.000000 basinmaker-3.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5505 2023-04-10 22:43:29.030584 basinmaker-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2022-07-20 16:58:36.000000 basinmaker-3.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.622676 basinmaker-3.0.3/basinmaker/
+-rw-rw-rw-   0        0        0        0 2022-07-20 16:58:36.000000 basinmaker-3.0.3/basinmaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.679523 basinmaker-3.0.3/basinmaker/addattributes/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/__init__.py
+-rw-rw-rw-   0        0        0    13278 2023-03-04 13:49:59.000000 basinmaker-3.0.3/basinmaker/addattributes/addattributestocatchments.py
+-rw-rw-rw-   0        0        0     2915 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/addgaugeattributesqgis.py
+-rw-rw-rw-   0        0        0     6980 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/addlakeattributesqgis.py
+-rw-rw-rw-   0        0        0    12534 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addattributes/calbkfwidthdepthqgis.py
+-rw-rw-rw-   0        0        0    17015 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addattributes/calculatebasicattributesqgis.py
+-rw-rw-rw-   0        0        0     3919 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/calfloodmanningnqgis.py
+-rw-rw-rw-   0        0        0    20857 2023-03-17 02:53:13.000000 basinmaker-3.0.3/basinmaker/addattributes/createattributestemplatearcgis.py
+-rw-rw-rw-   0        0        0     1403 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/createattributestemplateqgis.py
+-rw-rw-rw-   0        0        0     5634 2023-03-04 13:50:28.000000 basinmaker-3.0.3/basinmaker/addattributes/exportoutputsqgis.py
+-rw-rw-rw-   0        0        0     2844 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addattributes/joinpandastoattributesqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.714429 basinmaker-3.0.3/basinmaker/addlakeandobs/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/__init__.py
+-rw-rw-rw-   0        0        0    10672 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakeandobsintowatershed.py
+-rw-rw-rw-   0        0        0     7245 2023-03-27 15:33:34.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesarcgis.py
+-rw-rw-rw-   0        0        0    14219 2022-12-12 16:45:02.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addlakesqgis.py
+-rw-rw-rw-   0        0        0     3984 2023-02-09 00:34:07.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addobsarcgis.py
+-rw-rw-rw-   0        0        0     6701 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/addobsqgis.py
+-rw-rw-rw-   0        0        0     5535 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivarcgis.py
+-rw-rw-rw-   0        0        0     6490 2022-12-12 17:39:29.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivqgis.py
+-rw-rw-rw-   0        0        0     1859 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/definelaketypeqgis.py
+-rw-rw-rw-   0        0        0     4943 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/filterlakesqgis.py
+-rw-rw-rw-   0        0        0    31231 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/modifyfdr.py
+-rw-rw-rw-   0        0        0     3281 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/modifystr.py
+-rw-rw-rw-   0        0        0    16301 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/addlakeandobs/pourpointsqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.733380 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/__init__.py
+-rw-rw-rw-   0        0        0     1826 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1141 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1377 2022-08-17 20:01:16.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0      626 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0     1194 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py
+-rw-rw-rw-   0        0        0    68581 2023-04-10 22:39:55.000000 basinmaker-3.0.3/basinmaker/basinmaker.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.757320 basinmaker-3.0.3/basinmaker/delineationnolake/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/__init__.py
+-rw-rw-rw-   0        0        0     8657 2023-01-03 01:23:58.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watdelineationwithoutlake.py
+-rw-rw-rw-   0        0        0     3000 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemarcgis.py
+-rw-rw-rw-   0        0        0     2079 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemqgis.py
+-rw-rw-rw-   0        0        0     3018 2022-11-27 20:34:05.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfacqgis.py
+-rw-rw-rw-   0        0        0     3282 2023-04-02 02:37:44.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrarcgis.py
+-rw-rw-rw-   0        0        0     2915 2023-01-03 01:24:50.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrqgis.py
+-rw-rw-rw-   0        0        0     2339 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/delineationnolake/watusingsubregionddata.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.784244 basinmaker-3.0.3/basinmaker/extent/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/extent/__init__.py
+-rw-rw-rw-   0        0        0     7764 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/projectextent.py
+-rw-rw-rw-   0        0        0     3492 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/usingdemarcgis.py
+-rw-rw-rw-   0        0        0     4841 2022-12-18 02:16:17.000000 basinmaker-3.0.3/basinmaker/extent/usingdemqgis.py
+-rw-rw-rw-   0        0        0     4900 2022-08-17 20:01:17.000000 basinmaker-3.0.3/basinmaker/extent/usinghybasinplyarcgis.py
+-rw-rw-rw-   0        0        0     7193 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usinghybasinplyqgis.py
+-rw-rw-rw-   0        0        0     6027 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usinginputplyqgis.py
+-rw-rw-rw-   0        0        0     6861 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/extent/usingoutletpointqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.808179 basinmaker-3.0.3/basinmaker/func/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.837102 basinmaker-3.0.3/basinmaker/func/__pycache__/
+-rw-rw-rw-   0        0        0      164 2022-08-17 20:03:20.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    18510 2023-02-27 03:41:01.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/arcgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6084 2022-08-17 20:05:59.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/fgdal.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15904 2022-08-18 02:30:26.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/grassgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    47805 2023-04-01 13:38:31.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/pdtable.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10361 2022-11-27 20:15:59.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/purepy.cpython-39.pyc
+-rw-rw-rw-   0        0        0    26797 2022-08-18 02:30:27.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/qgis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    12224 2022-08-18 02:30:32.000000 basinmaker-3.0.3/basinmaker/func/__pycache__/rarray.cpython-39.pyc
+-rw-rw-rw-   0        0        0    35090 2023-02-27 03:39:45.000000 basinmaker-3.0.3/basinmaker/func/arcgis.py
+-rw-rw-rw-   0        0        0     9448 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/fgdal.py
+-rw-rw-rw-   0        0        0    27465 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/grassgis.py
+-rw-rw-rw-   0        0        0   139946 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/func/pdtable.py
+-rw-rw-rw-   0        0        0    17567 2023-04-10 21:29:09.000000 basinmaker-3.0.3/basinmaker/func/purepy.py
+-rw-rw-rw-   0        0        0    42623 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/qgis.py
+-rw-rw-rw-   0        0        0    25878 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/func/rarray.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.844084 basinmaker-3.0.3/basinmaker/hymodin/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/hymodin/__init__.py
+-rw-rw-rw-   0        0        0    92339 2022-11-17 01:32:01.000000 basinmaker-3.0.3/basinmaker/hymodin/raveninput.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.926861 basinmaker-3.0.3/basinmaker/postprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0    10250 2023-04-01 13:38:13.000000 basinmaker-3.0.3/basinmaker/postprocessing/assigninterestsites.py
+-rw-rw-rw-   0        0        0     6500 2023-03-04 13:51:54.000000 basinmaker-3.0.3/basinmaker/postprocessing/combine.py
+-rw-rw-rw-   0        0        0     6538 2023-03-04 13:52:08.000000 basinmaker-3.0.3/basinmaker/postprocessing/combinearcgis.py
+-rw-rw-rw-   0        0        0     5693 2023-03-04 13:52:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/combinepurepy.py
+-rw-rw-rw-   0        0        0     7412 2023-04-01 14:30:36.000000 basinmaker-3.0.3/basinmaker/postprocessing/downloadpd.py
+-rw-rw-rw-   0        0        0     2836 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/downloadpdptspurepy.py
+-rw-rw-rw-   0        0        0    21586 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/gridweight.py
+-rw-rw-rw-   0        0        0     3482 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/gridweightarcgis.py
+-rw-rw-rw-   0        0        0    59494 2022-08-17 20:01:18.000000 basinmaker-3.0.3/basinmaker/postprocessing/hru.py
+-rw-rw-rw-   0        0        0    40585 2022-09-07 02:20:09.000000 basinmaker-3.0.3/basinmaker/postprocessing/hruarcgis.py
+-rw-rw-rw-   0        0        0    38578 2022-11-27 18:54:39.000000 basinmaker-3.0.3/basinmaker/postprocessing/hrupurepy.py
+-rw-rw-rw-   0        0        0    10971 2023-03-04 13:53:00.000000 basinmaker-3.0.3/basinmaker/postprocessing/increaseda.py
+-rw-rw-rw-   0        0        0     9072 2023-03-04 14:14:28.000000 basinmaker-3.0.3/basinmaker/postprocessing/increasedaarcgis.py
+-rw-rw-rw-   0        0        0     8693 2023-03-04 13:53:46.000000 basinmaker-3.0.3/basinmaker/postprocessing/increasedapurepy.py
+-rw-rw-rw-   0        0        0     3303 2022-09-11 18:50:03.000000 basinmaker-3.0.3/basinmaker/postprocessing/inversetopology.py
+-rw-rw-rw-   0        0        0     8035 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/plotleaflet.py
+-rw-rw-rw-   0        0        0    15290 2023-02-05 00:48:12.000000 basinmaker-3.0.3/basinmaker/postprocessing/postprocessingfunctions.py
+-rw-rw-rw-   0        0        0    10902 2023-03-04 14:03:13.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlake.py
+-rw-rw-rw-   0        0        0     8912 2023-03-04 14:08:34.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlakearcgis.py
+-rw-rw-rw-   0        0        0     8114 2023-03-04 14:09:00.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectlakepurepy.py
+-rw-rw-rw-   0        0        0    11957 2023-03-04 14:09:12.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprod.py
+-rw-rw-rw-   0        0        0    11211 2023-03-04 14:09:22.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprodarcgis.py
+-rw-rw-rw-   0        0        0     7266 2023-04-01 13:38:19.000000 basinmaker-3.0.3/basinmaker/postprocessing/selectprodpurepy.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.958776 basinmaker-3.0.3/basinmaker/preprocessing/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     1180 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preinputpolygonqgis.py
+-rw-rw-rw-   0        0        0     3446 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessinglakeply.py
+-rw-rw-rw-   0        0        0     1363 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessingobs.py
+-rw-rw-rw-   0        0        0     2665 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/preprocessrasterqgis.py
+-rw-rw-rw-   0        0        0     4187 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py
+-rw-rw-rw-   0        0        0     3610 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.973736 basinmaker-3.0.3/basinmaker/subreg/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/subreg/__init__.py
+-rw-rw-rw-   0        0        0     3612 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/subreg/defsubreg.py
+-rw-rw-rw-   0        0        0    38989 2022-11-23 01:59:53.000000 basinmaker-3.0.3/basinmaker/subreg/generatesubregionqgis.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.980718 basinmaker-3.0.3/basinmaker/utilities/
+-rw-rw-rw-   0        0        0        0 2022-08-17 20:01:19.000000 basinmaker-3.0.3/basinmaker/utilities/__init__.py
+-rw-rw-rw-   0        0        0     7554 2022-11-27 20:24:39.000000 basinmaker-3.0.3/basinmaker/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:28.649610 basinmaker-3.0.3/basinmaker.egg-info/
+-rw-rw-rw-   0        0        0     5505 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 22:43:28.000000 basinmaker-3.0.3/basinmaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-07-20 16:58:37.000000 basinmaker-3.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:43:29.033578 basinmaker-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-01-22 00:27:34.000000 basinmaker-3.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:43:29.027593 basinmaker-3.0.3/tests/
+-rw-rw-rw-   0        0        0     5251 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_AutomatedWatershedsandLakesFilterToolset.py
+-rw-rw-rw-   0        0        0     6085 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_Generateinputdata.py
+-rw-rw-rw-   0        0        0     6187 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_Generatmaskregion.py
+-rw-rw-rw-   0        0        0     5729 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Customize_Routing_Topology.py
+-rw-rw-rw-   0        0        0     2298 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Define_Final_Catchment.py
+-rw-rw-rw-   0        0        0     3378 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateHRUS.py
+-rw-rw-rw-   0        0        0     3474 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_GenerateRavenInput.py
+-rw-rw-rw-   0        0        0     1966 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Locate_subid_needsbyuser.py
+-rw-rw-rw-   0        0        0     4695 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_SelectLakes.py
+-rw-rw-rw-   0        0        0     7034 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_PostProcessing_Select_Routing_product_based_SubId.py
+-rw-rw-rw-   0        0        0     5916 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_RoutingNetworkTopologyUpdateToolset_riv.py
+-rw-rw-rw-   0        0        0     6998 2022-07-20 16:58:37.000000 basinmaker-3.0.3/tests/test_RoutingTool_WatershedDiscretizationToolset.py
```

### Comparing `basinmaker-3.0.1/LICENSE` & `basinmaker-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/PKG-INFO` & `basinmaker-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.1
+Version: 3.0.3
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.1/README.md` & `basinmaker-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/addattributestocatchments.py` & `basinmaker-3.0.3/basinmaker/addattributes/addattributestocatchments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,299 +1,316 @@
-from basinmaker.utilities.utilities import *
-from basinmaker.func.pdtable import *
-
-
-def add_attributes_to_catchments(
-    input_geo_names,
-    path_bkfwidthdepth="#",
-    bkfwd_attributes=[],
-    path_landuse="#",
-    path_landuse_info="#",
-    path_k_c_zone_polygon = '#',
-    k_in=-1,
-    c_in=-1,
-    out_cat_name="catchment_without_merging_lakes",
-    out_riv_name="river_without_merging_lakes",
-    grassdb="#",
-    grass_location="#",
-    qgis_prefix_path="#",
-    gis_platform="qgis",
-    projection="EPSG:3573",
-    obs_attributes=[],
-    lake_attributes=[],
-    outlet_obs_id=1,
-    path_sub_reg_outlets_v="#",
-    output_folder="#",
-):
-
-    """Calculate hydrological paramters
-
-    Calculate hydrological paramters for each subbasin generated by
-    "AutomatedWatershedsandLakesFilterToolset". The result generaed
-    by this tool can be used as inputs for Define_Final_Catchment
-    and other post processing tools
-
-    Parameters
-    ----------
-    input_geo_names                : dict
-        it is a dictionary that list the required input file names,should at
-        least indicate the name of following items:
-        sl_nonconnect_lake          : raster
-            it is a raster represent all non connected lakes that are selected
-            by lake area threstholds
-        sl_connected_lake           : raster
-            it is a raster represent allconnected lakes that are selected
-            by lake area threstholds
-        river_without_merging_lakes : raster/vector
-            it is the updated river segment for each subbasin
-        catchment_without_merging_lakes   : raster/vector
-            it is a raster represent updated subbasins after adding lake inflow
-            and outflow points as new subbasin outlet.
-        snapped_obs_points          : raster/vector
-            it is a name of the point gis file represent successfully sanpped
-            observation points
-
-    path_bkfwidthdepth             : string
-        It is a string to indicate the full path of the
-        polyline shapefile that having bankfull width and
-        depth data
-    bkfwd_attributes               :
-        the columns names that indicate following items has to be included
-        1) column name for the Bankfull width in m;
-        2) column name for the Bankfull depth in m;
-        3) column name for the annual mean discharge in m3/s;
-    path_landuse                   : string
-        It is a string to indicate the full path of the landuse data.
-        It will be used to estimate the floodplain roughness
-        coefficient. Should have the same projection with the DEM data
-        in ".tif" format.
-    path_landuse_info              : string
-        It is a string to indicate the full path of the table in '.csv'
-        format.The table describe the floodplain roughness coefficient
-        correspond to a given landuse type. The table should have two
-        columns: RasterV and MannV. RasterV is the landuse value in the
-        landuse raster for each land use type and the MannV is the
-        roughness coefficient value for each landuse type.
-    gis_platform                   : string
-        It is a string indicate with gis platform is used:
-        'qgis'                : the basinmaker is running within QGIS
-        'arcgis'              : the basinmaker is running within ArcGIS
-    lake_attributes                : list
-        the columns names that indicate following items has to be included
-        1) column name for the unique Id of each lake within the lake polygon shpfile;
-        2) column name for type of the lake should be integer;
-        3) column name for the volume of the lake in km3;
-        4) column name for the average depth of the lake in m;
-        5) column name for the area of the lake in km2.
-    obs_attributes                 : list
-        the columns names that indicate following items has to be included
-        1) column name for the unique Id of each observation point;
-        2) column name for the unique name of each observation point;
-        3) column name for the drainage area of each observation point in km3;
-        4) column name for the source of the observation point:
-            'CA' for observation in canada;
-            'US' for observation in US;
-    outlet_obs_id                  : int
-        It is one 'Obs_ID' in the provided observation gauge
-        shapefile. If it is larger than zero. Subbasins that
-        do not drainage to this gauge will be removed from
-        delineation result.
-    projection                     : string
-        It is a string indicate a projected coordinate system,
-        which wiil be used to calcuate area, slope and aspect.
-    output_folder                  : string
-        The path to a folder to save outputs
-    path_sub_reg_outlets_v         : string
-
-    Notes
-    -------
-    Five vector files will be generated by this function. these files
-    can be used to define final routing structure by "Define_Final_Catchment"
-    or be used as input for other postprocessing tools. All files
-    are stored at self.OutputFolder
-
-    catchment_without_merging_lakes.shp             : shapefile
-        It is the subbasin polygon before merging lakes catchments and
-        need to be processed before used.
-    river_without_merging_lakes.shp                 : shapefile
-        It is the subbasin river segment before merging lakes catchments and
-        need to be processed before used.
-    sl_connected_lake.shp                           : shapefile
-        It is the connected lake polygon. Connected lakes are lakes that
-        are connected by  Path_final_riv.
-    sl_non_connected_lake.shp                       : shapefile
-        It is the  non connected lake polygon. Connected lakes are lakes
-        that are not connected by Path_final_cat_riv or Path_final_riv.
-    obs_gauges                                      : shapefile
-        It is the point shapefile that represent the observation gauge
-        after snap to river network.
-
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-
-    """
-
-    columns = COLUMN_NAMES_CONSTANT
-    coltypes = COLUMN_TYPES_CONSTANT
-
-    # local geo file names
-    cat_ply_info = Internal_Constant_Names["cat_ply_info"]
-    cat_riv_info = Internal_Constant_Names["cat_riv_info"]
-    outlet_pt_info = Internal_Constant_Names["outlet_pt_info"]
-
-    if not os.path.exists(output_folder):
-        os.makedirs(output_folder)
-
-    if gis_platform == "qgis":
-        assert (
-            grassdb != "#"
-        ), "grass database folder is needed, when gis_platform = qgis"
-        assert (
-            grass_location != "#"
-        ), "grass location name is needed, when gis_platform = qgis"
-        assert (
-            qgis_prefix_path != "#"
-        ), "qgis prefix path is needed, when gis_platform = qgis"
-        from basinmaker.addattributes.createattributestemplateqgis import (
-            create_catchments_attributes_template_table,
-        )
-        from basinmaker.addattributes.calculatebasicattributesqgis import (
-            calculate_basic_attributes,
-        )
-        from basinmaker.addattributes.addlakeattributesqgis import add_lake_attributes
-        from basinmaker.addattributes.joinpandastoattributesqgis import (
-            join_pandas_table_to_vector_attributes,
-        )
-        from basinmaker.addattributes.exportoutputsqgis import export_files_to_output_folder
-        from basinmaker.addattributes.addgaugeattributesqgis import add_gauge_attributes
-        from basinmaker.addattributes.calfloodmanningnqgis import calculate_flood_plain_manning_n
-        from basinmaker.addattributes.calbkfwidthdepthqgis import (
-            calculate_bankfull_width_depth_from_polyline,
-        )
-
-        attr_template = create_catchments_attributes_template_table(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            columns=columns,
-            input_geo_names=input_geo_names,
-        )
-        
-        attr_basic = calculate_basic_attributes(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            qgis_prefix_path=qgis_prefix_path,
-            input_geo_names=input_geo_names,
-            projection=projection,
-            catinfo=attr_template,
-            cat_ply_info=cat_ply_info,
-            cat_riv_info=cat_riv_info,
-            outlet_pt_info=outlet_pt_info,
-        )
-        input_geo_names["cat_ply_info"] = cat_ply_info
-        input_geo_names["cat_riv_info"] = cat_riv_info
-        input_geo_names["outlet_pt_info"] = outlet_pt_info
-        
-        if len(lake_attributes) > 0:
-            attr_lake = add_lake_attributes(
-                grassdb=grassdb,
-                grass_location=grass_location,
-                qgis_prefix_path=qgis_prefix_path,
-                input_geo_names=input_geo_names,
-                lake_attributes=lake_attributes,
-                catinfo=attr_basic,
-            )
-        else:
-            attr_lake = attr_basic
-        
-        if len(obs_attributes) > 0:
-            attr_obs = add_gauge_attributes(
-                grassdb=grassdb,
-                grass_location=grass_location,
-                qgis_prefix_path=qgis_prefix_path,
-                input_geo_names=input_geo_names,
-                obs_attributes=obs_attributes,
-                catinfo=attr_lake,
-            )
-        else:
-            attr_obs = attr_lake
-        
-        if outlet_obs_id > 0:
-            attr_select = return_interest_catchments_info(
-                catinfo=attr_obs,
-                outlet_obs_id=outlet_obs_id,
-                path_sub_reg_outlets_v=path_sub_reg_outlets_v,
-            )
-        else:
-            attr_select = attr_obs
-        
-        if path_landuse != "#":
-            attr_landuse = calculate_flood_plain_manning_n(
-                grassdb=grassdb,
-                grass_location=grass_location,
-                qgis_prefix_path=qgis_prefix_path,
-                catinfo=attr_select,
-                input_geo_names=input_geo_names,
-                path_landuse=path_landuse,
-                path_landuse_info=path_landuse_info,
-            )
-        else:
-            attr_landuse = attr_select
-        
-        attr_da = streamorderanddrainagearea(attr_landuse)
-         
-        if path_bkfwidthdepth != "#" or k_in != -1 or path_k_c_zone_polygon != '#':
-            attr_bkf = calculate_bankfull_width_depth_from_polyline(
-                grassdb=grassdb,
-                grass_location=grass_location,
-                qgis_prefix_path=qgis_prefix_path,
-                path_bkfwidthdepth=path_bkfwidthdepth,
-                path_k_c_zone_polygon = path_k_c_zone_polygon,
-                bkfwd_attributes=bkfwd_attributes,
-                catinfo=attr_da,
-                input_geo_names=input_geo_names,
-                k_in=k_in,
-                c_in=k_in,
-            )
-        else:
-            attr_bkf = attr_da
-        
-        attr_ncl = update_non_connected_catchment_info(attr_bkf)
-        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'RivSlope'] = -1.2345
-        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'FloodP_n'] = -1.2345
-        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Max_DEM'] = -1.2345
-        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Min_DEM'] = -1.2345
-        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Ch_n'] = -1.2345
-        
-        join_pandas_table_to_vector_attributes(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            qgis_prefix_path=qgis_prefix_path,
-            vector_name=cat_ply_info,
-            pd_table=attr_ncl,
-            column_types=coltypes,
-            columns_names=columns,
-        )
-        
-        join_pandas_table_to_vector_attributes(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            qgis_prefix_path=qgis_prefix_path,
-            vector_name=cat_riv_info,
-            pd_table=attr_ncl,
-            column_types=coltypes,
-            columns_names=columns,
-        )
-
-        export_files_to_output_folder(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            qgis_prefix_path=qgis_prefix_path,
-            input_geo_names=input_geo_names,
-            output_riv=out_riv_name,
-            output_cat=out_cat_name,
-            output_folder=output_folder,
-            obs_attributes = obs_attributes,
-        )
+from basinmaker.utilities.utilities import *
+from basinmaker.func.pdtable import *
+
+
+def add_attributes_to_catchments(
+    input_geo_names,
+    path_bkfwidthdepth="#",
+    bkfwd_attributes=[],
+    path_landuse="#",
+    path_landuse_info="#",
+    path_k_c_zone_polygon = '#',
+    k_in=-1,
+    c_in=-1,
+    out_cat_name="catchment_without_merging_lakes",
+    out_riv_name="river_without_merging_lakes",
+    grassdb="#",
+    grass_location="#",
+    qgis_prefix_path="#",
+    gis_platform="qgis",
+    projection="EPSG:3573",
+    obs_attributes=[],
+    lake_attributes=[],
+    outlet_obs_id=1,
+    path_sub_reg_outlets_v="#",
+    output_folder="#",
+):
+
+    """Calculate hydrological paramters
+
+    Calculate hydrological paramters for each subbasin generated by
+    "AutomatedWatershedsandLakesFilterToolset". The result generaed
+    by this tool can be used as inputs for Define_Final_Catchment
+    and other post processing tools
+
+    Parameters
+    ----------
+    input_geo_names                : dict
+        it is a dictionary that list the required input file names,should at
+        least indicate the name of following items:
+        sl_nonconnect_lake          : raster
+            it is a raster represent all non connected lakes that are selected
+            by lake area threstholds
+        sl_connected_lake           : raster
+            it is a raster represent allconnected lakes that are selected
+            by lake area threstholds
+        river_without_merging_lakes : raster/vector
+            it is the updated river segment for each subbasin
+        catchment_without_merging_lakes   : raster/vector
+            it is a raster represent updated subbasins after adding lake inflow
+            and outflow points as new subbasin outlet.
+        snapped_obs_points          : raster/vector
+            it is a name of the point gis file represent successfully sanpped
+            observation points
+
+    path_bkfwidthdepth             : string
+        It is a string to indicate the full path of the
+        polyline shapefile that having bankfull width and
+        depth data
+    bkfwd_attributes               :
+        the columns names that indicate following items has to be included
+        1) column name for the Bankfull width in m;
+        2) column name for the Bankfull depth in m;
+        3) column name for the annual mean discharge in m3/s;
+    path_landuse                   : string
+        It is a string to indicate the full path of the landuse data.
+        It will be used to estimate the floodplain roughness
+        coefficient. Should have the same projection with the DEM data
+        in ".tif" format.
+    path_landuse_info              : string
+        It is a string to indicate the full path of the table in '.csv'
+        format.The table describe the floodplain roughness coefficient
+        correspond to a given landuse type. The table should have two
+        columns: RasterV and MannV. RasterV is the landuse value in the
+        landuse raster for each land use type and the MannV is the
+        roughness coefficient value for each landuse type.
+    gis_platform                   : string
+        It is a string indicate with gis platform is used:
+        'qgis'                : the basinmaker is running within QGIS
+        'arcgis'              : the basinmaker is running within ArcGIS
+    lake_attributes                : list
+        the columns names that indicate following items has to be included
+        1) column name for the unique Id of each lake within the lake polygon shpfile;
+        2) column name for type of the lake should be integer;
+        3) column name for the volume of the lake in km3;
+        4) column name for the average depth of the lake in m;
+        5) column name for the area of the lake in km2.
+    obs_attributes                 : list
+        the columns names that indicate following items has to be included
+        1) column name for the unique Id of each observation point;
+        2) column name for the unique name of each observation point;
+        3) column name for the drainage area of each observation point in km3;
+        4) column name for the source of the observation point:
+            'CA' for observation in canada;
+            'US' for observation in US;
+    outlet_obs_id                  : int
+        It is one 'Obs_ID' in the provided observation gauge
+        shapefile. If it is larger than zero. Subbasins that
+        do not drainage to this gauge will be removed from
+        delineation result.
+    projection                     : string
+        It is a string indicate a projected coordinate system,
+        which wiil be used to calcuate area, slope and aspect.
+    output_folder                  : string
+        The path to a folder to save outputs
+    path_sub_reg_outlets_v         : string
+
+    Notes
+    -------
+    Five vector files will be generated by this function. these files
+    can be used to define final routing structure by "Define_Final_Catchment"
+    or be used as input for other postprocessing tools. All files
+    are stored at self.OutputFolder
+
+    catchment_without_merging_lakes.shp             : shapefile
+        It is the subbasin polygon before merging lakes catchments and
+        need to be processed before used.
+    river_without_merging_lakes.shp                 : shapefile
+        It is the subbasin river segment before merging lakes catchments and
+        need to be processed before used.
+    sl_connected_lake.shp                           : shapefile
+        It is the connected lake polygon. Connected lakes are lakes that
+        are connected by  Path_final_riv.
+    sl_non_connected_lake.shp                       : shapefile
+        It is the  non connected lake polygon. Connected lakes are lakes
+        that are not connected by Path_final_cat_riv or Path_final_riv.
+    poi                                             : shapefile
+        It is the point shapefile that represent the observation gauge
+        after snap to river network.
+
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+
+    """
+
+    columns = COLUMN_NAMES_CONSTANT
+    coltypes = COLUMN_TYPES_CONSTANT
+
+    # local geo file names
+    cat_ply_info = Internal_Constant_Names["cat_ply_info"]
+    cat_riv_info = Internal_Constant_Names["cat_riv_info"]
+    outlet_pt_info = Internal_Constant_Names["outlet_pt_info"]
+
+    if not os.path.exists(output_folder):
+        os.makedirs(output_folder)
+
+    if gis_platform == "qgis":
+        assert (
+            grassdb != "#"
+        ), "grass database folder is needed, when gis_platform = qgis"
+        assert (
+            grass_location != "#"
+        ), "grass location name is needed, when gis_platform = qgis"
+        assert (
+            qgis_prefix_path != "#"
+        ), "qgis prefix path is needed, when gis_platform = qgis"
+        from basinmaker.addattributes.createattributestemplateqgis import (
+            create_catchments_attributes_template_table,
+        )
+        from basinmaker.addattributes.calculatebasicattributesqgis import (
+            calculate_basic_attributes,
+        )
+        from basinmaker.addattributes.addlakeattributesqgis import add_lake_attributes
+        from basinmaker.addattributes.joinpandastoattributesqgis import (
+            join_pandas_table_to_vector_attributes,
+        )
+        from basinmaker.addattributes.exportoutputsqgis import export_files_to_output_folder
+        from basinmaker.addattributes.addgaugeattributesqgis import add_gauge_attributes
+        from basinmaker.addattributes.calfloodmanningnqgis import calculate_flood_plain_manning_n
+        from basinmaker.addattributes.calbkfwidthdepthqgis import (
+            calculate_bankfull_width_depth_from_polyline,
+        )
+
+        attr_template = create_catchments_attributes_template_table(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            columns=columns,
+            input_geo_names=input_geo_names,
+        )
+
+        attr_basic = calculate_basic_attributes(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            qgis_prefix_path=qgis_prefix_path,
+            input_geo_names=input_geo_names,
+            projection=projection,
+            catinfo=attr_template,
+            cat_ply_info=cat_ply_info,
+            cat_riv_info=cat_riv_info,
+            outlet_pt_info=outlet_pt_info,
+        )
+        input_geo_names["cat_ply_info"] = cat_ply_info
+        input_geo_names["cat_riv_info"] = cat_riv_info
+        input_geo_names["outlet_pt_info"] = outlet_pt_info
+
+        if len(lake_attributes) > 0:
+            attr_lake = add_lake_attributes(
+                grassdb=grassdb,
+                grass_location=grass_location,
+                qgis_prefix_path=qgis_prefix_path,
+                input_geo_names=input_geo_names,
+                lake_attributes=lake_attributes,
+                catinfo=attr_basic,
+            )
+        else:
+            attr_lake = attr_basic
+
+        if len(obs_attributes) > 0:
+            attr_obs = add_gauge_attributes(
+                grassdb=grassdb,
+                grass_location=grass_location,
+                qgis_prefix_path=qgis_prefix_path,
+                input_geo_names=input_geo_names,
+                obs_attributes=obs_attributes,
+                catinfo=attr_lake,
+            )
+        else:
+            attr_obs = attr_lake
+
+        if outlet_obs_id > 0:
+            attr_select = return_interest_catchments_info(
+                catinfo=attr_obs,
+                outlet_obs_id=outlet_obs_id,
+                path_sub_reg_outlets_v=path_sub_reg_outlets_v,
+            )
+        else:
+            attr_select = attr_obs
+
+        if path_landuse != "#":
+            attr_landuse = calculate_flood_plain_manning_n(
+                grassdb=grassdb,
+                grass_location=grass_location,
+                qgis_prefix_path=qgis_prefix_path,
+                catinfo=attr_select,
+                input_geo_names=input_geo_names,
+                path_landuse=path_landuse,
+                path_landuse_info=path_landuse_info,
+            )
+        else:
+            attr_landuse = attr_select
+
+        attr_da = streamorderanddrainagearea(attr_landuse)
+
+        if path_bkfwidthdepth != "#" or k_in != -1 or path_k_c_zone_polygon != '#':
+            attr_bkf = calculate_bankfull_width_depth_from_polyline(
+                grassdb=grassdb,
+                grass_location=grass_location,
+                qgis_prefix_path=qgis_prefix_path,
+                path_bkfwidthdepth=path_bkfwidthdepth,
+                path_k_c_zone_polygon = path_k_c_zone_polygon,
+                bkfwd_attributes=bkfwd_attributes,
+                catinfo=attr_da,
+                input_geo_names=input_geo_names,
+                k_in=k_in,
+                c_in=k_in,
+            )
+        else:
+            attr_bkf = attr_da
+
+        attr_ncl = update_non_connected_catchment_info(attr_bkf)
+        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'RivSlope'] = -1.2345
+        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'FloodP_n'] = -1.2345
+        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Max_DEM'] = -1.2345
+        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Min_DEM'] = -1.2345
+        attr_ncl.loc[attr_ncl['RivLength'] == -1.2345,'Ch_n'] = -1.2345
+
+        join_pandas_table_to_vector_attributes(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            qgis_prefix_path=qgis_prefix_path,
+            vector_name=cat_ply_info,
+            pd_table=attr_ncl,
+            column_types=coltypes,
+            columns_names=columns,
+        )
+
+        join_pandas_table_to_vector_attributes(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            qgis_prefix_path=qgis_prefix_path,
+            vector_name=cat_riv_info,
+            pd_table=attr_ncl,
+            column_types=coltypes,
+            columns_names=columns,
+        )
+
+        export_files_to_output_folder(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            qgis_prefix_path=qgis_prefix_path,
+            input_geo_names=input_geo_names,
+            output_riv=out_riv_name,
+            output_cat=out_cat_name,
+            output_folder=output_folder,
+            obs_attributes = obs_attributes,
+        )
+    elif gis_platform == "arcgis":
+        from basinmaker.addattributes.createattributestemplatearcgis import (
+            create_catchments_attributes_template_table,
+        )
+
+        create_catchments_attributes_template_table(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            columns=columns,
+            input_geo_names=input_geo_names,
+            obs_attributes=obs_attributes,
+            lake_attributes=lake_attributes,
+            path_landuse=path_landuse,
+            path_landuse_info=path_landuse_info,
+            path_k_c_zone_polygon = path_k_c_zone_polygon,
+            output_folder = output_folder,
+        )
```

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/addgaugeattributesqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/addgaugeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/addlakeattributesqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/addlakeattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/calbkfwidthdepthqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/calbkfwidthdepthqgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,17 @@
         da = catinfo.loc[idx_i, "DrainArea"] / 1000 / 1000  # m2 to km2
         catid = catinfo.loc[idx_i, "SubId"]
         if k > 0:
             q = func_Q_DA(da, k, c)
             catinfo.loc[idx_i, "BkfWidth"] =  max(7.2 * q ** 0.5,min_bkf_width)
             catinfo.loc[idx_i, "BkfDepth"] =  max(0.27 * q ** 0.3,min_bkf_depth)
             catinfo.loc[idx_i, "Q_Mean"] = q
+            catinfo.loc[idx_i, "k"] = k
+            catinfo.loc[idx_i, "c"] = c
+
         elif 'k_c_sub' in locals():
             if len(k_c_sub.loc[k_c_sub["b_Gridcode"] == catid]) < 1:
                 k_sub =  0.00450718
                 c_sub =  0.98579699
                 print("k_sub not found .....")
             else:
                 k_sub = k_c_sub.loc[k_c_sub["b_Gridcode"] == catid]["a_k"].values[0]
@@ -177,14 +180,16 @@
                     k_sub =  0.00450718
                     c_sub =  0.98579699
 
             q = func_Q_DA(da, k_sub, c_sub)
             catinfo.loc[idx_i, "BkfWidth"] =  max(7.2 * q ** 0.5,min_bkf_width)
             catinfo.loc[idx_i, "BkfDepth"] =  max(0.27 * q ** 0.3,min_bkf_depth)
             catinfo.loc[idx_i, "Q_Mean"] = q
+            catinfo.loc[idx_i, "k"] = k_sub
+            catinfo.loc[idx_i, "c"] = c_sub
 
         else:
             catinfo.loc[idx_i, "BkfWidth"] = default_bkf_width
             catinfo.loc[idx_i, "BkfDepth"] = default_bkf_depth
             catinfo.loc[idx_i, "Q_Mean"] = default_bkf_q
 
         if catinfo.loc[idx_i, "Lake_Cat"] < 2:
@@ -270,16 +275,16 @@
             n_rch = min(n_rch,max_manning_n)
 
             catinfo.loc[catinfo["SubId"] == subid, "RivSlope"] = slope_rch
             catinfo.loc[catinfo["SubId"] == subid, "Ch_n"] = n_rch
             catinfo.loc[catinfo["SubId"] == subid, "RivLength"] = length_rch
 
 
-            if subid == 504:
-                print(floodn_rch)
+            # if subid == 504:
+            #     print(floodn_rch)
 
 
             if floodn_rch < 0:
                 if floodn_Seg > 0:
                     floodn_rch = floodn_Seg
                 else:
                     floodn_rch = DEFALUT_FLOOD_N
```

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/calculatebasicattributesqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/calculatebasicattributesqgis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,538 +1,538 @@
-from basinmaker.func.grassgis import *
-from basinmaker.func.qgis import *
-from basinmaker.func.pdtable import *
-from basinmaker.func.rarray import *
-from basinmaker.utilities.utilities import *
-import sqlite3
-
-
-def calculate_basic_attributes(
-    grassdb,
-    grass_location,
-    qgis_prefix_path,
-    input_geo_names,
-    projection,
-    catinfo,
-    cat_ply_info,
-    cat_riv_info,
-    outlet_pt_info,
-):
-
-    catchments = input_geo_names["catchment_without_merging_lakes"]
-    river_r = input_geo_names["river_without_merging_lakes"]
-    river_v = input_geo_names["str_v"]
-    dem = input_geo_names["dem"]
-    fdr = input_geo_names["nfdr_grass"]
-    acc = input_geo_names["acc"]
-    cat_use_default_acc = input_geo_names["cat_use_default_acc"]
-    problem_seg = input_geo_names["problem_seg"]
-    nfdr_arcgis = input_geo_names["nfdr_arcgis"]
-
-    import grass.script as grass
-    import grass.script.setup as gsetup
-    from grass.pygrass.modules import Module
-    from grass.pygrass.modules.shortcuts import general as g
-    from grass.pygrass.modules.shortcuts import raster as r
-    from grass.script import array as garray
-    from grass.script import core as gcore
-    from grass_session import Session
-
-    QgsApplication.setPrefixPath(qgis_prefix_path, True)
-    Qgs = QgsApplication([], False)
-    Qgs.initQgis()
-    from processing.core.Processing import Processing
-    from processing.tools import dataobjects
-    from qgis import processing
-
-    feedback = QgsProcessingFeedback()
-    Processing.initialize()
-    QgsApplication.processingRegistry().addProvider(QgsNativeAlgorithms())
-    context = dataobjects.createContext()
-    context.setInvalidGeometryCheck(QgsFeatureRequest.GeometryNoCheck)
-
-    os.environ.update(
-        dict(GRASS_COMPRESS_NULLS="1", GRASS_COMPRESSOR="ZSTD", GRASS_VERBOSE="1")
-    )
-    PERMANENT = Session()
-    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
-
-    con = sqlite3.connect(
-        os.path.join(grassdb, grass_location, "PERMANENT", "sqlite", "sqlite.db")
-    )
-
-    # create a catchment vector and overlay with str v
-    exp = "%s = int(%s)" % (catchments, catchments)
-    grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-
-    grass.run_command(
-        "r.to.vect",
-        input=catchments,
-        output=cat_ply_info + "t1",
-        type="area",
-        overwrite=True,
-    )
-    grass.run_command(
-        "v.db.addcolumn", map=cat_ply_info + "t1", columns="GC_str VARCHAR(40)"
-    )
-    grass.run_command(
-        "v.db.addcolumn", map=cat_ply_info + "t1", columns="Area_m double"
-    )
-    grass.run_command(
-        "v.db.update", map=cat_ply_info + "t1", column="GC_str", qcol="value"
-    )
-    # dissolve based on gridcode
-    grass.run_command(
-        "v.dissolve",
-        input=cat_ply_info + "t1",
-        column="GC_str",
-        output=cat_ply_info,
-        overwrite=True,
-    )
-
-    grass.run_command("v.db.addcolumn", map=cat_ply_info, columns="Gridcode INT")
-    grass.run_command("v.db.update", map=cat_ply_info, column="Gridcode", qcol="GC_str")
-
-    ## obtain a stream vector, segmentation based on new catchment polygon
-    grass.run_command(
-        "v.overlay",
-        ainput=river_v,
-        alayer=2,
-        atype="line",
-        binput=cat_ply_info,
-        operator="and",
-        output=cat_riv_info + "t1",
-        overwrite=True,
-    )
-    grass.run_command(
-        "v.out.ogr",
-        input=cat_riv_info + "t1",
-        output=os.path.join(grassdb, cat_riv_info + "t1" + ".shp"),
-        format="ESRI_Shapefile",
-        overwrite=True,
-    )
-    processing.run(
-        "gdal:dissolve",
-        {
-            "INPUT": os.path.join(grassdb, cat_riv_info + "t1" + ".shp"),
-            "FIELD": "b_GC_str",
-            "OUTPUT": os.path.join(grassdb, cat_riv_info + ".shp"),
-        },
-    )
-    grass.run_command(
-        "v.import",
-        input=os.path.join(grassdb, cat_riv_info + ".shp"),
-        output=cat_riv_info,
-        overwrite=True,
-    )
-
-    grass.run_command("v.db.addcolumn", map=cat_riv_info, columns="Gridcode INT")
-    grass.run_command("v.db.addcolumn", map=cat_riv_info, columns="Length_m double")
-    grass.run_command(
-        "v.db.update", map=cat_riv_info, column="Gridcode", qcol="b_GC_str"
-    )
-    grass.run_command("v.db.dropcolumn", map=cat_riv_info, columns=["b_GC_str"])
-
-    grass.run_command(
-        "r.out.gdal",
-        input=dem,
-        output=os.path.join(grassdb, "dem_par.tif"),
-        format="GTiff",
-        overwrite=True,
-    )
-
-    PERMANENT.close()
-
-    os.system(
-        "gdalwarp "
-        + '"'
-        + os.path.join(grassdb, "dem_par.tif")
-        + '"'
-        + "    "
-        + '"'
-        + os.path.join(grassdb, "dem_proj.tif")
-        + '"'
-        + " -t_srs  "
-        + '"'
-        + projection
-        + '"'
-    )
-
-    project = Session()
-    project.open(
-        gisdb=grassdb, location=grass_location + "_proj", create_opts=projection
-    )
-
-    grass.run_command(
-        "r.import",
-        input=os.path.join(grassdb, "dem_proj.tif"),
-        output="dem_proj",
-        overwrite=True,
-    )
-    grass.run_command("g.region", raster="dem_proj")
-    grass.run_command(
-        "v.proj",
-        location=grass_location,
-        mapset="PERMANENT",
-        input=cat_riv_info,
-        overwrite=True,
-    )
-    grass.run_command(
-        "v.proj",
-        location=grass_location,
-        mapset="PERMANENT",
-        input=cat_ply_info,
-        overwrite=True,
-    )
-
-    grass.run_command(
-        "v.to.db",
-        map=cat_ply_info,
-        option="area",
-        columns="Area_m",
-        units="meters",
-        overwrite=True,
-    )
-    grass.run_command(
-        "v.to.db",
-        map=cat_riv_info,
-        option="length",
-        columns="Length_m",
-        units="meters",
-        overwrite=True,
-    )
-
-    grass.run_command(
-        "r.slope.aspect",
-        elevation="dem_proj",
-        slope="slope",
-        aspect="aspect",
-        precision="DCELL",
-        overwrite=True,
-    )
-
-    ### calcuate averaged slope and aspect of each subbasin
-    grass.run_command(
-        "v.rast.stats",
-        map=cat_ply_info,
-        raster="slope",
-        column_prefix="s",
-        method="average",
-    )
-    grass.run_command(
-        "v.rast.stats",
-        map=cat_ply_info,
-        raster="aspect",
-        column_prefix="a",
-        method="average",
-    )
-    
-    grass.run_command(
-        "v.rast.stats",
-        map=cat_ply_info,
-        raster="dem_proj",
-        column_prefix="d",
-        method="average",
-    )
-    
-    ### calcuate minimum and maximum dem along the channel
-    grass.run_command(
-        "v.rast.stats",
-        map=cat_riv_info,
-        raster="dem_proj",
-        column_prefix="d",
-        method=["minimum", "maximum"],
-    )
-
-    project.close()
-
-    PERMANENT = Session()
-    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
-    grass.run_command("g.region", raster="dem")
-    grass.run_command(
-        "v.proj",
-        location=grass_location + "_proj",
-        mapset="PERMANENT",
-        input=cat_riv_info,
-        overwrite=True,
-    )        
-    grass.run_command(
-        "v.proj",
-        location=grass_location + "_proj",
-        mapset="PERMANENT",
-        input=cat_ply_info,
-        overwrite=True,
-    )
-    
-    ### calcuate averaged DEM in each subbasin
-    # grass.run_command(
-    #     "v.rast.stats",
-    #     map=cat_ply_info,
-    #     raster="dem",
-    #     column_prefix="d",
-    #     method="average",
-    # )
-    # 
-    # ### calcuate minimum and maximum dem along the channel
-    # grass.run_command(
-    #     "v.rast.stats",
-    #     map=cat_riv_info,
-    #     raster="dem",
-    #     column_prefix="d",
-    #     method=["minimum", "maximum"],
-    # )
-    
-    ## get routing structure
-
-    exp = "%s = int(%s)" % (fdr, fdr)
-    grass.run_command(
-        "r.mapcalc",
-        expression=exp,
-        overwrite=True,
-    )
-
-    grass.run_command(
-        "r.accumulate",
-        direction=fdr,
-        accumulation="acc_grass_CatOL",
-        overwrite=True,
-    )
-
-    ##### obtain catment id overlaied with problem seg
-    prom_seg_id, cat_pro_id = generate_stats_list_from_grass_raster(
-        grass, mode=2, input_a=problem_seg, input_b=catchments
-    )
-    cat_pro_id = np.unique(cat_pro_id)
-    grass.run_command("g.copy", rast=(catchments, cat_use_default_acc), overwrite=True)
-    if len(cat_pro_id) > 0:
-        grass.run_command(
-            "r.null", map=cat_use_default_acc, setnull=cat_pro_id, overwrite=True
-        )
-    else:
-        cat_pro_id = []
-
-    exp = "acc_grass_CatOL2 = if(isnull(%s),%s,%s)" % (
-        cat_use_default_acc,
-        "acc_grass_CatOL",
-        acc,
-    )
-    grass.run_command(
-        "r.mapcalc",
-        expression=exp,
-        overwrite=True,
-    )
-
-    routing_temp = generate_routing_info_of_catchments(
-        grass,
-        con,
-        cat=catchments,
-        acc="acc_grass_CatOL2",
-        Name="Final",
-        str=river_r,
-        garray = garray,
-    )
-
-    routing_temp = generate_routing_info_of_catchments(
-        grass,
-        con,
-        cat=river_r,
-        acc="acc_grass_CatOL2",
-        Name="Friv",
-        str=river_r,
-        garray = garray,
-    )
-
-    cat_array = garray.array(mapname=catchments)
-    nfdr_arcgis_array = garray.array(mapname=nfdr_arcgis)
-    cat_outlet_array = garray.array(mapname="Final_OL")
-    ncols = int(cat_array.shape[1])
-    nrows = int(cat_array.shape[0])
-
-    grass.run_command("g.copy", vector=("Final_OL_v", outlet_pt_info), overwrite=True)
-    PERMANENT.close()
-    
-    
-    ## add coordinates to outlet point in wgs84 system
-    project_wgs84 = Session()
-    project_wgs84.open(
-        gisdb=grassdb, location=grass_location + "_wgs84", create_opts='EPSG:4326'
-    )
-    grass.run_command(
-        "v.proj",
-        location=grass_location,
-        mapset="PERMANENT",
-        input=outlet_pt_info,
-        overwrite=True,
-    )
-    grass.run_command(
-        "v.to.db",
-        map = outlet_pt_info,
-        type = 'point',
-        option = 'coor',
-        columns = ['outletLng','outletLat'],
-        overwrite=True,
-    )  
-    project_wgs84.close()
-
-    ## import updated outlet points after add coordinates in wgs84 system
-    PERMANENT = Session()
-    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
-    grass.run_command("g.region", raster="dem")
-    grass.run_command(
-        "v.proj",
-        location=grass_location + "_wgs84",
-        mapset="PERMANENT",
-        input=outlet_pt_info,
-        overwrite=True,
-    )   
- 
-    ### update dataframe
-    ###
-    sqlstat = "SELECT Gridcode, Length_m, d_minimum, d_maximum FROM %s" % (cat_riv_info)
-    leninfo = pd.read_sql_query(sqlstat, con)
-    ### read catchment
-    sqlstat = "SELECT Gridcode, Area_m,d_average,s_average,a_average FROM %s" % (
-        cat_ply_info
-    )
-    areainfo = pd.read_sql_query(sqlstat, con)
-
-    ### read catchment
-    sqlstat = "SELECT SubId, DowSubId,ILSubIdmax,ILSubIdmin,outletLat, outletLng FROM %s" % (outlet_pt_info)
-    outletinfo = pd.read_sql_query(sqlstat, con)
-    outletinfo = outletinfo.fillna(-9999)
-    outletinfo = outletinfo.loc[outletinfo['SubId'] >= 0]
-    ### read catchment
-    sqlstat = "SELECT SubId, DSubId_str FROM %s" % ('Friv_OL_v')
-    outlet_riv_info = pd.read_sql_query(sqlstat, con)
-    outlet_riv_info = outlet_riv_info.fillna(-9999)
-
-
-    leninfo = leninfo.astype(float).fillna(-9999)
-    areainfo = areainfo.astype(float).fillna(-9999)
-
-    for i in range(0, len(outletinfo)):
-        catid = outletinfo["SubId"].values[i]
-        DownSubID_cat = outletinfo["DowSubId"].values[i]
-        outlet_lat = outletinfo["outletLat"].values[i]
-        outlet_lon = outletinfo["outletLng"].values[i]
-        
-        catinfo.loc[i, "SubId"] = catid
-        catinfo.loc[i, "outletLat"] = outlet_lat
-        catinfo.loc[i, "outletLng"] = outlet_lon
-
-        # load routing info based on str
-        outlet_riv_info_i = outlet_riv_info.loc[outlet_riv_info['SubId'] == catid]
-
-        # check if riv outlet exist
-        if len(outlet_riv_info_i) < 1:
-            DownSubID = DownSubID_cat
-            DownSubID_riv = -9999
-        else:
-           # get down sub id based in river network
-           DownSubID_riv = outlet_riv_info_i['DSubId_str'].values[0]
-
-           # may need to modify if downsub id from river != down subid from cat
-           if DownSubID_riv != DownSubID_cat:
-
-               # check if DownSubID_cat drainage to DSubId_str
-               Down_id_of_downriv_info = outletinfo.loc[outletinfo['SubId'] == DownSubID_riv]
-               if len(Down_id_of_downriv_info) > 0:
-                   # get down subid of down subid of river
-                   DSubId_DSubId_str = Down_id_of_downriv_info['DowSubId'].values[0]
-                   # if down subid of down sub id of river  = down sub id from cat
-                   if catid == 10762:
-                       print(DSubId_DSubId_str,DownSubID_cat)
-
-                   if DSubId_DSubId_str == DownSubID_cat:
-                       DownSubID = DownSubID_riv
-                   else:
-                       DownSubID = DownSubID_cat
-               else:
-                   DownSubID = DownSubID_cat
-           else:
-               DownSubID = DownSubID_cat
-
-        if catid in cat_pro_id or DownSubID == catid or DownSubID == -9999:
-            downsubid_array = return_subid_of_next_down_stream_grids(
-                cat_array, catid, nfdr_arcgis_array, cat_outlet_array, ncols, nrows
-            )
-            #            print(catid,DownSubID,downsubid_array)
-            if downsubid_array > 0:
-                DownSubID = downsubid_array
-
-        ### change the downsub id to -1 for watershed outlet
-        if len(outletinfo.loc[outletinfo["SubId"] == DownSubID]) < 1:
-            catinfo.loc[i, "DowSubId"] = -1
-        elif catid == DownSubID:
-            catinfo.loc[i, "DowSubId"] = -1
-        else:
-            catinfo.loc[i, "DowSubId"] = DownSubID
-
-        catarea = np.unique(
-            areainfo.loc[areainfo["Gridcode"] == catid]["Area_m"].values
-        )  #'Area_m'
-        catslope = np.unique(
-            areainfo.loc[areainfo["Gridcode"] == catid]["s_average"].values
-        )
-        catelev = np.unique(
-            areainfo.loc[areainfo["Gridcode"] == catid]["d_average"].values
-        )
-        cataspect = np.unique(
-            areainfo.loc[areainfo["Gridcode"] == catid]["a_average"].values
-        )
-        if len(catarea) == 1:
-            catinfo.loc[i, "BasArea"] = catarea
-            catinfo.loc[i, "BasSlope"] = catslope
-            catinfo.loc[i, "BasAspect"] = cataspect
-            catinfo.loc[i, "MeanElev"] = catelev
-        else:
-            print(
-                "Warning  basin area of stream  ",
-                catid,
-                "   need check   ",
-                len(catarea),
-            )
-            catinfo.loc[i, "BasArea"] = -9999
-            catinfo.loc[i, "BasSlope"] = -9999
-            catinfo.loc[i, "BasAspect"] = -9999
-            catinfo.loc[i, "MeanElev"] = -9999
-
-        ### add river parameters
-        rivlen = np.unique(
-            leninfo.loc[leninfo["Gridcode"] == catid]["Length_m"].values
-        )  #'Area_m'
-        dmaxelev = np.unique(
-            leninfo.loc[leninfo["Gridcode"] == catid]["d_maximum"].values
-        )
-        dminelev = np.unique(
-            leninfo.loc[leninfo["Gridcode"] == catid]["d_minimum"].values
-        )
-        if len(rivlen) > 0:
-            catinfo.loc[i, "RivLength"] = rivlen[0]
-            maxdem = dmaxelev[0]
-            mindem = dminelev[0]
-            catinfo.loc[i, "Min_DEM"] = mindem
-            catinfo.loc[i, "Max_DEM"] = maxdem
-            if rivlen[0] >= 0:
-                if max(0, float((maxdem - mindem)) / float(rivlen[0])) == 0:
-                    slope_rch = -9999
-                else:
-                    slope_rch = max(
-                        0, float((maxdem - mindem)) / float(rivlen[0])
-                    )
-
-                slope_rch = max(slope_rch,min_riv_slope)  
-                slope_rch = min(slope_rch,max_riv_slope)
-                  
-                catinfo.loc[i, "RivSlope"] = slope_rch
-                
-            else:
-                catinfo.loc[i, "RivSlope"] = -9999
-        else:
-            catinfo.loc[i, "RivLength"] = -9999
-            catinfo.loc[i, "RivSlope"] = -9999
-            catinfo.loc[i, "FloodP_n"] = -9999
-            catinfo.loc[i, "Min_DEM"] = -9999
-            catinfo.loc[i, "Max_DEM"] = -9999
-
-    PERMANENT.close()
-    return catinfo
+from basinmaker.func.grassgis import *
+from basinmaker.func.qgis import *
+from basinmaker.func.pdtable import *
+from basinmaker.func.rarray import *
+from basinmaker.utilities.utilities import *
+import sqlite3
+
+
+def calculate_basic_attributes(
+    grassdb,
+    grass_location,
+    qgis_prefix_path,
+    input_geo_names,
+    projection,
+    catinfo,
+    cat_ply_info,
+    cat_riv_info,
+    outlet_pt_info,
+):
+
+    catchments = input_geo_names["catchment_without_merging_lakes"]
+    river_r = input_geo_names["river_without_merging_lakes"]
+    river_v = input_geo_names["str_v"]
+    dem = input_geo_names["dem"]
+    fdr = input_geo_names["nfdr_grass"]
+    acc = input_geo_names["acc"]
+    cat_use_default_acc = input_geo_names["cat_use_default_acc"]
+    problem_seg = input_geo_names["problem_seg"]
+    nfdr_arcgis = input_geo_names["nfdr_arcgis"]
+
+    import grass.script as grass
+    import grass.script.setup as gsetup
+    from grass.pygrass.modules import Module
+    from grass.pygrass.modules.shortcuts import general as g
+    from grass.pygrass.modules.shortcuts import raster as r
+    from grass.script import array as garray
+    from grass.script import core as gcore
+    from grass_session import Session
+
+    QgsApplication.setPrefixPath(qgis_prefix_path, True)
+    Qgs = QgsApplication([], False)
+    Qgs.initQgis()
+    from processing.core.Processing import Processing
+    from processing.tools import dataobjects
+    from qgis import processing
+
+    feedback = QgsProcessingFeedback()
+    Processing.initialize()
+    QgsApplication.processingRegistry().addProvider(QgsNativeAlgorithms())
+    context = dataobjects.createContext()
+    context.setInvalidGeometryCheck(QgsFeatureRequest.GeometryNoCheck)
+
+    os.environ.update(
+        dict(GRASS_COMPRESS_NULLS="1", GRASS_COMPRESSOR="ZSTD", GRASS_VERBOSE="1")
+    )
+    PERMANENT = Session()
+    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
+
+    con = sqlite3.connect(
+        os.path.join(grassdb, grass_location, "PERMANENT", "sqlite", "sqlite.db")
+    )
+
+    # create a catchment vector and overlay with str v
+    exp = "%s = int(%s)" % (catchments, catchments)
+    grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+    grass.run_command(
+        "r.to.vect",
+        input=catchments,
+        output=cat_ply_info + "t1",
+        type="area",
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.db.addcolumn", map=cat_ply_info + "t1", columns="GC_str VARCHAR(40)"
+    )
+    grass.run_command(
+        "v.db.addcolumn", map=cat_ply_info + "t1", columns="Area_m double"
+    )
+    grass.run_command(
+        "v.db.update", map=cat_ply_info + "t1", column="GC_str", qcol="value"
+    )
+    # dissolve based on gridcode
+    grass.run_command(
+        "v.dissolve",
+        input=cat_ply_info + "t1",
+        column="GC_str",
+        output=cat_ply_info,
+        overwrite=True,
+    )
+
+    grass.run_command("v.db.addcolumn", map=cat_ply_info, columns="Gridcode INT")
+    grass.run_command("v.db.update", map=cat_ply_info, column="Gridcode", qcol="GC_str")
+
+    ## obtain a stream vector, segmentation based on new catchment polygon
+    grass.run_command(
+        "v.overlay",
+        ainput=river_v,
+        alayer=2,
+        atype="line",
+        binput=cat_ply_info,
+        operator="and",
+        output=cat_riv_info + "t1",
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.out.ogr",
+        input=cat_riv_info + "t1",
+        output=os.path.join(grassdb, cat_riv_info + "t1" + ".shp"),
+        format="ESRI_Shapefile",
+        overwrite=True,
+    )
+    processing.run(
+        "gdal:dissolve",
+        {
+            "INPUT": os.path.join(grassdb, cat_riv_info + "t1" + ".shp"),
+            "FIELD": "b_GC_str",
+            "OUTPUT": os.path.join(grassdb, cat_riv_info + ".shp"),
+        },
+    )
+    grass.run_command(
+        "v.import",
+        input=os.path.join(grassdb, cat_riv_info + ".shp"),
+        output=cat_riv_info,
+        overwrite=True,
+    )
+
+    grass.run_command("v.db.addcolumn", map=cat_riv_info, columns="Gridcode INT")
+    grass.run_command("v.db.addcolumn", map=cat_riv_info, columns="Length_m double")
+    grass.run_command(
+        "v.db.update", map=cat_riv_info, column="Gridcode", qcol="b_GC_str"
+    )
+    grass.run_command("v.db.dropcolumn", map=cat_riv_info, columns=["b_GC_str"])
+
+    grass.run_command(
+        "r.out.gdal",
+        input=dem,
+        output=os.path.join(grassdb, "dem_par.tif"),
+        format="GTiff",
+        overwrite=True,
+    )
+
+    PERMANENT.close()
+
+    os.system(
+        "gdalwarp "
+        + '"'
+        + os.path.join(grassdb, "dem_par.tif")
+        + '"'
+        + "    "
+        + '"'
+        + os.path.join(grassdb, "dem_proj.tif")
+        + '"'
+        + " -t_srs  "
+        + '"'
+        + projection
+        + '"'
+    )
+
+    project = Session()
+    project.open(
+        gisdb=grassdb, location=grass_location + "_proj", create_opts=projection
+    )
+
+    grass.run_command(
+        "r.import",
+        input=os.path.join(grassdb, "dem_proj.tif"),
+        output="dem_proj",
+        overwrite=True,
+    )
+    grass.run_command("g.region", raster="dem_proj")
+    grass.run_command(
+        "v.proj",
+        location=grass_location,
+        mapset="PERMANENT",
+        input=cat_riv_info,
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.proj",
+        location=grass_location,
+        mapset="PERMANENT",
+        input=cat_ply_info,
+        overwrite=True,
+    )
+
+    grass.run_command(
+        "v.to.db",
+        map=cat_ply_info,
+        option="area",
+        columns="Area_m",
+        units="meters",
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.to.db",
+        map=cat_riv_info,
+        option="length",
+        columns="Length_m",
+        units="meters",
+        overwrite=True,
+    )
+
+    grass.run_command(
+        "r.slope.aspect",
+        elevation="dem_proj",
+        slope="slope",
+        aspect="aspect",
+        precision="DCELL",
+        overwrite=True,
+    )
+
+    ### calcuate averaged slope and aspect of each subbasin
+    grass.run_command(
+        "v.rast.stats",
+        map=cat_ply_info,
+        raster="slope",
+        column_prefix="s",
+        method="average",
+    )
+    grass.run_command(
+        "v.rast.stats",
+        map=cat_ply_info,
+        raster="aspect",
+        column_prefix="a",
+        method="average",
+    )
+
+    grass.run_command(
+        "v.rast.stats",
+        map=cat_ply_info,
+        raster="dem_proj",
+        column_prefix="d",
+        method="average",
+    )
+
+    ### calcuate minimum and maximum dem along the channel
+    grass.run_command(
+        "v.rast.stats",
+        map=cat_riv_info,
+        raster="dem_proj",
+        column_prefix="d",
+        method=["minimum", "maximum"],
+    )
+
+    project.close()
+
+    PERMANENT = Session()
+    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
+    grass.run_command("g.region", raster="dem")
+    grass.run_command(
+        "v.proj",
+        location=grass_location + "_proj",
+        mapset="PERMANENT",
+        input=cat_riv_info,
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.proj",
+        location=grass_location + "_proj",
+        mapset="PERMANENT",
+        input=cat_ply_info,
+        overwrite=True,
+    )
+
+    ### calcuate averaged DEM in each subbasin
+    # grass.run_command(
+    #     "v.rast.stats",
+    #     map=cat_ply_info,
+    #     raster="dem",
+    #     column_prefix="d",
+    #     method="average",
+    # )
+    #
+    # ### calcuate minimum and maximum dem along the channel
+    # grass.run_command(
+    #     "v.rast.stats",
+    #     map=cat_riv_info,
+    #     raster="dem",
+    #     column_prefix="d",
+    #     method=["minimum", "maximum"],
+    # )
+
+    ## get routing structure
+
+    exp = "%s = int(%s)" % (fdr, fdr)
+    grass.run_command(
+        "r.mapcalc",
+        expression=exp,
+        overwrite=True,
+    )
+
+    grass.run_command(
+        "r.accumulate",
+        direction=fdr,
+        accumulation="acc_grass_CatOL",
+        overwrite=True,
+    )
+
+    ##### obtain catment id overlaied with problem seg
+    prom_seg_id, cat_pro_id = generate_stats_list_from_grass_raster(
+        grass, mode=2, input_a=problem_seg, input_b=catchments
+    )
+    cat_pro_id = np.unique(cat_pro_id)
+    grass.run_command("g.copy", rast=(catchments, cat_use_default_acc), overwrite=True)
+    if len(cat_pro_id) > 0:
+        grass.run_command(
+            "r.null", map=cat_use_default_acc, setnull=cat_pro_id, overwrite=True
+        )
+    else:
+        cat_pro_id = []
+
+    exp = "acc_grass_CatOL2 = if(isnull(%s),%s,%s)" % (
+        cat_use_default_acc,
+        "acc_grass_CatOL",
+        acc,
+    )
+    grass.run_command(
+        "r.mapcalc",
+        expression=exp,
+        overwrite=True,
+    )
+
+    routing_temp = generate_routing_info_of_catchments(
+        grass,
+        con,
+        cat=catchments,
+        acc="acc_grass_CatOL2",
+        Name="Final",
+        str=river_r,
+        garray = garray,
+    )
+
+    routing_temp = generate_routing_info_of_catchments(
+        grass,
+        con,
+        cat=river_r,
+        acc="acc_grass_CatOL2",
+        Name="Friv",
+        str=river_r,
+        garray = garray,
+    )
+
+    cat_array = garray.array(mapname=catchments)
+    nfdr_arcgis_array = garray.array(mapname=nfdr_arcgis)
+    cat_outlet_array = garray.array(mapname="Final_OL")
+    ncols = int(cat_array.shape[1])
+    nrows = int(cat_array.shape[0])
+
+    grass.run_command("g.copy", vector=("Final_OL_v", outlet_pt_info), overwrite=True)
+    PERMANENT.close()
+
+
+    ## add coordinates to outlet point in wgs84 system
+    project_wgs84 = Session()
+    project_wgs84.open(
+        gisdb=grassdb, location=grass_location + "_wgs84", create_opts='EPSG:4326'
+    )
+    grass.run_command(
+        "v.proj",
+        location=grass_location,
+        mapset="PERMANENT",
+        input=outlet_pt_info,
+        overwrite=True,
+    )
+    grass.run_command(
+        "v.to.db",
+        map = outlet_pt_info,
+        type = 'point',
+        option = 'coor',
+        columns = ['outletLng','outletLat'],
+        overwrite=True,
+    )
+    project_wgs84.close()
+
+    ## import updated outlet points after add coordinates in wgs84 system
+    PERMANENT = Session()
+    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
+    grass.run_command("g.region", raster="dem")
+    grass.run_command(
+        "v.proj",
+        location=grass_location + "_wgs84",
+        mapset="PERMANENT",
+        input=outlet_pt_info,
+        overwrite=True,
+    )
+
+    ### update dataframe
+    ###
+    sqlstat = "SELECT Gridcode, Length_m, d_minimum, d_maximum FROM %s" % (cat_riv_info)
+    leninfo = pd.read_sql_query(sqlstat, con)
+    ### read catchment
+    sqlstat = "SELECT Gridcode, Area_m,d_average,s_average,a_average FROM %s" % (
+        cat_ply_info
+    )
+    areainfo = pd.read_sql_query(sqlstat, con)
+
+    ### read catchment
+    sqlstat = "SELECT SubId, DowSubId,ILSubIdmax,ILSubIdmin,outletLat, outletLng FROM %s" % (outlet_pt_info)
+    outletinfo = pd.read_sql_query(sqlstat, con)
+    outletinfo = outletinfo.fillna(-9999)
+    outletinfo = outletinfo.loc[outletinfo['SubId'] >= 0]
+    ### read catchment
+    sqlstat = "SELECT SubId, DSubId_str FROM %s" % ('Friv_OL_v')
+    outlet_riv_info = pd.read_sql_query(sqlstat, con)
+    outlet_riv_info = outlet_riv_info.fillna(-9999)
+
+
+    leninfo = leninfo.astype(float).fillna(-9999)
+    areainfo = areainfo.astype(float).fillna(-9999)
+
+    for i in range(0, len(outletinfo)):
+        catid = outletinfo["SubId"].values[i]
+        DownSubID_cat = outletinfo["DowSubId"].values[i]
+        outlet_lat = outletinfo["outletLat"].values[i]
+        outlet_lon = outletinfo["outletLng"].values[i]
+
+        catinfo.loc[i, "SubId"] = catid
+        catinfo.loc[i, "outletLat"] = outlet_lat
+        catinfo.loc[i, "outletLng"] = outlet_lon
+
+        # load routing info based on str
+        outlet_riv_info_i = outlet_riv_info.loc[outlet_riv_info['SubId'] == catid]
+
+        # check if riv outlet exist
+        if len(outlet_riv_info_i) < 1:
+            DownSubID = DownSubID_cat
+            DownSubID_riv = -9999
+        else:
+           # get down sub id based in river network
+           DownSubID_riv = outlet_riv_info_i['DSubId_str'].values[0]
+
+           # may need to modify if downsub id from river != down subid from cat
+           if DownSubID_riv != DownSubID_cat:
+
+               # check if DownSubID_cat drainage to DSubId_str
+               Down_id_of_downriv_info = outletinfo.loc[outletinfo['SubId'] == DownSubID_riv]
+               if len(Down_id_of_downriv_info) > 0:
+                   # get down subid of down subid of river
+                   DSubId_DSubId_str = Down_id_of_downriv_info['DowSubId'].values[0]
+                   # if down subid of down sub id of river  = down sub id from cat
+                   # if catid == 10762:
+                   #     print(DSubId_DSubId_str,DownSubID_cat)
+
+                   if DSubId_DSubId_str == DownSubID_cat:
+                       DownSubID = DownSubID_riv
+                   else:
+                       DownSubID = DownSubID_cat
+               else:
+                   DownSubID = DownSubID_cat
+           else:
+               DownSubID = DownSubID_cat
+
+        if catid in cat_pro_id or DownSubID == catid or DownSubID == -9999:
+            downsubid_array = return_subid_of_next_down_stream_grids(
+                cat_array, catid, nfdr_arcgis_array, cat_outlet_array, ncols, nrows
+            )
+            #            print(catid,DownSubID,downsubid_array)
+            if downsubid_array > 0:
+                DownSubID = downsubid_array
+
+        ### change the downsub id to -1 for watershed outlet
+        if len(outletinfo.loc[outletinfo["SubId"] == DownSubID]) < 1:
+            catinfo.loc[i, "DowSubId"] = -1
+        elif catid == DownSubID:
+            catinfo.loc[i, "DowSubId"] = -1
+        else:
+            catinfo.loc[i, "DowSubId"] = DownSubID
+
+        catarea = np.unique(
+            areainfo.loc[areainfo["Gridcode"] == catid]["Area_m"].values
+        )  #'Area_m'
+        catslope = np.unique(
+            areainfo.loc[areainfo["Gridcode"] == catid]["s_average"].values
+        )
+        catelev = np.unique(
+            areainfo.loc[areainfo["Gridcode"] == catid]["d_average"].values
+        )
+        cataspect = np.unique(
+            areainfo.loc[areainfo["Gridcode"] == catid]["a_average"].values
+        )
+        if len(catarea) == 1:
+            catinfo.loc[i, "BasArea"] = catarea
+            catinfo.loc[i, "BasSlope"] = catslope
+            catinfo.loc[i, "BasAspect"] = cataspect
+            catinfo.loc[i, "MeanElev"] = catelev
+        else:
+            print(
+                "Warning  basin area of stream  ",
+                catid,
+                "   need check   ",
+                len(catarea),
+            )
+            catinfo.loc[i, "BasArea"] = -9999
+            catinfo.loc[i, "BasSlope"] = -9999
+            catinfo.loc[i, "BasAspect"] = -9999
+            catinfo.loc[i, "MeanElev"] = -9999
+
+        ### add river parameters
+        rivlen = np.unique(
+            leninfo.loc[leninfo["Gridcode"] == catid]["Length_m"].values
+        )  #'Area_m'
+        dmaxelev = np.unique(
+            leninfo.loc[leninfo["Gridcode"] == catid]["d_maximum"].values
+        )
+        dminelev = np.unique(
+            leninfo.loc[leninfo["Gridcode"] == catid]["d_minimum"].values
+        )
+        if len(rivlen) > 0:
+            catinfo.loc[i, "RivLength"] = rivlen[0]
+            maxdem = dmaxelev[0]
+            mindem = dminelev[0]
+            catinfo.loc[i, "Min_DEM"] = mindem
+            catinfo.loc[i, "Max_DEM"] = maxdem
+            if rivlen[0] >= 0:
+                if max(0, float((maxdem - mindem)) / float(rivlen[0])) == 0:
+                    slope_rch = -9999
+                else:
+                    slope_rch = max(
+                        0, float((maxdem - mindem)) / float(rivlen[0])
+                    )
+
+                slope_rch = max(slope_rch,min_riv_slope)
+                slope_rch = min(slope_rch,max_riv_slope)
+
+                catinfo.loc[i, "RivSlope"] = slope_rch
+
+            else:
+                catinfo.loc[i, "RivSlope"] = -9999
+        else:
+            catinfo.loc[i, "RivLength"] = -9999
+            catinfo.loc[i, "RivSlope"] = -9999
+            catinfo.loc[i, "FloodP_n"] = -9999
+            catinfo.loc[i, "Min_DEM"] = -9999
+            catinfo.loc[i, "Max_DEM"] = -9999
+
+    PERMANENT.close()
+    return catinfo
```

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/calfloodmanningnqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/calfloodmanningnqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/createattributestemplateqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/createattributestemplateqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/exportoutputsqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/exportoutputsqgis.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         processing=processing,
         context=context,
         FORMULA=formular,
         FIELD_NAME="centroid_x",
         INPUT=layer_cat,
         OUTPUT="memory:",
     )["OUTPUT"]
-        
+
 
     formular = "y(centroid(transform($geometry,'%s','%s')))" % (
         layer_cat.crs().authid(),
         "EPSG:4326",
     )
 
     layer_cat = qgis_vector_field_calculator(
@@ -108,26 +108,26 @@
     Selectfeatureattributes(
         processing,
         Input=os.path.join(grassdb, cat_riv_info + "_dis.shp"),
         Output=os.path.join(grassdb, output_riv + "withnegv.shp"),
         Attri_NM="SubId",
         Values=subinfo[subinfo["SubId"] > 0]["SubId"].values,
     )
-    
+
     change_neg_value_to_null_in_attribute_table(
                  processing,
                  os.path.join(grassdb, output_cat + "withnegv.shp"),
                  os.path.join(output_folder, output_cat + ".shp")
     )
     change_neg_value_to_null_in_attribute_table(
                  processing,
                  os.path.join(grassdb, output_riv + "withnegv.shp"),
                  os.path.join(output_folder, output_riv + ".shp")
     )
-    
+
     # Add_centroid_to_feature(
     #     os.path.join(output_folder, output_cat + ".shp"), "centroid_x", "centroid_y"
     # )
 
     subinfo = Dbf_To_Dataframe(os.path.join(output_folder, output_cat + ".shp"))
 
     if os.path.exists(os.path.join(grassdb, all_lakes + ".shp")):
@@ -155,15 +155,15 @@
         os.path.exists(os.path.join(grassdb, snapped_obs_points + ".shp"))
         and len(subinfo.loc[subinfo["Has_POI"] > 0]["Has_POI"].values) > 0
     ):
 
         Selectfeatureattributes(
             processing,
             Input=os.path.join(grassdb, snapped_obs_points + ".shp"),
-            Output=os.path.join(output_folder, "obs_gauges.shp"),
+            Output=os.path.join(output_folder, "poi.shp"),
             Attri_NM=obs_attributes[1],
             Values=subinfo.loc[subinfo["Has_POI"] > 0]["Obs_NM"].values,
             Is_str = True,
         )
 
     Clean_Attribute_Name(
         os.path.join(output_folder, output_cat + ".shp"), COLUMN_NAMES_CONSTANT_CLEAN
```

### Comparing `basinmaker-3.0.1/basinmaker/addattributes/joinpandastoattributesqgis.py` & `basinmaker-3.0.3/basinmaker/addattributes/joinpandastoattributesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/addlakeandobsintowatershed.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/addlakeandobsintowatershed.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,235 +1,242 @@
-from basinmaker.utilities.utilities import Internal_Constant_Names
-
-
-def add_lakes_and_obs_into_existing_watershed_delineation(
-    input_geo_names,
-    path_lakefile_in="#",
-    lake_attributes=[],
-    path_obsfile_in="#",
-    obs_attributes=[],
-    path_sub_reg_outlets_v="#",
-    threshold_con_lake=0,
-    threshold_non_con_lake=0,
-    only_included_lake_at_river_interction = False,
-    search_radius=100,
-    sl_connected_lake="#",
-    sl_non_connected_lake="#",
-    sl_lakes="#",
-    path_sub_reg_lake_r="#",
-    path_sub_reg_lake_bd_r="#",
-    catchment_without_merging_lakes="catchment_without_merging_lakes",
-    river_without_merging_lakes="river_without_merging_lakes",
-    snapped_obs_points="#",
-    cat_use_default_acc="#",
-    nfdr_arcgis="#",
-    nfdr_grass="#",
-    max_memroy=1024 * 4,
-    grassdb="#",
-    grass_location="#",
-    qgis_prefix_path="#",
-    gis_platform="qgis",
-):
-    """Add lake inflow and outflow points as new subabsin outlet
-
-    Update the subbasin delineation result generated by
-    "watershed_delineation_without_lake_method". Lake's inflow and outflow
-    points will be added into subbasin delineation result as a new subbasin
-    outlet. Result from this tool is not the final delineation result.
-    Because some lake may cover several subbasins. these subbasin
-    are not megered into one subbasin yet.
-
-    Parameters
-    ----------
-    input_geo_names             : dict
-        it is a dictionary that list the required input file names,should at
-        least indicate the name of following items:
-        fdr_arcgis                   : raster
-            it is a raster represent flow direction dataset, which is
-            using 1,2,4,...64,128 to represent different directions
-        fdr_grass                    : raster
-            it is a raster represent flow direction dataset, which is
-            using 1 - 8 to represent different directions
-        str_r                        : raster
-            it is a river network in vector format
-
-        str_v                        : vector
-            it is a river network in raster format
-
-        cat_no_lake                  : raster
-             it is the raster represent the delineated subbasins without
-             considering lakes
-        mask                         : raster
-            it is a mask raster stored in grass database, which indicate
-            the PSE
-        dem                          : raster
-            it is a dem raster stored in grass database, which is
-            has the same extent with MASK.
-        acc                          : raster
-            it is the raster represent the flow accumulation
-    path_lakefile_in            : string (optional)
-        It is a string to indicate the full path of the polygon
-        shapefile that include lake data.
-    lake_attributes             : list
-        the columns names that indicate following items has to be included
-        1) column name for the unique Id of each lake within the lake polygon shpfile;
-        2) column name for type of the lake should be integer;
-        3) column name for the volume of the lake in km3;
-        4) column name for the average depth of the lake in m;
-        5) column name for the area of the lake in km2.
-    threshold_con_lake          : float
-        It is a lake area thresthold for connected lakes in km2
-        Connected Lake with lake area below this value will be
-        not added into the subbasin delineation
-    threshold_non_con_lake      : float
-        It is a lake area thresthold for non-connected lakes in km2
-        Non connected Lake with lake area below this value will be
-        not added into the subbasin delineation
-    path_obsfile_in             : string
-        It is a string to indicate the full path of the point
-        shapefile that indicate observation gauges
-    obs_attributes              : list
-        the columns names that indicate following items has to be included
-        1) column name for the unique Id of each observation point;
-        2) column name for the unique name of each observation point;
-        3) column name for the drainage area of each observation point in km3;
-        4) column name for the source of the observation point:
-            'CA' for observation in canada;
-            'US' for observation in US;
-    search_radius               : integer
-        It is the search ratio in number of grids to snap observation
-        point into the river network.
-    path_sub_reg_outlets_v      : path
-        It is the full path of the subregion outlet vector file
-    max_memroy                  : integer
-        It is the maximum memeory that allow to be used.
-    grassdb                     : path (required)
-        It is a path to project grass database folder
-    grass_location              : string (required)
-        It is a string of grass location name
-    qgis_prefix_path            : string (required)
-        It is a string of qgis prefix path
-    gis_platform                : string
-        It is a string indicate with gis platform is used:
-        'qgis'                       : the basinmaker is running within QGIS
-        'arcgis'                     : the basinmaker is running within ArcGIS
-    Notes
-    -------
-    Raster and vector files that are generated by this function and
-    will be used by next step are list as following. All files are
-    stored at a grass database
-
-    selected_lakes              : raster
-        it is a raster represent all lakes that are selected by two lake
-        area threstholds
-    sl_nonconnect_lake          : raster
-        it is a raster represent all non connected lakes that are selected
-        by lake area threstholds
-    sl_connected_lake           : raster
-        it is a raster represent allconnected lakes that are selected
-        by lake area threstholds
-    river_without_merging_lakes : raster/vector
-        it is the updated river segment for each subbasin
-    catchment_without_merging_lakes   : raster/vector
-        it is a raster represent updated subbasins after adding lake inflow
-        and outflow points as new subbasin outlet.
-    snapped_obs_points          : raster/vector
-        it is a name of the point gis file represent successfully sanpped
-        observation points
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-
-    """
-
-    # define internal file names
-    cat_add_lake = Internal_Constant_Names["cat_add_lake"]
-    pourpoints_with_lakes = Internal_Constant_Names["pourpoints_with_lakes"]
-    pourpoints_add_obs = Internal_Constant_Names["pourpoints_add_obs"]
-    lake_outflow_pourpoints = Internal_Constant_Names["lake_outflow_pourpoints"]
-
-    if gis_platform == "qgis":
-        assert (
-            grassdb != "#"
-        ), "grass database folder is needed, when gis_platform = qgis"
-        assert (
-            grass_location != "#"
-        ), "grass location name is needed, when gis_platform = qgis"
-        assert (
-            qgis_prefix_path != "#"
-        ), "qgis prefix path is needed, when gis_platform = qgis"
-        from basinmaker.addlakeandobs.addlakesqgis import (
-            add_lakes_into_existing_watershed_delineation,
-        )
-        from basinmaker.addlakeandobs.addobsqgis import add_obs_into_existing_watershed_delineation
-        from basinmaker.addlakeandobs.definecatrivqgis import (
-            define_cat_and_riv_without_merge_lake_cats,
-        )
-    elif gis_platform == "arcgis":
-        from basinmaker.addlakeandobs.addlakesarcgis import (
-            add_lakes_into_existing_watershed_delineation,
-        )
-    else:
-        print('gis_platform    ',gis_platform,'   do not support') 
-            
-    lake_outflow_pourpoints = add_lakes_into_existing_watershed_delineation(
-        grassdb=grassdb,
-        grass_location=grass_location,
-        qgis_prefix_path=qgis_prefix_path,
-        input_geo_names=input_geo_names,
-        path_lakefile_in=path_lakefile_in,
-        lake_attributes=lake_attributes,
-        threshold_con_lake=threshold_con_lake,
-        path_sub_reg_lake_r=path_sub_reg_lake_r,
-        path_sub_reg_lake_bd_r=path_sub_reg_lake_bd_r,
-        threshold_non_con_lake=threshold_non_con_lake,
-        only_included_lake_at_river_interction = only_included_lake_at_river_interction,
-        sl_connected_lake=sl_connected_lake,
-        sl_non_connected_lake=sl_non_connected_lake,
-        sl_lakes=sl_lakes,
-        nfdr_arcgis=nfdr_arcgis,
-        nfdr_grass=nfdr_grass,
-        cat_add_lake=cat_add_lake,
-        pourpoints_with_lakes=pourpoints_with_lakes,
-        cat_use_default_acc=cat_use_default_acc,
-        lake_outflow_pourpoints=lake_outflow_pourpoints,
-        max_memroy=max_memroy,
-    )
-    ## add variable into input geo names
-    input_geo_names["cat_add_lake"] = cat_add_lake
-    input_geo_names["pourpoints_with_lakes"] = pourpoints_with_lakes
-    input_geo_names["lake_outflow_pourpoints"] = lake_outflow_pourpoints
-    input_geo_names["sl_non_connected_lake"] = sl_non_connected_lake
-    input_geo_names["nfdr_grass"] = nfdr_grass
-
-    if path_obsfile_in != "#":
-        add_obs_into_existing_watershed_delineation(
-            grassdb=grassdb,
-            grass_location=grass_location,
-            qgis_prefix_path=qgis_prefix_path,
-            input_geo_names=input_geo_names,
-            path_obsfile_in=path_obsfile_in,
-            obs_attributes=obs_attributes,
-            search_radius=search_radius,
-            path_sub_reg_outlets_v=path_sub_reg_outlets_v,
-            max_memroy=max_memroy,
-            pourpoints_add_obs=pourpoints_add_obs,
-            snapped_obs_points=snapped_obs_points,
-        )
-    else:
-        pourpoints_add_obs = pourpoints_with_lakes
-
-    input_geo_names["pourpoints_add_obs"] = pourpoints_add_obs
-
-    define_cat_and_riv_without_merge_lake_cats(
-        grassdb=grassdb,
-        grass_location=grass_location,
-        qgis_prefix_path=qgis_prefix_path,
-        input_geo_names=input_geo_names,
-        path_lakefile_in=path_lakefile_in,
-        catchment_without_merging_lakes=catchment_without_merging_lakes,
-        river_without_merging_lakes=river_without_merging_lakes,
-        max_memroy=max_memroy,
-    )
+from basinmaker.utilities.utilities import Internal_Constant_Names
+
+
+def add_lakes_and_obs_into_existing_watershed_delineation(
+    input_geo_names,
+    path_lakefile_in="#",
+    lake_attributes=[],
+    path_obsfile_in="#",
+    obs_attributes=[],
+    path_sub_reg_outlets_v="#",
+    threshold_con_lake=0,
+    threshold_non_con_lake=0,
+    only_included_lake_at_river_interction = False,
+    search_radius=100,
+    sl_connected_lake="#",
+    sl_non_connected_lake="#",
+    sl_lakes="#",
+    path_sub_reg_lake_r="#",
+    path_sub_reg_lake_bd_r="#",
+    catchment_without_merging_lakes="catchment_without_merging_lakes",
+    river_without_merging_lakes="river_without_merging_lakes",
+    snapped_obs_points="#",
+    cat_use_default_acc="#",
+    nfdr_arcgis="#",
+    nfdr_grass="#",
+    fac_thresold = 5000,
+    max_memroy=1024 * 4,
+    grassdb="#",
+    grass_location="#",
+    qgis_prefix_path="#",
+    gis_platform="qgis",
+):
+    """Add lake inflow and outflow points as new subabsin outlet
+
+    Update the subbasin delineation result generated by
+    "watershed_delineation_without_lake_method". Lake's inflow and outflow
+    points will be added into subbasin delineation result as a new subbasin
+    outlet. Result from this tool is not the final delineation result.
+    Because some lake may cover several subbasins. these subbasin
+    are not megered into one subbasin yet.
+
+    Parameters
+    ----------
+    input_geo_names             : dict
+        it is a dictionary that list the required input file names,should at
+        least indicate the name of following items:
+        fdr_arcgis                   : raster
+            it is a raster represent flow direction dataset, which is
+            using 1,2,4,...64,128 to represent different directions
+        fdr_grass                    : raster
+            it is a raster represent flow direction dataset, which is
+            using 1 - 8 to represent different directions
+        str_r                        : raster
+            it is a river network in vector format
+
+        str_v                        : vector
+            it is a river network in raster format
+
+        cat_no_lake                  : raster
+             it is the raster represent the delineated subbasins without
+             considering lakes
+        mask                         : raster
+            it is a mask raster stored in grass database, which indicate
+            the PSE
+        dem                          : raster
+            it is a dem raster stored in grass database, which is
+            has the same extent with MASK.
+        acc                          : raster
+            it is the raster represent the flow accumulation
+    path_lakefile_in            : string (optional)
+        It is a string to indicate the full path of the polygon
+        shapefile that include lake data.
+    lake_attributes             : list
+        the columns names that indicate following items has to be included
+        1) column name for the unique Id of each lake within the lake polygon shpfile;
+        2) column name for type of the lake should be integer;
+        3) column name for the volume of the lake in km3;
+        4) column name for the average depth of the lake in m;
+        5) column name for the area of the lake in km2.
+    threshold_con_lake          : float
+        It is a lake area thresthold for connected lakes in km2
+        Connected Lake with lake area below this value will be
+        not added into the subbasin delineation
+    threshold_non_con_lake      : float
+        It is a lake area thresthold for non-connected lakes in km2
+        Non connected Lake with lake area below this value will be
+        not added into the subbasin delineation
+    path_obsfile_in             : string
+        It is a string to indicate the full path of the point
+        shapefile that indicate observation gauges
+    obs_attributes              : list
+        the columns names that indicate following items has to be included
+        1) column name for the unique Id of each observation point;
+        2) column name for the unique name of each observation point;
+        3) column name for the drainage area of each observation point in km3;
+        4) column name for the source of the observation point:
+            'CA' for observation in canada;
+            'US' for observation in US;
+    search_radius               : integer
+        It is the search ratio in number of grids to snap observation
+        point into the river network.
+    path_sub_reg_outlets_v      : path
+        It is the full path of the subregion outlet vector file
+    max_memroy                  : integer
+        It is the maximum memeory that allow to be used.
+    grassdb                     : path (required)
+        It is a path to project grass database folder
+    grass_location              : string (required)
+        It is a string of grass location name
+    qgis_prefix_path            : string (required)
+        It is a string of qgis prefix path
+    gis_platform                : string
+        It is a string indicate with gis platform is used:
+        'qgis'                       : the basinmaker is running within QGIS
+        'arcgis'                     : the basinmaker is running within ArcGIS
+    Notes
+    -------
+    Raster and vector files that are generated by this function and
+    will be used by next step are list as following. All files are
+    stored at a grass database
+
+    selected_lakes              : raster
+        it is a raster represent all lakes that are selected by two lake
+        area threstholds
+    sl_nonconnect_lake          : raster
+        it is a raster represent all non connected lakes that are selected
+        by lake area threstholds
+    sl_connected_lake           : raster
+        it is a raster represent allconnected lakes that are selected
+        by lake area threstholds
+    river_without_merging_lakes : raster/vector
+        it is the updated river segment for each subbasin
+    catchment_without_merging_lakes   : raster/vector
+        it is a raster represent updated subbasins after adding lake inflow
+        and outflow points as new subbasin outlet.
+    snapped_obs_points          : raster/vector
+        it is a name of the point gis file represent successfully sanpped
+        observation points
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+
+    """
+
+    # define internal file names
+    cat_add_lake = Internal_Constant_Names["cat_add_lake"]
+    pourpoints_with_lakes = Internal_Constant_Names["pourpoints_with_lakes"]
+    pourpoints_add_obs = Internal_Constant_Names["pourpoints_add_obs"]
+    lake_outflow_pourpoints = Internal_Constant_Names["lake_outflow_pourpoints"]
+
+    if gis_platform == "qgis":
+        assert (
+            grassdb != "#"
+        ), "grass database folder is needed, when gis_platform = qgis"
+        assert (
+            grass_location != "#"
+        ), "grass location name is needed, when gis_platform = qgis"
+        assert (
+            qgis_prefix_path != "#"
+        ), "qgis prefix path is needed, when gis_platform = qgis"
+        from basinmaker.addlakeandobs.addlakesqgis import (
+            add_lakes_into_existing_watershed_delineation,
+        )
+        from basinmaker.addlakeandobs.addobsqgis import add_obs_into_existing_watershed_delineation
+        from basinmaker.addlakeandobs.definecatrivqgis import (
+            define_cat_and_riv_without_merge_lake_cats,
+        )
+    elif gis_platform == "arcgis":
+        from basinmaker.addlakeandobs.addlakesarcgis import (
+            add_lakes_into_existing_watershed_delineation,
+        )
+        from basinmaker.addlakeandobs.addobsarcgis import add_obs_into_existing_watershed_delineation
+
+        from basinmaker.addlakeandobs.definecatrivarcgis import (
+            define_cat_and_riv_without_merge_lake_cats,
+        )
+
+    else:
+        print('gis_platform    ',gis_platform,'   do not support')
+
+    lake_outflow_pourpoints = add_lakes_into_existing_watershed_delineation(
+        grassdb=grassdb,
+        grass_location=grass_location,
+        qgis_prefix_path=qgis_prefix_path,
+        input_geo_names=input_geo_names,
+        path_lakefile_in=path_lakefile_in,
+        lake_attributes=lake_attributes,
+        threshold_con_lake=threshold_con_lake,
+        path_sub_reg_lake_r=path_sub_reg_lake_r,
+        path_sub_reg_lake_bd_r=path_sub_reg_lake_bd_r,
+        threshold_non_con_lake=threshold_non_con_lake,
+        only_included_lake_at_river_interction = only_included_lake_at_river_interction,
+        sl_connected_lake=sl_connected_lake,
+        sl_non_connected_lake=sl_non_connected_lake,
+        sl_lakes=sl_lakes,
+        nfdr_arcgis=nfdr_arcgis,
+        nfdr_grass=nfdr_grass,
+        cat_add_lake=cat_add_lake,
+        pourpoints_with_lakes=pourpoints_with_lakes,
+        cat_use_default_acc=cat_use_default_acc,
+        lake_outflow_pourpoints=lake_outflow_pourpoints,
+        max_memroy=max_memroy,
+    )
+    ## add variable into input geo names
+    input_geo_names["cat_add_lake"] = cat_add_lake
+    input_geo_names["pourpoints_with_lakes"] = pourpoints_with_lakes
+    input_geo_names["lake_outflow_pourpoints"] = lake_outflow_pourpoints
+    input_geo_names["sl_non_connected_lake"] = sl_non_connected_lake
+    input_geo_names["nfdr_grass"] = nfdr_grass
+
+    if path_obsfile_in != "#":
+        add_obs_into_existing_watershed_delineation(
+            grassdb=grassdb,
+            grass_location=grass_location,
+            qgis_prefix_path=qgis_prefix_path,
+            input_geo_names=input_geo_names,
+            path_obsfile_in=path_obsfile_in,
+            obs_attributes=obs_attributes,
+            search_radius=search_radius,
+            path_sub_reg_outlets_v=path_sub_reg_outlets_v,
+            max_memroy=max_memroy,
+            pourpoints_add_obs=pourpoints_add_obs,
+            snapped_obs_points=snapped_obs_points,
+        )
+    else:
+        pourpoints_add_obs = pourpoints_with_lakes
+
+    input_geo_names["pourpoints_add_obs"] = pourpoints_add_obs
+
+    define_cat_and_riv_without_merge_lake_cats(
+        grassdb=grassdb,
+        grass_location=grass_location,
+        qgis_prefix_path=qgis_prefix_path,
+        input_geo_names=input_geo_names,
+        path_lakefile_in=path_lakefile_in,
+        catchment_without_merging_lakes=catchment_without_merging_lakes,
+        river_without_merging_lakes=river_without_merging_lakes,
+        max_memroy=max_memroy,
+    )
```

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/addobsqgis.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/addobsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/definecatrivqgis.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/definecatrivqgis.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from basinmaker.func.grassgis import *
-from basinmaker.func.qgis import *
-from basinmaker.func.pdtable import *
-from basinmaker.func.rarray import *
-from basinmaker.utilities.utilities import *
-import sqlite3
-
-
-def define_cat_and_riv_without_merge_lake_cats(
-    grassdb,
-    grass_location,
-    qgis_prefix_path,
-    input_geo_names,
-    path_lakefile_in,
-    catchment_without_merging_lakes="catchment_without_merging_lakes",
-    river_without_merging_lakes="river_without_merging_lakes",
-    max_memroy=1024 * 4,
-):
-
-    fdr_arcgis = input_geo_names["fdr_arcgis"]
-    fdr_grass = input_geo_names["fdr_grass"]
-    str_r = input_geo_names["str_r"]
-    str_v = input_geo_names["str_v"]
-    acc = input_geo_names["acc"]
-    mask = input_geo_names["mask"]
-    dem = input_geo_names["dem"]
-    nfdr_grass = input_geo_names["nfdr_grass"]
-    sl_non_connected_lake = input_geo_names["sl_non_connected_lake"]
-    pourpoints_add_obs = input_geo_names["pourpoints_add_obs"]
-    lake_outflow_pourpoints = input_geo_names["lake_outflow_pourpoints"]
-
-    import grass.script as grass
-    import grass.script.setup as gsetup
-    from grass.pygrass.modules import Module
-    from grass.pygrass.modules.shortcuts import general as g
-    from grass.pygrass.modules.shortcuts import raster as r
-    from grass.script import array as garray
-    from grass.script import core as gcore
-    from grass_session import Session
-
-    os.environ.update(
-        dict(GRASS_COMPRESS_NULLS="1", GRASS_COMPRESSOR="ZSTD", GRASS_VERBOSE="1")
-    )
-    PERMANENT = Session()
-    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
-
-    grass.run_command(
-        "r.to.vect",
-        input=pourpoints_add_obs,
-        output=pourpoints_add_obs,
-        type="point",
-        overwrite=True,
-        flags="v",
-    )
-
-    if path_lakefile_in != "#":
-        grass.run_command(
-            "r.stream.basins",
-            direction=nfdr_grass,
-            points=pourpoints_add_obs,
-            basins="define_cat_and_riv_1",
-            overwrite=True,
-            memory=max_memroy,
-        )
-        # find non connected lake catchments
-        lakeid, catid = generate_stats_list_from_grass_raster(
-            grass,
-            mode=2,
-            input_a=lake_outflow_pourpoints,
-            input_b="define_cat_and_riv_1",
-        )
-        lakecat_ids = np.column_stack((lakeid, catid))
-
-        # find all non connected cat ids
-        non_connected_lakeids, temp = generate_stats_list_from_grass_raster(
-            grass,
-            mode=1,
-            input_a=sl_non_connected_lake,
-        )
-
-        non_cl_lake_catid = lakecat_ids[
-            np.isin(lakecat_ids[:, 0], np.array(non_connected_lakeids)), 1
-        ]
-
-        # find all catids
-        all_catids, temp = generate_stats_list_from_grass_raster(
-            grass,
-            mode=1,
-            input_a="define_cat_and_riv_1",
-        )
-        all_catids = np.array(all_catids)
-        not_non_cl_lake_catids = all_catids[
-            np.logical_not(np.isin(all_catids, non_cl_lake_catid))
-        ]
-        # grass.run_command(
-        #     "g.copy", rast=("define_cat_and_riv_1", "non_cl_lake_cat"), overwrite=True
-        # )
-        non_cl_lake_cat_array = garray.array(mapname="define_cat_and_riv_1")
-        if (len(not_non_cl_lake_catids) > 0):
-            mask = np.isin(non_cl_lake_cat_array, not_non_cl_lake_catids)
-            non_cl_lake_cat_array[mask] = -9999
-        temparray = garray.array()
-        temparray[:, :] = non_cl_lake_cat_array[:, :]
-        temparray.write(mapname="non_cl_lake_cat", overwrite=True)
-        grass.run_command("r.null", map="non_cl_lake_cat", setnull=[-9999, 0])
-        exp = "%s = int(%s)" % (
-            "non_cl_lake_cat",
-            "non_cl_lake_cat",
-        )
-        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-
-        # grass.run_command(
-        #     "r.null",
-        #     map="non_cl_lake_cat",
-        #     setnull=not_non_cl_lake_catids,
-        #     overwrite=True,
-        # )
-
-        # define str and cat
-        grass.run_command(
-            "r.cross",
-            input=[str_r, "define_cat_and_riv_1"],
-            output="nstr_seg_t",
-            flags="z",
-            overwrite=True,
-        )
-        grass.run_command(
-            "r.mapcalc", expression="nstr_seg = int(nstr_seg_t) + 1", overwrite=True
-        )
-        grass.run_command(
-            "r.stream.basins",
-            direction=nfdr_grass,
-            stream="nstr_seg",
-            basins="define_cat_and_riv_2",
-            overwrite=True,
-        )
-
-        grass.run_command(
-            "r.cross",
-            input=["define_cat_and_riv_2", "non_cl_lake_cat"],
-            output=catchment_without_merging_lakes,
-            overwrite=True,
-        )
-
-        exp = "%s = %s + 1" % (
-            catchment_without_merging_lakes,
-            catchment_without_merging_lakes,
-        )
-        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-
-        exp = "%s = if(isnull(int(%s)),null(),%s)" % (
-            river_without_merging_lakes,
-            str_r,
-            catchment_without_merging_lakes,
-        )
-        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-
-    else:
-        grass.run_command(
-            "r.stream.basins",
-            direction=fdr_grass,
-            points=pourpoints_add_obs,
-            basins="define_cat_and_riv_1",
-            overwrite=True,
-            memory=max_memroy,
-        )
-
-        grass.run_command(
-            "r.cross",
-            input=[str_r, "define_cat_and_riv_1"],
-            output="nstr_seg_t",
-            flags="z",
-            overwrite=True,
-        )
-        grass.run_command(
-            "r.mapcalc", expression="nstr_seg = int(nstr_seg_t) + 1", overwrite=True
-        )
-
-        grass.run_command(
-            "r.stream.basins",
-            direction=fdr_grass,
-            stream="nstr_seg",
-            basins=catchment_without_merging_lakes,
-            overwrite=True,
-        )
-
-        exp = "%s = if(isnull(int(%s)),null(),%s)" % (
-            river_without_merging_lakes,
-            str_r,
-            catchment_without_merging_lakes,
-        )
-        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-
-    PERMANENT.close()
-    return
+from basinmaker.func.grassgis import *
+from basinmaker.func.qgis import *
+from basinmaker.func.pdtable import *
+from basinmaker.func.rarray import *
+from basinmaker.utilities.utilities import *
+import sqlite3
+
+
+def define_cat_and_riv_without_merge_lake_cats(
+    grassdb,
+    grass_location,
+    qgis_prefix_path,
+    input_geo_names,
+    path_lakefile_in,
+    catchment_without_merging_lakes="catchment_without_merging_lakes",
+    river_without_merging_lakes="river_without_merging_lakes",
+    max_memroy=1024 * 4,
+):
+
+    fdr_arcgis = input_geo_names["fdr_arcgis"]
+    fdr_grass = input_geo_names["fdr_grass"]
+    str_r = input_geo_names["str_r"]
+    str_v = input_geo_names["str_v"]
+    acc = input_geo_names["acc"]
+    mask = input_geo_names["mask"]
+    dem = input_geo_names["dem"]
+    nfdr_grass = input_geo_names["nfdr_grass"]
+    sl_non_connected_lake = input_geo_names["sl_non_connected_lake"]
+    pourpoints_add_obs = input_geo_names["pourpoints_add_obs"]
+    lake_outflow_pourpoints = input_geo_names["lake_outflow_pourpoints"]
+
+    import grass.script as grass
+    import grass.script.setup as gsetup
+    from grass.pygrass.modules import Module
+    from grass.pygrass.modules.shortcuts import general as g
+    from grass.pygrass.modules.shortcuts import raster as r
+    from grass.script import array as garray
+    from grass.script import core as gcore
+    from grass_session import Session
+
+    os.environ.update(
+        dict(GRASS_COMPRESS_NULLS="1", GRASS_COMPRESSOR="ZSTD", GRASS_VERBOSE="1")
+    )
+    PERMANENT = Session()
+    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
+
+    grass.run_command(
+        "r.to.vect",
+        input=pourpoints_add_obs,
+        output=pourpoints_add_obs,
+        type="point",
+        overwrite=True,
+        flags="v",
+    )
+
+    if path_lakefile_in != "#":
+        grass.run_command(
+            "r.stream.basins",
+            direction=nfdr_grass,
+            points=pourpoints_add_obs,
+            basins="define_cat_and_riv_1",
+            overwrite=True,
+            memory=max_memroy,
+        )
+        # find non connected lake catchments
+        lakeid, catid = generate_stats_list_from_grass_raster(
+            grass,
+            mode=2,
+            input_a=lake_outflow_pourpoints,
+            input_b="define_cat_and_riv_1",
+        )
+        lakecat_ids = np.column_stack((lakeid, catid))
+
+        # find all non connected cat ids
+        non_connected_lakeids, temp = generate_stats_list_from_grass_raster(
+            grass,
+            mode=1,
+            input_a=sl_non_connected_lake,
+        )
+
+        non_cl_lake_catid = lakecat_ids[
+            np.isin(lakecat_ids[:, 0], np.array(non_connected_lakeids)), 1
+        ]
+
+        # find all catids
+        all_catids, temp = generate_stats_list_from_grass_raster(
+            grass,
+            mode=1,
+            input_a="define_cat_and_riv_1",
+        )
+        all_catids = np.array(all_catids)
+        not_non_cl_lake_catids = all_catids[
+            np.logical_not(np.isin(all_catids, non_cl_lake_catid))
+        ]
+        # grass.run_command(
+        #     "g.copy", rast=("define_cat_and_riv_1", "non_cl_lake_cat"), overwrite=True
+        # )
+        non_cl_lake_cat_array = garray.array(mapname="define_cat_and_riv_1")
+        if (len(not_non_cl_lake_catids) > 0):
+            mask = np.isin(non_cl_lake_cat_array, not_non_cl_lake_catids)
+            non_cl_lake_cat_array[mask] = -9999
+        temparray = garray.array()
+        temparray[:, :] = non_cl_lake_cat_array[:, :]
+        temparray.write(mapname="non_cl_lake_cat", overwrite=True)
+        grass.run_command("r.null", map="non_cl_lake_cat", setnull=[-9999, 0])
+        exp = "%s = int(%s)" % (
+            "non_cl_lake_cat",
+            "non_cl_lake_cat",
+        )
+        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+        # grass.run_command(
+        #     "r.null",
+        #     map="non_cl_lake_cat",
+        #     setnull=not_non_cl_lake_catids,
+        #     overwrite=True,
+        # )
+
+        # define str and cat
+        grass.run_command(
+            "r.cross",
+            input=[str_r, "define_cat_and_riv_1"],
+            output="nstr_seg_t",
+            flags="z",
+            overwrite=True,
+        )
+        grass.run_command(
+            "r.mapcalc", expression="nstr_seg = int(nstr_seg_t) + 1", overwrite=True
+        )
+        grass.run_command(
+            "r.stream.basins",
+            direction=nfdr_grass,
+            stream="nstr_seg",
+            basins="define_cat_and_riv_2",
+            overwrite=True,
+        )
+
+        grass.run_command(
+            "r.cross",
+            input=["define_cat_and_riv_2", "non_cl_lake_cat"],
+            output=catchment_without_merging_lakes,
+            overwrite=True,
+        )
+
+        exp = "%s = %s + 1" % (
+            catchment_without_merging_lakes,
+            catchment_without_merging_lakes,
+        )
+        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+        exp = "%s = if(isnull(int(%s)),null(),%s)" % (
+            river_without_merging_lakes,
+            str_r,
+            catchment_without_merging_lakes,
+        )
+        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+    else:
+        grass.run_command(
+            "r.stream.basins",
+            direction=fdr_grass,
+            points=pourpoints_add_obs,
+            basins="define_cat_and_riv_1",
+            overwrite=True,
+            memory=max_memroy,
+        )
+
+        grass.run_command(
+            "r.cross",
+            input=[str_r, "define_cat_and_riv_1"],
+            output="nstr_seg_t",
+            flags="z",
+            overwrite=True,
+        )
+        grass.run_command(
+            "r.mapcalc", expression="nstr_seg = int(nstr_seg_t) + 1", overwrite=True
+        )
+
+        grass.run_command(
+            "r.stream.basins",
+            direction=fdr_grass,
+            stream="nstr_seg",
+            basins=catchment_without_merging_lakes,
+            overwrite=True,
+        )
+
+        exp = "%s = if(isnull(int(%s)),null(),%s)" % (
+            river_without_merging_lakes,
+            str_r,
+            catchment_without_merging_lakes,
+        )
+        grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+    PERMANENT.close()
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/definelaketypeqgis.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/definelaketypeqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/filterlakesqgis.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/filterlakesqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/modifyfdr.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/modifyfdr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/modifystr.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/modifystr.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/addlakeandobs/pourpointsqgis.py` & `basinmaker-3.0.3/basinmaker/addlakeandobs/pourpointsqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py` & `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generatehru_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py` & `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/generateraveninput_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py` & `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/selectprod_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py` & `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplyda_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py` & `basinmaker-3.0.3/basinmaker/arcgisguiwarpper/simplylakes_arcgis_wrapper.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/basinmaker.py` & `basinmaker-3.0.3/basinmaker/basinmaker.py`

 * *Files 10% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     def Remove_Small_Lakes(
         self,
         path_output_folder="#",
         routing_product_folder  = '#',
         connected_lake_area_thresthold=-1,
         non_connected_lake_area_thresthold =-1,
         selected_lake_ids=[],
+        area_thresthold = 10*30*30/1000/1000,
         gis_platform="qgis",
     ):
         """This function is to simplify the hydrologic routing network by removing
         lakes.
 
         Parameters
         ----------
@@ -207,14 +208,21 @@
         non_connected_lake_area_thresthold             : float (optional)
             is a lake area thresthold for non-connected lakes in km2
             Non connected lake with lake area below below which lake will be removed
         selected_lake_ids          : list (optional)
             A list of lake IDs from in the hydrologic routing network (Column 'HyLakeId').
             Lakes with their lake ID in this list will be kept by the BasinMaker even
             if their area smaller than the lake area threstholds
+        area_thresthold             : float (optional)
+            This parameter sets a subbasin area threshold in square kilometers (km²). 
+            Subbasins with an area below this threshold will be merged with downstream 
+            or upstream subbasins, depending on their location within the river network. 
+            This can be useful for simplifying the river network and reducing computational
+            requirements. The parameter is optional and has a default value of 0.009 km2. 
+            If the parameter is set to 0, no subbasin merging will be performed.
 
         Returns
         -------
 
         Notes
         -----
         This function has no return values, The simplified hydrological routing
@@ -247,15 +255,15 @@
             minimum drainage area threshold)
         sl_connected_lake.shp                           : shapefile
             the GIS layer containing the lake polygons of lakes that are connected
             by the river_without_merging_lakes.shp
         sl_non_connected_lake.shp                       : shapefile
             the GIS layer containing the lake polygons of lakes that are not connected
             by the river_without_merging_lakes.shp
-        obs_gauges                                      : shapefile
+        poi                                            : shapefile
             It is the point shapefile that represent the point of interest
             after snap to river network.
 
         Examples
         -------
 
 
@@ -284,45 +292,50 @@
         from basinmaker.postprocessing.postprocessingfunctions import (
             combine_catchments_covered_by_the_same_lake_method,
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = path_output_folder,
             qgis_prefix_path=self.qgispp,
+            area_thresthold = area_thresthold,
             gis_platform=gis_platform,
         )
 
 
     def Decrease_River_Network_Resolution(
         self,
         path_output_folder="#",
         routing_product_folder = '#',
         gis_platform="qgis",
         minimum_subbasin_drainage_area=-1,
+        area_thresthold = 10*30*30/1000/1000,
     ):
         """ This function is to simplify the hydrologic routing network by
         removing subbasins/river reaches with their drainage area below user provided
         drainage area thresthold.
 
         Parameters
         ----------
-
-        Parameters
-        ----------
         path_output_folder                   : string
             is the folder path that stores generated outputs
         routing_product_folder         : string
             is the folder path where the input hydrologic routing network is stored
         gis_platform                   : string
             is the parameter indicating which gis platform is used. It can be
             either "qgis" or "arcgis".
         minimum_subbasin_drainage_area                 : float
             is a subbasin drainage area thresthold, subbasin with their
             drainage area smaller than this thresthold will be removed.
-
+        area_thresthold             : float (optional)
+            This parameter sets a subbasin area threshold in square kilometers (km²). 
+            Subbasins with an area below this threshold will be merged with downstream 
+            or upstream subbasins, depending on their location within the river network. 
+            This can be useful for simplifying the river network and reducing computational
+            requirements. The parameter is optional and has a default value of 0.009 km2. 
+            If the parameter is set to 0, no subbasin merging will be performed.
 
         Returns
         -------
 
         Notes
         -----
         This function has no return values, The simplified hydrological routing
@@ -355,15 +368,15 @@
             minimum drainage area threshold)
         sl_connected_lake.shp                           : shapefile
             the GIS layer containing the lake polygons of lakes that are connected
             by the river_without_merging_lakes.shp
         sl_non_connected_lake.shp                       : shapefile
             the GIS layer containing the lake polygons of lakes that are not connected
             by the river_without_merging_lakes.shp
-        obs_gauges                                      : shapefile
+        poi                                      : shapefile
             It is the point shapefile that represent the point of interest
             after snap to river network.
 
         Examples
         -------
 
 
@@ -383,14 +396,130 @@
         from basinmaker.postprocessing.postprocessingfunctions import (
             combine_catchments_covered_by_the_same_lake_method,
         )
 
         combine_catchments_covered_by_the_same_lake_method(
             Routing_Product_Folder = path_output_folder,
             qgis_prefix_path=self.qgispp,
+            area_thresthold = area_thresthold,
+            gis_platform=gis_platform,
+        )
+
+    def Add_Point_Of_Interest_Sites_In_Routing_Product(
+        self,
+        routing_product_folder= '#',
+        path_to_points_of_interest_points = '#',
+        path_output_folder="#",
+        clean_exist_pois = True,
+        gis_platform="purepy",
+        area_thresthold = 10*30*30/1000/1000,
+    ):
+        """ The function allows the user to modify point of interest (POI) 
+        related attributes in the routing product. The function is particularly
+        useful when the user wants to add new POI sites, remove existing POI 
+        sites,or modify the location of existing POI sites in the developed 
+        routing products. If the user observes a small subbasin that cannot 
+        be removed by the Decrease_River_Network_Resolution function due 
+        to it representing an unexpected POI, they can use this function to 
+        remove the POI from the routing product and then 
+        apply the Decrease_River_Network_Resolution function.
+
+        Parameters
+        ----------
+        path_output_folder                   : string
+            is the folder path that stores generated outputs
+        routing_product_folder         : string
+            is the folder path where the input hydrologic routing network is stored
+        path_to_points_of_interest_points                : string
+            is the path to the point shapefile that contains the point of 
+            interest (POI) sites. The shapefile must have an attribute table that includes 
+            the following columns:
+              - Obs_NM (string): This column should contain the name or ID of the POI site.
+              - DA_Obs (float): This column should contain the drainage area of the POI site.
+              - SRC_obs (string): This column should contain the source of the POI site.
+        gis_platform                   : string
+            is the parameter indicating which gis platform is used. Currenly, only "purepy" 
+            is allowed for this parameter.
+        clean_exist_pois                : boolean
+            Indicate if user want to remove all existing POI in the input routing product.
+        area_thresthold             : float (optional)
+            This parameter sets a subbasin area threshold in square kilometers (km²). 
+            Subbasins with an area below this threshold will be merged with downstream 
+            or upstream subbasins, depending on their location within the river network. 
+            This can be useful for simplifying the river network and reducing computational
+            requirements. The parameter is optional and has a default value of 0.009 km2. 
+            If the parameter is set to 0, no subbasin merging will be performed.
+
+        Returns
+        -------
+
+        Notes
+        -----
+        This function has no return values, The modified hydrological routing
+        network will be generated in the path_output_folder including following
+        files:
+
+        finalcat_info.shp                     : shapefile
+            The finalized hydrologic routing network. the GIS layer containing
+            subbasin polygons which respect the lake inflow and outflow routing
+            structures. This layer contains all the necessary information for
+            hydrologic routing through the lake-river network.
+        finalcat_info_riv.shp                 : shapefile
+            The finalized hydrologic routing network. the GIS layer containing
+            river network polylines in the routing network.
+        catchment_without_merging_lakes.shp             : shapefile
+            The GIS layer containing subbasin polygons of an incomplete hydrologic
+            routing network. In this incomplete hydrologic routing network subbasin
+            polygons covered by the same lake are not merged into one lake subbasin
+            yet. This incomplete hydrologic routing network is only intended as
+            input to customize the routing network with our BasinMaker GIS toolbox
+            (for example by defining new lake area thresholds and/or a new catchment
+            minimum drainage area threshold)
+        river_without_merging_lakes.shp                 : shapefile
+            The GIS layer containing river polylines of an incomplete hydrologic
+            routing network. In this incomplete hydrologic routing network, the
+            river polylines covered by the same lake are not merged into one river
+            segment yet. This incomplete hydrologic routing network is only intended as
+            input to customize the routing network with our BasinMaker GIS toolbox
+            (for example by defining new lake area thresholds and/or a new catchment
+            minimum drainage area threshold)
+        sl_connected_lake.shp                           : shapefile
+            the GIS layer containing the lake polygons of lakes that are connected
+            by the river_without_merging_lakes.shp
+        sl_non_connected_lake.shp                       : shapefile
+            the GIS layer containing the lake polygons of lakes that are not connected
+            by the river_without_merging_lakes.shp
+        poi                                      : shapefile
+            It is the point shapefile that represent the point of interest
+            after snap to river network.
+
+        Examples
+        -------
+
+        """
+        from basinmaker.postprocessing.postprocessingfunctions import (
+            add_point_of_interest_sites_in_routing_product_method,
+        )
+
+        add_point_of_interest_sites_in_routing_product_method(
+            routing_product_folder= routing_product_folder,
+            path_to_points_of_interest_points = path_to_points_of_interest_points,
+            path_output_folder = path_output_folder,
+            clean_exist_pois = clean_exist_pois,
+            gis_platform=gis_platform,
+        )
+
+        from basinmaker.postprocessing.postprocessingfunctions import (
+            combine_catchments_covered_by_the_same_lake_method,
+        )
+
+        combine_catchments_covered_by_the_same_lake_method(
+            Routing_Product_Folder = path_output_folder,
+            qgis_prefix_path=self.qgispp,
+            area_thresthold = area_thresthold,
             gis_platform=gis_platform,
         )
 
     def Select_Subregion_Of_Routing_Structure(
         self,
         path_output_folder="#",
         routing_product_folder = '#',
@@ -409,21 +538,16 @@
         gis_platform                   : string
             is the parameter indicating which gis platform is used. It can be
             either "qgis" or "arcgis".
         most_down_stream_subbasin_ids                    : list
             A list of subbasin ID, the subbasin IDs in this list should
             be the most downstream subbasin ID of each interested watershed.
         most_up_stream_subbasin_ids                      : list
-            A list of subbasin ID, the subbasin IDs in this list should be
-            the most upstream subbasin ID of each interested watershed.
-            Value -1 is required to extracting the entire contribute subbains.
-            subbasins between most_down_stream_subbasin_ids[i] and
-            most_up_stream_subbasin_ids[i] are extracted when positive
-            most_up_stream_subbasin_ids[i] is provided. i represent ith time in
-            most_down_stream_subbasin_ids and  most_up_stream_subbasin_ids
+            A list of subbasin ID, the subbasins that drainage to the SubID in this list will be excluded.
+            Value [-1] is required to indicate no upstream subbasin needs to be removed.
 
         Returns
         -------
 
         Notes
         -----
         This function has no return values, The extracted hydrological routing
@@ -456,15 +580,15 @@
             minimum drainage area threshold)
         sl_connected_lake.shp                           : shapefile
             the GIS layer containing the lake polygons of lakes that are connected
             by the river_without_merging_lakes.shp
         sl_non_connected_lake.shp                       : shapefile
             the GIS layer containing the lake polygons of lakes that are not connected
             by the river_without_merging_lakes.shp
-        obs_gauges                                      : shapefile
+        poi                                      : shapefile
             It is the point shapefile that represent the point of interest
             after snap to river network.
 
         Examples
         -------
 
         """
@@ -581,22 +705,21 @@
         path_vegetation_polygon                     : string (Optional)
             is the path to the vegetation polygon. when vegetation polygon is not
             provided. The Veg ID in path_veg_info should be the same
             as Landuse ID.
         path_other_polygon_1                 : string (Optional)
             is the path to the other polygon that will be used to define HRU,
             such as elevation band, or aspect.
-        path_other_polygon_2                 : string (Optional)
-            is the path to the other polygon that will be used to define HRU,
-            such as elevation band, or aspect.
         DEM                              : string (optional)
             is the path to a raster elevation dataset, that is used to
             calcuate average apspect, elevation and slope within each HRU.
             if no data is provided, subbasin averaged value will be used for
             each HRU.
+        area_ratio_thresholds                  : list (optional)
+            It is a list of HRU area thresthold for landuse, soil and other_1 layer respectively. In BasinMaker HRU calculation, each layer will firstly be overlaid to the subbasin map. Attributes falling into each subbasin with their area ratios (i.e., the intersected area to the subbasin area) smaller than the defined threshold values will then be dissolved into the largest part. For example, if forest area ratio in a subbasin, say subbasin #10, is 0.05, while we set the area threshold for land cover is 0.1. The forest polygons will then be dissolved to the largest land cover type in subbasin #10. 
         Returns
         -------
 
         Notes
         -----
         This function has no return values, but a HRU map saved in the
         path_output_folder
@@ -666,24 +789,28 @@
 
     """
 
     def __init__(
         self,
         path_output_folder="#",
         path_working_folder="#",
+        fac_thresold = 5000,
     ):
 
         # define drived values
         # create folders
         self.path_output_folder = path_output_folder
         self.path_working_folder = path_working_folder
-
+        self.fac_thresold = fac_thresold
         #        os.makedirs(self.path_output_folder, exist_ok=True)
         os.makedirs(self.path_working_folder, exist_ok=True)
 
+        file = open(os.path.join(path_working_folder, "log.txt"), 'w')
+        file.close()
+
         # obtain qgis prefix path
         if os.getenv("QGIS_PREFIX_PATH"):
             self.qgispp = os.environ["QGIS_PREFIX_PATH"]
         else:
             self.qgispp = '#'
         # obtain basinmaker path
         # define grass database folder
@@ -704,15 +831,14 @@
 
         # define constants
 
         # default channel manning's coefficient
         DEFAULT_CHN = 0.035
         # minimum channel slope
         MIN_RIV_SLP = 0.00001
-
         # default pre processed and well prepared spatial data name
         self.geofilenames = {
             "dem": "dem",
             "mask": "MASK",
             "dem_proj": "dem_proj",
             "fdr_grass": "fdr_grass",
             "fdr_arcgis": "fdr_arcgis",
@@ -754,14 +880,15 @@
         mode,
         path_to_dem_input,
         watershed_outlet_coordinates = [-1, -1],
         path_to_spatial_extent_polygon="#",
         buffer_distance=0.0,
         path_to_hydrobasin_polygon="#",
         hydrobasin_id_of_watershed_outlet=-1,
+        path_to_snap_raster = "#",
         gis_platform="qgis",
     ):
 
         """This function is to define project spatial extent (PSE). Domain ouside
         of the PSE is not processed by BasinMaker functions.
 
         Parameters
@@ -824,14 +951,15 @@
             path_dem_in=path_to_dem_input,
             outlet_pt=watershed_outlet_coordinates,
             path_extent_ply=path_to_spatial_extent_polygon,
             buffer_distance=buffer_distance,
             hybasin_ply=path_to_hydrobasin_polygon,
             down_hybasin_id=hydrobasin_id_of_watershed_outlet,
             up_hybasin_id=up_hybasin_id,
+            path_to_snap_raster = path_to_snap_raster,
             mask=self.geofilenames["mask"],
             dem=self.geofilenames["dem"],
             gis_platform=gis_platform,
         )
 
     def Delineation_Initial_Subbasins_Without_Lakes(
         self,
@@ -1053,14 +1181,15 @@
             river_without_merging_lakes=self.geofilenames[
                 "river_without_merging_lakes"
             ],
             snapped_obs_points=self.geofilenames["snapped_obs_points"],
             cat_use_default_acc=self.geofilenames["cat_use_default_acc"],
             nfdr_arcgis=self.geofilenames["nfdr_arcgis"],
             nfdr_grass=self.geofilenames["nfdr_grass"],
+            fac_thresold = self.fac_thresold,
             max_memroy=max_memroy,
             grassdb=self.grassdb,
             grass_location=self.grass_location_geo,
             qgis_prefix_path=self.qgispp,
             gis_platform=gis_platform,
         )
 
@@ -1182,15 +1311,15 @@
             minimum drainage area threshold)
         sl_connected_lake.shp                           : shapefile
             the GIS layer containing the lake polygons of lakes that are connected
             by the river_without_merging_lakes.shp
         sl_non_connected_lake.shp                       : shapefile
             the GIS layer containing the lake polygons of lakes that are not connected
             by the river_without_merging_lakes.shp
-        obs_gauges                                      : shapefile
+        poi                                       : shapefile
             It is the point shapefile that represent the point of interest
             after snap to river network.
 
 
         Examples
         -------
```

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watdelineationwithoutlake.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watdelineationwithoutlake.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,31 +129,31 @@
         from basinmaker.delineationnolake.watusingdemarcgis import (
             delineate_watershed_no_lake_using_dem,
         )
         from basinmaker.delineationnolake.watusingfdrarcgis import (
             delineate_watershed_no_lake_using_fdr,
         )
     else:
-        print('gis_platform    ',gis_platform,'   do not support')    
-        
+        print('gis_platform    ',gis_platform,'   do not support')
+
     if mode == "usingdem":
         assert (
             acc_thresold > 0
         ), "the flow accumulation thresthold is needed to delineate watershed from dem"
 
     if mode == "usingfdr":
         assert (
             fdr_path != "#"
         ), "The path of the provided flow direction data is needed to delineate watershed from flow direction"
 
     if mode == "usingfac":
         assert (
             fac_path != "#"
         ), "The path of the provided flow direction data is needed to delineate watershed from flow direction"
-        
+
     if mode == "usingsubreg":
         assert (
             subreg_acc_path != "#"
         ), "subregion flow accumulation is neeeded to delineate watershed for current subregion "
 
         assert (
             subreg_fdr_path != "#"
@@ -194,31 +194,32 @@
             fdr_arcgis=fdr_arcgis,
             fdr_grass=fdr_grass,
             str_r=str_r,
             str_v=str_v,
             acc=acc,
             cat_no_lake=cat_no_lake,
             max_memroy=max_memroy,
+            fac_path=fac_path,
         )
     if mode == "usingfac":
         delineate_watershed_no_lake_using_fac(
             grassdb=grassdb,
             grass_location=grass_location,
             qgis_prefix_path=qgis_prefix_path,
             input_geo_names=input_geo_names,
             fac_path=fac_path,
             acc_thresold=acc_thresold,
             fdr_arcgis=fdr_arcgis,
-            fdr_grass=fdr_grass,            
+            fdr_grass=fdr_grass,
             str_r=str_r,
             str_v=str_v,
             acc=acc,
             cat_no_lake=cat_no_lake,
             max_memroy=max_memroy,
-        )        
+        )
     if mode == "usingsubreg":
         delineate_watershed_no_lake_using_subregion_data(
             grassdb=grassdb,
             grass_location=grass_location,
             qgis_prefix_path=qgis_prefix_path,
             input_geo_names=input_geo_names,
             subreg_fdr_path=subreg_fdr_path,
```

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingdemarcgis.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingdemqgis.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingdemqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingfacqgis.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfacqgis.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     write_grass_and_arcgis_fdr_rules(grassdb)
     print("using fac dataset     ")
     grass_raster_r_in_gdal(grass, raster_path=fac_path, output_nm="fac_in")
 
 
     # burn in DEM based on input flow accumulation raster
 
-    exp = "%s = int(%s)" % (
-        "fac_in",
-        "fac_in",
-    )
-    grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+    # exp = "%s = int(%s)" % (
+    #     "fac_in",
+    #     "fac_in",
+    # )
+    # grass.run_command("r.mapcalc", expression=exp, overwrite=True)
 
     exp = "%s = if( %s >= 1 ,-%s-1000, %s - 0*%s/%s)" % (
           "dem_acc",
           "fac_in",
           "fac_in",
           dem,
           "fac_in",
```

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingfdrarcgis.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrarcgis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,84 @@
-from basinmaker.func.arcgis import *
-from basinmaker.func.pdtable import *
-from basinmaker.func.rarray import *
-from basinmaker.utilities.utilities import *
-
-
-def delineate_watershed_no_lake_using_fdr(
-    grassdb,
-    grass_location,
-    qgis_prefix_path,
-    input_geo_names,
-    fdr_path,
-    acc_thresold,
-    fdr_arcgis,
-    fdr_grass,
-    str_r,
-    str_v,
-    acc,
-    cat_no_lake,
-    max_memroy,
-):
-    work_folder = grassdb
-    mask = input_geo_names["mask"]
-    dem = input_geo_names["dem"]
-
-    # read and define arcgis work enviroments
-    if not os.path.exists(work_folder):
-        os.makedirs(work_folder)
-    arcpy.env.workspace = work_folder
-     
-    arcpy.env.overwriteOutput = True
-    arcpy.CheckOutExtension("Spatial")
-    cellSize = float(arcpy.GetRasterProperties_management(dem+'.tif', "CELLSIZEX").getOutput(0))
-    SptailRef = arcpy.Describe(dem+'.tif').spatialReference
-    arcpy.env.XYTolerance = cellSize
-    arcpy.arcpy.env.cellSize = cellSize    
-    arcpy.env.outputCoordinateSystem = arcpy.SpatialReference(int(SptailRef.factoryCode)) ### WGS84
-    arcpy.env.extent = arcpy.Describe(dem + '.tif').extent
-    
-    
-    outFlowDirection = ExtractByMask(fdr_path, mask + ".shp")
-    dirraster = SetNull(Raster(outFlowDirection) < 1, Raster(outFlowDirection))
-    dirraster.save(fdr_arcgis + '.tif')
-
-    outFlowAccumulation = FlowAccumulation(dirraster)
-    outFlowAccumulation.save(acc + ".tif")
-
-    StreamRaster = SetNull(Raster(outFlowAccumulation) < acc_thresold, Raster(outFlowAccumulation))
-    StreamRaster = Con(StreamRaster >= 0, 1, 0)
-    StreamRaster.save("str_1.tif")
-    
-    Strlink = StreamLink(StreamRaster, dirraster)
-    Strlink.save(str_r + '.tif')
-    
-    Catchment = Watershed(dirraster,Strlink)
-
-    Catchment.save(cat_no_lake+'.tif')
-
-    StreamToFeature(Strlink, dirraster, str_v + '.shp',"NO_SIMPLIFY")
-    
-    # copyfile( OutputFolder + "/"+"dir.prj" ,  OutputFolder + "/"+"Cat1.prj")
-    # StreamToFeature(Strlink, dirraster, "DrainL1","NO_SIMPLIFY")
-    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"DrainL1.prj")
-    # arcpy.RasterToPolygon_conversion("Cat1", "Cattemp.shp", "NO_SIMPLIFY")
-    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"Cattemp.prj")
-    # arcpy.Dissolve_management("Cattemp.shp", "Cat1.shp", ["gridcode"])
-    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"Cat1.prj")
-    # arcpy.AddField_management("Cat1.shp", "COAST", "LONG",10,"","", "", "NULLABLE")
-    # arcpy.AddField_management("Cat1.shp", "HYBAS_ID", "LONG",10,"","", "", "NULLABLE")
-    # arcpy.AddField_management("Cat1.shp", "NEXT_DOWN", "LONG",10,"","", "", "NULLABLE")
-    # fieldList = ["GRID_CODE", "FROM_NODE","TO_NODE"]
-    # arcpy.JoinField_management("Cat1.shp", "gridcode", "DrainL1.shp", "GRID_CODE", fieldList)
-    # arcpy.CalculateField_management("Cat1.shp", "HYBAS_ID", '!FROM_NODE! * 1', "PYTHON")
-    # arcpy.CalculateField_management("Cat1.shp", "NEXT_DOWN", '!TO_NODE! * 1', "PYTHON")
-
-    return
+from basinmaker.func.arcgis import *
+from basinmaker.func.pdtable import *
+from basinmaker.func.rarray import *
+from basinmaker.utilities.utilities import *
+
+
+def delineate_watershed_no_lake_using_fdr(
+    grassdb,
+    grass_location,
+    qgis_prefix_path,
+    input_geo_names,
+    fdr_path,
+    acc_thresold,
+    fdr_arcgis,
+    fdr_grass,
+    str_r,
+    str_v,
+    acc,
+    cat_no_lake,
+    max_memroy,
+    fac_path,
+):
+    work_folder = grassdb
+    mask = input_geo_names["mask"]
+    dem = input_geo_names["dem"]
+
+    # read and define arcgis work enviroments
+    if not os.path.exists(work_folder):
+        os.makedirs(work_folder)
+    arcpy.env.workspace = os.path.join(work_folder,"arcgis.gdb")
+
+    arcpy.env.overwriteOutput = True
+    arcpy.CheckOutExtension("Spatial")
+    cellSize = float(arcpy.GetRasterProperties_management(dem, "CELLSIZEX").getOutput(0))
+    SptailRef = arcpy.Describe(dem).spatialReference
+    arcpy.env.XYTolerance = cellSize
+    arcpy.arcpy.env.cellSize = cellSize
+    arcpy.env.outputCoordinateSystem = arcpy.SpatialReference(int(SptailRef.factoryCode)) ### WGS84
+    arcpy.env.extent = arcpy.Describe(dem).extent
+    arcpy.env.snapRaster =  dem
+
+    outFlowDirection = ExtractByMask(fdr_path, mask)
+    dirraster = SetNull(Raster(outFlowDirection) < 1, Raster(outFlowDirection))
+    dirraster.save(fdr_arcgis)
+
+    # outFlowAccumulation= ExtractByMask(fac_path, mask)
+    # outFlowAccumulation.save("acc_to_str")
+
+    finalacc = FlowAccumulation(in_flow_direction_raster = fdr_arcgis, data_type = "INTEGER" )
+    finalacc.save(acc)
+
+    #
+    # outFlowAccumulation = FlowAccumulation(dirraster)
+    # outFlowAccumulation.save(acc)
+
+    StreamRaster = SetNull(Raster(finalacc) < acc_thresold, Raster(finalacc))
+    StreamRaster = Con(StreamRaster >= 0, 1, 0)
+    StreamRaster.save("str_1")
+
+    Strlink = StreamLink(StreamRaster, dirraster)
+    Strlink.save(str_r)
+
+    Catchment = Watershed(dirraster,Strlink)
+
+    Catchment.save(cat_no_lake)
+
+    StreamToFeature(Strlink, dirraster, str_v,"NO_SIMPLIFY")
+
+    # copyfile( OutputFolder + "/"+"dir.prj" ,  OutputFolder + "/"+"Cat1.prj")
+    # StreamToFeature(Strlink, dirraster, "DrainL1","NO_SIMPLIFY")
+    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"DrainL1.prj")
+    # arcpy.RasterToPolygon_conversion("Cat1", "Cattemp.shp", "NO_SIMPLIFY")
+    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"Cattemp.prj")
+    # arcpy.Dissolve_management("Cattemp.shp", "Cat1.shp", ["gridcode"])
+    # copyfile( OutputFolder + "/"+"HyMask.prj" ,  OutputFolder + "/"+"Cat1.prj")
+    # arcpy.AddField_management("Cat1.shp", "COAST", "LONG",10,"","", "", "NULLABLE")
+    # arcpy.AddField_management("Cat1.shp", "HYBAS_ID", "LONG",10,"","", "", "NULLABLE")
+    # arcpy.AddField_management("Cat1.shp", "NEXT_DOWN", "LONG",10,"","", "", "NULLABLE")
+    # fieldList = ["GRID_CODE", "FROM_NODE","TO_NODE"]
+    # arcpy.JoinField_management("Cat1.shp", "gridcode", "DrainL1.shp", "GRID_CODE", fieldList)
+    # arcpy.CalculateField_management("Cat1.shp", "HYBAS_ID", '!FROM_NODE! * 1', "PYTHON")
+    # arcpy.CalculateField_management("Cat1.shp", "NEXT_DOWN", '!TO_NODE! * 1', "PYTHON")
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingfdrqgis.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingfdrqgis.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,60 +15,61 @@
     fdr_arcgis,
     fdr_grass,
     str_r,
     str_v,
     acc,
     cat_no_lake,
     max_memroy,
+    fac_path
 ):
     mask = input_geo_names["mask"]
     dem = input_geo_names["dem"]
-    
+
     import grass.script as grass
     import grass.script.setup as gsetup
     from grass.pygrass.modules import Module
     from grass.pygrass.modules.shortcuts import general as g
     from grass.pygrass.modules.shortcuts import raster as r
     from grass.script import array as garray
     from grass.script import core as gcore
     from grass_session import Session
 
-    
+
     os.environ.update(
         dict(GRASS_COMPRESS_NULLS="1", GRASS_COMPRESSOR="ZSTD", GRASS_VERBOSE="1")
     )
     PERMANENT = Session()
     PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
 
     write_grass_and_arcgis_fdr_rules(grassdb)
     print("using fdr dataset     ")
     grass_raster_r_in_gdal(grass, raster_path=fdr_path, output_nm="fdr_arcgis_temp")
     # reclassify it into grass flow direction data
-    
+
     grass_raster_r_reclass(
         grass,
         input="fdr_arcgis_temp",
         output="fdr_grass_temp",
         rules=os.path.join(grassdb, "Arcgis2GrassDIR.txt"),
     )
     # calcuate flow accumulation from provided dir
-    
+
     grass.run_command(
         "r.accumulate",
         direction="fdr_grass_temp",
         accumulation=acc,
         overwrite=True,
     )
 
     exp = "%s = %s - %s/%s" % (
         'dem_acc',
         dem,
         acc,
         str(1),
-    )        
+    )
     grass.run_command("r.mapcalc", expression=exp, overwrite=True)
 
 
 
     grass.run_command(
         "r.stream.extract",
         elevation='dem_acc',
@@ -78,40 +79,40 @@
         direction=fdr_grass,
         stream_vector=str_v,
         overwrite=True,
         memory=max_memroy,
         stream_length = 10,
         d8cut = 0,
     )
-                        
+
     # create a arcgis flow direction
     grass_raster_r_reclass(
         grass,
         input=fdr_grass,
         output=fdr_arcgis,
         rules=os.path.join(grassdb, "Grass2ArcgisDIR.txt"),
     )
 
-    # update acc with new flow direction 
+    # update acc with new flow direction
     grass_raster_r_accumulate(
         grass, direction=fdr_grass, accumulation=acc
     )
-    
-    
+
+
     grass_raster_r_stream_basins(
         grass,
         direction=fdr_grass,
         stream=str_r,
         basins=cat_no_lake,
         memory=max_memroy,
     )
 
     grass.run_command(
         "r.out.gdal",
         input=cat_no_lake,
         output=os.path.join(grassdb, "catchment_no_lake.tif"),
         format="GTiff",
         overwrite=True,
-    )     
-     
+    )
+
     PERMANENT.close()
     return
```

### Comparing `basinmaker-3.0.1/basinmaker/delineationnolake/watusingsubregionddata.py` & `basinmaker-3.0.3/basinmaker/delineationnolake/watusingsubregionddata.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/extent/projectextent.py` & `basinmaker-3.0.3/basinmaker/extent/projectextent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,192 @@
-import shutil
-import os
-
-
-def define_project_extent(
-    mode,
-    path_dem_in,
-    outlet_pt=[-1, -1],
-    path_extent_ply="#",
-    buffer_distance=0.0,
-    hybasin_ply="#",
-    down_hybasin_id=-1,
-    up_hybasin_id=-1,
-    mask="MASK",
-    dem="dem",
-    grassdb="#",
-    grass_location="#",
-    qgis_prefix_path="#",
-    gis_platform="qgis",
-):
-    """Define processing extent
-
-    Function that used to define project processing spatial extent (PSE).
-    The processing spatial extent is a region where Toolbox will work in. Toolbox
-    will not process grids or features outside the processing spatial extent.
-    Several options is available here. 1) The PSE can be defined as the extent of
-    input DEM. 2)The PSE can be defined using Hybasin product and a hydrobasin
-    ID. All subbasin drainage to that hydrobasin ID will be extracted. And
-    the extent of the extracted polygon will be used as PSE. 3)The PSE
-    can be defined using DEM and an point coordinates. the drainage area
-    contribute to that point coordinate will be used as boundary polygon. 4)
-    The PSE can be defined using input polygon
-
-    Parameters
-    ----------
-    grassdb                           : path (required)
-        It is a path to project grass database folder
-    grass_location                    : string (required)
-        It is a string of grass location name
-    qgis_prefix_path                  : string (required)
-        It is a string of qgis prefix path
-    mode                              : string (required)
-        It is a string indicate which method to define project processing
-        spatial extent
-        'using_dem'            : the extent of input dem will be used
-        'using_hybasin'        : the extent will be defined using hydrobasin
-                                 product
-        'using_outlet_pt'      : the extent will be defined with provided outlet
-                                 point
-        'using_provided_ply'   : the extent will be defined by provided polygon
-    path_dem_in                      : string (required)
-        It is the path to input dem
-    outlet_pt                        : list (optional)
-        It is list that indicate the outlet coordinates of the
-        region of interest. If it is provided, the PSE
-        will be defined as the drainage area controlled by this point.
-    path_extent_ply                  : string (optional)
-        It is the path of a subregion polygon. It is only used when the Region
-        of interest is very large and the resolution of the dem is very high.
-        toolbox will first divide the whole region into several small subregions.
-        And then using devided subregion polygon as PSE.
-    buffer_distance                  : float (optional)
-        It is a float number to increase the extent of the PSE
-        obtained from Hydrobasins. It is needed when input DEM is not from
-        HydroSHEDS. Then the extent of the watershed will be different
-        with PSE defined by HydroBASINS.
-    hybasin_ply                      : string (optional)
-        It is a path to hydrobasin routing product, If it is provided, the
-        PSE will be based on the OutHyID and OutHyID2 and
-        this HydroBASINS routing product.
-    down_hybasin_id                  : int (optional)
-        It is a HydroBASINS subbasin ID, which should be the ID of the most
-        downstream subbasin in the region of interest.
-    up_hybasin_id                    : int (optional)
-        It is a HydroBASINS subbasin ID, which should be the ID of the most
-        upstream subbasin in the region of interest, normally do not needed.
-    mask                             : string (optional)
-        It is a output mask name, which will stored in grass_location in both
-        vector and raster format
-    dem                              : string (optional)
-        It is a output dem raster name, which will be stored in grass_location
-
-    Notes
-    -------
-    Outputs are following files
-
-    MASK                   : raster
-        it is a mask raster stored in grass database, which indicate
-        the PSE. The grass database is located at
-        os.path.join(grassdb, grass_location)
-    dem                   : raster
-        it is a dem raster stored in grass database, which is
-        has the same extent with MASK. The grass database is located at
-        os.path.join(grassdb, grass_location)
-
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-    """
-    shutil.rmtree(grassdb)
-    if not os.path.exists(grassdb):
-        os.makedirs(grassdb)
-
-    if gis_platform == "qgis":
-        assert (
-            grassdb != "#"
-        ), "grass database folder is needed, when gis_platform = qgis"
-        assert (
-            grass_location != "#"
-        ), "grass location name is needed, when gis_platform = qgis"
-        assert (
-            qgis_prefix_path != "#"
-        ), "qgis prefix path is needed, when gis_platform = qgis"
-        from basinmaker.extent.usingdemqgis import define_project_extent_using_dem
-        from basinmaker.extent.usingoutletpointqgis import define_project_extent_using_outlet_point
-        from basinmaker.extent.usinginputplyqgis import define_project_extent_using_input_polygon
-        from basinmaker.extent.usinghybasinplyqgis import define_project_extent_using_hybasin_ply
-    
-    if gis_platform == "arcgis":
-        from basinmaker.extent.usingdemarcgis import define_project_extent_using_dem
-        from basinmaker.extent.usinghybasinplyarcgis import define_project_extent_using_hybasin_ply
-        
-    if mode == "using_hybasin":
-        assert (
-            hybasin_ply != "#"
-        ), "HydroBasin product is needed to define processing extent with mode = using_hybasin"
-        assert (
-            down_hybasin_id != "#"
-        ), "The watershed outlet HydroBasin sub Id is needed to define processing extent with mode = using_hybasin"
-
-    if mode == "using_outlet_pt":
-        assert (
-            outlet_pt[0] != "-1"
-        ), "outlet_pt needs to be define processing extent with mode = using_outlet_pt"
-
-    if mode == "using_provided_ply":
-        assert (
-            path_extent_ply != "#"
-        ), "path_extent_ply needs to be defined when mode = using_provided_ply"
-
-    if mode == "using_dem":
-        define_project_extent_using_dem(
-            grassdb,
-            grass_location,
-            qgis_prefix_path,
-            path_dem_in,
-            mask=mask,
-            dem=dem,
-        )
-
-    if mode == "using_outlet_pt":
-        define_project_extent_using_outlet_point(
-            grassdb,
-            grass_location,
-            qgis_prefix_path,
-            path_dem_in,
-            outlet_pt,
-            buffer_distance=buffer_distance,
-            mask="MASK",
-            dem="dem",
-        )
-
-    if mode == "using_provided_ply":
-        define_project_extent_using_input_polygon(
-            grassdb,
-            grass_location,
-            qgis_prefix_path,
-            path_dem_in,
-            path_extent_ply,
-            mask="MASK",
-            dem="dem",
-        )
-
-    if mode == "using_hybasin":
-        define_project_extent_using_hybasin_ply(
-            grassdb,
-            grass_location,
-            qgis_prefix_path,
-            path_dem_in,
-            buffer_distance=buffer_distance,
-            hybasin_ply=hybasin_ply,
-            down_hybasin_id=down_hybasin_id,
-            up_hybasin_id=up_hybasin_id,
-            mask="MASK",
-            dem="dem",
-        )
+import shutil
+import os
+
+
+def define_project_extent(
+    mode,
+    path_dem_in,
+    outlet_pt=[-1, -1],
+    path_extent_ply="#",
+    buffer_distance=0.0,
+    hybasin_ply="#",
+    down_hybasin_id=-1,
+    up_hybasin_id=-1,
+    mask="MASK",
+    dem="dem",
+    path_to_snap_raster = "#",
+    grassdb="#",
+    grass_location="#",
+    qgis_prefix_path="#",
+    gis_platform="qgis",
+):
+    """Define processing extent
+
+    Function that used to define project processing spatial extent (PSE).
+    The processing spatial extent is a region where Toolbox will work in. Toolbox
+    will not process grids or features outside the processing spatial extent.
+    Several options is available here. 1) The PSE can be defined as the extent of
+    input DEM. 2)The PSE can be defined using Hybasin product and a hydrobasin
+    ID. All subbasin drainage to that hydrobasin ID will be extracted. And
+    the extent of the extracted polygon will be used as PSE. 3)The PSE
+    can be defined using DEM and an point coordinates. the drainage area
+    contribute to that point coordinate will be used as boundary polygon. 4)
+    The PSE can be defined using input polygon
+
+    Parameters
+    ----------
+    grassdb                           : path (required)
+        It is a path to project grass database folder
+    grass_location                    : string (required)
+        It is a string of grass location name
+    qgis_prefix_path                  : string (required)
+        It is a string of qgis prefix path
+    mode                              : string (required)
+        It is a string indicate which method to define project processing
+        spatial extent
+        'using_dem'            : the extent of input dem will be used
+        'using_hybasin'        : the extent will be defined using hydrobasin
+                                 product
+        'using_outlet_pt'      : the extent will be defined with provided outlet
+                                 point
+        'using_provided_ply'   : the extent will be defined by provided polygon
+    path_dem_in                      : string (required)
+        It is the path to input dem
+    outlet_pt                        : list (optional)
+        It is list that indicate the outlet coordinates of the
+        region of interest. If it is provided, the PSE
+        will be defined as the drainage area controlled by this point.
+    path_extent_ply                  : string (optional)
+        It is the path of a subregion polygon. It is only used when the Region
+        of interest is very large and the resolution of the dem is very high.
+        toolbox will first divide the whole region into several small subregions.
+        And then using devided subregion polygon as PSE.
+    buffer_distance                  : float (optional)
+        It is a float number to increase the extent of the PSE
+        obtained from Hydrobasins. It is needed when input DEM is not from
+        HydroSHEDS. Then the extent of the watershed will be different
+        with PSE defined by HydroBASINS.
+    hybasin_ply                      : string (optional)
+        It is a path to hydrobasin routing product, If it is provided, the
+        PSE will be based on the OutHyID and OutHyID2 and
+        this HydroBASINS routing product.
+    down_hybasin_id                  : int (optional)
+        It is a HydroBASINS subbasin ID, which should be the ID of the most
+        downstream subbasin in the region of interest.
+    up_hybasin_id                    : int (optional)
+        It is a HydroBASINS subbasin ID, which should be the ID of the most
+        upstream subbasin in the region of interest, normally do not needed.
+    mask                             : string (optional)
+        It is a output mask name, which will stored in grass_location in both
+        vector and raster format
+    dem                              : string (optional)
+        It is a output dem raster name, which will be stored in grass_location
+
+    Notes
+    -------
+    Outputs are following files
+
+    MASK                   : raster
+        it is a mask raster stored in grass database, which indicate
+        the PSE. The grass database is located at
+        os.path.join(grassdb, grass_location)
+    dem                   : raster
+        it is a dem raster stored in grass database, which is
+        has the same extent with MASK. The grass database is located at
+        os.path.join(grassdb, grass_location)
+
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+    """
+    shutil.rmtree(grassdb)
+    if not os.path.exists(grassdb):
+        os.makedirs(grassdb)
+
+    if gis_platform == "qgis":
+        assert (
+            grassdb != "#"
+        ), "grass database folder is needed, when gis_platform = qgis"
+        assert (
+            grass_location != "#"
+        ), "grass location name is needed, when gis_platform = qgis"
+        assert (
+            qgis_prefix_path != "#"
+        ), "qgis prefix path is needed, when gis_platform = qgis"
+        from basinmaker.extent.usingdemqgis import define_project_extent_using_dem
+        from basinmaker.extent.usingoutletpointqgis import define_project_extent_using_outlet_point
+        from basinmaker.extent.usinginputplyqgis import define_project_extent_using_input_polygon
+        from basinmaker.extent.usinghybasinplyqgis import define_project_extent_using_hybasin_ply
+
+    if gis_platform == "arcgis":
+        from basinmaker.extent.usingdemarcgis import define_project_extent_using_dem
+        from basinmaker.extent.usinghybasinplyarcgis import define_project_extent_using_hybasin_ply
+
+    if mode == "using_hybasin":
+        assert (
+            hybasin_ply != "#"
+        ), "HydroBasin product is needed to define processing extent with mode = using_hybasin"
+        assert (
+            down_hybasin_id != "#"
+        ), "The watershed outlet HydroBasin sub Id is needed to define processing extent with mode = using_hybasin"
+
+    if mode == "using_outlet_pt":
+        assert (
+            outlet_pt[0] != "-1"
+        ), "outlet_pt needs to be define processing extent with mode = using_outlet_pt"
+
+    if mode == "using_provided_ply":
+        assert (
+            path_extent_ply != "#"
+        ), "path_extent_ply needs to be defined when mode = using_provided_ply"
+
+    if mode == "using_dem":
+        define_project_extent_using_dem(
+            grassdb,
+            grass_location,
+            qgis_prefix_path,
+            path_dem_in,
+            mask=mask,
+            dem=dem,
+            path_to_snap_raster = path_to_snap_raster,
+        )
+
+    if mode == "using_outlet_pt":
+        define_project_extent_using_outlet_point(
+            grassdb,
+            grass_location,
+            qgis_prefix_path,
+            path_dem_in,
+            outlet_pt,
+            buffer_distance=buffer_distance,
+            mask="MASK",
+            dem="dem",
+        )
+
+    if mode == "using_provided_ply":
+        define_project_extent_using_input_polygon(
+            grassdb,
+            grass_location,
+            qgis_prefix_path,
+            path_dem_in,
+            path_extent_ply,
+            mask="MASK",
+            dem="dem",
+        )
+
+    if mode == "using_hybasin":
+        define_project_extent_using_hybasin_ply(
+            grassdb,
+            grass_location,
+            qgis_prefix_path,
+            path_dem_in,
+            buffer_distance=buffer_distance,
+            hybasin_ply=hybasin_ply,
+            down_hybasin_id=down_hybasin_id,
+            up_hybasin_id=up_hybasin_id,
+            mask="MASK",
+            dem="dem",
+        )
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/extent/usingdemarcgis.py` & `basinmaker-3.0.3/basinmaker/extent/usingdemarcgis.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,99 @@
-from basinmaker.func.arcgis import *
-from basinmaker.func.pdtable import *
-from basinmaker.func.rarray import *
-from basinmaker.utilities.utilities import *
-
-
-def define_project_extent_using_dem(
-    work_folder, 
-    grass_location,
-    qgis_prefix_path,
-    path_dem_in, 
-    mask="MASK", 
-    dem="dem"
-):
-
-    """Define processing extent
-
-    Function that used to define project processing spatial extent (PSE).
-    The processing spatial extent is a region where Toolbox will work in. Toolbox
-    will not process grids or features outside the processing spatial extent.
-    Several options is available here. The PSE can be defined as the extent of
-    input DEM.
-
-    Parameters
-    ----------
-    grassdb                           : path (required)
-        It is a path to project grass database folder
-    grass_location                    : string (required)
-        It is a string of grass location name
-    qgis_prefix_path                  : string (required)
-        It is a string of qgis prefix path
-    path_dem_in                      : string (required)
-        It is the path to input dem
-    mask                             : string (optional)
-        It is a output mask name, which will stored in grass_location in both
-        vector and raster format
-    dem                              : string (optional)
-        It is a output dem raster name, which will be stored in grass_location
-
-    Notes
-    -------
-    Outputs are following files
-
-    MASK                   : raster
-        it is a mask raster stored in grass database, which indicate
-        the PSE. The grass database is located at
-        os.path.join(grassdb, grass_location)
-    dem                   : raster
-        it is a dem raster stored in grass database, which is
-        has the same extent with MASK. The grass database is located at
-        os.path.join(grassdb, grass_location)
-
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-    """
-
-    print("Mask Region:   Using provided DEM : ")
-    
-    # read and define arcgis work enviroments 
-    arcpy.env.overwriteOutput = True
-    arcpy.CheckOutExtension("Spatial")
-    cellSize = float(arcpy.GetRasterProperties_management(path_dem_in, "CELLSIZEX").getOutput(0))
-    SptailRef = arcpy.Describe(path_dem_in).spatialReference
-    arcpy.env.XYTolerance = cellSize
-    arcpy.arcpy.env.cellSize = cellSize    
-    arcpy.env.outputCoordinateSystem = arcpy.SpatialReference(int(SptailRef.factoryCode)) ### WGS84
-    if not os.path.exists(work_folder):
-        os.makedirs(work_folder)
-    arcpy.env.workspace = work_folder
-    
-    # copy dem to the work fokder 
-    arcpy.CopyRaster_management(path_dem_in,dem + '.tif')
-    arcpy.env.extent = arcpy.Describe(dem + '.tif').extent
-    
-    # create mask raster 
-    mask_raster = Con(dem + '.tif', 1, 1, "VALUE >= 0")
-    mask_raster.save(mask+'.tif')
-    
-    # create mask polygon 
-    arcpy.RasterToPolygon_conversion(mask_raster, mask+'.shp', "NO_SIMPLIFY", "VALUE")
-
-    return
+from basinmaker.func.arcgis import *
+from basinmaker.func.pdtable import *
+from basinmaker.func.rarray import *
+from basinmaker.utilities.utilities import *
+
+
+def define_project_extent_using_dem(
+    work_folder,
+    grass_location,
+    qgis_prefix_path,
+    path_dem_in,
+    mask="MASK",
+    dem="dem",
+    path_to_snap_raster = "#",
+):
+
+    """Define processing extent
+
+    Function that used to define project processing spatial extent (PSE).
+    The processing spatial extent is a region where Toolbox will work in. Toolbox
+    will not process grids or features outside the processing spatial extent.
+    Several options is available here. The PSE can be defined as the extent of
+    input DEM.
+
+    Parameters
+    ----------
+    grassdb                           : path (required)
+        It is a path to project grass database folder
+    grass_location                    : string (required)
+        It is a string of grass location name
+    qgis_prefix_path                  : string (required)
+        It is a string of qgis prefix path
+    path_dem_in                      : string (required)
+        It is the path to input dem
+    mask                             : string (optional)
+        It is a output mask name, which will stored in grass_location in both
+        vector and raster format
+    dem                              : string (optional)
+        It is a output dem raster name, which will be stored in grass_location
+
+    Notes
+    -------
+    Outputs are following files
+
+    MASK                   : raster
+        it is a mask raster stored in grass database, which indicate
+        the PSE. The grass database is located at
+        os.path.join(grassdb, grass_location)
+    dem                   : raster
+        it is a dem raster stored in grass database, which is
+        has the same extent with MASK. The grass database is located at
+        os.path.join(grassdb, grass_location)
+
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+    """
+
+    print("Mask Region:   Using provided DEM : ")
+
+    # read and define arcgis work enviroments
+    arcpy.env.overwriteOutput = True
+    arcpy.CheckOutExtension("Spatial")
+    cellSize = float(arcpy.GetRasterProperties_management(path_dem_in, "CELLSIZEX").getOutput(0))
+    extent = arcpy.Describe(path_dem_in).extent
+    SptailRef = arcpy.Describe(path_dem_in).spatialReference
+    arcgis_env = {
+        "extent":extent,
+        "georef":arcpy.SpatialReference(int(SptailRef.factoryCode)),
+        "cellSize":cellSize,
+        }
+    if not os.path.exists(work_folder):
+        os.makedirs(work_folder)
+    arcpy.CreateFileGDB_management(work_folder, "arcgis.gdb")
+
+    
+    arcpy.env.XYTolerance = arcgis_env["cellSize"]
+    arcpy.arcpy.env.cellSize = arcgis_env["cellSize"]
+    arcpy.env.outputCoordinateSystem = arcgis_env["georef"] ### WGS84
+    arcpy.env.extent = arcgis_env["extent"]
+    arcpy.env.workspace = os.path.join(work_folder,"arcgis.gdb")
+
+    if path_to_snap_raster != "#":
+        arcpy.env.snapRaster =  path_to_snap_raster
+
+    # copy dem to the work fokder
+    arcpy.CopyRaster_management(path_dem_in,dem )
+    arcpy.env.extent = arcpy.Describe(dem).extent
+
+    # create mask raster
+    mask_raster = Con(dem, 1, 1, "VALUE >= 0")
+    mask_raster.save(mask)
+    # create mask polygon
+    arcpy.RasterToPolygon_conversion(mask_raster, mask+'_ply', "NO_SIMPLIFY", "VALUE")
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/extent/usingdemqgis.py` & `basinmaker-3.0.3/basinmaker/extent/usingdemqgis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-from basinmaker.func.grassgis import *
-from basinmaker.func.qgis import *
-from basinmaker.func.pdtable import *
-from basinmaker.func.rarray import *
-from basinmaker.utilities.utilities import *
-
-
-def define_project_extent_using_dem(
-    grassdb, grass_location, qgis_prefix_path, path_dem_in, mask="MASK", dem="dem"
-):
-
-    """Define processing extent
-
-    Function that used to define project processing spatial extent (PSE).
-    The processing spatial extent is a region where Toolbox will work in. Toolbox
-    will not process grids or features outside the processing spatial extent.
-    Several options is available here. The PSE can be defined as the extent of
-    input DEM.
-
-    Parameters
-    ----------
-    grassdb                           : path (required)
-        It is a path to project grass database folder
-    grass_location                    : string (required)
-        It is a string of grass location name
-    qgis_prefix_path                  : string (required)
-        It is a string of qgis prefix path
-    path_dem_in                      : string (required)
-        It is the path to input dem
-    mask                             : string (optional)
-        It is a output mask name, which will stored in grass_location in both
-        vector and raster format
-    dem                              : string (optional)
-        It is a output dem raster name, which will be stored in grass_location
-
-    Notes
-    -------
-    Outputs are following files
-
-    MASK                   : raster
-        it is a mask raster stored in grass database, which indicate
-        the PSE. The grass database is located at
-        os.path.join(grassdb, grass_location)
-    dem                   : raster
-        it is a dem raster stored in grass database, which is
-        has the same extent with MASK. The grass database is located at
-        os.path.join(grassdb, grass_location)
-
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-    """
-
-    print("Mask Region:   Using provided DEM : ")
-
-    QgsApplication.setPrefixPath(qgis_prefix_path, True)
-    Qgs = QgsApplication([], False)
-    Qgs.initQgis()
-    from processing.core.Processing import Processing
-    from processing.tools import dataobjects
-    from qgis import processing
-
-    feedback = QgsProcessingFeedback()
-    Processing.initialize()
-    QgsApplication.processingRegistry().addProvider(QgsNativeAlgorithms())
-    context = dataobjects.createContext()
-    context.setInvalidGeometryCheck(QgsFeatureRequest.GeometryNoCheck)
-
-    import grass.script as grass
-    import grass.script.setup as gsetup
-    from grass.pygrass.modules import Module
-    from grass.pygrass.modules.shortcuts import general as g
-    from grass.pygrass.modules.shortcuts import raster as r
-    from grass.script import array as garray
-    from grass.script import core as gcore
-    from grass_session import Session
-
-    os.environ.update(
-        dict(
-            GRASS_COMPRESS_NULLS="1",
-            GRASS_COMPRESSOR="ZSTD",
-            GRASS_VERBOSE="1",
-        )
-    )
-    PERMANENT = Session()
-    PERMANENT.open(
-        gisdb=grassdb,
-        location=grass_location + "t1",
-        create_opts="EPSG:4326",
-    )
-
-    # load dem raster to target location
-    grass_raster_r_in_gdal(
-        grass=grass,
-        raster_path=path_dem_in,
-        output_nm=dem,
-        location=grass_location,
-    )
-    PERMANENT.close()
-
-    PERMANENT = Session()
-    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
-
-    exp = "%s = %s/%s" % (
-        dem,
-        dem,
-        str(1),
-    )        
-    grass.run_command("r.mapcalc", expression=exp, overwrite=True)
-    
-    # define mask of current working enviroments
-    grass_raster_r_mask(grass, dem)
-    # define processing extent of the current working enviroment
-    grass_raster_g_region(grass, dem)
-
-    # export generated mask to folder ouside grass work env in
-    # tif format
-    grass_raster_r_out_gdal(
-        grass,
-        input_nm="MASK",
-        output=os.path.join(grassdb, mask + ".tif"),
-        format="GTiff",
-    )
-    # polygonize exported mask raster, and polygonize and dissove it.
-    qgis_raster_gdal_polygonize(
-        processing,
-        context,
-        INPUT=os.path.join(grassdb, mask + ".tif"),
-        OUTPUT=os.path.join(grassdb, mask + "_t1.shp"),
-    )
-    # qgis dissolve function for some reason not working here....
-    qgis_vector_dissolve(
-        processing,
-        context,
-        INPUT=os.path.join(grassdb, mask + "_t1.shp"),
-        FIELD="DN",
-        OUTPUT=os.path.join(grassdb, mask + ".shp"),
-        USING_GDAL_FUNCTION=True,
-    )
-    PERMANENT.close()
-
-    Qgs.exit()
-
-    return
+from basinmaker.func.grassgis import *
+from basinmaker.func.qgis import *
+from basinmaker.func.pdtable import *
+from basinmaker.func.rarray import *
+from basinmaker.utilities.utilities import *
+
+
+def define_project_extent_using_dem(
+    grassdb, grass_location, qgis_prefix_path, path_dem_in, mask="MASK", dem="dem",path_to_snap_raster="#",
+):
+
+    """Define processing extent
+
+    Function that used to define project processing spatial extent (PSE).
+    The processing spatial extent is a region where Toolbox will work in. Toolbox
+    will not process grids or features outside the processing spatial extent.
+    Several options is available here. The PSE can be defined as the extent of
+    input DEM.
+
+    Parameters
+    ----------
+    grassdb                           : path (required)
+        It is a path to project grass database folder
+    grass_location                    : string (required)
+        It is a string of grass location name
+    qgis_prefix_path                  : string (required)
+        It is a string of qgis prefix path
+    path_dem_in                      : string (required)
+        It is the path to input dem
+    mask                             : string (optional)
+        It is a output mask name, which will stored in grass_location in both
+        vector and raster format
+    dem                              : string (optional)
+        It is a output dem raster name, which will be stored in grass_location
+
+    Notes
+    -------
+    Outputs are following files
+
+    MASK                   : raster
+        it is a mask raster stored in grass database, which indicate
+        the PSE. The grass database is located at
+        os.path.join(grassdb, grass_location)
+    dem                   : raster
+        it is a dem raster stored in grass database, which is
+        has the same extent with MASK. The grass database is located at
+        os.path.join(grassdb, grass_location)
+
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+    """
+
+    print("Mask Region:   Using provided DEM : ")
+
+    QgsApplication.setPrefixPath(qgis_prefix_path, True)
+    Qgs = QgsApplication([], False)
+    Qgs.initQgis()
+    from processing.core.Processing import Processing
+    from processing.tools import dataobjects
+    from qgis import processing
+
+    feedback = QgsProcessingFeedback()
+    Processing.initialize()
+    QgsApplication.processingRegistry().addProvider(QgsNativeAlgorithms())
+    context = dataobjects.createContext()
+    context.setInvalidGeometryCheck(QgsFeatureRequest.GeometryNoCheck)
+
+    import grass.script as grass
+    import grass.script.setup as gsetup
+    from grass.pygrass.modules import Module
+    from grass.pygrass.modules.shortcuts import general as g
+    from grass.pygrass.modules.shortcuts import raster as r
+    from grass.script import array as garray
+    from grass.script import core as gcore
+    from grass_session import Session
+
+    os.environ.update(
+        dict(
+            GRASS_COMPRESS_NULLS="1",
+            GRASS_COMPRESSOR="ZSTD",
+            GRASS_VERBOSE="1",
+        )
+    )
+    PERMANENT = Session()
+    PERMANENT.open(
+        gisdb=grassdb,
+        location=grass_location + "t1",
+        create_opts="EPSG:4326",
+    )
+
+    # load dem raster to target location
+    grass_raster_r_in_gdal(
+        grass=grass,
+        raster_path=path_dem_in,
+        output_nm=dem,
+        location=grass_location,
+    )
+    PERMANENT.close()
+
+    PERMANENT = Session()
+    PERMANENT.open(gisdb=grassdb, location=grass_location, create_opts="")
+
+    exp = "%s = %s/%s" % (
+        dem,
+        dem,
+        str(1),
+    )
+    grass.run_command("r.mapcalc", expression=exp, overwrite=True)
+
+    # define mask of current working enviroments
+    grass_raster_r_mask(grass, dem)
+    # define processing extent of the current working enviroment
+    grass_raster_g_region(grass, dem)
+
+    # export generated mask to folder ouside grass work env in
+    # tif format
+    grass_raster_r_out_gdal(
+        grass,
+        input_nm="MASK",
+        output=os.path.join(grassdb, mask + ".tif"),
+        format="GTiff",
+    )
+    # polygonize exported mask raster, and polygonize and dissove it.
+    qgis_raster_gdal_polygonize(
+        processing,
+        context,
+        INPUT=os.path.join(grassdb, mask + ".tif"),
+        OUTPUT=os.path.join(grassdb, mask + "_t1.shp"),
+    )
+    # qgis dissolve function for some reason not working here....
+    qgis_vector_dissolve(
+        processing,
+        context,
+        INPUT=os.path.join(grassdb, mask + "_t1.shp"),
+        FIELD="DN",
+        OUTPUT=os.path.join(grassdb, mask + ".shp"),
+        USING_GDAL_FUNCTION=True,
+    )
+    PERMANENT.close()
+
+    Qgs.exit()
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/extent/usinghybasinplyarcgis.py` & `basinmaker-3.0.3/basinmaker/extent/usinghybasinplyarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/extent/usinghybasinplyqgis.py` & `basinmaker-3.0.3/basinmaker/extent/usinghybasinplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/extent/usinginputplyqgis.py` & `basinmaker-3.0.3/basinmaker/extent/usinginputplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/extent/usingoutletpointqgis.py` & `basinmaker-3.0.3/basinmaker/extent/usingoutletpointqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/fgdal.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/fgdal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/grassgis.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/grassgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/pdtable.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/pdtable.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Nov  2 00:12:18 2022 UTC, .py size: 133734 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,2844 +1,2988 @@
-00000000: 610d 0d0a 0000 0000 e2b5 6163 660a 0200  a.........acf...
+00000000: 610d 0d0a 0000 0000 cb33 2864 aa22 0200  a........3(d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 7401 0000 6400  .....@...st...d.
+00000020: 0006 0000 0040 0000 0073 9601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 5400 6400 6401 6c08  ..d.d.l.T.d.d.l.
 00000060: 5a08 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  Z.d.d.l.m.Z.m.Z.
-00000070: 0100 6400 6401 6c0c 5a0c 6405 6406 8400  ..d.d.l.Z.d.d...
-00000080: 5a0d 6407 6408 8400 5a0e 6409 640a 8400  Z.d.d...Z.d.d...
-00000090: 5a0f 640b 640c 8400 5a10 640d 640e 8400  Z.d.d...Z.d.d...
-000000a0: 5a11 644b 6410 6411 8401 5a12 6412 6412  Z.dKd.d...Z.d.d.
-000000b0: 6412 6701 6412 6701 6412 6412 6606 6413  d.g.d.g.d.d.f.d.
-000000c0: 6414 8401 5a13 644c 6416 6417 8401 5a14  d...Z.dLd.d...Z.
-000000d0: 644d 6418 6419 8401 5a15 641a 641b 8400  dMd.d...Z.d.d...
-000000e0: 5a16 641c 641d 8400 5a17 641e 641f 8400  Z.d.d...Z.d.d...
-000000f0: 5a18 6420 6421 8400 5a19 6422 6423 8400  Z.d d!..Z.d"d#..
-00000100: 5a1a 6424 6425 8400 5a1b 6426 6427 8400  Z.d$d%..Z.d&d'..
-00000110: 5a1c 6428 6429 8400 5a1d 642a 642b 8400  Z.d(d)..Z.d*d+..
-00000120: 5a1e 642c 642d 8400 5a1f 642e 642f 8400  Z.d,d-..Z.d.d/..
-00000130: 5a20 6430 6431 8400 5a21 6432 6433 8400  Z d0d1..Z!d2d3..
-00000140: 5a22 6434 6435 8400 5a23 6436 6437 8400  Z"d4d5..Z#d6d7..
-00000150: 5a24 6438 6439 8400 5a25 643a 643b 8400  Z$d8d9..Z%d:d;..
-00000160: 5a26 644e 643c 643d 8401 5a27 643e 643f  Z&dNd<d=..Z'd>d?
-00000170: 8400 5a28 6440 6441 8400 5a29 6442 6443  ..Z(d@dA..Z)dBdC
-00000180: 8400 5a2a 644f 6445 6446 8401 5a2b 6447  ..Z*dOdEdF..Z+dG
-00000190: 6448 8400 5a2c 6449 644a 8400 5a2d 6401  dH..Z,dIdJ..Z-d.
-000001a0: 5300 2950 e900 0000 004e 2901 da09 6375  S.)P.....N)...cu
-000001b0: 7276 655f 6669 7429 01da 012a 2902 da08  rve_fit)...*)...
-000001c0: 5061 7261 6c6c 656c da07 6465 6c61 7965  Parallel..delaye
-000001d0: 6463 0400 0000 0000 0000 0000 0000 0d00  dc..............
-000001e0: 0000 0500 0000 4300 0000 7334 0100 007c  ......C...s4...|
-000001f0: 0064 016b 0172 0c7c 0153 007c 0164 027c  .d.k.r.|.S.|.d.|
-00000200: 0364 0367 0319 006a 0064 0464 058d 017d  .d.g...j.d.d...}
-00000210: 047c 046a 0164 0364 0669 0164 078d 017d  .|.j.d.d.i.d...}
-00000220: 047c 046a 0264 027c 0367 0264 0864 098d  .|.j.d.|.g.d.d..
-00000230: 02a0 03a1 007d 0474 046a 057c 047c 0264  .....}.t.j.|.|.d
-00000240: 0264 0a8d 037d 047c 0464 0619 007c 0464  .d...}.|.d...|.d
-00000250: 0b19 001b 007c 0464 0c3c 007c 046a 0664  .....|.d.<.|.j.d
-00000260: 0264 0667 0264 0864 0d8d 027d 047c 046a  .d.g.d.d...}.|.j
-00000270: 0764 0267 0164 0e64 0f8d 026a 0064 0464  .d.g.d.d...j.d.d
-00000280: 058d 017d 057c 047c 0464 0c19 007c 006b  ...}.|.|.d...|.k
-00000290: 0019 0064 027c 0367 0219 006a 0064 0464  ...d.|.g...j.d.d
-000002a0: 058d 017d 0674 0864 0174 097c 0683 0183  ...}.t.d.t.|....
-000002b0: 0244 005d 6a7d 077c 0664 0219 006a 0a7c  .D.]j}.|.d...j.|
-000002c0: 0719 007d 087c 067c 0319 006a 0a7c 0719  ...}.|.|...j.|..
-000002d0: 007d 097c 0164 0219 007c 086b 027d 0a7c  .}.|.d...|.k.}.|
-000002e0: 017c 0319 007c 096b 027d 0b74 0ba0 0c7c  .|...|.k.}.t...|
-000002f0: 0a7c 0ba1 027d 0c7c 056a 0d7c 0564 0219  .|...}.|.j.|.d..
-00000300: 007c 086b 0219 007c 0319 006a 0a64 0119  .|.k...|...j.d..
-00000310: 007c 016a 0d7c 0c7c 0366 023c 0071 c47c  .|.j.|.|.f.<.q.|
-00000320: 0153 0029 104e 7201 0000 00da 0553 7562  .S.).Nr......Sub
-00000330: 4964 da08 4852 555f 4172 6561 54a9 01da  Id..HRU_AreaT...
-00000340: 0464 6565 705a 0949 6e70 7574 5f41 5f47  .deepZ.Input_A_G
-00000350: a901 da07 636f 6c75 6d6e 7346 a901 da08  ....columnsF....
-00000360: 6173 5f69 6e64 6578 2901 da02 6f6e da07  as_index)...on..
-00000370: 4261 735f 415f 475a 0a41 7265 615f 7261  Bas_A_GZ.Area_ra
-00000380: 7469 6fa9 02da 0262 79da 0961 7363 656e  tio....by..ascen
-00000390: 6469 6e67 da05 6669 7273 7429 02da 0673  ding..first)...s
-000003a0: 7562 7365 74da 046b 6565 7029 0eda 0463  ubset..keep)...c
-000003b0: 6f70 79da 0672 656e 616d 65da 0767 726f  opy..rename..gro
-000003c0: 7570 6279 da03 7375 6dda 0270 64da 056d  upby..sum..pd..m
-000003d0: 6572 6765 da0b 736f 7274 5f76 616c 7565  erge..sort_value
-000003e0: 73da 0f64 726f 705f 6475 706c 6963 6174  s..drop_duplicat
-000003f0: 6573 da05 7261 6e67 65da 036c 656e da06  es..range..len..
-00000400: 7661 6c75 6573 da02 6e70 da0b 6c6f 6769  values..np..logi
-00000410: 6361 6c5f 616e 64da 036c 6f63 290d da0d  cal_and..loc)...
-00000420: 6c61 6e64 7573 655f 7468 7265 73da 0768  landuse_thres..h
-00000430: 7275 696e 666f da08 7375 625f 6172 6561  ruinfo..sub_area
-00000440: da0a 4c61 6e64 7573 655f 4944 5a0a 7375  ..Landuse_IDZ.su
-00000450: 6269 6e66 6f5f 6c75 5a14 7375 6269 6e66  binfo_luZ.subinf
-00000460: 6f5f 6c75 5f64 6f6d 696e 6174 6564 5a16  o_lu_dominatedZ.
-00000470: 7375 6269 6e66 6f5f 6c75 5f6e 6565 645f  subinfo_lu_need_
-00000480: 6368 616e 6765 da01 69da 0573 7562 6964  change..i..subid
-00000490: 5a07 6c61 6e64 7573 65da 056d 6173 6b31  Z.landuse..mask1
-000004a0: da05 6d61 736b 32da 046d 6173 6ba9 0072  ..mask2..mask..r
-000004b0: 2d00 0000 fa48 633a 5c75 7365 7273 5c6d  -....Hc:\users\m
-000004c0: 3433 6861 6e5f 325c 646f 6375 6d65 6e74  43han_2\document
-000004d0: 735c 6769 7468 7562 5c62 6173 696e 6d61  s\github\basinma
-000004e0: 6b65 725c 6261 7369 6e6d 616b 6572 5c66  ker\basinmaker\f
-000004f0: 756e 635c 7064 7461 626c 652e 7079 da27  unc\pdtable.py.'
-00000500: 7265 6d6f 7665 5f6c 616e 6475 7365 5f74  remove_landuse_t
-00000510: 7970 655f 696e 7075 745f 6261 7365 645f  ype_input_based_
-00000520: 6f6e 5f61 7265 610b 0000 0073 2400 0000  on_area....s$...
-00000530: 0002 0801 0402 1601 1001 1603 1001 1403  ................
-00000540: 1201 1803 2002 1201 0e01 0e01 0c01 0c01  .... ...........
-00000550: 0c01 2802 722f 0000 0063 0700 0000 0000  ..(.r/...c......
-00000560: 0000 0000 0000 0e00 0000 0600 0000 4300  ..............C.
-00000570: 0000 73c2 0000 007c 016a 007c 0164 0119  ..s....|.j.|.d..
-00000580: 0064 026b 0419 00a0 01a1 007d 077c 016a  .d.k.......}.|.j
-00000590: 007c 0164 0119 0064 026b 0119 00a0 01a1  .|.d...d.k......
-000005a0: 007d 087c 0164 0364 0467 0219 006a 0164  .}.|.d.d.g...j.d
-000005b0: 0564 068d 017d 097c 096a 0264 0464 0769  .d...}.|.j.d.d.i
-000005c0: 0164 088d 017d 097c 096a 0364 0367 0164  .d...}.|.j.d.g.d
-000005d0: 0964 0a8d 02a0 04a1 007d 097c 0064 0219  .d.......}.|.d..
-000005e0: 007d 0a7c 027c 037c 0567 037d 0b74 0564  .}.|.|.|.g.}.t.d
-000005f0: 0274 067c 0b83 0183 0244 005d 227d 0c7c  .t.|.....D.]"}.|
-00000600: 0b7c 0c19 007d 0d7c 007c 0c19 007d 0a74  .|...}.|.|...}.t
-00000610: 077c 0a7c 087c 097c 0d83 047d 0871 847c  .|.|.|.|...}.q.|
-00000620: 087c 0219 007c 087c 043c 007c 07a0 087c  .|...|.|.<.|...|
-00000630: 08a1 017d 017c 0153 0029 0b4e da0a 4852  ...}.|.S.).N..HR
-00000640: 555f 4973 4c61 6b65 7201 0000 0072 0600  U_IsLaker....r..
-00000650: 0000 7207 0000 0054 7208 0000 0072 0f00  ..r....Tr....r..
-00000660: 0000 720a 0000 0046 720c 0000 0029 0972  ..r....Fr....).r
-00000670: 2300 0000 7216 0000 0072 1700 0000 7218  #...r....r....r.
-00000680: 0000 0072 1900 0000 721e 0000 0072 1f00  ...r....r....r..
-00000690: 0000 722f 0000 00da 0661 7070 656e 6429  ..r/.....append)
-000006a0: 0eda 1561 7265 615f 7261 7469 6f5f 7468  ...area_ratio_th
-000006b0: 7265 7368 6f6c 6473 7225 0000 0072 2700  resholdsr%...r'.
-000006c0: 0000 da07 536f 696c 5f49 44da 0656 6567  ....Soil_ID..Veg
-000006d0: 5f49 44da 0e4f 7468 6572 5f50 6c79 5f49  _ID..Other_Ply_I
-000006e0: 445f 31da 0e4f 7468 6572 5f50 6c79 5f49  D_1..Other_Ply_I
-000006f0: 445f 325a 0d68 7275 5f6c 616b 655f 696e  D_2Z.hru_lake_in
-00000700: 666f 5a0d 6872 755f 6c61 6e64 5f69 6e66  foZ.hru_land_inf
-00000710: 6f72 2600 0000 7224 0000 00da 046c 6973  or&...r$.....lis
-00000720: 7472 2800 0000 da04 4974 656d 722d 0000  tr(.....Itemr-..
-00000730: 0072 2d00 0000 722e 0000 00da 1573 696d  .r-...r......sim
-00000740: 706c 6966 795f 6872 7573 5f6d 6574 686f  plify_hrus_metho
-00000750: 6432 2900 0000 731c 0000 0000 0316 0116  d2)...s.........
-00000760: 0214 0110 0114 0308 010a 0112 0108 0108  ................
-00000770: 0110 010c 020a 0272 3900 0000 6303 0000  .......r9...c...
-00000780: 0000 0000 0000 0000 001d 0000 0009 0000  ................
-00000790: 0043 0000 0073 8e02 0000 7c01 6401 1900  .C...s....|.d...
-000007a0: 7c01 6402 3c00 7400 a001 7c01 6403 1900  |.d.<.t...|.d...
-000007b0: 6a02 a101 7d03 7403 6404 7404 7c03 8301  j...}.t.d.t.|...
-000007c0: 8302 4400 9002 5d4e 7d04 7c03 7c04 1900  ..D...]N}.|.|...
-000007d0: 7d05 7c01 6a05 7c01 6403 1900 7c05 6b02  }.|.j.|.d...|.k.
-000007e0: 1900 6a06 6405 6406 8d01 7d06 7400 a007  ..j.d.d...}.t...
-000007f0: 7c06 6407 1900 6a02 a101 7d07 7c00 7c07  |.d...j...}.|.|.
-00000800: 1400 7d08 7c06 6a05 7c06 6407 1900 7c08  ..}.|.j.|.d...|.
-00000810: 6b00 1900 a006 a100 7d09 7c06 6a05 7c06  k.......}.|.j.|.
-00000820: 6407 1900 7c08 6b05 1900 a006 a100 7d0a  d...|.k.......}.
-00000830: 7c0a 6a08 7d0b 7c0b 7c0b 6402 6b03 1900  |.j.}.|.|.d.k...
-00000840: 7d0b 7c02 6404 1900 7d0c 7c09 6a06 6405  }.|.d...}.|.j.d.
-00000850: 6406 8d01 7d0d 7400 a001 7c0d 7c0c 1900  d...}.t...|.|...
-00000860: 6a02 a101 7d0e 7403 6404 7404 7c0e 8301  j...}.t.d.t.|...
-00000870: 8302 4400 5dbc 7d0f 7c0e 7c0f 1900 7d10  ..D.].}.|.|...}.
-00000880: 7c0d 6a05 7c0d 7c0c 1900 7c10 6b02 1900  |.j.|.|...|.k...
-00000890: 6a06 6405 6406 8d01 7d11 7400 a007 7c11  j.d.d...}.t...|.
-000008a0: 6407 1900 6a02 a101 7d12 7c12 7c08 6b05  d...j...}.|.|.k.
-000008b0: 72da 7c11 6a09 6407 6701 6408 6409 8d02  r.|.j.d.g.d.d...
-000008c0: 7d11 7403 6404 7404 7c0b 8301 8302 4400  }.t.d.t.|.....D.
-000008d0: 5d44 7d13 7c0b 7c13 1900 7d14 7c14 640a  ]D}.|.|...}.|.d.
-000008e0: 6b02 9001 7250 9001 7136 7c11 7c14 1900  k...rP..q6|.|...
-000008f0: 6a02 6404 1900 7c01 6a05 7c01 6402 1900  j.d...|.j.|.d...
-00000900: a00a 7c11 6402 1900 6a02 a101 7c14 6602  ..|.d...j...|.f.
-00000910: 3c00 9001 7136 7c09 7c09 6402 1900 a00a  <...q6|.|.d.....
-00000920: 7c11 6402 1900 6a02 a101 0f00 1900 7d09  |.d...j.......}.
-00000930: 71da 7c09 6a0b 7d15 7403 6404 7404 7c15  q.|.j.}.t.d.t.|.
-00000940: 8301 8302 4400 5dcc 7d16 7c15 7c16 1900  ....D.].}.|.|...
-00000950: 7d17 7c09 6a05 7c17 6402 6602 1900 7d18  }.|.j.|.d.f...}.
-00000960: 7403 6404 7404 7c02 8301 8302 4400 5da0  t.d.t.|.....D.].
-00000970: 7d19 7c02 7c19 1900 7d1a 7c09 6a05 7c17  }.|.|...}.|.j.|.
-00000980: 7c1a 6602 1900 7d1b 7c0a 6a05 7c0a 7c1a  |.f...}.|.j.|.|.
-00000990: 1900 7c1b 6b02 1900 a006 a100 7d1c 7404  ..|.k.......}.t.
-000009a0: 7c1c 8301 6404 6b04 9001 72d4 7c1c 6a09  |...d.k...r.|.j.
-000009b0: 6407 6408 6409 8d02 7d1c 7403 6404 7404  d.d.d...}.t.d.t.
-000009c0: 7c0b 8301 8302 4400 5d3c 7d13 7c0b 7c13  |.....D.]<}.|.|.
-000009d0: 1900 7d14 7c14 640a 6b02 9002 7248 9002  ..}.|.d.k...rH..
-000009e0: 712e 7c1c 7c14 1900 6a02 6404 1900 7c01  q.|.|...j.d...|.
-000009f0: 6a05 7c01 6402 1900 7c18 6b02 7c14 6602  j.|.d...|.k.|.f.
-00000a00: 3c00 9002 712e 6e04 9001 71d4 9001 71d4  <...q.n...q...q.
-00000a10: 9001 71ac 712a 7c01 6a0c 6402 6701 640b  ..q.q*|.j.d.g.d.
-00000a20: 8d01 7d01 7c01 5300 290c 4eda 0a48 5255  ..}.|.S.).N..HRU
-00000a30: 5f49 445f 4e65 775a 0b48 5255 5f49 445f  _ID_NewZ.HRU_ID_
-00000a40: 4e65 7732 7206 0000 0072 0100 0000 5472  New2r....r....Tr
-00000a50: 0800 0000 7207 0000 0046 7210 0000 00da  ....r....Fr.....
-00000a60: 0553 4841 5045 720a 0000 0029 0d72 2100  .SHAPEr....).r!.
-00000a70: 0000 da06 756e 6971 7565 7220 0000 0072  ....uniquer ...r
-00000a80: 1e00 0000 721f 0000 0072 2300 0000 7216  ....r....r#...r.
-00000a90: 0000 0072 1900 0000 720b 0000 0072 1c00  ...r....r....r..
-00000aa0: 0000 da04 6973 696e da05 696e 6465 78da  ....isin..index.
-00000ab0: 0464 726f 7029 1dda 146d 696e 5f68 7275  .drop)...min_hru
-00000ac0: 5f70 6374 5f73 7562 5f61 7265 6172 2500  _pct_sub_arear%.
-00000ad0: 0000 da10 696d 706f 7274 616e 6365 5f6f  ....importance_o
-00000ae0: 7264 6572 da06 7375 6269 6473 7228 0000  rder..subidsr(..
-00000af0: 0072 2900 0000 5a0c 7375 625f 6872 755f  .r)...Z.sub_hru_
-00000b00: 696e 666f 5a08 7375 6261 7372 6561 5a0c  infoZ.subasreaZ.
-00000b10: 7375 6261 7265 615f 7468 7273 5a10 6e65  subarea_thrsZ.ne
-00000b20: 6564 5f72 656d 6f76 655f 6872 7573 5a09  ed_remove_hrusZ.
-00000b30: 676f 6f64 5f68 7275 735a 0b68 7275 5f63  good_hrusZ.hru_c
-00000b40: 6f6c 756d 6e73 5a06 636f 6c6e 6d31 5a1c  olumnsZ.colnm1Z.
-00000b50: 696d 706f 7274 315f 4172 6561 5f6e 6565  import1_Area_nee
-00000b60: 645f 7265 6d6f 7665 5f68 7275 5a0e 756e  d_remove_hruZ.un
-00000b70: 6971 7565 5f69 6d70 6f72 7431 5a08 695f  ique_import1Z.i_
-00000b80: 696d 706f 7274 5a08 695f 636f 6c6e 6d31  importZ.i_colnm1
-00000b90: 5a1e 695f 696d 706f 7274 315f 4172 6561  Z.i_import1_Area
-00000ba0: 5f6e 6565 645f 7265 6d6f 7665 5f68 7275  _need_remove_hru
-00000bb0: 5a27 746f 7461 6c5f 6172 6561 5f69 5f69  Z'total_area_i_i
-00000bc0: 6d70 6f72 745f 696e 5f6e 6565 645f 7265  mport_in_need_re
-00000bd0: 6d6f 7665 5f68 7275 735a 0469 5f6e 6d5a  move_hrusZ.i_nmZ
-00000be0: 0a63 6f6c 756d 6e6e 616d 65da 0769 6e64  .columnname..ind
-00000bf0: 6578 6573 da01 6ada 0369 6478 da05 6872  exes..j..idx..hr
-00000c00: 7569 64da 016b 5a05 636f 6c6e 6d5a 1061  uid..kZ.colnmZ.a
-00000c10: 7474 7269 5f72 656d 6f76 655f 6872 755a  ttri_remove_hruZ
-00000c20: 0b67 6f6f 645f 6872 7573 5f6b 722d 0000  .good_hrus_kr-..
-00000c30: 0072 2d00 0000 722e 0000 00da 0e73 696d  .r-...r......sim
-00000c40: 706c 6964 6679 5f68 7275 7342 0000 0073  plidfy_hrusB...s
-00000c50: 5800 0000 0002 0c02 1003 1401 0802 1a02  X...............
-00000c60: 1001 0803 1602 1602 0602 0c03 0801 0c01  ................
-00000c70: 1005 1201 0801 1a01 1005 0803 1001 1201  ................
-00000c80: 0801 0a01 0402 2c03 1c02 0604 1201 0801  ......,.........
-00000c90: 0e04 1201 0802 0e03 1602 0e02 0e01 1201  ................
-00000ca0: 0801 0a01 0402 2602 0e01 0e01 7248 0000  ......&.....rH..
-00000cb0: 0063 0100 0000 0000 0000 0000 0000 0a00  .c..............
-00000cc0: 0000 0500 0000 4300 0000 733e 0200 007c  ......C...s>...|
-00000cd0: 0064 0164 0267 0219 00a0 0064 03a1 016a  .d.d.g.....d...j
-00000ce0: 017d 017c 006a 027c 0064 0419 0064 056b  .}.|.j.|.d...d.k
-00000cf0: 0219 00a0 03a1 007d 027c 0264 0119 00a0  .......}.|.d....
-00000d00: 03a1 007d 0364 067c 006a 027c 0064 0119  ...}.d.|.j.|.d..
-00000d10: 00a0 047c 03a1 0164 0766 023c 0074 0564  ...|...d.f.<.t.d
-00000d20: 0874 067c 0283 0183 0244 0090 015d da7d  .t.|.....D...].}
-00000d30: 047c 0264 0119 006a 017c 0419 007d 057c  .|.d...j.|...}.|
-00000d40: 0264 0219 006a 017c 0419 007d 067c 006a  .d...j.|...}.|.j
-00000d50: 027c 0064 0119 007c 066b 0219 00a0 03a1  .|.d...|.k......
-00000d60: 007d 077c 067d 0874 067c 0783 0164 096b  .}.|.}.t.|...d.k
-00000d70: 0072 a671 5c7c 0764 0419 006a 0164 0819  .r.q\|.d...j.d..
-00000d80: 0064 056b 0290 0172 107c 006a 027c 0064  .d.k...r.|.j.|.d
-00000d90: 0119 007c 086b 0219 00a0 03a1 007d 097c  ...|.k.......}.|
-00000da0: 0964 0219 006a 0164 0819 007d 067c 006a  .d...j.d...}.|.j
-00000db0: 027c 0064 0119 007c 066b 0219 00a0 03a1  .|.d...|.k......
-00000dc0: 007d 0774 067c 0783 0164 096b 0090 0172  .}.t.|...d.k...r
-00000dd0: 0a64 0a7d 0890 0171 107c 067d 0871 a67c  .d.}...q.|.}.q.|
-00000de0: 0864 0a6b 0290 0172 1c71 5c64 0b7c 006a  .d.k...r.q\d.|.j
-00000df0: 027c 0064 0119 007c 056b 0264 0c66 023c  .|.d...|.k.d.f.<
-00000e00: 0064 0b7c 006a 027c 0064 0119 007c 056b  .d.|.j.|.d...|.k
-00000e10: 0264 0d66 023c 0064 0b7c 006a 027c 0064  .d.f.<.d.|.j.|.d
-00000e20: 0119 007c 056b 0264 0766 023c 0064 0b7c  ...|.k.d.f.<.d.|
-00000e30: 006a 027c 0064 0119 007c 056b 0264 0e66  .j.|.d...|.k.d.f
-00000e40: 023c 0064 0b7c 006a 027c 0064 0119 007c  .<.d.|.j.|.d...|
-00000e50: 056b 0264 0f66 023c 0064 0b7c 006a 027c  .k.d.f.<.d.|.j.|
-00000e60: 0064 0119 007c 056b 0264 1066 023c 0064  .d...|.k.d.f.<.d
-00000e70: 117c 006a 0776 0090 0172 d864 0b7c 006a  .|.j.v...r.d.|.j
-00000e80: 027c 0064 0119 007c 056b 0264 1166 023c  .|.d...|.k.d.f.<
-00000e90: 0064 0b7c 006a 027c 0064 0119 007c 056b  .d.|.j.|.d...|.k
-00000ea0: 0264 1266 023c 007c 0764 1319 006a 0164  .d.f.<.|.d...j.d
-00000eb0: 0819 007c 006a 027c 0064 0119 007c 056b  ...|.j.|.d...|.k
-00000ec0: 0264 1366 023c 007c 0764 1419 006a 0164  .d.f.<.|.d...j.d
-00000ed0: 0819 007c 006a 027c 0064 0119 007c 056b  ...|.j.|.d...|.k
-00000ee0: 0264 1466 023c 007c 0764 1519 006a 0164  .d.f.<.|.d...j.d
-00000ef0: 0819 007c 006a 027c 0064 0119 007c 056b  ...|.j.|.d...|.k
-00000f00: 0264 1566 023c 0071 5c7c 0053 0029 164e  .d.f.<.q\|.S.).N
-00000f10: 7206 0000 00da 0844 6f77 5375 6249 64da  r......DowSubId.
-00000f20: 0566 6c6f 6174 da08 4c61 6b65 5f43 6174  .float..Lake_Cat
-00000f30: e902 0000 00e7 0000 0000 0000 0000 da09  ................
-00000f40: 5269 764c 656e 6774 6872 0100 0000 e901  RivLengthr......
-00000f50: 0000 00e9 ffff ffff e78d 976e 1283 c0f3  ...........n....
-00000f60: bfda 0852 6976 536c 6f70 65da 0443 685f  ...RivSlope..Ch_
-00000f70: 6eda 074d 696e 5f44 454d da07 4d61 785f  n..Min_DEM..Max_
-00000f80: 4445 4dda 0846 6c6f 6f64 505f 6eda 0844  DEM..FloodP_n..D
-00000f90: 415f 4368 6e5f 4cda 0a44 415f 4368 6e5f  A_Chn_L..DA_Chn_
-00000fa0: 536c 70da 0853 7472 6168 6c65 72da 0653  Slp..Strahler..S
-00000fb0: 6567 5f49 44da 0953 6567 5f6f 7264 6572  eg_ID..Seg_order
-00000fc0: 2908 da06 6173 7479 7065 7220 0000 0072  )...astyper ...r
-00000fd0: 2300 0000 7216 0000 0072 3d00 0000 721e  #...r....r=...r.
-00000fe0: 0000 0072 1f00 0000 720b 0000 0029 0ada  ...r....r....)..
-00000ff0: 0763 6174 696e 666f da0c 726f 7574 696e  .catinfo..routin
-00001000: 675f 696e 666f 5a15 6361 7469 6e66 6f5f  g_infoZ.catinfo_
-00001010: 6e6f 6e5f 636f 6e6e 6563 7465 645a 0963  non_connectedZ.c
-00001020: 6174 6964 735f 6e63 7228 0000 005a 0763  atids_ncr(...Z.c
-00001030: 5f73 7562 6964 5a07 645f 7375 6269 645a  _subidZ.d_subidZ
-00001040: 0a64 5f73 7562 5f69 6e66 6f5a 086c 635f  .d_sub_infoZ.lc_
-00001050: 7375 6269 645a 0d6c 635f 7375 6269 645f  subidZ.lc_subid_
-00001060: 696e 666f 722d 0000 0072 2d00 0000 722e  infor-...r-...r.
-00001070: 0000 00da 2375 7064 6174 655f 6e6f 6e5f  ....#update_non_
-00001080: 636f 6e6e 6563 7465 645f 6361 7463 686d  connected_catchm
-00001090: 656e 745f 696e 666f 9900 0000 7362 0000  ent_info....sb..
-000010a0: 0000 0114 0116 020c 0402 fe04 0110 ff02  ................
-000010b0: 0414 010e 010e 0116 0204 0a0c 0102 0614  ................
-000010c0: 0216 010e 0116 010e 0104 0104 0106 020a  ................
-000010d0: 0102 0216 0116 0116 0116 0116 0116 010c  ................
-000010e0: 0116 0116 0c02 0102 ff04 0202 fe16 0302  ................
-000010f0: 0102 ff04 0202 fe16 0302 0102 ff04 0202  ................
-00001100: fe18 0472 5f00 0000 6301 0000 0000 0000  ...r_...c.......
-00001110: 0000 0000 0010 0000 0006 0000 0043 0000  .............C..
-00001120: 0073 be01 0000 7c00 6a00 6401 6701 6402  .s....|.j.d.g.d.
-00001130: 6403 8d02 7d01 7401 a002 6404 6405 a102  d...}.t...d.d...
-00001140: 7d02 6406 7d03 7401 a002 6407 6408 a102  }.d.}.t...d.d...
-00001150: 7d04 7c01 6409 1900 6a03 6405 1900 7d05  }.|.d...j.d...}.
-00001160: 6406 7d06 7c05 7c04 7c03 6406 1800 3c00  d.}.|.|.|.d...<.
-00001170: 7404 7c04 7c04 6405 6b04 1900 8301 6405  t.|.|.d.k.....d.
-00001180: 6b04 9001 72b2 7401 a002 6407 6408 a102  k...r.t...d.d...
-00001190: 7d07 7c06 7d03 7405 6405 7c06 8302 4400  }.|.}.t.d.|...D.
-000011a0: 9001 5d2a 7d08 7c04 7c08 1900 7d09 7c09  ..]*}.|.|...}.|.
-000011b0: 6405 6b00 7292 717a 7c01 6a06 7c01 6409  d.k.r.qz|.j.|.d.
-000011c0: 1900 7c09 6b02 640a 6602 1900 7c02 7c08  ..|.k.d.f...|.|.
-000011d0: 1900 1700 7c02 7c08 3c00 7c01 6a06 7c01  ....|.|.<.|.j.|.
-000011e0: 6409 1900 7c09 6b02 640b 6602 1900 6a03  d...|.k.d.f...j.
-000011f0: 6405 1900 7d0a 7c01 6a06 7c01 640c 1900  d...}.|.j.|.d...
-00001200: 7c09 6b02 1900 7d0b 7404 7c0b 8301 6405  |.k...}.t.|...d.
-00001210: 6b01 72f0 717a 7c0b 6a06 7c0b 640b 1900  k.r.qz|.j.|.d...
-00001220: 7c0a 6b02 1900 7d0c 7404 7c0c 8301 6405  |.k...}.t.|...d.
-00001230: 6b04 9001 7226 7c0c 6409 1900 6a03 6405  k...r&|.d...j.d.
-00001240: 1900 7c07 7c08 3c00 717a 717a 7c0b 6a06  ..|.|.<.qzqz|.j.
-00001250: 7c0b 640b 1900 7c0a 6406 1800 6b02 1900  |.d...|.d...k...
-00001260: 7d0d 7405 6405 7404 7c0d 8301 8302 4400  }.t.d.t.|.....D.
-00001270: 5d5a 7d0e 7c0e 6405 6b02 9001 726c 7c0d  ]Z}.|.d.k...rl|.
-00001280: 6409 1900 6a03 7c0e 1900 7c07 7c08 3c00  d...j.|...|.|.<.
-00001290: 6e36 7c0d 6409 1900 6a03 7c0e 1900 7c07  n6|.d...j.|...|.
-000012a0: 7c03 6406 1700 6406 1800 3c00 7c02 7c08  |.d...d...<.|.|.
-000012b0: 1900 7c02 7c03 6406 1700 6406 1800 3c00  ..|.|.d...d...<.
-000012c0: 7c03 6406 1700 7d03 9001 714a 717a 7c07  |.d...}...qJqz|.
-000012d0: 7d04 7c03 7d06 714a 7407 7c02 8301 7d0f  }.|.}.qJt.|...}.
-000012e0: 7c0f 5300 290d 4eda 0944 7261 696e 4172  |.S.).N..DrainAr
-000012f0: 6561 46a9 0172 1200 0000 e964 0000 0072  eaF..r.....d...r
-00001300: 0100 0000 724f 0000 00e9 e803 0000 7250  ....rO........rP
-00001310: 0000 0072 0600 0000 724e 0000 0072 5900  ...r....rN...rY.
-00001320: 0000 7249 0000 0029 0872 1c00 0000 7221  ..rI...).r....r!
-00001330: 0000 00da 0466 756c 6c72 2000 0000 721f  .....fullr ...r.
-00001340: 0000 0072 1e00 0000 7223 0000 00da 036d  ...r....r#.....m
-00001350: 6178 2910 da11 6d61 696e 7269 765f 6d65  ax)...mainriv_me
-00001360: 7267 5f69 6e66 6f5a 166d 6169 6e72 6976  rg_infoZ.mainriv
-00001370: 5f6d 6572 675f 696e 666f 5f73 6f72 745a  _merg_info_sortZ
-00001380: 136c 6f6e 6765 7374 5f66 6c6f 775f 7061  .longest_flow_pa
-00001390: 7468 6573 da05 6e70 6174 685a 0650 6174  thes..npathZ.Pat
-000013a0: 6869 6472 2900 0000 5a0d 6e70 6174 685f  hidr)...Z.npath_
-000013b0: 6375 7272 656e 745a 076e 5061 7468 6964  currentZ.nPathid
-000013c0: 5a05 6970 6174 685a 0d63 5f73 7562 6964  Z.ipathZ.c_subid
-000013d0: 5f69 7061 7468 5a14 5374 7261 686c 6572  _ipathZ.Strahler
-000013e0: 5f6f 7264 6572 5f69 7061 7468 5a12 7570  _order_ipathZ.up
-000013f0: 7374 7265 616d 5f73 7562 5f69 6e66 6f73  stream_sub_infos
-00001400: 5a1e 7570 7374 7265 616d 5f73 7562 5f69  Z.upstream_sub_i
-00001410: 6e66 6f73 5f65 715f 5374 7261 686c 6572  nfos_eq_Strahler
-00001420: 5a20 7570 7374 7265 616d 5f73 7562 5f69  Z upstream_sub_i
-00001430: 6e66 6f73 5f65 715f 5374 7261 686c 6572  nfos_eq_Strahler
-00001440: 5f31 5a06 696e 7061 7468 5a0b 4c6f 6e67  _1Z.inpathZ.Long
-00001450: 6573 7470 6174 6872 2d00 0000 722d 0000  estpathr-...r-..
-00001460: 0072 2e00 0000 da1a 4361 6c63 756c 6174  .r......Calculat
-00001470: 655f 4c6f 6e67 6573 745f 666c 6f77 7061  e_Longest_flowpa
-00001480: 7468 e700 0000 737c 0000 0000 0110 020c  th....s|........
-00001490: 0204 030c 010e 0104 010c 0216 010c 0104  ................
-000014a0: 0510 0108 0306 ff02 0302 0304 010e ff02  ................
-000014b0: 0306 fd02 ff06 0604 010e ff04 0202 fe04  ................
-000014c0: 0404 010a ff04 050a ff02 0402 0504 010a  ................
-000014d0: ff04 050a ff04 0308 0102 ff08 0304 0204  ................
-000014e0: 010e ff04 0412 020a 0102 0102 ff04 0202  ................
-000014f0: fe0a 0502 0102 ff04 0202 fe10 0314 020e  ................
-00001500: 0204 0106 0108 0272 6800 0000 724f 0000  .......rh...rO..
-00001510: 0063 0200 0000 0000 0000 0000 0000 2100  .c............!.
-00001520: 0000 0800 0000 4300 0000 732c 0500 007c  ......C...s,...|
-00001530: 006a 0064 0164 028d 017d 027c 007c 0064  .j.d.d...}.|.|.d
-00001540: 0319 0064 041b 0064 041b 007c 016b 0019  ...d...d...|.k..
-00001550: 006a 0064 0164 028d 017d 037c 037c 0364  .j.d.d...}.|.|.d
-00001560: 0519 0064 066b 0219 006a 0064 0164 028d  ...d.k...j.d.d..
-00001570: 017d 037c 0364 0719 006a 017d 0464 087d  .}.|.d...j.}.d.}
-00001580: 0564 087c 006a 0276 0172 6064 097d 0574  .d.|.j.v.r`d.}.t
-00001590: 0364 0674 047c 0383 0183 0244 0090 045d  .d.t.|.....D...]
-000015a0: b67d 067c 0364 0719 006a 017c 0619 007d  .}.|.d...j.|...}
-000015b0: 077c 0364 0a19 006a 017c 0619 007d 087c  .|.d...j.|...}.|
-000015c0: 0364 0b19 006a 017c 0619 007d 0974 047c  .d...j.|...}.t.|
-000015d0: 007c 0064 0a19 007c 076b 0219 0083 0164  .|.d...|.k.....d
-000015e0: 066b 027d 0a7c 0364 0519 006a 017c 0619  .k.}.|.d...j.|..
-000015f0: 0064 066b 027d 0b7c 037c 0519 006a 017c  .d.k.}.|.|...j.|
-00001600: 0619 0064 066b 017d 0c7c 007c 0064 0719  ...d.k.}.|.|.d..
-00001610: 007c 086b 0219 006a 0064 0164 028d 017d  .|.k...j.d.d...}
-00001620: 0d7c 007c 0064 0a19 007c 076b 0219 006a  .|.|.d...|.k...j
-00001630: 0064 0164 028d 017d 0e7c 0e7c 0e64 0b19  .d.d...}.|.|.d..
-00001640: 007c 096b 0219 006a 0064 0164 028d 017d  .|.k...j.d.d...}
-00001650: 0f74 047c 0d83 0164 066b 0490 0172 5464  .t.|...d.k...rTd
-00001660: 017d 107c 0d64 0b19 006a 0164 0619 007c  .}.|.d...j.d...|
-00001670: 096b 0290 0172 4e64 017d 116e 0464 0c7d  .k...rNd.}.n.d.}
-00001680: 116e 0864 0c7d 1064 0c7d 1174 047c 0e83  .n.d.}.d.}.t.|..
-00001690: 0164 066b 0490 0172 8864 017d 1274 047c  .d.k...r.d.}.t.|
-000016a0: 0f83 0164 066b 0490 0172 8264 017d 136e  ...d.k...r.d.}.n
-000016b0: 0464 0c7d 136e 0864 0c7d 1264 0c7d 137c  .d.}.n.d.}.d.}.|
-000016c0: 1090 0272 007c 1190 0272 007c 0b90 0272  ...r.|...r.|...r
-000016d0: 007c 0c90 0272 007c 027c 0264 0719 007c  .|...r.|.|.d...|
-000016e0: 0d64 0719 006a 0164 0619 006b 0219 006a  .d...j.d...k...j
-000016f0: 0064 0164 028d 017d 1464 017d 157c 027c  .d.d...}.d.}.|.|
-00001700: 0264 0719 007c 0d64 0719 006a 0164 0619  .d...|.d...j.d..
-00001710: 006b 0219 006a 0064 0164 028d 017d 167c  .k...j.d.d...}.|
-00001720: 1664 0a19 006a 0164 0619 007d 176e de7c  .d...j.d...}.n.|
-00001730: 1290 0272 667c 1390 0272 667c 0b90 0272  ...rf|...rf|...r
-00001740: 667c 0c90 0272 667c 027c 0264 0719 007c  f|...rf|.|.d...|
-00001750: 0f64 0719 006a 0164 0619 006b 0219 006a  .d...j.d...k...j
-00001760: 0064 0164 028d 017d 1464 017d 157c 027c  .d.d...}.d.}.|.|
-00001770: 0264 0719 007c 076b 0219 006a 0064 0164  .d...|.k...j.d.d
-00001780: 028d 017d 187c 1864 0a19 006a 0164 0619  ...}.|.d...j.d..
-00001790: 007d 176e 7874 047c 007c 0064 0b19 007c  .}.nxt.|.|.d...|
-000017a0: 096b 0219 0083 0164 0d6b 0290 0272 d47c  .k.....d.k...r.|
-000017b0: 1090 0272 d47c 027c 0264 0719 007c 0d64  ...r.|.|.d...|.d
-000017c0: 0719 006a 0164 0619 006b 0219 006a 0064  ...j.d...k...j.d
-000017d0: 0164 028d 017d 1464 017d 157c 027c 0264  .d...}.d.}.|.|.d
-000017e0: 0719 007c 086b 0219 006a 0064 0164 028d  ...|.k...j.d.d..
-000017f0: 017d 167c 1664 0a19 006a 0164 0619 007d  .}.|.d...j.d...}
-00001800: 176e 0a64 0c7d 1567 007d 1471 6e7c 1572  .n.d.}.g.}.qn|.r
-00001810: 6e74 047c 007c 0064 0a19 007c 1464 0719  nt.|.|.d...|.d..
-00001820: 006a 0164 0619 006b 0219 0083 0164 066b  .j.d...k.....d.k
-00001830: 027d 1974 047c 007c 0064 0a19 007c 1464  .}.t.|.|.d...|.d
-00001840: 0719 006a 0164 0619 006b 027c 0064 0519  ...j.d...k.|.d..
-00001850: 0064 0e6b 0040 0019 0083 0164 0d6b 017d  .d.k.@.....d.k.}
-00001860: 1a7c 0264 0719 007c 076b 027d 1b7c 0264  .|.d...|.k.}.|.d
-00001870: 0f19 007c 076b 027d 1c7c 0264 0f19 007c  ...|.k.}.|.d...|
-00001880: 1464 0f19 006a 0164 0619 006b 027d 1d74  .d...j.d...k.}.t
-00001890: 05a0 067c 1b7c 1da1 027d 1e74 05a0 067c  ...|.|...}.t...|
-000018a0: 1e7c 1ca1 027d 1f74 047c 1483 0164 0d6b  .|...}.t.|...d.k
-000018b0: 0490 0372 ba74 0474 05a0 077c 1464 1019  ...r.t.t...|.d..
-000018c0: 006a 01a1 0183 0164 0d6b 0490 0372 ba74  .j.....d.k...r.t
-000018d0: 087c 077c 0983 0201 0074 087c 1467 0064  .|.|.....t.|.g.d
-000018e0: 11a2 0119 0083 0101 007c 146a 0244 005d  .........|.j.D.]
-000018f0: dc7d 207c 2064 036b 0290 0472 0274 05a0  .} | d.k...r.t..
-00001900: 097c 1464 0319 006a 0164 0619 007c 026a  .|.d...j.d...|.j
-00001910: 0a7c 1b64 0366 0219 006a 0164 0619 0017  .|.d.f...j.d....
-00001920: 00a1 017c 026a 0a7c 1f7c 2066 023c 006e  ...|.j.|.| f.<.n
-00001930: 987c 2064 076b 0290 0472 267c 1464 0f19  .| d.k...r&|.d..
-00001940: 006a 0164 0619 007c 026a 0a7c 1f64 0f66  .j.d...|.j.|.d.f
-00001950: 023c 006e 747c 2064 0a6b 0290 0472 407c  .<.nt| d.k...r@|
-00001960: 177c 026a 0a7c 1f7c 2066 023c 006e 5a7c  .|.j.|.| f.<.nZ|
-00001970: 2064 0f6b 0290 0373 c07c 2064 126b 0290   d.k...s.| d.k..
-00001980: 0373 c07c 2064 136b 0290 0373 c07c 2064  .s.| d.k...s.| d
-00001990: 146b 0290 0373 c07c 2064 156b 0290 0373  .k...s.| d.k...s
-000019a0: c07c 2064 166b 0290 0472 8290 0371 c06e  .| d.k...r...q.n
-000019b0: 187c 147c 2019 006a 0164 0619 007c 026a  .|.| ..j.d...|.j
-000019c0: 0a7c 1f7c 2066 023c 0090 0371 c07c 1990  .|.| f.<...q.|..
-000019d0: 0473 a87c 0a72 6e7c 1a72 6e64 177c 026a  .s.|.rn|.rnd.|.j
-000019e0: 0a7c 1f64 1866 023c 0064 177c 026a 0a7c  .|.d.f.<.d.|.j.|
-000019f0: 1f64 1966 023c 0064 177c 026a 0a7c 1f64  .d.f.<.d.|.j.|.d
-00001a00: 1a66 023c 0064 177c 026a 0a7c 1f64 1b66  .f.<.d.|.j.|.d.f
-00001a10: 023c 0064 177c 026a 0a7c 1f64 1c66 023c  .<.d.|.j.|.d.f.<
-00001a20: 0064 177c 026a 0a7c 1f64 1d66 023c 0064  .d.|.j.|.d.f.<.d
-00001a30: 1e7c 026a 0276 0072 6e64 177c 026a 0a7c  .|.j.v.rnd.|.j.|
-00001a40: 1f64 1e66 023c 0064 177c 026a 0a7c 1f64  .d.f.<.d.|.j.|.d
-00001a50: 1f66 023c 0071 6e7c 0253 0029 204e 5472  .f.<.qn|.S.) NTr
-00001a60: 0800 0000 da07 4261 7341 7265 6172 6300  ......BasArearc.
-00001a70: 0000 724b 0000 0072 0100 0000 7206 0000  ..rK...r....r...
-00001a80: 00da 0748 6173 5f50 4f49 da09 4861 735f  ...Has_POI..Has_
-00001a90: 4761 7567 6572 4900 0000 725a 0000 0046  GaugerI...rZ...F
-00001aa0: 724f 0000 0072 4c00 0000 da06 6e73 7562  rO...rL.....nsub
-00001ab0: 6964 da08 4879 4c61 6b65 4964 2904 7206  id..HyLakeId).r.
-00001ac0: 0000 0072 4900 0000 725a 0000 0072 6d00  ...rI...rZ...rm.
-00001ad0: 0000 da0a 6e64 6f77 6e73 7562 6964 da09  ....ndownsubid..
-00001ae0: 4f6c 645f 5375 6249 64da 0c4f 6c64 5f44  Old_SubId..Old_D
-00001af0: 6f77 5375 6249 6472 3b00 0000 da08 6765  owSubIdr;.....ge
-00001b00: 6f6d 6574 7279 7251 0000 0072 5200 0000  ometryrQ...rR...
-00001b10: 724e 0000 0072 5600 0000 7253 0000 0072  rN...rV...rS...r
-00001b20: 5400 0000 7255 0000 0072 5700 0000 7258  T...rU...rW...rX
-00001b30: 0000 0029 0b72 1600 0000 7220 0000 0072  ...).r....r ...r
-00001b40: 0b00 0000 721e 0000 0072 1f00 0000 7221  ....r....r....r!
-00001b50: 0000 00da 0a6c 6f67 6963 616c 5f6f 7272  .....logical_orr
-00001b60: 3c00 0000 da05 7072 696e 7472 1900 0000  <.....printr....
-00001b70: 7223 0000 0029 21da 0e6d 6170 6f6c 646e  r#...)!..mapoldn
-00001b80: 6577 5f69 6e66 6fda 0f61 7265 615f 7468  ew_info..area_th
-00001b90: 7265 7374 686f 6c64 5a12 6d61 706f 6c64  restholdZ.mapold
-00001ba0: 6e65 775f 696e 666f 5f6e 6577 5a12 736d  new_info_newZ.sm
-00001bb0: 616c 6c5f 7375 625f 6e6f 6e5f 6c61 6b65  all_sub_non_lake
-00001bc0: 5a18 736d 616c 6c5f 7375 625f 6e6f 6e5f  Z.small_sub_non_
-00001bd0: 6c61 6b65 5f73 7562 6964 da0e 4761 7567  lake_subid..Gaug
-00001be0: 655f 636f 6c5f 4e61 6d65 7228 0000 005a  e_col_Namer(...Z
-00001bf0: 0c73 6d61 6c6c 5f73 7562 5f69 645a 1073  .small_sub_idZ.s
-00001c00: 6d61 6c6c 5f64 6f77 6e73 7562 5f69 645a  mall_downsub_idZ
-00001c10: 1073 6d61 6c6c 5f73 7562 5f73 6567 5f69  .small_sub_seg_i
-00001c20: 645a 1b73 6d61 6c6c 5f73 7562 5f69 735f  dZ.small_sub_is_
-00001c30: 6865 6164 5f77 6174 6572 5f73 7562 5a15  head_water_subZ.
-00001c40: 736d 616c 6c5f 7375 625f 6973 5f6e 6f74  small_sub_is_not
-00001c50: 5f4c 616b 655a 1673 6d61 6c6c 5f73 7562  _LakeZ.small_sub
-00001c60: 5f69 735f 6e6f 745f 6761 7567 655a 0d64  _is_not_gaugeZ.d
-00001c70: 6f77 6e5f 7375 625f 696e 666f 5a11 7570  own_sub_infoZ.up
-00001c80: 7374 7265 616d 5f73 7562 5f69 6e66 6f5a  stream_sub_infoZ
-00001c90: 1a75 7073 7472 6561 6d5f 7375 625f 696e  .upstream_sub_in
-00001ca0: 666f 5f73 616d 655f 7365 675a 0c68 6173  fo_same_segZ.has
-00001cb0: 5f64 6f77 6e5f 7375 625a 1864 6f77 6e5f  _down_subZ.down_
-00001cc0: 7375 625f 6861 735f 7361 6d65 5f73 6567  sub_has_same_seg
-00001cd0: 5f69 645a 0c68 6173 5f75 7073 7472 6561  _idZ.has_upstrea
-00001ce0: 6d5a 1675 705f 7375 625f 6861 735f 7361  mZ.up_sub_has_sa
-00001cf0: 6d65 5f73 6567 5f69 64da 0774 6172 696e  me_seg_id..tarin
-00001d00: 666f da06 6d6f 6469 6679 5a0f 646f 776e  fo..modifyZ.down
-00001d10: 5f73 7562 5f69 6e66 6f5f 325a 0b6e 646f  _sub_info_2Z.ndo
-00001d20: 776e 5f73 7562 6964 5a12 6375 7272 656e  wn_subidZ.curren
-00001d30: 745f 7375 625f 696e 666f 5f32 5a1c 7461  t_sub_info_2Z.ta
-00001d40: 7267 6574 5f73 7562 5f69 735f 6865 6164  rget_sub_is_head
-00001d50: 5f77 6174 6572 5f73 7562 5a21 7461 7267  _water_subZ!targ
-00001d60: 6574 5f73 7562 5f68 6173 5f6c 6573 735f  et_sub_has_less_
-00001d70: 6f6e 655f 7570 5f73 7472 6561 6d72 2a00  one_up_streamr*.
-00001d80: 0000 5a05 6d61 736b 3372 2b00 0000 5a08  ..Z.mask3r+...Z.
-00001d90: 6d61 736b 7465 6d70 722c 0000 00da 0363  masktempr,.....c
-00001da0: 6f6c 722d 0000 0072 2d00 0000 722e 0000  olr-...r-...r...
-00001db0: 00da 1f72 656d 6f76 655f 706f 7373 6962  ...remove_possib
-00001dc0: 6c65 5f73 6d61 6c6c 5f73 7562 6261 7369  le_small_subbasi
-00001dd0: 6e73 3f01 0000 73ba 0000 0000 010c 0320  ns?...s........ 
-00001de0: 0118 010a 0304 010a 0104 0314 010e 010e  ................
-00001df0: 010e 0218 0212 0112 0218 0118 0118 040e  ................
-00001e00: 0104 0114 0106 0206 0204 0104 030e 0104  ................
-00001e10: 020e 0106 0206 0304 0104 0318 0322 0104  ............."..
-00001e20: 0122 0110 0218 0322 0104 0118 0110 0220  ."....."....... 
-00001e30: 0322 0104 0118 0110 0304 0104 0102 0204  ."..............
-00001e40: 0122 012e 020c 010c 0116 010c 010c 0228  .".............(
-00001e50: 010a 0110 0c0a 010a 0234 020a 021a 020a  .........4......
-00001e60: 0110 0206 ff04 0206 fe04 0306 fd04 0406  ................
-00001e70: fc04 0506 fb04 0606 fa04 0806 021c 020a  ................
-00001e80: 0104 010e 010e 010e 010e 010e 010e 010a  ................
-00001e90: 010e 0110 0a72 7a00 0000 7250 0000 0063  .....rz...rP...c
-00001ea0: 0900 0000 0000 0000 0000 0000 1600 0000  ................
-00001eb0: 0500 0000 4300 0000 73de 0400 0064 017d  ....C...s....d.}
-00001ec0: 097c 0164 0164 0267 0219 00a0 0064 03a1  .|.d.d.g.....d..
-00001ed0: 016a 017d 0a7c 0464 046b 0072 5e74 027c  .j.}.|.d.k.r^t.|
-00001ee0: 0a7c 0083 027d 0b7c 0364 046b 0472 5874  .|...}.|.d.k.rXt
-00001ef0: 027c 0a7c 0383 027d 0c74 03a0 047c 0b7c  .|.|...}.t...|.|
-00001f00: 0ca1 027d 0d7c 0b74 03a0 057c 0da1 0119  ...}.|.t...|....
-00001f10: 007d 0e71 627c 0b7d 0e6e 047c 057d 0e7c  .}.qb|.}.n.|.}.|
-00001f20: 017c 017c 0919 00a0 067c 0ea1 0119 00a0  .|.|.....|......
-00001f30: 07a1 007d 0f7c 017c 017c 0919 007c 006b  ...}.|.|.|...|.k
-00001f40: 0219 00a0 07a1 007d 107c 066a 087c 0664  .......}.|.j.|.d
-00001f50: 0119 00a0 067c 0ea1 0119 00a0 07a1 007d  .....|.........}
-00001f60: 117c 116a 087c 1164 0519 0064 046b 0419  .|.j.|.d...d.k..
-00001f70: 00a0 07a1 007d 117c 106a 0964 0419 007d  .....}.|.j.d...}
-00001f80: 1274 0a7c 1183 0164 046b 0490 0172 e474  .t.|...d.k...r.t
-00001f90: 03a0 0b7c 1164 0519 006a 01a1 017c 106a  ...|.d...j...|.j
-00001fa0: 087c 1264 0566 023c 0074 036a 0c7c 1164  .|.d.f.<.t.j.|.d
-00001fb0: 0619 006a 017c 1164 0519 006a 0164 078d  ...j.|.d...j.d..
-00001fc0: 027c 106a 087c 1264 0666 023c 0074 036a  .|.j.|.d.f.<.t.j
-00001fd0: 0c7c 1164 0819 006a 017c 1164 0519 006a  .|.d...j.|.d...j
-00001fe0: 0164 078d 027c 106a 087c 1264 0866 023c  .d...|.j.|.d.f.<
-00001ff0: 0074 036a 0c7c 1164 0919 006a 017c 1164  .t.j.|.d...j.|.d
-00002000: 0519 006a 0164 078d 027c 106a 087c 1264  ...j.d...|.j.|.d
-00002010: 0966 023c 0074 036a 0c7c 1164 0a19 006a  .f.<.t.j.|.d...j
-00002020: 017c 1164 0519 006a 0164 078d 027c 106a  .|.d...j.d...|.j
-00002030: 087c 1264 0a66 023c 0074 03a0 0d7c 1164  .|.d.f.<.t...|.d
-00002040: 0b19 006a 01a1 017c 106a 087c 1264 0b66  ...j...|.j.|.d.f
-00002050: 023c 0074 03a0 0d7c 1164 0c19 006a 01a1  .<.t...|.d...j..
-00002060: 017c 106a 087c 1264 0c66 023c 0074 03a0  .|.j.|.d.f.<.t..
-00002070: 0d7c 1164 0d19 006a 01a1 017c 106a 087c  .|.d...j...|.j.|
-00002080: 1264 0d66 023c 0074 03a0 0e7c 1164 0e19  .d.f.<.t...|.d..
-00002090: 006a 01a1 017c 106a 087c 1264 0e66 023c  .j...|.j.|.d.f.<
-000020a0: 0074 03a0 0b7c 0f64 0f19 006a 01a1 017c  .t...|.d...j...|
-000020b0: 106a 087c 1264 0f66 023c 0074 0a7c 0f83  .j.|.d.f.<.t.|..
-000020c0: 0164 046b 0490 0272 7874 036a 0c7c 0f64  .d.k...rxt.j.|.d
-000020d0: 1019 006a 017c 0f64 0f19 006a 0164 078d  ...j.|.d...j.d..
-000020e0: 027c 106a 087c 1264 1066 023c 0074 036a  .|.j.|.d.f.<.t.j
-000020f0: 0c7c 0f64 1119 006a 017c 0f64 0f19 006a  .|.d...j.|.d...j
-00002100: 0164 078d 027c 106a 087c 1264 1166 023c  .d...|.j.|.d.f.<
-00002110: 0074 036a 0c7c 0f64 1219 006a 017c 0f64  .t.j.|.d...j.|.d
-00002120: 0f19 006a 0164 078d 027c 106a 087c 1264  ...j.d...|.j.|.d
-00002130: 1266 023c 007c 0764 136b 0290 0372 0064  .f.<.|.d.k...r.d
-00002140: 147c 106a 087c 1264 0666 023c 0064 147c  .|.j.|.d.f.<.d.|
-00002150: 106a 087c 1264 0566 023c 0064 147c 106a  .j.|.d.f.<.d.|.j
-00002160: 087c 1264 0866 023c 0064 147c 106a 087c  .|.d.f.<.d.|.j.|
-00002170: 1264 0a66 023c 0064 147c 106a 087c 1264  .d.f.<.d.|.j.|.d
-00002180: 0e66 023c 0064 147c 106a 087c 1264 0d66  .f.<.d.|.j.|.d.f
-00002190: 023c 0064 157c 106a 0f76 0090 0372 f464  .<.d.|.j.v...r.d
-000021a0: 147c 106a 087c 1264 1566 023c 0064 147c  .|.j.|.d.f.<.d.|
-000021b0: 106a 087c 1264 1666 023c 006e f47c 0764  .j.|.d.f.<.n.|.d
-000021c0: 176b 0290 0372 9664 147c 106a 087c 1264  .k...r.d.|.j.|.d
-000021d0: 0666 023c 0064 147c 106a 087c 1264 0566  .f.<.d.|.j.|.d.f
-000021e0: 023c 0064 147c 106a 087c 1264 0866 023c  .<.d.|.j.|.d.f.<
-000021f0: 0064 147c 106a 087c 1264 0a66 023c 0064  .d.|.j.|.d.f.<.d
-00002200: 147c 106a 087c 1264 0e66 023c 0064 147c  .|.j.|.d.f.<.d.|
-00002210: 106a 087c 1264 0d66 023c 0064 157c 106a  .j.|.d.f.<.d.|.j
-00002220: 0f76 0090 0372 8664 147c 106a 087c 1264  .v...r.d.|.j.|.d
-00002230: 1566 023c 0064 147c 106a 087c 1264 1666  .f.<.d.|.j.|.d.f
-00002240: 023c 0064 177c 106a 087c 1264 1866 023c  .<.d.|.j.|.d.f.<
-00002250: 006e 5e7c 0764 046b 0190 0372 f464 047c  .n^|.d.k...r.d.|
-00002260: 106a 087c 1264 1966 023c 0064 047c 106a  .j.|.d.f.<.d.|.j
-00002270: 087c 1264 1a66 023c 0064 047c 106a 087c  .|.d.f.<.d.|.j.|
-00002280: 1264 1b66 023c 0064 047c 106a 087c 1264  .d.f.<.d.|.j.|.d
-00002290: 1c66 023c 0064 047c 106a 087c 1264 1d66  .f.<.d.|.j.|.d.f
-000022a0: 023c 0064 047c 106a 087c 1264 1866 023c  .<.d.|.j.|.d.f.<
-000022b0: 0064 147c 106a 087c 1264 1e66 023c 0064  .d.|.j.|.d.f.<.d
-000022c0: 147c 106a 087c 1264 1f66 023c 007c 0864  .|.j.|.d.f.<.|.d
-000022d0: 046b 0490 0472 287c 087c 106a 087c 1264  .k...r(|.|.j.|.d
-000022e0: 2066 023c 007c 0264 0119 00a0 067c 0ea1   f.<.|.d.....|..
-000022f0: 017d 137c 0264 2119 007c 006b 027d 1474  .}.|.d!..|.k.}.t
-00002300: 03a0 107c 137c 14a1 027d 0d7c 106a 0f44  ...|.|...}.|.j.D
-00002310: 005d 847d 157c 1564 016b 0290 0472 7c7c  .].}.|.d.k...r||
-00002320: 107c 1519 006a 0164 0419 007c 026a 087c  .|...j.d...|.j.|
-00002330: 0d64 2166 023c 006e 5a7c 1564 216b 0290  .d!f.<.nZ|.d!k..
-00002340: 0473 547c 1564 226b 0290 0473 547c 1564  .sT|.d"k...sT|.d
-00002350: 236b 0290 0473 547c 1564 246b 0290 0473  #k...sT|.d$k...s
-00002360: 547c 1564 256b 0290 0473 547c 1564 266b  T|.d%k...sT|.d&k
-00002370: 0290 0472 be90 0471 546e 187c 107c 1519  ...r...qTn.|.|..
-00002380: 006a 0164 0419 007c 026a 087c 0d7c 1566  .j.d...|.j.|.|.f
-00002390: 023c 0090 0471 547c 0253 0029 274e 7206  .<...qT|.S.)'Nr.
-000023a0: 0000 0072 4900 0000 da05 696e 7433 3272  ...rI.....int32r
-000023b0: 0100 0000 724e 0000 0072 5200 0000 a901  ....rN...rR.....
-000023c0: da07 7765 6967 6874 7372 5600 0000 5a06  ..weightsrV...Z.
-000023d0: 515f 4d65 616e 7253 0000 005a 0842 6b66  Q_MeanrS...Z.Bkf
-000023e0: 5769 6474 685a 0842 6b66 4465 7074 6872  WidthZ.BkfDepthr
-000023f0: 5500 0000 7254 0000 0072 6900 0000 da08  U...rT...ri.....
-00002400: 4261 7353 6c6f 7065 5a08 4d65 616e 456c  BasSlopeZ.MeanEl
-00002410: 6576 5a09 4261 7341 7370 6563 7472 4f00  evZ.BasAspectrO.
-00002420: 0000 7251 0000 0072 5700 0000 7258 0000  ..rQ...rW...rX..
-00002430: 0072 4c00 0000 724b 0000 0072 6d00 0000  .rL...rK...rm...
-00002440: da07 4c61 6b65 566f 6cda 084c 616b 6541  ..LakeVol..LakeA
-00002450: 7265 61da 094c 616b 6544 6570 7468 da08  rea..LakeDepth..
-00002460: 4c61 6b65 7479 7065 da0a 6365 6e74 726f  Laketype..centro
-00002470: 6964 5f78 da0a 6365 6e74 726f 6964 5f79  id_x..centroid_y
-00002480: 725b 0000 0072 6c00 0000 726e 0000 0072  r[...rl...rn...r
-00002490: 6f00 0000 7270 0000 0072 3b00 0000 7271  o...rp...r;...rq
-000024a0: 0000 0029 1172 5c00 0000 7220 0000 00da  ...).r\...r ....
-000024b0: 0664 6566 6361 7472 2100 0000 da04 696e  .defcatr!.....in
-000024c0: 3164 da0b 6c6f 6769 6361 6c5f 6e6f 7472  1d..logical_notr
-000024d0: 3d00 0000 7216 0000 0072 2300 0000 723e  =...r....r#...r>
-000024e0: 0000 0072 1f00 0000 7219 0000 00da 0761  ...r....r......a
-000024f0: 7665 7261 6765 7265 0000 00da 036d 696e  veragere.....min
-00002500: 720b 0000 0072 7200 0000 2916 7229 0000  r....rr...).r)..
-00002510: 00da 0d63 6174 6368 6d65 6e74 696e 666f  ...catchmentinfo
-00002520: 7274 0000 005a 0775 7073 7562 6964 da0a  rt...Z.upsubid..
-00002530: 6973 6d6f 6469 6669 6473 da0a 6d6f 6469  ismodifids..modi
-00002540: 6669 6964 696e da07 6d61 696e 7269 7672  fiidin..mainrivr
-00002550: 4b00 0000 da09 7365 675f 6f72 6465 72da  K.....seg_order.
-00002560: 0973 7562 5f63 6f6c 6e6d 725e 0000 005a  .sub_colnmr^...Z
-00002570: 0e4d 6f64 6966 795f 7375 6269 6473 315a  .Modify_subids1Z
-00002580: 0e4d 6f64 6966 795f 7375 6269 6473 3272  .Modify_subids2r
-00002590: 2c00 0000 5a0d 4d6f 6469 6679 5f73 7562  ,...Z.Modify_sub
-000025a0: 6964 735a 0763 6272 616e 6368 7277 0000  idsZ.cbranchrw..
-000025b0: 0072 6600 0000 7245 0000 0072 2a00 0000  .rf...rE...r*...
-000025c0: 722b 0000 0072 7900 0000 722d 0000 0072  r+...ry...r-...r
-000025d0: 2d00 0000 722e 0000 00da 154e 6577 5f53  -...r......New_S
-000025e0: 7562 4964 5f54 6f5f 4469 7373 6f6c 7665  ubId_To_Dissolve
-000025f0: d801 0000 73da 0000 0000 0b04 0114 0108  ....s...........
-00002600: 0102 0104 ff04 0308 010a 010c 0110 0206  ................
-00002610: 0304 0416 0102 010a ff08 0418 0116 010a  ................
-00002620: 020e 011a 0104 0108 0108 fe10 0404 0108  ................
-00002630: 0108 fe10 0404 0108 0108 fe10 0404 0108  ................
-00002640: 0108 fe10 041a 011a 021a 011a 021a 020e  ................
-00002650: 0104 0110 ff10 0304 0110 ff10 0304 0110  ................
-00002660: ff10 0506 ff04 040e 010e 010e 010e 010e  ................
-00002670: 010e 010c 010e 0110 020a 010e 010e 010e  ................
-00002680: 010e 010e 010e 010c 010e 010e 0110 010a  ................
-00002690: 050e 010e 010e 010e 010e 010e 020e 010e  ................
-000026a0: 020a 010e 0208 0102 ff04 040a ff02 030c  ................
-000026b0: 030a 010a 021a 0306 ff04 0206 fe04 0306  ................
-000026c0: fd04 0406 fc04 0506 fb04 0606 fa04 0806  ................
-000026d0: 021c 0372 9000 0000 7206 0000 0063 0300  ...r....r....c..
-000026e0: 0000 0000 0000 0000 0000 0800 0000 0400  ................
-000026f0: 0000 4300 0000 73a4 0000 007c 006a 007c  ..C...s....|.j.|
-00002700: 016a 006b 03a0 01a1 0072 2874 027c 006a  .j.k.....r(t.|.j
-00002710: 0083 0101 0074 027c 016a 0083 0101 0064  .....t.|.j.....d
-00002720: 0153 0064 027d 037c 006a 0044 005d 627d  .S.d.}.|.j.D.]b}
-00002730: 047c 0464 036b 0272 487c 0364 0417 007d  .|.d.k.rH|.d...}
-00002740: 0371 327c 007c 0419 006a 037d 057c 017c  .q2|.|...j.}.|.|
-00002750: 0419 006a 037d 067c 057c 066b 03a0 01a1  ...j.}.|.|.k....
-00002760: 0072 8c74 027c 0483 0101 007c 057c 066b  .r.t.|.....|.|.k
-00002770: 037d 0774 027c 007c 0219 006a 037c 0719  .}.t.|.|...j.|..
-00002780: 0083 0101 0071 327c 0364 0417 007d 0371  .....q2|.d...}.q
-00002790: 327c 0374 047c 006a 0083 016b 0253 0029  2|.t.|.j...k.S.)
-000027a0: 054e 4672 0100 0000 da06 4852 555f 4944  .NFr......HRU_ID
-000027b0: 724f 0000 0029 0572 0b00 0000 da03 616c  rO...).r......al
-000027c0: 6c72 7300 0000 7220 0000 0072 1f00 0000  lrs...r ...r....
-000027d0: 2908 5a08 4578 7065 6374 6564 5a06 5265  ).Z.ExpectedZ.Re
-000027e0: 7375 6c74 5a0c 4368 6563 6b5f 436f 6c5f  sultZ.Check_Col_
-000027f0: 4e4d 5a04 6e65 716c 7279 0000 005a 0c41  NMZ.neqlry...Z.A
-00002800: 7272 6179 5f65 7870 6563 745a 0c41 7272  rray_expectZ.Arr
-00002810: 6179 5f72 6573 756c 7472 2c00 0000 722d  ay_resultr,...r-
-00002820: 0000 0072 2d00 0000 722e 0000 00da 1745  ...r-...r......E
-00002830: 7661 6c75 6174 655f 5477 6f5f 4461 7461  valuate_Two_Data
-00002840: 6672 616d 6573 6c02 0000 7322 0000 0000  framesl...s"....
-00002850: 0210 010a 010a 0104 0104 020a 0108 0108  ................
-00002860: 0102 010a 010a 010c 0108 0108 0114 020a  ................
-00002870: 0272 9300 0000 6303 0000 0000 0000 0000  .r....c.........
-00002880: 0000 000b 0000 0005 0000 0043 0000 0073  ...........C...s
-00002890: ac01 0000 7c00 6a00 7d03 7c02 6401 6b04  ....|.j.}.|.d.k.
-000028a0: 72e2 7401 6401 7402 7c03 8301 8302 4400  r.t.d.t.|.....D.
-000028b0: 5d8c 7d04 7c00 6a03 7c03 7c04 1900 6402  ].}.|.j.|.|...d.
-000028c0: 6602 1900 7d05 7c00 6a03 7c03 7c04 1900  f...}.|.j.|.|...
-000028d0: 6403 6602 1900 7d06 7c00 6a03 7c03 7c04  d.f...}.|.j.|.|.
-000028e0: 1900 6404 6602 1900 7d07 7c00 6a03 7c00  ..d.f...}.|.j.|.
-000028f0: 6403 1900 7c07 6b02 1900 a004 a100 7d08  d...|.k.......}.
-00002900: 7402 7c08 8301 6401 6b04 7296 7c08 6402  t.|...d.k.r.|.d.
-00002910: 1900 6a05 6401 1900 7c00 6a03 7c03 7c04  ..j.d...|.j.|.|.
-00002920: 1900 6405 6602 3c00 711c 6406 7c00 6a03  ..d.f.<.q.d.|.j.
-00002930: 7c03 7c04 1900 6405 6602 3c00 711c 7c00  |.|...d.f.<.q.|.
-00002940: 6403 1900 6a05 7c00 6407 3c00 7c00 6404  d...j.|.d.<.|.d.
-00002950: 1900 6a05 7c00 6408 3c00 7c00 6402 1900  ..j.|.d.<.|.d...
-00002960: 6a05 7c00 6403 3c00 7c00 6405 1900 6a05  j.|.d.<.|.d...j.
-00002970: 7c00 6404 3c00 7c01 6401 6b00 72ee 7c00  |.d.<.|.d.k.r.|.
-00002980: 5300 7c00 6a06 6403 6409 640a 8d02 7d09  S.|.j.d.d.d...}.
-00002990: 7407 7c09 8301 7d09 7401 6401 7402 7c09  t.|...}.t.d.t.|.
-000029a0: 8301 8302 4400 5d94 7d04 7c09 6403 1900  ....D.].}.|.d...
-000029b0: 6a05 7c04 1900 7d0a 7c09 640b 1900 6a05  j.|...}.|.d...j.
-000029c0: 7c04 1900 7c00 6a03 7c00 6403 1900 7c0a  |...|.j.|.d...|.
-000029d0: 6b02 640b 6602 3c00 7c09 640c 1900 6a05  k.d.f.<.|.d...j.
-000029e0: 7c04 1900 7c00 6a03 7c00 6403 1900 7c0a  |...|.j.|.d...|.
-000029f0: 6b02 640c 6602 3c00 7c09 640d 1900 6a05  k.d.f.<.|.d...j.
-00002a00: 7c04 1900 7c00 6a03 7c00 6403 1900 7c0a  |...|.j.|.d...|.
-00002a10: 6b02 640d 6602 3c00 7c09 640e 1900 6a05  k.d.f.<.|.d...j.
-00002a20: 7c04 1900 7c00 6a03 7c00 6403 1900 7c0a  |...|.j.|.d...|.
-00002a30: 6b02 640e 6602 3c00 9001 7112 7c00 5300  k.d.f.<...q.|.S.
-00002a40: 290f fadf 4675 6e63 7469 6f6e 7320 7769  )...Functions wi
-00002a50: 6c6c 2075 7064 6174 6520 7375 6269 642c  ll update subid,
-00002a60: 646f 776e 7375 6269 642c 2063 616c 6375  downsubid, calcu
-00002a70: 6174 6520 7374 7265 616d 206f 7264 6572  ate stream order
-00002a80: 2061 6e64 0a20 2020 2020 2020 2075 7064   and.        upd
-00002a90: 6174 6520 6472 6169 6e61 6765 2061 7265  ate drainage are
-00002aa0: 6120 696e 2074 6865 2061 7474 7269 6275  a in the attribu
-00002ab0: 7465 2074 6162 6c65 206d 6170 6f6c 646e  te table mapoldn
-00002ac0: 6577 5f69 6e66 6f0a 2020 2020 2d2d 2d2d  ew_info.    ----
-00002ad0: 2d2d 2d2d 2d2d 0a0a 2020 2020 4e6f 7465  ------..    Note
-00002ae0: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20  s.    -------.. 
-00002af0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002b00: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00002b10: 6d61 706f 6c64 6e65 775f 696e 666f 0a20  mapoldnew_info. 
-00002b20: 2020 2072 0100 0000 726c 0000 0072 0600     r....rl...r..
-00002b30: 0000 7249 0000 0072 6e00 0000 7250 0000  ..rI...rn...rP..
-00002b40: 0072 6f00 0000 7270 0000 0072 1300 0000  .ro...rp...r....
-00002b50: a901 7215 0000 0072 5900 0000 725a 0000  ..r....rY...rZ..
-00002b60: 0072 5b00 0000 7260 0000 0029 0872 3e00  .r[...r`...).r>.
-00002b70: 0000 721e 0000 0072 1f00 0000 7223 0000  ..r....r....r#..
-00002b80: 0072 1600 0000 7220 0000 0072 1d00 0000  .r....r ...r....
-00002b90: da1a 7374 7265 616d 6f72 6465 7261 6e64  ..streamorderand
-00002ba0: 6472 6169 6e61 6765 6172 6561 290b 7274  drainagearea).rt
-00002bb0: 0000 00da 1155 7064 6174 6553 7472 6561  .....UpdateStrea
-00002bc0: 6d6f 7264 6572 da0b 5570 6461 7465 5375  morder..UpdateSu
-00002bd0: 6249 6472 4500 0000 7228 0000 0072 6c00  bIdrE...r(...rl.
-00002be0: 0000 7229 0000 00da 0a6f 646f 776e 7375  ..r).....odownsu
-00002bf0: 6269 64da 0c64 6f6e 7375 6269 6469 6e66  bid..donsubidinf
-00002c00: 6fda 156d 6170 6f6c 646e 6577 5f69 6e66  o..mapoldnew_inf
-00002c10: 6f5f 756e 6971 7565 da06 6973 7562 6964  o_unique..isubid
-00002c20: 722d 0000 0072 2d00 0000 722e 0000 00da  r-...r-...r.....
-00002c30: 0e55 7064 6174 6554 6f70 6f6c 6f67 7984  .UpdateTopology.
-00002c40: 0200 0073 5600 0000 000d 0602 0801 1201  ...sV...........
-00002c50: 1201 1201 1202 0401 0aff 0804 0c01 0201  ................
-00002c60: 02ff 0402 02fe 1404 1402 0e01 0e01 0e02  ................
-00002c70: 0e02 0801 0402 0e02 0802 1201 0e03 0cfe  ................
-00002c80: 0401 0eff 0205 0cfe 0401 0eff 0205 0cfe  ................
-00002c90: 0401 0eff 0205 0cfe 0401 0eff 0604 729d  ..............r.
-00002ca0: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00002cb0: 0800 0000 0500 0000 4300 0000 738a 0000  ........C...s...
-00002cc0: 0064 017c 0064 021b 0064 021b 0064 0313  .d.|.d...d...d..
-00002cd0: 0014 007d 0364 047c 0164 021b 0014 007c  ...}.d.|.d.....|
-00002ce0: 0064 021b 0064 021b 0064 0513 0014 007c  .d...d...d.....|
-00002cf0: 0264 0613 0014 007d 0464 077c 0164 021b  .d.....}.d.|.d..
-00002d00: 0064 0813 0014 007c 0264 0913 0014 007d  .d.....|.d.....}
-00002d10: 0564 0a7c 0164 021b 007c 0264 0313 001b  .d.|.d...|.d....
-00002d20: 0064 0b13 0014 007d 0664 0c7c 017c 0264  .d.....}.d.|.|.d
-00002d30: 0313 001b 0064 0d13 0014 007d 077c 037c  .....d.....}.|.|
-00002d40: 047c 057c 067c 0766 0553 0029 0e4e 679a  .|.|.|.f.S.).Ng.
-00002d50: 9999 9999 99e5 3f72 6300 0000 e700 0000  ......?rc.......
-00002d60: 0000 00e0 3f67 933a 014d 840d cf3f 679a  ....?g.:.M...?g.
-00002d70: 9999 9999 99b9 bf67 9a99 9999 9999 c9bf  .......g........
-00002d80: 6733 3333 3333 33d3 3f67 52b8 1e85 eb51  g333333.?gR....Q
-00002d90: e83f 6752 b81e 85eb 51c8 bf67 abaa aaaa  .?gR....Q..g....
-00002da0: aaaa 1240 6714 ae47 e17a 14de 3f67 c20f  ...@g..G.z..?g..
-00002db0: e172 cfcd 413f 6748 e17a 14ae 47e9 3f72  .r..A?gH.z..G.?r
-00002dc0: 2d00 0000 2908 7260 0000 0072 5700 0000  -...).r`...rW...
-00002dd0: 7258 0000 005a 0454 435f 315a 0454 435f  rX...Z.TC_1Z.TC_
-00002de0: 325a 0454 435f 335a 0454 435f 345a 0454  2Z.TC_3Z.TC_4Z.T
-00002df0: 435f 3572 2d00 0000 722d 0000 0072 2e00  C_5r-...r-...r..
-00002e00: 0000 da0c 6361 6c63 756c 6174 655f 5463  ....calculate_Tc
-00002e10: c202 0000 730c 0000 0000 0214 0124 0118  ....s........$..
-00002e20: 0118 0114 0172 9f00 0000 6301 0000 0000  .....r....c.....
-00002e30: 0000 0000 0000 0018 0000 0006 0000 0043  ...............C
-00002e40: 0000 0073 ae09 0000 6401 7d01 6401 7c00  ...s....d.}.d.|.
-00002e50: 6a00 7601 7212 6402 7d01 7c00 6a01 7c00  j.v.r.d.}.|.j.|.
-00002e60: 6403 1900 6404 6b03 1900 a002 a100 7d02  d...d.k.......}.
-00002e70: 7c00 6a01 7c00 6403 1900 6404 6b02 1900  |.j.|.d...d.k...
-00002e80: a002 a100 7d03 7c03 6405 6406 6702 1900  ....}.|.d.d.g...
-00002e90: a003 6407 a101 6a04 7d04 7405 a006 7407  ..d...j.}.t...t.
-00002ea0: 7c02 8301 6408 a102 7d05 6409 7d06 640a  |...d...}.d.}.d.
-00002eb0: 7d07 7408 6409 7407 7c02 8301 8302 4400  }.t.d.t.|.....D.
-00002ec0: 9001 5dfc 7d08 7c02 6a09 7c08 1900 7d09  ..].}.|.j.|...}.
-00002ed0: 7c02 6405 1900 6a04 7c08 1900 7c02 6406  |.d...j.|...|.d.
-00002ee0: 1900 6a04 7c08 1900 6b02 72b2 640b 7c02  ..j.|...k.r.d.|.
-00002ef0: 6a01 7c09 6406 6602 3c00 7c02 6405 1900  j.|.d.f.<.|.d...
-00002f00: 6a04 7c08 1900 7d0a 7407 7c02 7c02 6406  j.|...}.t.|.|.d.
-00002f10: 1900 7c0a 6b02 1900 8301 6409 6b02 7278  ..|.k.....d.k.rx
-00002f20: 740a 7c02 6406 1900 6a04 7c08 1900 8301  t.|.d...j.|.....
-00002f30: 7c05 7c06 3c00 7407 7c04 8301 6409 6b02  |.|.<.t.|...d.k.
-00002f40: 9001 7206 640c 7d0b 640c 7d0c 6e62 740b  ..r.d.}.d.}.nbt.
-00002f50: 7c04 7c0a 8302 7d0d 7c03 6a01 7c03 6405  |.|...}.|.j.|.d.
-00002f60: 1900 a00c 7c0d a101 1900 a002 a100 7d0e  ....|.........}.
-00002f70: 7407 7c0e 8301 6409 6b04 9001 7260 740d  t.|...d.k...r`t.
-00002f80: 7c0e 640d 1900 6a04 8301 7d0b 7405 6a0e  |.d...j...}.t.j.
-00002f90: 7c0e 640e 1900 6a04 7c0e 640d 1900 6a04  |.d...j.|.d...j.
-00002fa0: 640f 8d02 7d0c 6e08 640c 7d0b 640c 7d0c  d...}.n.d.}.d.}.
-00002fb0: 7c0b 7c02 640d 1900 6a04 7c08 1900 1700  |.|.d...j.|.....
-00002fc0: 7c02 6a01 7c09 6410 6602 3c00 640a 7c02  |.j.|.d.f.<.d.|.
-00002fd0: 6a01 7c09 6411 6602 3c00 640a 7c02 6a01  j.|.d.f.<.d.|.j.
-00002fe0: 7c09 6412 6602 3c00 7c07 7c02 6a01 7c09  |.d.f.<.|.|.j.|.
-00002ff0: 6413 6602 3c00 6414 7c02 6a00 7600 9001  d.f.<.d.|.j.v...
-00003000: 72d6 6415 7c02 6a01 7c09 6414 6602 3c00  r.d.|.j.|.d.f.<.
-00003010: 6415 7c02 6a01 7c09 6416 6602 3c00 6415  d.|.j.|.d.f.<.d.
-00003020: 7c02 6a01 7c09 6417 6602 3c00 6415 7c02  |.j.|.d.f.<.d.|.
-00003030: 6a01 7c09 6418 6602 3c00 6415 7c02 6a01  j.|.d.f.<.d.|.j.
-00003040: 7c09 6419 6602 3c00 6415 7c02 6a01 7c09  |.d.f.<.d.|.j.|.
-00003050: 641a 6602 3c00 6415 7c02 6a01 7c09 641b  d.f.<.d.|.j.|.d.
-00003060: 6602 3c00 6415 7c02 6a01 7c09 641c 6602  f.<.d.|.j.|.d.f.
-00003070: 3c00 7c02 640e 1900 6a04 7c08 1900 7c02  <.|.d...j.|...|.
-00003080: 640d 1900 6a04 7c08 1900 1400 7c0b 7c0c  d...j.|.....|.|.
-00003090: 1400 1700 7c02 6a01 7c09 6410 6602 1900  ....|.j.|.d.f...
-000030a0: 1b00 7c02 6a01 7c09 641d 6602 3c00 7c06  ..|.j.|.d.f.<.|.
-000030b0: 640a 1700 7d06 7c07 640a 1700 7d07 7178  d...}.|.d...}.qx
-000030c0: 7405 a00f 7c05 a101 7d05 7c05 7c05 6409  t...|...}.|.|.d.
-000030d0: 6b04 1900 7d05 7405 a006 7407 7c02 8301  k...}.t...t.|...
-000030e0: 6408 a102 7d0f 6409 7d10 7408 6409 7407  d...}.d.}.t.d.t.
-000030f0: 7c05 8301 8302 4400 9004 5d92 7d08 7c05  |.....D...].}.|.
-00003100: 7c08 1900 7d0a 640a 7d11 7c11 640a 6b02  |...}.d.}.|.d.k.
-00003110: 9002 72b0 7c0a 6409 6b04 9002 72b0 7c02  ..r.|.d.k...r.|.
-00003120: 6a01 7c02 6406 1900 7c0a 6b02 1900 a002  j.|.d...|.k.....
-00003130: a100 7d12 7c02 6a01 7c02 6405 1900 7c0a  ..}.|.j.|.d...|.
-00003140: 6b02 1900 a002 a100 7d13 7c02 6405 1900  k.......}.|.d...
-00003150: 7c0a 6b02 7d14 7407 7c04 8301 6409 6b02  |.k.}.t.|...d.k.
-00003160: 9003 7226 640c 7d0b 640c 7d0c 6e62 740b  ..r&d.}.d.}.nbt.
-00003170: 7c04 7c0a 8302 7d0d 7c03 6a01 7c03 6405  |.|...}.|.j.|.d.
-00003180: 1900 a00c 7c0d a101 1900 a002 a100 7d0e  ....|.........}.
-00003190: 7407 7c0e 8301 6409 6b04 9003 7280 740d  t.|...d.k...r.t.
-000031a0: 7c0e 640d 1900 6a04 8301 7d0b 7405 6a0e  |.d...j...}.t.j.
-000031b0: 7c0e 640e 1900 6a04 7c0e 640d 1900 6a04  |.d...j.|.d...j.
-000031c0: 640f 8d02 7d0c 6e08 640c 7d0b 640c 7d0c  d...}.n.d.}.d.}.
-000031d0: 7407 7c13 8301 6409 6b01 9003 729a 9002  t.|...d.k...r...
-000031e0: 71b0 7407 7c12 8301 640a 6b02 9005 721e  q.t.|...d.k...r.
-000031f0: 7c13 640d 1900 6a04 6409 1900 7c12 6410  |.d...j.d...|.d.
-00003200: 1900 6a04 6409 1900 1700 7c0b 1700 7c02  ..j.d.....|...|.
-00003210: 6a01 7c14 6410 6602 3c00 7c12 6411 1900  j.|.d.f.<.|.d...
-00003220: 6a04 6409 1900 7c02 6a01 7c14 6411 6602  j.d...|.j.|.d.f.
-00003230: 3c00 7c12 6412 1900 6a04 6409 1900 640a  <.|.d...j.d...d.
-00003240: 1700 7c02 6a01 7c14 6412 6602 3c00 7c12  ..|.j.|.d.f.<.|.
-00003250: 6413 1900 6a04 6409 1900 7c02 6a01 7c14  d...j.d...|.j.|.
-00003260: 6413 6602 3c00 6414 7c02 6a00 7600 9005  d.f.<.d.|.j.v...
-00003270: 7208 7405 a010 7c12 6414 1900 6a04 6409  r.t...|.d...j.d.
-00003280: 1900 6409 a102 7c13 6417 1900 6a04 6409  ..d...|.d...j.d.
-00003290: 1900 1700 7c02 6a01 7c14 6414 6602 3c00  ....|.j.|.d.f.<.
-000032a0: 7c13 6418 1900 6a04 6409 1900 7405 a010  |.d...j.d...t...
-000032b0: 7c12 6414 1900 6a04 6409 1900 6409 a102  |.d...j.d...d...
-000032c0: 1400 7c12 6414 1900 6a04 6409 1900 7c12  ..|.d...j.d...|.
-000032d0: 6416 1900 6a04 6409 1900 1400 1700 7c02  d...j.d.......|.
-000032e0: 6a01 7c14 6414 6602 1900 1b00 7c02 6a01  j.|.d.f.....|.j.
-000032f0: 7c14 6416 6602 3c00 7c13 640e 1900 6a04  |.d.f.<.|.d...j.
-00003300: 6409 1900 7c13 640d 1900 6a04 6409 1900  d...|.d...j.d...
-00003310: 1400 7c0b 7c0c 1400 1700 7c12 641d 1900  ..|.|.....|.d...
-00003320: 6a04 6409 1900 7c12 6410 1900 6a04 6409  j.d...|.d...j.d.
-00003330: 1900 1400 1700 7c02 6a01 7c14 6410 6602  ......|.j.|.d.f.
-00003340: 1900 1b00 7c02 6a01 7c14 641d 6602 3c00  ....|.j.|.d.f.<.
-00003350: 740a 7c13 6406 1900 6a04 6409 1900 8301  t.|.d...j.d.....
-00003360: 7d0a 9002 71c2 7405 a011 7c12 6411 1900  }...q.t...|.d...
-00003370: 6a04 a101 6409 6b04 9007 7226 6414 7c12  j...d.k...r&d.|.
-00003380: 6a00 7600 9005 724e 7c12 6a12 6414 641e  j.v...rN|.j.d.d.
-00003390: 641f 8d02 7d12 7c13 640d 1900 6a04 6409  d...}.|.d...j.d.
-000033a0: 1900 7405 a00d 7c12 6410 1900 6a04 a101  ..t...|.d...j...
-000033b0: 1700 7c0b 1700 7c02 6a01 7c14 6410 6602  ..|...|.j.|.d.f.
-000033c0: 3c00 6414 7c02 6a00 7600 9006 7264 7405  <.d.|.j.v...rdt.
-000033d0: a010 7c12 6414 1900 6a04 6409 1900 6409  ..|.d...j.d...d.
-000033e0: a102 7c13 6417 1900 6a04 6409 1900 1700  ..|.d...j.d.....
-000033f0: 7c02 6a01 7c14 6414 6602 3c00 7c13 6418  |.j.|.d.f.<.|.d.
-00003400: 1900 6a04 6409 1900 7405 a010 7c12 6414  ..j.d...t...|.d.
-00003410: 1900 6a04 6409 1900 6409 a102 1400 7c12  ..j.d...d.....|.
-00003420: 6414 1900 6a04 6409 1900 7c12 6416 1900  d...j.d...|.d...
-00003430: 6a04 6409 1900 1400 1700 7c02 6a01 7c14  j.d.......|.j.|.
-00003440: 6414 6602 1900 1b00 7c02 6a01 7c14 6416  d.f.....|.j.|.d.
-00003450: 6602 3c00 7c13 640e 1900 6a04 6409 1900  f.<.|.d...j.d...
-00003460: 7c13 640d 1900 6a04 6409 1900 1400 7c0b  |.d...j.d.....|.
-00003470: 7c0c 1400 1700 7c12 641d 1900 6a04 6409  |.....|.d...j.d.
-00003480: 1900 7c12 6410 1900 6a04 6409 1900 1400  ..|.d...j.d.....
-00003490: 1700 7c02 6a01 7c14 6410 6602 1900 1b00  ..|.j.|.d.f.....
-000034a0: 7c02 6a01 7c14 641d 6602 3c00 7405 a011  |.j.|.d.f.<.t...
-000034b0: 7c12 6411 1900 6a04 a101 7405 a010 7c12  |.d...j...t...|.
-000034c0: 6411 1900 6a04 a101 6b02 9006 72cc 7c12  d...j...k...r.|.
-000034d0: 6411 1900 6a04 6409 1900 640a 1700 7c02  d...j.d...d...|.
-000034e0: 6a01 7c14 6411 6602 3c00 640a 7c02 6a01  j.|.d.f.<.d.|.j.
-000034f0: 7c14 6412 6602 3c00 7c07 640a 1700 7c02  |.d.f.<.|.d...|.
-00003500: 6a01 7c14 6413 6602 3c00 7c07 640a 1700  j.|.d.f.<.|.d...
-00003510: 7d07 6e46 7405 a010 7c12 6411 1900 6a04  }.nFt...|.d...j.
-00003520: a101 7d15 7c15 7c02 6a01 7c14 6411 6602  ..}.|.|.j.|.d.f.
-00003530: 3c00 640a 7c02 6a01 7c14 6412 6602 3c00  <.d.|.j.|.d.f.<.
-00003540: 7c07 640a 1700 7c02 6a01 7c14 6413 6602  |.d...|.j.|.d.f.
-00003550: 3c00 7c07 640a 1700 7d07 740a 7c13 6406  <.|.d...}.t.|.d.
-00003560: 1900 6a04 6409 1900 8301 7d0a 6e18 740a  ..j.d.....}.n.t.
-00003570: 7c0a 8301 7c0f 7c10 3c00 7c10 640a 1700  |...|.|.<.|.d...
-00003580: 7d10 6409 7d11 9002 71c2 9002 71b0 7c00  }.d.}...q...q.|.
-00003590: 6405 1900 a00c 7c02 6405 1900 6a04 a101  d.....|.d...j...
-000035a0: 7d16 7c02 6413 1900 6a04 7c00 6a01 7c16  }.|.d...j.|.j.|.
-000035b0: 6413 6602 3c00 7c02 6412 1900 6a04 7c00  d.f.<.|.d...j.|.
-000035c0: 6a01 7c16 6412 6602 3c00 7c02 6411 1900  j.|.d.f.<.|.d...
-000035d0: 6a04 7c00 6a01 7c16 6411 6602 3c00 7c02  j.|.j.|.d.f.<.|.
-000035e0: 6413 1900 6a04 7c00 6a01 7c16 6413 6602  d...j.|.j.|.d.f.
-000035f0: 3c00 7c02 6410 1900 6a04 7c00 6a01 7c16  <.|.d...j.|.j.|.
-00003600: 6410 6602 3c00 6414 7c00 6a00 7600 9008  d.f.<.d.|.j.v...
-00003610: 7206 7c02 6414 1900 6a04 7c00 6a01 7c16  r.|.d...j.|.j.|.
-00003620: 6414 6602 3c00 7c02 641d 1900 6a04 7c00  d.f.<.|.d...j.|.
-00003630: 6a01 7c16 641d 6602 3c00 7c02 6416 1900  j.|.d.f.<.|.d...
-00003640: 6a04 7c00 6a01 7c16 6416 6602 3c00 7c02  j.|.j.|.d.f.<.|.
-00003650: 6417 1900 6a04 7c00 6a01 7c16 6417 6602  d...j.|.j.|.d.f.
-00003660: 3c00 7c02 6418 1900 6a04 7c00 6a01 7c16  <.|.d...j.|.j.|.
-00003670: 6418 6602 3c00 7408 6409 7407 7c00 8301  d.f.<.t.d.t.|...
-00003680: 8302 4400 9001 5d6a 7d08 7c00 6a09 7c08  ..D...]j}.|.j.|.
-00003690: 1900 7d09 7c00 7c01 1900 6a04 7c08 1900  ..}.|.|...j.|...
-000036a0: 6409 6b04 9008 72a2 7c00 6420 1900 6a04  d.k...r.|.d ..j.
-000036b0: 7c08 1900 6409 6b04 9008 72a2 7c00 6410  |...d.k...r.|.d.
-000036c0: 1900 6a04 7c08 1900 6421 1b00 6421 1b00  ..j.|...d!..d!..
-000036d0: 7c00 6420 1900 6a04 7c08 1900 1b00 7c00  |.d ..j.|.....|.
-000036e0: 6a01 7c09 6422 6602 3c00 7c00 6403 1900  j.|.d"f.<.|.d...
-000036f0: 6a04 7c08 1900 6404 6b02 9008 723c 7c00  j.|...d.k...r<|.
-00003700: 6405 1900 6a04 7c08 1900 7d0a 740b 7c04  d...j.|...}.t.|.
-00003710: 7c0a 8302 7d0d 7c03 6a01 7c03 6405 1900  |...}.|.j.|.d...
-00003720: a00c 7c0d a101 1900 6a02 6423 6424 8d01  ..|.....j.d#d$..
-00003730: 7d0e 740d 7c0e 640d 1900 6a04 8301 7d17  }.t.|.d...j...}.
-00003740: 7c17 7c00 6a01 7c09 6410 6602 3c00 7405  |.|.j.|.d.f.<.t.
-00003750: 6a0e 7c0e 640e 1900 6a04 7c0e 640d 1900  j.|.d...j.|.d...
-00003760: 6a04 640f 8d02 7c00 6a01 7c09 641d 6602  j.d...|.j.|.d.f.
-00003770: 3c00 6415 7c00 6a01 7c09 6417 6602 3c00  <.d.|.j.|.d.f.<.
-00003780: 6415 7c00 6a01 7c09 6418 6602 3c00 6415  d.|.j.|.d.f.<.d.
-00003790: 7c00 6a01 7c09 6419 6602 3c00 6415 7c00  |.j.|.d.f.<.d.|.
-000037a0: 6a01 7c09 641c 6602 3c00 6415 7c00 6a01  j.|.d.f.<.d.|.j.
-000037b0: 7c09 641a 6602 3c00 6415 7c00 6a01 7c09  |.d.f.<.d.|.j.|.
-000037c0: 641b 6602 3c00 6414 7c00 6a00 7600 9008  d.f.<.d.|.j.v...
-000037d0: 723c 6415 7c00 6a01 7c09 6416 6602 3c00  r<d.|.j.|.d.f.<.
-000037e0: 6415 7c00 6a01 7c09 6414 6602 3c00 9008  d.|.j.|.d.f.<...
-000037f0: 713c 7c00 5300 2925 7ac0 4675 6e63 7469  q<|.S.)%z.Functi
-00003800: 6f6e 7320 7769 6c6c 2020 6361 6c63 7561  ons will  calcua
-00003810: 7465 2073 7472 6561 6d20 6f72 6465 7220  te stream order 
-00003820: 616e 640a 2020 2020 2020 2020 7570 6461  and.        upda
-00003830: 7465 2064 7261 696e 6167 6520 6172 6561  te drainage area
-00003840: 2069 6e20 7468 6520 6174 7472 6962 7574   in the attribut
-00003850: 6520 7461 626c 6520 6361 7469 6e66 6f61  e table catinfoa
-00003860: 6c6c 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  ll.    ---------
-00003870: 2d0a 0a20 2020 204e 6f74 6573 0a20 2020  -..    Notes.   
-00003880: 202d 2d2d 2d2d 2d2d 0a0a 2020 2020 5265   -------..    Re
-00003890: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-000038a0: 2d2d 0a20 2020 2020 2020 2063 6174 696e  --.        catin
-000038b0: 666f 616c 6c0a 2020 2020 726a 0000 0072  foall.    rj...r
-000038c0: 6b00 0000 724b 0000 0072 4c00 0000 7206  k...rK...rL...r.
-000038d0: 0000 0072 4900 0000 724a 0000 0069 f7ff  ...rI...rJ...i..
-000038e0: ffff 7201 0000 0072 4f00 0000 7250 0000  ..r....rO...rP..
-000038f0: 0072 4d00 0000 7269 0000 0072 7e00 0000  .rM...ri...r~...
-00003900: 727c 0000 0072 6000 0000 7259 0000 0072  r|...r`...rY...r
-00003910: 5b00 0000 725a 0000 0072 5700 0000 7251  [...rZ...rW...rQ
-00003920: 0000 0072 5800 0000 724e 0000 0072 5200  ...rX...rN...rR.
-00003930: 0000 7254 0000 0072 5600 0000 7253 0000  ..rT...rV...rS..
-00003940: 0072 5500 0000 5a08 4441 5f53 6c6f 7065  .rU...Z.DA_Slope
-00003950: 4672 1000 0000 da06 4441 5f4f 6273 e700  Fr......DA_Obs..
-00003960: 0000 0000 408f 40da 0844 415f 6572 726f  ....@.@..DA_erro
-00003970: 7254 7208 0000 0029 1372 0b00 0000 7223  rTr....).r....r#
-00003980: 0000 0072 1600 0000 725c 0000 0072 2000  ...r....r\...r .
-00003990: 0000 7221 0000 0072 6400 0000 721f 0000  ..r!...rd...r...
-000039a0: 0072 1e00 0000 723e 0000 00da 0369 6e74  .r....r>.....int
-000039b0: 7285 0000 0072 3d00 0000 7219 0000 0072  r....r=...r....r
-000039c0: 8800 0000 723c 0000 0072 6500 0000 7289  ....r<...re...r.
-000039d0: 0000 0072 1c00 0000 2918 5a0a 6361 7469  ...r....).Z.cati
-000039e0: 6e66 6f61 6c6c 7276 0000 0072 5d00 0000  nfoallrv...r]...
-000039f0: 5a0b 6361 7469 6e66 6f5f 6e63 6c5a 0b72  Z.catinfo_nclZ.r
-00003a00: 6f75 7469 6e67 5f6e 636c 5a07 6361 746c  outing_nclZ.catl
-00003a10: 6973 745a 0469 6361 74da 0469 7365 6772  istZ.icat..isegr
-00003a20: 2800 0000 7245 0000 00da 0563 6174 6964  (...rE.....catid
-00003a30: 5a06 4441 5f6e 636c 5a07 736c 705f 6e63  Z.DA_nclZ.slp_nc
-00003a40: 6c5a 0c55 7073 7472 6561 6d63 6174 735a  lZ.UpstreamcatsZ
-00003a50: 0b55 705f 6361 745f 696e 666f 5a0a 6e65  .Up_cat_infoZ.ne
-00003a60: 7763 6174 6c69 7374 5a09 696e 6577 7374  wcatlistZ.inewst
-00003a70: 6172 745a 0b46 5f69 6e74 6572 7365 6374  artZ.F_intersect
-00003a80: 5a0f 5570 5f52 6561 6368 6573 5f69 6e66  Z.Up_Reaches_inf
-00003a90: 6f5a 0e63 7572 5f52 6561 6368 5f69 6e66  oZ.cur_Reach_inf
-00003aa0: 6f5a 0a63 7572 6361 745f 6964 785a 0d6d  oZ.curcat_idxZ.m
-00003ab0: 6178 5f73 7472 616f 7264 6572 722c 0000  ax_straorderr,..
-00003ac0: 005a 0244 4172 2d00 0000 722d 0000 0072  .Z.DAr-...r-...r
-00003ad0: 2e00 0000 7296 0000 00cc 0200 0073 6c01  ....r........sl.
-00003ae0: 0000 000c 0401 0a01 0402 0401 0aff 0803  ................
-00003af0: 1601 1402 1001 0401 0402 1401 0a01 1c01  ................
-00003b00: 0e01 0e02 16ff 0203 0201 0cff 0805 0e01  ................
-00003b10: 0401 0602 0a01 0401 0cff 0804 0e01 0e01  ................
-00003b20: 1c02 0401 0402 1c01 0e01 0e01 0e02 0c01  ................
-00003b30: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
-00003b40: 3c0b 0801 0a02 0a01 0c03 1001 0402 1401  <...............
-00003b50: 0801 0402 1401 1601 1601 0c03 0e01 0401  ................
-00003b60: 0605 0a01 0401 0cff 0803 0e01 0e01 1c02  ................
-00003b70: 0401 0403 0aff 0403 0402 0e02 0c01 0cff  ................
-00003b80: 0202 02fe 02ff 0c05 0201 02ff 0402 02fe  ................
-00003b90: 0e04 10ff 0c05 1802 0c01 2e02 2201 1aff  ............"...
-00003ba0: 0201 0cff 0e03 1a01 06ff 0202 1afe 0203  ................
-00003bb0: 0cfd 0e10 1603 12ff 0404 0c01 0e03 0c01  ................
-00003bc0: 0eff 0202 02fe 02ff 0c06 0c01 2e02 2201  ..............".
-00003bd0: 1aff 0201 0cff 0e03 1a01 06ff 0202 1afe  ................
-00003be0: 0203 0cfd 0e0e 1201 08ff 0804 10ff 0c03  ................
-00003bf0: 0e01 1201 0a03 1001 0e01 0e01 1201 0802  ................
-00003c00: 1402 0c01 0801 0c02 1401 1401 1401 1401  ................
-00003c10: 1401 1401 0c01 1401 1401 1401 1401 1409  ................
-00003c20: 1401 0a04 1401 1402 1401 0cfe 0e06 1401  ................
-00003c30: 0e02 0a01 1c01 0e01 0e02 2403 0e01 0e01  ..........$.....
-00003c40: 0e01 0e01 0e01 0e02 0c01 0e01 120c 7296  ..............r.
-00003c50: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00003c60: 0b00 0000 0600 0000 4300 0000 7320 0100  ........C...s ..
-00003c70: 0074 00a0 0164 017c 01a1 027d 0274 00a0  .t...d.|...}.t..
-00003c80: 0174 027c 0083 0164 0217 0064 0266 0264  .t.|...d...d.f.d
-00003c90: 03a1 027d 0364 047d 0474 03a0 037c 00a1  ...}.d.}.t...|..
-00003ca0: 017d 0574 027c 0283 0164 046b 0490 0172  .}.t.|...d.k...r
-00003cb0: 0674 00a0 0174 027c 0083 0164 0217 0064  .t...t.|...d...d
-00003cc0: 0266 0264 03a1 027d 0664 047d 0774 0464  .f.d...}.d.}.t.d
-00003cd0: 0474 027c 0283 0183 0244 005d 827d 087c  .t.|.....D.].}.|
-00003ce0: 027c 0819 007c 037c 043c 007c 0464 0217  .|...|.|.<.|.d..
-00003cf0: 007d 0474 00a0 057c 0564 0564 0585 0264  .}.t...|.d.d...d
-00003d00: 0266 0219 007c 027c 0819 006b 02a1 01a0  .f...|.|...k....
-00003d10: 0674 07a1 017d 0974 0464 0474 027c 0983  .t...}.t.d.t.|..
-00003d20: 0183 0244 005d 367d 0a7c 057c 097c 0a19  ...D.]6}.|.|.|..
-00003d30: 0064 0466 0219 007c 0376 0072 ce71 b47c  .d.f...|.v.r.q.|
-00003d40: 057c 097c 0a19 0064 0466 0219 007c 067c  .|.|...d.f...|.|
-00003d50: 073c 007c 0764 0217 007d 0771 b471 6a74  .<.|.d...}.q.qjt
-00003d60: 00a0 087c 06a1 017d 067c 067c 0664 046b  ...|...}.|.|.d.k
-00003d70: 0519 007d 0271 3274 00a0 087c 03a1 017d  ...}.q2t...|...}
-00003d80: 037c 037c 0364 046b 0519 007d 037c 0353  .|.|.d.k...}.|.S
-00003d90: 0029 067a 9f46 756e 6374 696f 6e73 2077  .).z.Functions w
-00003da0: 696c 6c20 7265 7475 726e 2075 7073 7472  ill return upstr
-00003db0: 6561 6d20 6964 7320 696e 206f 7574 2074  eam ids in out t
-00003dc0: 6168 7420 6472 6169 6e61 6765 0a20 2020  aht drainage.   
-00003dd0: 2020 2020 2074 6f20 6f75 746c 6574 6964       to outletid
-00003de0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00003df0: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
-00003e00: 2d2d 2d2d 2d2d 0a0a 2020 2020 5265 7475  ------..    Retu
-00003e10: 726e 733a 0a20 2020 202d 2d2d 2d2d 2d2d  rns:.    -------
-00003e20: 0a20 2020 2020 2020 2053 6865 6469 640a  .        Shedid.
-00003e30: 2020 2020 2902 724f 0000 0072 4f00 0000      ).rO...rO...
-00003e40: 724f 0000 006c fdff ffff ff67 ed10 5d00  rO...l.....g..].
-00003e50: 7201 0000 004e 2909 7221 0000 0072 6400  r....N).r!...rd.
-00003e60: 0000 721f 0000 0072 1600 0000 721e 0000  ..r....r....r...
-00003e70: 00da 0861 7267 7768 6572 6572 5c00 0000  ...argwherer\...
-00003e80: 72a3 0000 0072 3c00 0000 290b da03 6f75  r....r<...)...ou
-00003e90: 74da 086f 7574 6c65 7469 645a 076f 7473  t..outletidZ.ots
-00003ea0: 6865 6473 5a06 5368 6564 6964 5a04 7073  hedsZ.ShedidZ.ps
-00003eb0: 6964 da04 726f 7574 5a07 6e6f 7574 7368  id..routZ.noutsh
-00003ec0: 645a 0770 6f73 6864 6964 7228 0000 005a  dZ.poshdidr(...Z
-00003ed0: 0469 726f 7772 4400 0000 722d 0000 0072  .irowrD...r-...r
-00003ee0: 2d00 0000 722e 0000 0072 8500 0000 eb03  -...r....r......
-00003ef0: 0000 732a 0000 0000 0c0c 0118 0104 010a  ..s*............
-00003f00: 010e 0118 0104 0212 030c 0308 0124 0212  .............$..
-00003f10: 0214 0102 0114 010c 010a 010e 010a 010c  ................
-00003f20: 0172 8500 0000 6303 0000 0000 0000 0000  .r....c.........
-00003f30: 0000 000d 0000 0006 0000 0043 0000 0073  ...........C...s
-00003f40: a601 0000 7c02 6401 6402 6702 1900 a000  ....|.d.d.g.....
-00003f50: 6403 a101 6a01 7d03 7402 6404 7403 7c02  d...j.}.t.d.t.|.
-00003f60: 8301 8302 4400 9001 5d78 7d04 7c02 6401  ....D...]x}.|.d.
-00003f70: 1900 6a01 7c04 1900 7d05 7c02 6405 1900  ..j.|...}.|.d...
-00003f80: 6a01 7c04 1900 7d06 7c00 6a04 7c00 6406  j.|...}.|.j.|.d.
-00003f90: 1900 7c05 6b02 1900 a005 a100 7d07 7403  ..|.k.......}.t.
-00003fa0: 7406 7c03 7c05 8302 8301 7c02 6a04 7c02  t.|.|.....|.j.|.
-00003fb0: 6401 1900 7c05 6b02 6407 6602 3c00 7403  d...|.k.d.f.<.t.
-00003fc0: 7c07 8301 6404 6b01 7288 7122 7c07 6408  |...d.k.r.q"|.d.
-00003fd0: 1900 6409 6b02 7d08 7c07 6a04 7c08 640a  ..d.k.}.|.j.|.d.
-00003fe0: 6602 1900 6a01 6404 1900 7d09 7c09 7c02  f...j.d...}.|.|.
-00003ff0: 6a04 7c02 6401 1900 7c05 6b02 640b 6602  j.|.d...|.k.d.f.
-00004000: 3c00 7c02 6402 1900 6a01 7c04 1900 7d0a  <.|.d...j.|...}.
-00004010: 7c0a 6404 6b00 72d6 7122 7c01 6a04 7c01  |.d.k.r.q"|.j.|.
-00004020: 6405 1900 7c06 6b02 1900 a005 a100 7d0b  d...|.k.......}.
-00004030: 7403 7c0b 8301 640c 6b02 9001 722a 7c0a  t.|...d.k...r*|.
-00004040: 640d 6b03 9001 722a 7c0b 640a 1900 6a01  d.k...r*|.d...j.
-00004050: 6404 1900 7d0c 7c0c 7c00 6a04 7c00 640a  d...}.|.|.j.|.d.
-00004060: 1900 7c09 6b02 6408 6602 3c00 7122 7c0a  ..|.k.d.f.<.q"|.
-00004070: 640d 6b02 9001 724c 6409 7c00 6a04 7c00  d.k...rLd.|.j.|.
-00004080: 640a 1900 7c09 6b02 6408 6602 3c00 7122  d...|.k.d.f.<.q"
-00004090: 7407 640e 8301 0100 7407 640f 7c05 6410  t.d.....t.d.|.d.
-000040a0: 7c0a 8304 0100 7407 7c0a 7c06 8302 0100  |.....t.|.|.....
-000040b0: 7407 7c0b 8301 0100 7407 7c09 8301 0100  t.|.....t.|.....
-000040c0: 7407 7c01 6405 640a 6702 1900 8301 0100  t.|.d.d.g.......
-000040d0: 7407 6411 8301 0100 7407 640e 8301 0100  t.d.....t.d.....
-000040e0: 7122 7c00 7c02 6602 5300 2912 612b 0400  q"|.|.f.S.).a+..
-000040f0: 004d 6f64 6966 7920 6f75 746c 6574 2073  .Modify outlet s
-00004100: 7562 6261 7369 6e27 7320 646f 776e 7374  ubbasin's downst
-00004110: 7265 616d 2073 7562 6261 7369 6e20 4944  ream subbasin ID
-00004120: 2066 6f72 2065 6163 6820 7375 6272 6567   for each subreg
-00004130: 696f 6e0a 2020 2020 5061 7261 6d65 7465  ion.    Paramete
-00004140: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00004150: 2d0a 2020 2020 416c 6c43 6174 696e 666f  -.    AllCatinfo
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 2020 2020 3a20 6461 7461 6672          : datafr
-00004180: 616d 650a 2020 2020 2020 2020 6974 2069  ame.        it i
-00004190: 7320 6120 6461 7461 6672 616d 6520 6f66  s a dataframe of
-000041a0: 2074 6865 2061 7474 7269 6275 7465 2074   the attribute t
-000041b0: 6162 6c65 2072 6561 6465 6420 6672 6f6d  able readed from
-000041c0: 2066 696e 616c 6361 745f 696e 666f 0a20   finalcat_info. 
-000041d0: 2020 2020 2020 202e 7368 7020 6f72 2066         .shp or f
-000041e0: 696e 616c 7269 7670 6c79 5f69 6e66 6f2e  inalrivply_info.
-000041f0: 7368 700a 2020 2020 446f 776e 4361 7469  shp.    DownCati
-00004200: 6e66 6f20 2020 2020 2020 2020 2020 2020  nfo             
-00004210: 2020 2020 2020 2020 2020 3a20 6461 7461            : data
-00004220: 6672 616d 650a 2020 2020 2020 2020 4974  frame.        It
-00004230: 2069 7320 6120 6461 7461 6672 616d 6520   is a dataframe 
-00004240: 696e 636c 7564 6573 2074 776f 2063 6f6c  includes two col
-00004250: 756d 6e73 3a0a 2020 2020 2020 2020 2753  umns:.        'S
-00004260: 7562 5f52 6567 5f49 4427 3a20 7468 6520  ub_Reg_ID': the 
-00004270: 7375 6272 6567 696f 6e20 6964 0a20 2020  subregion id.   
-00004280: 2020 2020 2027 446f 775f 5375 625f 5265       'Dow_Sub_Re
-00004290: 675f 4964 273a 2064 6f77 6e73 7472 6561  g_Id': downstrea
-000042a0: 6d20 7375 6262 6173 696e 2069 6420 6f66  m subbasin id of
-000042b0: 2074 6865 206f 7574 6c65 7420 7375 6262   the outlet subb
-000042c0: 6173 696e 2069 6e0a 2020 2020 2020 2020  asin in.        
-000042d0: 7468 6973 2073 7562 7265 6769 6f6e 0a20  this subregion. 
-000042e0: 2020 2053 7562 5f52 6567 696f 6e5f 696e     Sub_Region_in
-000042f0: 666f 2020 2020 2020 2020 2020 2020 2020  fo              
-00004300: 2020 2020 203a 2064 6174 6166 7261 6d65       : dataframe
-00004310: 0a20 2020 2020 2020 2049 7420 6973 2061  .        It is a
-00004320: 2064 6174 6166 7261 6d65 2069 6e63 6c75   dataframe inclu
-00004330: 6465 7320 7375 6272 6567 696f 6e20 696e  des subregion in
-00004340: 666f 726d 6174 696f 6e73 2c20 7769 7468  formations, with
-00004350: 2066 6f6c 6c6f 7769 6e67 0a20 2020 2020   following.     
-00004360: 2020 2063 6f6c 756d 6e73 3a0a 2020 2020     columns:.    
-00004370: 2020 2020 2753 7562 5f52 6567 5f49 4427      'Sub_Reg_ID'
-00004380: 203a 2074 6865 2073 7562 7265 6769 6f6e   : the subregion
-00004390: 2069 640a 2020 2020 2020 2020 2744 6f77   id.        'Dow
-000043a0: 5f53 7562 5f52 6567 5f49 6427 3a20 7468  _Sub_Reg_Id': th
-000043b0: 6520 646f 776e 7374 7265 616d 2073 7562  e downstream sub
-000043c0: 7265 6769 6f6e 2069 640a 0a20 2020 204e  region id..    N
-000043d0: 6f74 6573 0a20 2020 202d 2d2d 2d2d 2d2d  otes.    -------
-000043e0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000043f0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00004400: 2020 2053 7562 5f52 6567 696f 6e5f 696e     Sub_Region_in
-00004410: 666f 2020 2020 2020 3a20 6461 7461 6672  fo      : datafr
-00004420: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00004430: 416e 206e 6577 2063 6f6c 756d 6e73 2069  An new columns i
-00004440: 6e64 6963 6174 6520 7468 6520 6f75 746c  ndicate the outl
-00004450: 6574 2073 7562 6261 7369 6e20 6964 206f  et subbasin id o
-00004460: 6620 7468 6520 7375 6220 7265 6769 6f6e  f the sub region
-00004470: 0a20 2020 2020 2020 2020 2020 2077 696c  .            wil
-00004480: 6c20 6265 2061 6464 6564 0a20 2020 2020  l be added.     
-00004490: 2020 2041 6c6c 4361 7469 6e66 6f20 2020     AllCatinfo   
-000044a0: 2020 2020 2020 2020 3a20 6461 7461 6672          : datafr
-000044b0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-000044c0: 446f 776e 7374 7265 616d 2073 7562 6261  Downstream subba
-000044d0: 7369 6e20 4944 206f 6620 6561 6368 2073  sin ID of each s
-000044e0: 7562 7265 6769 6f6e 2773 206f 7574 6c65  ubregion's outle
-000044f0: 7420 7375 6262 6173 696e 2077 696c 6c0a  t subbasin will.
-00004500: 2020 2020 2020 2020 2020 2020 6265 2075              be u
-00004510: 7064 6174 6564 2e0a 2020 2020 da0a 5375  pdated..    ..Su
-00004520: 625f 5265 675f 4944 da0e 446f 775f 5375  b_Reg_ID..Dow_Su
-00004530: 625f 5265 675f 4964 724a 0000 0072 0100  b_Reg_IdrJ...r..
-00004540: 0000 da07 494c 7074 5f49 44da 0952 6567  ....ILpt_ID..Reg
-00004550: 696f 6e5f 4944 da0e 4e5f 5570 5f53 7562  ion_ID..N_Up_Sub
-00004560: 5265 6769 6f6e 7249 0000 0072 5000 0000  RegionrI...rP...
-00004570: 7206 0000 00da 0c4f 7574 6c65 745f 5375  r......Outlet_Su
-00004580: 6249 6472 4f00 0000 e97f 3801 007a 3223  bIdrO.....8..z2#
-00004590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000045a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000045b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000045c0: 237a 0c53 7562 7265 6769 6f6e 203a 207a  #z.Subregion : z
-000045d0: 0720 2020 546f 2020 7a1a 4e65 6564 2062  .   To  z.Need b
-000045e0: 6520 6d61 6e75 616c 6c79 2063 6f6e 6e65  e manually conne
-000045f0: 6374 6564 2908 725c 0000 0072 2000 0000  cted).r\...r ...
-00004600: 721e 0000 0072 1f00 0000 7223 0000 0072  r....r....r#...r
-00004610: 1600 0000 7285 0000 0072 7300 0000 290d  ....r....rs...).
-00004620: da0a 416c 6c43 6174 696e 666f 5a0b 446f  ..AllCatinfoZ.Do
-00004630: 776e 4361 7469 6e66 6fda 0f53 7562 5f52  wnCatinfo..Sub_R
-00004640: 6567 696f 6e5f 696e 666f 725e 0000 0072  egion_infor^...r
-00004650: 2800 0000 5a0a 6973 7562 7265 6769 6f6e  (...Z.isubregion
-00004660: 72ac 0000 005a 1353 7562 5f52 6567 696f  r....Z.Sub_Regio
-00004670: 6e5f 6361 745f 696e 666f 5a0b 6f75 746c  n_cat_infoZ.outl
-00004680: 6574 5f6d 6173 6b5a 1169 5265 675f 4f75  et_maskZ.iReg_Ou
-00004690: 746c 6574 5f53 7562 6964 5a11 446f 775f  tlet_SubidZ.Dow_
-000046a0: 5375 625f 5265 6769 6f6e 5f69 64da 0d44  Sub_Region_id..D
-000046b0: 6f77 6e5f 5375 625f 696e 666f 5a09 446f  own_Sub_infoZ.Do
-000046c0: 776e 5375 6269 6472 2d00 0000 722d 0000  wnSubidr-...r-..
-000046d0: 0072 2e00 0000 da22 436f 6e6e 6563 745f  .r....."Connect_
-000046e0: 5375 6252 6567 696f 6e5f 5570 6461 7465  SubRegion_Update
-000046f0: 5f44 6f77 6e53 7562 4964 1504 0000 7352  _DownSubId....sR
-00004700: 0000 0000 2312 ff02 0314 030e 020e 0204  ....#...........
-00004710: 010a ff08 060c fe04 010e ff02 050c 0102  ................
-00004720: 030c 0114 0402 fe04 010e ff02 040e 0408  ................
-00004730: 0102 0316 0218 010e 0302 fe04 010e ff04  ................
-00004740: 060a 0118 0208 010e 010a 0108 0108 0110  ................
-00004750: 0108 010a 0172 b400 0000 6304 0000 0000  .....r....c.....
-00004760: 0000 0000 0000 001b 0000 000a 0000 0043  ...............C
-00004770: 0000 0073 0e05 0000 6401 7d04 6402 7d05  ...s....d.}.d.}.
-00004780: 7c01 7c01 6403 1900 6404 6b02 1900 6405  |.|.d...d.k...d.
-00004790: 1900 6a00 7d06 7401 a002 7c06 a101 7d06  ..j.}.t...|...}.
-000047a0: 7c06 a003 a100 7d06 7404 7c00 6a05 7c00  |.....}.t.|.j.|.
-000047b0: 6406 1900 6407 6b02 1900 8301 6404 6b04  d...d.k.....d.k.
-000047c0: 726c 7406 6408 8301 0100 7406 7c00 6a05  rlt.d.....t.|.j.
-000047d0: 7c00 6406 1900 6407 6b02 1900 8301 0100  |.d...d.k.......
-000047e0: 7c00 5300 7404 7c00 6a05 7c00 6406 1900  |.S.t.|.j.|.d...
-000047f0: 6407 6b02 1900 8301 6409 6b02 7292 7406  d.k.....d.k.r.t.
-00004800: 640a 8301 0100 7c00 5300 7c00 6a05 7c00  d.....|.S.|.j.|.
-00004810: 6406 1900 6407 6b02 1900 640b 1900 6a00  d...d.k...d...j.
-00004820: 6409 1900 a007 7408 a101 7d07 640c 7d08  d.....t...}.d.}.
-00004830: 7409 6409 7404 7c01 8301 8302 4400 5d94  t.d.t.|.....D.].
-00004840: 7d09 7c01 640d 1900 6a00 7c09 1900 7d0a  }.|.d...j.|...}.
-00004850: 7c08 7c00 6a05 7c00 640b 1900 7c0a 6b02  |.|.j.|.d...|.k.
-00004860: 1900 640e 1900 6a00 6409 1900 1700 7d08  ..d...j.d.....}.
-00004870: 7406 640f 7c01 6405 1900 6a00 7c09 1900  t.d.|.d...j.|...
-00004880: 8302 0100 7406 6410 7c00 6a05 7c00 640b  ....t.d.|.j.|.d.
-00004890: 1900 7c0a 6b02 1900 640e 1900 6a00 6409  ..|.k...d...j.d.
-000048a0: 1900 8302 0100 7406 6411 740a 7c00 6a05  ......t.d.t.|.j.
-000048b0: 7c00 6412 1900 7c01 6405 1900 6a00 7c09  |.d...|.d...j.|.
-000048c0: 1900 6b02 1900 6413 1900 6a00 8301 8302  ..k...d...j.....
-000048d0: 0100 71c6 6404 7d0b 7404 7c06 8301 6409  ..q.d.}.t.|...d.
-000048e0: 6b04 9004 72be 7406 6414 7c0b 8302 0100  k...r.t.d.|.....
-000048f0: 7406 7c06 8301 0100 740b a00b 7c06 a101  t.|.....t...|...
-00004900: 7d0c 6700 7d06 7409 6409 7404 7c0c 8301  }.g.}.t.d.t.|...
-00004910: 8302 4400 9003 5d06 7d09 7c0c 7c09 1900  ..D...].}.|.|...
-00004920: 7d0d 7c0d 6415 6b02 9001 72b8 9001 719c  }.|.d.k...r...q.
-00004930: 7c01 7c01 6405 1900 7c0d 6b02 1900 6416  |.|.d...|.k...d.
-00004940: 1900 6a00 6409 1900 7d0e 7c06 a00c 7c0e  ..j.d...}.|...|.
-00004950: a101 0100 7c01 7c01 6405 1900 7c0d 6b02  ....|.|.d...|.k.
-00004960: 1900 640d 1900 6a00 6409 1900 7d0a 7c00  ..d...j.d...}.|.
-00004970: 6a05 7c00 640b 1900 7c0a 6b02 1900 a00b  j.|.d...|.k.....
-00004980: a100 7d0f 7c0f 6406 1900 6a00 6409 1900  ..}.|.d...j.d...
-00004990: 7d10 7404 7c00 6a05 7c00 640b 1900 7c10  }.t.|.j.|.d...|.
-000049a0: 6b02 1900 8301 6409 6b01 9002 7274 7408  k.....d.k...rtt.
-000049b0: 7c0d 8301 7408 7c07 8301 6b03 9001 729c  |...t.|...k...r.
-000049c0: 7406 6417 7c0d 8302 0100 7406 6418 7c0a  t.d.|.....t.d.|.
-000049d0: 6419 7c10 7c07 7408 7c0d 8301 7408 7c07  d.|.|.t.|...t.|.
-000049e0: 8301 6b03 8306 0100 9001 719c 7c00 6a05  ..k.......q.|.j.
-000049f0: 7c00 640b 1900 7c10 6b02 1900 6412 1900  |.d...|.k...d...
-00004a00: 6a00 6409 1900 7d11 7406 6417 7c0d 7c11  j.d...}.t.d.|.|.
-00004a10: 7c0e 7c10 8305 0100 7c11 7c0e 6b03 9002  |.|.....|.|.k...
-00004a20: 72bc 7406 6417 7c0d 641a 7c0e 8304 0100  r.t.d.|.d.|.....
-00004a30: 9001 719c 7c11 7c0e 6b02 9001 729c 7c10  ..q.|.|.k...r.|.
-00004a40: 7d12 7406 6417 7c0d 7c11 7c0e 7c10 7c12  }.t.d.|.|.|.|.|.
-00004a50: 8306 0100 7c00 6a05 7c00 640b 1900 7c12  ....|.j.|.d...|.
-00004a60: 6b02 1900 a00b a100 7d13 7c00 6a05 7c00  k.......}.|.j.|.
-00004a70: 6406 1900 7c12 6b02 1900 a00b a100 7d14  d...|.k.......}.
-00004a80: 7c13 6413 1900 6a00 6409 1900 740a 7c14  |.d...j.d...t.|.
-00004a90: 640e 1900 6a00 8301 1700 7d15 7c14 641b  d...j.....}.|.d.
-00004aa0: 1900 6a00 7d16 740d 7c16 8301 7d17 7401  ..j.}.t.|...}.t.
-00004ab0: a00a 7c16 7c17 6b02 a101 641c 6b05 9003  ..|.|.k...d.k...
-00004ac0: 7254 7c17 6404 1700 7d18 6e04 7c17 7d18  rT|.d...}.n.|.}.
-00004ad0: 7c18 7c00 6a05 7c00 640b 1900 7c12 6b02  |.|.j.|.d...|.k.
-00004ae0: 641b 6602 3c00 7c15 7c00 6a05 7c00 640b  d.f.<.|.|.j.|.d.
-00004af0: 1900 7c12 6b02 640e 6602 3c00 7c00 7c00  ..|.k.d.f.<.|.|.
-00004b00: 640b 1900 7c12 6b02 1900 641d 1900 6a00  d...|.k...d...j.
-00004b10: 6409 1900 6409 6b04 9004 721a 7c00 7c00  d...d.k...r.|.|.
-00004b20: 640b 1900 7c12 6b02 1900 641d 1900 6a00  d...|.k...d...j.
-00004b30: 6409 1900 7d19 7c00 7c00 640b 1900 7c12  d...}.|.|.d...|.
-00004b40: 6b02 1900 640e 1900 6a00 6409 1900 641e  k...d...j.d...d.
-00004b50: 1b00 641e 1b00 7d1a 7c19 6409 6b04 9004  ..d...}.|.d.k...
-00004b60: 721a 7c1a 7c19 1b00 7c00 6a05 7c00 640b  r.|.|...|.j.|.d.
-00004b70: 1900 7c12 6b02 641f 6602 3c00 6404 7c00  ..|.k.d.f.<.d.|.
-00004b80: 6a05 7c00 640b 1900 7c12 6b02 6420 6602  j.|.d...|.k.d f.
-00004b90: 3c00 7c13 6406 1900 6a00 6409 1900 7d10  <.|.d...j.d...}.
-00004ba0: 7404 7c00 6a05 7c00 640b 1900 7c10 6b02  t.|.j.|.d...|.k.
-00004bb0: 1900 8301 6409 6b01 9004 7282 7408 7c12  ....d.k...r.t.|.
-00004bc0: 8301 7408 7c07 8301 6b03 9004 72a2 7406  ..t.|...k...r.t.
-00004bd0: 6417 7c0e 8302 0100 7406 6418 7c12 6419  d.|.....t.d.|.d.
-00004be0: 7c10 7c07 7408 7c12 8301 7408 7c07 8301  |.|.t.|...t.|...
-00004bf0: 6b03 8306 0100 9001 719c 7c00 6a05 7c00  k.......q.|.j.|.
-00004c00: 640b 1900 7c10 6b02 1900 6412 1900 6a00  d...|.k...d...j.
-00004c10: 6409 1900 7d11 9002 71bc 9001 719c 740e  d...}...q...q.t.
-00004c20: 740f 7c06 8301 8301 7d06 7c0b 6404 1700  t.|.....}.|.d...
-00004c30: 7d0b 9001 7160 7406 6421 8301 0100 7406  }...q`t.d!....t.
-00004c40: 6422 740a 7c00 6413 1900 6a00 8301 8302  d"t.|.d...j.....
-00004c50: 0100 7406 6423 7c00 6a05 7c00 640b 1900  ..t.d#|.j.|.d...
-00004c60: 7408 7c07 8301 6b02 1900 640e 1900 6a00  t.|...k...d...j.
-00004c70: 6409 1900 8302 0100 7406 6424 7c08 8302  d.......t.d$|...
-00004c80: 0100 7c00 5300 2925 6115 0300 0055 7064  ..|.S.)%a....Upd
-00004c90: 6174 6520 4472 6169 6e61 6765 2061 7265  ate Drainage are
-00004ca0: 612c 2073 7472 6168 6c65 7220 6f72 6465  a, strahler orde
-00004cb0: 7220 6f66 2073 7562 6261 696e 730a 0a20  r of subbains.. 
-00004cc0: 2020 2055 7064 6174 6520 6472 6169 6e61     Update draina
-00004cd0: 6765 2061 7265 6120 616e 6420 7374 7261  ge area and stra
-00004ce0: 686c 6572 206f 7264 6572 2066 6f72 2063  hler order for c
-00004cf0: 6f6d 6269 6e65 6420 726f 7574 696e 6720  ombined routing 
-00004d00: 7072 6f64 7563 740a 2020 2020 6f66 2065  product.    of e
-00004d10: 6163 6820 7375 6272 6567 696f 6e73 0a20  ach subregions. 
-00004d20: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00004d30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00004d40: 2041 6c6c 4361 7469 6e66 6f20 2020 2020   AllCatinfo     
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 203a 2064 6174 6166 7261 6d65 0a20     : dataframe. 
-00004d70: 2020 2020 2020 2069 7420 6973 2061 2064         it is a d
-00004d80: 6174 6166 7261 6d65 206f 6620 7468 6520  ataframe of the 
-00004d90: 6174 7472 6962 7574 6520 7461 626c 6520  attribute table 
-00004da0: 7265 6164 6564 2066 726f 6d20 6669 6e61  readed from fina
-00004db0: 6c63 6174 5f69 6e66 6f0a 2020 2020 2020  lcat_info.      
-00004dc0: 2020 2e73 6870 206f 7220 6669 6e61 6c72    .shp or finalr
-00004dd0: 6976 706c 795f 696e 666f 2e73 6870 0a20  ivply_info.shp. 
-00004de0: 2020 2053 7562 5f52 6567 696f 6e5f 696e     Sub_Region_in
-00004df0: 666f 2020 2020 2020 2020 2020 2020 2020  fo              
-00004e00: 2020 2020 203a 2064 6174 6166 7261 6d65       : dataframe
-00004e10: 0a20 2020 2020 2020 2049 7420 6973 2061  .        It is a
-00004e20: 2064 6174 6166 7261 6d65 2069 6e63 6c75   dataframe inclu
-00004e30: 6465 7320 7375 6272 6567 696f 6e20 696e  des subregion in
-00004e40: 666f 726d 6174 696f 6e73 2c20 7769 7468  formations, with
-00004e50: 2066 6f6c 6c6f 7769 6e67 0a20 2020 2020   following.     
-00004e60: 2020 2063 6f6c 756d 6e73 3a0a 2020 2020     columns:.    
-00004e70: 2020 2020 2753 7562 5f52 6567 5f49 4427      'Sub_Reg_ID'
-00004e80: 203a 2074 6865 2073 7562 7265 6769 6f6e   : the subregion
-00004e90: 2069 640a 2020 2020 2020 2020 2744 6f77   id.        'Dow
-00004ea0: 5f53 7562 5f52 6567 5f49 6427 3a20 7468  _Sub_Reg_Id': th
-00004eb0: 6520 646f 776e 7374 7265 616d 2073 7562  e downstream sub
-00004ec0: 7265 6769 6f6e 2069 640a 0a20 2020 204e  region id..    N
-00004ed0: 6f74 6573 0a20 2020 202d 2d2d 2d2d 2d2d  otes.    -------
-00004ee0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00004ef0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2041     -------.    A
-00004f00: 6c6c 4361 7469 6e66 6f20 2020 2020 2020  llCatinfo       
-00004f10: 2020 2020 3a20 6461 7461 6672 616d 650a      : dataframe.
-00004f20: 2020 2020 2020 2020 446f 776e 7374 7265          Downstre
-00004f30: 616d 2044 4120 616e 6420 7374 7261 686c  am DA and strahl
-00004f40: 6572 206f 7264 6572 206f 6620 6561 6368  er order of each
-00004f50: 2073 7562 7265 6769 6f6e 2061 6c6f 6e67   subregion along
-00004f60: 2074 6865 2066 6c6f 770a 2020 2020 2020   the flow.      
-00004f70: 2020 7061 7468 7761 7920 6265 7477 6565    pathway betwee
-00004f80: 6e20 7375 6272 6567 696f 6e73 2077 696c  n subregions wil
-00004f90: 6c20 6265 2075 7064 6174 6564 2e0a 2020  l be updated..  
-00004fa0: 2020 677b 14ae 47e1 7a84 3f67 3333 3333    g{..G.z.?g3333
-00004fb0: 3333 c33f 72ae 0000 0072 4f00 0000 72aa  33.?r....rO...r.
-00004fc0: 0000 0072 4900 0000 7250 0000 007a 1f57  ...rI...rP...z.W
-00004fd0: 6174 6865 7273 6564 2068 6173 206d 756c  athersed has mul
-00004fe0: 7469 706c 6520 6f75 746c 6574 2020 7201  tiple outlet  r.
-00004ff0: 0000 007a 1757 6174 6572 7368 6564 2068  ...z.Watershed h
-00005000: 6173 206e 6f20 6f75 746c 6574 7206 0000  as no outletr...
-00005010: 0072 4d00 0000 72af 0000 0072 6000 0000  .rM...r....r`...
-00005020: 7a26 2323 2323 2323 4172 6561 2061 6e64  z&######Area and
-00005030: 2044 4120 6368 6563 6b20 666f 7220 7375   DA check for su
-00005040: 6272 6567 696f 6e20 7a21 4441 2061 7420  bregion z!DA at 
-00005050: 7468 6520 7375 6272 6567 696f 6e20 6f75  the subregion ou
-00005060: 746c 6574 2069 7320 2020 207a 2154 6f74  tlet is    z!Tot
-00005070: 616c 2073 7562 7265 6769 6f6e 2061 7265  al subregion are
-00005080: 6120 6973 2020 2020 2020 2020 2020 72ad  a is          r.
-00005090: 0000 0072 6900 0000 7a06 6c6f 6f70 2020  ...ri...z.loop  
-000050a0: 72b0 0000 0072 ab00 0000 7a0d 5375 6272  r....r....z.Subr
-000050b0: 6567 696f 6e3a 2020 207a 0953 7562 4964  egion:   z.SubId
-000050c0: 2069 7320 7a0f 2044 6f77 6e53 7562 4964   is z. DownSubId
-000050d0: 2069 7320 207a 1c20 2064 6964 206e 6f74   is  z.  did not
-000050e0: 2063 6f6e 6e65 6374 6564 2077 6974 6820   connected with 
-000050f0: 2020 2072 5900 0000 724c 0000 0072 a000     rY...rL...r..
-00005100: 0000 72a1 0000 0072 a200 0000 da0a 5573  ..r....r......Us
-00005110: 655f 7265 6769 6f6e 7a14 4368 6563 6b20  e_regionz.Check 
-00005120: 6472 6169 6e61 6765 2061 7265 613a 7a21  drainage area:z!
-00005130: 546f 7461 6c20 6261 7369 6e20 6172 6561  Total basin area
-00005140: 2069 7320 2020 2020 2020 2020 2020 2020   is             
-00005150: 207a 2144 4120 6f66 2074 6865 2077 6174   z!DA of the wat
-00005160: 6572 7365 6864 206f 7574 6c65 7420 6973  ersehd outlet is
-00005170: 2020 2020 7a21 546f 7461 6c20 4441 206f      z!Total DA o
-00005180: 6620 6561 6368 2073 7562 7265 6769 6f6e  f each subregion
-00005190: 2020 2020 2020 2029 1072 2000 0000 7221         ).r ...r!
-000051a0: 0000 0072 3c00 0000 da06 746f 6c69 7374  ...r<.....tolist
-000051b0: 721f 0000 0072 2300 0000 7273 0000 0072  r....r#...rs...r
-000051c0: 5c00 0000 72a3 0000 0072 1e00 0000 7219  \...r....r....r.
-000051d0: 0000 0072 1600 0000 7231 0000 0072 6500  ...r....r1...re.
-000051e0: 0000 7237 0000 00da 0373 6574 291b 72b1  ..r7.....set).r.
-000051f0: 0000 0072 b200 0000 7247 0000 00da 0163  ...r....rG.....c
-00005200: 5a0d 6d69 6e5f 6d61 6e6e 696e 675f 6e5a  Z.min_manning_nZ
-00005210: 0d6d 6178 5f6d 616e 6e69 6e67 5f6e 5a0e  .max_manning_nZ.
-00005220: 5375 6272 6567 696f 6e5f 6c69 7374 5a14  Subregion_listZ.
-00005230: 5761 7465 7273 6865 646f 7574 6c65 7473  Watershedoutlets
-00005240: 7562 6964 5a12 546f 7461 6c5f 4441 5f53  ubidZ.Total_DA_S
-00005250: 7562 7265 6769 6f6e 7228 0000 005a 114f  ubregionr(...Z.O
-00005260: 7574 6c65 7473 7562 6964 5f63 7375 6272  utletsubid_csubr
-00005270: 5a05 696c 6f6f 705a 1163 7572 7265 6e74  Z.iloopZ.current
-00005280: 5f6c 6f6f 705f 6c69 7374 5a09 635f 7375  _loop_listZ.c_su
-00005290: 6272 5f69 645a 0964 5f73 7562 725f 6964  br_idZ.d_subr_id
-000052a0: 5a0e 4f75 746c 6574 7375 625f 696e 666f  Z.Outletsub_info
-000052b0: da09 646f 776e 7375 6269 645a 0e64 6f77  ..downsubidZ.dow
-000052c0: 6e73 7562 5f72 6567 5f69 64da 0663 7375  nsub_reg_id..csu
-000052d0: 6269 645a 0a43 5f73 7562 5f69 6e66 6f5a  bidZ.C_sub_infoZ
-000052e0: 0e55 7070 6572 5f73 7562 5f69 6e66 6f5a  .Upper_sub_infoZ
-000052f0: 054e 6577 4441 5a09 5374 7261 686c 6572  .NewDAZ.Strahler
-00005300: 735a 0b6d 6178 5374 7261 686c 6572 5a0b  sZ.maxStrahlerZ.
-00005310: 6e65 7753 7472 6168 6c65 725a 0664 615f  newStrahlerZ.da_
-00005320: 6f62 735a 0664 615f 7369 6d72 2d00 0000  obsZ.da_simr-...
-00005330: 722d 0000 0072 2e00 0000 da26 5570 6461  r-...r.....&Upda
-00005340: 7465 5f44 415f 5374 7261 686c 6572 5f46  te_DA_Strahler_F
-00005350: 6f72 5f43 6f6d 6269 6e65 645f 5265 7375  or_Combined_Resu
-00005360: 6c74 7504 0000 7322 0100 0000 1904 0104  ltu...s"........
-00005370: 020e 0102 ff06 030a 0108 051a 0108 0116  ................
-00005380: 0104 011a 0108 0104 0320 ff02 0504 0112  ......... ......
-00005390: 010e 0202 011a ff02 ff02 0402 0102 010c  ................
-000053a0: fe04 0402 0102 011a fe04 0402 0102 0102  ................
-000053b0: 0104 0114 ff02 0202 fe04 ff02 fe06 0904  ................
-000053c0: 010e 010a 0108 010a 0104 0214 0208 020a  ................
-000053d0: 0104 020e 0102 ff04 0202 fe04 040a 0302  ................
-000053e0: 010a ff02 0202 fe04 0202 fe04 0404 010a  ................
-000053f0: ff08 040e 031c 0112 010a 0102 0102 0102  ................
-00005400: 0102 0102 0102 010e fa04 0804 0210 0102  ................
-00005410: ff04 0202 fe04 0410 020a 0102 0102 0102  ................
-00005420: 0102 0102 fc04 0604 020a 0104 0112 0216  ................
-00005430: 0216 040e 0108 ff06 060a 0108 0114 010a  ................
-00005440: 0204 0216 0116 0220 011a 0122 010a 011a  ....... ..."....
-00005450: 0116 150e 031c 0112 010a 0102 0102 0102  ................
-00005460: 0102 0102 0102 010e fa04 0804 0210 0102  ................
-00005470: ff04 0202 fe0c 050c 010c 0308 0114 0102  ................
-00005480: 0102 011a 0102 ff02 fe04 060a 0172 bb00  .............r..
-00005490: 0000 6301 0000 0000 0000 0000 0000 0012  ..c.............
-000054a0: 0000 0008 0000 0043 0000 0073 e002 0000  .......C...s....
-000054b0: 6401 7d01 6402 7d02 6403 7d03 7400 7c00  d.}.d.}.d.}.t.|.
-000054c0: 7c01 1900 6a01 8301 7d04 7402 7c00 8301  |...j...}.t.|...
-000054d0: 7d05 6404 7d06 7403 a004 7c05 6405 1700  }.d.}.t...|.d...
-000054e0: 7403 6a05 a102 7d07 7403 a004 7c05 6405  t.j...}.t...|.d.
-000054f0: 1700 7403 6a05 a102 7d08 7406 6406 7402  ..t.j...}.t.d.t.
-00005500: 7c00 8301 8302 4400 9001 5d6a 7d09 7c00  |.....D...]j}.|.
-00005510: 7c01 1900 6a01 7c09 1900 7d0a 7c00 7c03  |...j.|...}.|.|.
-00005520: 1900 6a01 7c09 1900 7d0b 7c00 7c02 1900  ..j.|...}.|.|...
-00005530: 6a01 7c09 1900 7d0c 7a0c 7407 7c0a 8301  j.|...}.z.t.|...
-00005540: 7d0d 5700 6e1e 0100 0100 0100 6407 7d0d  }.W.n.......d.}.
-00005550: 6407 7c00 6a08 7c09 7c01 6602 3c00 5900  d.|.j.|.|.f.<.Y.
-00005560: 6e02 3000 7a0c 7407 7c0b 8301 7d0e 5700  n.0.z.t.|...}.W.
-00005570: 6e1e 0100 0100 0100 6407 7d0e 6407 7c00  n.......d.}.d.|.
-00005580: 6a08 7c09 7c03 6602 3c00 5900 6e02 3000  j.|.|.f.<.Y.n.0.
-00005590: 7a0c 7407 7c0c 8301 7d0f 5700 6e1e 0100  z.t.|...}.W.n...
-000055a0: 0100 0100 6407 7d0f 6407 7c00 6a08 7c09  ....d.}.d.|.j.|.
-000055b0: 7c02 6602 3c00 5900 6e02 3000 7c0d 6406  |.f.<.Y.n.0.|.d.
-000055c0: 6b00 9001 7218 7158 7c0f 6406 6b01 9001  k...r.qX|.d.k...
-000055d0: 7234 7c0d 7d10 6407 7c00 6a08 7c09 6408  r4|.}.d.|.j.|.d.
-000055e0: 6602 3c00 7c0f 6406 6b04 9001 727a 7c0e  f.<.|.d.k...rz|.
-000055f0: 7c0f 6b02 9001 7264 7c0d 7c04 1700 6409  |.k...rd|.|...d.
-00005600: 1700 7d10 6404 7c00 6a08 7c09 6408 6602  ..}.d.|.j.|.d.f.
-00005610: 3c00 6e16 7407 7c0d 8301 7d10 6407 7c00  <.n.t.|...}.d.|.
-00005620: 6a08 7c09 6408 6602 3c00 7c10 7c08 7601  j.|.d.f.<.|.|.v.
-00005630: 9001 72a4 7c06 7c00 6a08 7c09 640a 6602  ..r.|.|.j.|.d.f.
-00005640: 3c00 7c10 7c08 7c06 3c00 7c06 6404 1700  <.|.|.|.<.|.d...
-00005650: 7d06 7158 7409 7403 a00a 7c08 7c10 6b02  }.qXt.t...|.|.k.
-00005660: a101 6406 1900 8301 7c00 6a08 7c09 640a  ..d.....|.j.|.d.
-00005670: 6602 3c00 7158 7406 6406 7402 7c00 8301  f.<.qXt.d.t.|...
-00005680: 8302 4400 9001 5d04 7d09 7c00 7c01 1900  ..D...].}.|.|...
-00005690: 6a01 7c09 1900 7d0d 7c00 7c03 1900 6a01  j.|...}.|.|...j.
-000056a0: 7c09 1900 7d0e 7c00 7c02 1900 6a01 7c09  |...}.|.|...j.|.
-000056b0: 1900 7d0f 7c0d 6406 6b04 9002 7212 9001  ..}.|.d.k...r...
-000056c0: 71d4 7c0e 6406 6b01 9002 723e 740b 640b  q.|.d.k...r>t.d.
-000056d0: 8301 0100 740b 7c00 6a08 7c09 640c 640c  ....t.|.j.|.d.d.
-000056e0: 8502 6602 1900 8301 0100 9001 71d4 7c00  ..f.........q.|.
-000056f0: 6a08 7c00 7c03 1900 7c0e 6b02 7c00 6408  j.|.|...|.k.|.d.
-00005700: 1900 6406 6b04 4000 1900 7d11 7402 7c11  ..d.k.@...}.t.|.
-00005710: 8301 6406 6b01 9002 7278 740b 640d 7c0e  ..d.k...rxt.d.|.
-00005720: 8302 0100 9001 71d4 7c11 7c01 1900 6a01  ......q.|.|...j.
-00005730: 6406 1900 7c00 6a08 7c09 7c01 6602 3c00  d...|.j.|.|.f.<.
-00005740: 7c11 6408 1900 6a01 6406 1900 7c00 6a08  |.d...j.d...|.j.
-00005750: 7c09 6408 6602 3c00 7c11 640a 1900 6a01  |.d.f.<.|.d...j.
-00005760: 6406 1900 7c00 6a08 7c09 640a 6602 3c00  d...|.j.|.d.f.<.
-00005770: 7c11 7c02 1900 6a01 6406 1900 7c00 6a08  |.|...j.d...|.j.
-00005780: 7c09 7c02 6602 3c00 9001 71d4 7c00 5300  |.|.f.<...q.|.S.
-00005790: 290e 7aa1 4675 6e63 7469 6f6e 2074 6f20  ).z.Function to 
-000057a0: 6465 7465 726d 696e 2068 7275 6964 2061  determin hruid a
-000057b0: 6674 6572 2063 6f6d 6269 6e65 206c 616b  fter combine lak
-000057c0: 6520 706f 6c79 676f 6e0a 2020 2020 616e  e polygon.    an
-000057d0: 6420 7375 6262 6173 696e 2070 6f6c 7967  d subbasin polyg
-000057e0: 6f6e 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  on.    ---------
-000057f0: 2d0a 0a20 2020 204e 6f74 6573 0a20 2020  -..    Notes.   
-00005800: 202d 2d2d 2d2d 2d2d 0a0a 2020 2020 5265   -------..    Re
-00005810: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-00005820: 2d2d 0a20 2020 2020 2020 204e 6f6e 652c  --.        None,
-00005830: 0a20 2020 2072 0600 0000 726d 0000 00da  .    r....rm....
-00005840: 0848 796c 616b 5f69 6472 4f00 0000 7262  .Hylak_idrO...rb
-00005850: 0000 0072 0100 0000 7250 0000 0072 3000  ...r....rP...r0.
-00005860: 0000 e90a 0000 00da 0a48 5255 4c61 6b65  .........HRULake
-00005870: 5f49 447a 1a6c 616b 6520 6861 7320 756e  _IDz.lake has un
-00005880: 6578 7065 6374 6564 2068 6f6c 6573 204e  expected holes N
-00005890: 7a16 4c61 6b65 6964 2064 6f20 6e6f 7420  z.Lakeid do not 
-000058a0: 6578 6973 7420 2020 290c 7265 0000 0072  exist   ).re...r
-000058b0: 2000 0000 721f 0000 0072 2100 0000 7264   ...r....r!...rd
-000058c0: 0000 00da 036e 616e 721e 0000 0072 4a00  .....nanr....rJ.
-000058d0: 0000 7223 0000 0072 a300 0000 72a6 0000  ..r#...r....r...
-000058e0: 0072 7300 0000 2912 5a0f 4174 7472 6962  .rs...).Z.Attrib
-000058f0: 7574 655f 5461 626c 65da 0653 7562 5f49  ute_Table..Sub_I
-00005900: 44da 0b53 7562 5f4c 616b 655f 4944 da07  D..Sub_Lake_ID..
-00005910: 4c61 6b65 5f49 645a 0f6d 6178 5f73 7562  Lake_IdZ.max_sub
-00005920: 6261 7369 6e5f 6964 5a0e 4e5f 6e65 775f  basin_idZ.N_new_
-00005930: 6665 6174 7572 6573 5a09 6e65 775f 6872  featuresZ.new_hr
-00005940: 7569 645a 0e6e 6577 5f68 7275 6964 5f6c  uidZ.new_hruid_l
-00005950: 6973 745a 116f 6c64 5f6e 6577 6872 7569  istZ.old_newhrui
-00005960: 645f 6c69 7374 7228 0000 005a 0c73 7562  d_listr(...Z.sub
-00005970: 6964 5f73 665f 6f62 6a5a 116c 616b 656c  id_sf_objZ.lakel
-00005980: 616b 6569 645f 7366 5f6f 626a 5a11 5375  akeid_sf_objZ.Su
-00005990: 625f 4c61 6b65 6964 5f73 665f 6f62 6a5a  b_Lakeid_sf_objZ
-000059a0: 0873 7562 6964 5f73 665a 0d6c 616b 656c  .subid_sfZ.lakel
-000059b0: 616b 6569 645f 7366 5a0d 5375 625f 4c61  akeid_sfZ.Sub_La
-000059c0: 6b65 6964 5f73 665a 0d6f 6c64 5f6e 6577  keid_sfZ.old_new
-000059d0: 5f68 7275 6964 5a08 7461 725f 696e 666f  _hruidZ.tar_info
-000059e0: 722d 0000 0072 2d00 0000 722e 0000 00da  r-...r-...r.....
-000059f0: 1544 6574 6572 6d69 6e65 5f4c 616b 655f  .Determine_Lake_
-00005a00: 4852 555f 4964 5405 0000 7390 0000 0000  HRU_IdT...s.....
-00005a10: 0d04 0104 0104 030e 0208 0104 0112 0112  ................
-00005a20: 0b14 010e 010e 010e 0402 010c 0106 0104  ................
-00005a30: 010e 0106 0202 010c 0106 0104 010e 0106  ................
-00005a40: 0202 010c 0106 0104 010e 0106 040a 0102  ................
-00005a50: 030a 0104 010e 020a 0206 ff04 030c 0110  ................
-00005a60: 0208 010e 030a 010e 0108 010a 0302 0110  ................
-00005a70: ff10 0814 010e 010e 010e 010a 0104 010a  ................
-00005a80: 0108 0116 0104 0204 010a 010a ff02 ff04  ................
-00005a90: 040e 010a 0104 0118 0118 0118 011c 0272  ...............r
-00005aa0: c300 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00005ab0: 0006 0000 0004 0000 0043 0000 0073 8a00  .........C...s..
-00005ac0: 0000 7c00 6a00 7c00 7c02 1900 6401 6b03  ..|.j.|.|...d.k.
-00005ad0: 1900 7d04 7401 7c04 8301 6401 6b04 722e  ..}.t.|...d.k.r.
-00005ae0: 7c04 7c02 1900 6a02 6401 1900 7d05 6e58  |.|...j.d...}.nX
-00005af0: 7c01 6a00 7c01 7c02 1900 6401 6b03 1900  |.j.|.|...d.k...
-00005b00: 7d01 7c01 6a03 6402 6403 6404 8d02 7d01  }.|.j.d.d.d...}.
-00005b10: 7401 7c01 8301 6401 6b04 726a 7c01 7c02  t.|...d.k.rj|.|.
-00005b20: 1900 6a02 6401 1900 7d05 6e1c 7c03 6a00  ..j.d...}.n.|.j.
-00005b30: 7c03 7c02 1900 6401 6b03 1900 7c02 1900  |.|...d.k...|...
-00005b40: 6a02 6401 1900 7d05 7c05 5300 2905 4e72  j.d...}.|.S.).Nr
-00005b50: 0100 0000 7207 0000 0046 7210 0000 0029  ....r....Fr....)
-00005b60: 0472 2300 0000 721f 0000 0072 2000 0000  .r#...r....r ...
-00005b70: 721c 0000 0029 06da 1641 7474 7269 5f74  r....)...Attri_t
-00005b80: 6162 6c65 5f4c 616b 655f 4852 555f 69da  able_Lake_HRU_i.
-00005b90: 0753 7562 496e 666f da06 436f 6c5f 4e4d  .SubInfo..Col_NM
-00005ba0: 5a09 696e 666f 5f64 6174 615a 0d69 6e66  Z.info_dataZ.inf
-00005bb0: 6f5f 6c61 6b65 5f68 7275 5a0b 5570 6461  o_lake_hruZ.Upda
-00005bc0: 7465 7661 6c75 6572 2d00 0000 722d 0000  tevaluer-...r-..
-00005bd0: 0072 2e00 0000 da1f 5265 7472 756e 5f56  .r......Retrun_V
-00005be0: 616c 6964 6174 655f 4174 7472 6962 7574  alidate_Attribut
-00005bf0: 655f 5661 6c75 65cf 0500 0073 1400 0000  e_Value....s....
-00005c00: 0002 1202 0aff 0203 1002 1201 0e01 0c01  ................
-00005c10: 1002 1c03 72c7 0000 0063 0a00 0000 0000  ....r....c......
-00005c20: 0000 0000 0000 1a00 0000 0700 0000 4300  ..............C.
-00005c30: 0000 735e 0400 007c 007c 0119 0064 016b  ..s^...|.|...d.k
-00005c40: 017d 0a7c 007c 0219 0064 016b 017c 007c  .}.|.|...d.k.|.|
-00005c50: 0219 0064 026b 0340 007d 0b7c 007c 0319  ...d.k.@.}.|.|..
-00005c60: 0064 016b 017c 007c 0319 0064 026b 0340  .d.k.|.|...d.k.@
-00005c70: 007d 0c7c 007c 0419 0064 016b 017c 007c  .}.|.|...d.k.|.|
-00005c80: 0419 0064 026b 0340 007d 0d7c 007c 0619  ...d.k.@.}.|.|..
-00005c90: 0064 016b 017c 007c 0619 0064 026b 0340  .d.k.|.|...d.k.@
-00005ca0: 007d 0e7c 0a7c 0b42 007c 0c42 007c 0d42  .}.|.|.B.|.B.|.B
-00005cb0: 007c 0e42 007d 0f74 00a0 017c 006a 027c  .|.B.}.t...|.j.|
-00005cc0: 0f64 0366 0219 006a 03a1 017d 107c 107c  .d.f...j...}.|.|
-00005cd0: 1064 016b 0419 007d 1074 0464 0174 057c  .d.k...}.t.d.t.|
-00005ce0: 1083 0183 0244 0090 025d f27d 117c 107c  .....D...].}.|.|
-00005cf0: 1119 007d 127c 1264 016b 0272 c871 b07c  ...}.|.d.k.r.q.|
-00005d00: 006a 027c 0064 0319 007c 126b 0219 007d  .j.|.d...|.k...}
-00005d10: 137c 136a 0664 0464 0564 068d 027d 137c  .|.j.d.d.d...}.|
-00005d20: 1364 0719 006a 0364 0119 007d 147c 006a  .d...j.d...}.|.j
-00005d30: 027c 0064 0719 007c 146b 0219 007d 1574  .|.d...|.k...}.t
-00005d40: 0464 0174 057c 1383 0183 0244 0090 025d  .d.t.|.....D...]
-00005d50: 8a7d 167c 1364 0819 006a 037c 1619 007d  .}.|.d...j.|...}
-00005d60: 177c 1364 0919 006a 037c 1619 007d 187c  .|.d...j.|...}.|
-00005d70: 1864 016b 0490 0272 887c 137c 0319 006a  .d.k...r.|.|...j
-00005d80: 0364 0119 0064 016b 0290 0172 7c74 077c  .d...d.k...r|t.|
-00005d90: 137c 157c 037c 0883 047d 197c 197c 006a  .|.|.|...}.|.|.j
-00005da0: 027c 0064 0819 007c 176b 027c 0366 023c  .|.d...|.k.|.f.<
-00005db0: 006e 207c 137c 0319 006a 0364 0119 007c  .n |.|...j.d...|
-00005dc0: 006a 027c 0064 0819 007c 176b 027c 0366  .j.|.d...|.k.|.f
-00005dd0: 023c 007c 137c 0519 006a 0364 0119 0064  .<.|.|...j.d...d
-00005de0: 016b 0290 0172 d674 077c 137c 157c 057c  .k...r.t.|.|.|.|
-00005df0: 0083 047d 197c 197c 006a 027c 0064 0819  ...}.|.|.j.|.d..
-00005e00: 007c 176b 027c 0566 023c 006e 207c 137c  .|.k.|.f.<.n |.|
-00005e10: 0519 006a 0364 0119 007c 006a 027c 0064  ...j.d...|.j.|.d
-00005e20: 0819 007c 176b 027c 0566 023c 007c 137c  ...|.k.|.f.<.|.|
-00005e30: 0619 006a 0364 0119 0064 016b 0290 0272  ...j.d...d.k...r
-00005e40: 3074 077c 137c 157c 067c 0083 047d 197c  0t.|.|.|.|...}.|
-00005e50: 197c 006a 027c 0064 0819 007c 176b 027c  .|.j.|.d...|.k.|
-00005e60: 0666 023c 006e 207c 137c 0619 006a 0364  .f.<.n |.|...j.d
-00005e70: 0119 007c 006a 027c 0064 0819 007c 176b  ...|.j.|.d...|.k
-00005e80: 027c 0666 023c 0074 0864 0283 017c 006a  .|.f.<.t.d...|.j
-00005e90: 027c 0064 0819 007c 176b 027c 0266 023c  .|.d...|.k.|.f.<
-00005ea0: 0074 0864 0283 017c 006a 027c 0064 0819  .t.d...|.j.|.d..
-00005eb0: 007c 176b 027c 0466 023c 0090 0171 167c  .|.k.|.f.<...q.|
-00005ec0: 137c 0319 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
-00005ed0: 0272 c074 077c 137c 157c 037c 0883 047d  .r.t.|.|.|.|...}
-00005ee0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
-00005ef0: 027c 0366 023c 007c 137c 0219 006a 037c  .|.f.<.|.|...j.|
-00005f00: 1619 0064 016b 0290 0272 f874 077c 137c  ...d.k...r.t.|.|
-00005f10: 157c 027c 0783 047d 197c 197c 006a 027c  .|.|...}.|.|.j.|
-00005f20: 0064 0819 007c 176b 027c 0266 023c 007c  .d...|.k.|.f.<.|
-00005f30: 137c 0419 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
-00005f40: 0372 3074 077c 137c 157c 047c 0983 047d  .r0t.|.|.|.|...}
-00005f50: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
-00005f60: 027c 0466 023c 007c 137c 0519 006a 037c  .|.f.<.|.|...j.|
-00005f70: 1619 0064 016b 0290 0372 6874 077c 137c  ...d.k...rht.|.|
-00005f80: 157c 057c 0083 047d 197c 197c 006a 027c  .|.|...}.|.|.j.|
-00005f90: 0064 0819 007c 176b 027c 0566 023c 007c  .d...|.k.|.f.<.|
-00005fa0: 137c 0619 006a 037c 1619 0064 016b 0290  .|...j.|...d.k..
-00005fb0: 0172 1674 077c 137c 157c 067c 0083 047d  .r.t.|.|.|.|...}
-00005fc0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
-00005fd0: 027c 0666 023c 0090 0171 1671 b07c 006a  .|.f.<...q.q.|.j
-00005fe0: 0967 0064 0aa2 0164 0b8d 017d 0074 0a6a  .g.d...d...}.t.j
-00005ff0: 0b7c 007c 0764 0c7c 0264 0d8d 046a 0c64  .|.|.d.|.d...j.d
-00006000: 0e64 0f8d 017d 0074 0a6a 0b7c 007c 0864  .d...}.t.j.|.|.d
-00006010: 0c7c 0364 0d8d 046a 0c64 0e64 0f8d 017d  .|.d...j.d.d...}
-00006020: 0074 0a6a 0b7c 007c 0964 0c7c 0464 0d8d  .t.j.|.|.d.|.d..
-00006030: 046a 0c64 0e64 0f8d 017d 007c 0064 0319  .j.d.d...}.|.d..
-00006040: 00a0 0d74 0ea1 017c 007c 0219 00a0 0d74  ...t...|.|.....t
-00006050: 0ea1 0117 007c 007c 0319 00a0 0d74 0ea1  .....|.|.....t..
-00006060: 0117 007c 007c 0519 00a0 0d74 0ea1 0117  ...|.|.....t....
-00006070: 007c 0064 103c 0074 0aa0 0f7c 0064 1019  .|.d.<.t...|.d..
-00006080: 00a1 0164 0119 0064 1117 007c 0064 123c  ...d...d...|.d.<
-00006090: 007c 0053 0029 137a ab46 756e 6374 696f  .|.S.).z.Functio
-000060a0: 6e20 746f 2064 6574 6572 6d69 6e65 206c  n to determine l
-000060b0: 616e 6475 7365 2c73 6f69 6c2c 616e 6420  anduse,soil,and 
-000060c0: 7665 6720 616e 6420 6f74 6865 7220 7072  veg and other pr
-000060d0: 6f70 6572 7469 6573 2061 6674 6572 2075  operties after u
-000060e0: 6e69 6f6e 2061 6c6c 2070 6f6c 7967 6f6e  nion all polygon
-000060f0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00006100: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
-00006110: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052 6574  -------..    Ret
-00006120: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
-00006130: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c0a  -.        None,.
-00006140: 2020 2020 7201 0000 0072 5000 0000 72be      r....rP...r.
-00006150: 0000 0072 0700 0000 4672 1000 0000 7206  ...r....Fr....r.
-00006160: 0000 0072 9100 0000 7230 0000 0029 035a  ...r....r0...).Z
-00006170: 0a4c 414e 445f 5553 455f 435a 0556 4547  .LAND_USE_CZ.VEG
-00006180: 5f43 5a09 534f 494c 5f50 524f 4672 0a00  _CZ.SOIL_PROFr..
-00006190: 0000 da05 696e 6e65 7229 02da 0368 6f77  ....inner)...how
-000061a0: 720e 0000 0054 7208 0000 00da 0766 6163  r....Tr......fac
-000061b0: 7465 7273 724f 0000 0072 3a00 0000 2910  tersrO...r:...).
-000061c0: 7221 0000 0072 3c00 0000 7223 0000 0072  r!...r<...r#...r
-000061d0: 2000 0000 721e 0000 0072 1f00 0000 721c   ...r....r....r.
-000061e0: 0000 0072 c700 0000 72a3 0000 0072 3f00  ...r....r....r?.
-000061f0: 0000 721a 0000 0072 1b00 0000 7216 0000  ..r....r....r...
-00006200: 0072 5c00 0000 da03 7374 72da 0966 6163  .r\.....str..fac
-00006210: 746f 7269 7a65 291a 5a0b 4174 7472 695f  torize).Z.Attri_
-00006220: 7461 626c 6572 c000 0000 7227 0000 0072  tabler....r'...r
-00006230: 3300 0000 7234 0000 0072 3500 0000 7236  3...r4...r5...r6
-00006240: 0000 005a 114c 616e 6475 7365 5f69 6e66  ...Z.Landuse_inf
-00006250: 6f5f 6461 7461 5a0e 536f 696c 5f69 6e66  o_dataZ.Soil_inf
-00006260: 6f5f 6461 7461 5a0d 5665 675f 696e 666f  o_dataZ.Veg_info
-00006270: 5f64 6174 615a 0969 6e76 616c 5f73 7562  _dataZ.inval_sub
-00006280: 5a0d 696e 7661 6c5f 6c61 6e64 7573 655a  Z.inval_landuseZ
-00006290: 0a69 6e76 616c 5f73 6f69 6c5a 0969 6e76  .inval_soilZ.inv
-000062a0: 616c 5f76 6567 5a08 696e 7661 6c5f 6f32  al_vegZ.inval_o2
-000062b0: 5a0a 696e 7661 6c5f 726f 7773 5a0c 4c61  Z.inval_rowsZ.La
-000062c0: 6b65 5f48 5255 5f49 4453 7228 0000 005a  ke_HRU_IDSr(...Z
-000062d0: 0c69 6c61 6b65 5f68 7275 5f69 6472 c400  .ilake_hru_idr..
-000062e0: 0000 da05 5375 6269 6472 c500 0000 7244  ....Subidr....rD
-000062f0: 0000 005a 0769 6872 755f 6964 5a07 6973  ...Z.ihru_idZ.is
-00006300: 5f4c 616b 655a 0a56 616c 695f 5661 6c75  _LakeZ.Vali_Valu
-00006310: 6572 2d00 0000 722d 0000 0072 2e00 0000  er-...r-...r....
-00006320: da18 4465 7465 726d 696e 655f 4852 555f  ..Determine_HRU_
-00006330: 4174 7472 6962 7574 6573 e205 0000 73f8  Attributes....s.
-00006340: 0000 0000 180c 0118 0118 0118 0118 0214  ................
-00006350: 0116 010c 0314 0108 0108 0102 0204 010a  ................
-00006360: ff04 0304 0104 ff06 030e 0112 0114 010e  ................
-00006370: 010e 010a 0310 ff04 0302 0108 ff04 0502  ................
-00006380: fe04 010e ff04 060c fe04 010e ff02 0510  ................
-00006390: ff04 0302 0108 ff04 0502 fe04 010e ff04  ................
-000063a0: 060c fe04 010e ff02 0510 ff04 0302 0108  ................
-000063b0: ff04 0502 fe04 010e ff04 060c fe04 010e  ................
-000063c0: ff02 041a 011e 0410 ff04 0302 0108 ff04  ................
-000063d0: 0502 fe04 010e ff02 0410 ff04 0302 0108  ................
-000063e0: ff04 0502 fe04 010e ff02 0410 ff04 0302  ................
-000063f0: 0108 ff04 0502 fe04 010e ff02 0410 ff04  ................
-00006400: 0302 0108 ff04 0502 fe04 010e ff02 0410  ................
-00006410: ff04 0302 0108 ff04 0502 fe04 010e ff08  ................
-00006420: 0410 011a 011a 011a 580c 010c ff02 020c  ........X.......
-00006430: fe02 040c fc02 ff06 081a 0172 ce00 0000  ...........r....
-00006440: 6303 0000 0000 0000 0000 0000 0041 0000  c............A..
-00006450: 000c 0000 0043 0000 0073 720b 0000 6401  .....C...sr...d.
-00006460: 7d03 6402 7d04 6403 7d05 6404 7d06 6405  }.d.}.d.}.d.}.d.
-00006470: 7d07 6405 7c00 6a00 7601 7222 6406 7d07  }.d.|.j.v.r"d.}.
-00006480: 7c00 6a01 6407 6408 8d01 7d08 6409 7c08  |.j.d.d...}.d.|.
-00006490: 640a 3c00 6409 7c08 640b 3c00 7c08 6a02  d.<.d.|.d.<.|.j.
-000064a0: 6407 6407 640c 8d02 0100 7403 a004 7c08  d.d.d.....t...|.
-000064b0: 6403 1900 6a05 a101 7d09 7c02 640d 1400  d...j...}.|.d...
-000064c0: 640d 1400 7c09 6b04 728c 7c09 640e 1b00  d...|.k.r.|.d...
-000064d0: 640e 1b00 640f 1800 7d02 6409 7c08 7c07  d...d...}.d.|.|.
-000064e0: 3c00 6409 7c00 7c07 3c00 7c00 6a06 7c00  <.d.|.|.<.|.j.|.
-000064f0: 7c05 1900 7c02 640d 1400 640d 1400 6b05  |...|.d...d...k.
-00006500: 1900 a001 a100 7d0a 7407 7c0a 6409 6410  ......}.t.|.d.d.
-00006510: 8d02 7d0a 7c0a 6a08 6411 6701 6407 6412  ..}.|.j.d.g.d.d.
-00006520: 8d02 7d0a 7c0a 6a06 7c0a 6413 1900 6414  ..}.|.j.|.d...d.
-00006530: 6b03 1900 a001 a100 7d0a 7c0a 7c03 1900  k.......}.|.|...
-00006540: 6a05 7d0b 7c0a 6a06 7c0a 6413 1900 640f  j.}.|.j.|.d...d.
-00006550: 6b02 1900 6415 1900 6a05 7d0c 7403 a009  k...d...j.}.t...
-00006560: 7c0c 7c0c 6416 6b04 1900 a101 7d0c 7c00  |.|.d.k.....}.|.
-00006570: 6a06 7c00 6415 1900 a00a 7c0c a101 1900  j.|.d.....|.....
-00006580: a001 a100 7d0d 7c0d 7c03 1900 6a05 7d0e  ....}.|.|...j.}.
-00006590: 7c00 6a06 7c00 6401 1900 a00a 7c0b a101  |.j.|.d.....|...
-000065a0: 0f00 7c00 7c07 1900 6416 6b04 4000 1900  ..|.|...d.k.@...
-000065b0: 6a01 6407 6408 8d01 7d0f 7c0f 6a06 7c0f  j.d.d...}.|.j.|.
-000065c0: 6415 1900 6416 6b01 1900 6401 1900 6a05  d...d.k...d...j.
-000065d0: 7d10 7c00 6a01 6407 6408 8d01 7d11 7c11  }.|.j.d.d...}.|.
-000065e0: 6401 1900 a00a 7c10 a101 7d12 7c11 6415  d.....|...}.|.d.
-000065f0: 1900 640f 6b00 7d13 7403 a00b 7c12 7c13  ..d.k.}.t...|.|.
-00006600: a102 7d14 7c11 6a06 7c11 6401 1900 a00a  ..}.|.j.|.d.....
-00006610: 7c10 a101 6401 6602 1900 0b00 7c11 6a06  |...d.f.....|.j.
-00006620: 7c14 6415 6602 3c00 7c11 6a06 7c11 6401  |.d.f.<.|.j.|.d.
-00006630: 1900 a00a 7c10 a101 6415 6602 1900 6a05  ....|...d.f...j.
-00006640: 7d15 7c01 6417 1900 6a05 7d16 7403 a00c  }.|.d...j.}.t...
-00006650: 7c16 7c0c a102 7d14 7c16 7403 a00d 7c14  |.|...}.|.t...|.
-00006660: a101 1900 a001 a100 7d17 7c11 6a06 7c11  ........}.|.j.|.
-00006670: 6415 1900 a00a 7c17 a101 7c11 6415 1900  d.....|...|.d...
-00006680: a00a 7c15 a101 4200 1900 a001 a100 7d18  ..|...B.......}.
-00006690: 7c00 6a06 7c00 6413 1900 6414 6b02 1900  |.j.|.d...d.k...
-000066a0: 6401 1900 6a05 7d19 7403 a009 7c19 7c19  d...j.}.t...|.|.
-000066b0: 6416 6b04 1900 a101 7d19 7c00 6a06 7c00  d.k.....}.|.j.|.
-000066c0: 6413 1900 6414 6b02 1900 6415 1900 6a05  d...d.k...d...j.
-000066d0: 7d1a 7403 a009 7c1a 7c1a 6416 6b04 1900  }.t...|.|.d.k...
-000066e0: a101 7d1a 7403 a009 7c0b a101 7d1b 7c00  ..}.t...|...}.|.
-000066f0: 6401 6402 6702 1900 a00e 6418 a101 6a05  d.d.g.....d...j.
-00006700: 7d1c 7c0a 6404 1900 6a05 7d1d 7403 a009  }.|.d...j.}.t...
-00006710: 7c1d a101 7d1d 7c08 6a06 7c08 6413 1900  |...}.|.j.|.d...
-00006720: 6414 6b02 1900 6401 1900 6a05 7c08 6a06  d.k...d...j.|.j.
-00006730: 7c08 6413 1900 6414 6b02 640a 6602 3c00  |.d...d.k.d.f.<.
-00006740: 7c18 a00f 6415 6701 a101 6403 1900 a010  |...d.g...d.....
-00006750: 7404 a101 7c18 6403 1900 6b02 7d1e 7c18  t...|.d...k.}.|.
-00006760: 7c1e 1900 7d1f 7c1f 6a08 6411 6403 6702  |...}.|.j.d.d.g.
-00006770: 6407 6407 6702 6412 8d02 7d1f 7c00 7c00  d.d.g.d...}.|.|.
-00006780: 6402 1900 6416 6b00 1900 6a01 6407 6408  d...d.k...j.d.d.
-00006790: 8d01 7d20 7411 6416 7412 7c20 8301 8302  ..} t.d.t.| ....
-000067a0: 4400 5d50 7d21 7c20 6403 1900 6a05 7c21  D.]P}!| d...j.|!
-000067b0: 1900 7c02 640d 1400 640d 1400 6b01 9003  ..|.d...d...k...
-000067c0: 7244 7c20 6401 1900 6a05 7c21 1900 7d22  rD| d...j.|!..}"
-000067d0: 7413 7c1c 7c22 8302 7d23 7414 7c22 7c00  t.|.|"..}#t.|"|.
-000067e0: 7c08 640f 7c00 7c23 6409 6419 8d07 7d08  |.d.|.|#d.d...}.
-000067f0: 9003 7144 7411 6416 7412 7c1f 8301 8302  ..qDt.d.t.|.....
-00006800: 4400 9001 5d08 7d21 7403 a009 7c08 6a06  D...].}!t...|.j.
-00006810: 7c08 640a 1900 6416 6b04 1900 7c03 1900  |.d...d.k...|...
-00006820: 6a05 a101 7d24 7c1f 6415 1900 6a05 7c21  j...}$|.d...j.|!
-00006830: 1900 7d25 7c11 7c11 6415 1900 7c25 6b02  ..}%|.|.d...|%k.
-00006840: 1900 7d26 7403 a009 7c26 6404 1900 6a05  ..}&t...|&d...j.
-00006850: a101 7d27 6700 7d28 7411 6416 7412 7c27  ..}'g.}(t.d.t.|'
-00006860: 8301 8302 4400 5d82 7d29 7c27 7c29 1900  ....D.].})|'|)..
-00006870: 7d2a 7c26 6a06 7c26 6404 1900 7c2a 6b02  }*|&j.|&d...|*k.
-00006880: 1900 a001 a100 7d2b 7c2b 6a08 6403 6701  ......}+|+j.d.g.
-00006890: 641a 6412 8d02 7d2b 7c2b 6401 1900 6a05  d.d...}+|+d...j.
-000068a0: 6416 1900 7d22 7413 7c1c 7c22 8302 7d23  d...}"t.|.|"..}#
-000068b0: 7c23 7c23 6416 6b04 1900 7d23 7403 a00c  |#|#d.k...}#t...
-000068c0: 7c23 7c24 a102 7d14 7c23 7403 a00d 7c14  |#|$..}.|#t...|.
-000068d0: a101 1900 7d2c 6700 7c28 a201 7c2c a015  ....},g.|(..|,..
-000068e0: a100 a201 7d28 9004 7108 7403 a016 7c28  ....}(..q.t...|(
-000068f0: a101 7d28 7414 7c22 7c11 7c08 640f 7c11  ..}(t.|"|.|.d.|.
-00006900: 7c28 6414 6419 8d07 7d08 9003 71a4 7411  |(d.d...}...q.t.
-00006910: 6416 7412 7c1d 8301 8302 4400 9006 5d1e  d.t.|.....D...].
-00006920: 7d2d 7c1d 7c2d 1900 7d2e 7c0a 6a06 7c0a  }-|.|-..}.|.j.|.
-00006930: 6404 1900 7c2e 6b02 1900 a001 a100 7d2f  d...|.k.......}/
-00006940: 7c2f 6a08 641b 6701 6407 6412 8d02 7d2f  |/j.d.g.d.d...}/
-00006950: 6416 7d30 6700 7d28 640f 7d31 7411 6416  d.}0g.}(d.}1t.d.
-00006960: 7412 7c2f 8301 8302 4400 9005 5dcc 7d32  t.|/....D...].}2
-00006970: 7c2f 6401 1900 6a05 7c32 1900 7d22 7c2f  |/d...j.|2..}"|/
-00006980: 6415 1900 6a05 7c32 1900 7d33 7c28 a017  d...j.|2..}3|(..
-00006990: 7c22 a101 0100 7403 a009 7c08 6a06 7c08  |"....t...|.j.|.
-000069a0: 640a 1900 6416 6b04 1900 7c03 1900 6a05  d...d.k...|...j.
-000069b0: a101 7d24 7c30 7c2f 641c 1900 6a05 7c32  ..}$|0|/d...j.|2
-000069c0: 1900 1700 7d30 7c32 7412 7c2f 8301 640f  ....}0|2t.|/..d.
-000069d0: 1800 6b03 9005 729c 7c2f 6415 1900 6a05  ..k...r.|/d...j.
-000069e0: 7c32 1900 7c2f 6415 1900 6a05 7c32 640f  |2..|/d...j.|2d.
-000069f0: 1700 1900 6b02 7d34 6e04 641a 7d34 7c2f  ....k.}4n.d.}4|/
-00006a00: 7c07 1900 6a05 7c32 1900 6416 6b01 7d35  |...j.|2..d.k.}5
-00006a10: 7c32 7412 7c2f 8301 6414 1800 6b01 9005  |2t.|/..d...k...
-00006a20: 72f4 7c2f 641c 1900 6a05 7c32 640f 1700  r.|/d...j.|2d...
-00006a30: 1900 641d 6b00 9005 72e2 6407 7d36 6e10  ..d.k...r.d.}6n.
-00006a40: 7c30 7c02 640d 1400 640d 1400 6b00 7d36  |0|.d...d...k.}6
-00006a50: 6e10 7c30 7c02 640d 1400 640d 1400 6b00  n.|0|.d...d...k.
-00006a60: 7d36 7c30 641d 6b00 7d37 7c32 640f 6b05  }6|0d.k.}7|2d.k.
-00006a70: 9006 728c 7c32 7412 7c2f 8301 6414 1800  ..r.|2t.|/..d...
-00006a80: 6b01 9006 728c 7c2f 6415 1900 6a05 7c32  k...r.|/d...j.|2
-00006a90: 640f 1800 1900 7c2f 6415 1900 6a05 7c32  d.....|/d...j.|2
-00006aa0: 1900 6b03 7d38 7c2f 6415 1900 6a05 7c32  ..k.}8|/d...j.|2
-00006ab0: 1900 7c2f 6415 1900 6a05 7c32 640f 1700  ..|/d...j.|2d...
-00006ac0: 1900 6b03 7d39 7c2f 6415 1900 6a05 7c32  ..k.}9|/d...j.|2
-00006ad0: 1900 6416 6b01 7d3a 7c2f 641c 1900 6a05  ..d.k.}:|/d...j.
-00006ae0: 7c32 1900 641d 6b00 7d37 7c32 6416 6b02  |2..d.k.}7|2d.k.
-00006af0: 9006 72f0 7c32 7412 7c2f 8301 640f 1800  ..r.|2t.|/..d...
-00006b00: 6b00 9006 72f0 6407 7d38 7c2f 6415 1900  k...r.d.}8|/d...
-00006b10: 6a05 7c32 1900 7c2f 6415 1900 6a05 7c32  j.|2..|/d...j.|2
-00006b20: 640f 1700 1900 6b03 7d39 7c2f 6415 1900  d.....k.}9|/d...
-00006b30: 6a05 7c32 1900 6416 6b01 7d3a 7c2f 641c  j.|2..d.k.}:|/d.
-00006b40: 1900 6a05 7c32 1900 641d 6b00 7d37 7c32  ..j.|2..d.k.}7|2
-00006b50: 7412 7c2f 8301 6414 1800 6b02 9008 723c  t.|/..d...k...r<
-00006b60: 7c2f 6415 1900 6a05 7c32 1900 6416 6b04  |/d...j.|2..d.k.
-00006b70: 9008 723c 6407 7d38 7c2f 6415 1900 6a05  ..r<d.}8|/d...j.
-00006b80: 7c32 1900 7c2f 6415 1900 6a05 7c32 640f  |2..|/d...j.|2d.
-00006b90: 1700 1900 6b03 7d39 7c2f 6415 1900 6a05  ....k.}9|/d...j.
-00006ba0: 7c32 1900 6416 6b04 7d3a 7c2f 6402 1900  |2..d.k.}:|/d...
-00006bb0: 6a05 7c32 1900 7d3b 7c2f 641c 1900 6a05  j.|2..};|/d...j.
-00006bc0: 7c32 640f 1700 1900 641d 6b00 7d37 7c37  |2d.....d.k.}7|7
-00006bd0: 9008 723c 7c39 9008 723c 7c2f 6415 1900  ..r<|9..r<|/d...
-00006be0: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006bf0: 7c3b 6b02 6415 6602 3c00 7c2f 6413 1900  |;k.d.f.<.|/d...
-00006c00: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006c10: 7c3b 6b02 6413 6602 3c00 7c2f 641e 1900  |;k.d.f.<.|/d...
-00006c20: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006c30: 7c3b 6b02 641e 6602 3c00 7c2f 641f 1900  |;k.d.f.<.|/d...
-00006c40: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006c50: 7c3b 6b02 641f 6602 3c00 7c2f 6420 1900  |;k.d.f.<.|/d ..
-00006c60: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006c70: 7c3b 6b02 6420 6602 3c00 7c2f 6421 1900  |;k.d f.<.|/d!..
-00006c80: 6a05 7c32 1900 7c00 6a06 7c00 6401 1900  j.|2..|.j.|.d...
-00006c90: 7c3b 6b02 6421 6602 3c00 7c32 7412 7c2f  |;k.d!f.<.|2t.|/
-00006ca0: 8301 640f 1800 6b02 9008 725a 6407 7d38  ..d...k...rZd.}8
-00006cb0: 641a 7d39 6407 7d3a 7c32 7412 7c2f 8301  d.}9d.}:|2t.|/..
-00006cc0: 640f 1800 6b02 9009 7284 6416 7d30 7403  d...k...r.d.}0t.
-00006cd0: a016 7c28 a101 7d2c 7c33 6416 6b04 9008  ..|(..},|3d.k...
-00006ce0: 72d8 7c00 6a06 7c00 6415 1900 7c33 6b02  r.|.j.|.d...|3k.
-00006cf0: 1900 a001 a100 7d3c 7c3c 6401 6402 6702  ......}<|<d.d.g.
-00006d00: 1900 a00e 6418 a101 6a05 7d3d 7413 7c3d  ....d...j.}=t.|=
-00006d10: 7c22 8302 7d3e 7403 a009 7403 a018 7c2c  |"..}>t...t...|,
-00006d20: 7c3e 6702 a101 a101 7d2c 7c2c 7c2c 6416  |>g.....},|,|,d.
-00006d30: 6b04 1900 7d2c 7413 7c1c 7c22 8302 7d23  k...},t.|.|"..}#
-00006d40: 7c23 7c23 6416 6b04 1900 7d23 7403 a00c  |#|#d.k...}#t...
-00006d50: 7c23 7c0b a102 7d12 7c23 7403 a00d 7c12  |#|...}.|#t...|.
-00006d60: a101 1900 7d3f 7403 a009 7403 a018 7c2c  ....}?t...t...|,
-00006d70: 7c3f 6702 a101 a101 7d2c 7c2c 7c2c 6416  |?g.....},|,|,d.
-00006d80: 6b04 1900 7d2c 7403 a00c 7c2c 7c24 a102  k...},t...|,|$..
-00006d90: 7d14 7c2c 7403 a00d 7c14 a101 1900 7d2c  }.|,t...|.....},
-00006da0: 7403 a00c 7c2c 7c19 a102 7d40 7c2c 7403  t...|,|...}@|,t.
-00006db0: a00d 7c40 a101 1900 7d2c 7414 7c22 7c00  ..|@....},t.|"|.
-00006dc0: 7c08 640f 7c2c 7c0a 6422 7c31 6423 8d08  |.d.|,|.d"|1d#..
-00006dd0: 7d08 6700 7d28 7c31 640f 1700 7d31 9005  }.g.}(|1d...}1..
-00006de0: 710c 7c38 9009 72aa 7c39 9009 72aa 7c3a  q.|8..r.|9..r.|:
-00006df0: 9009 72aa 7c35 9009 72aa 7c37 9009 72aa  ..r.|5..r.|7..r.
-00006e00: 9005 710c 9005 710c 7c34 9009 72c4 7c35  ..q...q.|4..r.|5
-00006e10: 9009 72c4 7c36 9009 72c4 9005 710c 9005  ..r.|6..r...q...
-00006e20: 710c 6416 7d30 7403 a016 7c28 a101 7d2c  q.d.}0t...|(..},
-00006e30: 7c33 6416 6b04 900a 7230 7c00 6a06 7c00  |3d.k...r0|.j.|.
-00006e40: 6415 1900 7c33 6b02 1900 a001 a100 7d3c  d...|3k.......}<
-00006e50: 7c3c 6401 6402 6702 1900 a00e 6418 a101  |<d.d.g.....d...
-00006e60: 6a05 7d3d 7413 7c3d 7c22 8302 7d3e 7403  j.}=t.|=|"..}>t.
-00006e70: a009 7403 a018 7c2c 7c3e 6702 a101 a101  ..t...|,|>g.....
-00006e80: 7d2c 7c2c 7c2c 6416 6b04 1900 7d2c 7413  },|,|,d.k...},t.
-00006e90: 7c1c 7c22 8302 7d23 7c23 7c23 6416 6b04  |.|"..}#|#|#d.k.
-00006ea0: 1900 7d23 7403 a00c 7c23 7c0b a102 7d12  ..}#t...|#|...}.
-00006eb0: 7c23 7403 a00d 7c12 a101 1900 7d3f 7403  |#t...|.....}?t.
-00006ec0: a009 7403 a018 7c2c 7c3f 6702 a101 a101  ..t...|,|?g.....
-00006ed0: 7d2c 7c2c 7c2c 6416 6b04 1900 7d2c 7403  },|,|,d.k...},t.
-00006ee0: a00c 7c2c 7c24 a102 7d14 7c2c 7403 a00d  ..|,|$..}.|,t...
-00006ef0: 7c14 a101 1900 7d2c 7403 a00c 7c2c 7c19  |.....},t...|,|.
-00006f00: a102 7d40 7c2c 7403 a00d 7c40 a101 1900  ..}@|,t...|@....
-00006f10: 7d2c 7414 7c22 7c00 7c08 640f 7c2c 7c0a  },t.|"|.|.d.|,|.
-00006f20: 6422 7c31 6423 8d08 7d08 6700 7d28 7c31  d"|1d#..}.g.}(|1
-00006f30: 640f 1700 7d31 9005 710c 9004 71be 6416  d...}1..q...q.d.
-00006f40: 7c08 6a06 7c08 6415 1900 6416 6b01 6415  |.j.|.d...d.k.d.
-00006f50: 6602 3c00 6416 7c08 6a06 7c08 6415 1900  f.<.d.|.j.|.d...
-00006f60: 6416 6b01 6413 6602 3c00 6416 7c08 6a06  d.k.d.f.<.d.|.j.
-00006f70: 7c08 6415 1900 6416 6b01 641e 6602 3c00  |.d...d.k.d.f.<.
-00006f80: 6416 7c08 6a06 7c08 6415 1900 6416 6b01  d.|.j.|.d...d.k.
-00006f90: 641f 6602 3c00 6416 7c08 6a06 7c08 6415  d.f.<.d.|.j.|.d.
-00006fa0: 1900 6416 6b01 6420 6602 3c00 6416 7c08  ..d.k.d f.<.d.|.
-00006fb0: 6a06 7c08 6415 1900 6416 6b01 6421 6602  j.|.d...d.k.d!f.
-00006fc0: 3c00 7c08 7c1b 7c0c 7c1a 7c17 6605 5300  <.|.|.|.|.|.f.S.
-00006fd0: 2924 7aac 4d6f 6469 6679 2061 7474 7269  )$z.Modify attri
-00006fe0: 6275 7465 2074 6162 6c65 206d 6170 6f6c  bute table mapol
-00006ff0: 646e 6577 5f69 6e66 6f2c 2063 7265 6174  dnew_info, creat
-00007000: 6520 6e65 7720 7375 6220 6964 2066 6f72  e new sub id for
-00007010: 2073 7562 6261 7369 6e20 6e65 6564 7320   subbasin needs 
-00007020: 746f 2062 6520 6d65 7267 6564 2e0a 2020  to be merged..  
-00007030: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020    ----------..  
-00007040: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
-00007050: 2d2d 2d0a 0a20 2020 2052 6574 7572 6e73  ---..    Returns
-00007060: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  :.    -------.  
-00007070: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
-00007080: 7206 0000 0072 4900 0000 7260 0000 0072  r....rI...r`...r
-00007090: 5a00 0000 726a 0000 0072 6b00 0000 5472  Z...rj...rk...Tr
-000070a0: 0800 0000 7250 0000 0072 6c00 0000 726e  ....rP...rl...rn
-000070b0: 0000 00a9 0272 3f00 0000 da07 696e 706c  .....r?.....inpl
-000070c0: 6163 6572 6300 0000 72a1 0000 0072 4f00  acerc...r....rO.
-000070d0: 0000 2901 7298 0000 0072 5900 0000 7261  ..).r....rY...ra
-000070e0: 0000 0072 4b00 0000 724c 0000 0072 6d00  ...rK...rL...rm.
-000070f0: 0000 7201 0000 0072 bc00 0000 724a 0000  ..r....r....rJ..
-00007100: 0029 0772 2900 0000 728a 0000 0072 7400  .).r)...r....rt.
-00007110: 0000 728b 0000 0072 8d00 0000 728c 0000  ..r....r....r...
-00007120: 0072 4b00 0000 4672 5b00 0000 7269 0000  .rK...Fr[...ri..
-00007130: 0069 8096 9800 727f 0000 0072 8100 0000  .i....r....r....
-00007140: 7280 0000 0072 8200 0000 e903 0000 00a9  r....r..........
-00007150: 0872 2900 0000 728a 0000 0072 7400 0000  .r)...r....rt...
-00007160: 728b 0000 0072 8c00 0000 728d 0000 0072  r....r....r....r
-00007170: 4b00 0000 728e 0000 0029 1972 0b00 0000  K...r....).r....
-00007180: 7216 0000 00da 0b72 6573 6574 5f69 6e64  r......reset_ind
-00007190: 6578 7221 0000 0072 6500 0000 7220 0000  exr!...re...r ..
-000071a0: 0072 2300 0000 729d 0000 0072 1c00 0000  .r#...r....r....
-000071b0: 723c 0000 0072 3d00 0000 7222 0000 0072  r<...r=...r"...r
-000071c0: 8600 0000 7287 0000 0072 5c00 0000 7218  ....r....r\...r.
-000071d0: 0000 00da 0974 7261 6e73 666f 726d 721e  .....transformr.
-000071e0: 0000 0072 1f00 0000 7285 0000 0072 9000  ...r....r....r..
-000071f0: 0000 72b6 0000 00da 0761 7361 7272 6179  ..r......asarray
-00007200: 7231 0000 00da 0b63 6f6e 6361 7465 6e61  r1.....concatena
-00007210: 7465 2941 5a0d 6669 6e61 6c72 6976 5f69  te)AZ.finalriv_i
-00007220: 6e66 6f5a 0e43 6f6e 6e5f 4c61 6b65 735f  nfoZ.Conn_Lakes_
-00007230: 706c 79da 0841 7265 615f 4d69 6e72 8f00  ply..Area_Minr..
-00007240: 0000 da0a 646f 776e 5f63 6f6c 6e6d 5a08  ....down_colnmZ.
-00007250: 4441 5f63 6f6c 6e6d 5a0b 5365 6749 445f  DA_colnmZ.SegID_
-00007260: 636f 6c6e 6d72 7600 0000 7274 0000 005a  colnmrv...rt...Z
-00007270: 066d 6178 5f64 615a 0c53 656c 6563 7465  .max_daZ.Selecte
-00007280: 645f 7269 765a 0a53 7562 6964 5f6d 6169  d_rivZ.Subid_mai
-00007290: 6e5a 1643 6f6e 6e65 6374 6564 5f4c 616b  nZ.Connected_Lak
-000072a0: 655f 4d61 696e 7269 765a 0d4c 616b 6563  e_MainrivZ.Lakec
-000072b0: 6f76 6572 5f72 6976 5a0b 5375 6269 645f  over_rivZ.Subid_
-000072c0: 6c61 6b65 735a 1d75 6e73 656c 6563 7465  lakesZ.unselecte
-000072d0: 645f 6761 7567 6573 5f73 7562 6964 735f  d_gauges_subids_
-000072e0: 696e 666f 5a18 756e 7365 6c65 6374 6564  infoZ.unselected
-000072f0: 5f67 6175 6765 735f 7375 6269 6473 5a11  _gauges_subidsZ.
-00007300: 6669 6e61 6c72 6976 5f69 6e66 6f5f 6e63  finalriv_info_nc
-00007310: 6c72 2a00 0000 722b 0000 0072 2c00 0000  lr*...r+...r,...
-00007320: 5a12 6661 6b65 5f6f 6273 5f68 7961 6c6b  Z.fake_obs_hyalk
-00007330: 6569 6473 5a10 416c 6c5f 436f 6e6e 5f4c  eidsZ.All_Conn_L
-00007340: 616b 6569 6473 5a15 436f 6e6e 5f54 6f5f  akeidsZ.Conn_To_
-00007350: 4e6f 6e43 6f6e 6c61 6b65 6964 735a 1743  NonConlakeidsZ.C
-00007360: 6f6e 6e5f 546f 5f4e 6f6e 436f 6e6c 616b  onn_To_NonConlak
-00007370: 655f 696e 666f 5a16 4f6c 645f 4e6f 6e5f  e_infoZ.Old_Non_
-00007380: 436f 6e6e 6563 745f 5375 6249 6473 5a17  Connect_SubIdsZ.
-00007390: 4f6c 645f 4e6f 6e5f 436f 6e6e 6563 745f  Old_Non_Connect_
-000073a0: 4c61 6b65 4964 735a 1053 656c 6563 7465  LakeIdsZ.Selecte
-000073b0: 645f 7269 765f 6964 7372 5e00 0000 da07  d_riv_idsr^.....
-000073c0: 5365 675f 4944 5372 4500 0000 5a1e 436f  Seg_IDSrE...Z.Co
-000073d0: 6e6e 5f54 6f5f 4e6f 6e43 6f6e 6c61 6b65  nn_To_NonConlake
-000073e0: 5f69 6e66 6f5f 6f75 746c 6574 5a13 616c  _info_outletZ.al
-000073f0: 6c5f 6f75 746c 6574 5f73 7562 5f69 6e66  l_outlet_sub_inf
-00007400: 6f72 2800 0000 da06 7473 7562 6964 5a0d  or(.....tsubidZ.
-00007410: 416c 6c5f 7570 5f73 7562 6964 735a 0f70  All_up_subidsZ.p
-00007420: 726f 6365 7373 6564 5f73 7562 6964 5a0c  rocessed_subidZ.
-00007430: 435f 545f 4e5f 4c61 6b65 6964 5a0d 4c61  C_T_N_LakeidZ.La
-00007440: 6b65 5f43 6174 5f69 6e66 6f5a 0b52 6976  ke_Cat_infoZ.Riv
-00007450: 5f53 6567 5f49 4453 da0c 6d6f 6469 6679  _Seg_IDS..modify
-00007460: 7375 6269 6473 7244 0000 005a 0869 7269  subidsrD...Z.iri
-00007470: 765f 7365 675a 114c 616b 655f 4361 745f  v_segZ.Lake_Cat_
-00007480: 7365 675f 696e 666f da0b 7365 675f 7375  seg_info..seg_su
-00007490: 625f 6964 7372 a400 0000 da08 695f 7365  b_idsr......i_se
-000074a0: 675f 6964 da0a 695f 7365 675f 696e 666f  g_id..i_seg_info
-000074b0: 5a08 7375 6d5f 6172 6561 728e 0000 00da  Z.sum_arear.....
-000074c0: 0669 6f72 6465 725a 0d69 6f72 6465 725f  .iorderZ.iorder_
-000074d0: 4c61 6b65 6964 5a08 636f 6e5f 6c61 6b65  LakeidZ.con_lake
-000074e0: 5a09 636f 6e5f 6761 7567 655a 0863 6f6e  Z.con_gaugeZ.con
-000074f0: 5f61 7265 615a 0d63 6f6e 5f61 7265 615f  _areaZ.con_area_
-00007500: 6c61 6b65 5a0b 636f 6e5f 6c61 6b65 5f75  lakeZ.con_lake_u
-00007510: 705a 0d63 6f6e 5f6c 616b 655f 646f 776e  pZ.con_lake_down
-00007520: 5a07 6973 5f6c 616b 6572 b900 0000 5a13  Z.is_laker....Z.
-00007530: 7375 6269 645f 6375 725f 6c61 6b65 5f69  subid_cur_lake_i
-00007540: 6e66 6f5a 1172 6f75 7469 6e67 5f69 6e66  nfoZ.routing_inf
-00007550: 6f5f 6c61 6b65 5a0f 5570 7374 7265 616d  o_lakeZ.Upstream
-00007560: 4c61 6b65 6964 735a 1541 6c6c 5f75 705f  LakeidsZ.All_up_
-00007570: 7375 6269 6473 5f6e 6f5f 6d61 696e 5a10  subids_no_mainZ.
-00007580: 6d61 736b 5f6f 6c64 5f6e 6f6e 4c61 6b65  mask_old_nonLake
-00007590: 722d 0000 0072 2d00 0000 722e 0000 00da  r-...r-...r.....
-000075a0: 4743 6861 6e67 655f 4174 7472 6962 7574  GChange_Attribut
-000075b0: 655f 5661 6c75 6573 5f46 6f72 5f43 6174  e_Values_For_Cat
-000075c0: 6368 6d65 6e74 735f 4e65 6564 5f54 6f5f  chments_Need_To_
-000075d0: 4265 5f4d 6572 6765 645f 4279 5f49 6e63  Be_Merged_By_Inc
-000075e0: 7265 6173 655f 4441 d906 0000 7362 0200  rease_DA....sb..
-000075f0: 0000 0d04 0104 0104 0104 0204 010a 0104  ................
-00007600: 070c 0108 0108 010e 0110 0310 0110 0108  ................
-00007610: 0108 0404 0112 ff08 050c 0104 0106 ff06  ................
-00007620: 0316 010a 0310 0102 ff06 0304 010a ff04  ................
-00007630: 0304 010c ff08 030a 0504 010e 010a ff02  ................
-00007640: ff04 0302 fd06 0418 020c 020e 010c 010c  ................
-00007650: 0124 011a 040a 010c 0112 0104 010c 010c  .$..............
-00007660: ff02 ff08 0a10 0102 ff06 0304 010a ff04  ................
-00007670: 0310 0102 ff06 0304 010a ff04 0504 0102  ................
-00007680: ff04 0314 010a 010a 0304 010a ff02 0202  ................
-00007690: fe18 0614 0106 ff02 ff02 0408 0204 010c  ................
-000076a0: ff06 0618 0212 011c 010e 010a 0202 0102  ................
-000076b0: 0102 0102 0102 0102 0102 0102 f90a 0d14  ................
-000076c0: 0104 0116 ff04 040e 0110 0110 0104 0112  ................
-000076d0: 0208 0104 010a ff08 0310 010e 020a 010c  ................
-000076e0: 020c 010e 0202 0102 ff02 0206 fe08 050a  ................
-000076f0: 0202 0102 0102 0102 0102 0102 0102 0102  ................
-00007700: f90a 0b14 0208 0116 0110 0104 0104 0104  ................
-00007710: 0114 010e 010e 010a 0104 0116 ff04 0312  ................
-00007720: 0412 0122 0204 0212 0312 0118 0106 0212  ..."............
-00007730: 0210 0308 021c 0220 0220 0212 0212 021c  ....... . ......
-00007740: 0204 0220 0212 0212 0226 0204 0220 0212  ... .....&... ..
-00007750: 050e 0216 020c 020c ff04 010e ff02 030c  ................
-00007760: ff04 010e ff02 030c ff04 010e ff02 030c  ................
-00007770: ff04 010e ff02 030c ff04 010e ff02 030c  ................
-00007780: ff04 010e ff02 0312 0104 0104 0104 0712  ................
-00007790: 0104 010a 020a 0104 010a ff08 040c 0102  ................
-000077a0: ff04 ff02 050a 0104 010c ff04 030c 030a  ................
-000077b0: 010c 0104 0104 ff04 030e 0204 010c ff04  ................
-000077c0: 030c 010c 010e 020c 010e 0202 0102 0102  ................
-000077d0: 0102 0102 0102 0102 0102 0102 f806 0b04  ................
-000077e0: 010c 021e 0108 0212 0108 0304 010a 020a  ................
-000077f0: 0104 010a ff08 040c 0102 ff04 ff02 050a  ................
-00007800: 0104 010c ff04 030c 020a 010c 0104 0104  ................
-00007810: ff04 030e 0204 010c ff04 030c 010c 010e  ................
-00007820: 020c 010e 0302 0102 0102 0102 0102 0102  ................
-00007830: 0102 0102 0102 f806 0a04 0110 0216 0116  ................
-00007840: 0116 0116 0116 0116 0302 0102 0102 0102  ................
-00007850: 0102 fb72 e000 0000 6304 0000 0000 0000  ...r....c.......
-00007860: 0000 0000 0012 0000 0007 0000 0043 0000  .............C..
-00007870: 0073 b201 0000 7c00 6401 1900 a000 7401  .s....|.d.....t.
-00007880: a101 7c00 6401 3c00 7c00 6402 1900 a000  ..|.d.<.|.d.....
-00007890: 7402 a101 7c00 6402 3c00 7c00 6403 1900  t...|.d.<.|.d...
-000078a0: a000 7402 a101 7c00 6403 3c00 7c00 6a03  ..t...|.d.<.|.j.
-000078b0: 7c00 6404 1900 6405 6b02 1900 6a04 6406  |.d...d.k...j.d.
-000078c0: 6407 8d01 7d04 7c00 6a03 7c00 6404 1900  d...}.|.j.|.d...
-000078d0: 6408 6b02 1900 6a04 6406 6407 8d01 7d05  d.k...j.d.d...}.
-000078e0: 7c05 6a03 7c05 6401 1900 7c01 6b05 1900  |.j.|.d...|.k...
-000078f0: 6402 1900 6a05 7d06 7c06 7c06 6409 6b04  d...j.}.|.|.d.k.
-00007900: 1900 7d06 7406 a007 7c06 a101 7d06 7c04  ..}.t...|...}.|.
-00007910: 7c04 6401 1900 7c02 6b05 1900 6402 1900  |.d...|.k...d...
-00007920: 6a05 7d07 7c07 7c07 6409 6b04 1900 7d07  j.}.|.|.d.k...}.
-00007930: 7406 a007 7c07 a101 7d07 7408 7c03 8301  t...|...}.t.|...
-00007940: 6409 6b04 72d6 7c03 7d08 6e06 640a 6701  d.k.r.|.}.n.d.g.
-00007950: 7d08 7c05 6402 1900 6a05 7d09 7c04 6402  }.|.d...j.}.|.d.
-00007960: 1900 6a05 7d0a 7406 a009 7c08 a101 7d0b  ..j.}.t...|...}.
-00007970: 7406 a00a 7c09 7c0b a102 7d0c 7406 a00a  t...|.|...}.t...
-00007980: 7c0a 7c0b a102 7d0d 7c09 7c0c 1900 7d0e  |.|...}.|.|...}.
-00007990: 7406 a007 7c0e a101 7d0e 7c0a 7c0d 1900  t...|...}.|.|...
-000079a0: 7d0f 7406 a007 7c0f a101 7d0f 7406 6a0b  }.t...|...}.t.j.
-000079b0: 7c07 7c0f 6602 6409 640b 8d02 7d07 7406  |.|.f.d.d...}.t.
-000079c0: 6a0b 7c06 7c0e 6602 6409 640b 8d02 7d06  j.|.|.f.d.d...}.
-000079d0: 7c00 6a03 7c00 6404 1900 6408 6b02 7406  |.j.|.d...d.k.t.
-000079e0: a00c 7c00 6402 1900 a00d 7c06 a101 a101  ..|.d.....|.....
-000079f0: 4000 1900 7d10 7c00 6a03 7c00 6404 1900  @...}.|.j.|.d...
-00007a00: 6405 6b02 7406 a00c 7c00 6402 1900 a00d  d.k.t...|.d.....
-00007a10: 7c07 a101 a101 4000 1900 7d11 7c07 7c06  |.....@...}.|.|.
-00007a20: 7c10 7c11 6604 5300 290c 7a80 5265 7472  |.|.f.S.).z.Retr
-00007a30: 756e 2073 656c 6563 7465 6420 6c61 6b65  un selected lake
-00007a40: 2773 2061 7474 7269 6275 7465 2074 6162  's attribute tab
-00007a50: 6c65 2061 6e64 2049 440a 2020 2020 2d2d  le and ID.    --
-00007a60: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 4e6f  --------..    No
-00007a70: 7465 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  tes.    -------.
-00007a80: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00007a90: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00007aa0: 2020 4e6f 6e65 2c0a 2020 2020 7280 0000    None,.    r...
-00007ab0: 0072 6d00 0000 725a 0000 0072 4b00 0000  .rm...rZ...rK...
-00007ac0: 724c 0000 0054 7208 0000 0072 4f00 0000  rL...Tr....rO...
-00007ad0: 7201 0000 0069 8169 67ff a901 da04 6178  r....i.ig.....ax
-00007ae0: 6973 290e 725c 0000 0072 4a00 0000 72a3  is).r\...rJ...r.
-00007af0: 0000 0072 2300 0000 7216 0000 0072 2000  ...r#...r....r .
-00007b00: 0000 7221 0000 0072 3c00 0000 721f 0000  ..r!...r<...r...
-00007b10: 00da 0561 7272 6179 7286 0000 0072 d600  ...arrayr....r..
-00007b20: 0000 7287 0000 0072 3d00 0000 2912 da0d  ..r....r=...)...
-00007b30: 6669 6e61 6c63 6174 5f69 6e66 6fda 1554  finalcat_info..T
-00007b40: 6872 6573 5f41 7265 615f 436f 6e6e 5f4c  hres_Area_Conn_L
-00007b50: 616b 6573 da19 5468 7265 735f 4172 6561  akes..Thres_Area
-00007b60: 5f4e 6f6e 5f43 6f6e 6e5f 4c61 6b65 73da  _Non_Conn_Lakes.
-00007b70: 1553 656c 6563 7465 645f 4c61 6b65 5f4c  .Selected_Lake_L
-00007b80: 6973 745f 696e 5a0e 4e6f 6e5f 436f 6e6e  ist_inZ.Non_Conn
-00007b90: 4c5f 696e 666f 5a0a 436f 6e6e 4c5f 696e  L_infoZ.ConnL_in
-00007ba0: 666f 5a12 5365 6c65 6374 6564 5f43 6f6e  foZ.Selected_Con
-00007bb0: 6e4c 616b 6573 5a16 5365 6c65 6374 6564  nLakesZ.Selected
-00007bc0: 5f4e 6f6e 5f43 6f6e 6e4c 616b 6573 5a12  _Non_ConnLakesZ.
-00007bd0: 5365 6c65 6374 6564 5f4c 616b 655f 4c69  Selected_Lake_Li
-00007be0: 7374 5a09 416c 6c5f 436f 6e6e 4c5a 0d41  stZ.All_ConnLZ.A
-00007bf0: 6c6c 5f4e 6f6e 5f43 6f6e 6e4c 5a1b 5365  ll_Non_ConnLZ.Se
-00007c00: 6c65 6374 6564 5f4c 616b 655f 4c69 7374  lected_Lake_List
-00007c10: 5f69 6e5f 6172 7261 795a 076d 6173 6b5f  _in_arrayZ.mask_
-00007c20: 434c 5a08 6d61 736b 5f4e 434c 5a17 5365  CLZ.mask_NCLZ.Se
-00007c30: 6c65 6374 6564 5f43 6f6e 6e4c 616b 6573  lected_ConnLakes
-00007c40: 5f4c 6973 745a 1b53 656c 6563 7465 645f  _ListZ.Selected_
-00007c50: 4e6f 6e5f 436f 6e6e 4c61 6b65 735f 4c69  Non_ConnLakes_Li
-00007c60: 7374 da1a 556e 5f53 656c 6563 7465 645f  st..Un_Selected_
-00007c70: 436f 6e6e 4c61 6b65 735f 696e 666f da1a  ConnLakes_info..
-00007c80: 556e 5f53 656c 6563 7465 645f 4e6f 6e5f  Un_Selected_Non_
-00007c90: 436f 6e6e 4c5f 696e 666f 722d 0000 0072  ConnL_infor-...r
-00007ca0: 2d00 0000 722e 0000 00da 2c52 6574 7572  -...r.....,Retur
-00007cb0: 6e5f 5365 6c65 6374 6564 5f4c 616b 6573  n_Selected_Lakes
-00007cc0: 5f41 7474 7269 6275 7465 5f54 6162 6c65  _Attribute_Table
-00007cd0: 5f41 6e64 5f49 647b 0800 0073 6000 0000  _And_Id{...s`...
-00007ce0: 0010 1201 1201 1202 1a01 1a04 0401 0aff  ................
-00007cf0: 0202 02fe 0604 0c01 0a04 0201 0aff 0202  ................
-00007d00: 02fe 0603 0c01 0a04 0c01 0603 0601 0a01  ................
-00007d10: 0a01 0a02 0c01 0c02 0801 0a01 0801 0a03  ................
-00007d20: 1201 1202 0401 0a01 12ff 02ff 0404 0401  ................
-00007d30: 0a01 12ff 02ff 0406 0201 0201 0201 02fc  ................
-00007d40: 72ea 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00007d50: 0000 0e00 0000 0c00 0000 4300 0000 7322  ..........C...s"
-00007d60: 0200 007c 006a 0064 0164 028d 017d 0264  ...|.j.d.d...}.d
-00007d70: 037c 0264 043c 0064 037c 0264 053c 007c  .|.d.<.d.|.d.<.|
-00007d80: 0264 0619 007c 0264 073c 007c 026a 0164  .d...|.d.<.|.j.d
-00007d90: 0164 0164 088d 0201 0064 097d 0364 097c  .d.d.....d.}.d.|
-00007da0: 026a 0276 0172 4864 0a7d 037c 0164 0b19  .j.v.rHd.}.|.d..
-00007db0: 006a 037d 0474 04a0 057c 04a1 017d 0474  .j.}.t...|...}.t
-00007dc0: 0664 0c74 077c 0483 0183 0244 0090 015d  .d.t.|.....D...]
-00007dd0: b07d 057c 047c 0519 007d 067c 006a 087c  .}.|.|...}.|.j.|
-00007de0: 0064 0b19 007c 066b 027c 0064 0d19 0064  .d...|.k.|.d...d
-00007df0: 0e6b 0340 0019 00a0 00a1 007d 077c 076a  .k.@.......}.|.j
-00007e00: 0964 0f67 0164 0164 108d 027d 0774 04a0  .d.g.d.d...}.t..
-00007e10: 057c 0764 1119 006a 03a1 017d 0874 077c  .|.d...j...}.t.|
-00007e20: 0783 0174 077c 0883 016b 0272 cc71 6a74  ...t.|...k.r.qjt
-00007e30: 04a0 0a7c 08a1 0190 0172 2674 04a0 0a7c  ...|.....r&t...|
-00007e40: 077c 0319 006a 03a1 0164 0c6b 0190 0172  .|...j...d.k...r
-00007e50: 267c 0764 0619 006a 0374 077c 0783 0164  &|.d...j.t.|...d
-00007e60: 1218 0019 007d 097c 0764 0619 006a 037d  .....}.|.d...j.}
-00007e70: 0a74 0b7c 097c 007c 0264 127c 0a7c 0064  .t.|.|.|.d.|.|.d
-00007e80: 0364 1264 138d 087d 0267 007d 0b64 127d  .d.d...}.g.}.d.}
-00007e90: 0c74 0664 0c74 077c 0783 0183 0244 005d  .t.d.t.|.....D.]
-00007ea0: de7d 0d7c 0764 0619 006a 037c 0d19 007d  .}.|.d...j.|...}
-00007eb0: 097c 0ba0 0c7c 09a1 0101 007c 0d74 077c  .|...|.....|.t.|
-00007ec0: 0783 0164 1218 006b 0290 0172 a474 04a0  ...d...k...r.t..
-00007ed0: 0d7c 0ba1 017d 0a74 0b7c 097c 007c 0264  .|...}.t.|.|.|.d
-00007ee0: 127c 0a7c 007c 0764 1119 006a 037c 0d19  .|.|.|.d...j.|..
-00007ef0: 007c 0c64 138d 087d 0267 007d 0b7c 0c64  .|.d...}.g.}.|.d
-00007f00: 1217 007d 0c6e 747c 0764 1119 006a 037c  ...}.nt|.d...j.|
-00007f10: 0d19 007c 0764 1119 006a 037c 0d64 1217  ...|.d...j.|.d..
-00007f20: 0019 006b 0290 0172 e07c 077c 0319 006a  ...k...r.|.|...j
-00007f30: 037c 0d19 0064 0c6b 0190 0172 e090 0171  .|...d.k...r...q
-00007f40: 3c6e 3874 04a0 0d7c 0ba1 017d 0a74 0b7c  <n8t...|...}.t.|
-00007f50: 097c 007c 0264 127c 0a7c 007c 0764 1119  .|.|.d.|.|.|.d..
-00007f60: 006a 037c 0d19 007c 0c64 138d 087d 0267  .j.|...|.d...}.g
-00007f70: 007d 0b7c 0c64 1217 007d 0c90 0171 3c71  .}.|.d...}...q<q
-00007f80: 6a7c 0253 0029 147a b143 6861 6e67 6520  j|.S.).z.Change 
-00007f90: 6174 7472 6962 7574 6573 2066 6f72 2063  attributes for c
-00007fa0: 6174 6368 6d65 6e74 7320 7468 6174 206e  atchments that n
-00007fb0: 6565 6473 2074 6f20 6265 206d 6572 6765  eeds to be merge
-00007fc0: 6420 6475 6520 746f 2072 656d 6f76 650a  d due to remove.
-00007fd0: 2020 2020 2020 2020 636f 6e6e 6563 7465          connecte
-00007fe0: 6420 6c61 6b65 730a 2020 2020 2d2d 2d2d  d lakes.    ----
-00007ff0: 2d2d 2d2d 2d2d 0a0a 2020 2020 4e6f 7465  ------..    Note
-00008000: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20  s.    -------.. 
-00008010: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00008020: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00008030: 4e6f 6e65 2c0a 2020 2020 5472 0800 0000  None,.    Tr....
-00008040: 7250 0000 0072 6c00 0000 726e 0000 0072  rP...rl...rn...r
-00008050: 0600 0000 da07 6e73 7562 6964 3272 cf00  ......nsubid2r..
-00008060: 0000 726a 0000 0072 6b00 0000 725a 0000  ..rj...rk...rZ..
-00008070: 0072 0100 0000 724b 0000 0072 4c00 0000  .r....rK...rL...
-00008080: 725b 0000 0072 6100 0000 726d 0000 0072  r[...ra...rm...r
-00008090: 4f00 0000 72d2 0000 0029 0e72 1600 0000  O...r....).r....
-000080a0: 72d3 0000 0072 0b00 0000 7220 0000 0072  r....r....r ...r
-000080b0: 2100 0000 723c 0000 0072 1e00 0000 721f  !...r<...r....r.
-000080c0: 0000 0072 2300 0000 721c 0000 0072 6500  ...r#...r....re.
-000080d0: 0000 7290 0000 0072 3100 0000 72d5 0000  ..r....r1...r...
-000080e0: 0029 0eda 1266 696e 616c 6361 745f 696e  .)...finalcat_in
-000080f0: 666f 5f74 656d 7072 e800 0000 7274 0000  fo_tempr....rt..
-00008100: 0072 7600 0000 72d9 0000 0072 a400 0000  .rv...r....r....
-00008110: 72dd 0000 0072 de00 0000 5a0a 4e5f 4879  r....r....Z.N_Hy
-00008120: 6c61 6b65 6964 72da 0000 0072 dc00 0000  lakeidr....r....
-00008130: 72db 0000 0072 8e00 0000 72df 0000 0072  r....r....r....r
-00008140: 2d00 0000 722d 0000 0072 2e00 0000 da45  -...r-...r.....E
-00008150: 4368 616e 6765 5f41 7474 7269 6275 7465  Change_Attribute
-00008160: 5f56 616c 7565 735f 466f 725f 4361 7463  _Values_For_Catc
-00008170: 686d 656e 7473 5f4e 6565 645f 546f 5f42  hments_Need_To_B
-00008180: 655f 4d65 7267 6564 5f42 795f 5265 6d6f  e_Merged_By_Remo
-00008190: 7665 5f43 4ccb 0800 0073 9400 0000 000e  ve_CL....s......
-000081a0: 0c01 0801 0801 0c01 0e03 0401 0a01 0403  ................
-000081b0: 0a01 0a01 1402 0801 0401 0a01 0aff 02ff  ................
-000081c0: 0804 1003 1001 1001 0203 2201 1601 0a01  ..........".....
-000081d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000081e0: 02f8 060c 0401 0401 1201 0e01 0a03 1201  ................
-000081f0: 0a01 0201 0201 0201 0201 0201 0201 0201  ................
-00008200: 0c01 02f8 060a 0401 0a03 0c01 10ff 02ff  ................
-00008210: 0403 10fd 0405 0602 0a01 0201 0201 0201  ................
-00008220: 0201 0201 0201 0201 0c01 02f8 060a 0401  ................
-00008230: 0e01 72ed 0000 0063 0300 0000 0000 0000  ..r....c........
-00008240: 0000 0000 0f00 0000 0a00 0000 4300 0000  ............C...
-00008250: 7300 0200 007c 026a 0064 0167 0164 0267  s....|.j.d.g.d.g
-00008260: 0164 038d 027d 0274 0164 0474 027c 0283  .d...}.t.d.t.|..
-00008270: 0183 0244 0090 015d a47d 037c 0264 0519  ...D...].}.|.d..
-00008280: 006a 037c 0319 007d 047c 016a 047c 0164  .j.|...}.|.j.|.d
-00008290: 0519 007c 046b 0219 00a0 05a1 007d 0574  ...|.k.......}.t
-000082a0: 027c 0583 0164 066b 0372 6874 0664 0783  .|...d.k.rht.d..
-000082b0: 0101 0074 067c 0583 0101 0071 2067 007d  ...t.|.....q g.}
-000082c0: 067c 0564 0819 006a 0364 0419 007d 077c  .|.d...j.d...}.|
-000082d0: 0564 0919 006a 0364 0419 007d 087c 06a0  .d...j.d...}.|..
-000082e0: 077c 07a1 0101 0064 0a7d 0964 047d 0a7c  .|.....d.}.d.}.|
-000082f0: 016a 047c 0164 0819 007c 086b 0219 00a0  .j.|.d...|.k....
-00008300: 05a1 007d 0b74 027c 0b83 0164 046b 0272  ...}.t.|...d.k.r
-00008310: c67c 0864 046b 0072 c671 207c 0b64 0b19  .|.d.k.r.q |.d..
-00008320: 006a 0364 0419 0064 0c6b 0390 0172 287c  .j.d...d.k...r(|
-00008330: 006a 047c 0064 0819 007c 086b 0219 0064  .j.|.d...|.k...d
-00008340: 0d19 006a 0364 0419 007d 0c7c 0c64 046b  ...j.d...}.|.d.k
-00008350: 0490 0172 147c 0c7d 0964 067d 0a7c 06a0  ...r.|.}.d.}.|..
-00008360: 077c 09a1 0101 006e 127c 087d 0964 0a7d  .|.....n.|.}.d.}
-00008370: 0a7c 06a0 077c 09a1 0101 006e 4c7c 006a  .|...|.....nL|.j
-00008380: 047c 0064 0819 007c 086b 0219 0064 0d19  .|.d...|.k...d..
-00008390: 006a 0364 0419 007d 0c7c 0c64 046b 0490  .j.d...}.|.d.k..
-000083a0: 0172 627c 0c7d 0964 067d 0a7c 06a0 077c  .rb|.}.d.}.|...|
-000083b0: 09a1 0101 006e 127c 087d 0964 0a7d 0a7c  .....n.|.}.d.}.|
-000083c0: 06a0 077c 09a1 0101 007c 007c 0064 0819  ...|.....|.|.d..
-000083d0: 007c 096b 0219 0064 0519 006a 0364 0419  .|.k...d...j.d..
-000083e0: 007d 0d7c 0a64 046b 0490 0172 b074 087c  .}.|.d.k...r.t.|
-000083f0: 097c 007c 0064 067c 067c 017c 0d64 0e8d  .|.|.d.|.|.|.d..
-00008400: 077d 0071 2074 087c 097c 007c 0064 067c  .}.q t.|.|.|.d.|
-00008410: 067c 017c 0d64 0e8d 077d 0071 207c 0064  .|.|.d...}.q |.d
-00008420: 0d19 0064 046b 017d 0e7c 006a 047c 0e64  ...d.k.}.|.j.|.d
-00008430: 0f66 0219 006a 037c 006a 047c 0e64 0d66  .f...j.|.j.|.d.f
-00008440: 023c 007c 006a 0964 0f67 0164 108d 0101  .<.|.j.d.g.d....
-00008450: 007c 0053 0029 117a b543 6861 6e67 6520  .|.S.).z.Change 
-00008460: 6174 7472 6962 7574 6573 2066 6f72 2063  attributes for c
-00008470: 6174 6368 6d65 6e74 7320 7468 6174 206e  atchments that n
-00008480: 6565 6473 2074 6f20 6265 206d 6572 6765  eeds to be merge
-00008490: 6420 6475 6520 746f 2072 656d 6f76 650a  d due to remove.
-000084a0: 2020 2020 2020 2020 6e6f 6e20 636f 6e6e          non conn
-000084b0: 6563 7465 6420 6c61 6b65 730a 2020 2020  ected lakes.    
-000084c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
-000084d0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d2d  Notes.    ------
-000084e0: 2d0a 0a20 2020 2052 6574 7572 6e73 3a0a  -..    Returns:.
-000084f0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00008500: 2020 2020 4e6f 6e65 2c0a 2020 2020 7260      None,.    r`
-00008510: 0000 0046 7261 0000 0072 0100 0000 726d  ...Fra...r....rm
-00008520: 0000 0072 4f00 0000 7a28 4974 2069 7320  ...rO...z(It is 
-00008530: 6e6f 7420 6120 6e6f 6e20 636f 6e6e 6563  not a non connec
-00008540: 7465 6420 6c61 6b65 2063 6174 6368 6d65  ted lake catchme
-00008550: 6e74 7206 0000 0072 4900 0000 7250 0000  ntr....rI...rP..
-00008560: 0072 4b00 0000 724c 0000 0072 6c00 0000  .rK...rL...rl...
-00008570: a907 7229 0000 0072 8a00 0000 7274 0000  ..r)...r....rt..
-00008580: 0072 8b00 0000 728c 0000 0072 8d00 0000  .r....r....r....
-00008590: 724b 0000 0072 eb00 0000 720a 0000 0029  rK...r....r....)
-000085a0: 0a72 1c00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000085b0: 7220 0000 0072 2300 0000 7216 0000 0072  r ...r#...r....r
-000085c0: 7300 0000 7231 0000 0072 9000 0000 723f  s...r1...r....r?
-000085d0: 0000 0029 0f72 7400 0000 72ec 0000 0072  ...).rt...r....r
-000085e0: e900 0000 7228 0000 005a 1752 656d 6f76  ....r(...Z.Remov
-000085f0: 655f 4e6f 6e5f 436f 6e6e 4c5f 4c61 6b65  e_Non_ConnL_Lake
-00008600: 6964 5a1e 5265 6d6f 7665 5f4e 6f6e 5f43  idZ.Remove_Non_C
-00008610: 6f6e 6e4c 5f4c 616b 655f 5375 625f 696e  onnL_Lake_Sub_in
-00008620: 666f 72db 0000 0072 ba00 0000 72b9 0000  for....r....r...
-00008630: 0072 da00 0000 5a0f 6973 5f70 7265 5f6d  .r....Z.is_pre_m
-00008640: 6f64 6966 6965 6472 b300 0000 726c 0000  odifiedr....rl..
-00008650: 005a 0b54 6172 5f4c 616b 655f 4964 5a0f  .Z.Tar_Lake_IdZ.
-00008660: 756e 7072 6f63 6573 7365 646d 6173 6b72  unprocessedmaskr
-00008670: 2d00 0000 722d 0000 0072 2e00 0000 da46  -...r-...r.....F
-00008680: 4368 616e 6765 5f41 7474 7269 6275 7465  Change_Attribute
-00008690: 5f56 616c 7565 735f 466f 725f 4361 7463  _Values_For_Catc
-000086a0: 686d 656e 7473 5f4e 6565 645f 546f 5f42  hments_Need_To_B
-000086b0: 655f 4d65 7267 6564 5f42 795f 5265 6d6f  e_Merged_By_Remo
-000086c0: 7665 5f4e 434c 3209 0000 73a4 0000 0000  ve_NCL2...s.....
-000086d0: 0f04 0108 ff06 0314 0108 0102 ff04 0304  ................
-000086e0: 010a ff08 030c 0108 0108 0102 0104 010e  ................
-000086f0: 0108 0102 ff04 030a 0104 0104 0204 010a  ................
-00008700: ff08 0314 0102 0114 0210 0102 ff04 0302  ................
-00008710: fd04 060a 0104 0104 010c 0204 0104 010c  ................
-00008720: 0410 0102 ff04 0202 fe04 030a 0104 0104  ................
-00008730: 010c 0204 0204 010a 020e 0102 ff04 0202  ................
-00008740: fe04 040a 0102 0102 0102 0102 0102 0102  ................
-00008750: 0102 0102 f908 0a02 0102 0102 0102 0102  ................
-00008760: 0102 0102 0102 f908 0a0c 0204 0106 ff10  ................
-00008770: 040e 0272 ef00 0000 6301 0000 0000 0000  ...r....c.......
-00008780: 0000 0000 0009 0000 000a 0000 0043 0000  .............C..
-00008790: 0073 cc00 0000 6401 7d01 7c00 6a00 6402  .s....d.}.|.j.d.
-000087a0: 6403 8d01 7d02 7c02 6401 1900 6a01 7c02  d...}.|.d...j.|.
-000087b0: 6404 3c00 7c02 6404 1900 a002 6405 a101  d.<.|.d.....d...
-000087c0: 7c02 6404 3c00 7c00 6406 1900 6a01 7d03  |.d.<.|.d...j.}.
-000087d0: 7c03 7c03 6407 6b04 1900 7d03 7403 a004  |.|.d.k...}.t...
-000087e0: 7c03 a101 7d03 7405 6407 7406 7c03 8301  |...}.t.d.t.|...
-000087f0: 8302 4400 5d68 7d04 7c03 7c04 1900 7d05  ..D.]h}.|.|...}.
-00008800: 7c00 6a07 7c00 6406 1900 7c05 6b02 1900  |.j.|.d...|.k...
-00008810: 7d06 7c06 6a08 6408 6701 6409 640a 8d02  }.|.j.d.g.d.d...
-00008820: 7d06 7c06 7c01 1900 6a01 6407 1900 7d07  }.|.|...j.d...}.
-00008830: 7c06 7c01 1900 6a01 7d08 7406 7c08 8301  |.|...j.}.t.|...
-00008840: 640b 6b04 725e 7409 7c07 7c00 7c02 640b  d.k.r^t.|.|.|.d.
-00008850: 7c08 7c00 640b 640c 8d07 7d02 715e 7c02  |.|.d.d...}.q^|.
-00008860: 5300 290d e12c 0100 0043 6861 6e67 6520  S.)..,...Change 
-00008870: 6174 7472 6962 7574 6573 2066 6f72 2063  attributes for c
-00008880: 6174 6368 6d65 6e74 7320 7468 6174 2063  atchments that c
-00008890: 6f76 6572 6564 2062 7920 7468 6520 7361  overed by the sa
-000088a0: 6d65 206c 616b 652e 0a20 2020 202d 2d2d  me lake..    ---
-000088b0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 6f74  -------..    Not
-000088c0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  es.    -------. 
-000088d0: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
-000088e0: 6c65 2c20 6c61 6b65 2027 6c61 2720 636f  le, lake 'la' co
-000088f0: 7665 7269 6e67 2063 6174 6368 6d65 6e74  vering catchment
-00008900: 2061 2c62 2c63 2e20 7468 6520 6c61 6b65   a,b,c. the lake
-00008910: 206f 7574 6c65 7420 6361 7463 686d 656e   outlet catchmen
-00008920: 740a 2020 2020 2020 2020 6973 2061 2e20  t.        is a. 
-00008930: 7468 656e 2074 6869 7320 6675 6e63 7469  then this functi
-00008940: 6f6e 2077 696c 6c20 6368 616e 6765 2061  on will change a
-00008950: 7474 7269 6275 7465 206f 6620 6220 616e  ttribute of b an
-00008960: 6420 6320 746f 2061 2e0a 2020 2020 5265  d c to a..    Re
-00008970: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-00008980: 2d2d 0a20 2020 2020 2020 204e 6f6e 652c  --.        None,
-00008990: 0a20 2020 2072 0600 0000 5472 0800 0000  .    r....Tr....
-000089a0: 726c 0000 0072 7b00 0000 726d 0000 0072  rl...r{...rm...r
-000089b0: 0100 0000 7260 0000 0046 7261 0000 0072  ....r`...Fra...r
-000089c0: 4f00 0000 72ee 0000 0029 0a72 1600 0000  O...r....).r....
-000089d0: 7220 0000 0072 5c00 0000 7221 0000 0072  r ...r\...r!...r
-000089e0: 3c00 0000 721e 0000 0072 1f00 0000 7223  <...r....r....r#
-000089f0: 0000 0072 1c00 0000 7290 0000 00a9 095a  ...r....r......Z
-00008a00: 1066 696e 616c 7269 7670 6c79 5f69 6e66  .finalrivply_inf
-00008a10: 6f72 8f00 0000 7274 0000 005a 1141 6c6c  or....rt...Z.All
-00008a20: 436f 6e6e 6563 744c 616b 6549 4453 7228  ConnectLakeIDSr(
-00008a30: 0000 005a 066c 616b 6569 645a 0c4c 616b  ...Z.lakeidZ.Lak
-00008a40: 6573 7562 5f69 6e66 6f72 da00 0000 5a0a  esub_infor....Z.
-00008a50: 6c61 6b65 7375 6269 6473 722d 0000 0072  lakesubidsr-...r
-00008a60: 2d00 0000 722e 0000 00da 3b43 6861 6e67  -...r.....;Chang
-00008a70: 655f 4174 7472 6962 7574 655f 5661 6c75  e_Attribute_Valu
-00008a80: 6573 5f46 6f72 5f43 6174 6368 6d65 6e74  es_For_Catchment
-00008a90: 735f 436f 7665 7265 645f 4279 5f53 616d  s_Covered_By_Sam
-00008aa0: 655f 4c61 6b65 a109 0000 7334 0000 0000  e_Lake....s4....
-00008ab0: 0d04 010c 010e 0112 010a 010c 010a 0312  ................
-00008ac0: 0108 0112 0110 0108 0102 ff04 030a 010c  ................
-00008ad0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00008ae0: f908 0972 f200 0000 6303 0000 0000 0000  ...r....c.......
-00008af0: 0000 0000 0008 0000 0006 0000 0043 0000  .............C..
-00008b00: 0073 6800 0000 7400 7c00 7c01 8302 7d03  .sh...t.|.|...}.
-00008b10: 7c02 6401 6b04 7260 7400 7c00 7c02 8302  |.d.k.r`t.|.|...
-00008b20: 7d04 7401 7402 7c04 8301 8301 4400 5d30  }.t.t.|.....D.]0
-00008b30: 7d05 7c04 7c05 1900 7c02 6b02 723a 7128  }.|.|...|.k.r:q(
-00008b40: 7403 a004 7c03 7c04 7c05 1900 6b02 a101  t...|.|.|...k...
-00008b50: 7d06 7403 a005 7c03 7c06 a102 7d03 7128  }.t...|.|...}.q(
-00008b60: 7c03 7d07 6e04 7c03 7d07 7c07 5300 2902  |.}.n.|.}.|.S.).
-00008b70: 7a95 5265 7475 726e 2073 7562 6964 206f  z.Return subid o
-00008b80: 6620 7375 6262 6173 696e 7320 6265 7477  f subbasins betw
-00008b90: 6565 6e20 7477 6f20 7375 6269 6420 696e  een two subid in
-00008ba0: 2074 6865 2072 6f75 7469 6e67 206e 6574   the routing net
-00008bb0: 776f 726b 0a20 2020 202d 2d2d 2d2d 2d2d  work.    -------
-00008bc0: 2d2d 2d0a 0a20 2020 204e 6f74 6573 0a20  ---..    Notes. 
-00008bd0: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
-00008be0: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
-00008bf0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00008c00: 652c 0a20 2020 2072 0100 0000 2906 7285  e,.    r....).r.
-00008c10: 0000 0072 1e00 0000 721f 0000 0072 2100  ...r....r....r!.
-00008c20: 0000 72a6 0000 00da 0664 656c 6574 6529  ..r......delete)
-00008c30: 0872 5e00 0000 5a10 7375 6269 645f 646f  .r^...Z.subid_do
-00008c40: 776e 7374 7265 616d 5a0e 7375 6269 645f  wnstreamZ.subid_
-00008c50: 7570 7374 7265 616d da0c 4879 6472 6f42  upstream..HydroB
-00008c60: 6173 696e 7331 da0c 4879 6472 6f42 6173  asins1..HydroBas
-00008c70: 696e 7332 7228 0000 00da 0472 6f77 73da  ins2r(.....rows.
-00008c80: 0b48 7964 726f 4261 7369 6e73 722d 0000  .HydroBasinsr-..
-00008c90: 0072 2d00 0000 722e 0000 00da 3552 6574  .r-...r.....5Ret
-00008ca0: 7572 6e5f 5375 6249 6473 5f42 6574 7765  urn_SubIds_Betwe
-00008cb0: 656e 5f54 776f 5f53 7562 6261 7369 6e73  en_Two_Subbasins
-00008cc0: 5f49 6e5f 526f 7569 6e67 5f4e 6574 776f  _In_Rouing_Netwo
-00008cd0: 726b cc09 0000 731a 0000 0000 0e02 0104  rk....s.........
-00008ce0: ff04 0408 010a 0110 010c 0102 0112 010e  ................
-00008cf0: 0106 0204 0272 f800 0000 6306 0000 0000  .....r....c.....
-00008d00: 0000 0000 0000 0020 0000 0008 0000 0043  ....... .......C
-00008d10: 0000 0073 4404 0000 7c04 6401 6402 6702  ...sD...|.d.d.g.
-00008d20: 1900 a000 6403 a101 6a01 7d06 7402 a003  ....d...j.}.t...
-00008d30: 7c00 7c01 6602 a101 7d07 7c07 7c07 6400  |.|.f...}.|.|.d.
-00008d40: 6400 8502 6404 6602 1900 a004 a100 1900  d...d.f.........
-00008d50: 7d07 7402 a003 7c02 7c03 6602 a101 7d08  }.t...|.|.f...}.
-00008d60: 7c08 7c08 6400 6400 8502 6404 6602 1900  |.|.d.d...d.f...
-00008d70: a004 a100 1900 7d08 7402 6a05 7c07 7c08  ......}.t.j.|.|.
-00008d80: 6405 6406 8d03 7d07 7402 a006 7402 a007  d.d...}.t...t...
-00008d90: 7c07 6400 6400 8502 6405 6602 1900 a101  |.d.d...d.f.....
-00008da0: a101 7d09 7402 a006 7402 a007 7c07 6400  ..}.t...t...|.d.
-00008db0: 6400 8502 6407 6602 1900 a101 a101 7d0a  d...d.f.......}.
-00008dc0: 7402 a008 7409 7c07 8301 6405 6602 7402  t...t.|...d.f.t.
-00008dd0: 6a0a a102 7d0b 740b 6404 7409 7c09 8301  j...}.t.d.t.|...
-00008de0: 8302 4400 5d40 7d0c 7c09 7c0c 1900 7d0d  ..D.]@}.|.|...}.
-00008df0: 7c04 6a0c 7c04 6401 1900 7c0d 6b02 1900  |.j.|.d...|.k...
-00008e00: 6408 1900 6a01 6404 1900 7d0e 7c0e 7c0b  d...j.d...}.|.|.
-00008e10: 7c07 6400 6400 8502 6405 6602 1900 7c0d  |.d.d...d.f...|.
-00008e20: 6b02 3c00 71cc 7402 6a05 7c07 7c0b 6405  k.<.q.t.j.|.|.d.
-00008e30: 6406 8d03 7d07 6700 7d0f 6700 7d10 6700  d...}.g.}.g.}.g.
-00008e40: 7d11 740b 6404 7409 7c0a 8301 8302 4400  }.t.d.t.|.....D.
-00008e50: 9002 5de6 7d0c 7c0a 7c0c 1900 7d03 7c07  ..].}.|.|...}.|.
-00008e60: 7c07 6400 6400 8502 6407 6602 1900 7c03  |.d.d...d.f...|.
-00008e70: 6b02 1900 7d12 7c12 7c12 6400 6400 8502  k...}.|.|.d.d...
-00008e80: 6409 6602 1900 a004 a100 1900 7d12 7c12  d.f.........}.|.
-00008e90: 7409 7c12 8301 6405 1800 6405 6602 1900  t.|...d...d.f...
-00008ea0: 7d13 7c04 6a0c 7c04 6401 1900 a00d 7c12  }.|.j.|.d.....|.
-00008eb0: 6400 6400 8502 6405 6602 1900 a101 1900  d.d...d.f.......
-00008ec0: 7d14 7409 7c12 8301 6405 6b02 9002 720c  }.t.|...d.k...r.
-00008ed0: 7c12 640a 1900 7d15 7c05 6a0c 7c05 640b  |.d...}.|.j.|.d.
-00008ee0: 1900 7c15 6b02 1900 640c 1900 6a01 6404  ..|.k...d...j.d.
-00008ef0: 1900 7c03 6b03 9001 72f6 7c10 a005 740e  ..|.k...r.|...t.
-00008f00: 7c12 640a 1900 8301 a101 0100 6e12 7c0f  |.d.........n.|.
-00008f10: a005 740e 7c12 640d 1900 8301 a101 0100  ..t.|.d.........
-00008f20: 9001 7138 740f 7c06 7c13 8302 7d16 7402  ..q8t.|.|...}.t.
-00008f30: a006 7c12 6400 6400 8502 6405 6602 1900  ..|.d.d...d.f...
-00008f40: a101 7d17 740b 6404 7409 7c12 8301 8302  ..}.t.d.t.|.....
-00008f50: 4400 9001 5de0 7d18 7c12 7c18 6405 6602  D...].}.|.|.d.f.
-00008f60: 1900 7d15 7c15 7c13 6b03 9003 7266 7c11  ..}.|.|.k...rf|.
-00008f70: a005 740e 7c12 7c18 6405 6602 1900 8301  ..t.|.|.d.f.....
-00008f80: a101 0100 7409 7c04 6a0c 7c04 6401 1900  ....t.|.j.|.d...
-00008f90: 7c15 6b02 1900 8301 6404 6b04 9003 7266  |.k.....d.k...rf
-00008fa0: 7c04 6a0c 7c04 6401 1900 7c15 6b02 1900  |.j.|.d...|.k...
-00008fb0: 6402 1900 6a01 6404 1900 7d19 7c19 7c16  d...j.d...}.|.|.
-00008fc0: 7600 9003 7266 7c19 7c12 6400 6400 8502  v...rf|.|.d.d...
-00008fd0: 6405 6602 1900 7601 9003 7266 7c11 a005  d.f...v...rf|...
-00008fe0: 740e 7c19 8301 a101 0100 7c19 7d1a 6404  t.|.......|.}.d.
-00008ff0: 7d1b 7c1b 640e 6b00 9003 7266 7c1b 6405  }.|.d.k...rf|.d.
-00009000: 1700 7d1b 7409 7c04 6a0c 7c04 6401 1900  ..}.t.|.j.|.d...
-00009010: 7c1a 6b02 1900 8301 6404 6b04 9003 7266  |.k.....d.k...rf
-00009020: 7c04 6a0c 7c04 6401 1900 7c1a 6b02 1900  |.j.|.d...|.k...
-00009030: 6402 1900 6a01 6404 1900 7d1c 7c1c 7c12  d...j.d...}.|.|.
-00009040: 6400 6400 8502 6405 6602 1900 7601 9003  d.d...d.f...v...
-00009050: 7266 7c1c 7c16 7600 9003 7266 7c11 a005  rf|.|.v...rf|...
-00009060: 740e 7c1c 8301 a101 0100 7c1c 7d1a 6e04  t.|.......|.}.n.
-00009070: 9003 7166 6e04 9003 7166 9002 71da 740f  ..qfn...qf..q.t.
-00009080: 7c06 7c15 8302 7d1d 7409 7c1d 8301 6404  |.|...}.t.|...d.
-00009090: 6b04 9003 72a4 7402 a00d 7c1d 7c17 a102  k...r.t...|.|...
-000090a0: 7d1e 7410 7c1e 8301 640f 6b05 9003 729e  }.t.|...d.k...r.
-000090b0: 6410 7d1f 6e04 6411 7d1f 6e04 6411 7d1f  d.}.n.d.}.n.d.}.
-000090c0: 7409 7c14 6a0c 7c14 6402 1900 7c15 6b02  t.|.j.|.d...|.k.
-000090d0: 1900 8301 6404 6b04 9003 73ec 7c05 6a0c  ....d.k...s.|.j.
-000090e0: 7c05 640b 1900 7c15 6b02 1900 640c 1900  |.d...|.k...d...
-000090f0: 6a01 6404 1900 7c03 6b02 9003 73ec 7c1f  j.d...|.k...s.|.
-00009100: 9004 7204 7c0f a005 740e 7c12 7c18 6404  ..r.|...t.|.|.d.
-00009110: 6602 1900 8301 a101 0100 6e16 7c10 a005  f.........n.|...
-00009120: 740e 7c12 7c18 6405 6602 1900 8301 a101  t.|.|.d.f.......
-00009130: 0100 9002 713a 9001 7138 7411 7412 7c11  ....q:..q8t.t.|.
-00009140: 8301 8301 7411 7412 7c0f 8301 8301 7411  ....t.t.|.....t.
-00009150: 7412 7c10 8301 8301 6603 5300 2912 4e72  t.|.....f.S.).Nr
-00009160: 0600 0000 7249 0000 0072 a300 0000 7201  ....rI...r....r.
-00009170: 0000 0072 4f00 0000 72e1 0000 0072 d100  ...rO...r....r..
-00009180: 0000 da0a 4d61 7841 6363 5f63 6174 e904  ....MaxAcc_cat..
-00009190: 0000 0029 0272 0100 0000 724f 0000 005a  ...).r....rO...Z
-000091a0: 0849 4c5f 5375 6249 645a 0873 6c5f 636c  .IL_SubIdZ.sl_cl
-000091b0: 5f69 6429 0272 0100 0000 7201 0000 0072  _id).r....r....r
-000091c0: 6200 0000 724c 0000 0054 4629 1372 5c00  b...rL...TF).r\.
-000091d0: 0000 7220 0000 0072 2100 0000 da0c 636f  ..r ...r!.....co
-000091e0: 6c75 6d6e 5f73 7461 636b da07 6172 6773  lumn_stack..args
-000091f0: 6f72 7472 3100 0000 723c 0000 0072 e300  ortr1...r<...r..
-00009200: 0000 7264 0000 0072 1f00 0000 72bf 0000  ..rd...r....r...
-00009210: 0072 1e00 0000 7223 0000 0072 3d00 0000  .r....r#...r=...
-00009220: 72a3 0000 0072 8500 0000 7219 0000 0072  r....r....r....r
-00009230: 3700 0000 72b7 0000 0029 205a 0b72 6976  7...r....) Z.riv
-00009240: 5f6c 616b 655f 6964 5a06 7374 725f 6964  _lake_idZ.str_id
-00009250: 5a0c 7269 765f 6c61 6b65 5f69 6432 5a05  Z.riv_lake_id2Z.
-00009260: 636c 5f69 6472 5e00 0000 5a13 7374 725f  cl_idr^...Z.str_
-00009270: 7374 6172 745f 7074 5f6c 616b 6569 645a  start_pt_lakeidZ
-00009280: 1172 6f75 7469 6e67 5f69 6e66 6f5f 726f  .routing_info_ro
-00009290: 7574 5a08 7269 765f 6c61 6b65 5a0b 7269  utZ.riv_lakeZ.ri
-000092a0: 765f 6c61 6b65 5f63 6c5a 0d73 7472 5f69  v_lake_clZ.str_i
-000092b0: 645f 756e 6971 7565 5a0c 636c 5f69 645f  d_uniqueZ.cl_id_
-000092c0: 756e 6971 7565 5a0a 6163 635f 7374 725f  uniqueZ.acc_str_
-000092d0: 636c 7228 0000 00da 0573 7472 6964 da06  clr(.....strid..
-000092e0: 6d61 7861 6363 5a14 6e6f 6e5f 6c61 6b65  maxaccZ.non_lake
-000092f0: 5f69 6e66 6c6f 775f 7365 6773 5a12 7374  _inflow_segsZ.st
-00009300: 725f 6964 5f6c 616b 655f 696e 6c66 6f77  r_id_lake_inlfow
-00009310: 5a13 7374 725f 6964 5f77 6974 6869 6e5f  Z.str_id_within_
-00009320: 6c61 6b65 735a 0b72 6976 5f6c 616b 655f  lakesZ.riv_lake_
-00009330: 696c 5a0a 6f75 746c 6574 5f73 7472 5a10  ilZ.outlet_strZ.
-00009340: 7375 625f 726f 7574 696e 675f 696e 666f  sub_routing_info
-00009350: 5a0b 7374 725f 6964 5f63 6c5f 6a5a 1373  Z.str_id_cl_jZ.s
-00009360: 7472 735f 746f 5f6c 616b 655f 6f75 746c  trs_to_lake_outl
-00009370: 6574 5a18 756e 6971 7565 5f73 7472 5f69  etZ.unique_str_i
-00009380: 645f 6376 5f62 795f 6c61 6b65 7244 0000  d_cv_by_lakerD..
-00009390: 005a 1a64 6f77 6e5f 7375 6e5f 6f66 5f6c  .Z.down_sun_of_l
-000093a0: 616b 655f 636f 7665 725f 7374 725a 0663  ake_cover_strZ.c
-000093b0: 7374 7269 645a 036b 5f64 5a07 6473 7472  stridZ.k_dZ.dstr
-000093c0: 5f69 645a 0b75 705f 7374 725f 636c 5f6a  _idZ.up_str_cl_j
-000093d0: 722c 0000 005a 1168 6173 5f75 705f 7374  r,...Z.has_up_st
-000093e0: 725f 696e 6c61 6b65 722d 0000 0072 2d00  r_inlaker-...r-.
-000093f0: 0000 722e 0000 00da 3172 6574 7572 6e5f  ..r.....1return_
-00009400: 6e6f 6e5f 6c61 6b65 5f69 6e66 6c6f 775f  non_lake_inflow_
-00009410: 7365 6773 5f61 6e64 5f73 6567 735f 7769  segs_and_segs_wi
-00009420: 7468 696e 5f6c 616b 6573 ec09 0000 73ae  thin_lakes....s.
-00009430: 0000 0000 0414 020e 0118 010e 0118 0110  ................
-00009440: 031c 011c 0216 0112 0108 0116 0102 ff04  ................
-00009450: 031a 0110 0504 0104 0104 0114 0208 0218  ................
-00009460: 0118 0114 0104 0118 ff04 050e 0108 0310  ................
-00009470: 0102 ff04 0202 fe02 0302 fd02 ff04 0614  ................
-00009480: 0212 0104 020a 0716 0214 010c 030a 0116  ................
-00009490: 021c 021c 0320 030e 0204 0104 010a 0108  ..... ..........
-000094a0: 011c 011c 0220 010e 0106 0206 0208 030a  ..... ..........
-000094b0: 020e 040c 010e 0106 0206 0204 0314 0102  ................
-000094c0: ff02 ff04 0304 010a ff02 0202 fe04 0202  ................
-000094d0: fe02 0302 fd02 fd04 0702 f904 0b18 021e  ................
-000094e0: 0272 ff00 0000 6303 0000 0000 0000 0000  .r....c.........
-000094f0: 0000 0015 0000 0006 0000 0043 0000 0073  ...........C...s
-00009500: d801 0000 6700 7d03 6700 7d04 7400 a001  ....g.}.g.}.t...
-00009510: 7c00 7c01 6602 a101 7d05 7400 a002 7400  |.|.f...}.t...t.
-00009520: a003 7c01 a101 a101 7d06 7400 a002 7400  ..|.....}.t...t.
-00009530: a003 7c00 a101 a101 7d07 7400 a004 7405  ..|.....}.t...t.
-00009540: 7c05 8301 6401 6602 7400 6a06 a102 7d08  |...d.f.t.j...}.
-00009550: 7407 6402 7405 7c06 8301 8302 4400 5d40  t.d.t.|.....D.]@
-00009560: 7d09 7c06 7c09 1900 7d0a 7c02 6a08 7c02  }.|.|...}.|.j.|.
-00009570: 6403 1900 7c0a 6b02 1900 6404 1900 6a09  d...|.k...d...j.
-00009580: 6402 1900 7d0b 7c0b 7c08 7c05 6400 6400  d...}.|.|.|.d.d.
-00009590: 8502 6401 6602 1900 7c0a 6b02 3c00 715a  ..d.f...|.k.<.qZ
-000095a0: 7400 6a0a 7c05 7c08 6401 6405 8d03 7d05  t.j.|.|.d.d...}.
-000095b0: 7c05 7c05 6400 6400 8502 6406 6602 1900  |.|.d.d...d.f...
-000095c0: a00b a100 1900 7d05 7c02 6403 6407 6702  ......}.|.d.d.g.
-000095d0: 1900 a00c 6408 a101 6a09 7d0c 7407 6402  ....d...j.}.t.d.
-000095e0: 7405 7c07 8301 8302 4400 5de8 7d09 7c07  t.|.....D.].}.|.
-000095f0: 7c09 1900 7d0d 7c05 7c05 6400 6400 8502  |...}.|.|.d.d...
-00009600: 6402 6602 1900 7c0d 6b02 1900 7d0e 7405  d.f...|.k...}.t.
-00009610: 7c0e 8301 6401 6b01 9001 721a 71e6 7c0e  |...d.k...r.q.|.
-00009620: 7405 7c0e 8301 6401 1800 6401 6602 1900  t.|...d...d.f...
-00009630: 7d0f 740d 7c0c 7c0f 8302 7d10 7400 a00e  }.t.|.|...}.t...
-00009640: 7c0e 6400 6400 8502 6401 6602 1900 7c10  |.d.d...d.f...|.
-00009650: a102 7d11 6700 7d12 7405 7c11 7c11 6409  ..}.g.}.t.|.|.d.
-00009660: 6b02 1900 8301 7405 7c0e 6400 6400 8502  k.....t.|.d.d...
-00009670: 6401 6602 1900 8301 6b00 72e6 7c0e 7400  d.f.....k.r.|.t.
-00009680: a00f 7c11 a101 6401 6602 1900 7d13 7407  ..|...d.f...}.t.
-00009690: 6402 7405 7c13 8301 8302 4400 5d22 7d14  d.t.|.....D.]"}.
-000096a0: 7c13 7c14 1900 7d0a 7c0a 7c0f 6b03 9001  |.|...}.|.|.k...
-000096b0: 7298 7c12 a00a 7c0a a101 0100 9001 7198  r.|...|.......q.
-000096c0: 7c04 7c12 1700 7d04 7c03 a00a 7c0d a101  |.|...}.|...|...
-000096d0: 0100 71e6 7c03 7c04 6602 5300 290a 4e72  ..q.|.|.f.S.).Nr
-000096e0: 4f00 0000 7201 0000 0072 0600 0000 72f9  O...r....r....r.
-000096f0: 0000 0072 e100 0000 724c 0000 0072 4900  ...r....rL...rI.
-00009700: 0000 72a3 0000 0054 2910 7221 0000 0072  ..r....T).r!...r
-00009710: fb00 0000 723c 0000 0072 e300 0000 7264  ....r<...r....rd
-00009720: 0000 0072 1f00 0000 72bf 0000 0072 1e00  ...r....r....r..
-00009730: 0000 7223 0000 0072 2000 0000 7231 0000  ..r#...r ...r1..
-00009740: 0072 fc00 0000 725c 0000 0072 8500 0000  .r....r\...r....
-00009750: 723d 0000 0072 8700 0000 2915 5a05 434c  r=...r....).Z.CL
-00009760: 5f49 645a 0653 7472 5f49 645a 0c52 6f75  _IdZ.Str_IdZ.Rou
-00009770: 7469 6e67 5f69 6e66 6f5a 174c 616b 6573  ting_infoZ.Lakes
-00009780: 5f57 4974 685f 4d75 6c74 695f 4f75 746c  _WIth_Multi_Outl
-00009790: 6574 5a0a 5265 6d6f 7665 5f53 7472 5a06  etZ.Remove_StrZ.
-000097a0: 434c 5f53 7472 5a0d 5374 725f 4964 5f75  CL_StrZ.Str_Id_u
-000097b0: 6e69 7175 655a 0c43 4c5f 4964 5f75 6e69  niqueZ.CL_Id_uni
-000097c0: 7175 655a 0a41 6363 5f53 7472 5f43 4c72  queZ.Acc_Str_CLr
-000097d0: 2800 0000 72fd 0000 0072 fe00 0000 5a11  (...r....r....Z.
-000097e0: 726f 7574 696e 675f 696e 666f 5f6f 6e6c  routing_info_onl
-000097f0: 795a 076c 616b 655f 6964 5a08 695f 434c  yZ.lake_idZ.i_CL
-00009800: 5f53 7472 5a0b 7374 725f 6d61 785f 6163  _StrZ.str_max_ac
-00009810: 635a 1273 7472 5f74 6f5f 7374 725f 6d61  cZ.str_to_str_ma
-00009820: 785f 6163 6372 2c00 0000 5a0c 5265 6d6f  x_accr,...Z.Remo
-00009830: 7665 5f53 7472 5f69 5a18 7374 725f 6e6f  ve_Str_iZ.str_no
-00009840: 7466 6c6f 7774 6f5f 6c61 6b65 6f75 746c  tflowto_lakeoutl
-00009850: 6574 5a04 6973 7472 722d 0000 0072 2d00  etZ.istrr-...r-.
-00009860: 0000 722e 0000 00da 1f43 6865 636b 5f49  ..r......Check_I
-00009870: 665f 4c61 6b65 5f48 6176 655f 4d75 6c74  f_Lake_Have_Mult
-00009880: 695f 4f75 744c 6574 6f0a 0000 7342 0000  i_OutLeto...sB..
-00009890: 0000 0304 0104 020e 0210 0210 0316 0112  ................
-000098a0: 0108 0116 0102 ff04 031a 0110 0318 0314  ................
-000098b0: 0312 0208 0218 030e 0102 0814 030a 0818  ................
-000098c0: 0404 0324 0212 0212 0208 050a 010e 0508  ...$............
-000098d0: 010c 0272 0001 0000 6301 0000 0000 0000  ...r....c.......
-000098e0: 0000 0000 0009 0000 000a 0000 0043 0000  .............C..
-000098f0: 0073 ba00 0000 6401 7d01 7c00 6a00 6402  .s....d.}.|.j.d.
-00009900: 6403 8d01 7d02 7c02 6401 1900 6a01 7c02  d...}.|.d...j.|.
-00009910: 6404 3c00 7c00 6405 1900 6a01 7d03 7c03  d.<.|.d...j.}.|.
-00009920: 7c03 6406 6b04 1900 7d03 7402 a003 7c03  |.d.k...}.t...|.
-00009930: a101 7d03 7404 6406 7405 7c03 8301 8302  ..}.t.d.t.|.....
-00009940: 4400 5d68 7d04 7c03 7c04 1900 7d05 7c00  D.]h}.|.|...}.|.
-00009950: 6a06 7c00 6405 1900 7c05 6b02 1900 7d06  j.|.d...|.k...}.
-00009960: 7c06 6a07 6407 6701 6408 6409 8d02 7d06  |.j.d.g.d.d...}.
-00009970: 7c06 7c01 1900 6a01 6406 1900 7d07 7c06  |.|...j.d...}.|.
-00009980: 7c01 1900 6a01 7d08 7405 7c08 8301 640a  |...j.}.t.|...d.
-00009990: 6b04 724c 7408 7c07 7c00 7c02 640a 7c08  k.rLt.|.|.|.d.|.
-000099a0: 7c00 640a 640b 8d07 7d02 714c 7c02 5300  |.d.d...}.qL|.S.
-000099b0: 290c 72f0 0000 0072 0600 0000 5472 0800  ).r....r....Tr..
-000099c0: 0000 726c 0000 0072 6d00 0000 7201 0000  ..rl...rm...r...
-000099d0: 0072 6000 0000 4672 6100 0000 724f 0000  .r`...Fra...rO..
-000099e0: 0072 ee00 0000 2909 7216 0000 0072 2000  .r....).r....r .
-000099f0: 0000 7221 0000 0072 3c00 0000 721e 0000  ..r!...r<...r...
-00009a00: 0072 1f00 0000 7223 0000 0072 1c00 0000  .r....r#...r....
-00009a10: 7290 0000 0072 f100 0000 722d 0000 0072  r....r....r-...r
-00009a20: 2d00 0000 722e 0000 00da 3b63 6861 6e67  -...r.....;chang
-00009a30: 655f 6174 7472 6962 7574 655f 7661 6c75  e_attribute_valu
-00009a40: 6573 5f66 6f72 5f63 6174 6368 6d65 6e74  es_for_catchment
-00009a50: 735f 636f 7665 7265 645f 6279 5f73 616d  s_covered_by_sam
-00009a60: 655f 6c61 6b65 c50a 0000 7332 0000 0000  e_lake....s2....
-00009a70: 0d04 010c 010e 010a 010c 010a 0312 0108  ................
-00009a80: 0112 0110 0108 0102 ff04 030a 010c 0102  ................
-00009a90: 0102 0102 0102 0102 0102 0102 0102 f908  ................
-00009aa0: 0972 0101 0000 6303 0000 0000 0000 0000  .r....c.........
-00009ab0: 0000 000d 0000 0005 0000 0043 0000 0073  ...........C...s
-00009ac0: a802 0000 7c00 6a00 7d03 7c02 6401 6b04  ....|.j.}.|.d.k.
-00009ad0: 9001 72dc 7401 6401 7402 7c03 8301 8302  ..r.t.d.t.|.....
-00009ae0: 4400 5ddc 7d04 7c00 6a03 7c03 7c04 1900  D.].}.|.j.|.|...
-00009af0: 6402 6602 1900 7d05 7c00 6a03 7c03 7c04  d.f...}.|.j.|.|.
-00009b00: 1900 6403 6602 1900 7d06 7c00 6a03 7c03  ..d.f...}.|.j.|.
-00009b10: 7c04 1900 6404 6602 1900 7d07 7c00 6a03  |...d.f...}.|.j.
-00009b20: 7c00 6403 1900 7c07 6b02 1900 a004 a100  |.d...|.k.......
-00009b30: 7d08 7402 7c08 8301 6401 6b04 7298 7c08  }.t.|...d.k.r.|.
-00009b40: 6402 1900 6a05 6401 1900 7c00 6a03 7c03  d...j.d...|.j.|.
-00009b50: 7c04 1900 6405 6602 3c00 6e12 6406 7c00  |...d.f.<.n.d.|.
-00009b60: 6a03 7c03 7c04 1900 6405 6602 3c00 7c05  j.|.|...d.f.<.|.
-00009b70: 7c00 6a03 7c03 7c04 1900 6405 6602 1900  |.j.|.|...d.f...
-00009b80: 6b02 72d2 6406 7c00 6a03 7c03 7c04 1900  k.r.d.|.j.|.|...
-00009b90: 6405 6602 3c00 7c05 7c00 6a03 7c03 7c04  d.f.<.|.|.j.|.|.
-00009ba0: 1900 6405 6602 1900 6b02 721e 6406 7c00  ..d.f...k.r.d.|.
-00009bb0: 6a03 7c03 7c04 1900 6405 6602 3c00 711e  j.|.|...d.f.<.q.
-00009bc0: 7c00 6403 1900 6a05 7c00 6407 3c00 7c00  |.d...j.|.d.<.|.
-00009bd0: 6404 1900 6a05 7c00 6408 3c00 7c00 6402  d...j.|.d.<.|.d.
-00009be0: 1900 6a05 7c00 6403 3c00 7c00 6405 1900  ..j.|.d.<.|.d...
-00009bf0: 6a05 7c00 6404 3c00 7c00 7c00 6409 1900  j.|.d.<.|.|.d...
-00009c00: 640a 6b03 1900 6a04 640b 640c 8d01 7d09  d.k...j.d.d...}.
-00009c10: 7c00 6403 1900 a006 7c09 6404 1900 a101  |.d.....|.d.....
-00009c20: 0f00 7d0a 640d 7c00 6a07 7600 9001 7288  ..}.d.|.j.v...r.
-00009c30: 640e 7c00 6a03 7c0a 640d 6602 3c00 640e  d.|.j.|.d.f.<.d.
-00009c40: 7c00 6a03 7c0a 640f 6602 3c00 640e 7c00  |.j.|.d.f.<.d.|.
-00009c50: 6a03 7c0a 6410 6602 3c00 640e 7c00 6a03  j.|.d.f.<.d.|.j.
-00009c60: 7c0a 6411 6602 3c00 640e 7c00 6a03 7c0a  |.d.f.<.d.|.j.|.
-00009c70: 6412 6602 3c00 640e 7c00 6a03 7c0a 6413  d.f.<.d.|.j.|.d.
-00009c80: 6602 3c00 640e 7c00 6a03 7c0a 6414 6602  f.<.d.|.j.|.d.f.
-00009c90: 3c00 640e 7c00 6a03 7c0a 6415 6602 3c00  <.d.|.j.|.d.f.<.
-00009ca0: 7c01 6401 6b00 9001 72ea 7c00 5300 7c00  |.d.k...r.|.S.|.
-00009cb0: 6a08 6403 6416 6417 8d02 7d0b 7409 7c0b  j.d.d.d...}.t.|.
-00009cc0: 8301 7d0b 7401 6401 7402 7c0b 8301 8302  ..}.t.d.t.|.....
-00009cd0: 4400 5d94 7d04 7c0b 6403 1900 6a05 7c04  D.].}.|.d...j.|.
-00009ce0: 1900 7d0c 7c0b 6418 1900 6a05 7c04 1900  ..}.|.d...j.|...
-00009cf0: 7c00 6a03 7c00 6403 1900 7c0c 6b02 6418  |.j.|.d...|.k.d.
-00009d00: 6602 3c00 7c0b 6419 1900 6a05 7c04 1900  f.<.|.d...j.|...
-00009d10: 7c00 6a03 7c00 6403 1900 7c0c 6b02 6419  |.j.|.d...|.k.d.
-00009d20: 6602 3c00 7c0b 641a 1900 6a05 7c04 1900  f.<.|.d...j.|...
-00009d30: 7c00 6a03 7c00 6403 1900 7c0c 6b02 641a  |.j.|.d...|.k.d.
-00009d40: 6602 3c00 7c0b 641b 1900 6a05 7c04 1900  f.<.|.d...j.|...
-00009d50: 7c00 6a03 7c00 6403 1900 7c0c 6b02 641b  |.j.|.d...|.k.d.
-00009d60: 6602 3c00 9002 710e 7c00 5300 291c 7294  f.<...q.|.S.).r.
-00009d70: 0000 0072 0100 0000 726c 0000 0072 0600  ...r....rl...r..
-00009d80: 0000 7249 0000 0072 6e00 0000 7250 0000  ..rI...rn...rP..
-00009d90: 0072 6f00 0000 7270 0000 0072 4b00 0000  .ro...rp...rK...
-00009da0: 724c 0000 0054 7208 0000 0072 5700 0000  rL...Tr....rW...
-00009db0: 7251 0000 0072 5800 0000 724e 0000 0072  rQ...rX...rN...r
-00009dc0: 5200 0000 7256 0000 0072 5300 0000 7255  R...rV...rS...rU
-00009dd0: 0000 0072 5400 0000 7213 0000 0072 9500  ...rT...r....r..
-00009de0: 0000 7259 0000 0072 5a00 0000 725b 0000  ..rY...rZ...r[..
-00009df0: 0072 6000 0000 290a 723e 0000 0072 1e00  .r`...).r>...r..
-00009e00: 0000 721f 0000 0072 2300 0000 7216 0000  ..r....r#...r...
-00009e10: 0072 2000 0000 723d 0000 0072 0b00 0000  .r ...r=...r....
-00009e20: 721d 0000 005a 1a53 7472 6561 6d6f 7264  r....Z.Streamord
-00009e30: 6572 616e 6464 7261 696e 6167 6561 7265  eranddrainageare
-00009e40: 6129 0d72 7400 0000 7297 0000 0072 9800  a).rt...r....r..
-00009e50: 0000 7245 0000 0072 2800 0000 726c 0000  ..rE...r(...rl..
-00009e60: 0072 2900 0000 7299 0000 0072 9a00 0000  .r)...r....r....
-00009e70: da19 7269 765f 7064 5f6e 6e63 6c73 5f72  ..riv_pd_nncls_r
-00009e80: 6f75 7469 6e67 5f69 6e66 6f72 2c00 0000  outing_infor,...
-00009e90: 729b 0000 0072 9c00 0000 722d 0000 0072  r....r....r-...r
-00009ea0: 2d00 0000 722e 0000 00da 0f75 7064 6174  -...r......updat
-00009eb0: 655f 746f 706f 6c6f 6779 ef0a 0000 7374  e_topology....st
-00009ec0: 0000 0000 0d06 020a 0112 0112 0112 0112  ................
-00009ed0: 0204 010a ff08 040c 0102 0102 ff04 0202  ................
-00009ee0: fe14 0412 0216 0112 0216 0114 020e 010e  ................
-00009ef0: 010e 020e 0318 0114 020c 010e 010e 010e  ................
-00009f00: 010e 010e 010e 010e 010e 030a 0104 020e  ................
-00009f10: 0208 0212 010e 030c fe04 010e ff02 050c  ................
-00009f20: fe04 010e ff02 050c fe04 010e ff02 050c  ................
-00009f30: fe04 010e ff06 0472 0301 0000 6303 0000  .......r....c...
-00009f40: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00009f50: 0043 0000 0073 0c00 0000 7c01 7c00 7c02  .C...s....|.|.|.
-00009f60: 1300 1400 5300 2901 4e72 2d00 0000 2903  ....S.).Nr-...).
-00009f70: da01 4172 4700 0000 72b8 0000 0072 2d00  ..ArG...r....r-.
-00009f80: 0000 722d 0000 0072 2e00 0000 da09 6675  ..r-...r......fu
-00009f90: 6e63 5f51 5f44 4143 0b00 0073 0200 0000  nc_Q_DAC...s....
-00009fa0: 0001 7205 0100 0063 0100 0000 0000 0000  ..r....c........
-00009fb0: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
-00009fc0: 7364 0000 007a 2c74 0074 017c 0064 0064  sd...z,t.t.|.d.d
-00009fd0: 0085 0264 0166 0219 007c 0064 0064 0085  ...d.f...|.d.d..
-00009fe0: 0264 0266 0219 0083 035c 027d 017d 0257  .d.f.....\.}.}.W
-00009ff0: 006e 2604 0074 0279 5201 0001 0001 0074  .n&..t.yR......t
-0000a000: 0364 0383 0101 0074 04a0 0564 0464 05a1  .d.....t...d.d..
-0000a010: 027d 0159 006e 0230 007c 0164 0119 007c  .}.Y.n.0.|.d...|
-0000a020: 0164 0219 0066 0253 0029 064e 7201 0000  .d...f.S.).Nr...
-0000a030: 0072 4f00 0000 7a37 2323 2323 2323 2323  .rO...z7########
-0000a040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a050: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a060: 2323 2323 2323 2323 2323 2323 2323 2372  ###############r
-0000a070: 4c00 0000 7250 0000 0029 0672 0200 0000  L...rP...).r....
-0000a080: 7205 0100 00da 0c52 756e 7469 6d65 4572  r......RuntimeEr
-0000a090: 726f 7272 7300 0000 7221 0000 0072 6400  rorrs...r!...rd.
-0000a0a0: 0000 2903 5a04 6461 5f71 5a05 706f 7074  ..).Z.da_qZ.popt
-0000a0b0: 325a 0570 636f 7632 722d 0000 0072 2d00  2Z.pcov2r-...r-.
-0000a0c0: 0000 722e 0000 00da 2372 6574 7572 6e5f  ..r.....#return_
-0000a0d0: 6b5f 616e 645f 635f 696e 5f71 5f64 615f  k_and_c_in_q_da_
-0000a0e0: 7265 6c61 7469 6f6e 7368 6970 470b 0000  relationshipG...
-0000a0f0: 730c 0000 0000 0202 012c 010c 0108 0112  s........,......
-0000a100: 0272 0701 0000 6304 0000 0000 0000 0000  .r....c.........
-0000a110: 0000 000d 0000 0005 0000 0043 0000 0073  ...........C...s
-0000a120: c200 0000 6401 7d04 7c04 7c01 1400 7d05  ....d.}.|.|...}.
-0000a130: 6402 7d06 7c00 6401 7c05 1400 1800 7d07  d.}.|.d.|.....}.
-0000a140: 7c07 6403 6b00 7244 6404 7c00 1400 7d07  |.d.k.rDd.|...}.
-0000a150: 6405 7c00 1400 7d05 7c00 7c07 1800 6401  d.|...}.|.|...d.
-0000a160: 1b00 7c01 1b00 7d04 7c07 7c01 1400 6401  ..|...}.|.|...d.
-0000a170: 7c04 1400 7c01 1400 7c01 1400 6401 1b00  |...|...|...d...
-0000a180: 1700 7d08 7c07 6401 7c01 1400 6406 7c04  ..}.|.d.|...d.|.
-0000a190: 6401 1300 1700 6404 1300 1400 1700 7d09  d.....d.......}.
-0000a1a0: 7400 7c08 8301 7400 7c09 8301 1b00 7d0a  t.|...t.|.....}.
-0000a1b0: 7400 7c02 8301 7400 7c08 8301 1b00 7d0b  t.|...t.|.....}.
-0000a1c0: 7c0b 6403 6b04 72ba 7c0a 6407 1300 7c03  |.d.k.r.|.d...|.
-0000a1d0: 6404 1300 1400 7c0b 1b00 7d0c 6e04 6408  d.....|...}.n.d.
-0000a1e0: 7d0c 7c0c 5300 2909 4e72 4c00 0000 7a0a  }.|.S.).NrL...z.
-0000a1f0: 2020 2020 2020 2020 2020 7201 0000 0072            r....r
-0000a200: 9e00 0000 6700 0000 0000 00d0 3f72 4f00  ....g.......?rO.
-0000a210: 0000 6755 5555 5555 55e5 3f72 5100 0000  ..gUUUUUU.?rQ...
-0000a220: 2901 724a 0000 0029 0dda 0577 6964 7468  ).rJ...)...width
-0000a230: da05 6465 7074 68da 0151 5a05 736c 6f70  ..depth..QZ.slop
-0000a240: 655a 037a 6368 5a05 7369 6477 64da 0374  eZ.zchZ.sidwd..t
-0000a250: 6162 5a05 626f 7477 645a 0341 6368 5a03  abZ.botwdZ.AchZ.
-0000a260: 5063 685a 0352 6368 da01 56da 016e 722d  PchZ.Rch..V..nr-
-0000a270: 0000 0072 2d00 0000 722e 0000 00da 1163  ...r-...r......c
-0000a280: 616c 6375 6c61 7465 4368 616e 6e61 6c6e  alculateChannaln
-0000a290: 520b 0000 7320 0000 0000 0104 0108 0104  R...s ..........
-0000a2a0: 010c 0108 0108 0108 0110 011c 071c 0110  ................
-0000a2b0: 0110 0108 0116 0204 0172 0e01 0000 fa01  .........r......
-0000a2c0: 2363 0300 0000 0000 0000 0000 0000 1000  #c..............
-0000a2d0: 0000 0700 0000 4300 0000 73c8 0100 007c  ......C...s....|
-0000a2e0: 0164 016b 0072 0c7c 0053 007c 0064 0264  .d.k.r.|.S.|.d.d
-0000a2f0: 0367 0219 00a0 0064 04a1 016a 017d 0364  .g.....d...j.}.d
-0000a300: 057d 0464 057c 006a 0276 0172 3264 067d  .}.d.|.j.v.r2d.}
-0000a310: 047c 0264 076b 0390 0172 6474 037c 0283  .|.d.k...rdt.|..
-0000a320: 0164 0819 006a 017d 0574 04a0 057c 05a1  .d...j.}.t...|..
-0000a330: 017d 067c 067c 0664 016b 0419 007d 067c  .}.|.|.d.k...}.|
-0000a340: 006a 067c 007c 0419 00a0 077c 06a1 0119  .j.|.|.....|....
-0000a350: 007d 0764 097d 087c 0164 016b 0072 8c74  .}.d.}.|.d.k.r.t
-0000a360: 0864 0a83 0101 007c 0053 007c 006a 067c  .d.....|.S.|.j.|
-0000a370: 007c 0419 007c 016b 0219 007d 0974 097c  .|...|.k...}.t.|
-0000a380: 0983 0164 016b 0472 ba7c 0964 0219 006a  ...d.k.r.|.d...j
-0000a390: 0164 0119 007d 086e 0e74 0864 0b7c 0983  .d...}.n.t.d.|..
-0000a3a0: 0201 007c 0053 0074 0a7c 037c 0883 027d  ...|.S.t.|.|...}
-0000a3b0: 0a74 097c 0783 0164 0c6b 0590 0172 4874  .t.|...d.k...rHt
-0000a3c0: 0b64 0174 097c 0783 0183 0244 005d 587d  .d.t.|.....D.]X}
-0000a3d0: 0b7c 0764 0219 006a 017c 0b19 007d 0c7c  .|.d...j.|...}.|
-0000a3e0: 0c7c 086b 0273 ee74 04a0 0c74 04a0 0d7c  .|.k.s.t...t...|
-0000a3f0: 0a7c 0ca1 02a1 0164 0d6b 0090 0172 2271  .|.....d.k...r"q
-0000a400: ee74 0a7c 037c 0c83 027d 0d74 04a0 0d7c  .t.|.|...}.t...|
-0000a410: 0a7c 0da1 027d 0e7c 0a74 04a0 0e7c 0ea1  .|...}.|.t...|..
-0000a420: 0119 007d 0a71 ee7c 0a7d 0f7c 006a 067c  ...}.q.|.}.|.j.|
-0000a430: 0064 0219 00a0 077c 0fa1 0119 007d 007c  .d.....|.....}.|
-0000a440: 0053 0064 097d 087c 006a 067c 007c 0419  .S.d.}.|.j.|.|..
-0000a450: 007c 016b 0219 007d 0974 097c 0983 0164  .|.k...}.t.|...d
-0000a460: 016b 0490 0172 a27c 0964 0219 006a 0164  .k...r.|.d...j.d
-0000a470: 0119 007d 0874 0a7c 037c 0883 027d 0f6e  ...}.t.|.|...}.n
-0000a480: 0a7c 0064 0219 006a 017d 0f7c 006a 067c  .|.d...j.}.|.j.|
-0000a490: 0064 0219 00a0 077c 0fa1 0119 007d 007c  .d.....|.....}.|
-0000a4a0: 0053 0064 0053 0029 0e4e 7201 0000 0072  .S.d.S.).Nr....r
-0000a4b0: 0600 0000 7249 0000 0072 4a00 0000 726a  ....rI...rJ...rj
-0000a4c0: 0000 0072 6b00 0000 720f 0100 005a 0972  ...rk...r....Z.r
-0000a4d0: 6567 5f73 7562 6964 7250 0000 007a 4154  eg_subidrP...zAT
-0000a4e0: 6f20 7573 6520 7375 6272 6567 696f 6e2c  o use subregion,
-0000a4f0: 2074 6865 2053 7562 7265 6769 6f6e 2049   the Subregion I
-0000a500: 6420 4d55 5354 2070 726f 7669 6465 6420  d MUST provided 
-0000a510: 6173 204f 7574 6c65 745f 4f62 735f 4944  as Outlet_Obs_ID
-0000a520: 7a28 4e6f 204f 7574 6c65 7420 6964 2069  z(No Outlet id i
-0000a530: 7320 666f 756e 6465 6420 666f 7220 7375  s founded for su
-0000a540: 6272 6567 696f 6e20 2020 724c 0000 0072  bregion   rL...r
-0000a550: 4f00 0000 290f 725c 0000 0072 2000 0000  O...).r\...r ...
-0000a560: 720b 0000 005a 1044 6266 5f54 6f5f 4461  r....Z.Dbf_To_Da
-0000a570: 7461 6672 616d 6572 2100 0000 723c 0000  taframer!...r<..
-0000a580: 0072 2300 0000 723d 0000 0072 7300 0000  .r#...r=...rs...
-0000a590: 721f 0000 0072 8500 0000 721e 0000 0072  r....r....r....r
-0000a5a0: 1900 0000 7286 0000 0072 8700 0000 2910  ....r....r....).
-0000a5b0: 725d 0000 00da 0d6f 7574 6c65 745f 6f62  r].....outlet_ob
-0000a5c0: 735f 6964 da16 7061 7468 5f73 7562 5f72  s_id..path_sub_r
-0000a5d0: 6567 5f6f 7574 6c65 7473 5f76 725e 0000  eg_outlets_vr^..
-0000a5e0: 0072 7600 0000 5a0f 5375 625f 7265 675f  .rv...Z.Sub_reg_
-0000a5f0: 6f75 746c 6574 735a 1353 7562 5f72 6567  outletsZ.Sub_reg
-0000a600: 5f6f 7574 6c65 7473 5f69 6473 5a0f 7265  _outlets_idsZ.re
-0000a610: 675f 6f75 746c 6574 5f69 6e66 6f72 a800  g_outlet_infor..
-0000a620: 0000 5a0d 6f75 746c 6574 4944 5f69 6e66  ..Z.outletID_inf
-0000a630: 6f72 f400 0000 7228 0000 005a 0775 7072  or....r(...Z.upr
-0000a640: 6567 6964 5a12 4879 6472 6f42 6173 696e  egidZ.HydroBasin
-0000a650: 735f 7265 6d6f 7665 722c 0000 0072 f700  s_remover,...r..
-0000a660: 0000 722d 0000 0072 2d00 0000 722e 0000  ..r-...r-...r...
-0000a670: 00da 1f72 6574 7572 6e5f 696e 7465 7265  ...return_intere
-0000a680: 7374 5f63 6174 6368 6d65 6e74 735f 696e  st_catchments_in
-0000a690: 666f 6c0b 0000 7354 0000 0000 0208 0104  fol...sT........
-0000a6a0: 0214 0204 010a 0104 020a 020e 010a 010c  ................
-0000a6b0: 0314 0304 0208 0108 0104 0212 010c 0110  ................
-0000a6c0: 020a 0104 030a 040e 0212 010e 0220 0102  ............. ..
-0000a6d0: 010a 0104 0104 ff04 0310 0104 0214 0104  ................
-0000a6e0: 0304 0112 010e 010e 020c 020a 0214 0172  ...............r
-0000a6f0: 1201 0000 6302 0000 0000 0000 0000 0000  ....c...........
-0000a700: 000c 0000 0005 0000 0003 0000 0073 5201  .............sR.
-0000a710: 0000 6700 7d02 8801 6401 1900 6a00 7d03  ..g.}...d...j.}.
-0000a720: 7401 a002 7c03 a101 7d03 6700 7d02 7403  t...|...}.g.}.t.
-0000a730: a004 a100 7405 6a06 6402 3c00 7c02 a007  ....t.j.d.<.|...
-0000a740: 6403 a101 0100 7c02 a007 6404 a101 0100  d.....|...d.....
-0000a750: 7c02 a007 6405 a101 0100 7408 7c03 8301  |...d.....t.|...
-0000a760: 7d04 7c02 a007 6406 7409 7c04 8301 1700  }.|...d.t.|.....
-0000a770: a101 0100 740a 7c01 6407 1900 6a00 8301  ....t.|.d...j...
-0000a780: 6408 1700 740a 7c01 6409 1900 6a00 8301  d...t.|.d...j...
-0000a790: 6408 1700 1400 7d05 7c02 a007 640a 7409  d.....}.|...d.t.
-0000a7a0: 7c05 8301 1700 a101 0100 7c02 a007 640b  |.........|...d.
-0000a7b0: a101 0100 7c02 a007 640c a101 0100 740a  ....|...d.....t.
-0000a7c0: 7c01 6409 1900 6a00 8301 8902 7c01 640d  |.d...j.....|.d.
-0000a7d0: 1900 6a00 8900 740b 7408 7c03 8301 640e  ..j...t.t.|...d.
-0000a7e0: 1b00 8301 7d06 7408 7c03 8301 640f 6b04  ....}.t.|...d.k.
-0000a7f0: 72ee 7401 a00c 7c03 7c06 a102 7d07 6e06  r.t...|.|...}.n.
-0000a800: 7c03 6701 7d07 740d 6410 7408 7c07 8301  |.g.}.t.d.t.|...
-0000a810: 8302 4400 5d36 7d08 7c07 7c08 1900 7d09  ..D.]6}.|.|...}.
-0000a820: 740e 6411 6412 8d01 8700 8701 8702 6603  t.d.d.........f.
-0000a830: 6413 6414 8408 7c09 4400 8301 8301 7d0a  d.d...|.D.....}.
-0000a840: 7c02 7c0a 1700 7d02 9001 7102 7c02 a007  |.|...}...q.|...
-0000a850: 6415 a101 0100 6416 a00f 7c02 a101 7d0b  d.....d...|...}.
-0000a860: 7c0b 5300 2917 4e72 9100 0000 5a12 4a4f  |.S.).Nr....Z.JO
-0000a870: 424c 4942 5f54 454d 505f 464f 4c44 4552  BLIB_TEMP_FOLDER
-0000a880: 7a0c 3a47 7269 6457 6569 6768 7473 7a0a  z.:GridWeightsz.
-0000a890: 2020 2023 2020 2020 2020 7a0d 2020 2023     #      z.   #
-0000a8a0: 205b 2320 4852 5573 5d7a 1520 2020 3a4e   [# HRUs]z.   :N
-0000a8b0: 756d 6265 7248 5255 7320 2020 2020 2020  umberHRUs       
-0000a8c0: 5a03 526f 7772 4f00 0000 da03 436f 6c7a  Z.RowrO.....Colz
-0000a8d0: 1520 2020 3a4e 756d 6265 7247 7269 6443  .   :NumberGridC
-0000a8e0: 656c 6c73 2020 7a10 2020 2023 2020 2020  ells  z.   #    
-0000a8f0: 2020 2020 2020 2020 7a1d 2020 2023 205b          z.   # [
-0000a900: 4852 5520 4944 5d20 5b43 656c 6c20 235d  HRU ID] [Cell #]
-0000a910: 205b 775f 6b6c 5d5a 0446 4749 4472 bd00   [w_kl]Z.FGIDr..
-0000a920: 0000 7263 0000 0072 0100 0000 72fa 0000  ..rc...r....r...
-0000a930: 0029 015a 066e 5f6a 6f62 7363 0100 0000  .).Z.n_jobsc....
-0000a940: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-0000a950: 3300 0000 7328 0000 007c 005d 207d 0174  3...s(...|.] }.t
-0000a960: 0074 0183 017c 0188 016a 0264 0064 018d  .t...|...j.d.d..
-0000a970: 0188 0088 0283 0456 0001 0071 0264 0253  .......V...q.d.S
-0000a980: 0029 0354 7208 0000 004e 2903 7205 0000  .).Tr....N).r...
-0000a990: 00da 1663 7265 6174 655f 6772 6964 5f77  ...create_grid_w
-0000a9a0: 6569 6768 745f 6872 7572 1600 0000 2902  eight_hrur....).
-0000a9b0: da02 2e30 7228 0000 00a9 03da 0741 7661  ...0r(.......Ava
-0000a9c0: 6667 6964 da0a 4d61 7066 6f72 6369 6e67  fgid..Mapforcing
-0000a9d0: da07 6d61 785f 636f 6c72 2d00 0000 722e  ..max_colr-...r.
-0000a9e0: 0000 00da 093c 6765 6e65 7870 723e d50b  .....<genexpr>..
-0000a9f0: 0000 f300 0000 007a 2a63 7265 6174 655f  .......z*create_
-0000aa00: 6772 6964 5f77 6569 6768 745f 6d61 696e  grid_weight_main
-0000aa10: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-0000aa20: 7072 3e7a 0f3a 456e 6447 7269 6457 6569  pr>z.:EndGridWei
-0000aa30: 6768 7473 da01 0a29 1072 2000 0000 7221  ghts...).r ...r!
-0000aa40: 0000 0072 3c00 0000 da08 7465 6d70 6669  ...r<.....tempfi
-0000aa50: 6c65 da0a 6765 7474 656d 7064 6972 da02  le..gettempdir..
-0000aa60: 6f73 da07 656e 7669 726f 6e72 3100 0000  os..environr1...
-0000aa70: 721f 0000 0072 cb00 0000 7265 0000 0072  r....r....re...r
-0000aa80: a300 0000 da0b 6172 7261 795f 7370 6c69  ......array_spli
-0000aa90: 7472 1e00 0000 7204 0000 00da 046a 6f69  tr....r......joi
-0000aaa0: 6e29 0c72 1801 0000 5a08 466f 7263 696e  n).r....Z.Forcin
-0000aab0: 666f 5a17 6772 6964 5f77 6569 6768 745f  foZ.grid_weight_
-0000aac0: 7374 7269 6e67 5f6c 6973 745a 0668 7275  string_listZ.hru
-0000aad0: 6964 735a 0573 4e68 7275 5a06 734e 6365  idsZ.sNhruZ.sNce
-0000aae0: 6c6c 5a0b 6e5f 6872 755f 6772 6f75 705a  llZ.n_hru_groupZ
-0000aaf0: 0e68 7275 5f69 6473 5f67 726f 7570 7372  .hru_ids_groupsr
-0000ab00: 2800 0000 5a0b 695f 6872 755f 6772 6f75  (...Z.i_hru_grou
-0000ab10: 705a 1867 7269 645f 7765 6967 6874 5f73  pZ.grid_weight_s
-0000ab20: 7472 696e 675f 6872 7573 695a 1267 7269  tring_hrusiZ.gri
-0000ab30: 645f 7765 6967 6874 5f73 7472 696e 6772  d_weight_stringr
-0000ab40: 2d00 0000 7216 0100 0072 2e00 0000 da17  -...r....r......
-0000ab50: 6372 6561 7465 5f67 7269 645f 7765 6967  create_grid_weig
-0000ab60: 6874 5f6d 6169 6eb1 0b00 0073 3600 0000  ht_main....s6...
-0000ab70: 0002 0401 0a01 0a02 0402 0e03 0a01 0a01  ................
-0000ab80: 0a02 0801 1202 2401 1201 0a01 0a01 0e01  ......$.........
-0000ab90: 0a04 1002 0c01 0e02 0602 1201 0801 2001  .............. .
-0000aba0: 0c02 0a01 0a01 7223 0100 0063 0400 0000  ......r#...c....
-0000abb0: 0000 0000 0000 0000 0e00 0000 0600 0000  ................
-0000abc0: 4300 0000 7316 0200 0064 017d 047c 016a  C...s....d.}.|.j
-0000abd0: 007c 0164 0219 007c 006b 0219 006a 0164  .|.d...|.k...j.d
-0000abe0: 0364 048d 017d 0574 027c 0583 0164 056b  .d...}.t.|...d.k
-0000abf0: 0172 5c7c 016a 007c 0164 0219 007c 006b  .r\|.j.|.d...|.k
-0000ac00: 0219 006a 0164 0364 048d 017d 0574 0364  ...j.d.d...}.t.d
-0000ac10: 0683 0101 0074 037c 0564 0719 0083 0101  .....t.|.d......
-0000ac20: 007c 0453 0074 047c 0564 0819 006a 0583  .|.S.t.|.d...j..
-0000ac30: 017d 067c 0564 0719 006a 057d 0774 06a0  .}.|.d...j.}.t..
-0000ac40: 077c 07a1 017d 0764 097d 0874 0864 0574  .|...}.d.}.t.d.t
-0000ac50: 027c 0783 0183 0244 0090 015d 7e7d 097c  .|.....D...]~}.|
-0000ac60: 057c 0564 0719 007c 077c 0919 006b 0219  .|.d...|.|...k..
-0000ac70: 007d 0a7c 0974 027c 0783 0164 0a18 006b  .}.|.t.|...d...k
-0000ac80: 0072 e274 047c 0a64 0819 006a 0583 017d  .r.t.|.d...j...}
-0000ac90: 0b74 097c 0b83 0174 097c 0683 011b 007d  .t.|...t.|.....}
-0000aca0: 0c7c 087c 0c17 007d 086e 0864 0a7c 0818  .|.|...}.n.d.|..
-0000acb0: 007d 0c74 027c 0a64 0b19 006a 0583 0164  .}.t.|.d...j...d
-0000acc0: 0a6b 0490 0172 4074 0374 0a74 0b83 0164  .k...r@t.t.t...d
-0000acd0: 0c17 0083 0101 0074 0a74 0c7c 0a64 0b19  .......t.t.|.d..
-0000ace0: 006a 0564 0519 007c 0364 0a17 0014 007c  .j.d...|.d.....|
-0000acf0: 0a64 0d19 006a 0564 0519 0017 0083 0183  .d...j.d........
-0000ad00: 0164 0e17 007d 0d6e 3074 0a74 0c7c 0a64  .d...}.n0t.t.|.d
-0000ad10: 0b19 006a 0564 0519 007c 0364 0a17 0014  ...j.d...|.d....
-0000ad20: 007c 0a64 0d19 006a 0564 0519 0017 0083  .|.d...j.d......
-0000ad30: 0183 0164 0e17 007d 0d74 027c 0783 0164  ...d...}.t.|...d
-0000ad40: 0a6b 0290 0172 a87c 0464 0f17 0074 0a74  .k...r.|.d...t.t
-0000ad50: 0c7c 0083 0183 0117 0064 1017 007c 0d17  .|.......d...|..
-0000ad60: 0064 0e17 0074 0a7c 0c83 0117 007d 0471  .d...t.|.....}.q
-0000ad70: 907c 0974 027c 0783 0164 0a18 006b 0290  .|.t.|...d...k..
-0000ad80: 0172 e47c 0464 0f17 0074 0a74 0c7c 0083  .r.|.d...t.t.|..
-0000ad90: 0183 0117 0064 1017 007c 0d17 0064 0e17  .....d...|...d..
-0000ada0: 0074 0a7c 0c83 0117 007d 0471 907c 0464  .t.|.....}.q.|.d
-0000adb0: 0f17 0074 0a74 0c7c 0083 0183 0117 0064  ...t.t.|.......d
-0000adc0: 1017 007c 0d17 0064 0e17 0074 0a7c 0c83  ...|...d...t.|..
-0000add0: 0117 0064 1117 007d 0471 907c 0453 0029  ...d...}.q.|.S.)
-0000ade0: 124e fa01 2072 9100 0000 5472 0800 0000  .N.. r....Tr....
-0000adf0: 7201 0000 007a 2846 6f6c 6c6f 7769 6e67  r....z(Following
-0000ae00: 2047 7269 6420 6861 7320 746f 2062 6520   Grid has to be 
-0000ae10: 696e 6c75 6465 643a 2e2e 2e2e 2e2e 2e5a  inluded:.......Z
-0000ae20: 084d 6170 5f46 4749 445a 0673 5f61 7265  .Map_FGIDZ.s_are
-0000ae30: 6172 4d00 0000 724f 0000 005a 074d 6170  arM...rO...Z.Map
-0000ae40: 5f52 6f77 7a3d 6572 726f 723a 2031 2068  _Rowz=error: 1 h
-0000ae50: 7275 2c20 3120 6772 6964 2c20 7072 6f64  ru, 1 grid, prod
-0000ae60: 7563 6520 6d75 7469 2070 6f6c 7967 6f6e  uce muti polygon
-0000ae70: 206e 6565 6420 746f 2062 6520 6d65 7267   need to be merg
-0000ae80: 6564 205a 074d 6170 5f43 6f6c 7a06 2020  ed Z.Map_Colz.  
-0000ae90: 2020 2020 7a04 2020 2020 7a05 2020 2020      z.    z.    
-0000aea0: 2072 1c01 0000 290d 7223 0000 0072 1600   r....).r#...r..
-0000aeb0: 0000 721f 0000 0072 7300 0000 7219 0000  ..r....rs...r...
-0000aec0: 0072 2000 0000 7221 0000 0072 3c00 0000  .r ...r!...r<...
-0000aed0: 721e 0000 0072 4a00 0000 72cb 0000 0072  r....rJ...r....r
-0000aee0: a500 0000 72a3 0000 0029 0e72 4600 0000  ....r....).rF...
-0000aef0: 7218 0100 0072 1701 0000 7219 0100 005a  r....r....r....Z
-0000af00: 1667 7269 645f 7765 6967 6874 5f73 7472  .grid_weight_str
-0000af10: 696e 675f 6872 75da 0463 6174 735a 0574  ing_hru..catsZ.t
-0000af20: 6172 6561 5a04 6669 6473 5a05 7375 6d77  areaZ.fidsZ.sumw
-0000af30: 7472 4400 0000 5a04 7363 6174 5a05 7361  trD...Z.scatZ.sa
-0000af40: 7265 61da 0277 745a 0953 7472 6365 6c6c  rea..wtZ.Strcell
-0000af50: 6964 722d 0000 0072 2d00 0000 722e 0000  idr-...r-...r...
-0000af60: 0072 1401 0000 dc0b 0000 736c 0000 0000  .r........sl....
-0000af70: 0204 021a 040c 011a 0108 010c 0104 020e  ................
-0000af80: 010a 010a 0104 0114 0114 0110 010e 0110  ................
-0000af90: 010a 0208 0214 0102 0106 0102 ff02 ff04  ................
-0000afa0: 0502 0102 010c 0106 ff02 020c fe02 ff02  ................
-0000afb0: ff02 0702 f902 ff04 0c02 0102 010c 0106  ................
-0000afc0: ff02 020c fe02 ff02 ff02 0702 f902 ff02  ................
-0000afd0: 0a0e 012a 0212 012a 022e 0272 1401 0000  ...*...*...r....
-0000afe0: 2901 724f 0000 0029 0172 0600 0000 2902  ).rO...).r....).
-0000aff0: 724f 0000 0072 4f00 0000 2902 724f 0000  rO...rO...).rO..
-0000b000: 0072 4f00 0000 2901 720f 0100 0029 2e72  .rO...).r....).r
-0000b010: 1600 0000 da05 6e75 6d70 7972 2100 0000  ......numpyr!...
-0000b020: da06 7061 6e64 6173 721a 0000 005a 0e73  ..pandasr....Z.s
-0000b030: 6369 7079 2e6f 7074 696d 697a 6572 0200  cipy.optimizer..
-0000b040: 0000 5a1e 6261 7369 6e6d 616b 6572 2e75  ..Z.basinmaker.u
-0000b050: 7469 6c69 7469 6573 2e75 7469 6c69 7469  tilities.utiliti
-0000b060: 6573 da07 6e75 6d62 6572 735a 066a 6f62  es..numbersZ.job
-0000b070: 6c69 6272 0400 0000 7205 0000 0072 1d01  libr....r....r..
-0000b080: 0000 722f 0000 0072 3900 0000 7248 0000  ..r/...r9...rH..
-0000b090: 0072 5f00 0000 7268 0000 0072 7a00 0000  .r_...rh...rz...
-0000b0a0: 7290 0000 0072 9300 0000 729d 0000 0072  r....r....r....r
-0000b0b0: 9f00 0000 7296 0000 0072 8500 0000 72b4  ....r....r....r.
-0000b0c0: 0000 0072 bb00 0000 72c3 0000 0072 c700  ...r....r....r..
-0000b0d0: 0000 72ce 0000 0072 e000 0000 72ea 0000  ..r....r....r...
-0000b0e0: 0072 ed00 0000 72ef 0000 0072 f200 0000  .r....r....r....
-0000b0f0: 72f8 0000 0072 ff00 0000 7200 0100 0072  r....r....r....r
-0000b100: 0101 0000 7203 0100 0072 0501 0000 7207  ....r....r....r.
-0000b110: 0100 0072 0e01 0000 7212 0100 0072 2301  ...r....r....r#.
-0000b120: 0000 7214 0100 0072 2d00 0000 722d 0000  ..r....r-...r-..
-0000b130: 0072 2d00 0000 722e 0000 00da 083c 6d6f  .r-...r......<mo
-0000b140: 6475 6c65 3e01 0000 0073 7000 0000 0802  dule>....sp.....
-0000b150: 0801 0801 0c01 0801 0801 1001 0802 081e  ................
-0000b160: 0819 0857 084e 0858 0a7f 001e 0201 0201  ...W.N.X........
-0000b170: 0401 0401 0201 02f7 0a7f 0015 0a18 0a3e  ...............>
-0000b180: 080a 087f 007f 0021 082a 0860 087f 0060  .......!.*.`...`
-0000b190: 087b 0813 087f 0078 087f 007f 007f 0025  .{.....x.......%
-0000b1a0: 0850 0867 086f 082b 0820 087f 0004 0856  .P.g.o.+. .....V
-0000b1b0: 082a 0a54 0804 080b 081a 0a45 082b       .*.T.......E.+
+00000070: 0100 6400 6401 6c0c 5a0c 6401 6504 6a0d  ..d.d.l.Z.d.e.j.
+00000080: 6a0e 5f0f 6405 6406 8400 5a10 6407 6408  j._.d.d...Z.d.d.
+00000090: 8400 5a11 6409 640a 8400 5a12 640b 640c  ..Z.d.d...Z.d.d.
+000000a0: 8400 5a13 640d 640e 8400 5a14 640f 6410  ..Z.d.d...Z.d.d.
+000000b0: 8400 5a15 6411 6412 8400 5a16 6413 6414  ..Z.d.d...Z.d.d.
+000000c0: 8400 5a17 6451 6416 6417 8401 5a18 6418  ..Z.dQd.d...Z.d.
+000000d0: 6418 6418 6701 6418 6701 6418 6418 6606  d.d.g.d.g.d.d.f.
+000000e0: 6419 641a 8401 5a19 6452 641c 641d 8401  d.d...Z.dRd.d...
+000000f0: 5a1a 6453 641e 641f 8401 5a1b 6420 6421  Z.dSd.d...Z.d d!
+00000100: 8400 5a1c 6422 6423 8400 5a1d 6424 6425  ..Z.d"d#..Z.d$d%
+00000110: 8400 5a1e 6426 6427 8400 5a1f 6428 6429  ..Z.d&d'..Z.d(d)
+00000120: 8400 5a20 642a 642b 8400 5a21 642c 642d  ..Z d*d+..Z!d,d-
+00000130: 8400 5a22 642e 642f 8400 5a23 6430 6431  ..Z"d.d/..Z#d0d1
+00000140: 8400 5a24 6432 6433 8400 5a25 6434 6435  ..Z$d2d3..Z%d4d5
+00000150: 8400 5a26 6436 6437 8400 5a27 6438 6439  ..Z&d6d7..Z'd8d9
+00000160: 8400 5a28 643a 643b 8400 5a29 643c 643d  ..Z(d:d;..Z)d<d=
+00000170: 8400 5a2a 643e 643f 8400 5a2b 6440 6441  ..Z*d>d?..Z+d@dA
+00000180: 8400 5a2c 6454 6442 6443 8401 5a2d 6444  ..Z,dTdBdC..Z-dD
+00000190: 6445 8400 5a2e 6446 6447 8400 5a2f 6448  dE..Z.dFdG..Z/dH
+000001a0: 6449 8400 5a30 6455 644b 644c 8401 5a31  dI..Z0dUdKdL..Z1
+000001b0: 644d 644e 8400 5a32 644f 6450 8400 5a33  dMdN..Z2dOdP..Z3
+000001c0: 6401 5300 2956 e900 0000 004e 2901 da09  d.S.)V.....N)...
+000001d0: 6375 7276 655f 6669 7429 01da 012a 2902  curve_fit)...*).
+000001e0: da08 5061 7261 6c6c 656c da07 6465 6c61  ..Parallel..dela
+000001f0: 7965 6463 0400 0000 0000 0000 0000 0000  yedc............
+00000200: 1200 0000 0600 0000 4300 0000 7352 0100  ........C...sR..
+00000210: 0064 017d 0464 017d 0564 017d 0664 017d  .d.}.d.}.d.}.d.}
+00000220: 077c 007c 0064 0219 00a0 007c 0064 0319  .|.|.d.....|.d..
+00000230: 006a 01a1 010f 0019 007d 087c 0864 0219  .j.......}.|.d..
+00000240: 00a0 007c 01a1 016a 0264 0464 058d 017d  ...|...j.d.d...}
+00000250: 097c 087c 0919 007d 0a74 037c 0a83 0164  .|.|...}.t.|...d
+00000260: 066b 0172 5e7c 017c 027c 0766 0353 007c  .k.r^|.|.|.f.S.|
+00000270: 0a7c 0a64 0319 00a0 007c 01a1 010f 0019  .|.d.....|......
+00000280: 006a 0264 0464 058d 017d 0b74 037c 0b83  .j.d.d...}.t.|..
+00000290: 0164 066b 0172 907c 017c 027c 0766 0353  .d.k.r.|.|.|.f.S
+000002a0: 007c 0064 0364 0267 0219 00a0 0464 07a1  .|.d.d.g.....d..
+000002b0: 016a 017d 0c7c 0b64 0319 006a 0144 005d  .j.}.|.d...j.D.]
+000002c0: 947d 0d74 057c 0c7c 0d83 027d 0e7c 007c  .}.t.|.|...}.|.|
+000002d0: 0064 0319 00a0 007c 0ea1 0119 007d 0f7c  .d.....|.....}.|
+000002e0: 026a 067c 0f64 0364 0864 098d 037d 027c  .j.|.d.d.d...}.|
+000002f0: 0264 0319 00a0 007c 0ea1 017d 107c 026a  .d.....|...}.|.j
+00000300: 077c 1064 0266 0219 006a 017c 026a 077c  .|.d.f...j.|.j.|
+00000310: 1064 0a66 023c 007c 0264 0364 0a67 0219  .d.f.<.|.d.d.g..
+00000320: 00a0 0464 07a1 016a 017d 0374 057c 037c  ...d...j.}.t.|.|
+00000330: 0d83 027d 1174 086a 097c 017c 1166 0264  ...}.t.j.|.|.f.d
+00000340: 0664 0b8d 027d 017c 026a 0a64 0264 0c8d  .d...}.|.j.d.d..
+00000350: 017d 0271 ae64 047d 077c 017c 027c 0766  .}.q.d.}.|.|.|.f
+00000360: 0353 0029 0d4e 465a 0c53 6563 5f44 6f77  .S.).NFZ.Sec_Dow
+00000370: 5375 6249 64da 0553 7562 4964 54a9 01da  SubId..SubIdT...
+00000380: 0464 6565 7072 0100 0000 da05 696e 7433  .deepr......int3
+00000390: 32da 046c 6566 7429 02da 026f 6eda 0368  2..left)...on..h
+000003a0: 6f77 da08 446f 7753 7562 4964 a901 da04  ow..DowSubId....
+000003b0: 6178 6973 a901 da07 636f 6c75 6d6e 7329  axis....columns)
+000003c0: 0bda 0469 7369 6eda 0676 616c 7565 73da  ...isin..values.
+000003d0: 0463 6f70 79da 036c 656e da06 6173 7479  .copy..len..asty
+000003e0: 7065 da06 6465 6663 6174 da05 6d65 7267  pe..defcat..merg
+000003f0: 65da 036c 6f63 da02 6e70 da0b 636f 6e63  e..loc..np..conc
+00000400: 6174 656e 6174 65da 0464 726f 7029 12da  atenate..drop)..
+00000410: 1073 6563 5f64 6f77 6e5f 7375 6269 6e66  .sec_down_subinf
+00000420: 6fda 0d75 7073 7472 6561 6d5f 7375 6273  o..upstream_subs
+00000430: da07 6361 745f 706c 79da 0968 7973 6864  ..cat_ply..hyshd
+00000440: 696e 666f 5a23 6973 5f73 6563 5f64 6f77  infoZ#is_sec_dow
+00000450: 6e5f 7375 6269 645f 696e 5f73 656c 6563  n_subid_in_selec
+00000460: 7465 645f 7375 6269 645a 2b69 735f 7375  ted_subidZ+is_su
+00000470: 6269 645f 6f66 5f73 6563 5f64 6f77 6e73  bid_of_sec_downs
+00000480: 7562 6964 5f69 6e5f 7365 6c65 6374 6564  ubid_in_selected
+00000490: 5f73 7562 6964 da25 7570 6461 7465 5f64  _subid.%update_d
+000004a0: 6f77 6e73 7562 6964 735f 7573 696e 675f  ownsubids_using_
+000004b0: 7365 635f 646f 776e 7375 6269 64da 0f75  sec_downsubid..u
+000004c0: 7064 6174 655f 746f 706f 6c6f 6779 5a19  pdate_topologyZ.
+000004d0: 7365 635f 646f 776e 5f73 7562 696e 666f  sec_down_subinfo
+000004e0: 5f6d 6f73 7464 6f77 6e5a 2073 6563 5f64  _mostdownZ sec_d
+000004f0: 6f77 6e5f 7375 6269 645f 696e 5f73 656c  own_subid_in_sel
+00000500: 6563 7465 645f 7375 6269 645a 2473 6563  ected_subidZ$sec
+00000510: 5f64 6f77 6e5f 7375 6269 6e66 6f5f 646f  _down_subinfo_do
+00000520: 776e 7375 625f 696e 5f73 656c 6563 7465  wnsub_in_selecte
+00000530: 645a 1a6d 6973 7369 6e67 5f73 7562 6964  dZ.missing_subid
+00000540: 5f69 6e5f 7365 635f 7461 626c 655a 0d68  _in_sec_tableZ.h
+00000550: 7973 6864 696e 666f 5f73 6563 5a09 7375  yshdinfo_secZ.su
+00000560: 6269 645f 7365 635a 1175 7073 7472 6561  bid_secZ.upstrea
+00000570: 6d5f 7375 6273 5f73 6563 5a16 7365 635f  m_subs_secZ.sec_
+00000580: 646f 776e 5f73 7562 696e 666f 7365 6c65  down_subinfosele
+00000590: 6374 da04 6d61 736b 5a19 7570 7374 7265  ct..maskZ.upstre
+000005a0: 616d 5f73 7562 735f 6e65 775f 7375 625f  am_subs_new_sub_
+000005b0: 7365 63a9 0072 2400 0000 fa48 633a 5c75  sec..r$....Hc:\u
+000005c0: 7365 7273 5c6d 3433 6861 6e5f 325c 646f  sers\m43han_2\do
+000005d0: 6375 6d65 6e74 735c 6769 7468 7562 5c62  cuments\github\b
+000005e0: 6173 696e 6d61 6b65 725c 6261 7369 6e6d  asinmaker\basinm
+000005f0: 616b 6572 5c66 756e 635c 7064 7461 626c  aker\func\pdtabl
+00000600: 652e 7079 da29 7570 6461 7465 5f73 656c  e.py.)update_sel
+00000610: 6563 7465 645f 7375 6269 645f 7573 696e  ected_subid_usin
+00000620: 675f 7365 635f 646f 776e 7375 6269 640d  g_sec_downsubid.
+00000630: 0000 0073 3200 0000 0001 0401 0401 0401  ...s2...........
+00000640: 0402 1a01 1605 0802 0c01 0a07 1c02 0c01  ................
+00000650: 0a03 1401 0e02 0a01 1202 1001 0e01 1a02  ................
+00000660: 1401 0a02 1201 0e01 0401 7226 0000 0063  ..........r&...c
+00000670: 0400 0000 0000 0000 0000 0000 1000 0000  ................
+00000680: 0600 0000 4300 0000 733a 0100 0064 017d  ....C...s:...d.}
+00000690: 0464 017d 057c 0064 0264 0367 0219 00a0  .d.}.|.d.d.g....
+000006a0: 0064 04a1 016a 017d 0664 057d 0764 057d  .d...j.}.d.}.d.}
+000006b0: 0874 0264 0574 037c 0183 0183 0244 005d  .t.d.t.|.....D.]
+000006c0: 487d 097c 017c 0919 007d 0a74 047c 0a7c  H}.|.|...}.t.|.|
+000006d0: 067c 037c 0083 045c 037d 0b7d 007d 087c  .|.|...\.}.}.}.|
+000006e0: 077c 0817 007d 077c 0964 056b 0272 687c  .|...}.|.d.k.rh|
+000006f0: 0b7d 0c71 3274 056a 067c 0c7c 0b66 0264  .}.q2t.j.|.|.f.d
+00000700: 0564 068d 027d 0c71 3274 05a0 077c 0ca1  .d...}.q2t...|..
+00000710: 017d 0c74 056a 0864 0574 0964 078d 027d  .}.t.j.d.t.d...}
+00000720: 0d74 0264 0574 037c 0283 0183 0244 005d  .t.d.t.|.....D.]
+00000730: 4a7d 0e7c 027c 0e19 007d 0a7c 0a64 056b  J}.|.|...}.|.d.k
+00000740: 0072 b871 a274 047c 0a7c 067c 037c 0083  .r.q.t.|.|.|.|..
+00000750: 045c 037d 0b7d 007d 087c 0e64 056b 0272  .\.}.}.}.|.d.k.r
+00000760: da7c 0b7d 0d71 a274 056a 067c 0d7c 0b66  .|.}.q.t.j.|.|.f
+00000770: 0264 0564 068d 027d 0d71 a274 037c 0d83  .d.d...}.q.t.|..
+00000780: 0164 056b 0490 0172 1c74 05a0 077c 0da1  .d.k...r.t...|..
+00000790: 017d 0d74 05a0 0a7c 0c7c 0da1 020f 007d  .}.t...|.|.....}
+000007a0: 0f7c 0c7c 0f19 007d 0c7c 0764 086b 0590  .|.|...}.|.d.k..
+000007b0: 0172 2c64 097d 086e 0464 017d 087c 0c7c  .r,d.}.n.d.}.|.|
+000007c0: 007c 0866 0353 0029 0a4e 4672 0600 0000  .|.f.S.).NFr....
+000007d0: 720d 0000 0072 0900 0000 7201 0000 0072  r....r....r....r
+000007e0: 0e00 0000 2901 da05 6474 7970 65e9 0100  ....)...dtype...
+000007f0: 0000 5429 0b72 1600 0000 7213 0000 00da  ..T).r....r.....
+00000800: 0572 616e 6765 7215 0000 00da 1f72 6574  .ranger......ret
+00000810: 7572 6e5f 7375 6269 6473 5f64 7261 696e  urn_subids_drain
+00000820: 6167 655f 746f 5f73 7562 6964 721a 0000  age_to_subidr...
+00000830: 0072 1b00 0000 da06 756e 6971 7565 da05  .r......unique..
+00000840: 656d 7074 79da 0369 6e74 da04 696e 3164  empty..int..in1d
+00000850: 2910 721f 0000 00da 0a6d 6f73 7464 6f77  ).r......mostdow
+00000860: 6e69 64da 0e6d 6f73 7475 7073 7472 6561  nid..mostupstrea
+00000870: 6d69 6472 1d00 0000 5a0f 6861 735f 7365  midr....Z.has_se
+00000880: 635f 646f 776e 7375 6272 2100 0000 7220  c_downsubr!...r 
+00000890: 0000 005a 1373 756d 5f75 7064 6174 655f  ...Z.sum_update_
+000008a0: 746f 706f 6c6f 6779 7222 0000 005a 0669  topologyr"...Z.i
+000008b0: 5f64 6f77 6eda 0974 6172 5f73 7562 6964  _down..tar_subid
+000008c0: 721e 0000 005a 0d73 656c 6563 7465 645f  r....Z.selected_
+000008d0: 7375 6273 5a0b 7265 6d6f 7665 5f73 7562  subsZ.remove_sub
+000008e0: 735a 0469 5f75 7072 2300 0000 7224 0000  sZ.i_upr#...r$..
+000008f0: 0072 2400 0000 7225 0000 00da 1772 6574  .r$...r%.....ret
+00000900: 7572 6e5f 6578 7472 6163 7465 645f 7375  urn_extracted_su
+00000910: 6269 6473 3b00 0000 733c 0000 0000 0304  bids;...s<......
+00000920: 0104 0214 0104 0104 0212 0208 0214 0108  ................
+00000930: 0108 0106 0214 020a 030e 0212 0208 0208  ................
+00000940: 0102 0214 0208 0106 0214 020e 010a 020e  ................
+00000950: 0208 010a 0106 0204 0172 3200 0000 6304  .........r2...c.
+00000960: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+00000970: 0000 0043 0000 0073 3800 0000 7400 7c01  ...C...s8...t.|.
+00000980: 7c00 8302 7d04 6401 7d05 7401 7c02 8301  |...}.d.}.t.|...
+00000990: 6401 6b04 722e 7402 7c02 7c04 7c03 7c01  d.k.r.t.|.|.|.|.
+000009a0: 8304 5c03 7d04 7d03 7d05 7c04 7c03 7c05  ..\.}.}.}.|.|.|.
+000009b0: 6603 5300 2902 4e72 0100 0000 2903 7217  f.S.).Nr....).r.
+000009c0: 0000 0072 1500 0000 7226 0000 0029 0672  ...r....r&...).r
+000009d0: 3100 0000 7220 0000 0072 1d00 0000 721f  1...r ...r....r.
+000009e0: 0000 0072 1e00 0000 7222 0000 0072 2400  ...r....r"...r$.
+000009f0: 0000 7224 0000 0072 2500 0000 722a 0000  ..r$...r%...r*..
+00000a00: 0073 0000 0073 0a00 0000 0003 0a01 0402  .s...s..........
+00000a10: 0c01 1402 722a 0000 0063 0400 0000 0000  ....r*...c......
+00000a20: 0000 0000 0000 0d00 0000 0500 0000 4300  ..............C.
+00000a30: 0000 7334 0100 007c 0064 016b 0172 0c7c  ..s4...|.d.k.r.|
+00000a40: 0153 007c 0164 027c 0364 0367 0319 006a  .S.|.d.|.d.g...j
+00000a50: 0064 0464 058d 017d 047c 046a 0164 0364  .d.d...}.|.j.d.d
+00000a60: 0669 0164 078d 017d 047c 046a 0264 027c  .i.d...}.|.j.d.|
+00000a70: 0367 0264 0864 098d 02a0 03a1 007d 0474  .g.d.d.......}.t
+00000a80: 046a 057c 047c 0264 0264 0a8d 037d 047c  .j.|.|.d.d...}.|
+00000a90: 0464 0619 007c 0464 0b19 001b 007c 0464  .d...|.d.....|.d
+00000aa0: 0c3c 007c 046a 0664 0264 0667 0264 0864  .<.|.j.d.d.g.d.d
+00000ab0: 0d8d 027d 047c 046a 0764 0267 0164 0e64  ...}.|.j.d.g.d.d
+00000ac0: 0f8d 026a 0064 0464 058d 017d 057c 047c  ...j.d.d...}.|.|
+00000ad0: 0464 0c19 007c 006b 0019 0064 027c 0367  .d...|.k...d.|.g
+00000ae0: 0219 006a 0064 0464 058d 017d 0674 0864  ...j.d.d...}.t.d
+00000af0: 0174 097c 0683 0183 0244 005d 6a7d 077c  .t.|.....D.]j}.|
+00000b00: 0664 0219 006a 0a7c 0719 007d 087c 067c  .d...j.|...}.|.|
+00000b10: 0319 006a 0a7c 0719 007d 097c 0164 0219  ...j.|...}.|.d..
+00000b20: 007c 086b 027d 0a7c 017c 0319 007c 096b  .|.k.}.|.|...|.k
+00000b30: 027d 0b74 0ba0 0c7c 0a7c 0ba1 027d 0c7c  .}.t...|.|...}.|
+00000b40: 056a 0d7c 0564 0219 007c 086b 0219 007c  .j.|.d...|.k...|
+00000b50: 0319 006a 0a64 0119 007c 016a 0d7c 0c7c  ...j.d...|.j.|.|
+00000b60: 0366 023c 0071 c47c 0153 0029 104e 7201  .f.<.q.|.S.).Nr.
+00000b70: 0000 0072 0600 0000 da08 4852 555f 4172  ...r......HRU_Ar
+00000b80: 6561 5472 0700 0000 5a09 496e 7075 745f  eaTr....Z.Input_
+00000b90: 415f 4772 1000 0000 46a9 01da 0861 735f  A_Gr....F....as_
+00000ba0: 696e 6465 7829 0172 0b00 0000 da07 4261  index).r......Ba
+00000bb0: 735f 415f 475a 0a41 7265 615f 7261 7469  s_A_GZ.Area_rati
+00000bc0: 6fa9 02da 0262 79da 0961 7363 656e 6469  o....by..ascendi
+00000bd0: 6e67 da05 6669 7273 7429 02da 0673 7562  ng..first)...sub
+00000be0: 7365 74da 046b 6565 7029 0e72 1400 0000  set..keep).r....
+00000bf0: da06 7265 6e61 6d65 da07 6772 6f75 7062  ..rename..groupb
+00000c00: 79da 0373 756d da02 7064 7218 0000 00da  y..sum..pdr.....
+00000c10: 0b73 6f72 745f 7661 6c75 6573 da0f 6472  .sort_values..dr
+00000c20: 6f70 5f64 7570 6c69 6361 7465 7372 2900  op_duplicatesr).
+00000c30: 0000 7215 0000 0072 1300 0000 721a 0000  ..r....r....r...
+00000c40: 00da 0b6c 6f67 6963 616c 5f61 6e64 7219  ...logical_andr.
+00000c50: 0000 0029 0dda 0d6c 616e 6475 7365 5f74  ...)...landuse_t
+00000c60: 6872 6573 da07 6872 7569 6e66 6fda 0873  hres..hruinfo..s
+00000c70: 7562 5f61 7265 61da 0a4c 616e 6475 7365  ub_area..Landuse
+00000c80: 5f49 445a 0a73 7562 696e 666f 5f6c 755a  _IDZ.subinfo_luZ
+00000c90: 1473 7562 696e 666f 5f6c 755f 646f 6d69  .subinfo_lu_domi
+00000ca0: 6e61 7465 645a 1673 7562 696e 666f 5f6c  natedZ.subinfo_l
+00000cb0: 755f 6e65 6564 5f63 6861 6e67 65da 0169  u_need_change..i
+00000cc0: da05 7375 6269 645a 076c 616e 6475 7365  ..subidZ.landuse
+00000cd0: da05 6d61 736b 31da 056d 6173 6b32 7223  ..mask1..mask2r#
+00000ce0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00000cf0: 0000 da27 7265 6d6f 7665 5f6c 616e 6475  ...'remove_landu
+00000d00: 7365 5f74 7970 655f 696e 7075 745f 6261  se_type_input_ba
+00000d10: 7365 645f 6f6e 5f61 7265 617e 0000 0073  sed_on_area~...s
+00000d20: 2400 0000 0002 0801 0402 1601 1001 1603  $...............
+00000d30: 1001 1403 1201 1803 2002 1201 0e01 0e01  ........ .......
+00000d40: 0c01 0c01 0c01 2802 724c 0000 0063 0700  ......(.rL...c..
+00000d50: 0000 0000 0000 0000 0000 0e00 0000 0600  ................
+00000d60: 0000 4300 0000 73c2 0000 007c 016a 007c  ..C...s....|.j.|
+00000d70: 0164 0119 0064 026b 0419 00a0 01a1 007d  .d...d.k.......}
+00000d80: 077c 016a 007c 0164 0119 0064 026b 0119  .|.j.|.d...d.k..
+00000d90: 00a0 01a1 007d 087c 0164 0364 0467 0219  .....}.|.d.d.g..
+00000da0: 006a 0164 0564 068d 017d 097c 096a 0264  .j.d.d...}.|.j.d
+00000db0: 0464 0769 0164 088d 017d 097c 096a 0364  .d.i.d...}.|.j.d
+00000dc0: 0367 0164 0964 0a8d 02a0 04a1 007d 097c  .g.d.d.......}.|
+00000dd0: 0064 0219 007d 0a7c 027c 037c 0567 037d  .d...}.|.|.|.g.}
+00000de0: 0b74 0564 0274 067c 0b83 0183 0244 005d  .t.d.t.|.....D.]
+00000df0: 227d 0c7c 0b7c 0c19 007d 0d7c 007c 0c19  "}.|.|...}.|.|..
+00000e00: 007d 0a74 077c 0a7c 087c 097c 0d83 047d  .}.t.|.|.|.|...}
+00000e10: 0871 847c 087c 0219 007c 087c 043c 007c  .q.|.|...|.|.<.|
+00000e20: 07a0 087c 08a1 017d 017c 0153 0029 0b4e  ...|...}.|.S.).N
+00000e30: da0a 4852 555f 4973 4c61 6b65 7201 0000  ..HRU_IsLaker...
+00000e40: 0072 0600 0000 7233 0000 0054 7207 0000  .r....r3...Tr...
+00000e50: 0072 3600 0000 7210 0000 0046 7234 0000  .r6...r....Fr4..
+00000e60: 0029 0972 1900 0000 7214 0000 0072 3d00  .).r....r....r=.
+00000e70: 0000 723e 0000 0072 3f00 0000 7229 0000  ..r>...r?...r)..
+00000e80: 0072 1500 0000 724c 0000 00da 0661 7070  .r....rL.....app
+00000e90: 656e 6429 0eda 1561 7265 615f 7261 7469  end)...area_rati
+00000ea0: 6f5f 7468 7265 7368 6f6c 6473 7245 0000  o_thresholdsrE..
+00000eb0: 0072 4700 0000 da07 536f 696c 5f49 44da  .rG.....Soil_ID.
+00000ec0: 0656 6567 5f49 44da 0e4f 7468 6572 5f50  .Veg_ID..Other_P
+00000ed0: 6c79 5f49 445f 31da 0e4f 7468 6572 5f50  ly_ID_1..Other_P
+00000ee0: 6c79 5f49 445f 325a 0d68 7275 5f6c 616b  ly_ID_2Z.hru_lak
+00000ef0: 655f 696e 666f 5a0d 6872 755f 6c61 6e64  e_infoZ.hru_land
+00000f00: 5f69 6e66 6f72 4600 0000 7244 0000 00da  _inforF...rD....
+00000f10: 046c 6973 7472 4800 0000 da04 4974 656d  .listrH.....Item
+00000f20: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00000f30: 1573 696d 706c 6966 795f 6872 7573 5f6d  .simplify_hrus_m
+00000f40: 6574 686f 6432 9c00 0000 731c 0000 0000  ethod2....s.....
+00000f50: 0316 0116 0214 0110 0114 0308 010a 0112  ................
+00000f60: 0108 0108 0110 010c 020a 0272 5600 0000  ...........rV...
+00000f70: 6303 0000 0000 0000 0000 0000 001d 0000  c...............
+00000f80: 0009 0000 0043 0000 0073 8e02 0000 7c01  .....C...s....|.
+00000f90: 6401 1900 7c01 6402 3c00 7400 a001 7c01  d...|.d.<.t...|.
+00000fa0: 6403 1900 6a02 a101 7d03 7403 6404 7404  d...j...}.t.d.t.
+00000fb0: 7c03 8301 8302 4400 9002 5d4e 7d04 7c03  |.....D...]N}.|.
+00000fc0: 7c04 1900 7d05 7c01 6a05 7c01 6403 1900  |...}.|.j.|.d...
+00000fd0: 7c05 6b02 1900 6a06 6405 6406 8d01 7d06  |.k...j.d.d...}.
+00000fe0: 7400 a007 7c06 6407 1900 6a02 a101 7d07  t...|.d...j...}.
+00000ff0: 7c00 7c07 1400 7d08 7c06 6a05 7c06 6407  |.|...}.|.j.|.d.
+00001000: 1900 7c08 6b00 1900 a006 a100 7d09 7c06  ..|.k.......}.|.
+00001010: 6a05 7c06 6407 1900 7c08 6b05 1900 a006  j.|.d...|.k.....
+00001020: a100 7d0a 7c0a 6a08 7d0b 7c0b 7c0b 6402  ..}.|.j.}.|.|.d.
+00001030: 6b03 1900 7d0b 7c02 6404 1900 7d0c 7c09  k...}.|.d...}.|.
+00001040: 6a06 6405 6406 8d01 7d0d 7400 a001 7c0d  j.d.d...}.t...|.
+00001050: 7c0c 1900 6a02 a101 7d0e 7403 6404 7404  |...j...}.t.d.t.
+00001060: 7c0e 8301 8302 4400 5dbc 7d0f 7c0e 7c0f  |.....D.].}.|.|.
+00001070: 1900 7d10 7c0d 6a05 7c0d 7c0c 1900 7c10  ..}.|.j.|.|...|.
+00001080: 6b02 1900 6a06 6405 6406 8d01 7d11 7400  k...j.d.d...}.t.
+00001090: a007 7c11 6407 1900 6a02 a101 7d12 7c12  ..|.d...j...}.|.
+000010a0: 7c08 6b05 72da 7c11 6a09 6407 6701 6408  |.k.r.|.j.d.g.d.
+000010b0: 6409 8d02 7d11 7403 6404 7404 7c0b 8301  d...}.t.d.t.|...
+000010c0: 8302 4400 5d44 7d13 7c0b 7c13 1900 7d14  ..D.]D}.|.|...}.
+000010d0: 7c14 640a 6b02 9001 7250 9001 7136 7c11  |.d.k...rP..q6|.
+000010e0: 7c14 1900 6a02 6404 1900 7c01 6a05 7c01  |...j.d...|.j.|.
+000010f0: 6402 1900 a00a 7c11 6402 1900 6a02 a101  d.....|.d...j...
+00001100: 7c14 6602 3c00 9001 7136 7c09 7c09 6402  |.f.<...q6|.|.d.
+00001110: 1900 a00a 7c11 6402 1900 6a02 a101 0f00  ....|.d...j.....
+00001120: 1900 7d09 71da 7c09 6a0b 7d15 7403 6404  ..}.q.|.j.}.t.d.
+00001130: 7404 7c15 8301 8302 4400 5dcc 7d16 7c15  t.|.....D.].}.|.
+00001140: 7c16 1900 7d17 7c09 6a05 7c17 6402 6602  |...}.|.j.|.d.f.
+00001150: 1900 7d18 7403 6404 7404 7c02 8301 8302  ..}.t.d.t.|.....
+00001160: 4400 5da0 7d19 7c02 7c19 1900 7d1a 7c09  D.].}.|.|...}.|.
+00001170: 6a05 7c17 7c1a 6602 1900 7d1b 7c0a 6a05  j.|.|.f...}.|.j.
+00001180: 7c0a 7c1a 1900 7c1b 6b02 1900 a006 a100  |.|...|.k.......
+00001190: 7d1c 7404 7c1c 8301 6404 6b04 9001 72d4  }.t.|...d.k...r.
+000011a0: 7c1c 6a09 6407 6408 6409 8d02 7d1c 7403  |.j.d.d.d...}.t.
+000011b0: 6404 7404 7c0b 8301 8302 4400 5d3c 7d13  d.t.|.....D.]<}.
+000011c0: 7c0b 7c13 1900 7d14 7c14 640a 6b02 9002  |.|...}.|.d.k...
+000011d0: 7248 9002 712e 7c1c 7c14 1900 6a02 6404  rH..q.|.|...j.d.
+000011e0: 1900 7c01 6a05 7c01 6402 1900 7c18 6b02  ..|.j.|.d...|.k.
+000011f0: 7c14 6602 3c00 9002 712e 6e04 9001 71d4  |.f.<...q.n...q.
+00001200: 9001 71d4 9001 71ac 712a 7c01 6a0c 6402  ..q...q.q*|.j.d.
+00001210: 6701 640b 8d01 7d01 7c01 5300 290c 4eda  g.d...}.|.S.).N.
+00001220: 0a48 5255 5f49 445f 4e65 775a 0b48 5255  .HRU_ID_NewZ.HRU
+00001230: 5f49 445f 4e65 7732 7206 0000 0072 0100  _ID_New2r....r..
+00001240: 0000 5472 0700 0000 7233 0000 0046 7237  ..Tr....r3...Fr7
+00001250: 0000 00da 0553 4841 5045 7210 0000 0029  .....SHAPEr....)
+00001260: 0d72 1a00 0000 722b 0000 0072 1300 0000  .r....r+...r....
+00001270: 7229 0000 0072 1500 0000 7219 0000 0072  r)...r....r....r
+00001280: 1400 0000 723f 0000 0072 1100 0000 7241  ....r?...r....rA
+00001290: 0000 0072 1200 0000 da05 696e 6465 7872  ...r......indexr
+000012a0: 1c00 0000 291d da14 6d69 6e5f 6872 755f  ....)...min_hru_
+000012b0: 7063 745f 7375 625f 6172 6561 7245 0000  pct_sub_arearE..
+000012c0: 00da 1069 6d70 6f72 7461 6e63 655f 6f72  ...importance_or
+000012d0: 6465 72da 0673 7562 6964 7372 4800 0000  der..subidsrH...
+000012e0: 7249 0000 005a 0c73 7562 5f68 7275 5f69  rI...Z.sub_hru_i
+000012f0: 6e66 6f5a 0873 7562 6173 7265 615a 0c73  nfoZ.subasreaZ.s
+00001300: 7562 6172 6561 5f74 6872 735a 106e 6565  ubarea_thrsZ.nee
+00001310: 645f 7265 6d6f 7665 5f68 7275 735a 0967  d_remove_hrusZ.g
+00001320: 6f6f 645f 6872 7573 5a0b 6872 755f 636f  ood_hrusZ.hru_co
+00001330: 6c75 6d6e 735a 0663 6f6c 6e6d 315a 1c69  lumnsZ.colnm1Z.i
+00001340: 6d70 6f72 7431 5f41 7265 615f 6e65 6564  mport1_Area_need
+00001350: 5f72 656d 6f76 655f 6872 755a 0e75 6e69  _remove_hruZ.uni
+00001360: 7175 655f 696d 706f 7274 315a 0869 5f69  que_import1Z.i_i
+00001370: 6d70 6f72 745a 0869 5f63 6f6c 6e6d 315a  mportZ.i_colnm1Z
+00001380: 1e69 5f69 6d70 6f72 7431 5f41 7265 615f  .i_import1_Area_
+00001390: 6e65 6564 5f72 656d 6f76 655f 6872 755a  need_remove_hruZ
+000013a0: 2774 6f74 616c 5f61 7265 615f 695f 696d  'total_area_i_im
+000013b0: 706f 7274 5f69 6e5f 6e65 6564 5f72 656d  port_in_need_rem
+000013c0: 6f76 655f 6872 7573 5a04 695f 6e6d 5a0a  ove_hrusZ.i_nmZ.
+000013d0: 636f 6c75 6d6e 6e61 6d65 da07 696e 6465  columnname..inde
+000013e0: 7865 73da 016a da03 6964 78da 0568 7275  xes..j..idx..hru
+000013f0: 6964 da01 6b5a 0563 6f6c 6e6d 5a10 6174  id..kZ.colnmZ.at
+00001400: 7472 695f 7265 6d6f 7665 5f68 7275 5a0b  tri_remove_hruZ.
+00001410: 676f 6f64 5f68 7275 735f 6b72 2400 0000  good_hrus_kr$...
+00001420: 7224 0000 0072 2500 0000 da0e 7369 6d70  r$...r%.....simp
+00001430: 6c69 6466 795f 6872 7573 b500 0000 7358  lidfy_hrus....sX
+00001440: 0000 0000 020c 0210 0314 0108 021a 0210  ................
+00001450: 0108 0316 0216 0206 020c 0308 010c 0110  ................
+00001460: 0512 0108 011a 0110 0508 0310 0112 0108  ................
+00001470: 010a 0104 022c 031c 0206 0412 0108 010e  .....,..........
+00001480: 0412 0108 020e 0316 020e 020e 0112 0108  ................
+00001490: 010a 0104 0226 020e 010e 0172 6200 0000  .....&.....rb...
+000014a0: 6301 0000 0000 0000 0000 0000 000b 0000  c...............
+000014b0: 0005 0000 0043 0000 0073 ba02 0000 7c00  .....C...s....|.
+000014c0: 6401 6402 6702 1900 a000 6403 a101 6a01  d.d.g.....d...j.
+000014d0: 7d01 7c00 6a02 7c00 6404 1900 6405 6b02  }.|.j.|.d...d.k.
+000014e0: 1900 a003 a100 7d02 7c02 6401 1900 a003  ......}.|.d.....
+000014f0: a100 7d03 7c00 6406 1900 a004 a100 7d04  ..}.|.d.......}.
+00001500: 6407 7c00 6a02 7c00 6401 1900 a005 7c03  d.|.j.|.d.....|.
+00001510: a101 6408 6602 3c00 7406 6409 7407 7c02  ..d.f.<.t.d.t.|.
+00001520: 8301 8302 4400 9002 5d4a 7d05 7c02 6401  ....D...]J}.|.d.
+00001530: 1900 6a01 7c05 1900 7d06 7c02 6402 1900  ..j.|...}.|.d...
+00001540: 6a01 7c05 1900 7d07 7c00 6a02 7c00 6401  j.|...}.|.j.|.d.
+00001550: 1900 7c07 6b02 1900 a003 a100 7d08 7c07  ..|.k.......}.|.
+00001560: 7d09 7407 7c08 8301 640a 6b00 72fc 640a  }.t.|...d.k.r.d.
+00001570: 7c00 6a02 7c00 6401 1900 7c06 6b02 640b  |.j.|.d...|.k.d.
+00001580: 6602 3c00 7c04 7c05 1700 640a 1700 7c00  f.<.|.|...d...|.
+00001590: 6a02 7c00 6401 1900 7c06 6b02 6406 6602  j.|.d...|.k.d.f.
+000015a0: 3c00 640a 7c00 6a02 7c00 6401 1900 7c06  <.d.|.j.|.d...|.
+000015b0: 6b02 640c 6602 3c00 7168 7c08 6404 1900  k.d.f.<.qh|.d...
+000015c0: 6a01 6409 1900 6405 6b02 9001 728c 7c00  j.d...d.k...r.|.
+000015d0: 6a02 7c00 6401 1900 7c09 6b02 1900 a003  j.|.d...|.k.....
+000015e0: a100 7d0a 7c0a 6402 1900 6a01 6409 1900  ..}.|.d...j.d...
+000015f0: 7d07 7c00 6a02 7c00 6401 1900 7c07 6b02  }.|.j.|.d...|.k.
+00001600: 1900 a003 a100 7d08 7407 7c08 8301 640a  ......}.t.|...d.
+00001610: 6b00 9001 7260 640d 7d09 9001 718c 7c09  k...r`d.}...q.|.
+00001620: 7c08 6402 1900 6a01 6409 1900 6b02 9001  |.d...j.d...k...
+00001630: 7286 7408 7c09 7c07 8302 0100 640d 7d09  r.t.|.|.....d.}.
+00001640: 9001 718c 7c07 7d09 71fc 7c09 640d 6b02  ..q.|.}.q.|.d.k.
+00001650: 9001 7298 7168 640e 7c00 6a02 7c00 6401  ..r.qhd.|.j.|.d.
+00001660: 1900 7c06 6b02 640f 6602 3c00 640e 7c00  ..|.k.d.f.<.d.|.
+00001670: 6a02 7c00 6401 1900 7c06 6b02 6410 6602  j.|.d...|.k.d.f.
+00001680: 3c00 640e 7c00 6a02 7c00 6401 1900 7c06  <.d.|.j.|.d...|.
+00001690: 6b02 6408 6602 3c00 640e 7c00 6a02 7c00  k.d.f.<.d.|.j.|.
+000016a0: 6401 1900 7c06 6b02 6411 6602 3c00 640e  d...|.k.d.f.<.d.
+000016b0: 7c00 6a02 7c00 6401 1900 7c06 6b02 6412  |.j.|.d...|.k.d.
+000016c0: 6602 3c00 640e 7c00 6a02 7c00 6401 1900  f.<.d.|.j.|.d...
+000016d0: 7c06 6b02 6413 6602 3c00 6414 7c00 6a09  |.k.d.f.<.d.|.j.
+000016e0: 7600 9002 7254 640e 7c00 6a02 7c00 6401  v...rTd.|.j.|.d.
+000016f0: 1900 7c06 6b02 6414 6602 3c00 640e 7c00  ..|.k.d.f.<.d.|.
+00001700: 6a02 7c00 6401 1900 7c06 6b02 6415 6602  j.|.d...|.k.d.f.
+00001710: 3c00 7c08 640b 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
+00001720: 6a02 7c00 6401 1900 7c06 6b02 640b 6602  j.|.d...|.k.d.f.
+00001730: 3c00 7c08 6406 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
+00001740: 6a02 7c00 6401 1900 7c06 6b02 6406 6602  j.|.d...|.k.d.f.
+00001750: 3c00 7c08 640c 1900 6a01 6409 1900 7c00  <.|.d...j.d...|.
+00001760: 6a02 7c00 6401 1900 7c06 6b02 640c 6602  j.|.d...|.k.d.f.
+00001770: 3c00 7168 7c00 5300 2916 4e72 0600 0000  <.qh|.S.).Nr....
+00001780: 720d 0000 00da 0566 6c6f 6174 da08 4c61  r......float..La
+00001790: 6b65 5f43 6174 e902 0000 00da 0653 6567  ke_Cat.......Seg
+000017a0: 5f49 44e7 0000 0000 0000 0000 da09 5269  _ID...........Ri
+000017b0: 764c 656e 6774 6872 0100 0000 7228 0000  vLengthr....r(..
+000017c0: 00da 0853 7472 6168 6c65 72da 0953 6567  ...Strahler..Seg
+000017d0: 5f6f 7264 6572 e9ff ffff ffe7 8d97 6e12  _order........n.
+000017e0: 83c0 f3bf da08 5269 7653 6c6f 7065 da04  ......RivSlope..
+000017f0: 4368 5f6e da07 4d69 6e5f 4445 4dda 074d  Ch_n..Min_DEM..M
+00001800: 6178 5f44 454d da08 466c 6f6f 6450 5f6e  ax_DEM..FloodP_n
+00001810: da08 4441 5f43 686e 5f4c da0a 4441 5f43  ..DA_Chn_L..DA_C
+00001820: 686e 5f53 6c70 290a 7216 0000 0072 1300  hn_Slp).r....r..
+00001830: 0000 7219 0000 0072 1400 0000 da03 6d61  ..r....r......ma
+00001840: 7872 1200 0000 7229 0000 0072 1500 0000  xr....r)...r....
+00001850: da05 7072 696e 7472 1100 0000 290b da07  ..printr....)...
+00001860: 6361 7469 6e66 6fda 0c72 6f75 7469 6e67  catinfo..routing
+00001870: 5f69 6e66 6f5a 1563 6174 696e 666f 5f6e  _infoZ.catinfo_n
+00001880: 6f6e 5f63 6f6e 6e65 6374 6564 5a09 6361  on_connectedZ.ca
+00001890: 7469 6473 5f6e 635a 0a6d 6178 5f73 6567  tids_ncZ.max_seg
+000018a0: 5f69 6472 4800 0000 5a07 635f 7375 6269  _idrH...Z.c_subi
+000018b0: 645a 0764 5f73 7562 6964 5a0a 645f 7375  dZ.d_subidZ.d_su
+000018c0: 625f 696e 666f 5a08 6c63 5f73 7562 6964  b_infoZ.lc_subid
+000018d0: 5a0d 6c63 5f73 7562 6964 5f69 6e66 6f72  Z.lc_subid_infor
+000018e0: 2400 0000 7224 0000 0072 2500 0000 da23  $...r$...r%....#
+000018f0: 7570 6461 7465 5f6e 6f6e 5f63 6f6e 6e65  update_non_conne
+00001900: 6374 6564 5f63 6174 6368 6d65 6e74 5f69  cted_catchment_i
+00001910: 6e66 6f0c 0100 0073 7200 0000 0001 1401  nfo....sr.......
+00001920: 1602 0c01 0c03 02fe 0401 10ff 0204 1401  ................
+00001930: 0e01 0e01 1602 040a 0c01 1601 1e01 1601  ................
+00001940: 0206 1401 1601 0e01 1601 0e01 0401 0401  ................
+00001950: 1401 0a01 0401 0401 0602 0a01 0202 1601  ................
+00001960: 1601 1601 1601 1601 1601 0c01 1601 160c  ................
+00001970: 0201 02ff 0402 02fe 1603 0201 02ff 0402  ................
+00001980: 02fe 1603 0201 02ff 0402 02fe 1804 7278  ..............rx
+00001990: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000019a0: 1000 0000 0600 0000 4300 0000 73be 0100  ........C...s...
+000019b0: 007c 006a 0064 0167 0164 0264 038d 027d  .|.j.d.g.d.d...}
+000019c0: 0174 01a0 0264 0464 05a1 027d 0264 067d  .t...d.d...}.d.}
+000019d0: 0374 01a0 0264 0764 08a1 027d 047c 0164  .t...d.d...}.|.d
+000019e0: 0919 006a 0364 0519 007d 0564 067d 067c  ...j.d...}.d.}.|
+000019f0: 057c 047c 0364 0618 003c 0074 047c 047c  .|.|.d...<.t.|.|
+00001a00: 0464 056b 0419 0083 0164 056b 0490 0172  .d.k.....d.k...r
+00001a10: b274 01a0 0264 0764 08a1 027d 077c 067d  .t...d.d...}.|.}
+00001a20: 0374 0564 057c 0683 0244 0090 015d 2a7d  .t.d.|...D...]*}
+00001a30: 087c 047c 0819 007d 097c 0964 056b 0072  .|.|...}.|.d.k.r
+00001a40: 9271 7a7c 016a 067c 0164 0919 007c 096b  .qz|.j.|.d...|.k
+00001a50: 0264 0a66 0219 007c 027c 0819 0017 007c  .d.f...|.|.....|
+00001a60: 027c 083c 007c 016a 067c 0164 0919 007c  .|.<.|.j.|.d...|
+00001a70: 096b 0264 0b66 0219 006a 0364 0519 007d  .k.d.f...j.d...}
+00001a80: 0a7c 016a 067c 0164 0c19 007c 096b 0219  .|.j.|.d...|.k..
+00001a90: 007d 0b74 047c 0b83 0164 056b 0172 f071  .}.t.|...d.k.r.q
+00001aa0: 7a7c 0b6a 067c 0b64 0b19 007c 0a6b 0219  z|.j.|.d...|.k..
+00001ab0: 007d 0c74 047c 0c83 0164 056b 0490 0172  .}.t.|...d.k...r
+00001ac0: 267c 0c64 0919 006a 0364 0519 007c 077c  &|.d...j.d...|.|
+00001ad0: 083c 0071 7a71 7a7c 0b6a 067c 0b64 0b19  .<.qzqz|.j.|.d..
+00001ae0: 007c 0a64 0618 006b 0219 007d 0d74 0564  .|.d...k...}.t.d
+00001af0: 0574 047c 0d83 0183 0244 005d 5a7d 0e7c  .t.|.....D.]Z}.|
+00001b00: 0e64 056b 0290 0172 6c7c 0d64 0919 006a  .d.k...rl|.d...j
+00001b10: 037c 0e19 007c 077c 083c 006e 367c 0d64  .|...|.|.<.n6|.d
+00001b20: 0919 006a 037c 0e19 007c 077c 0364 0617  ...j.|...|.|.d..
+00001b30: 0064 0618 003c 007c 027c 0819 007c 027c  .d...<.|.|...|.|
+00001b40: 0364 0617 0064 0618 003c 007c 0364 0617  .d...d...<.|.d..
+00001b50: 007d 0390 0171 4a71 7a7c 077d 047c 037d  .}...qJqz|.}.|.}
+00001b60: 0671 4a74 077c 0283 017d 0f7c 0f53 0029  .qJt.|...}.|.S.)
+00001b70: 0d4e da09 4472 6169 6e41 7265 6146 a901  .N..DrainAreaF..
+00001b80: 7239 0000 00e9 6400 0000 7201 0000 0072  r9....d...r....r
+00001b90: 2800 0000 e9e8 0300 0072 6b00 0000 7206  (........rk...r.
+00001ba0: 0000 0072 6800 0000 7269 0000 0072 0d00  ...rh...ri...r..
+00001bb0: 0000 2908 7241 0000 0072 1a00 0000 da04  ..).rA...r......
+00001bc0: 6675 6c6c 7213 0000 0072 1500 0000 7229  fullr....r....r)
+00001bd0: 0000 0072 1900 0000 7274 0000 0029 10da  ...r....rt...)..
+00001be0: 116d 6169 6e72 6976 5f6d 6572 675f 696e  .mainriv_merg_in
+00001bf0: 666f 5a16 6d61 696e 7269 765f 6d65 7267  foZ.mainriv_merg
+00001c00: 5f69 6e66 6f5f 736f 7274 5a13 6c6f 6e67  _info_sortZ.long
+00001c10: 6573 745f 666c 6f77 5f70 6174 6865 735a  est_flow_pathesZ
+00001c20: 056e 7061 7468 5a06 5061 7468 6964 7249  .npathZ.PathidrI
+00001c30: 0000 005a 0d6e 7061 7468 5f63 7572 7265  ...Z.npath_curre
+00001c40: 6e74 5a07 6e50 6174 6869 645a 0569 7061  ntZ.nPathidZ.ipa
+00001c50: 7468 5a0d 635f 7375 6269 645f 6970 6174  thZ.c_subid_ipat
+00001c60: 685a 1453 7472 6168 6c65 725f 6f72 6465  hZ.Strahler_orde
+00001c70: 725f 6970 6174 685a 1275 7073 7472 6561  r_ipathZ.upstrea
+00001c80: 6d5f 7375 625f 696e 666f 735a 1e75 7073  m_sub_infosZ.ups
+00001c90: 7472 6561 6d5f 7375 625f 696e 666f 735f  tream_sub_infos_
+00001ca0: 6571 5f53 7472 6168 6c65 725a 2075 7073  eq_StrahlerZ ups
+00001cb0: 7472 6561 6d5f 7375 625f 696e 666f 735f  tream_sub_infos_
+00001cc0: 6571 5f53 7472 6168 6c65 725f 315a 0669  eq_Strahler_1Z.i
+00001cd0: 6e70 6174 685a 0b4c 6f6e 6765 7374 7061  npathZ.Longestpa
+00001ce0: 7468 7224 0000 0072 2400 0000 7225 0000  thr$...r$...r%..
+00001cf0: 00da 1a43 616c 6375 6c61 7465 5f4c 6f6e  ...Calculate_Lon
+00001d00: 6765 7374 5f66 6c6f 7770 6174 6860 0100  gest_flowpath`..
+00001d10: 0073 7c00 0000 0001 1002 0c02 0403 0c01  .s|.............
+00001d20: 0e01 0401 0c02 1601 0c01 0405 1001 0803  ................
+00001d30: 06ff 0203 0203 0401 0eff 0203 06fd 02ff  ................
+00001d40: 0606 0401 0eff 0402 02fe 0404 0401 0aff  ................
+00001d50: 0405 0aff 0204 0205 0401 0aff 0405 0aff  ................
+00001d60: 0403 0801 02ff 0803 0402 0401 0eff 0404  ................
+00001d70: 1202 0a01 0201 02ff 0402 02fe 0a05 0201  ................
+00001d80: 02ff 0402 02fe 1003 1402 0e02 0401 0601  ................
+00001d90: 0802 727f 0000 0072 2800 0000 6302 0000  ..r....r(...c...
+00001da0: 0000 0000 0000 0000 0021 0000 0008 0000  .........!......
+00001db0: 0043 0000 0073 5805 0000 7c00 6a00 6401  .C...sX...|.j.d.
+00001dc0: 6402 8d01 7d02 6403 7d03 6403 7c00 6a01  d...}.d.}.d.|.j.
+00001dd0: 7601 721e 6404 7d03 7c00 7c00 6405 1900  v.r.d.}.|.|.d...
+00001de0: 6406 1b00 6406 1b00 7c01 6b00 1900 6a00  d...d...|.k...j.
+00001df0: 6401 6402 8d01 7d04 7c04 7c04 6407 1900  d.d...}.|.|.d...
+00001e00: 6408 6b02 1900 6a00 6401 6402 8d01 7d04  d.k...j.d.d...}.
+00001e10: 7c04 7c04 7c03 1900 6408 6b02 1900 6a00  |.|.|...d.k...j.
+00001e20: 6401 6402 8d01 7d04 7c04 6409 1900 6a02  d.d...}.|.d...j.
+00001e30: 7d05 7403 6408 7404 7c04 8301 8302 4400  }.t.d.t.|.....D.
+00001e40: 9004 5dca 7d06 7c04 6409 1900 6a02 7c06  ..].}.|.d...j.|.
+00001e50: 1900 7d07 7c04 640a 1900 6a02 7c06 1900  ..}.|.d...j.|...
+00001e60: 7d08 7c04 640b 1900 6a02 7c06 1900 7d09  }.|.d...j.|...}.
+00001e70: 7404 7c00 7c00 640a 1900 7c07 6b02 1900  t.|.|.d...|.k...
+00001e80: 8301 6408 6b02 7d0a 7c04 6407 1900 6a02  ..d.k.}.|.d...j.
+00001e90: 7c06 1900 6408 6b02 7d0b 7c04 7c03 1900  |...d.k.}.|.|...
+00001ea0: 6a02 7c06 1900 6408 6b01 7d0c 7c00 7c00  j.|...d.k.}.|.|.
+00001eb0: 6409 1900 7c08 6b02 1900 6a00 6401 6402  d...|.k...j.d.d.
+00001ec0: 8d01 7d0d 7c00 7c00 640a 1900 7c07 6b02  ..}.|.|.d...|.k.
+00001ed0: 1900 6a00 6401 6402 8d01 7d0e 7c0e 7c0e  ..j.d.d...}.|.|.
+00001ee0: 640b 1900 7c09 6b02 1900 6a00 6401 6402  d...|.k...j.d.d.
+00001ef0: 8d01 7d0f 7404 7c0d 8301 6408 6b04 9001  ..}.t.|...d.k...
+00001f00: 726c 6401 7d10 7c0d 640b 1900 6a02 6408  rld.}.|.d...j.d.
+00001f10: 1900 7c09 6b02 9001 7266 6401 7d11 6e04  ..|.k...rfd.}.n.
+00001f20: 640c 7d11 6e08 640c 7d10 640c 7d11 7404  d.}.n.d.}.d.}.t.
+00001f30: 7c0e 8301 6408 6b04 9001 72b4 6401 7d12  |...d.k...r.d.}.
+00001f40: 7404 7c0f 8301 6408 6b04 9001 72ae 7c0f  t.|...d.k...r.|.
+00001f50: 7c03 1900 6a02 6408 1900 6408 6b02 9001  |...j.d...d.k...
+00001f60: 72ae 6401 7d13 6e04 640c 7d13 6e08 640c  r.d.}.n.d.}.n.d.
+00001f70: 7d12 640c 7d13 7c10 9002 722c 7c11 9002  }.d.}.|...r,|...
+00001f80: 722c 7c0b 9002 722c 7c0c 9002 722c 7c02  r,|...r,|...r,|.
+00001f90: 7c02 6409 1900 7c0d 6409 1900 6a02 6408  |.d...|.d...j.d.
+00001fa0: 1900 6b02 1900 6a00 6401 6402 8d01 7d14  ..k...j.d.d...}.
+00001fb0: 6401 7d15 7c02 7c02 6409 1900 7c0d 6409  d.}.|.|.d...|.d.
+00001fc0: 1900 6a02 6408 1900 6b02 1900 6a00 6401  ..j.d...k...j.d.
+00001fd0: 6402 8d01 7d16 7c16 640a 1900 6a02 6408  d...}.|.d...j.d.
+00001fe0: 1900 7d17 6ede 7c12 9002 7292 7c13 9002  ..}.n.|...r.|...
+00001ff0: 7292 7c0b 9002 7292 7c0c 9002 7292 7c02  r.|...r.|...r.|.
+00002000: 7c02 6409 1900 7c0f 6409 1900 6a02 6408  |.d...|.d...j.d.
+00002010: 1900 6b02 1900 6a00 6401 6402 8d01 7d14  ..k...j.d.d...}.
+00002020: 6401 7d15 7c02 7c02 6409 1900 7c07 6b02  d.}.|.|.d...|.k.
+00002030: 1900 6a00 6401 6402 8d01 7d18 7c18 640a  ..j.d.d...}.|.d.
+00002040: 1900 6a02 6408 1900 7d17 6e78 7404 7c00  ..j.d...}.nxt.|.
+00002050: 7c00 640b 1900 7c09 6b02 1900 8301 640d  |.d...|.k.....d.
+00002060: 6b02 9003 7200 7c10 9003 7200 7c02 7c02  k...r.|...r.|.|.
+00002070: 6409 1900 7c0d 6409 1900 6a02 6408 1900  d...|.d...j.d...
+00002080: 6b02 1900 6a00 6401 6402 8d01 7d14 6401  k...j.d.d...}.d.
+00002090: 7d15 7c02 7c02 6409 1900 7c08 6b02 1900  }.|.|.d...|.k...
+000020a0: 6a00 6401 6402 8d01 7d16 7c16 640a 1900  j.d.d...}.|.d...
+000020b0: 6a02 6408 1900 7d17 6e0a 640c 7d15 6700  j.d...}.n.d.}.g.
+000020c0: 7d14 7186 7c15 7286 7404 7c00 7c00 640a  }.q.|.r.t.|.|.d.
+000020d0: 1900 7c14 6409 1900 6a02 6408 1900 6b02  ..|.d...j.d...k.
+000020e0: 1900 8301 6408 6b02 7d19 7404 7c00 7c00  ....d.k.}.t.|.|.
+000020f0: 640a 1900 7c14 6409 1900 6a02 6408 1900  d...|.d...j.d...
+00002100: 6b02 7c00 6407 1900 640e 6b00 4000 1900  k.|.d...d.k.@...
+00002110: 8301 640d 6b01 7d1a 7c02 6409 1900 7c07  ..d.k.}.|.d...|.
+00002120: 6b02 7d1b 7c02 640f 1900 7c07 6b02 7d1c  k.}.|.d...|.k.}.
+00002130: 7c02 640f 1900 7c14 640f 1900 6a02 6408  |.d...|.d...j.d.
+00002140: 1900 6b02 7d1d 7405 a006 7c1b 7c1d a102  ..k.}.t...|.|...
+00002150: 7d1e 7405 a006 7c1e 7c1c a102 7d1f 7404  }.t...|.|...}.t.
+00002160: 7c14 8301 640d 6b04 9003 72e6 7404 7405  |...d.k...r.t.t.
+00002170: a007 7c14 6410 1900 6a02 a101 8301 640d  ..|.d...j.....d.
+00002180: 6b04 9003 72e6 7408 7c07 7c09 8302 0100  k...r.t.|.|.....
+00002190: 7408 7c14 6700 6411 a201 1900 8301 0100  t.|.g.d.........
+000021a0: 7c14 6a01 4400 5ddc 7d20 7c20 6405 6b02  |.j.D.].} | d.k.
+000021b0: 9004 722e 7405 a009 7c14 6405 1900 6a02  ..r.t...|.d...j.
+000021c0: 6408 1900 7c02 6a0a 7c1b 6405 6602 1900  d...|.j.|.d.f...
+000021d0: 6a02 6408 1900 1700 a101 7c02 6a0a 7c1f  j.d.......|.j.|.
+000021e0: 7c20 6602 3c00 6e98 7c20 6409 6b02 9004  | f.<.n.| d.k...
+000021f0: 7252 7c14 640f 1900 6a02 6408 1900 7c02  rR|.d...j.d...|.
+00002200: 6a0a 7c1f 640f 6602 3c00 6e74 7c20 640a  j.|.d.f.<.nt| d.
+00002210: 6b02 9004 726c 7c17 7c02 6a0a 7c1f 7c20  k...rl|.|.j.|.| 
+00002220: 6602 3c00 6e5a 7c20 640f 6b02 9003 73ec  f.<.nZ| d.k...s.
+00002230: 7c20 6412 6b02 9003 73ec 7c20 6413 6b02  | d.k...s.| d.k.
+00002240: 9003 73ec 7c20 6414 6b02 9003 73ec 7c20  ..s.| d.k...s.| 
+00002250: 6415 6b02 9003 73ec 7c20 6416 6b02 9004  d.k...s.| d.k...
+00002260: 72ae 9003 71ec 6e18 7c14 7c20 1900 6a02  r...q.n.|.| ..j.
+00002270: 6408 1900 7c02 6a0a 7c1f 7c20 6602 3c00  d...|.j.|.| f.<.
+00002280: 9003 71ec 7c19 9004 73d4 7c0a 7286 7c1a  ..q.|...s.|.r.|.
+00002290: 7286 6417 7c02 6a0a 7c1f 6418 6602 3c00  r.d.|.j.|.d.f.<.
+000022a0: 6417 7c02 6a0a 7c1f 6419 6602 3c00 6417  d.|.j.|.d.f.<.d.
+000022b0: 7c02 6a0a 7c1f 641a 6602 3c00 6417 7c02  |.j.|.d.f.<.d.|.
+000022c0: 6a0a 7c1f 641b 6602 3c00 6417 7c02 6a0a  j.|.d.f.<.d.|.j.
+000022d0: 7c1f 641c 6602 3c00 6417 7c02 6a0a 7c1f  |.d.f.<.d.|.j.|.
+000022e0: 641d 6602 3c00 641e 7c02 6a01 7600 7286  d.f.<.d.|.j.v.r.
+000022f0: 6417 7c02 6a0a 7c1f 641e 6602 3c00 6417  d.|.j.|.d.f.<.d.
+00002300: 7c02 6a0a 7c1f 641f 6602 3c00 7186 7c02  |.j.|.d.f.<.q.|.
+00002310: 5300 2920 4e54 7207 0000 00da 0748 6173  S.) NTr......Has
+00002320: 5f50 4f49 da09 4861 735f 4761 7567 65da  _POI..Has_Gauge.
+00002330: 0742 6173 4172 6561 727c 0000 0072 6400  .BasArear|...rd.
+00002340: 0000 7201 0000 0072 0600 0000 720d 0000  ..r....r....r...
+00002350: 0072 6600 0000 4672 2800 0000 7265 0000  .rf...Fr(...re..
+00002360: 00da 066e 7375 6269 64da 0848 794c 616b  ...nsubid..HyLak
+00002370: 6549 6429 0472 0600 0000 720d 0000 0072  eId).r....r....r
+00002380: 6600 0000 7284 0000 00da 0a6e 646f 776e  f...r......ndown
+00002390: 7375 6269 64da 094f 6c64 5f53 7562 4964  subid..Old_SubId
+000023a0: da0c 4f6c 645f 446f 7753 7562 4964 7258  ..Old_DowSubIdrX
+000023b0: 0000 00da 0867 656f 6d65 7472 7972 6c00  .....geometryrl.
+000023c0: 0000 726d 0000 0072 6800 0000 7271 0000  ..rm...rh...rq..
+000023d0: 0072 6e00 0000 726f 0000 0072 7000 0000  .rn...ro...rp...
+000023e0: 7272 0000 0072 7300 0000 290b 7214 0000  rr...rs...).r...
+000023f0: 0072 1100 0000 7213 0000 0072 2900 0000  .r....r....r)...
+00002400: 7215 0000 0072 1a00 0000 da0a 6c6f 6769  r....r......logi
+00002410: 6361 6c5f 6f72 722b 0000 0072 7500 0000  cal_orr+...ru...
+00002420: 723f 0000 0072 1900 0000 2921 da0e 6d61  r?...r....)!..ma
+00002430: 706f 6c64 6e65 775f 696e 666f da0f 6172  poldnew_info..ar
+00002440: 6561 5f74 6872 6573 7468 6f6c 645a 126d  ea_threstholdZ.m
+00002450: 6170 6f6c 646e 6577 5f69 6e66 6f5f 6e65  apoldnew_info_ne
+00002460: 77da 0e47 6175 6765 5f63 6f6c 5f4e 616d  w..Gauge_col_Nam
+00002470: 655a 1273 6d61 6c6c 5f73 7562 5f6e 6f6e  eZ.small_sub_non
+00002480: 5f6c 616b 655a 1873 6d61 6c6c 5f73 7562  _lakeZ.small_sub
+00002490: 5f6e 6f6e 5f6c 616b 655f 7375 6269 6472  _non_lake_subidr
+000024a0: 4800 0000 5a0c 736d 616c 6c5f 7375 625f  H...Z.small_sub_
+000024b0: 6964 5a10 736d 616c 6c5f 646f 776e 7375  idZ.small_downsu
+000024c0: 625f 6964 5a10 736d 616c 6c5f 7375 625f  b_idZ.small_sub_
+000024d0: 7365 675f 6964 5a1b 736d 616c 6c5f 7375  seg_idZ.small_su
+000024e0: 625f 6973 5f68 6561 645f 7761 7465 725f  b_is_head_water_
+000024f0: 7375 625a 1573 6d61 6c6c 5f73 7562 5f69  subZ.small_sub_i
+00002500: 735f 6e6f 745f 4c61 6b65 5a16 736d 616c  s_not_LakeZ.smal
+00002510: 6c5f 7375 625f 6973 5f6e 6f74 5f67 6175  l_sub_is_not_gau
+00002520: 6765 5a0d 646f 776e 5f73 7562 5f69 6e66  geZ.down_sub_inf
+00002530: 6f5a 1175 7073 7472 6561 6d5f 7375 625f  oZ.upstream_sub_
+00002540: 696e 666f 5a1a 7570 7374 7265 616d 5f73  infoZ.upstream_s
+00002550: 7562 5f69 6e66 6f5f 7361 6d65 5f73 6567  ub_info_same_seg
+00002560: 5a0c 6861 735f 646f 776e 5f73 7562 5a18  Z.has_down_subZ.
+00002570: 646f 776e 5f73 7562 5f68 6173 5f73 616d  down_sub_has_sam
+00002580: 655f 7365 675f 6964 5a0c 6861 735f 7570  e_seg_idZ.has_up
+00002590: 7374 7265 616d 5a16 7570 5f73 7562 5f68  streamZ.up_sub_h
+000025a0: 6173 5f73 616d 655f 7365 675f 6964 da07  as_same_seg_id..
+000025b0: 7461 7269 6e66 6fda 066d 6f64 6966 795a  tarinfo..modifyZ
+000025c0: 0f64 6f77 6e5f 7375 625f 696e 666f 5f32  .down_sub_info_2
+000025d0: 5a0b 6e64 6f77 6e5f 7375 6269 645a 1263  Z.ndown_subidZ.c
+000025e0: 7572 7265 6e74 5f73 7562 5f69 6e66 6f5f  urrent_sub_info_
+000025f0: 325a 1c74 6172 6765 745f 7375 625f 6973  2Z.target_sub_is
+00002600: 5f68 6561 645f 7761 7465 725f 7375 625a  _head_water_subZ
+00002610: 2174 6172 6765 745f 7375 625f 6861 735f  !target_sub_has_
+00002620: 6c65 7373 5f6f 6e65 5f75 705f 7374 7265  less_one_up_stre
+00002630: 616d 724a 0000 005a 056d 6173 6b33 724b  amrJ...Z.mask3rK
+00002640: 0000 005a 086d 6173 6b74 656d 7072 2300  ...Z.masktempr#.
+00002650: 0000 da03 636f 6c72 2400 0000 7224 0000  ....colr$...r$..
+00002660: 0072 2500 0000 da1f 7265 6d6f 7665 5f70  .r%.....remove_p
+00002670: 6f73 7369 626c 655f 736d 616c 6c5f 7375  ossible_small_su
+00002680: 6262 6173 696e 73b8 0100 0073 bc00 0000  bbasins....s....
+00002690: 0001 0c03 0401 0a01 0403 2001 1801 1802  .......... .....
+000026a0: 0a03 1401 0e01 0e01 0e02 1802 1201 1202  ................
+000026b0: 1801 1801 1804 0e01 0401 1401 0602 0602  ................
+000026c0: 0401 0403 0e01 0402 2201 0602 0603 0401  ........".......
+000026d0: 0403 1803 2201 0401 2201 1002 1803 2201  ...."...".....".
+000026e0: 0401 1801 1002 2003 2201 0401 1801 1003  ...... .".......
+000026f0: 0401 0401 0202 0401 2201 2e02 0c01 0c01  ........".......
+00002700: 1601 0c01 0c02 2801 0a01 100c 0a01 0a02  ......(.........
+00002710: 3402 0a02 1a02 0a01 1002 06ff 0402 06fe  4...............
+00002720: 0403 06fd 0404 06fc 0405 06fb 0406 06fa  ................
+00002730: 0408 0602 1c02 0a01 0401 0e01 0e01 0e01  ................
+00002740: 0e01 0e01 0e01 0a01 0e01 100a 7290 0000  ............r...
+00002750: 0072 6b00 0000 6309 0000 0000 0000 0000  .rk...c.........
+00002760: 0000 0016 0000 0005 0000 0043 0000 0073  ...........C...s
+00002770: de04 0000 6401 7d09 7c01 6401 6402 6702  ....d.}.|.d.d.g.
+00002780: 1900 a000 6403 a101 6a01 7d0a 7c04 6404  ....d...j.}.|.d.
+00002790: 6b00 725e 7402 7c0a 7c00 8302 7d0b 7c03  k.r^t.|.|...}.|.
+000027a0: 6404 6b04 7258 7402 7c0a 7c03 8302 7d0c  d.k.rXt.|.|...}.
+000027b0: 7403 a004 7c0b 7c0c a102 7d0d 7c0b 7403  t...|.|...}.|.t.
+000027c0: a005 7c0d a101 1900 7d0e 7162 7c0b 7d0e  ..|.....}.qb|.}.
+000027d0: 6e04 7c05 7d0e 7c01 7c01 7c09 1900 a006  n.|.}.|.|.|.....
+000027e0: 7c0e a101 1900 a007 a100 7d0f 7c01 7c01  |.........}.|.|.
+000027f0: 7c09 1900 7c00 6b02 1900 a007 a100 7d10  |...|.k.......}.
+00002800: 7c06 6a08 7c06 6401 1900 a006 7c0e a101  |.j.|.d.....|...
+00002810: 1900 a007 a100 7d11 7c11 6a08 7c11 6405  ......}.|.j.|.d.
+00002820: 1900 6404 6b04 1900 a007 a100 7d11 7c10  ..d.k.......}.|.
+00002830: 6a09 6404 1900 7d12 740a 7c11 8301 6404  j.d...}.t.|...d.
+00002840: 6b04 9001 72e4 7403 a00b 7c11 6405 1900  k...r.t...|.d...
+00002850: 6a01 a101 7c10 6a08 7c12 6405 6602 3c00  j...|.j.|.d.f.<.
+00002860: 7403 6a0c 7c11 6406 1900 6a01 7c11 6405  t.j.|.d...j.|.d.
+00002870: 1900 6a01 6407 8d02 7c10 6a08 7c12 6406  ..j.d...|.j.|.d.
+00002880: 6602 3c00 7403 6a0c 7c11 6408 1900 6a01  f.<.t.j.|.d...j.
+00002890: 7c11 6405 1900 6a01 6407 8d02 7c10 6a08  |.d...j.d...|.j.
+000028a0: 7c12 6408 6602 3c00 7403 6a0c 7c11 6409  |.d.f.<.t.j.|.d.
+000028b0: 1900 6a01 7c11 6405 1900 6a01 6407 8d02  ..j.|.d...j.d...
+000028c0: 7c10 6a08 7c12 6409 6602 3c00 7403 6a0c  |.j.|.d.f.<.t.j.
+000028d0: 7c11 640a 1900 6a01 7c11 6405 1900 6a01  |.d...j.|.d...j.
+000028e0: 6407 8d02 7c10 6a08 7c12 640a 6602 3c00  d...|.j.|.d.f.<.
+000028f0: 7403 a00d 7c11 640b 1900 6a01 a101 7c10  t...|.d...j...|.
+00002900: 6a08 7c12 640b 6602 3c00 7403 a00d 7c11  j.|.d.f.<.t...|.
+00002910: 640c 1900 6a01 a101 7c10 6a08 7c12 640c  d...j...|.j.|.d.
+00002920: 6602 3c00 7403 a00d 7c11 640d 1900 6a01  f.<.t...|.d...j.
+00002930: a101 7c10 6a08 7c12 640d 6602 3c00 7403  ..|.j.|.d.f.<.t.
+00002940: a00e 7c11 640e 1900 6a01 a101 7c10 6a08  ..|.d...j...|.j.
+00002950: 7c12 640e 6602 3c00 7403 a00b 7c0f 640f  |.d.f.<.t...|.d.
+00002960: 1900 6a01 a101 7c10 6a08 7c12 640f 6602  ..j...|.j.|.d.f.
+00002970: 3c00 740a 7c0f 8301 6404 6b04 9002 7278  <.t.|...d.k...rx
+00002980: 7403 6a0c 7c0f 6410 1900 6a01 7c0f 640f  t.j.|.d...j.|.d.
+00002990: 1900 6a01 6407 8d02 7c10 6a08 7c12 6410  ..j.d...|.j.|.d.
+000029a0: 6602 3c00 7403 6a0c 7c0f 6411 1900 6a01  f.<.t.j.|.d...j.
+000029b0: 7c0f 640f 1900 6a01 6407 8d02 7c10 6a08  |.d...j.d...|.j.
+000029c0: 7c12 6411 6602 3c00 7403 6a0c 7c0f 6412  |.d.f.<.t.j.|.d.
+000029d0: 1900 6a01 7c0f 640f 1900 6a01 6407 8d02  ..j.|.d...j.d...
+000029e0: 7c10 6a08 7c12 6412 6602 3c00 7c07 6413  |.j.|.d.f.<.|.d.
+000029f0: 6b02 9003 7200 6414 7c10 6a08 7c12 6406  k...r.d.|.j.|.d.
+00002a00: 6602 3c00 6414 7c10 6a08 7c12 6405 6602  f.<.d.|.j.|.d.f.
+00002a10: 3c00 6414 7c10 6a08 7c12 6408 6602 3c00  <.d.|.j.|.d.f.<.
+00002a20: 6414 7c10 6a08 7c12 640a 6602 3c00 6414  d.|.j.|.d.f.<.d.
+00002a30: 7c10 6a08 7c12 640e 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
+00002a40: 6a08 7c12 640d 6602 3c00 6415 7c10 6a0f  j.|.d.f.<.d.|.j.
+00002a50: 7600 9003 72f4 6414 7c10 6a08 7c12 6415  v...r.d.|.j.|.d.
+00002a60: 6602 3c00 6414 7c10 6a08 7c12 6416 6602  f.<.d.|.j.|.d.f.
+00002a70: 3c00 6ef4 7c07 6417 6b02 9003 7296 6414  <.n.|.d.k...r.d.
+00002a80: 7c10 6a08 7c12 6406 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
+00002a90: 6a08 7c12 6405 6602 3c00 6414 7c10 6a08  j.|.d.f.<.d.|.j.
+00002aa0: 7c12 6408 6602 3c00 6414 7c10 6a08 7c12  |.d.f.<.d.|.j.|.
+00002ab0: 640a 6602 3c00 6414 7c10 6a08 7c12 640e  d.f.<.d.|.j.|.d.
+00002ac0: 6602 3c00 6414 7c10 6a08 7c12 640d 6602  f.<.d.|.j.|.d.f.
+00002ad0: 3c00 6415 7c10 6a0f 7600 9003 7286 6414  <.d.|.j.v...r.d.
+00002ae0: 7c10 6a08 7c12 6415 6602 3c00 6414 7c10  |.j.|.d.f.<.d.|.
+00002af0: 6a08 7c12 6416 6602 3c00 6417 7c10 6a08  j.|.d.f.<.d.|.j.
+00002b00: 7c12 6418 6602 3c00 6e5e 7c07 6404 6b01  |.d.f.<.n^|.d.k.
+00002b10: 9003 72f4 6404 7c10 6a08 7c12 6419 6602  ..r.d.|.j.|.d.f.
+00002b20: 3c00 6404 7c10 6a08 7c12 641a 6602 3c00  <.d.|.j.|.d.f.<.
+00002b30: 6404 7c10 6a08 7c12 641b 6602 3c00 6404  d.|.j.|.d.f.<.d.
+00002b40: 7c10 6a08 7c12 641c 6602 3c00 6404 7c10  |.j.|.d.f.<.d.|.
+00002b50: 6a08 7c12 641d 6602 3c00 6404 7c10 6a08  j.|.d.f.<.d.|.j.
+00002b60: 7c12 6418 6602 3c00 6414 7c10 6a08 7c12  |.d.f.<.d.|.j.|.
+00002b70: 641e 6602 3c00 6414 7c10 6a08 7c12 641f  d.f.<.d.|.j.|.d.
+00002b80: 6602 3c00 7c08 6404 6b04 9004 7228 7c08  f.<.|.d.k...r(|.
+00002b90: 7c10 6a08 7c12 6420 6602 3c00 7c02 6401  |.j.|.d f.<.|.d.
+00002ba0: 1900 a006 7c0e a101 7d13 7c02 6421 1900  ....|...}.|.d!..
+00002bb0: 7c00 6b02 7d14 7403 a010 7c13 7c14 a102  |.k.}.t...|.|...
+00002bc0: 7d0d 7c10 6a0f 4400 5d84 7d15 7c15 6401  }.|.j.D.].}.|.d.
+00002bd0: 6b02 9004 727c 7c10 7c15 1900 6a01 6404  k...r||.|...j.d.
+00002be0: 1900 7c02 6a08 7c0d 6421 6602 3c00 6e5a  ..|.j.|.d!f.<.nZ
+00002bf0: 7c15 6421 6b02 9004 7354 7c15 6422 6b02  |.d!k...sT|.d"k.
+00002c00: 9004 7354 7c15 6423 6b02 9004 7354 7c15  ..sT|.d#k...sT|.
+00002c10: 6424 6b02 9004 7354 7c15 6425 6b02 9004  d$k...sT|.d%k...
+00002c20: 7354 7c15 6426 6b02 9004 72be 9004 7154  sT|.d&k...r...qT
+00002c30: 6e18 7c10 7c15 1900 6a01 6404 1900 7c02  n.|.|...j.d...|.
+00002c40: 6a08 7c0d 7c15 6602 3c00 9004 7154 7c02  j.|.|.f.<...qT|.
+00002c50: 5300 2927 4e72 0600 0000 720d 0000 0072  S.)'Nr....r....r
+00002c60: 0900 0000 7201 0000 0072 6800 0000 726d  ....r....rh...rm
+00002c70: 0000 00a9 01da 0777 6569 6768 7473 7271  .......weightsrq
+00002c80: 0000 005a 0651 5f4d 6561 6e72 6e00 0000  ...Z.Q_Meanrn...
+00002c90: 5a08 426b 6657 6964 7468 5a08 426b 6644  Z.BkfWidthZ.BkfD
+00002ca0: 6570 7468 7270 0000 0072 6f00 0000 7282  epthrp...ro...r.
+00002cb0: 0000 00da 0842 6173 536c 6f70 655a 084d  .....BasSlopeZ.M
+00002cc0: 6561 6e45 6c65 765a 0942 6173 4173 7065  eanElevZ.BasAspe
+00002cd0: 6374 7228 0000 0072 6c00 0000 7272 0000  ctr(...rl...rr..
+00002ce0: 0072 7300 0000 7265 0000 0072 6400 0000  .rs...re...rd...
+00002cf0: 7284 0000 00da 074c 616b 6556 6f6c da08  r......LakeVol..
+00002d00: 4c61 6b65 4172 6561 da09 4c61 6b65 4465  LakeArea..LakeDe
+00002d10: 7074 68da 084c 616b 6574 7970 65da 0a63  pth..Laketype..c
+00002d20: 656e 7472 6f69 645f 78da 0a63 656e 7472  entroid_x..centr
+00002d30: 6f69 645f 7972 6a00 0000 7283 0000 0072  oid_yrj...r....r
+00002d40: 8500 0000 7286 0000 0072 8700 0000 7258  ....r....r....rX
+00002d50: 0000 0072 8800 0000 2911 7216 0000 0072  ...r....).r....r
+00002d60: 1300 0000 7217 0000 0072 1a00 0000 722e  ....r....r....r.
+00002d70: 0000 00da 0b6c 6f67 6963 616c 5f6e 6f74  .....logical_not
+00002d80: 7212 0000 0072 1400 0000 7219 0000 0072  r....r....r....r
+00002d90: 5900 0000 7215 0000 0072 3f00 0000 da07  Y...r....r?.....
+00002da0: 6176 6572 6167 6572 7400 0000 da03 6d69  averagert.....mi
+00002db0: 6e72 1100 0000 7289 0000 0029 1672 4900  nr....r....).rI.
+00002dc0: 0000 da0d 6361 7463 686d 656e 7469 6e66  ....catchmentinf
+00002dd0: 6f72 8a00 0000 5a07 7570 7375 6269 64da  or....Z.upsubid.
+00002de0: 0a69 736d 6f64 6966 6964 73da 0a6d 6f64  .ismodifids..mod
+00002df0: 6966 6969 6469 6eda 076d 6169 6e72 6976  ifiidin..mainriv
+00002e00: 7264 0000 00da 0973 6567 5f6f 7264 6572  rd.....seg_order
+00002e10: da09 7375 625f 636f 6c6e 6d72 7700 0000  ..sub_colnmrw...
+00002e20: 5a0e 4d6f 6469 6679 5f73 7562 6964 7331  Z.Modify_subids1
+00002e30: 5a0e 4d6f 6469 6679 5f73 7562 6964 7332  Z.Modify_subids2
+00002e40: 7223 0000 005a 0d4d 6f64 6966 795f 7375  r#...Z.Modify_su
+00002e50: 6269 6473 5a07 6362 7261 6e63 6872 8d00  bidsZ.cbranchr..
+00002e60: 0000 727e 0000 0072 5f00 0000 724a 0000  ..r~...r_...rJ..
+00002e70: 0072 4b00 0000 728f 0000 0072 2400 0000  .rK...r....r$...
+00002e80: 7224 0000 0072 2500 0000 da15 4e65 775f  r$...r%.....New_
+00002e90: 5375 6249 645f 546f 5f44 6973 736f 6c76  SubId_To_Dissolv
+00002ea0: 6553 0200 0073 da00 0000 000b 0401 1401  eS...s..........
+00002eb0: 0801 0201 04ff 0403 0801 0a01 0c01 1002  ................
+00002ec0: 0603 0404 1601 0201 0aff 0804 1801 1601  ................
+00002ed0: 0a02 0e01 1a01 0401 0801 08fe 1004 0401  ................
+00002ee0: 0801 08fe 1004 0401 0801 08fe 1004 0401  ................
+00002ef0: 0801 08fe 1004 1a01 1a02 1a01 1a02 1a02  ................
+00002f00: 0e01 0401 10ff 1003 0401 10ff 1003 0401  ................
+00002f10: 10ff 1005 06ff 0404 0e01 0e01 0e01 0e01  ................
+00002f20: 0e01 0e01 0c01 0e01 1002 0a01 0e01 0e01  ................
+00002f30: 0e01 0e01 0e01 0e01 0c01 0e01 0e01 1001  ................
+00002f40: 0a05 0e01 0e01 0e01 0e01 0e01 0e02 0e01  ................
+00002f50: 0e02 0a01 0e02 0801 02ff 0404 0aff 0203  ................
+00002f60: 0c03 0a01 0a02 1a03 06ff 0402 06fe 0403  ................
+00002f70: 06fd 0404 06fc 0405 06fb 0406 06fa 0408  ................
+00002f80: 0602 1c03 72a3 0000 0072 0600 0000 6303  ....r....r....c.
+00002f90: 0000 0000 0000 0000 0000 0008 0000 0004  ................
+00002fa0: 0000 0043 0000 0073 a400 0000 7c00 6a00  ...C...s....|.j.
+00002fb0: 7c01 6a00 6b03 a001 a100 7228 7402 7c00  |.j.k.....r(t.|.
+00002fc0: 6a00 8301 0100 7402 7c01 6a00 8301 0100  j.....t.|.j.....
+00002fd0: 6401 5300 6402 7d03 7c00 6a00 4400 5d62  d.S.d.}.|.j.D.]b
+00002fe0: 7d04 7c04 6403 6b02 7248 7c03 6404 1700  }.|.d.k.rH|.d...
+00002ff0: 7d03 7132 7c00 7c04 1900 6a03 7d05 7c01  }.q2|.|...j.}.|.
+00003000: 7c04 1900 6a03 7d06 7c05 7c06 6b03 a001  |...j.}.|.|.k...
+00003010: a100 728c 7402 7c04 8301 0100 7c05 7c06  ..r.t.|.....|.|.
+00003020: 6b03 7d07 7402 7c00 7c02 1900 6a03 7c07  k.}.t.|.|...j.|.
+00003030: 1900 8301 0100 7132 7c03 6404 1700 7d03  ......q2|.d...}.
+00003040: 7132 7c03 7404 7c00 6a00 8301 6b02 5300  q2|.t.|.j...k.S.
+00003050: 2905 4e46 7201 0000 00da 0648 5255 5f49  ).NFr......HRU_I
+00003060: 4472 2800 0000 2905 7211 0000 00da 0361  Dr(...).r......a
+00003070: 6c6c 7275 0000 0072 1300 0000 7215 0000  llru...r....r...
+00003080: 0029 085a 0845 7870 6563 7465 645a 0652  .).Z.ExpectedZ.R
+00003090: 6573 756c 745a 0c43 6865 636b 5f43 6f6c  esultZ.Check_Col
+000030a0: 5f4e 4d5a 046e 6571 6c72 8f00 0000 5a0c  _NMZ.neqlr....Z.
+000030b0: 4172 7261 795f 6578 7065 6374 5a0c 4172  Array_expectZ.Ar
+000030c0: 7261 795f 7265 7375 6c74 7223 0000 0072  ray_resultr#...r
+000030d0: 2400 0000 7224 0000 0072 2500 0000 da17  $...r$...r%.....
+000030e0: 4576 616c 7561 7465 5f54 776f 5f44 6174  Evaluate_Two_Dat
+000030f0: 6166 7261 6d65 73e7 0200 0073 2200 0000  aframes....s"...
+00003100: 0002 1001 0a01 0a01 0401 0402 0a01 0801  ................
+00003110: 0801 0201 0a01 0a01 0c01 0801 0801 1402  ................
+00003120: 0a02 72a6 0000 0063 0300 0000 0000 0000  ..r....c........
+00003130: 0000 0000 0b00 0000 0500 0000 4300 0000  ............C...
+00003140: 73ac 0100 007c 006a 007d 037c 0264 016b  s....|.j.}.|.d.k
+00003150: 0472 e274 0164 0174 027c 0383 0183 0244  .r.t.d.t.|.....D
+00003160: 005d 8c7d 047c 006a 037c 037c 0419 0064  .].}.|.j.|.|...d
+00003170: 0266 0219 007d 057c 006a 037c 037c 0419  .f...}.|.j.|.|..
+00003180: 0064 0366 0219 007d 067c 006a 037c 037c  .d.f...}.|.j.|.|
+00003190: 0419 0064 0466 0219 007d 077c 006a 037c  ...d.f...}.|.j.|
+000031a0: 0064 0319 007c 076b 0219 00a0 04a1 007d  .d...|.k.......}
+000031b0: 0874 027c 0883 0164 016b 0472 967c 0864  .t.|...d.k.r.|.d
+000031c0: 0219 006a 0564 0119 007c 006a 037c 037c  ...j.d...|.j.|.|
+000031d0: 0419 0064 0566 023c 0071 1c64 067c 006a  ...d.f.<.q.d.|.j
+000031e0: 037c 037c 0419 0064 0566 023c 0071 1c7c  .|.|...d.f.<.q.|
+000031f0: 0064 0319 006a 057c 0064 073c 007c 0064  .d...j.|.d.<.|.d
+00003200: 0419 006a 057c 0064 083c 007c 0064 0219  ...j.|.d.<.|.d..
+00003210: 006a 057c 0064 033c 007c 0064 0519 006a  .j.|.d.<.|.d...j
+00003220: 057c 0064 043c 007c 0164 016b 0072 ee7c  .|.d.<.|.d.k.r.|
+00003230: 0053 007c 006a 0664 0364 0964 0a8d 027d  .S.|.j.d.d.d...}
+00003240: 0974 077c 0983 017d 0974 0164 0174 027c  .t.|...}.t.d.t.|
+00003250: 0983 0183 0244 005d 947d 047c 0964 0319  .....D.].}.|.d..
+00003260: 006a 057c 0419 007d 0a7c 0964 0b19 006a  .j.|...}.|.d...j
+00003270: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
+00003280: 0a6b 0264 0b66 023c 007c 0964 0c19 006a  .k.d.f.<.|.d...j
+00003290: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
+000032a0: 0a6b 0264 0c66 023c 007c 0964 0d19 006a  .k.d.f.<.|.d...j
+000032b0: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
+000032c0: 0a6b 0264 0d66 023c 007c 0964 0e19 006a  .k.d.f.<.|.d...j
+000032d0: 057c 0419 007c 006a 037c 0064 0319 007c  .|...|.j.|.d...|
+000032e0: 0a6b 0264 0e66 023c 0090 0171 127c 0053  .k.d.f.<...q.|.S
+000032f0: 0029 0ffa df46 756e 6374 696f 6e73 2077  .)...Functions w
+00003300: 696c 6c20 7570 6461 7465 2073 7562 6964  ill update subid
+00003310: 2c64 6f77 6e73 7562 6964 2c20 6361 6c63  ,downsubid, calc
+00003320: 7561 7465 2073 7472 6561 6d20 6f72 6465  uate stream orde
+00003330: 7220 616e 640a 2020 2020 2020 2020 7570  r and.        up
+00003340: 6461 7465 2064 7261 696e 6167 6520 6172  date drainage ar
+00003350: 6561 2069 6e20 7468 6520 6174 7472 6962  ea in the attrib
+00003360: 7574 6520 7461 626c 6520 6d61 706f 6c64  ute table mapold
+00003370: 6e65 775f 696e 666f 0a20 2020 202d 2d2d  new_info.    ---
+00003380: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 6f74  -------..    Not
+00003390: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
+000033a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000033b0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000033c0: 206d 6170 6f6c 646e 6577 5f69 6e66 6f0a   mapoldnew_info.
+000033d0: 2020 2020 7201 0000 0072 8300 0000 7206      r....r....r.
+000033e0: 0000 0072 0d00 0000 7285 0000 0072 6b00  ...r....r....rk.
+000033f0: 0000 7286 0000 0072 8700 0000 723a 0000  ..r....r....r:..
+00003400: 00a9 0172 3c00 0000 7269 0000 0072 6600  ...r<...ri...rf.
+00003410: 0000 726a 0000 0072 7900 0000 2908 7259  ..rj...ry...).rY
+00003420: 0000 0072 2900 0000 7215 0000 0072 1900  ...r)...r....r..
+00003430: 0000 7214 0000 0072 1300 0000 7242 0000  ..r....r....rB..
+00003440: 00da 1a73 7472 6561 6d6f 7264 6572 616e  ...streamorderan
+00003450: 6464 7261 696e 6167 6561 7265 6129 0b72  ddrainagearea).r
+00003460: 8a00 0000 da11 5570 6461 7465 5374 7265  ......UpdateStre
+00003470: 616d 6f72 6465 72da 0b55 7064 6174 6553  amorder..UpdateS
+00003480: 7562 4964 725f 0000 0072 4800 0000 7283  ubIdr_...rH...r.
+00003490: 0000 0072 4900 0000 da0a 6f64 6f77 6e73  ...rI.....odowns
+000034a0: 7562 6964 da0c 646f 6e73 7562 6964 696e  ubid..donsubidin
+000034b0: 666f da15 6d61 706f 6c64 6e65 775f 696e  fo..mapoldnew_in
+000034c0: 666f 5f75 6e69 7175 65da 0669 7375 6269  fo_unique..isubi
+000034d0: 6472 2400 0000 7224 0000 0072 2500 0000  dr$...r$...r%...
+000034e0: da0e 5570 6461 7465 546f 706f 6c6f 6779  ..UpdateTopology
+000034f0: ff02 0000 7356 0000 0000 0d06 0208 0112  ....sV..........
+00003500: 0112 0112 0112 0204 010a ff08 040c 0102  ................
+00003510: 0102 ff04 0202 fe14 0414 020e 010e 010e  ................
+00003520: 020e 0208 0104 020e 0208 0212 010e 030c  ................
+00003530: fe04 010e ff02 050c fe04 010e ff02 050c  ................
+00003540: fe04 010e ff02 050c fe04 010e ff06 0472  ...............r
+00003550: b000 0000 6303 0000 0000 0000 0000 0000  ....c...........
+00003560: 0008 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
+00003570: 0000 6401 7c00 6402 1b00 6402 1b00 6403  ..d.|.d...d...d.
+00003580: 1300 1400 7d03 6404 7c01 6402 1b00 1400  ....}.d.|.d.....
+00003590: 7c00 6402 1b00 6402 1b00 6405 1300 1400  |.d...d...d.....
+000035a0: 7c02 6406 1300 1400 7d04 6407 7c01 6402  |.d.....}.d.|.d.
+000035b0: 1b00 6408 1300 1400 7c02 6409 1300 1400  ..d.....|.d.....
+000035c0: 7d05 640a 7c01 6402 1b00 7c02 6403 1300  }.d.|.d...|.d...
+000035d0: 1b00 640b 1300 1400 7d06 640c 7c01 7c02  ..d.....}.d.|.|.
+000035e0: 6403 1300 1b00 640d 1300 1400 7d07 7c03  d.....d.....}.|.
+000035f0: 7c04 7c05 7c06 7c07 6605 5300 290e 4e67  |.|.|.|.f.S.).Ng
+00003600: 9a99 9999 9999 e53f 727c 0000 00e7 0000  .......?r|......
+00003610: 0000 0000 e03f 6793 3a01 4d84 0dcf 3f67  .....?g.:.M...?g
+00003620: 9a99 9999 9999 b9bf 679a 9999 9999 99c9  ........g.......
+00003630: bf67 3333 3333 3333 d33f 6752 b81e 85eb  .g333333.?gR....
+00003640: 51e8 3f67 52b8 1e85 eb51 c8bf 67ab aaaa  Q.?gR....Q..g...
+00003650: aaaa aa12 4067 14ae 47e1 7a14 de3f 67c2  ....@g..G.z..?g.
+00003660: 0fe1 72cf cd41 3f67 48e1 7a14 ae47 e93f  ..r..A?gH.z..G.?
+00003670: 7224 0000 0029 0872 7900 0000 7272 0000  r$...).ry...rr..
+00003680: 0072 7300 0000 5a04 5443 5f31 5a04 5443  .rs...Z.TC_1Z.TC
+00003690: 5f32 5a04 5443 5f33 5a04 5443 5f34 5a04  _2Z.TC_3Z.TC_4Z.
+000036a0: 5443 5f35 7224 0000 0072 2400 0000 7225  TC_5r$...r$...r%
+000036b0: 0000 00da 0c63 616c 6375 6c61 7465 5f54  .....calculate_T
+000036c0: 633d 0300 0073 0c00 0000 0002 1401 2401  c=...s........$.
+000036d0: 1801 1801 1401 72b2 0000 0063 0100 0000  ......r....c....
+000036e0: 0000 0000 0000 0000 1800 0000 0700 0000  ................
+000036f0: 4300 0000 73be 0900 0064 017d 0164 017c  C...s....d.}.d.|
+00003700: 006a 0076 0172 1264 027d 017c 006a 017c  .j.v.r.d.}.|.j.|
+00003710: 0064 0319 0064 046b 0319 00a0 02a1 007d  .d...d.k.......}
+00003720: 027c 006a 017c 0064 0319 0064 046b 0219  .|.j.|.d...d.k..
+00003730: 00a0 02a1 007d 037c 0364 0564 0667 0219  .....}.|.d.d.g..
+00003740: 00a0 0364 07a1 016a 047d 0474 05a0 0674  ...d...j.}.t...t
+00003750: 077c 0283 0164 08a1 027d 0564 097d 0664  .|...d...}.d.}.d
+00003760: 0a7d 0774 0864 0974 077c 0283 0183 0244  .}.t.d.t.|.....D
+00003770: 0090 015d fc7d 087c 026a 097c 0819 007d  ...].}.|.j.|...}
+00003780: 097c 0264 0519 006a 047c 0819 007c 0264  .|.d...j.|...|.d
+00003790: 0619 006a 047c 0819 006b 0272 b264 0b7c  ...j.|...k.r.d.|
+000037a0: 026a 017c 0964 0666 023c 007c 0264 0519  .j.|.d.f.<.|.d..
+000037b0: 006a 047c 0819 007d 0a74 077c 027c 0264  .j.|...}.t.|.|.d
+000037c0: 0619 007c 0a6b 0219 0083 0164 096b 0272  ...|.k.....d.k.r
+000037d0: 7874 0a7c 0264 0619 006a 047c 0819 0083  xt.|.d...j.|....
+000037e0: 017c 057c 063c 0074 077c 0483 0164 096b  .|.|.<.t.|...d.k
+000037f0: 0290 0172 0664 0c7d 0b64 0c7d 0c6e 6274  ...r.d.}.d.}.nbt
+00003800: 0b7c 047c 0a83 027d 0d7c 036a 017c 0364  .|.|...}.|.j.|.d
+00003810: 0519 00a0 0c7c 0da1 0119 00a0 02a1 007d  .....|.........}
+00003820: 0e74 077c 0e83 0164 096b 0490 0172 6074  .t.|...d.k...r`t
+00003830: 0d7c 0e64 0d19 006a 0483 017d 0b74 056a  .|.d...j...}.t.j
+00003840: 0e7c 0e64 0e19 006a 047c 0e64 0d19 006a  .|.d...j.|.d...j
+00003850: 0464 0f8d 027d 0c6e 0864 0c7d 0b64 0c7d  .d...}.n.d.}.d.}
+00003860: 0c7c 0b7c 0264 0d19 006a 047c 0819 0017  .|.|.d...j.|....
+00003870: 007c 026a 017c 0964 1066 023c 0064 0a7c  .|.j.|.d.f.<.d.|
+00003880: 026a 017c 0964 1166 023c 0064 0a7c 026a  .j.|.d.f.<.d.|.j
+00003890: 017c 0964 1266 023c 007c 077c 026a 017c  .|.d.f.<.|.|.j.|
+000038a0: 0964 1366 023c 0064 147c 026a 0076 0090  .d.f.<.d.|.j.v..
+000038b0: 0172 d664 157c 026a 017c 0964 1466 023c  .r.d.|.j.|.d.f.<
+000038c0: 0064 157c 026a 017c 0964 1666 023c 0064  .d.|.j.|.d.f.<.d
+000038d0: 157c 026a 017c 0964 1766 023c 0064 157c  .|.j.|.d.f.<.d.|
+000038e0: 026a 017c 0964 1866 023c 0064 157c 026a  .j.|.d.f.<.d.|.j
+000038f0: 017c 0964 1966 023c 0064 157c 026a 017c  .|.d.f.<.d.|.j.|
+00003900: 0964 1a66 023c 0064 157c 026a 017c 0964  .d.f.<.d.|.j.|.d
+00003910: 1b66 023c 0064 157c 026a 017c 0964 1c66  .f.<.d.|.j.|.d.f
+00003920: 023c 007c 0264 0e19 006a 047c 0819 007c  .<.|.d...j.|...|
+00003930: 0264 0d19 006a 047c 0819 0014 007c 0b7c  .d...j.|.....|.|
+00003940: 0c14 0017 007c 026a 017c 0964 1066 0219  .....|.j.|.d.f..
+00003950: 001b 007c 026a 017c 0964 1d66 023c 007c  ...|.j.|.d.f.<.|
+00003960: 0664 0a17 007d 067c 0764 0a17 007d 0771  .d...}.|.d...}.q
+00003970: 7874 05a0 0f7c 05a1 017d 057c 057c 0564  xt...|...}.|.|.d
+00003980: 096b 0419 007d 0574 05a0 0674 077c 0283  .k...}.t...t.|..
+00003990: 0164 08a1 027d 0f64 097d 1074 0864 0974  .d...}.d.}.t.d.t
+000039a0: 077c 0583 0183 0244 0090 045d a27d 087c  .|.....D...].}.|
+000039b0: 057c 0819 007d 0a64 0a7d 117c 1164 0a6b  .|...}.d.}.|.d.k
+000039c0: 0290 0272 b07c 0a64 096b 0490 0272 b07c  ...r.|.d.k...r.|
+000039d0: 026a 017c 0264 0619 007c 0a6b 0219 00a0  .j.|.d...|.k....
+000039e0: 02a1 007d 127c 026a 017c 0264 0519 007c  ...}.|.j.|.d...|
+000039f0: 0a6b 0219 00a0 02a1 007d 137c 0264 0519  .k.......}.|.d..
+00003a00: 007c 0a6b 027d 1474 077c 0483 0164 096b  .|.k.}.t.|...d.k
+00003a10: 0290 0372 2664 0c7d 0b64 0c7d 0c6e 6274  ...r&d.}.d.}.nbt
+00003a20: 0b7c 047c 0a83 027d 0d7c 036a 017c 0364  .|.|...}.|.j.|.d
+00003a30: 0519 00a0 0c7c 0da1 0119 00a0 02a1 007d  .....|.........}
+00003a40: 0e74 077c 0e83 0164 096b 0490 0372 8074  .t.|...d.k...r.t
+00003a50: 0d7c 0e64 0d19 006a 0483 017d 0b74 056a  .|.d...j...}.t.j
+00003a60: 0e7c 0e64 0e19 006a 047c 0e64 0d19 006a  .|.d...j.|.d...j
+00003a70: 0464 0f8d 027d 0c6e 0864 0c7d 0b64 0c7d  .d...}.n.d.}.d.}
+00003a80: 0c74 077c 1383 0164 096b 0190 0372 9a90  .t.|...d.k...r..
+00003a90: 0271 b074 077c 1283 0164 0a6b 0290 0572  .q.t.|...d.k...r
+00003aa0: 267c 1364 0d19 006a 0464 0919 007c 1264  &|.d...j.d...|.d
+00003ab0: 1019 006a 0464 0919 0017 007c 0b17 007c  ...j.d.....|...|
+00003ac0: 026a 017c 1464 1066 023c 007c 1264 1119  .j.|.d.f.<.|.d..
+00003ad0: 006a 0464 0919 007c 026a 017c 1464 1166  .j.d...|.j.|.d.f
+00003ae0: 023c 007c 1264 1219 006a 0464 0919 0064  .<.|.d...j.d...d
+00003af0: 0a17 007c 026a 017c 1464 1266 023c 007c  ...|.j.|.d.f.<.|
+00003b00: 1264 1319 006a 0464 0919 007c 026a 017c  .d...j.d...|.j.|
+00003b10: 1464 1366 023c 0064 147c 026a 0076 0090  .d.f.<.d.|.j.v..
+00003b20: 0572 1074 05a0 107c 1264 1419 006a 0464  .r.t...|.d...j.d
+00003b30: 0919 0064 09a1 027c 1364 1719 006a 0464  ...d...|.d...j.d
+00003b40: 0919 0017 007c 026a 017c 1464 1466 023c  .....|.j.|.d.f.<
+00003b50: 007c 1364 1819 006a 0464 0919 0074 05a0  .|.d...j.d...t..
+00003b60: 107c 1364 1719 006a 0464 0919 0064 09a1  .|.d...j.d...d..
+00003b70: 0214 007c 1264 1419 006a 0464 0919 0074  ...|.d...j.d...t
+00003b80: 05a0 107c 1264 1619 006a 0464 0919 0064  ...|.d...j.d...d
+00003b90: 09a1 0214 0017 007c 026a 017c 1464 1466  .......|.j.|.d.f
+00003ba0: 0219 001b 007c 026a 017c 1464 1666 023c  .....|.j.|.d.f.<
+00003bb0: 007c 1364 0e19 006a 0464 0919 007c 1364  .|.d...j.d...|.d
+00003bc0: 0d19 006a 0464 0919 0014 007c 0b7c 0c14  ...j.d.....|.|..
+00003bd0: 0017 007c 1264 1d19 006a 0464 0919 007c  ...|.d...j.d...|
+00003be0: 1264 1019 006a 0464 0919 0014 0017 007c  .d...j.d.......|
+00003bf0: 026a 017c 1464 1066 0219 001b 007c 026a  .j.|.d.f.....|.j
+00003c00: 017c 1464 1d66 023c 0074 0a7c 1364 0619  .|.d.f.<.t.|.d..
+00003c10: 006a 0464 0919 0083 017d 0a90 0271 c274  .j.d.....}...q.t
+00003c20: 05a0 117c 1264 1119 006a 04a1 0164 096b  ...|.d...j...d.k
+00003c30: 0490 0772 3664 147c 126a 0076 0090 0572  ...r6d.|.j.v...r
+00003c40: 567c 126a 1264 1464 1e64 1f8d 027d 127c  V|.j.d.d.d...}.|
+00003c50: 1364 0d19 006a 0464 0919 0074 05a0 0d7c  .d...j.d...t...|
+00003c60: 1264 1019 006a 04a1 0117 007c 0b17 007c  .d...j.....|...|
+00003c70: 026a 017c 1464 1066 023c 0064 147c 026a  .j.|.d.f.<.d.|.j
+00003c80: 0076 0090 0672 7474 05a0 107c 1264 1419  .v...rtt...|.d..
+00003c90: 006a 0464 0919 0064 09a1 027c 1364 1719  .j.d...d...|.d..
+00003ca0: 006a 0464 0919 0017 007c 026a 017c 1464  .j.d.....|.j.|.d
+00003cb0: 1466 023c 007c 1364 1819 006a 0464 0919  .f.<.|.d...j.d..
+00003cc0: 0074 05a0 107c 1364 1719 006a 0464 0919  .t...|.d...j.d..
+00003cd0: 0064 09a1 0214 007c 1264 1419 006a 0464  .d.....|.d...j.d
+00003ce0: 0919 0074 05a0 107c 1264 1619 006a 0464  ...t...|.d...j.d
+00003cf0: 0919 0064 09a1 0214 0017 007c 026a 017c  ...d.......|.j.|
+00003d00: 1464 1466 0219 001b 007c 026a 017c 1464  .d.f.....|.j.|.d
+00003d10: 1666 023c 007c 1364 0e19 006a 0464 0919  .f.<.|.d...j.d..
+00003d20: 007c 1364 0d19 006a 0464 0919 0014 007c  .|.d...j.d.....|
+00003d30: 0b7c 0c14 0017 007c 1264 1d19 006a 0464  .|.....|.d...j.d
+00003d40: 0919 007c 1264 1019 006a 0464 0919 0014  ...|.d...j.d....
+00003d50: 0017 007c 026a 017c 1464 1066 0219 001b  ...|.j.|.d.f....
+00003d60: 007c 026a 017c 1464 1d66 023c 0074 05a0  .|.j.|.d.f.<.t..
+00003d70: 117c 1264 1119 006a 04a1 0174 05a0 137c  .|.d...j...t...|
+00003d80: 1264 1119 006a 04a1 016b 0290 0672 dc7c  .d...j...k...r.|
+00003d90: 1264 1119 006a 0464 0919 0064 0a17 007c  .d...j.d...d...|
+00003da0: 026a 017c 1464 1166 023c 0064 0a7c 026a  .j.|.d.f.<.d.|.j
+00003db0: 017c 1464 1266 023c 007c 0764 0a17 007c  .|.d.f.<.|.d...|
+00003dc0: 026a 017c 1464 1366 023c 007c 0764 0a17  .j.|.d.f.<.|.d..
+00003dd0: 007d 076e 4674 05a0 137c 1264 1119 006a  .}.nFt...|.d...j
+00003de0: 04a1 017d 157c 157c 026a 017c 1464 1166  ...}.|.|.j.|.d.f
+00003df0: 023c 0064 0a7c 026a 017c 1464 1266 023c  .<.d.|.j.|.d.f.<
+00003e00: 007c 0764 0a17 007c 026a 017c 1464 1366  .|.d...|.j.|.d.f
+00003e10: 023c 007c 0764 0a17 007d 0774 0a7c 1364  .<.|.d...}.t.|.d
+00003e20: 0619 006a 0464 0919 0083 017d 0a6e 1874  ...j.d.....}.n.t
+00003e30: 0a7c 0a83 017c 0f7c 103c 007c 1064 0a17  .|...|.|.<.|.d..
+00003e40: 007d 1064 097d 1190 0271 c290 0271 b07c  .}.d.}...q...q.|
+00003e50: 0064 0519 00a0 0c7c 0264 0519 006a 04a1  .d.....|.d...j..
+00003e60: 017d 167c 0264 1319 006a 047c 006a 017c  .}.|.d...j.|.j.|
+00003e70: 1664 1366 023c 007c 0264 1219 006a 047c  .d.f.<.|.d...j.|
+00003e80: 006a 017c 1664 1266 023c 007c 0264 1119  .j.|.d.f.<.|.d..
+00003e90: 006a 047c 006a 017c 1664 1166 023c 007c  .j.|.j.|.d.f.<.|
+00003ea0: 0264 1319 006a 047c 006a 017c 1664 1366  .d...j.|.j.|.d.f
+00003eb0: 023c 007c 0264 1019 006a 047c 006a 017c  .<.|.d...j.|.j.|
+00003ec0: 1664 1066 023c 0064 147c 006a 0076 0090  .d.f.<.d.|.j.v..
+00003ed0: 0872 167c 0264 1419 006a 047c 006a 017c  .r.|.d...j.|.j.|
+00003ee0: 1664 1466 023c 007c 0264 1d19 006a 047c  .d.f.<.|.d...j.|
+00003ef0: 006a 017c 1664 1d66 023c 007c 0264 1619  .j.|.d.f.<.|.d..
+00003f00: 006a 047c 006a 017c 1664 1666 023c 007c  .j.|.j.|.d.f.<.|
+00003f10: 0264 1719 006a 047c 006a 017c 1664 1766  .d...j.|.j.|.d.f
+00003f20: 023c 007c 0264 1819 006a 047c 006a 017c  .<.|.d...j.|.j.|
+00003f30: 1664 1866 023c 0074 0864 0974 077c 0083  .d.f.<.t.d.t.|..
+00003f40: 0183 0244 0090 015d 6a7d 087c 006a 097c  ...D...]j}.|.j.|
+00003f50: 0819 007d 097c 007c 0119 006a 047c 0819  ...}.|.|...j.|..
+00003f60: 0064 096b 0490 0872 b27c 0064 2019 006a  .d.k...r.|.d ..j
+00003f70: 047c 0819 0064 096b 0490 0872 b27c 0064  .|...d.k...r.|.d
+00003f80: 1019 006a 047c 0819 0064 211b 0064 211b  ...j.|...d!..d!.
+00003f90: 007c 0064 2019 006a 047c 0819 001b 007c  .|.d ..j.|.....|
+00003fa0: 006a 017c 0964 2266 023c 007c 0064 0319  .j.|.d"f.<.|.d..
+00003fb0: 006a 047c 0819 0064 046b 0290 0872 4c7c  .j.|...d.k...rL|
+00003fc0: 0064 0519 006a 047c 0819 007d 0a74 0b7c  .d...j.|...}.t.|
+00003fd0: 047c 0a83 027d 0d7c 036a 017c 0364 0519  .|...}.|.j.|.d..
+00003fe0: 00a0 0c7c 0da1 0119 006a 0264 2364 248d  ...|.....j.d#d$.
+00003ff0: 017d 0e74 0d7c 0e64 0d19 006a 0483 017d  .}.t.|.d...j...}
+00004000: 177c 177c 006a 017c 0964 1066 023c 0074  .|.|.j.|.d.f.<.t
+00004010: 056a 0e7c 0e64 0e19 006a 047c 0e64 0d19  .j.|.d...j.|.d..
+00004020: 006a 0464 0f8d 027c 006a 017c 0964 1d66  .j.d...|.j.|.d.f
+00004030: 023c 0064 157c 006a 017c 0964 1766 023c  .<.d.|.j.|.d.f.<
+00004040: 0064 157c 006a 017c 0964 1866 023c 0064  .d.|.j.|.d.f.<.d
+00004050: 157c 006a 017c 0964 1966 023c 0064 157c  .|.j.|.d.f.<.d.|
+00004060: 006a 017c 0964 1c66 023c 0064 157c 006a  .j.|.d.f.<.d.|.j
+00004070: 017c 0964 1a66 023c 0064 157c 006a 017c  .|.d.f.<.d.|.j.|
+00004080: 0964 1b66 023c 0064 147c 006a 0076 0090  .d.f.<.d.|.j.v..
+00004090: 0872 4c64 157c 006a 017c 0964 1666 023c  .rLd.|.j.|.d.f.<
+000040a0: 0064 157c 006a 017c 0964 1466 023c 0090  .d.|.j.|.d.f.<..
+000040b0: 0871 4c7c 0053 0029 257a c046 756e 6374  .qL|.S.)%z.Funct
+000040c0: 696f 6e73 2077 696c 6c20 2063 616c 6375  ions will  calcu
+000040d0: 6174 6520 7374 7265 616d 206f 7264 6572  ate stream order
+000040e0: 2061 6e64 0a20 2020 2020 2020 2075 7064   and.        upd
+000040f0: 6174 6520 6472 6169 6e61 6765 2061 7265  ate drainage are
+00004100: 6120 696e 2074 6865 2061 7474 7269 6275  a in the attribu
+00004110: 7465 2074 6162 6c65 2063 6174 696e 666f  te table catinfo
+00004120: 616c 6c0a 2020 2020 2d2d 2d2d 2d2d 2d2d  all.    --------
+00004130: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
+00004140: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
+00004150: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00004160: 2d2d 2d0a 2020 2020 2020 2020 6361 7469  ---.        cati
+00004170: 6e66 6f61 6c6c 0a20 2020 2072 8000 0000  nfoall.    r....
+00004180: 7281 0000 0072 6400 0000 7265 0000 0072  r....rd...re...r
+00004190: 0600 0000 720d 0000 0072 6300 0000 69f7  ....r....rc...i.
+000041a0: ffff ff72 0100 0000 7228 0000 0072 6b00  ...r....r(...rk.
+000041b0: 0000 7267 0000 0072 8200 0000 7293 0000  ..rg...r....r...
+000041c0: 0072 9100 0000 7279 0000 0072 6900 0000  .r....ry...ri...
+000041d0: 726a 0000 0072 6600 0000 7272 0000 0072  rj...rf...rr...r
+000041e0: 6c00 0000 7273 0000 0072 6800 0000 726d  l...rs...rh...rm
+000041f0: 0000 0072 6f00 0000 7271 0000 0072 6e00  ...ro...rq...rn.
+00004200: 0000 7270 0000 005a 0844 415f 536c 6f70  ..rp...Z.DA_Slop
+00004210: 6546 7237 0000 00da 0644 415f 4f62 73e7  eFr7.....DA_Obs.
+00004220: 0000 0000 0040 8f40 da08 4441 5f65 7272  .....@.@..DA_err
+00004230: 6f72 5472 0700 0000 2914 7211 0000 0072  orTr....).r....r
+00004240: 1900 0000 7214 0000 0072 1600 0000 7213  ....r....r....r.
+00004250: 0000 0072 1a00 0000 727d 0000 0072 1500  ...r....r}...r..
+00004260: 0000 7229 0000 0072 5900 0000 722d 0000  ..r)...rY...r-..
+00004270: 0072 1700 0000 7212 0000 0072 3f00 0000  .r....r....r?...
+00004280: 729b 0000 0072 2b00 0000 da07 6d61 7869  r....r+.....maxi
+00004290: 6d75 6d72 9c00 0000 7241 0000 0072 7400  mumr....rA...rt.
+000042a0: 0000 2918 5a0a 6361 7469 6e66 6f61 6c6c  ..).Z.catinfoall
+000042b0: 728c 0000 0072 7600 0000 5a0b 6361 7469  r....rv...Z.cati
+000042c0: 6e66 6f5f 6e63 6c5a 0b72 6f75 7469 6e67  nfo_nclZ.routing
+000042d0: 5f6e 636c 5a07 6361 746c 6973 745a 0469  _nclZ.catlistZ.i
+000042e0: 6361 74da 0469 7365 6772 4800 0000 725f  cat..isegrH...r_
+000042f0: 0000 00da 0563 6174 6964 5a06 4441 5f6e  .....catidZ.DA_n
+00004300: 636c 5a07 736c 705f 6e63 6c5a 0c55 7073  clZ.slp_nclZ.Ups
+00004310: 7472 6561 6d63 6174 735a 0b55 705f 6361  treamcatsZ.Up_ca
+00004320: 745f 696e 666f 5a0a 6e65 7763 6174 6c69  t_infoZ.newcatli
+00004330: 7374 5a09 696e 6577 7374 6172 745a 0b46  stZ.inewstartZ.F
+00004340: 5f69 6e74 6572 7365 6374 5a0f 5570 5f52  _intersectZ.Up_R
+00004350: 6561 6368 6573 5f69 6e66 6f5a 0e63 7572  eaches_infoZ.cur
+00004360: 5f52 6561 6368 5f69 6e66 6f5a 0a63 7572  _Reach_infoZ.cur
+00004370: 6361 745f 6964 785a 0d6d 6178 5f73 7472  cat_idxZ.max_str
+00004380: 616f 7264 6572 7223 0000 005a 0244 4172  aorderr#...Z.DAr
+00004390: 2400 0000 7224 0000 0072 2500 0000 72a9  $...r$...r%...r.
+000043a0: 0000 0047 0300 0073 6001 0000 000c 0401  ...G...s`.......
+000043b0: 0a01 0402 1601 1601 1402 1001 0401 0402  ................
+000043c0: 1401 0a01 1c01 0e01 0e01 1801 1603 0e01  ................
+000043d0: 0401 0602 0a01 0401 0cff 0804 0e01 0e01  ................
+000043e0: 1c02 0401 0402 1c01 0e01 0e01 0e02 0c01  ................
+000043f0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
+00004400: 3c0b 0801 0a02 0a01 0c03 1001 0402 1401  <...............
+00004410: 0801 0402 1401 1601 1601 0c03 0e01 0401  ................
+00004420: 0605 0a01 0401 0cff 0803 0e01 0e01 1c02  ................
+00004430: 0401 0403 0aff 0403 0402 0e02 0c01 0cff  ................
+00004440: 0202 02fe 02ff 0c05 0201 02ff 0402 02fe  ................
+00004450: 0e04 10ff 0c05 1802 0c01 2e02 2201 22ff  ............".".
+00004460: 0202 0cfe 0e04 1a01 06ff 0202 1afe 0203  ................
+00004470: 0cfd 0e10 1602 1602 0c01 0e03 0c01 0eff  ................
+00004480: 0202 02fe 02ff 0c06 0c01 2e02 2201 22ff  ............".".
+00004490: 0202 0cfe 0e05 1a01 06ff 0202 1afe 0203  ................
+000044a0: 0cfd 0e0e 1201 08ff 0804 10ff 0c03 0e01  ................
+000044b0: 1201 0a03 1001 0e01 0e01 1201 0802 1402  ................
+000044c0: 0c01 0801 0c02 1401 1401 1401 1401 1401  ................
+000044d0: 1401 0c01 1401 1401 1401 1401 1409 1401  ................
+000044e0: 0a04 1401 1402 1401 0cfe 0e06 1401 0e02  ................
+000044f0: 0a01 1c01 0e01 0e02 2403 0e01 0e01 0e01  ........$.......
+00004500: 0e01 0e01 0e02 0c01 0e01 120c 72a9 0000  ............r...
+00004510: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
+00004520: 0000 0600 0000 4300 0000 7320 0100 0074  ......C...s ...t
+00004530: 00a0 0164 017c 01a1 027d 0274 00a0 0174  ...d.|...}.t...t
+00004540: 027c 0083 0164 0217 0064 0266 0264 03a1  .|...d...d.f.d..
+00004550: 027d 0364 047d 0474 03a0 037c 00a1 017d  .}.d.}.t...|...}
+00004560: 0574 027c 0283 0164 046b 0490 0172 0674  .t.|...d.k...r.t
+00004570: 00a0 0174 027c 0083 0164 0217 0064 0266  ...t.|...d...d.f
+00004580: 0264 03a1 027d 0664 047d 0774 0464 0474  .d...}.d.}.t.d.t
+00004590: 027c 0283 0183 0244 005d 827d 087c 027c  .|.....D.].}.|.|
+000045a0: 0819 007c 037c 043c 007c 0464 0217 007d  ...|.|.<.|.d...}
+000045b0: 0474 00a0 057c 0564 0564 0585 0264 0266  .t...|.d.d...d.f
+000045c0: 0219 007c 027c 0819 006b 02a1 01a0 0674  ...|.|...k.....t
+000045d0: 07a1 017d 0974 0464 0474 027c 0983 0183  ...}.t.d.t.|....
+000045e0: 0244 005d 367d 0a7c 057c 097c 0a19 0064  .D.]6}.|.|.|...d
+000045f0: 0466 0219 007c 0376 0072 ce71 b47c 057c  .f...|.v.r.q.|.|
+00004600: 097c 0a19 0064 0466 0219 007c 067c 073c  .|...d.f...|.|.<
+00004610: 007c 0764 0217 007d 0771 b471 6a74 00a0  .|.d...}.q.qjt..
+00004620: 087c 06a1 017d 067c 067c 0664 046b 0519  .|...}.|.|.d.k..
+00004630: 007d 0271 3274 00a0 087c 03a1 017d 037c  .}.q2t...|...}.|
+00004640: 037c 0364 046b 0519 007d 037c 0353 0029  .|.d.k...}.|.S.)
+00004650: 067a 9f46 756e 6374 696f 6e73 2077 696c  .z.Functions wil
+00004660: 6c20 7265 7475 726e 2075 7073 7472 6561  l return upstrea
+00004670: 6d20 6964 7320 696e 206f 7574 2074 6168  m ids in out tah
+00004680: 7420 6472 6169 6e61 6765 0a20 2020 2020  t drainage.     
+00004690: 2020 2074 6f20 6f75 746c 6574 6964 0a20     to outletid. 
+000046a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20     ----------.. 
+000046b0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+000046c0: 2d2d 2d2d 0a0a 2020 2020 5265 7475 726e  ----..    Return
+000046d0: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
+000046e0: 2020 2020 2020 2053 6865 6469 640a 2020         Shedid.  
+000046f0: 2020 2902 7228 0000 0072 2800 0000 7228    ).r(...r(...r(
+00004700: 0000 006c fdff ffff ff67 ed10 5d00 7201  ...l.....g..].r.
+00004710: 0000 004e 2909 721a 0000 0072 7d00 0000  ...N).r....r}...
+00004720: 7215 0000 0072 1400 0000 7229 0000 00da  r....r....r)....
+00004730: 0861 7267 7768 6572 6572 1600 0000 722d  .argwherer....r-
+00004740: 0000 0072 2b00 0000 290b da03 6f75 74da  ...r+...)...out.
+00004750: 086f 7574 6c65 7469 645a 076f 7473 6865  .outletidZ.otshe
+00004760: 6473 5a06 5368 6564 6964 5a04 7073 6964  dsZ.ShedidZ.psid
+00004770: da04 726f 7574 5a07 6e6f 7574 7368 645a  ..routZ.noutshdZ
+00004780: 0770 6f73 6864 6964 7248 0000 005a 0469  .poshdidrH...Z.i
+00004790: 726f 7772 5e00 0000 7224 0000 0072 2400  rowr^...r$...r$.
+000047a0: 0000 7225 0000 0072 1700 0000 6104 0000  ..r%...r....a...
+000047b0: 732a 0000 0000 0c0c 0118 0104 010a 010e  s*..............
+000047c0: 0118 0104 0212 030c 0308 0124 0212 0214  ...........$....
+000047d0: 0102 0114 010c 010a 010e 010a 010c 0172  ...............r
+000047e0: 1700 0000 6303 0000 0000 0000 0000 0000  ....c...........
+000047f0: 000d 0000 0006 0000 0043 0000 0073 a601  .........C...s..
+00004800: 0000 7c02 6401 6402 6702 1900 a000 6403  ..|.d.d.g.....d.
+00004810: a101 6a01 7d03 7402 6404 7403 7c02 8301  ..j.}.t.d.t.|...
+00004820: 8302 4400 9001 5d78 7d04 7c02 6401 1900  ..D...]x}.|.d...
+00004830: 6a01 7c04 1900 7d05 7c02 6405 1900 6a01  j.|...}.|.d...j.
+00004840: 7c04 1900 7d06 7c00 6a04 7c00 6406 1900  |...}.|.j.|.d...
+00004850: 7c05 6b02 1900 a005 a100 7d07 7403 7406  |.k.......}.t.t.
+00004860: 7c03 7c05 8302 8301 7c02 6a04 7c02 6401  |.|.....|.j.|.d.
+00004870: 1900 7c05 6b02 6407 6602 3c00 7403 7c07  ..|.k.d.f.<.t.|.
+00004880: 8301 6404 6b01 7288 7122 7c07 6408 1900  ..d.k.r.q"|.d...
+00004890: 6409 6b02 7d08 7c07 6a04 7c08 640a 6602  d.k.}.|.j.|.d.f.
+000048a0: 1900 6a01 6404 1900 7d09 7c09 7c02 6a04  ..j.d...}.|.|.j.
+000048b0: 7c02 6401 1900 7c05 6b02 640b 6602 3c00  |.d...|.k.d.f.<.
+000048c0: 7c02 6402 1900 6a01 7c04 1900 7d0a 7c0a  |.d...j.|...}.|.
+000048d0: 6404 6b00 72d6 7122 7c01 6a04 7c01 6405  d.k.r.q"|.j.|.d.
+000048e0: 1900 7c06 6b02 1900 a005 a100 7d0b 7403  ..|.k.......}.t.
+000048f0: 7c0b 8301 640c 6b02 9001 722a 7c0a 640d  |...d.k...r*|.d.
+00004900: 6b03 9001 722a 7c0b 640a 1900 6a01 6404  k...r*|.d...j.d.
+00004910: 1900 7d0c 7c0c 7c00 6a04 7c00 640a 1900  ..}.|.|.j.|.d...
+00004920: 7c09 6b02 6408 6602 3c00 7122 7c0a 640d  |.k.d.f.<.q"|.d.
+00004930: 6b02 9001 724c 6409 7c00 6a04 7c00 640a  k...rLd.|.j.|.d.
+00004940: 1900 7c09 6b02 6408 6602 3c00 7122 7407  ..|.k.d.f.<.q"t.
+00004950: 640e 8301 0100 7407 640f 7c05 6410 7c0a  d.....t.d.|.d.|.
+00004960: 8304 0100 7407 7c0a 7c06 8302 0100 7407  ....t.|.|.....t.
+00004970: 7c0b 8301 0100 7407 7c09 8301 0100 7407  |.....t.|.....t.
+00004980: 7c01 6405 640a 6702 1900 8301 0100 7407  |.d.d.g.......t.
+00004990: 6411 8301 0100 7407 640e 8301 0100 7122  d.....t.d.....q"
+000049a0: 7c00 7c02 6602 5300 2912 612b 0400 004d  |.|.f.S.).a+...M
+000049b0: 6f64 6966 7920 6f75 746c 6574 2073 7562  odify outlet sub
+000049c0: 6261 7369 6e27 7320 646f 776e 7374 7265  basin's downstre
+000049d0: 616d 2073 7562 6261 7369 6e20 4944 2066  am subbasin ID f
+000049e0: 6f72 2065 6163 6820 7375 6272 6567 696f  or each subregio
+000049f0: 6e0a 2020 2020 5061 7261 6d65 7465 7273  n.    Parameters
+00004a00: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00004a10: 2020 2020 416c 6c43 6174 696e 666f 2020      AllCatinfo  
+00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a30: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004a40: 650a 2020 2020 2020 2020 6974 2069 7320  e.        it is 
+00004a50: 6120 6461 7461 6672 616d 6520 6f66 2074  a dataframe of t
+00004a60: 6865 2061 7474 7269 6275 7465 2074 6162  he attribute tab
+00004a70: 6c65 2072 6561 6465 6420 6672 6f6d 2066  le readed from f
+00004a80: 696e 616c 6361 745f 696e 666f 0a20 2020  inalcat_info.   
+00004a90: 2020 2020 202e 7368 7020 6f72 2066 696e       .shp or fin
+00004aa0: 616c 7269 7670 6c79 5f69 6e66 6f2e 7368  alrivply_info.sh
+00004ab0: 700a 2020 2020 446f 776e 4361 7469 6e66  p.    DownCatinf
+00004ac0: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
+00004ad0: 2020 2020 2020 2020 3a20 6461 7461 6672          : datafr
+00004ae0: 616d 650a 2020 2020 2020 2020 4974 2069  ame.        It i
+00004af0: 7320 6120 6461 7461 6672 616d 6520 696e  s a dataframe in
+00004b00: 636c 7564 6573 2074 776f 2063 6f6c 756d  cludes two colum
+00004b10: 6e73 3a0a 2020 2020 2020 2020 2753 7562  ns:.        'Sub
+00004b20: 5f52 6567 5f49 4427 3a20 7468 6520 7375  _Reg_ID': the su
+00004b30: 6272 6567 696f 6e20 6964 0a20 2020 2020  bregion id.     
+00004b40: 2020 2027 446f 775f 5375 625f 5265 675f     'Dow_Sub_Reg_
+00004b50: 4964 273a 2064 6f77 6e73 7472 6561 6d20  Id': downstream 
+00004b60: 7375 6262 6173 696e 2069 6420 6f66 2074  subbasin id of t
+00004b70: 6865 206f 7574 6c65 7420 7375 6262 6173  he outlet subbas
+00004b80: 696e 2069 6e0a 2020 2020 2020 2020 7468  in in.        th
+00004b90: 6973 2073 7562 7265 6769 6f6e 0a20 2020  is subregion.   
+00004ba0: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 203a 2064 6174 6166 7261 6d65 0a20     : dataframe. 
+00004bd0: 2020 2020 2020 2049 7420 6973 2061 2064         It is a d
+00004be0: 6174 6166 7261 6d65 2069 6e63 6c75 6465  ataframe include
+00004bf0: 7320 7375 6272 6567 696f 6e20 696e 666f  s subregion info
+00004c00: 726d 6174 696f 6e73 2c20 7769 7468 2066  rmations, with f
+00004c10: 6f6c 6c6f 7769 6e67 0a20 2020 2020 2020  ollowing.       
+00004c20: 2063 6f6c 756d 6e73 3a0a 2020 2020 2020   columns:.      
+00004c30: 2020 2753 7562 5f52 6567 5f49 4427 203a    'Sub_Reg_ID' :
+00004c40: 2074 6865 2073 7562 7265 6769 6f6e 2069   the subregion i
+00004c50: 640a 2020 2020 2020 2020 2744 6f77 5f53  d.        'Dow_S
+00004c60: 7562 5f52 6567 5f49 6427 3a20 7468 6520  ub_Reg_Id': the 
+00004c70: 646f 776e 7374 7265 616d 2073 7562 7265  downstream subre
+00004c80: 6769 6f6e 2069 640a 0a20 2020 204e 6f74  gion id..    Not
+00004c90: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
+00004ca0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00004cb0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00004cc0: 2053 7562 5f52 6567 696f 6e5f 696e 666f   Sub_Region_info
+00004cd0: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004ce0: 650a 2020 2020 2020 2020 2020 2020 416e  e.            An
+00004cf0: 206e 6577 2063 6f6c 756d 6e73 2069 6e64   new columns ind
+00004d00: 6963 6174 6520 7468 6520 6f75 746c 6574  icate the outlet
+00004d10: 2073 7562 6261 7369 6e20 6964 206f 6620   subbasin id of 
+00004d20: 7468 6520 7375 6220 7265 6769 6f6e 0a20  the sub region. 
+00004d30: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00004d40: 6265 2061 6464 6564 0a20 2020 2020 2020  be added.       
+00004d50: 2041 6c6c 4361 7469 6e66 6f20 2020 2020   AllCatinfo     
+00004d60: 2020 2020 2020 3a20 6461 7461 6672 616d        : datafram
+00004d70: 650a 2020 2020 2020 2020 2020 2020 446f  e.            Do
+00004d80: 776e 7374 7265 616d 2073 7562 6261 7369  wnstream subbasi
+00004d90: 6e20 4944 206f 6620 6561 6368 2073 7562  n ID of each sub
+00004da0: 7265 6769 6f6e 2773 206f 7574 6c65 7420  region's outlet 
+00004db0: 7375 6262 6173 696e 2077 696c 6c0a 2020  subbasin will.  
+00004dc0: 2020 2020 2020 2020 2020 6265 2075 7064            be upd
+00004dd0: 6174 6564 2e0a 2020 2020 da0a 5375 625f  ated..    ..Sub_
+00004de0: 5265 675f 4944 da0e 446f 775f 5375 625f  Reg_ID..Dow_Sub_
+00004df0: 5265 675f 4964 7263 0000 0072 0100 0000  Reg_Idrc...r....
+00004e00: da07 494c 7074 5f49 44da 0952 6567 696f  ..ILpt_ID..Regio
+00004e10: 6e5f 4944 da0e 4e5f 5570 5f53 7562 5265  n_ID..N_Up_SubRe
+00004e20: 6769 6f6e 720d 0000 0072 6b00 0000 7206  gionr....rk...r.
+00004e30: 0000 00da 0c4f 7574 6c65 745f 5375 6249  .....Outlet_SubI
+00004e40: 6472 2800 0000 e97f 3801 007a 3223 2323  dr(.....8..z2###
+00004e50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004e60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004e70: 2323 2323 2323 2323 2323 2323 2323 237a  ###############z
+00004e80: 0c53 7562 7265 6769 6f6e 203a 207a 0720  .Subregion : z. 
+00004e90: 2020 546f 2020 7a1a 4e65 6564 2062 6520    To  z.Need be 
+00004ea0: 6d61 6e75 616c 6c79 2063 6f6e 6e65 6374  manually connect
+00004eb0: 6564 2908 7216 0000 0072 1300 0000 7229  ed).r....r....r)
+00004ec0: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
+00004ed0: 0000 7217 0000 0072 7500 0000 290d da0a  ..r....ru...)...
+00004ee0: 416c 6c43 6174 696e 666f 5a0b 446f 776e  AllCatinfoZ.Down
+00004ef0: 4361 7469 6e66 6fda 0f53 7562 5f52 6567  Catinfo..Sub_Reg
+00004f00: 696f 6e5f 696e 666f 7277 0000 0072 4800  ion_inforw...rH.
+00004f10: 0000 5a0a 6973 7562 7265 6769 6f6e 72bf  ..Z.isubregionr.
+00004f20: 0000 005a 1353 7562 5f52 6567 696f 6e5f  ...Z.Sub_Region_
+00004f30: 6361 745f 696e 666f 5a0b 6f75 746c 6574  cat_infoZ.outlet
+00004f40: 5f6d 6173 6b5a 1169 5265 675f 4f75 746c  _maskZ.iReg_Outl
+00004f50: 6574 5f53 7562 6964 5a11 446f 775f 5375  et_SubidZ.Dow_Su
+00004f60: 625f 5265 6769 6f6e 5f69 64da 0d44 6f77  b_Region_id..Dow
+00004f70: 6e5f 5375 625f 696e 666f 5a09 446f 776e  n_Sub_infoZ.Down
+00004f80: 5375 6269 6472 2400 0000 7224 0000 0072  Subidr$...r$...r
+00004f90: 2500 0000 da22 436f 6e6e 6563 745f 5375  %...."Connect_Su
+00004fa0: 6252 6567 696f 6e5f 5570 6461 7465 5f44  bRegion_Update_D
+00004fb0: 6f77 6e53 7562 4964 8b04 0000 7352 0000  ownSubId....sR..
+00004fc0: 0000 2312 ff02 0314 030e 020e 0204 010a  ..#.............
+00004fd0: ff08 060c fe04 010e ff02 050c 0102 030c  ................
+00004fe0: 0114 0402 fe04 010e ff02 040e 0408 0102  ................
+00004ff0: 0316 0218 010e 0302 fe04 010e ff04 060a  ................
+00005000: 0118 0208 010e 010a 0108 0108 0110 0108  ................
+00005010: 010a 0172 c700 0000 6304 0000 0000 0000  ...r....c.......
+00005020: 0000 0000 0019 0000 000a 0000 0043 0000  .............C..
+00005030: 0073 0605 0000 7c01 7c01 6401 1900 6402  .s....|.|.d...d.
+00005040: 6b02 1900 6403 1900 6a00 7d04 7401 a002  k...d...j.}.t...
+00005050: 7c04 a101 7d04 7c04 a003 a100 7d04 7404  |...}.|.....}.t.
+00005060: 7c00 6a05 7c00 6404 1900 6405 6b02 1900  |.j.|.d...d.k...
+00005070: 8301 6402 6b04 7264 7406 6406 8301 0100  ..d.k.rdt.d.....
+00005080: 7406 7c00 6a05 7c00 6404 1900 6405 6b02  t.|.j.|.d...d.k.
+00005090: 1900 8301 0100 7c00 5300 7404 7c00 6a05  ......|.S.t.|.j.
+000050a0: 7c00 6404 1900 6405 6b02 1900 8301 6407  |.d...d.k.....d.
+000050b0: 6b02 728a 7406 6408 8301 0100 7c00 5300  k.r.t.d.....|.S.
+000050c0: 7c00 6a05 7c00 6404 1900 6405 6b02 1900  |.j.|.d...d.k...
+000050d0: 6409 1900 6a00 6407 1900 a007 7408 a101  d...j.d.....t...
+000050e0: 7d05 640a 7d06 7409 6407 7404 7c01 8301  }.d.}.t.d.t.|...
+000050f0: 8302 4400 5d94 7d07 7c01 640b 1900 6a00  ..D.].}.|.d...j.
+00005100: 7c07 1900 7d08 7c06 7c00 6a05 7c00 6409  |...}.|.|.j.|.d.
+00005110: 1900 7c08 6b02 1900 640c 1900 6a00 6407  ..|.k...d...j.d.
+00005120: 1900 1700 7d06 7406 640d 7c01 6403 1900  ....}.t.d.|.d...
+00005130: 6a00 7c07 1900 8302 0100 7406 640e 7c00  j.|.......t.d.|.
+00005140: 6a05 7c00 6409 1900 7c08 6b02 1900 640c  j.|.d...|.k...d.
+00005150: 1900 6a00 6407 1900 8302 0100 7406 640f  ..j.d.......t.d.
+00005160: 740a 7c00 6a05 7c00 6410 1900 7c01 6403  t.|.j.|.d...|.d.
+00005170: 1900 6a00 7c07 1900 6b02 1900 6411 1900  ..j.|...k...d...
+00005180: 6a00 8301 8302 0100 71be 6402 7d09 7404  j.......q.d.}.t.
+00005190: 7c04 8301 6407 6b04 9004 72b6 7406 6412  |...d.k...r.t.d.
+000051a0: 7c09 8302 0100 7406 7c04 8301 0100 740b  |.....t.|.....t.
+000051b0: a00b 7c04 a101 7d0a 6700 7d04 7409 6407  ..|...}.g.}.t.d.
+000051c0: 7404 7c0a 8301 8302 4400 9003 5d06 7d07  t.|.....D...].}.
+000051d0: 7c0a 7c07 1900 7d0b 7c0b 6413 6b02 9001  |.|...}.|.d.k...
+000051e0: 72b0 9001 7194 7c01 7c01 6403 1900 7c0b  r...q.|.|.d...|.
+000051f0: 6b02 1900 6414 1900 6a00 6407 1900 7d0c  k...d...j.d...}.
+00005200: 7c04 a00c 7c0c a101 0100 7c01 7c01 6403  |...|.....|.|.d.
+00005210: 1900 7c0b 6b02 1900 640b 1900 6a00 6407  ..|.k...d...j.d.
+00005220: 1900 7d08 7c00 6a05 7c00 6409 1900 7c08  ..}.|.j.|.d...|.
+00005230: 6b02 1900 a00b a100 7d0d 7c0d 6404 1900  k.......}.|.d...
+00005240: 6a00 6407 1900 7d0e 7404 7c00 6a05 7c00  j.d...}.t.|.j.|.
+00005250: 6409 1900 7c0e 6b02 1900 8301 6407 6b01  d...|.k.....d.k.
+00005260: 9002 726c 7408 7c0b 8301 7408 7c05 8301  ..rlt.|...t.|...
+00005270: 6b03 9001 7294 7406 6415 7c0b 8302 0100  k...r.t.d.|.....
+00005280: 7406 6416 7c08 6417 7c0e 7c05 7408 7c0b  t.d.|.d.|.|.t.|.
+00005290: 8301 7408 7c05 8301 6b03 8306 0100 9001  ..t.|...k.......
+000052a0: 7194 7c00 6a05 7c00 6409 1900 7c0e 6b02  q.|.j.|.d...|.k.
+000052b0: 1900 6410 1900 6a00 6407 1900 7d0f 7406  ..d...j.d...}.t.
+000052c0: 6415 7c0b 7c0f 7c0c 7c0e 8305 0100 7c0f  d.|.|.|.|.....|.
+000052d0: 7c0c 6b03 9002 72b4 7406 6415 7c0b 6418  |.k...r.t.d.|.d.
+000052e0: 7c0c 8304 0100 9001 7194 7c0f 7c0c 6b02  |.......q.|.|.k.
+000052f0: 9001 7294 7c0e 7d10 7406 6415 7c0b 7c0f  ..r.|.}.t.d.|.|.
+00005300: 7c0c 7c0e 7c10 8306 0100 7c00 6a05 7c00  |.|.|.....|.j.|.
+00005310: 6409 1900 7c10 6b02 1900 a00b a100 7d11  d...|.k.......}.
+00005320: 7c00 6a05 7c00 6404 1900 7c10 6b02 1900  |.j.|.d...|.k...
+00005330: a00b a100 7d12 7c11 6411 1900 6a00 6407  ....}.|.d...j.d.
+00005340: 1900 740a 7c12 640c 1900 6a00 8301 1700  ..t.|.d...j.....
+00005350: 7d13 7c12 6419 1900 6a00 7d14 740d 7c14  }.|.d...j.}.t.|.
+00005360: 8301 7d15 7401 a00a 7c14 7c15 6b02 a101  ..}.t...|.|.k...
+00005370: 641a 6b05 9003 724c 7c15 6402 1700 7d16  d.k...rL|.d...}.
+00005380: 6e04 7c15 7d16 7c16 7c00 6a05 7c00 6409  n.|.}.|.|.j.|.d.
+00005390: 1900 7c10 6b02 6419 6602 3c00 7c13 7c00  ..|.k.d.f.<.|.|.
+000053a0: 6a05 7c00 6409 1900 7c10 6b02 640c 6602  j.|.d...|.k.d.f.
+000053b0: 3c00 7c00 7c00 6409 1900 7c10 6b02 1900  <.|.|.d...|.k...
+000053c0: 641b 1900 6a00 6407 1900 6407 6b04 9004  d...j.d...d.k...
+000053d0: 7212 7c00 7c00 6409 1900 7c10 6b02 1900  r.|.|.d...|.k...
+000053e0: 641b 1900 6a00 6407 1900 7d17 7c00 7c00  d...j.d...}.|.|.
+000053f0: 6409 1900 7c10 6b02 1900 640c 1900 6a00  d...|.k...d...j.
+00005400: 6407 1900 641c 1b00 641c 1b00 7d18 7c17  d...d...d...}.|.
+00005410: 6407 6b04 9004 7212 7c18 7c17 1b00 7c00  d.k...r.|.|...|.
+00005420: 6a05 7c00 6409 1900 7c10 6b02 641d 6602  j.|.d...|.k.d.f.
+00005430: 3c00 6402 7c00 6a05 7c00 6409 1900 7c10  <.d.|.j.|.d...|.
+00005440: 6b02 641e 6602 3c00 7c11 6404 1900 6a00  k.d.f.<.|.d...j.
+00005450: 6407 1900 7d0e 7404 7c00 6a05 7c00 6409  d...}.t.|.j.|.d.
+00005460: 1900 7c0e 6b02 1900 8301 6407 6b01 9004  ..|.k.....d.k...
+00005470: 727a 7408 7c10 8301 7408 7c05 8301 6b03  rzt.|...t.|...k.
+00005480: 9004 729a 7406 6415 7c0c 8302 0100 7406  ..r.t.d.|.....t.
+00005490: 6416 7c10 6417 7c0e 7c05 7408 7c10 8301  d.|.d.|.|.t.|...
+000054a0: 7408 7c05 8301 6b03 8306 0100 9001 7194  t.|...k.......q.
+000054b0: 7c00 6a05 7c00 6409 1900 7c0e 6b02 1900  |.j.|.d...|.k...
+000054c0: 6410 1900 6a00 6407 1900 7d0f 9002 71b4  d...j.d...}...q.
+000054d0: 9001 7194 740e 740f 7c04 8301 8301 7d04  ..q.t.t.|.....}.
+000054e0: 7c09 6402 1700 7d09 9001 7158 7406 641f  |.d...}...qXt.d.
+000054f0: 8301 0100 7406 6420 740a 7c00 6411 1900  ....t.d t.|.d...
+00005500: 6a00 8301 8302 0100 7406 6421 7c00 6a05  j.......t.d!|.j.
+00005510: 7c00 6409 1900 7408 7c05 8301 6b02 1900  |.d...t.|...k...
+00005520: 640c 1900 6a00 6407 1900 8302 0100 7406  d...j.d.......t.
+00005530: 6422 7c06 8302 0100 7c00 5300 2923 6115  d"|.....|.S.)#a.
+00005540: 0300 0055 7064 6174 6520 4472 6169 6e61  ...Update Draina
+00005550: 6765 2061 7265 612c 2073 7472 6168 6c65  ge area, strahle
+00005560: 7220 6f72 6465 7220 6f66 2073 7562 6261  r order of subba
+00005570: 696e 730a 0a20 2020 2055 7064 6174 6520  ins..    Update 
+00005580: 6472 6169 6e61 6765 2061 7265 6120 616e  drainage area an
+00005590: 6420 7374 7261 686c 6572 206f 7264 6572  d strahler order
+000055a0: 2066 6f72 2063 6f6d 6269 6e65 6420 726f   for combined ro
+000055b0: 7574 696e 6720 7072 6f64 7563 740a 2020  uting product.  
+000055c0: 2020 6f66 2065 6163 6820 7375 6272 6567    of each subreg
+000055d0: 696f 6e73 0a20 2020 2050 6172 616d 6574  ions.    Paramet
+000055e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000055f0: 2d2d 0a20 2020 2041 6c6c 4361 7469 6e66  --.    AllCatinf
+00005600: 6f20 2020 2020 2020 2020 2020 2020 2020  o               
+00005610: 2020 2020 2020 2020 203a 2064 6174 6166           : dataf
+00005620: 7261 6d65 0a20 2020 2020 2020 2069 7420  rame.        it 
+00005630: 6973 2061 2064 6174 6166 7261 6d65 206f  is a dataframe o
+00005640: 6620 7468 6520 6174 7472 6962 7574 6520  f the attribute 
+00005650: 7461 626c 6520 7265 6164 6564 2066 726f  table readed fro
+00005660: 6d20 6669 6e61 6c63 6174 5f69 6e66 6f0a  m finalcat_info.
+00005670: 2020 2020 2020 2020 2e73 6870 206f 7220          .shp or 
+00005680: 6669 6e61 6c72 6976 706c 795f 696e 666f  finalrivply_info
+00005690: 2e73 6870 0a20 2020 2053 7562 5f52 6567  .shp.    Sub_Reg
+000056a0: 696f 6e5f 696e 666f 2020 2020 2020 2020  ion_info        
+000056b0: 2020 2020 2020 2020 2020 203a 2064 6174             : dat
+000056c0: 6166 7261 6d65 0a20 2020 2020 2020 2049  aframe.        I
+000056d0: 7420 6973 2061 2064 6174 6166 7261 6d65  t is a dataframe
+000056e0: 2069 6e63 6c75 6465 7320 7375 6272 6567   includes subreg
+000056f0: 696f 6e20 696e 666f 726d 6174 696f 6e73  ion informations
+00005700: 2c20 7769 7468 2066 6f6c 6c6f 7769 6e67  , with following
+00005710: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+00005720: 3a0a 2020 2020 2020 2020 2753 7562 5f52  :.        'Sub_R
+00005730: 6567 5f49 4427 203a 2074 6865 2073 7562  eg_ID' : the sub
+00005740: 7265 6769 6f6e 2069 640a 2020 2020 2020  region id.      
+00005750: 2020 2744 6f77 5f53 7562 5f52 6567 5f49    'Dow_Sub_Reg_I
+00005760: 6427 3a20 7468 6520 646f 776e 7374 7265  d': the downstre
+00005770: 616d 2073 7562 7265 6769 6f6e 2069 640a  am subregion id.
+00005780: 0a20 2020 204e 6f74 6573 0a20 2020 202d  .    Notes.    -
+00005790: 2d2d 2d2d 2d2d 0a0a 2020 2020 5265 7475  ------..    Retu
+000057a0: 726e 733a 0a20 2020 202d 2d2d 2d2d 2d2d  rns:.    -------
+000057b0: 0a20 2020 2041 6c6c 4361 7469 6e66 6f20  .    AllCatinfo 
+000057c0: 2020 2020 2020 2020 2020 3a20 6461 7461            : data
+000057d0: 6672 616d 650a 2020 2020 2020 2020 446f  frame.        Do
+000057e0: 776e 7374 7265 616d 2044 4120 616e 6420  wnstream DA and 
+000057f0: 7374 7261 686c 6572 206f 7264 6572 206f  strahler order o
+00005800: 6620 6561 6368 2073 7562 7265 6769 6f6e  f each subregion
+00005810: 2061 6c6f 6e67 2074 6865 2066 6c6f 770a   along the flow.
+00005820: 2020 2020 2020 2020 7061 7468 7761 7920          pathway 
+00005830: 6265 7477 6565 6e20 7375 6272 6567 696f  between subregio
+00005840: 6e73 2077 696c 6c20 6265 2075 7064 6174  ns will be updat
+00005850: 6564 2e0a 2020 2020 72c1 0000 0072 2800  ed..    r....r(.
+00005860: 0000 72bd 0000 0072 0d00 0000 726b 0000  ..r....r....rk..
+00005870: 007a 1f57 6174 6865 7273 6564 2068 6173  .z.Wathersed has
+00005880: 206d 756c 7469 706c 6520 6f75 746c 6574   multiple outlet
+00005890: 2020 7201 0000 007a 1757 6174 6572 7368    r....z.Watersh
+000058a0: 6564 2068 6173 206e 6f20 6f75 746c 6574  ed has no outlet
+000058b0: 7206 0000 0072 6700 0000 72c2 0000 0072  r....rg...r....r
+000058c0: 7900 0000 7a26 2323 2323 2323 4172 6561  y...z&######Area
+000058d0: 2061 6e64 2044 4120 6368 6563 6b20 666f   and DA check fo
+000058e0: 7220 7375 6272 6567 696f 6e20 7a21 4441  r subregion z!DA
+000058f0: 2061 7420 7468 6520 7375 6272 6567 696f   at the subregio
+00005900: 6e20 6f75 746c 6574 2069 7320 2020 207a  n outlet is    z
+00005910: 2154 6f74 616c 2073 7562 7265 6769 6f6e  !Total subregion
+00005920: 2061 7265 6120 6973 2020 2020 2020 2020   area is        
+00005930: 2020 72c0 0000 0072 8200 0000 7a06 6c6f    r....r....z.lo
+00005940: 6f70 2020 72c3 0000 0072 be00 0000 7a0d  op  r....r....z.
+00005950: 5375 6272 6567 696f 6e3a 2020 207a 0953  Subregion:   z.S
+00005960: 7562 4964 2069 7320 7a0f 2044 6f77 6e53  ubId is z. DownS
+00005970: 7562 4964 2069 7320 207a 1c20 2064 6964  ubId is  z.  did
+00005980: 206e 6f74 2063 6f6e 6e65 6374 6564 2077   not connected w
+00005990: 6974 6820 2020 2072 6900 0000 7265 0000  ith    ri...re..
+000059a0: 0072 b300 0000 72b4 0000 0072 b500 0000  .r....r....r....
+000059b0: 5a0a 5573 655f 7265 6769 6f6e 7a14 4368  Z.Use_regionz.Ch
+000059c0: 6563 6b20 6472 6169 6e61 6765 2061 7265  eck drainage are
+000059d0: 613a 7a21 546f 7461 6c20 6261 7369 6e20  a:z!Total basin 
+000059e0: 6172 6561 2069 7320 2020 2020 2020 2020  area is         
+000059f0: 2020 2020 207a 2144 4120 6f66 2074 6865       z!DA of the
+00005a00: 2077 6174 6572 7365 6864 206f 7574 6c65   watersehd outle
+00005a10: 7420 6973 2020 2020 7a21 546f 7461 6c20  t is    z!Total 
+00005a20: 4441 206f 6620 6561 6368 2073 7562 7265  DA of each subre
+00005a30: 6769 6f6e 2020 2020 2020 2029 1072 1300  gion       ).r..
+00005a40: 0000 721a 0000 0072 2b00 0000 da06 746f  ..r....r+.....to
+00005a50: 6c69 7374 7215 0000 0072 1900 0000 7275  listr....r....ru
+00005a60: 0000 0072 1600 0000 722d 0000 0072 2900  ...r....r-...r).
+00005a70: 0000 723f 0000 0072 1400 0000 724e 0000  ..r?...r....rN..
+00005a80: 0072 7400 0000 7254 0000 00da 0373 6574  .rt...rT.....set
+00005a90: 2919 72c4 0000 0072 c500 0000 7261 0000  ).r....r....ra..
+00005aa0: 00da 0163 5a0e 5375 6272 6567 696f 6e5f  ...cZ.Subregion_
+00005ab0: 6c69 7374 5a14 5761 7465 7273 6865 646f  listZ.Watershedo
+00005ac0: 7574 6c65 7473 7562 6964 5a12 546f 7461  utletsubidZ.Tota
+00005ad0: 6c5f 4441 5f53 7562 7265 6769 6f6e 7248  l_DA_SubregionrH
+00005ae0: 0000 005a 114f 7574 6c65 7473 7562 6964  ...Z.Outletsubid
+00005af0: 5f63 7375 6272 5a05 696c 6f6f 705a 1163  _csubrZ.iloopZ.c
+00005b00: 7572 7265 6e74 5f6c 6f6f 705f 6c69 7374  urrent_loop_list
+00005b10: 5a09 635f 7375 6272 5f69 645a 0964 5f73  Z.c_subr_idZ.d_s
+00005b20: 7562 725f 6964 5a0e 4f75 746c 6574 7375  ubr_idZ.Outletsu
+00005b30: 625f 696e 666f da09 646f 776e 7375 6269  b_info..downsubi
+00005b40: 645a 0e64 6f77 6e73 7562 5f72 6567 5f69  dZ.downsub_reg_i
+00005b50: 64da 0663 7375 6269 645a 0a43 5f73 7562  d..csubidZ.C_sub
+00005b60: 5f69 6e66 6f5a 0e55 7070 6572 5f73 7562  _infoZ.Upper_sub
+00005b70: 5f69 6e66 6f5a 054e 6577 4441 5a09 5374  _infoZ.NewDAZ.St
+00005b80: 7261 686c 6572 735a 0b6d 6178 5374 7261  rahlersZ.maxStra
+00005b90: 686c 6572 5a0b 6e65 7753 7472 6168 6c65  hlerZ.newStrahle
+00005ba0: 725a 0664 615f 6f62 735a 0664 615f 7369  rZ.da_obsZ.da_si
+00005bb0: 6d72 2400 0000 7224 0000 0072 2500 0000  mr$...r$...r%...
+00005bc0: da26 5570 6461 7465 5f44 415f 5374 7261  .&Update_DA_Stra
+00005bd0: 686c 6572 5f46 6f72 5f43 6f6d 6269 6e65  hler_For_Combine
+00005be0: 645f 5265 7375 6c74 eb04 0000 731e 0100  d_Result....s...
+00005bf0: 0000 1a0e 0102 ff06 030a 0108 051a 0108  ................
+00005c00: 0116 0104 011a 0108 0104 0320 ff02 0504  ........... ....
+00005c10: 0112 010e 0202 011a ff02 ff02 0402 0102  ................
+00005c20: 010c fe04 0402 0102 011a fe04 0402 0102  ................
+00005c30: 0102 0104 0114 ff02 0202 fe04 ff02 fe06  ................
+00005c40: 0904 010e 010a 0108 010a 0104 0214 0208  ................
+00005c50: 020a 0104 020e 0102 ff04 0202 fe04 040a  ................
+00005c60: 0302 010a ff02 0202 fe04 0202 fe04 0404  ................
+00005c70: 010a ff08 040e 031c 0112 010a 0102 0102  ................
+00005c80: 0102 0102 0102 0102 010e fa04 0804 0210  ................
+00005c90: 0102 ff04 0202 fe04 0410 020a 0102 0102  ................
+00005ca0: 0102 0102 0102 fc04 0604 020a 0104 0112  ................
+00005cb0: 0216 0216 040e 0108 ff06 060a 0108 0114  ................
+00005cc0: 010a 0204 0216 0116 0220 011a 0122 010a  ......... ..."..
+00005cd0: 011a 0116 150e 031c 0112 010a 0102 0102  ................
+00005ce0: 0102 0102 0102 0102 010e fa04 0804 0210  ................
+00005cf0: 0102 ff04 0202 fe0c 050c 010c 0308 0114  ................
+00005d00: 0102 0102 011a 0102 ff02 fe04 060a 0172  ...............r
+00005d10: cd00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00005d20: 0012 0000 0008 0000 0043 0000 0073 e002  .........C...s..
+00005d30: 0000 6401 7d01 6402 7d02 6403 7d03 7400  ..d.}.d.}.d.}.t.
+00005d40: 7c00 7c01 1900 6a01 8301 7d04 7402 7c00  |.|...j...}.t.|.
+00005d50: 8301 7d05 6404 7d06 7403 a004 7c05 6405  ..}.d.}.t...|.d.
+00005d60: 1700 7403 6a05 a102 7d07 7403 a004 7c05  ..t.j...}.t...|.
+00005d70: 6405 1700 7403 6a05 a102 7d08 7406 6406  d...t.j...}.t.d.
+00005d80: 7402 7c00 8301 8302 4400 9001 5d6a 7d09  t.|.....D...]j}.
+00005d90: 7c00 7c01 1900 6a01 7c09 1900 7d0a 7c00  |.|...j.|...}.|.
+00005da0: 7c03 1900 6a01 7c09 1900 7d0b 7c00 7c02  |...j.|...}.|.|.
+00005db0: 1900 6a01 7c09 1900 7d0c 7a0c 7407 7c0a  ..j.|...}.z.t.|.
+00005dc0: 8301 7d0d 5700 6e1e 0100 0100 0100 6407  ..}.W.n.......d.
+00005dd0: 7d0d 6407 7c00 6a08 7c09 7c01 6602 3c00  }.d.|.j.|.|.f.<.
+00005de0: 5900 6e02 3000 7a0c 7407 7c0b 8301 7d0e  Y.n.0.z.t.|...}.
+00005df0: 5700 6e1e 0100 0100 0100 6407 7d0e 6407  W.n.......d.}.d.
+00005e00: 7c00 6a08 7c09 7c03 6602 3c00 5900 6e02  |.j.|.|.f.<.Y.n.
+00005e10: 3000 7a0c 7407 7c0c 8301 7d0f 5700 6e1e  0.z.t.|...}.W.n.
+00005e20: 0100 0100 0100 6407 7d0f 6407 7c00 6a08  ......d.}.d.|.j.
+00005e30: 7c09 7c02 6602 3c00 5900 6e02 3000 7c0d  |.|.f.<.Y.n.0.|.
+00005e40: 6406 6b00 9001 7218 7158 7c0f 6406 6b01  d.k...r.qX|.d.k.
+00005e50: 9001 7234 7c0d 7d10 6407 7c00 6a08 7c09  ..r4|.}.d.|.j.|.
+00005e60: 6408 6602 3c00 7c0f 6406 6b04 9001 727a  d.f.<.|.d.k...rz
+00005e70: 7c0e 7c0f 6b02 9001 7264 7c0d 7c04 1700  |.|.k...rd|.|...
+00005e80: 6409 1700 7d10 6404 7c00 6a08 7c09 6408  d...}.d.|.j.|.d.
+00005e90: 6602 3c00 6e16 7407 7c0d 8301 7d10 6407  f.<.n.t.|...}.d.
+00005ea0: 7c00 6a08 7c09 6408 6602 3c00 7c10 7c08  |.j.|.d.f.<.|.|.
+00005eb0: 7601 9001 72a4 7c06 7c00 6a08 7c09 640a  v...r.|.|.j.|.d.
+00005ec0: 6602 3c00 7c10 7c08 7c06 3c00 7c06 6404  f.<.|.|.|.<.|.d.
+00005ed0: 1700 7d06 7158 7409 7403 a00a 7c08 7c10  ..}.qXt.t...|.|.
+00005ee0: 6b02 a101 6406 1900 8301 7c00 6a08 7c09  k...d.....|.j.|.
+00005ef0: 640a 6602 3c00 7158 7406 6406 7402 7c00  d.f.<.qXt.d.t.|.
+00005f00: 8301 8302 4400 9001 5d04 7d09 7c00 7c01  ....D...].}.|.|.
+00005f10: 1900 6a01 7c09 1900 7d0d 7c00 7c03 1900  ..j.|...}.|.|...
+00005f20: 6a01 7c09 1900 7d0e 7c00 7c02 1900 6a01  j.|...}.|.|...j.
+00005f30: 7c09 1900 7d0f 7c0d 6406 6b04 9002 7212  |...}.|.d.k...r.
+00005f40: 9001 71d4 7c0e 6406 6b01 9002 723e 740b  ..q.|.d.k...r>t.
+00005f50: 640b 8301 0100 740b 7c00 6a08 7c09 640c  d.....t.|.j.|.d.
+00005f60: 640c 8502 6602 1900 8301 0100 9001 71d4  d...f.........q.
+00005f70: 7c00 6a08 7c00 7c03 1900 7c0e 6b02 7c00  |.j.|.|...|.k.|.
+00005f80: 6408 1900 6406 6b04 4000 1900 7d11 7402  d...d.k.@...}.t.
+00005f90: 7c11 8301 6406 6b01 9002 7278 740b 640d  |...d.k...rxt.d.
+00005fa0: 7c0e 8302 0100 9001 71d4 7c11 7c01 1900  |.......q.|.|...
+00005fb0: 6a01 6406 1900 7c00 6a08 7c09 7c01 6602  j.d...|.j.|.|.f.
+00005fc0: 3c00 7c11 6408 1900 6a01 6406 1900 7c00  <.|.d...j.d...|.
+00005fd0: 6a08 7c09 6408 6602 3c00 7c11 640a 1900  j.|.d.f.<.|.d...
+00005fe0: 6a01 6406 1900 7c00 6a08 7c09 640a 6602  j.d...|.j.|.d.f.
+00005ff0: 3c00 7c11 7c02 1900 6a01 6406 1900 7c00  <.|.|...j.d...|.
+00006000: 6a08 7c09 7c02 6602 3c00 9001 71d4 7c00  j.|.|.f.<...q.|.
+00006010: 5300 290e 7aa1 4675 6e63 7469 6f6e 2074  S.).z.Function t
+00006020: 6f20 6465 7465 726d 696e 2068 7275 6964  o determin hruid
+00006030: 2061 6674 6572 2063 6f6d 6269 6e65 206c   after combine l
+00006040: 616b 6520 706f 6c79 676f 6e0a 2020 2020  ake polygon.    
+00006050: 616e 6420 7375 6262 6173 696e 2070 6f6c  and subbasin pol
+00006060: 7967 6f6e 0a20 2020 202d 2d2d 2d2d 2d2d  ygon.    -------
+00006070: 2d2d 2d0a 0a20 2020 204e 6f74 6573 0a20  ---..    Notes. 
+00006080: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
+00006090: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
+000060a0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+000060b0: 652c 0a20 2020 2072 0600 0000 7284 0000  e,.    r....r...
+000060c0: 00da 0848 796c 616b 5f69 6472 2800 0000  ...Hylak_idr(...
+000060d0: 727b 0000 0072 0100 0000 726b 0000 0072  r{...r....rk...r
+000060e0: 4d00 0000 e90a 0000 00da 0a48 5255 4c61  M..........HRULa
+000060f0: 6b65 5f49 447a 1a6c 616b 6520 6861 7320  ke_IDz.lake has 
+00006100: 756e 6578 7065 6374 6564 2068 6f6c 6573  unexpected holes
+00006110: 204e 7a16 4c61 6b65 6964 2064 6f20 6e6f   Nz.Lakeid do no
+00006120: 7420 6578 6973 7420 2020 290c 7274 0000  t exist   ).rt..
+00006130: 0072 1300 0000 7215 0000 0072 1a00 0000  .r....r....r....
+00006140: 727d 0000 00da 036e 616e 7229 0000 0072  r}.....nanr)...r
+00006150: 6300 0000 7219 0000 0072 2d00 0000 72b9  c...r....r-...r.
+00006160: 0000 0072 7500 0000 2912 5a0f 4174 7472  ...ru...).Z.Attr
+00006170: 6962 7574 655f 5461 626c 65da 0653 7562  ibute_Table..Sub
+00006180: 5f49 44da 0b53 7562 5f4c 616b 655f 4944  _ID..Sub_Lake_ID
+00006190: da07 4c61 6b65 5f49 645a 0f6d 6178 5f73  ..Lake_IdZ.max_s
+000061a0: 7562 6261 7369 6e5f 6964 5a0e 4e5f 6e65  ubbasin_idZ.N_ne
+000061b0: 775f 6665 6174 7572 6573 5a09 6e65 775f  w_featuresZ.new_
+000061c0: 6872 7569 645a 0e6e 6577 5f68 7275 6964  hruidZ.new_hruid
+000061d0: 5f6c 6973 745a 116f 6c64 5f6e 6577 6872  _listZ.old_newhr
+000061e0: 7569 645f 6c69 7374 7248 0000 005a 0c73  uid_listrH...Z.s
+000061f0: 7562 6964 5f73 665f 6f62 6a5a 116c 616b  ubid_sf_objZ.lak
+00006200: 656c 616b 6569 645f 7366 5f6f 626a 5a11  elakeid_sf_objZ.
+00006210: 5375 625f 4c61 6b65 6964 5f73 665f 6f62  Sub_Lakeid_sf_ob
+00006220: 6a5a 0873 7562 6964 5f73 665a 0d6c 616b  jZ.subid_sfZ.lak
+00006230: 656c 616b 6569 645f 7366 5a0d 5375 625f  elakeid_sfZ.Sub_
+00006240: 4c61 6b65 6964 5f73 665a 0d6f 6c64 5f6e  Lakeid_sfZ.old_n
+00006250: 6577 5f68 7275 6964 5a08 7461 725f 696e  ew_hruidZ.tar_in
+00006260: 666f 7224 0000 0072 2400 0000 7225 0000  for$...r$...r%..
+00006270: 00da 1544 6574 6572 6d69 6e65 5f4c 616b  ...Determine_Lak
+00006280: 655f 4852 555f 4964 c805 0000 7390 0000  e_HRU_Id....s...
+00006290: 0000 0d04 0104 0104 030e 0208 0104 0112  ................
+000062a0: 0112 0b14 010e 010e 010e 0402 010c 0106  ................
+000062b0: 0104 010e 0106 0202 010c 0106 0104 010e  ................
+000062c0: 0106 0202 010c 0106 0104 010e 0106 040a  ................
+000062d0: 0102 030a 0104 010e 020a 0206 ff04 030c  ................
+000062e0: 0110 0208 010e 030a 010e 0108 010a 0302  ................
+000062f0: 0110 ff10 0814 010e 010e 010e 010a 0104  ................
+00006300: 010a 0108 0116 0104 0204 010a 010a ff02  ................
+00006310: ff04 040e 010a 0104 0118 0118 0118 011c  ................
+00006320: 0272 d500 0000 6304 0000 0000 0000 0000  .r....c.........
+00006330: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+00006340: 8a00 0000 7c00 6a00 7c00 7c02 1900 6401  ....|.j.|.|...d.
+00006350: 6b03 1900 7d04 7401 7c04 8301 6401 6b04  k...}.t.|...d.k.
+00006360: 722e 7c04 7c02 1900 6a02 6401 1900 7d05  r.|.|...j.d...}.
+00006370: 6e58 7c01 6a00 7c01 7c02 1900 6401 6b03  nX|.j.|.|...d.k.
+00006380: 1900 7d01 7c01 6a03 6402 6403 6404 8d02  ..}.|.j.d.d.d...
+00006390: 7d01 7401 7c01 8301 6401 6b04 726a 7c01  }.t.|...d.k.rj|.
+000063a0: 7c02 1900 6a02 6401 1900 7d05 6e1c 7c03  |...j.d...}.n.|.
+000063b0: 6a00 7c03 7c02 1900 6401 6b03 1900 7c02  j.|.|...d.k...|.
+000063c0: 1900 6a02 6401 1900 7d05 7c05 5300 2905  ..j.d...}.|.S.).
+000063d0: 4e72 0100 0000 7233 0000 0046 7237 0000  Nr....r3...Fr7..
+000063e0: 0029 0472 1900 0000 7215 0000 0072 1300  .).r....r....r..
+000063f0: 0000 7241 0000 0029 06da 1641 7474 7269  ..rA...)...Attri
+00006400: 5f74 6162 6c65 5f4c 616b 655f 4852 555f  _table_Lake_HRU_
+00006410: 69da 0753 7562 496e 666f da06 436f 6c5f  i..SubInfo..Col_
+00006420: 4e4d 5a09 696e 666f 5f64 6174 615a 0d69  NMZ.info_dataZ.i
+00006430: 6e66 6f5f 6c61 6b65 5f68 7275 5a0b 5570  nfo_lake_hruZ.Up
+00006440: 6461 7465 7661 6c75 6572 2400 0000 7224  datevaluer$...r$
+00006450: 0000 0072 2500 0000 da1f 5265 7472 756e  ...r%.....Retrun
+00006460: 5f56 616c 6964 6174 655f 4174 7472 6962  _Validate_Attrib
+00006470: 7574 655f 5661 6c75 6543 0600 0073 1400  ute_ValueC...s..
+00006480: 0000 0002 1202 0aff 0203 1002 1201 0e01  ................
+00006490: 0c01 1002 1c03 72d9 0000 0063 0a00 0000  ......r....c....
+000064a0: 0000 0000 0000 0000 1a00 0000 0700 0000  ................
+000064b0: 4300 0000 735e 0400 007c 007c 0119 0064  C...s^...|.|...d
+000064c0: 016b 017d 0a7c 007c 0219 0064 016b 017c  .k.}.|.|...d.k.|
+000064d0: 007c 0219 0064 026b 0340 007d 0b7c 007c  .|...d.k.@.}.|.|
+000064e0: 0319 0064 016b 017c 007c 0319 0064 026b  ...d.k.|.|...d.k
+000064f0: 0340 007d 0c7c 007c 0419 0064 016b 017c  .@.}.|.|...d.k.|
+00006500: 007c 0419 0064 026b 0340 007d 0d7c 007c  .|...d.k.@.}.|.|
+00006510: 0619 0064 016b 017c 007c 0619 0064 026b  ...d.k.|.|...d.k
+00006520: 0340 007d 0e7c 0a7c 0b42 007c 0c42 007c  .@.}.|.|.B.|.B.|
+00006530: 0d42 007c 0e42 007d 0f74 00a0 017c 006a  .B.|.B.}.t...|.j
+00006540: 027c 0f64 0366 0219 006a 03a1 017d 107c  .|.d.f...j...}.|
+00006550: 107c 1064 016b 0419 007d 1074 0464 0174  .|.d.k...}.t.d.t
+00006560: 057c 1083 0183 0244 0090 025d f27d 117c  .|.....D...].}.|
+00006570: 107c 1119 007d 127c 1264 016b 0272 c871  .|...}.|.d.k.r.q
+00006580: b07c 006a 027c 0064 0319 007c 126b 0219  .|.j.|.d...|.k..
+00006590: 007d 137c 136a 0664 0464 0564 068d 027d  .}.|.j.d.d.d...}
+000065a0: 137c 1364 0719 006a 0364 0119 007d 147c  .|.d...j.d...}.|
+000065b0: 006a 027c 0064 0719 007c 146b 0219 007d  .j.|.d...|.k...}
+000065c0: 1574 0464 0174 057c 1383 0183 0244 0090  .t.d.t.|.....D..
+000065d0: 025d 8a7d 167c 1364 0819 006a 037c 1619  .].}.|.d...j.|..
+000065e0: 007d 177c 1364 0919 006a 037c 1619 007d  .}.|.d...j.|...}
+000065f0: 187c 1864 016b 0490 0272 887c 137c 0319  .|.d.k...r.|.|..
+00006600: 006a 0364 0119 0064 016b 0290 0172 7c74  .j.d...d.k...r|t
+00006610: 077c 137c 157c 037c 0883 047d 197c 197c  .|.|.|.|...}.|.|
+00006620: 006a 027c 0064 0819 007c 176b 027c 0366  .j.|.d...|.k.|.f
+00006630: 023c 006e 207c 137c 0319 006a 0364 0119  .<.n |.|...j.d..
+00006640: 007c 006a 027c 0064 0819 007c 176b 027c  .|.j.|.d...|.k.|
+00006650: 0366 023c 007c 137c 0519 006a 0364 0119  .f.<.|.|...j.d..
+00006660: 0064 016b 0290 0172 d674 077c 137c 157c  .d.k...r.t.|.|.|
+00006670: 057c 0083 047d 197c 197c 006a 027c 0064  .|...}.|.|.j.|.d
+00006680: 0819 007c 176b 027c 0566 023c 006e 207c  ...|.k.|.f.<.n |
+00006690: 137c 0519 006a 0364 0119 007c 006a 027c  .|...j.d...|.j.|
+000066a0: 0064 0819 007c 176b 027c 0566 023c 007c  .d...|.k.|.f.<.|
+000066b0: 137c 0619 006a 0364 0119 0064 016b 0290  .|...j.d...d.k..
+000066c0: 0272 3074 077c 137c 157c 067c 0083 047d  .r0t.|.|.|.|...}
+000066d0: 197c 197c 006a 027c 0064 0819 007c 176b  .|.|.j.|.d...|.k
+000066e0: 027c 0666 023c 006e 207c 137c 0619 006a  .|.f.<.n |.|...j
+000066f0: 0364 0119 007c 006a 027c 0064 0819 007c  .d...|.j.|.d...|
+00006700: 176b 027c 0666 023c 0074 0864 0283 017c  .k.|.f.<.t.d...|
+00006710: 006a 027c 0064 0819 007c 176b 027c 0266  .j.|.d...|.k.|.f
+00006720: 023c 0074 0864 0283 017c 006a 027c 0064  .<.t.d...|.j.|.d
+00006730: 0819 007c 176b 027c 0466 023c 0090 0171  ...|.k.|.f.<...q
+00006740: 167c 137c 0319 006a 037c 1619 0064 016b  .|.|...j.|...d.k
+00006750: 0290 0272 c074 077c 137c 157c 037c 0883  ...r.t.|.|.|.|..
+00006760: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
+00006770: 176b 027c 0366 023c 007c 137c 0219 006a  .k.|.f.<.|.|...j
+00006780: 037c 1619 0064 016b 0290 0272 f874 077c  .|...d.k...r.t.|
+00006790: 137c 157c 027c 0783 047d 197c 197c 006a  .|.|.|...}.|.|.j
+000067a0: 027c 0064 0819 007c 176b 027c 0266 023c  .|.d...|.k.|.f.<
+000067b0: 007c 137c 0419 006a 037c 1619 0064 016b  .|.|...j.|...d.k
+000067c0: 0290 0372 3074 077c 137c 157c 047c 0983  ...r0t.|.|.|.|..
+000067d0: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
+000067e0: 176b 027c 0466 023c 007c 137c 0519 006a  .k.|.f.<.|.|...j
+000067f0: 037c 1619 0064 016b 0290 0372 6874 077c  .|...d.k...rht.|
+00006800: 137c 157c 057c 0083 047d 197c 197c 006a  .|.|.|...}.|.|.j
+00006810: 027c 0064 0819 007c 176b 027c 0566 023c  .|.d...|.k.|.f.<
+00006820: 007c 137c 0619 006a 037c 1619 0064 016b  .|.|...j.|...d.k
+00006830: 0290 0172 1674 077c 137c 157c 067c 0083  ...r.t.|.|.|.|..
+00006840: 047d 197c 197c 006a 027c 0064 0819 007c  .}.|.|.j.|.d...|
+00006850: 176b 027c 0666 023c 0090 0171 1671 b07c  .k.|.f.<...q.q.|
+00006860: 006a 0967 0064 0aa2 0164 0b8d 017d 0074  .j.g.d...d...}.t
+00006870: 0a6a 0b7c 007c 0764 0c7c 0264 0d8d 046a  .j.|.|.d.|.d...j
+00006880: 0c64 0e64 0f8d 017d 0074 0a6a 0b7c 007c  .d.d...}.t.j.|.|
+00006890: 0864 0c7c 0364 0d8d 046a 0c64 0e64 0f8d  .d.|.d...j.d.d..
+000068a0: 017d 0074 0a6a 0b7c 007c 0964 0c7c 0464  .}.t.j.|.|.d.|.d
+000068b0: 0d8d 046a 0c64 0e64 0f8d 017d 007c 0064  ...j.d.d...}.|.d
+000068c0: 0319 00a0 0d74 0ea1 017c 007c 0219 00a0  .....t...|.|....
+000068d0: 0d74 0ea1 0117 007c 007c 0319 00a0 0d74  .t.....|.|.....t
+000068e0: 0ea1 0117 007c 007c 0519 00a0 0d74 0ea1  .....|.|.....t..
+000068f0: 0117 007c 0064 103c 0074 0aa0 0f7c 0064  ...|.d.<.t...|.d
+00006900: 1019 00a1 0164 0119 0064 1117 007c 0064  .....d...d...|.d
+00006910: 123c 007c 0053 0029 137a ab46 756e 6374  .<.|.S.).z.Funct
+00006920: 696f 6e20 746f 2064 6574 6572 6d69 6e65  ion to determine
+00006930: 206c 616e 6475 7365 2c73 6f69 6c2c 616e   landuse,soil,an
+00006940: 6420 7665 6720 616e 6420 6f74 6865 7220  d veg and other 
+00006950: 7072 6f70 6572 7469 6573 2061 6674 6572  properties after
+00006960: 2075 6e69 6f6e 2061 6c6c 2070 6f6c 7967   union all polyg
+00006970: 6f6e 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ons.    --------
+00006980: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
+00006990: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
+000069a0: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+000069b0: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+000069c0: 2c0a 2020 2020 7201 0000 0072 6b00 0000  ,.    r....rk...
+000069d0: 72d0 0000 0072 3300 0000 4672 3700 0000  r....r3...Fr7...
+000069e0: 7206 0000 0072 a400 0000 724d 0000 0029  r....r....rM...)
+000069f0: 035a 0a4c 414e 445f 5553 455f 435a 0556  .Z.LAND_USE_CZ.V
+00006a00: 4547 5f43 5a09 534f 494c 5f50 524f 4672  EG_CZ.SOIL_PROFr
+00006a10: 1000 0000 da05 696e 6e65 7229 0272 0c00  ......inner).r..
+00006a20: 0000 720b 0000 0054 7207 0000 00da 0766  ..r....Tr......f
+00006a30: 6163 7465 7273 7228 0000 0072 5700 0000  actersr(...rW...
+00006a40: 2910 721a 0000 0072 2b00 0000 7219 0000  ).r....r+...r...
+00006a50: 0072 1300 0000 7229 0000 0072 1500 0000  .r....r)...r....
+00006a60: 7241 0000 0072 d900 0000 722d 0000 0072  rA...r....r-...r
+00006a70: 1c00 0000 7240 0000 0072 1800 0000 7214  ....r@...r....r.
+00006a80: 0000 0072 1600 0000 da03 7374 72da 0966  ...r......str..f
+00006a90: 6163 746f 7269 7a65 291a 5a0b 4174 7472  actorize).Z.Attr
+00006aa0: 695f 7461 626c 6572 d200 0000 7247 0000  i_tabler....rG..
+00006ab0: 0072 5000 0000 7251 0000 0072 5200 0000  .rP...rQ...rR...
+00006ac0: 7253 0000 005a 114c 616e 6475 7365 5f69  rS...Z.Landuse_i
+00006ad0: 6e66 6f5f 6461 7461 5a0e 536f 696c 5f69  nfo_dataZ.Soil_i
+00006ae0: 6e66 6f5f 6461 7461 5a0d 5665 675f 696e  nfo_dataZ.Veg_in
+00006af0: 666f 5f64 6174 615a 0969 6e76 616c 5f73  fo_dataZ.inval_s
+00006b00: 7562 5a0d 696e 7661 6c5f 6c61 6e64 7573  ubZ.inval_landus
+00006b10: 655a 0a69 6e76 616c 5f73 6f69 6c5a 0969  eZ.inval_soilZ.i
+00006b20: 6e76 616c 5f76 6567 5a08 696e 7661 6c5f  nval_vegZ.inval_
+00006b30: 6f32 5a0a 696e 7661 6c5f 726f 7773 5a0c  o2Z.inval_rowsZ.
+00006b40: 4c61 6b65 5f48 5255 5f49 4453 7248 0000  Lake_HRU_IDSrH..
+00006b50: 005a 0c69 6c61 6b65 5f68 7275 5f69 6472  .Z.ilake_hru_idr
+00006b60: d600 0000 5a05 5375 6269 6472 d700 0000  ....Z.Subidr....
+00006b70: 725e 0000 005a 0769 6872 755f 6964 5a07  r^...Z.ihru_idZ.
+00006b80: 6973 5f4c 616b 655a 0a56 616c 695f 5661  is_LakeZ.Vali_Va
+00006b90: 6c75 6572 2400 0000 7224 0000 0072 2500  luer$...r$...r%.
+00006ba0: 0000 da18 4465 7465 726d 696e 655f 4852  ....Determine_HR
+00006bb0: 555f 4174 7472 6962 7574 6573 5606 0000  U_AttributesV...
+00006bc0: 73f8 0000 0000 180c 0118 0118 0118 0118  s...............
+00006bd0: 0214 0116 010c 0314 0108 0108 0102 0204  ................
+00006be0: 010a ff04 0304 0104 ff06 030e 0112 0114  ................
+00006bf0: 010e 010e 010a 0310 ff04 0302 0108 ff04  ................
+00006c00: 0502 fe04 010e ff04 060c fe04 010e ff02  ................
+00006c10: 0510 ff04 0302 0108 ff04 0502 fe04 010e  ................
+00006c20: ff04 060c fe04 010e ff02 0510 ff04 0302  ................
+00006c30: 0108 ff04 0502 fe04 010e ff04 060c fe04  ................
+00006c40: 010e ff02 041a 011e 0410 ff04 0302 0108  ................
+00006c50: ff04 0502 fe04 010e ff02 0410 ff04 0302  ................
+00006c60: 0108 ff04 0502 fe04 010e ff02 0410 ff04  ................
+00006c70: 0302 0108 ff04 0502 fe04 010e ff02 0410  ................
+00006c80: ff04 0302 0108 ff04 0502 fe04 010e ff02  ................
+00006c90: 0410 ff04 0302 0108 ff04 0502 fe04 010e  ................
+00006ca0: ff08 0410 011a 011a 011a 580c 010c ff02  ..........X.....
+00006cb0: 020c fe02 040c fc02 ff06 081a 0172 de00  .............r..
+00006cc0: 0000 6303 0000 0000 0000 0000 0000 0041  ..c............A
+00006cd0: 0000 000c 0000 0043 0000 0073 440b 0000  .......C...sD...
+00006ce0: 6401 7d03 6402 7d04 6403 7d05 6404 7d06  d.}.d.}.d.}.d.}.
+00006cf0: 6405 7d07 6405 7c00 6a00 7601 7222 6406  d.}.d.|.j.v.r"d.
+00006d00: 7d07 7c00 6a01 6407 6408 8d01 7d08 6409  }.|.j.d.d...}.d.
+00006d10: 7c08 640a 3c00 6409 7c08 640b 3c00 7c08  |.d.<.d.|.d.<.|.
+00006d20: 6a02 6407 6407 640c 8d02 0100 7403 a004  j.d.d.d.....t...
+00006d30: 7c08 6403 1900 6a05 a101 7d09 7c02 640d  |.d...j...}.|.d.
+00006d40: 1400 640d 1400 7c09 6b04 728c 7c09 640e  ..d...|.k.r.|.d.
+00006d50: 1b00 640e 1b00 640f 1800 7d02 6409 7c08  ..d...d...}.d.|.
+00006d60: 7c07 3c00 6409 7c00 7c07 3c00 7c00 6a06  |.<.d.|.|.<.|.j.
+00006d70: 7c00 7c05 1900 7c02 640d 1400 640d 1400  |.|...|.d...d...
+00006d80: 6b05 1900 a001 a100 7d0a 7407 7c0a 6409  k.......}.t.|.d.
+00006d90: 6410 8d02 7d0a 7c0a 6a08 6411 6701 6407  d...}.|.j.d.g.d.
+00006da0: 6412 8d02 7d0a 7c0a 6a06 7c0a 6413 1900  d...}.|.j.|.d...
+00006db0: 6414 6b03 1900 a001 a100 7d0a 7c0a 7c03  d.k.......}.|.|.
+00006dc0: 1900 6a05 7d0b 7c0a 6a06 7c0a 6413 1900  ..j.}.|.j.|.d...
+00006dd0: 640f 6b02 1900 6415 1900 6a05 7d0c 7403  d.k...d...j.}.t.
+00006de0: a009 7c0c 7c0c 6416 6b04 1900 a101 7d0c  ..|.|.d.k.....}.
+00006df0: 7c00 6a06 7c00 6415 1900 a00a 7c0c a101  |.j.|.d.....|...
+00006e00: 1900 a001 a100 7d0d 7c0d 7c03 1900 6a05  ......}.|.|...j.
+00006e10: 7d0e 7c00 6a06 7c00 6401 1900 a00a 7c0b  }.|.j.|.d.....|.
+00006e20: a101 0f00 7c00 7c07 1900 6416 6b04 4000  ....|.|...d.k.@.
+00006e30: 1900 6a01 6407 6408 8d01 7d0f 7c0f 6a06  ..j.d.d...}.|.j.
+00006e40: 7c0f 6415 1900 6416 6b01 1900 6401 1900  |.d...d.k...d...
+00006e50: 6a05 7d10 7c00 6a01 6407 6408 8d01 7d11  j.}.|.j.d.d...}.
+00006e60: 7c11 6401 1900 a00a 7c10 a101 7d12 7c11  |.d.....|...}.|.
+00006e70: 6415 1900 640f 6b00 7d13 7403 a00b 7c12  d...d.k.}.t...|.
+00006e80: 7c13 a102 7d14 7c11 6a06 7c11 6401 1900  |...}.|.j.|.d...
+00006e90: a00a 7c10 a101 6401 6602 1900 0b00 7c11  ..|...d.f.....|.
+00006ea0: 6a06 7c14 6415 6602 3c00 7c11 6a06 7c11  j.|.d.f.<.|.j.|.
+00006eb0: 6401 1900 a00a 7c10 a101 6415 6602 1900  d.....|...d.f...
+00006ec0: 6a05 7d15 7c01 6417 1900 6a05 7d16 7403  j.}.|.d...j.}.t.
+00006ed0: a00c 7c16 7c0c a102 7d14 7c16 7403 a00d  ..|.|...}.|.t...
+00006ee0: 7c14 a101 1900 a001 a100 7d17 7c11 6a06  |.........}.|.j.
+00006ef0: 7c11 6415 1900 a00a 7c17 a101 7c11 6415  |.d.....|...|.d.
+00006f00: 1900 a00a 7c15 a101 4200 1900 a001 a100  ....|...B.......
+00006f10: 7d18 7c00 6a06 7c00 6413 1900 6414 6b02  }.|.j.|.d...d.k.
+00006f20: 1900 6401 1900 6a05 7d19 7403 a009 7c19  ..d...j.}.t...|.
+00006f30: 7c19 6416 6b04 1900 a101 7d19 7c00 6a06  |.d.k.....}.|.j.
+00006f40: 7c00 6413 1900 6414 6b02 1900 6415 1900  |.d...d.k...d...
+00006f50: 6a05 7d1a 7403 a009 7c1a 7c1a 6416 6b04  j.}.t...|.|.d.k.
+00006f60: 1900 a101 7d1a 7403 a009 7c0b a101 7d1b  ....}.t...|...}.
+00006f70: 7c00 6401 6402 6702 1900 a00e 6418 a101  |.d.d.g.....d...
+00006f80: 6a05 7d1c 7c0a 6404 1900 6a05 7d1d 7403  j.}.|.d...j.}.t.
+00006f90: a009 7c1d a101 7d1d 7c08 6a06 7c08 6413  ..|...}.|.j.|.d.
+00006fa0: 1900 6414 6b02 1900 6401 1900 6a05 7c08  ..d.k...d...j.|.
+00006fb0: 6a06 7c08 6413 1900 6414 6b02 640a 6602  j.|.d...d.k.d.f.
+00006fc0: 3c00 7c18 a00f 6415 6701 a101 6403 1900  <.|...d.g...d...
+00006fd0: a010 7404 a101 7c18 6403 1900 6b02 7d1e  ..t...|.d...k.}.
+00006fe0: 7c18 7c1e 1900 7d1f 7c1f 6a08 6411 6403  |.|...}.|.j.d.d.
+00006ff0: 6702 6407 6407 6702 6412 8d02 7d1f 7c00  g.d.d.g.d...}.|.
+00007000: 7c00 6402 1900 6416 6b00 1900 6a01 6407  |.d...d.k...j.d.
+00007010: 6408 8d01 7d20 7411 6416 7412 7c20 8301  d...} t.d.t.| ..
+00007020: 8302 4400 5d50 7d21 7c20 6403 1900 6a05  ..D.]P}!| d...j.
+00007030: 7c21 1900 7c02 640d 1400 640d 1400 6b01  |!..|.d...d...k.
+00007040: 9003 7244 7c20 6401 1900 6a05 7c21 1900  ..rD| d...j.|!..
+00007050: 7d22 7413 7c1c 7c22 8302 7d23 7414 7c22  }"t.|.|"..}#t.|"
+00007060: 7c00 7c08 640f 7c00 7c23 6409 6419 8d07  |.|.d.|.|#d.d...
+00007070: 7d08 9003 7144 7411 6416 7412 7c1f 8301  }...qDt.d.t.|...
+00007080: 8302 4400 9001 5d08 7d21 7403 a009 7c08  ..D...].}!t...|.
+00007090: 6a06 7c08 640a 1900 6416 6b04 1900 7c03  j.|.d...d.k...|.
+000070a0: 1900 6a05 a101 7d24 7c1f 6415 1900 6a05  ..j...}$|.d...j.
+000070b0: 7c21 1900 7d25 7c11 7c11 6415 1900 7c25  |!..}%|.|.d...|%
+000070c0: 6b02 1900 7d26 7403 a009 7c26 6404 1900  k...}&t...|&d...
+000070d0: 6a05 a101 7d27 6700 7d28 7411 6416 7412  j...}'g.}(t.d.t.
+000070e0: 7c27 8301 8302 4400 5d82 7d29 7c27 7c29  |'....D.].})|'|)
+000070f0: 1900 7d2a 7c26 6a06 7c26 6404 1900 7c2a  ..}*|&j.|&d...|*
+00007100: 6b02 1900 a001 a100 7d2b 7c2b 6a08 6403  k.......}+|+j.d.
+00007110: 6701 641a 6412 8d02 7d2b 7c2b 6401 1900  g.d.d...}+|+d...
+00007120: 6a05 6416 1900 7d22 7413 7c1c 7c22 8302  j.d...}"t.|.|"..
+00007130: 7d23 7c23 7c23 6416 6b04 1900 7d23 7403  }#|#|#d.k...}#t.
+00007140: a00c 7c23 7c24 a102 7d14 7c23 7403 a00d  ..|#|$..}.|#t...
+00007150: 7c14 a101 1900 7d2c 6700 7c28 a201 7c2c  |.....},g.|(..|,
+00007160: a015 a100 a201 7d28 9004 7108 7403 a016  ......}(..q.t...
+00007170: 7c28 a101 7d28 7414 7c22 7c11 7c08 640f  |(..}(t.|"|.|.d.
+00007180: 7c11 7c28 6414 6419 8d07 7d08 9003 71a4  |.|(d.d...}...q.
+00007190: 7411 6416 7412 7c1d 8301 8302 4400 9005  t.d.t.|.....D...
+000071a0: 5df0 7d2d 7c1d 7c2d 1900 7d2e 7c0a 6a06  ].}-|.|-..}.|.j.
+000071b0: 7c0a 6404 1900 7c2e 6b02 1900 a001 a100  |.d...|.k.......
+000071c0: 7d2f 7c2f 6a08 641b 6701 6407 6412 8d02  }/|/j.d.g.d.d...
+000071d0: 7d2f 6416 7d30 6700 7d28 640f 7d31 7411  }/d.}0g.}(d.}1t.
+000071e0: 6416 7412 7c2f 8301 8302 4400 9005 5d9e  d.t.|/....D...].
+000071f0: 7d32 7c2f 6401 1900 6a05 7c32 1900 7d22  }2|/d...j.|2..}"
+00007200: 7c2f 6415 1900 6a05 7c32 1900 7d33 7c28  |/d...j.|2..}3|(
+00007210: a017 7c22 a101 0100 7403 a009 7c08 6a06  ..|"....t...|.j.
+00007220: 7c08 640a 1900 6416 6b04 1900 7c03 1900  |.d...d.k...|...
+00007230: 6a05 a101 7d24 7c30 7c2f 641c 1900 6a05  j...}$|0|/d...j.
+00007240: 7c32 1900 1700 7d30 7c32 7412 7c2f 8301  |2....}0|2t.|/..
+00007250: 640f 1800 6b03 9005 729c 7c2f 6415 1900  d...k...r.|/d...
+00007260: 6a05 7c32 1900 7c2f 6415 1900 6a05 7c32  j.|2..|/d...j.|2
+00007270: 640f 1700 1900 6b02 7d34 6e04 641a 7d34  d.....k.}4n.d.}4
+00007280: 7c2f 7c07 1900 6a05 7c32 1900 6416 6b01  |/|...j.|2..d.k.
+00007290: 7d35 7c32 7412 7c2f 8301 6414 1800 6b01  }5|2t.|/..d...k.
+000072a0: 9005 72f4 7c2f 641c 1900 6a05 7c32 640f  ..r.|/d...j.|2d.
+000072b0: 1700 1900 641d 6b00 9005 72e2 6407 7d36  ....d.k...r.d.}6
+000072c0: 6e10 7c30 7c02 640d 1400 640d 1400 6b00  n.|0|.d...d...k.
+000072d0: 7d36 6e10 7c30 7c02 640d 1400 640d 1400  }6n.|0|.d...d...
+000072e0: 6b00 7d36 7c30 641d 6b00 7d37 7c32 640f  k.}6|0d.k.}7|2d.
+000072f0: 6b05 9006 727e 7c32 7412 7c2f 8301 6414  k...r~|2t.|/..d.
+00007300: 1800 6b01 9006 727e 7c2f 6415 1900 6a05  ..k...r~|/d...j.
+00007310: 7c32 640f 1800 1900 7c2f 6415 1900 6a05  |2d.....|/d...j.
+00007320: 7c32 1900 6b03 7d38 7c2f 6415 1900 6a05  |2..k.}8|/d...j.
+00007330: 7c32 1900 7c2f 6415 1900 6a05 7c32 640f  |2..|/d...j.|2d.
+00007340: 1700 1900 6b03 7d39 7c2f 6415 1900 6a05  ....k.}9|/d...j.
+00007350: 7c32 1900 6416 6b01 7d3a 641a 7d37 7c32  |2..d.k.}:d.}7|2
+00007360: 6416 6b02 9006 72d4 7c32 7412 7c2f 8301  d.k...r.|2t.|/..
+00007370: 640f 1800 6b00 9006 72d4 6407 7d38 7c2f  d...k...r.d.}8|/
+00007380: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
+00007390: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
+000073a0: 6415 1900 6a05 7c32 1900 6416 6b01 7d3a  d...j.|2..d.k.}:
+000073b0: 641a 7d37 7c32 7412 7c2f 8301 6414 1800  d.}7|2t.|/..d...
+000073c0: 6b02 9008 720e 7c2f 6415 1900 6a05 7c32  k...r.|/d...j.|2
+000073d0: 1900 6416 6b04 9008 720e 6407 7d38 7c2f  ..d.k...r.d.}8|/
+000073e0: 6415 1900 6a05 7c32 1900 7c2f 6415 1900  d...j.|2..|/d...
+000073f0: 6a05 7c32 640f 1700 1900 6b03 7d39 7c2f  j.|2d.....k.}9|/
+00007400: 6415 1900 6a05 7c32 1900 6416 6b04 7d3a  d...j.|2..d.k.}:
+00007410: 7c2f 6402 1900 6a05 7c32 1900 7d3b 641a  |/d...j.|2..};d.
+00007420: 7d37 7c37 9008 720e 7c39 9008 720e 7c2f  }7|7..r.|9..r.|/
+00007430: 6415 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007440: 6401 1900 7c3b 6b02 6415 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007450: 6413 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007460: 6401 1900 7c3b 6b02 6413 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007470: 641e 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+00007480: 6401 1900 7c3b 6b02 641e 6602 3c00 7c2f  d...|;k.d.f.<.|/
+00007490: 641f 1900 6a05 7c32 1900 7c00 6a06 7c00  d...j.|2..|.j.|.
+000074a0: 6401 1900 7c3b 6b02 641f 6602 3c00 7c2f  d...|;k.d.f.<.|/
+000074b0: 6420 1900 6a05 7c32 1900 7c00 6a06 7c00  d ..j.|2..|.j.|.
+000074c0: 6401 1900 7c3b 6b02 6420 6602 3c00 7c2f  d...|;k.d f.<.|/
+000074d0: 6421 1900 6a05 7c32 1900 7c00 6a06 7c00  d!..j.|2..|.j.|.
+000074e0: 6401 1900 7c3b 6b02 6421 6602 3c00 7c32  d...|;k.d!f.<.|2
+000074f0: 7412 7c2f 8301 640f 1800 6b02 9008 722c  t.|/..d...k...r,
+00007500: 6407 7d38 641a 7d39 6407 7d3a 7c32 7412  d.}8d.}9d.}:|2t.
+00007510: 7c2f 8301 640f 1800 6b02 9009 7256 6416  |/..d...k...rVd.
+00007520: 7d30 7403 a016 7c28 a101 7d2c 7c33 6416  }0t...|(..},|3d.
+00007530: 6b04 9008 72aa 7c00 6a06 7c00 6415 1900  k...r.|.j.|.d...
+00007540: 7c33 6b02 1900 a001 a100 7d3c 7c3c 6401  |3k.......}<|<d.
+00007550: 6402 6702 1900 a00e 6418 a101 6a05 7d3d  d.g.....d...j.}=
+00007560: 7413 7c3d 7c22 8302 7d3e 7403 a009 7403  t.|=|"..}>t...t.
+00007570: a018 7c2c 7c3e 6702 a101 a101 7d2c 7c2c  ..|,|>g.....},|,
+00007580: 7c2c 6416 6b04 1900 7d2c 7413 7c1c 7c22  |,d.k...},t.|.|"
+00007590: 8302 7d23 7c23 7c23 6416 6b04 1900 7d23  ..}#|#|#d.k...}#
+000075a0: 7403 a00c 7c23 7c0b a102 7d12 7c23 7403  t...|#|...}.|#t.
+000075b0: a00d 7c12 a101 1900 7d3f 7403 a009 7403  ..|.....}?t...t.
+000075c0: a018 7c2c 7c3f 6702 a101 a101 7d2c 7c2c  ..|,|?g.....},|,
+000075d0: 7c2c 6416 6b04 1900 7d2c 7403 a00c 7c2c  |,d.k...},t...|,
+000075e0: 7c24 a102 7d14 7c2c 7403 a00d 7c14 a101  |$..}.|,t...|...
+000075f0: 1900 7d2c 7403 a00c 7c2c 7c19 a102 7d40  ..},t...|,|...}@
+00007600: 7c2c 7403 a00d 7c40 a101 1900 7d2c 7414  |,t...|@....},t.
+00007610: 7c22 7c00 7c08 640f 7c2c 7c0a 6422 7c31  |"|.|.d.|,|.d"|1
+00007620: 6423 8d08 7d08 6700 7d28 7c31 640f 1700  d#..}.g.}(|1d...
+00007630: 7d31 9005 710c 7c38 9009 727c 7c39 9009  }1..q.|8..r||9..
+00007640: 727c 7c3a 9009 727c 7c35 9009 727c 7c37  r||:..r||5..r||7
+00007650: 9009 727c 9005 710c 9005 710c 7c34 9009  ..r|..q...q.|4..
+00007660: 7296 7c35 9009 7296 7c36 9009 7296 9005  r.|5..r.|6..r...
+00007670: 710c 9005 710c 6416 7d30 7403 a016 7c28  q...q.d.}0t...|(
+00007680: a101 7d2c 7c33 6416 6b04 900a 7202 7c00  ..},|3d.k...r.|.
+00007690: 6a06 7c00 6415 1900 7c33 6b02 1900 a001  j.|.d...|3k.....
+000076a0: a100 7d3c 7c3c 6401 6402 6702 1900 a00e  ..}<|<d.d.g.....
+000076b0: 6418 a101 6a05 7d3d 7413 7c3d 7c22 8302  d...j.}=t.|=|"..
+000076c0: 7d3e 7403 a009 7403 a018 7c2c 7c3e 6702  }>t...t...|,|>g.
+000076d0: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
+000076e0: 7d2c 7413 7c1c 7c22 8302 7d23 7c23 7c23  },t.|.|"..}#|#|#
+000076f0: 6416 6b04 1900 7d23 7403 a00c 7c23 7c0b  d.k...}#t...|#|.
+00007700: a102 7d12 7c23 7403 a00d 7c12 a101 1900  ..}.|#t...|.....
+00007710: 7d3f 7403 a009 7403 a018 7c2c 7c3f 6702  }?t...t...|,|?g.
+00007720: a101 a101 7d2c 7c2c 7c2c 6416 6b04 1900  ....},|,|,d.k...
+00007730: 7d2c 7403 a00c 7c2c 7c24 a102 7d14 7c2c  },t...|,|$..}.|,
+00007740: 7403 a00d 7c14 a101 1900 7d2c 7403 a00c  t...|.....},t...
+00007750: 7c2c 7c19 a102 7d40 7c2c 7403 a00d 7c40  |,|...}@|,t...|@
+00007760: a101 1900 7d2c 7414 7c22 7c00 7c08 640f  ....},t.|"|.|.d.
+00007770: 7c2c 7c0a 6422 7c31 6423 8d08 7d08 6700  |,|.d"|1d#..}.g.
+00007780: 7d28 7c31 640f 1700 7d31 9005 710c 9004  }(|1d...}1..q...
+00007790: 71be 6416 7c08 6a06 7c08 6415 1900 6416  q.d.|.j.|.d...d.
+000077a0: 6b01 6415 6602 3c00 6416 7c08 6a06 7c08  k.d.f.<.d.|.j.|.
+000077b0: 6415 1900 6416 6b01 6413 6602 3c00 6416  d...d.k.d.f.<.d.
+000077c0: 7c08 6a06 7c08 6415 1900 6416 6b01 641e  |.j.|.d...d.k.d.
+000077d0: 6602 3c00 6416 7c08 6a06 7c08 6415 1900  f.<.d.|.j.|.d...
+000077e0: 6416 6b01 641f 6602 3c00 6416 7c08 6a06  d.k.d.f.<.d.|.j.
+000077f0: 7c08 6415 1900 6416 6b01 6420 6602 3c00  |.d...d.k.d f.<.
+00007800: 6416 7c08 6a06 7c08 6415 1900 6416 6b01  d.|.j.|.d...d.k.
+00007810: 6421 6602 3c00 7c08 7c1b 7c0c 7c1a 7c17  d!f.<.|.|.|.|.|.
+00007820: 6605 5300 2924 7aac 4d6f 6469 6679 2061  f.S.)$z.Modify a
+00007830: 7474 7269 6275 7465 2074 6162 6c65 206d  ttribute table m
+00007840: 6170 6f6c 646e 6577 5f69 6e66 6f2c 2063  apoldnew_info, c
+00007850: 7265 6174 6520 6e65 7720 7375 6220 6964  reate new sub id
+00007860: 2066 6f72 2073 7562 6261 7369 6e20 6e65   for subbasin ne
+00007870: 6564 7320 746f 2062 6520 6d65 7267 6564  eds to be merged
+00007880: 2e0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
+00007890: 0a0a 2020 2020 4e6f 7465 730a 2020 2020  ..    Notes.    
+000078a0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052 6574  -------..    Ret
+000078b0: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
+000078c0: 2d0a 2020 2020 2020 2020 4e6f 6e65 2c0a  -.        None,.
+000078d0: 2020 2020 7206 0000 0072 0d00 0000 7279      r....r....ry
+000078e0: 0000 0072 6600 0000 7280 0000 0072 8100  ...rf...r....r..
+000078f0: 0000 5472 0700 0000 726b 0000 0072 8300  ..Tr....rk...r..
+00007900: 0000 7285 0000 00a9 0272 1c00 0000 da07  ..r......r......
+00007910: 696e 706c 6163 6572 7c00 0000 72b4 0000  inplacer|...r...
+00007920: 0072 2800 0000 2901 72ab 0000 0072 6900  .r(...).r....ri.
+00007930: 0000 727a 0000 0072 6400 0000 7265 0000  ..rz...rd...re..
+00007940: 0072 8400 0000 7201 0000 0072 ce00 0000  .r....r....r....
+00007950: 7263 0000 0029 0772 4900 0000 729d 0000  rc...).rI...r...
+00007960: 0072 8a00 0000 729e 0000 0072 a000 0000  .r....r....r....
+00007970: 729f 0000 0072 6400 0000 4672 6a00 0000  r....rd...Frj...
+00007980: 7282 0000 0069 8096 9800 7294 0000 0072  r....i....r....r
+00007990: 9600 0000 7295 0000 0072 9700 0000 e903  ....r....r......
+000079a0: 0000 00a9 0872 4900 0000 729d 0000 0072  .....rI...r....r
+000079b0: 8a00 0000 729e 0000 0072 9f00 0000 72a0  ....r....r....r.
+000079c0: 0000 0072 6400 0000 72a1 0000 0029 1972  ...rd...r....).r
+000079d0: 1100 0000 7214 0000 00da 0b72 6573 6574  ....r......reset
+000079e0: 5f69 6e64 6578 721a 0000 0072 7400 0000  _indexr....rt...
+000079f0: 7213 0000 0072 1900 0000 72b0 0000 0072  r....r....r....r
+00007a00: 4100 0000 722b 0000 0072 1200 0000 7243  A...r+...r....rC
+00007a10: 0000 0072 2e00 0000 729a 0000 0072 1600  ...r....r....r..
+00007a20: 0000 723e 0000 00da 0974 7261 6e73 666f  ..r>.....transfo
+00007a30: 726d 7229 0000 0072 1500 0000 7217 0000  rmr)...r....r...
+00007a40: 0072 a300 0000 72c8 0000 00da 0761 7361  .r....r......asa
+00007a50: 7272 6179 724e 0000 0072 1b00 0000 2941  rrayrN...r....)A
+00007a60: 5a0d 6669 6e61 6c72 6976 5f69 6e66 6f5a  Z.finalriv_infoZ
+00007a70: 0e43 6f6e 6e5f 4c61 6b65 735f 706c 79da  .Conn_Lakes_ply.
+00007a80: 0841 7265 615f 4d69 6e72 a200 0000 da0a  .Area_Minr......
+00007a90: 646f 776e 5f63 6f6c 6e6d 5a08 4441 5f63  down_colnmZ.DA_c
+00007aa0: 6f6c 6e6d 5a0b 5365 6749 445f 636f 6c6e  olnmZ.SegID_coln
+00007ab0: 6d72 8c00 0000 728a 0000 005a 066d 6178  mr....r....Z.max
+00007ac0: 5f64 615a 0c53 656c 6563 7465 645f 7269  _daZ.Selected_ri
+00007ad0: 765a 0a53 7562 6964 5f6d 6169 6e5a 1643  vZ.Subid_mainZ.C
+00007ae0: 6f6e 6e65 6374 6564 5f4c 616b 655f 4d61  onnected_Lake_Ma
+00007af0: 696e 7269 765a 0d4c 616b 6563 6f76 6572  inrivZ.Lakecover
+00007b00: 5f72 6976 5a0b 5375 6269 645f 6c61 6b65  _rivZ.Subid_lake
+00007b10: 735a 1d75 6e73 656c 6563 7465 645f 6761  sZ.unselected_ga
+00007b20: 7567 6573 5f73 7562 6964 735f 696e 666f  uges_subids_info
+00007b30: 5a18 756e 7365 6c65 6374 6564 5f67 6175  Z.unselected_gau
+00007b40: 6765 735f 7375 6269 6473 5a11 6669 6e61  ges_subidsZ.fina
+00007b50: 6c72 6976 5f69 6e66 6f5f 6e63 6c72 4a00  lriv_info_nclrJ.
+00007b60: 0000 724b 0000 0072 2300 0000 5a12 6661  ..rK...r#...Z.fa
+00007b70: 6b65 5f6f 6273 5f68 7961 6c6b 6569 6473  ke_obs_hyalkeids
+00007b80: 5a10 416c 6c5f 436f 6e6e 5f4c 616b 6569  Z.All_Conn_Lakei
+00007b90: 6473 5a15 436f 6e6e 5f54 6f5f 4e6f 6e43  dsZ.Conn_To_NonC
+00007ba0: 6f6e 6c61 6b65 6964 735a 1743 6f6e 6e5f  onlakeidsZ.Conn_
+00007bb0: 546f 5f4e 6f6e 436f 6e6c 616b 655f 696e  To_NonConlake_in
+00007bc0: 666f 5a16 4f6c 645f 4e6f 6e5f 436f 6e6e  foZ.Old_Non_Conn
+00007bd0: 6563 745f 5375 6249 6473 5a17 4f6c 645f  ect_SubIdsZ.Old_
+00007be0: 4e6f 6e5f 436f 6e6e 6563 745f 4c61 6b65  Non_Connect_Lake
+00007bf0: 4964 735a 1053 656c 6563 7465 645f 7269  IdsZ.Selected_ri
+00007c00: 765f 6964 7372 7700 0000 da07 5365 675f  v_idsrw.....Seg_
+00007c10: 4944 5372 5f00 0000 5a1e 436f 6e6e 5f54  IDSr_...Z.Conn_T
+00007c20: 6f5f 4e6f 6e43 6f6e 6c61 6b65 5f69 6e66  o_NonConlake_inf
+00007c30: 6f5f 6f75 746c 6574 5a13 616c 6c5f 6f75  o_outletZ.all_ou
+00007c40: 746c 6574 5f73 7562 5f69 6e66 6f72 4800  tlet_sub_inforH.
+00007c50: 0000 da06 7473 7562 6964 5a0d 416c 6c5f  ....tsubidZ.All_
+00007c60: 7570 5f73 7562 6964 735a 0f70 726f 6365  up_subidsZ.proce
+00007c70: 7373 6564 5f73 7562 6964 5a0c 435f 545f  ssed_subidZ.C_T_
+00007c80: 4e5f 4c61 6b65 6964 5a0d 4c61 6b65 5f43  N_LakeidZ.Lake_C
+00007c90: 6174 5f69 6e66 6f5a 0b52 6976 5f53 6567  at_infoZ.Riv_Seg
+00007ca0: 5f49 4453 da0c 6d6f 6469 6679 7375 6269  _IDS..modifysubi
+00007cb0: 6473 725e 0000 005a 0869 7269 765f 7365  dsr^...Z.iriv_se
+00007cc0: 675a 114c 616b 655f 4361 745f 7365 675f  gZ.Lake_Cat_seg_
+00007cd0: 696e 666f da0b 7365 675f 7375 625f 6964  info..seg_sub_id
+00007ce0: 7372 b700 0000 da08 695f 7365 675f 6964  sr......i_seg_id
+00007cf0: da0a 695f 7365 675f 696e 666f 5a08 7375  ..i_seg_infoZ.su
+00007d00: 6d5f 6172 6561 72a1 0000 00da 0669 6f72  m_arear......ior
+00007d10: 6465 725a 0d69 6f72 6465 725f 4c61 6b65  derZ.iorder_Lake
+00007d20: 6964 5a08 636f 6e5f 6c61 6b65 5a09 636f  idZ.con_lakeZ.co
+00007d30: 6e5f 6761 7567 655a 0863 6f6e 5f61 7265  n_gaugeZ.con_are
+00007d40: 615a 0d63 6f6e 5f61 7265 615f 6c61 6b65  aZ.con_area_lake
+00007d50: 5a0b 636f 6e5f 6c61 6b65 5f75 705a 0d63  Z.con_lake_upZ.c
+00007d60: 6f6e 5f6c 616b 655f 646f 776e 5a07 6973  on_lake_downZ.is
+00007d70: 5f6c 616b 6572 cb00 0000 5a13 7375 6269  _laker....Z.subi
+00007d80: 645f 6375 725f 6c61 6b65 5f69 6e66 6f5a  d_cur_lake_infoZ
+00007d90: 1172 6f75 7469 6e67 5f69 6e66 6f5f 6c61  .routing_info_la
+00007da0: 6b65 5a0f 5570 7374 7265 616d 4c61 6b65  keZ.UpstreamLake
+00007db0: 6964 735a 1541 6c6c 5f75 705f 7375 6269  idsZ.All_up_subi
+00007dc0: 6473 5f6e 6f5f 6d61 696e 5a10 6d61 736b  ds_no_mainZ.mask
+00007dd0: 5f6f 6c64 5f6e 6f6e 4c61 6b65 7224 0000  _old_nonLaker$..
+00007de0: 0072 2400 0000 7225 0000 00da 4743 6861  .r$...r%....GCha
+00007df0: 6e67 655f 4174 7472 6962 7574 655f 5661  nge_Attribute_Va
+00007e00: 6c75 6573 5f46 6f72 5f43 6174 6368 6d65  lues_For_Catchme
+00007e10: 6e74 735f 4e65 6564 5f54 6f5f 4265 5f4d  nts_Need_To_Be_M
+00007e20: 6572 6765 645f 4279 5f49 6e63 7265 6173  erged_By_Increas
+00007e30: 655f 4441 4d07 0000 7362 0200 0000 0d04  e_DAM...sb......
+00007e40: 0104 0104 0104 0204 010a 0104 070c 0108  ................
+00007e50: 0108 010e 0110 0310 0110 0108 0108 0404  ................
+00007e60: 0112 ff08 050c 0104 0106 ff06 0316 010a  ................
+00007e70: 0310 0102 ff06 0304 010a ff04 0304 010c  ................
+00007e80: ff08 030a 0504 010e 010a ff02 ff04 0302  ................
+00007e90: fd06 0418 020c 020e 010c 010c 0124 011a  .............$..
+00007ea0: 040a 010c 0112 0104 010c 010c ff02 ff08  ................
+00007eb0: 0a10 0102 ff06 0304 010a ff04 0310 0102  ................
+00007ec0: ff06 0304 010a ff04 0504 0102 ff04 0314  ................
+00007ed0: 010a 010a 0304 010a ff02 0202 fe18 0614  ................
+00007ee0: 0106 ff02 ff02 0408 0204 010c ff06 0618  ................
+00007ef0: 0212 011c 010e 010a 0202 0102 0102 0102  ................
+00007f00: 0102 0102 0102 0102 f90a 0d14 0104 0116  ................
+00007f10: ff04 040e 0110 0110 0104 0112 0208 0104  ................
+00007f20: 010a ff08 0310 010e 020a 010c 020c 010e  ................
+00007f30: 0202 0102 ff02 0206 fe08 050a 0202 0102  ................
+00007f40: 0102 0102 0102 0102 0102 0102 f90a 0b14  ................
+00007f50: 0208 0116 0110 0104 0104 0104 0114 010e  ................
+00007f60: 010e 010a 0104 0116 ff04 0312 0412 0122  ..............."
+00007f70: 0204 0212 0312 0118 0106 0212 0210 0308  ................
+00007f80: 021c 0220 0220 0212 0204 021c 0204 0220  ... . ......... 
+00007f90: 0212 0204 0226 0204 0220 0212 050e 0204  .....&... ......
+00007fa0: 020c 020c ff04 010e ff02 030c ff04 010e  ................
+00007fb0: ff02 030c ff04 010e ff02 030c ff04 010e  ................
+00007fc0: ff02 030c ff04 010e ff02 030c ff04 010e  ................
+00007fd0: ff02 0312 0104 0104 0104 0712 0104 010a  ................
+00007fe0: 020a 0104 010a ff08 040c 0102 ff04 ff02  ................
+00007ff0: 050a 0104 010c ff04 030c 030a 010c 0104  ................
+00008000: 0104 ff04 030e 0204 010c ff04 030c 010c  ................
+00008010: 010e 020c 010e 0202 0102 0102 0102 0102  ................
+00008020: 0102 0102 0102 0102 f806 0b04 010c 021e  ................
+00008030: 0108 0212 0108 0304 010a 020a 0104 010a  ................
+00008040: ff08 040c 0102 ff04 ff02 050a 0104 010c  ................
+00008050: ff04 030c 020a 010c 0104 0104 ff04 030e  ................
+00008060: 0204 010c ff04 030c 010c 010e 020c 010e  ................
+00008070: 0302 0102 0102 0102 0102 0102 0102 0102  ................
+00008080: 0102 f806 0a04 0110 0216 0116 0116 0116  ................
+00008090: 0116 0116 0302 0102 0102 0102 0102 fb72  ...............r
+000080a0: ef00 0000 6304 0000 0000 0000 0000 0000  ....c...........
+000080b0: 0016 0000 0007 0000 0043 0000 0073 0002  .........C...s..
+000080c0: 0000 7c00 6401 1900 a000 7401 a101 7c00  ..|.d.....t...|.
+000080d0: 6401 3c00 7c00 6402 1900 a000 7402 a101  d.<.|.d.....t...
+000080e0: 7c00 6402 3c00 7c00 6403 1900 a000 7402  |.d.<.|.d.....t.
+000080f0: a101 7c00 6403 3c00 7c00 6a03 7c00 6404  ..|.d.<.|.j.|.d.
+00008100: 1900 6405 6b02 1900 6a04 6406 6407 8d01  ..d.k...j.d.d...
+00008110: 7d04 7c00 6a03 7c00 6404 1900 6408 6b02  }.|.j.|.d...d.k.
+00008120: 1900 6a04 6406 6407 8d01 7d05 6409 7c00  ..j.d.d...}.d.|.
+00008130: 6a05 7600 727a 6409 7d06 6e04 640a 7d06  j.v.rzd.}.n.d.}.
+00008140: 7c05 6401 1900 7c01 6b05 7d07 7c05 7c06  |.d...|.k.}.|.|.
+00008150: 1900 6408 6b02 7d08 7406 a007 7c07 7c08  ..d.k.}.t...|.|.
+00008160: a102 7d09 7c05 6a03 7c09 1900 6402 1900  ..}.|.j.|...d...
+00008170: 6a08 7d0a 7c0a 7c0a 640b 6b04 1900 7d0a  j.}.|.|.d.k...}.
+00008180: 7406 a009 7c0a a101 7d0a 7c04 6401 1900  t...|...}.|.d...
+00008190: 7c02 6b05 7d07 7c04 7c06 1900 6408 6b02  |.k.}.|.|...d.k.
+000081a0: 7d08 7406 a007 7c07 7c08 a102 7d09 7c04  }.t...|.|...}.|.
+000081b0: 7c09 1900 6402 1900 6a08 7d0b 7c0b 7c0b  |...d...j.}.|.|.
+000081c0: 640b 6b04 1900 7d0b 7406 a009 7c0b a101  d.k...}.t...|...
+000081d0: 7d0b 740a 7c03 8301 640b 6b04 9001 7224  }.t.|...d.k...r$
+000081e0: 7c03 7d0c 6e06 640c 6701 7d0c 7c05 6402  |.}.n.d.g.}.|.d.
+000081f0: 1900 6a08 7d0d 7c04 6402 1900 6a08 7d0e  ..j.}.|.d...j.}.
+00008200: 7406 a00b 7c0c a101 7d0f 7406 a00c 7c0d  t...|...}.t...|.
+00008210: 7c0f a102 7d10 7406 a00c 7c0e 7c0f a102  |...}.t...|.|...
+00008220: 7d11 7c0d 7c10 1900 7d12 7406 a009 7c12  }.|.|...}.t...|.
+00008230: a101 7d12 7c0e 7c11 1900 7d13 7406 a009  ..}.|.|...}.t...
+00008240: 7c13 a101 7d13 7406 6a0d 7c0b 7c13 6602  |...}.t.j.|.|.f.
+00008250: 640b 640d 8d02 7d0b 7406 6a0d 7c0a 7c12  d.d...}.t.j.|.|.
+00008260: 6602 640b 640d 8d02 7d0a 7c00 6a03 7c00  f.d.d...}.|.j.|.
+00008270: 6404 1900 6408 6b02 7406 a00e 7c00 6402  d...d.k.t...|.d.
+00008280: 1900 a00f 7c0a a101 a101 4000 1900 7d14  ....|.....@...}.
+00008290: 7c00 6a03 7c00 6404 1900 6405 6b02 7406  |.j.|.d...d.k.t.
+000082a0: a00e 7c00 6402 1900 a00f 7c0b a101 a101  ..|.d.....|.....
+000082b0: 4000 1900 7d15 7c0b 7c0a 7c14 7c15 6604  @...}.|.|.|.|.f.
+000082c0: 5300 290e 7a80 5265 7472 756e 2073 656c  S.).z.Retrun sel
+000082d0: 6563 7465 6420 6c61 6b65 2773 2061 7474  ected lake's att
+000082e0: 7269 6275 7465 2074 6162 6c65 2061 6e64  ribute table and
+000082f0: 2049 440a 2020 2020 2d2d 2d2d 2d2d 2d2d   ID.    --------
+00008300: 2d2d 0a0a 2020 2020 4e6f 7465 730a 2020  --..    Notes.  
+00008310: 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020 2052    -------..    R
+00008320: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00008330: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00008340: 2c0a 2020 2020 7295 0000 0072 8400 0000  ,.    r....r....
+00008350: 7266 0000 0072 6400 0000 7265 0000 0054  rf...rd...re...T
+00008360: 7207 0000 0072 2800 0000 7280 0000 0072  r....r(...r....r
+00008370: 8100 0000 7201 0000 0069 8169 67ff 720e  ....r....i.ig.r.
+00008380: 0000 0029 1072 1600 0000 7263 0000 0072  ...).r....rc...r
+00008390: 2d00 0000 7219 0000 0072 1400 0000 7211  -...r....r....r.
+000083a0: 0000 0072 1a00 0000 7289 0000 0072 1300  ...r....r....r..
+000083b0: 0000 722b 0000 0072 1500 0000 da05 6172  ..r+...r......ar
+000083c0: 7261 7972 2e00 0000 721b 0000 0072 9a00  rayr....r....r..
+000083d0: 0000 7212 0000 0029 16da 0d66 696e 616c  ..r....)...final
+000083e0: 6361 745f 696e 666f da15 5468 7265 735f  cat_info..Thres_
+000083f0: 4172 6561 5f43 6f6e 6e5f 4c61 6b65 73da  Area_Conn_Lakes.
+00008400: 1954 6872 6573 5f41 7265 615f 4e6f 6e5f  .Thres_Area_Non_
+00008410: 436f 6e6e 5f4c 616b 6573 da15 5365 6c65  Conn_Lakes..Sele
+00008420: 6374 6564 5f4c 616b 655f 4c69 7374 5f69  cted_Lake_List_i
+00008430: 6e5a 0e4e 6f6e 5f43 6f6e 6e4c 5f69 6e66  nZ.Non_ConnL_inf
+00008440: 6f5a 0a43 6f6e 6e4c 5f69 6e66 6f72 8c00  oZ.ConnL_infor..
+00008450: 0000 724a 0000 0072 4b00 0000 7223 0000  ..rJ...rK...r#..
+00008460: 005a 1253 656c 6563 7465 645f 436f 6e6e  .Z.Selected_Conn
+00008470: 4c61 6b65 735a 1653 656c 6563 7465 645f  LakesZ.Selected_
+00008480: 4e6f 6e5f 436f 6e6e 4c61 6b65 735a 1253  Non_ConnLakesZ.S
+00008490: 656c 6563 7465 645f 4c61 6b65 5f4c 6973  elected_Lake_Lis
+000084a0: 745a 0941 6c6c 5f43 6f6e 6e4c 5a0d 416c  tZ.All_ConnLZ.Al
+000084b0: 6c5f 4e6f 6e5f 436f 6e6e 4c5a 1b53 656c  l_Non_ConnLZ.Sel
+000084c0: 6563 7465 645f 4c61 6b65 5f4c 6973 745f  ected_Lake_List_
+000084d0: 696e 5f61 7272 6179 5a07 6d61 736b 5f43  in_arrayZ.mask_C
+000084e0: 4c5a 086d 6173 6b5f 4e43 4c5a 1753 656c  LZ.mask_NCLZ.Sel
+000084f0: 6563 7465 645f 436f 6e6e 4c61 6b65 735f  ected_ConnLakes_
+00008500: 4c69 7374 5a1b 5365 6c65 6374 6564 5f4e  ListZ.Selected_N
+00008510: 6f6e 5f43 6f6e 6e4c 616b 6573 5f4c 6973  on_ConnLakes_Lis
+00008520: 74da 1a55 6e5f 5365 6c65 6374 6564 5f43  t..Un_Selected_C
+00008530: 6f6e 6e4c 616b 6573 5f69 6e66 6fda 1a55  onnLakes_info..U
+00008540: 6e5f 5365 6c65 6374 6564 5f4e 6f6e 5f43  n_Selected_Non_C
+00008550: 6f6e 6e4c 5f69 6e66 6f72 2400 0000 7224  onnL_infor$...r$
+00008560: 0000 0072 2500 0000 da2c 5265 7475 726e  ...r%....,Return
+00008570: 5f53 656c 6563 7465 645f 4c61 6b65 735f  _Selected_Lakes_
+00008580: 4174 7472 6962 7574 655f 5461 626c 655f  Attribute_Table_
+00008590: 416e 645f 4964 ef08 0000 7372 0000 0000  And_Id....sr....
+000085a0: 1012 0112 0112 021a 011a 020a 0106 0204  ................
+000085b0: 030c 010c 010c 0104 0102 ff02 0202 fe06  ................
+000085c0: 040c 010a 030c 010c 010c 0202 0102 ff02  ................
+000085d0: 0202 fe06 030c 010a 040e 0106 0306 010a  ................
+000085e0: 010a 010a 020c 010c 0208 010a 0108 010a  ................
+000085f0: 0312 0112 0204 010a 0112 ff02 ff04 0404  ................
+00008600: 010a 0112 ff02 ff04 0602 0102 0102 0102  ................
+00008610: fc72 f700 0000 6302 0000 0000 0000 0000  .r....c.........
+00008620: 0000 000e 0000 000c 0000 0043 0000 0073  ...........C...s
+00008630: 2202 0000 7c00 6a00 6401 6402 8d01 7d02  "...|.j.d.d...}.
+00008640: 6403 7c02 6404 3c00 6403 7c02 6405 3c00  d.|.d.<.d.|.d.<.
+00008650: 7c02 6406 1900 7c02 6407 3c00 7c02 6a01  |.d...|.d.<.|.j.
+00008660: 6401 6401 6408 8d02 0100 6409 7d03 6409  d.d.d.....d.}.d.
+00008670: 7c02 6a02 7601 7248 640a 7d03 7c01 640b  |.j.v.rHd.}.|.d.
+00008680: 1900 6a03 7d04 7404 a005 7c04 a101 7d04  ..j.}.t...|...}.
+00008690: 7406 640c 7407 7c04 8301 8302 4400 9001  t.d.t.|.....D...
+000086a0: 5db0 7d05 7c04 7c05 1900 7d06 7c00 6a08  ].}.|.|...}.|.j.
+000086b0: 7c00 640b 1900 7c06 6b02 7c00 640d 1900  |.d...|.k.|.d...
+000086c0: 640e 6b03 4000 1900 a000 a100 7d07 7c07  d.k.@.......}.|.
+000086d0: 6a09 640f 6701 6401 6410 8d02 7d07 7404  j.d.g.d.d...}.t.
+000086e0: a005 7c07 6411 1900 6a03 a101 7d08 7407  ..|.d...j...}.t.
+000086f0: 7c07 8301 7407 7c08 8301 6b02 72cc 716a  |...t.|...k.r.qj
+00008700: 7404 a00a 7c08 a101 9001 7226 7404 a00a  t...|.....r&t...
+00008710: 7c07 7c03 1900 6a03 a101 640c 6b01 9001  |.|...j...d.k...
+00008720: 7226 7c07 6406 1900 6a03 7407 7c07 8301  r&|.d...j.t.|...
+00008730: 6412 1800 1900 7d09 7c07 6406 1900 6a03  d.....}.|.d...j.
+00008740: 7d0a 740b 7c09 7c00 7c02 6412 7c0a 7c00  }.t.|.|.|.d.|.|.
+00008750: 6403 6412 6413 8d08 7d02 6700 7d0b 6412  d.d.d...}.g.}.d.
+00008760: 7d0c 7406 640c 7407 7c07 8301 8302 4400  }.t.d.t.|.....D.
+00008770: 5dde 7d0d 7c07 6406 1900 6a03 7c0d 1900  ].}.|.d...j.|...
+00008780: 7d09 7c0b a00c 7c09 a101 0100 7c0d 7407  }.|...|.....|.t.
+00008790: 7c07 8301 6412 1800 6b02 9001 72a4 7404  |...d...k...r.t.
+000087a0: a00d 7c0b a101 7d0a 740b 7c09 7c00 7c02  ..|...}.t.|.|.|.
+000087b0: 6412 7c0a 7c00 7c07 6411 1900 6a03 7c0d  d.|.|.|.d...j.|.
+000087c0: 1900 7c0c 6413 8d08 7d02 6700 7d0b 7c0c  ..|.d...}.g.}.|.
+000087d0: 6412 1700 7d0c 6e74 7c07 6411 1900 6a03  d...}.nt|.d...j.
+000087e0: 7c0d 1900 7c07 6411 1900 6a03 7c0d 6412  |...|.d...j.|.d.
+000087f0: 1700 1900 6b02 9001 72e0 7c07 7c03 1900  ....k...r.|.|...
+00008800: 6a03 7c0d 1900 640c 6b01 9001 72e0 9001  j.|...d.k...r...
+00008810: 713c 6e38 7404 a00d 7c0b a101 7d0a 740b  q<n8t...|...}.t.
+00008820: 7c09 7c00 7c02 6412 7c0a 7c00 7c07 6411  |.|.|.d.|.|.|.d.
+00008830: 1900 6a03 7c0d 1900 7c0c 6413 8d08 7d02  ..j.|...|.d...}.
+00008840: 6700 7d0b 7c0c 6412 1700 7d0c 9001 713c  g.}.|.d...}...q<
+00008850: 716a 7c02 5300 2914 7ab1 4368 616e 6765  qj|.S.).z.Change
+00008860: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
+00008870: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
+00008880: 6e65 6564 7320 746f 2062 6520 6d65 7267  needs to be merg
+00008890: 6564 2064 7565 2074 6f20 7265 6d6f 7665  ed due to remove
+000088a0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
+000088b0: 6564 206c 616b 6573 0a20 2020 202d 2d2d  ed lakes.    ---
+000088c0: 2d2d 2d2d 2d2d 2d0a 0a20 2020 204e 6f74  -------..    Not
+000088d0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 0a0a  es.    -------..
+000088e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000088f0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00008900: 204e 6f6e 652c 0a20 2020 2054 7207 0000   None,.    Tr...
+00008910: 0072 6b00 0000 7283 0000 0072 8500 0000  .rk...r....r....
+00008920: 7206 0000 00da 076e 7375 6269 6432 72df  r......nsubid2r.
+00008930: 0000 0072 8000 0000 7281 0000 0072 6600  ...r....r....rf.
+00008940: 0000 7201 0000 0072 6400 0000 7265 0000  ..r....rd...re..
+00008950: 0072 6a00 0000 727a 0000 0072 8400 0000  .rj...rz...r....
+00008960: 7228 0000 0072 e200 0000 290e 7214 0000  r(...r....).r...
+00008970: 0072 e300 0000 7211 0000 0072 1300 0000  .r....r....r....
+00008980: 721a 0000 0072 2b00 0000 7229 0000 0072  r....r+...r)...r
+00008990: 1500 0000 7219 0000 0072 4100 0000 7274  ....r....rA...rt
+000089a0: 0000 0072 a300 0000 724e 0000 0072 e500  ...r....rN...r..
+000089b0: 0000 290e da12 6669 6e61 6c63 6174 5f69  ..)...finalcat_i
+000089c0: 6e66 6f5f 7465 6d70 72f5 0000 0072 8a00  nfo_tempr....r..
+000089d0: 0000 728c 0000 0072 e800 0000 72b7 0000  ..r....r....r...
+000089e0: 0072 ec00 0000 72ed 0000 005a 0a4e 5f48  .r....r....Z.N_H
+000089f0: 796c 616b 6569 6472 e900 0000 72eb 0000  ylakeidr....r...
+00008a00: 0072 ea00 0000 72a1 0000 0072 ee00 0000  .r....r....r....
+00008a10: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00008a20: 4543 6861 6e67 655f 4174 7472 6962 7574  EChange_Attribut
+00008a30: 655f 5661 6c75 6573 5f46 6f72 5f43 6174  e_Values_For_Cat
+00008a40: 6368 6d65 6e74 735f 4e65 6564 5f54 6f5f  chments_Need_To_
+00008a50: 4265 5f4d 6572 6765 645f 4279 5f52 656d  Be_Merged_By_Rem
+00008a60: 6f76 655f 434c 4909 0000 7394 0000 0000  ove_CLI...s.....
+00008a70: 0e0c 0108 0108 010c 010e 0304 010a 0104  ................
+00008a80: 030a 010a 0114 0208 0104 010a 010a ff02  ................
+00008a90: ff08 0410 0310 0110 0102 0322 0116 010a  ..........."....
+00008aa0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00008ab0: 0102 f806 0c04 0104 0112 010e 010a 0312  ................
+00008ac0: 010a 0102 0102 0102 0102 0102 0102 0102  ................
+00008ad0: 010c 0102 f806 0a04 010a 030c 0110 ff02  ................
+00008ae0: ff04 0310 fd04 0506 020a 0102 0102 0102  ................
+00008af0: 0102 0102 0102 0102 010c 0102 f806 0a04  ................
+00008b00: 010e 0172 fa00 0000 6303 0000 0000 0000  ...r....c.......
+00008b10: 0000 0000 000f 0000 000a 0000 0043 0000  .............C..
+00008b20: 0073 0002 0000 7c02 6a00 6401 6701 6402  .s....|.j.d.g.d.
+00008b30: 6701 6403 8d02 7d02 7401 6404 7402 7c02  g.d...}.t.d.t.|.
+00008b40: 8301 8302 4400 9001 5da4 7d03 7c02 6405  ....D...].}.|.d.
+00008b50: 1900 6a03 7c03 1900 7d04 7c01 6a04 7c01  ..j.|...}.|.j.|.
+00008b60: 6405 1900 7c04 6b02 1900 a005 a100 7d05  d...|.k.......}.
+00008b70: 7402 7c05 8301 6406 6b03 7268 7406 6407  t.|...d.k.rht.d.
+00008b80: 8301 0100 7406 7c05 8301 0100 7120 6700  ....t.|.....q g.
+00008b90: 7d06 7c05 6408 1900 6a03 6404 1900 7d07  }.|.d...j.d...}.
+00008ba0: 7c05 6409 1900 6a03 6404 1900 7d08 7c06  |.d...j.d...}.|.
+00008bb0: a007 7c07 a101 0100 640a 7d09 6404 7d0a  ..|.....d.}.d.}.
+00008bc0: 7c01 6a04 7c01 6408 1900 7c08 6b02 1900  |.j.|.d...|.k...
+00008bd0: a005 a100 7d0b 7402 7c0b 8301 6404 6b02  ....}.t.|...d.k.
+00008be0: 72c6 7c08 6404 6b00 72c6 7120 7c0b 640b  r.|.d.k.r.q |.d.
+00008bf0: 1900 6a03 6404 1900 640c 6b03 9001 7228  ..j.d...d.k...r(
+00008c00: 7c00 6a04 7c00 6408 1900 7c08 6b02 1900  |.j.|.d...|.k...
+00008c10: 640d 1900 6a03 6404 1900 7d0c 7c0c 6404  d...j.d...}.|.d.
+00008c20: 6b04 9001 7214 7c0c 7d09 6406 7d0a 7c06  k...r.|.}.d.}.|.
+00008c30: a007 7c09 a101 0100 6e12 7c08 7d09 640a  ..|.....n.|.}.d.
+00008c40: 7d0a 7c06 a007 7c09 a101 0100 6e4c 7c00  }.|...|.....nL|.
+00008c50: 6a04 7c00 6408 1900 7c08 6b02 1900 640d  j.|.d...|.k...d.
+00008c60: 1900 6a03 6404 1900 7d0c 7c0c 6404 6b04  ..j.d...}.|.d.k.
+00008c70: 9001 7262 7c0c 7d09 6406 7d0a 7c06 a007  ..rb|.}.d.}.|...
+00008c80: 7c09 a101 0100 6e12 7c08 7d09 640a 7d0a  |.....n.|.}.d.}.
+00008c90: 7c06 a007 7c09 a101 0100 7c00 7c00 6408  |...|.....|.|.d.
+00008ca0: 1900 7c09 6b02 1900 6405 1900 6a03 6404  ..|.k...d...j.d.
+00008cb0: 1900 7d0d 7c0a 6404 6b04 9001 72b0 7408  ..}.|.d.k...r.t.
+00008cc0: 7c09 7c00 7c00 6406 7c06 7c01 7c0d 640e  |.|.|.d.|.|.|.d.
+00008cd0: 8d07 7d00 7120 7408 7c09 7c00 7c00 6406  ..}.q t.|.|.|.d.
+00008ce0: 7c06 7c01 7c0d 640e 8d07 7d00 7120 7c00  |.|.|.d...}.q |.
+00008cf0: 640d 1900 6404 6b01 7d0e 7c00 6a04 7c0e  d...d.k.}.|.j.|.
+00008d00: 640f 6602 1900 6a03 7c00 6a04 7c0e 640d  d.f...j.|.j.|.d.
+00008d10: 6602 3c00 7c00 6a09 640f 6701 6410 8d01  f.<.|.j.d.g.d...
+00008d20: 0100 7c00 5300 2911 7ab5 4368 616e 6765  ..|.S.).z.Change
+00008d30: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
+00008d40: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
+00008d50: 6e65 6564 7320 746f 2062 6520 6d65 7267  needs to be merg
+00008d60: 6564 2064 7565 2074 6f20 7265 6d6f 7665  ed due to remove
+00008d70: 0a20 2020 2020 2020 206e 6f6e 2063 6f6e  .        non con
+00008d80: 6e65 6374 6564 206c 616b 6573 0a20 2020  nected lakes.   
+00008d90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020   ----------..   
+00008da0: 204e 6f74 6573 0a20 2020 202d 2d2d 2d2d   Notes.    -----
+00008db0: 2d2d 0a0a 2020 2020 5265 7475 726e 733a  --..    Returns:
+00008dc0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00008dd0: 2020 2020 204e 6f6e 652c 0a20 2020 2072       None,.    r
+00008de0: 7900 0000 4672 7a00 0000 7201 0000 0072  y...Frz...r....r
+00008df0: 8400 0000 7228 0000 007a 2849 7420 6973  ....r(...z(It is
+00008e00: 206e 6f74 2061 206e 6f6e 2063 6f6e 6e65   not a non conne
+00008e10: 6374 6564 206c 616b 6520 6361 7463 686d  cted lake catchm
+00008e20: 656e 7472 0600 0000 720d 0000 0072 6b00  entr....r....rk.
+00008e30: 0000 7264 0000 0072 6500 0000 7283 0000  ..rd...re...r...
+00008e40: 00a9 0772 4900 0000 729d 0000 0072 8a00  ...rI...r....r..
+00008e50: 0000 729e 0000 0072 9f00 0000 72a0 0000  ..r....r....r...
+00008e60: 0072 6400 0000 72f8 0000 0072 1000 0000  .rd...r....r....
+00008e70: 290a 7241 0000 0072 2900 0000 7215 0000  ).rA...r)...r...
+00008e80: 0072 1300 0000 7219 0000 0072 1400 0000  .r....r....r....
+00008e90: 7275 0000 0072 4e00 0000 72a3 0000 0072  ru...rN...r....r
+00008ea0: 1c00 0000 290f 728a 0000 0072 f900 0000  ....).r....r....
+00008eb0: 72f6 0000 0072 4800 0000 5a17 5265 6d6f  r....rH...Z.Remo
+00008ec0: 7665 5f4e 6f6e 5f43 6f6e 6e4c 5f4c 616b  ve_Non_ConnL_Lak
+00008ed0: 6569 645a 1e52 656d 6f76 655f 4e6f 6e5f  eidZ.Remove_Non_
+00008ee0: 436f 6e6e 4c5f 4c61 6b65 5f53 7562 5f69  ConnL_Lake_Sub_i
+00008ef0: 6e66 6f72 ea00 0000 72cc 0000 0072 cb00  nfor....r....r..
+00008f00: 0000 72e9 0000 005a 0f69 735f 7072 655f  ..r....Z.is_pre_
+00008f10: 6d6f 6469 6669 6564 72c6 0000 0072 8300  modifiedr....r..
+00008f20: 0000 5a0b 5461 725f 4c61 6b65 5f49 645a  ..Z.Tar_Lake_IdZ
+00008f30: 0f75 6e70 726f 6365 7373 6564 6d61 736b  .unprocessedmask
+00008f40: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
+00008f50: 4643 6861 6e67 655f 4174 7472 6962 7574  FChange_Attribut
+00008f60: 655f 5661 6c75 6573 5f46 6f72 5f43 6174  e_Values_For_Cat
+00008f70: 6368 6d65 6e74 735f 4e65 6564 5f54 6f5f  chments_Need_To_
+00008f80: 4265 5f4d 6572 6765 645f 4279 5f52 656d  Be_Merged_By_Rem
+00008f90: 6f76 655f 4e43 4cb0 0900 0073 a400 0000  ove_NCL....s....
+00008fa0: 000f 0401 08ff 0603 1401 0801 02ff 0403  ................
+00008fb0: 0401 0aff 0803 0c01 0801 0801 0201 0401  ................
+00008fc0: 0e01 0801 02ff 0403 0a01 0401 0402 0401  ................
+00008fd0: 0aff 0803 1401 0201 1402 1001 02ff 0403  ................
+00008fe0: 02fd 0406 0a01 0401 0401 0c02 0401 0401  ................
+00008ff0: 0c04 1001 02ff 0402 02fe 0403 0a01 0401  ................
+00009000: 0401 0c02 0402 0401 0a02 0e01 02ff 0402  ................
+00009010: 02fe 0404 0a01 0201 0201 0201 0201 0201  ................
+00009020: 0201 0201 02f9 080a 0201 0201 0201 0201  ................
+00009030: 0201 0201 0201 02f9 080a 0c02 0401 06ff  ................
+00009040: 1004 0e02 72fc 0000 0063 0100 0000 0000  ....r....c......
+00009050: 0000 0000 0000 0900 0000 0a00 0000 4300  ..............C.
+00009060: 0000 73cc 0000 0064 017d 017c 006a 0064  ..s....d.}.|.j.d
+00009070: 0264 038d 017d 027c 0264 0119 006a 017c  .d...}.|.d...j.|
+00009080: 0264 043c 007c 0264 0419 00a0 0264 05a1  .d.<.|.d.....d..
+00009090: 017c 0264 043c 007c 0064 0619 006a 017d  .|.d.<.|.d...j.}
+000090a0: 037c 037c 0364 076b 0419 007d 0374 03a0  .|.|.d.k...}.t..
+000090b0: 047c 03a1 017d 0374 0564 0774 067c 0383  .|...}.t.d.t.|..
+000090c0: 0183 0244 005d 687d 047c 037c 0419 007d  ...D.]h}.|.|...}
+000090d0: 057c 006a 077c 0064 0619 007c 056b 0219  .|.j.|.d...|.k..
+000090e0: 007d 067c 066a 0864 0867 0164 0964 0a8d  .}.|.j.d.g.d.d..
+000090f0: 027d 067c 067c 0119 006a 0164 0719 007d  .}.|.|...j.d...}
+00009100: 077c 067c 0119 006a 017d 0874 067c 0883  .|.|...j.}.t.|..
+00009110: 0164 0b6b 0472 5e74 097c 077c 007c 0264  .d.k.r^t.|.|.|.d
+00009120: 0b7c 087c 0064 0b64 0c8d 077d 0271 5e7c  .|.|.d.d...}.q^|
+00009130: 0253 0029 0de1 2c01 0000 4368 616e 6765  .S.)..,...Change
+00009140: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
+00009150: 6361 7463 686d 656e 7473 2074 6861 7420  catchments that 
+00009160: 636f 7665 7265 6420 6279 2074 6865 2073  covered by the s
+00009170: 616d 6520 6c61 6b65 2e0a 2020 2020 2d2d  ame lake..    --
+00009180: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 4e6f  --------..    No
+00009190: 7465 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  tes.    -------.
+000091a0: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
+000091b0: 706c 652c 206c 616b 6520 276c 6127 2063  ple, lake 'la' c
+000091c0: 6f76 6572 696e 6720 6361 7463 686d 656e  overing catchmen
+000091d0: 7420 612c 622c 632e 2074 6865 206c 616b  t a,b,c. the lak
+000091e0: 6520 6f75 746c 6574 2063 6174 6368 6d65  e outlet catchme
+000091f0: 6e74 0a20 2020 2020 2020 2069 7320 612e  nt.        is a.
+00009200: 2074 6865 6e20 7468 6973 2066 756e 6374   then this funct
+00009210: 696f 6e20 7769 6c6c 2063 6861 6e67 6520  ion will change 
+00009220: 6174 7472 6962 7574 6520 6f66 2062 2061  attribute of b a
+00009230: 6e64 2063 2074 6f20 612e 0a20 2020 2052  nd c to a..    R
+00009240: 6574 7572 6e73 3a0a 2020 2020 2d2d 2d2d  eturns:.    ----
+00009250: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
+00009260: 2c0a 2020 2020 7206 0000 0054 7207 0000  ,.    r....Tr...
+00009270: 0072 8300 0000 7209 0000 0072 8400 0000  .r....r....r....
+00009280: 7201 0000 0072 7900 0000 4672 7a00 0000  r....ry...Frz...
+00009290: 7228 0000 0072 fb00 0000 290a 7214 0000  r(...r....).r...
+000092a0: 0072 1300 0000 7216 0000 0072 1a00 0000  .r....r....r....
+000092b0: 722b 0000 0072 2900 0000 7215 0000 0072  r+...r)...r....r
+000092c0: 1900 0000 7241 0000 0072 a300 0000 a909  ....rA...r......
+000092d0: 5a10 6669 6e61 6c72 6976 706c 795f 696e  Z.finalrivply_in
+000092e0: 666f 72a2 0000 0072 8a00 0000 5a11 416c  for....r....Z.Al
+000092f0: 6c43 6f6e 6e65 6374 4c61 6b65 4944 5372  lConnectLakeIDSr
+00009300: 4800 0000 5a06 6c61 6b65 6964 5a0c 4c61  H...Z.lakeidZ.La
+00009310: 6b65 7375 625f 696e 666f 72e9 0000 005a  kesub_infor....Z
+00009320: 0a6c 616b 6573 7562 6964 7372 2400 0000  .lakesubidsr$...
+00009330: 7224 0000 0072 2500 0000 da3b 4368 616e  r$...r%....;Chan
+00009340: 6765 5f41 7474 7269 6275 7465 5f56 616c  ge_Attribute_Val
+00009350: 7565 735f 466f 725f 4361 7463 686d 656e  ues_For_Catchmen
+00009360: 7473 5f43 6f76 6572 6564 5f42 795f 5361  ts_Covered_By_Sa
+00009370: 6d65 5f4c 616b 651f 0a00 0073 3400 0000  me_Lake....s4...
+00009380: 000d 0401 0c01 0e01 1201 0a01 0c01 0a03  ................
+00009390: 1201 0801 1201 1001 0801 02ff 0403 0a01  ................
+000093a0: 0c01 0201 0201 0201 0201 0201 0201 0201  ................
+000093b0: 02f9 0809 72ff 0000 0063 0300 0000 0000  ....r....c......
+000093c0: 0000 0000 0000 0800 0000 0600 0000 4300  ..............C.
+000093d0: 0000 7368 0000 0074 007c 007c 0183 027d  ..sh...t.|.|...}
+000093e0: 037c 0264 016b 0472 6074 007c 007c 0283  .|.d.k.r`t.|.|..
+000093f0: 027d 0474 0174 027c 0483 0183 0144 005d  .}.t.t.|.....D.]
+00009400: 307d 057c 047c 0519 007c 026b 0272 3a71  0}.|.|...|.k.r:q
+00009410: 2874 03a0 047c 037c 047c 0519 006b 02a1  (t...|.|.|...k..
+00009420: 017d 0674 03a0 057c 037c 06a1 027d 0371  .}.t...|.|...}.q
+00009430: 287c 037d 076e 047c 037d 077c 0753 0029  (|.}.n.|.}.|.S.)
+00009440: 027a 9552 6574 7572 6e20 7375 6269 6420  .z.Return subid 
+00009450: 6f66 2073 7562 6261 7369 6e73 2062 6574  of subbasins bet
+00009460: 7765 656e 2074 776f 2073 7562 6964 2069  ween two subid i
+00009470: 6e20 7468 6520 726f 7574 696e 6720 6e65  n the routing ne
+00009480: 7477 6f72 6b0a 2020 2020 2d2d 2d2d 2d2d  twork.    ------
+00009490: 2d2d 2d2d 0a0a 2020 2020 4e6f 7465 730a  ----..    Notes.
+000094a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 0a20 2020      -------..   
+000094b0: 2052 6574 7572 6e73 3a0a 2020 2020 2d2d   Returns:.    --
+000094c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+000094d0: 6e65 2c0a 2020 2020 7201 0000 0029 0672  ne,.    r....).r
+000094e0: 1700 0000 7229 0000 0072 1500 0000 721a  ....r)...r....r.
+000094f0: 0000 0072 b900 0000 da06 6465 6c65 7465  ...r......delete
+00009500: 2908 7277 0000 005a 1073 7562 6964 5f64  ).rw...Z.subid_d
+00009510: 6f77 6e73 7472 6561 6d5a 0e73 7562 6964  ownstreamZ.subid
+00009520: 5f75 7073 7472 6561 6dda 0c48 7964 726f  _upstream..Hydro
+00009530: 4261 7369 6e73 315a 0c48 7964 726f 4261  Basins1Z.HydroBa
+00009540: 7369 6e73 3272 4800 0000 da04 726f 7773  sins2rH.....rows
+00009550: da0b 4879 6472 6f42 6173 696e 7372 2400  ..HydroBasinsr$.
+00009560: 0000 7224 0000 0072 2500 0000 da35 5265  ..r$...r%....5Re
+00009570: 7475 726e 5f53 7562 4964 735f 4265 7477  turn_SubIds_Betw
+00009580: 6565 6e5f 5477 6f5f 5375 6262 6173 696e  een_Two_Subbasin
+00009590: 735f 496e 5f52 6f75 696e 675f 4e65 7477  s_In_Rouing_Netw
+000095a0: 6f72 6b4a 0a00 0073 1a00 0000 000e 0201  orkJ...s........
+000095b0: 04ff 0404 0801 0a01 1001 0c01 0201 1201  ................
+000095c0: 0e01 0602 0402 7204 0100 0063 0600 0000  ......r....c....
+000095d0: 0000 0000 0000 0000 2000 0000 0800 0000  ........ .......
+000095e0: 4300 0000 7344 0400 007c 0464 0164 0267  C...sD...|.d.d.g
+000095f0: 0219 00a0 0064 03a1 016a 017d 0674 02a0  .....d...j.}.t..
+00009600: 037c 007c 0166 02a1 017d 077c 077c 0764  .|.|.f...}.|.|.d
+00009610: 0064 0085 0264 0466 0219 00a0 04a1 0019  .d...d.f........
+00009620: 007d 0774 02a0 037c 027c 0366 02a1 017d  .}.t...|.|.f...}
+00009630: 087c 087c 0864 0064 0085 0264 0466 0219  .|.|.d.d...d.f..
+00009640: 00a0 04a1 0019 007d 0874 026a 057c 077c  .......}.t.j.|.|
+00009650: 0864 0564 068d 037d 0774 02a0 0674 02a0  .d.d...}.t...t..
+00009660: 077c 0764 0064 0085 0264 0566 0219 00a1  .|.d.d...d.f....
+00009670: 01a1 017d 0974 02a0 0674 02a0 077c 0764  ...}.t...t...|.d
+00009680: 0064 0085 0264 0766 0219 00a1 01a1 017d  .d...d.f.......}
+00009690: 0a74 02a0 0874 097c 0783 0164 0566 0274  .t...t.|...d.f.t
+000096a0: 026a 0aa1 027d 0b74 0b64 0474 097c 0983  .j...}.t.d.t.|..
+000096b0: 0183 0244 005d 407d 0c7c 097c 0c19 007d  ...D.]@}.|.|...}
+000096c0: 0d7c 046a 0c7c 0464 0119 007c 0d6b 0219  .|.j.|.d...|.k..
+000096d0: 0064 0819 006a 0164 0419 007d 0e7c 0e7c  .d...j.d...}.|.|
+000096e0: 0b7c 0764 0064 0085 0264 0566 0219 007c  .|.d.d...d.f...|
+000096f0: 0d6b 023c 0071 cc74 026a 057c 077c 0b64  .k.<.q.t.j.|.|.d
+00009700: 0564 068d 037d 0767 007d 0f67 007d 1067  .d...}.g.}.g.}.g
+00009710: 007d 1174 0b64 0474 097c 0a83 0183 0244  .}.t.d.t.|.....D
+00009720: 0090 025d e67d 0c7c 0a7c 0c19 007d 037c  ...].}.|.|...}.|
+00009730: 077c 0764 0064 0085 0264 0766 0219 007c  .|.d.d...d.f...|
+00009740: 036b 0219 007d 127c 127c 1264 0064 0085  .k...}.|.|.d.d..
+00009750: 0264 0966 0219 00a0 04a1 0019 007d 127c  .d.f.........}.|
+00009760: 1274 097c 1283 0164 0518 0064 0566 0219  .t.|...d...d.f..
+00009770: 007d 137c 046a 0c7c 0464 0119 00a0 0d7c  .}.|.j.|.d.....|
+00009780: 1264 0064 0085 0264 0566 0219 00a1 0119  .d.d...d.f......
+00009790: 007d 1474 097c 1283 0164 056b 0290 0272  .}.t.|...d.k...r
+000097a0: 0c7c 1264 0a19 007d 157c 056a 0c7c 0564  .|.d...}.|.j.|.d
+000097b0: 0b19 007c 156b 0219 0064 0c19 006a 0164  ...|.k...d...j.d
+000097c0: 0419 007c 036b 0390 0172 f67c 10a0 0574  ...|.k...r.|...t
+000097d0: 0e7c 1264 0a19 0083 01a1 0101 006e 127c  .|.d.........n.|
+000097e0: 0fa0 0574 0e7c 1264 0d19 0083 01a1 0101  ...t.|.d........
+000097f0: 0090 0171 3874 0f7c 067c 1383 027d 1674  ...q8t.|.|...}.t
+00009800: 02a0 067c 1264 0064 0085 0264 0566 0219  ...|.d.d...d.f..
+00009810: 00a1 017d 1774 0b64 0474 097c 1283 0183  ...}.t.d.t.|....
+00009820: 0244 0090 015d e07d 187c 127c 1864 0566  .D...].}.|.|.d.f
+00009830: 0219 007d 157c 157c 136b 0390 0372 667c  ...}.|.|.k...rf|
+00009840: 11a0 0574 0e7c 127c 1864 0566 0219 0083  ...t.|.|.d.f....
+00009850: 01a1 0101 0074 097c 046a 0c7c 0464 0119  .....t.|.j.|.d..
+00009860: 007c 156b 0219 0083 0164 046b 0490 0372  .|.k.....d.k...r
+00009870: 667c 046a 0c7c 0464 0119 007c 156b 0219  f|.j.|.d...|.k..
+00009880: 0064 0219 006a 0164 0419 007d 197c 197c  .d...j.d...}.|.|
+00009890: 1676 0090 0372 667c 197c 1264 0064 0085  .v...rf|.|.d.d..
+000098a0: 0264 0566 0219 0076 0190 0372 667c 11a0  .d.f...v...rf|..
+000098b0: 0574 0e7c 1983 01a1 0101 007c 197d 1a64  .t.|.......|.}.d
+000098c0: 047d 1b7c 1b64 0e6b 0090 0372 667c 1b64  .}.|.d.k...rf|.d
+000098d0: 0517 007d 1b74 097c 046a 0c7c 0464 0119  ...}.t.|.j.|.d..
+000098e0: 007c 1a6b 0219 0083 0164 046b 0490 0372  .|.k.....d.k...r
+000098f0: 667c 046a 0c7c 0464 0119 007c 1a6b 0219  f|.j.|.d...|.k..
+00009900: 0064 0219 006a 0164 0419 007d 1c7c 1c7c  .d...j.d...}.|.|
+00009910: 1264 0064 0085 0264 0566 0219 0076 0190  .d.d...d.f...v..
+00009920: 0372 667c 1c7c 1676 0090 0372 667c 11a0  .rf|.|.v...rf|..
+00009930: 0574 0e7c 1c83 01a1 0101 007c 1c7d 1a6e  .t.|.......|.}.n
+00009940: 0490 0371 666e 0490 0371 6690 0271 da74  ...qfn...qf..q.t
+00009950: 0f7c 067c 1583 027d 1d74 097c 1d83 0164  .|.|...}.t.|...d
+00009960: 046b 0490 0372 a474 02a0 0d7c 1d7c 17a1  .k...r.t...|.|..
+00009970: 027d 1e74 107c 1e83 0164 0f6b 0590 0372  .}.t.|...d.k...r
+00009980: 9e64 107d 1f6e 0464 117d 1f6e 0464 117d  .d.}.n.d.}.n.d.}
+00009990: 1f74 097c 146a 0c7c 1464 0219 007c 156b  .t.|.j.|.d...|.k
+000099a0: 0219 0083 0164 046b 0490 0373 ec7c 056a  .....d.k...s.|.j
+000099b0: 0c7c 0564 0b19 007c 156b 0219 0064 0c19  .|.d...|.k...d..
+000099c0: 006a 0164 0419 007c 036b 0290 0373 ec7c  .j.d...|.k...s.|
+000099d0: 1f90 0472 047c 0fa0 0574 0e7c 127c 1864  ...r.|...t.|.|.d
+000099e0: 0466 0219 0083 01a1 0101 006e 167c 10a0  .f.........n.|..
+000099f0: 0574 0e7c 127c 1864 0566 0219 0083 01a1  .t.|.|.d.f......
+00009a00: 0101 0090 0271 3a90 0171 3874 1174 127c  .....q:..q8t.t.|
+00009a10: 1183 0183 0174 1174 127c 0f83 0183 0174  .....t.t.|.....t
+00009a20: 1174 127c 1083 0183 0166 0353 0029 124e  .t.|.....f.S.).N
+00009a30: 7206 0000 0072 0d00 0000 722d 0000 0072  r....r....r-...r
+00009a40: 0100 0000 7228 0000 0072 0e00 0000 72e1  ....r(...r....r.
+00009a50: 0000 00da 0a4d 6178 4163 635f 6361 74e9  .....MaxAcc_cat.
+00009a60: 0400 0000 2902 7201 0000 0072 2800 0000  ....).r....r(...
+00009a70: 5a08 494c 5f53 7562 4964 5a08 736c 5f63  Z.IL_SubIdZ.sl_c
+00009a80: 6c5f 6964 2902 7201 0000 0072 0100 0000  l_id).r....r....
+00009a90: 727b 0000 0072 6500 0000 5446 2913 7216  r{...re...TF).r.
+00009aa0: 0000 0072 1300 0000 721a 0000 00da 0c63  ...r....r......c
+00009ab0: 6f6c 756d 6e5f 7374 6163 6bda 0761 7267  olumn_stack..arg
+00009ac0: 736f 7274 724e 0000 0072 2b00 0000 72f0  sortrN...r+...r.
+00009ad0: 0000 0072 7d00 0000 7215 0000 0072 d100  ...r}...r....r..
+00009ae0: 0000 7229 0000 0072 1900 0000 7212 0000  ..r)...r....r...
+00009af0: 0072 2d00 0000 7217 0000 0072 3f00 0000  .r-...r....r?...
+00009b00: 7254 0000 0072 c900 0000 2920 5a0b 7269  rT...r....) Z.ri
+00009b10: 765f 6c61 6b65 5f69 645a 0673 7472 5f69  v_lake_idZ.str_i
+00009b20: 645a 0c72 6976 5f6c 616b 655f 6964 325a  dZ.riv_lake_id2Z
+00009b30: 0563 6c5f 6964 7277 0000 005a 1373 7472  .cl_idrw...Z.str
+00009b40: 5f73 7461 7274 5f70 745f 6c61 6b65 6964  _start_pt_lakeid
+00009b50: 5a11 726f 7574 696e 675f 696e 666f 5f72  Z.routing_info_r
+00009b60: 6f75 745a 0872 6976 5f6c 616b 655a 0b72  outZ.riv_lakeZ.r
+00009b70: 6976 5f6c 616b 655f 636c 5a0d 7374 725f  iv_lake_clZ.str_
+00009b80: 6964 5f75 6e69 7175 655a 0c63 6c5f 6964  id_uniqueZ.cl_id
+00009b90: 5f75 6e69 7175 655a 0a61 6363 5f73 7472  _uniqueZ.acc_str
+00009ba0: 5f63 6c72 4800 0000 da05 7374 7269 64da  _clrH.....strid.
+00009bb0: 066d 6178 6163 635a 146e 6f6e 5f6c 616b  .maxaccZ.non_lak
+00009bc0: 655f 696e 666c 6f77 5f73 6567 735a 1273  e_inflow_segsZ.s
+00009bd0: 7472 5f69 645f 6c61 6b65 5f69 6e6c 666f  tr_id_lake_inlfo
+00009be0: 775a 1373 7472 5f69 645f 7769 7468 696e  wZ.str_id_within
+00009bf0: 5f6c 616b 6573 5a0b 7269 765f 6c61 6b65  _lakesZ.riv_lake
+00009c00: 5f69 6c5a 0a6f 7574 6c65 745f 7374 725a  _ilZ.outlet_strZ
+00009c10: 1073 7562 5f72 6f75 7469 6e67 5f69 6e66  .sub_routing_inf
+00009c20: 6f5a 0b73 7472 5f69 645f 636c 5f6a 5a13  oZ.str_id_cl_jZ.
+00009c30: 7374 7273 5f74 6f5f 6c61 6b65 5f6f 7574  strs_to_lake_out
+00009c40: 6c65 745a 1875 6e69 7175 655f 7374 725f  letZ.unique_str_
+00009c50: 6964 5f63 765f 6279 5f6c 616b 6572 5e00  id_cv_by_laker^.
+00009c60: 0000 5a1a 646f 776e 5f73 756e 5f6f 665f  ..Z.down_sun_of_
+00009c70: 6c61 6b65 5f63 6f76 6572 5f73 7472 5a06  lake_cover_strZ.
+00009c80: 6373 7472 6964 5a03 6b5f 645a 0764 7374  cstridZ.k_dZ.dst
+00009c90: 725f 6964 5a0b 7570 5f73 7472 5f63 6c5f  r_idZ.up_str_cl_
+00009ca0: 6a72 2300 0000 5a11 6861 735f 7570 5f73  jr#...Z.has_up_s
+00009cb0: 7472 5f69 6e6c 616b 6572 2400 0000 7224  tr_inlaker$...r$
+00009cc0: 0000 0072 2500 0000 da31 7265 7475 726e  ...r%....1return
+00009cd0: 5f6e 6f6e 5f6c 616b 655f 696e 666c 6f77  _non_lake_inflow
+00009ce0: 5f73 6567 735f 616e 645f 7365 6773 5f77  _segs_and_segs_w
+00009cf0: 6974 6869 6e5f 6c61 6b65 736a 0a00 0073  ithin_lakesj...s
+00009d00: ae00 0000 0004 1402 0e01 1801 0e01 1801  ................
+00009d10: 1003 1c01 1c02 1601 1201 0803 1601 02ff  ................
+00009d20: 0403 1a01 1005 0401 0401 0401 1402 0802  ................
+00009d30: 1801 1801 1401 0401 18ff 0405 0e01 0803  ................
+00009d40: 1001 02ff 0402 02fe 0203 02fd 02ff 0406  ................
+00009d50: 1402 1201 0402 0a07 1602 1401 0c03 0a01  ................
+00009d60: 1602 1c02 1c03 2003 0e02 0401 0401 0a01  ...... .........
+00009d70: 0801 1c01 1c02 2001 0e01 0602 0602 0803  ...... .........
+00009d80: 0a02 0e04 0c01 0e01 0602 0602 0403 1401  ................
+00009d90: 02ff 02ff 0403 0401 0aff 0202 02fe 0402  ................
+00009da0: 02fe 0203 02fd 02fd 0407 02f9 040b 1802  ................
+00009db0: 1e02 720b 0100 0063 0300 0000 0000 0000  ..r....c........
+00009dc0: 0000 0000 1500 0000 0600 0000 4300 0000  ............C...
+00009dd0: 73d8 0100 0067 007d 0367 007d 0474 00a0  s....g.}.g.}.t..
+00009de0: 017c 007c 0166 02a1 017d 0574 00a0 0274  .|.|.f...}.t...t
+00009df0: 00a0 037c 01a1 01a1 017d 0674 00a0 0274  ...|.....}.t...t
+00009e00: 00a0 037c 00a1 01a1 017d 0774 00a0 0474  ...|.....}.t...t
+00009e10: 057c 0583 0164 0166 0274 006a 06a1 027d  .|...d.f.t.j...}
+00009e20: 0874 0764 0274 057c 0683 0183 0244 005d  .t.d.t.|.....D.]
+00009e30: 407d 097c 067c 0919 007d 0a7c 026a 087c  @}.|.|...}.|.j.|
+00009e40: 0264 0319 007c 0a6b 0219 0064 0419 006a  .d...|.k...d...j
+00009e50: 0964 0219 007d 0b7c 0b7c 087c 0564 0064  .d...}.|.|.|.d.d
+00009e60: 0085 0264 0166 0219 007c 0a6b 023c 0071  ...d.f...|.k.<.q
+00009e70: 5a74 006a 0a7c 057c 0864 0164 058d 037d  Zt.j.|.|.d.d...}
+00009e80: 057c 057c 0564 0064 0085 0264 0666 0219  .|.|.d.d...d.f..
+00009e90: 00a0 0ba1 0019 007d 057c 0264 0364 0767  .......}.|.d.d.g
+00009ea0: 0219 00a0 0c64 08a1 016a 097d 0c74 0764  .....d...j.}.t.d
+00009eb0: 0274 057c 0783 0183 0244 005d e87d 097c  .t.|.....D.].}.|
+00009ec0: 077c 0919 007d 0d7c 057c 0564 0064 0085  .|...}.|.|.d.d..
+00009ed0: 0264 0266 0219 007c 0d6b 0219 007d 0e74  .d.f...|.k...}.t
+00009ee0: 057c 0e83 0164 016b 0190 0172 1a71 e67c  .|...d.k...r.q.|
+00009ef0: 0e74 057c 0e83 0164 0118 0064 0166 0219  .t.|...d...d.f..
+00009f00: 007d 0f74 0d7c 0c7c 0f83 027d 1074 00a0  .}.t.|.|...}.t..
+00009f10: 0e7c 0e64 0064 0085 0264 0166 0219 007c  .|.d.d...d.f...|
+00009f20: 10a1 027d 1167 007d 1274 057c 117c 1164  ...}.g.}.t.|.|.d
+00009f30: 096b 0219 0083 0174 057c 0e64 0064 0085  .k.....t.|.d.d..
+00009f40: 0264 0166 0219 0083 016b 0072 e67c 0e74  .d.f.....k.r.|.t
+00009f50: 00a0 0f7c 11a1 0164 0166 0219 007d 1374  ...|...d.f...}.t
+00009f60: 0764 0274 057c 1383 0183 0244 005d 227d  .d.t.|.....D.]"}
+00009f70: 147c 137c 1419 007d 0a7c 0a7c 0f6b 0390  .|.|...}.|.|.k..
+00009f80: 0172 987c 12a0 0a7c 0aa1 0101 0090 0171  .r.|...|.......q
+00009f90: 987c 047c 1217 007d 047c 03a0 0a7c 0da1  .|.|...}.|...|..
+00009fa0: 0101 0071 e67c 037c 0466 0253 0029 0a4e  ...q.|.|.f.S.).N
+00009fb0: 7228 0000 0072 0100 0000 7206 0000 0072  r(...r....r....r
+00009fc0: 0501 0000 720e 0000 0072 6500 0000 720d  ....r....re...r.
+00009fd0: 0000 0072 2d00 0000 5429 1072 1a00 0000  ...r-...T).r....
+00009fe0: 7207 0100 0072 2b00 0000 72f0 0000 0072  r....r+...r....r
+00009ff0: 7d00 0000 7215 0000 0072 d100 0000 7229  }...r....r....r)
+0000a000: 0000 0072 1900 0000 7213 0000 0072 4e00  ...r....r....rN.
+0000a010: 0000 7208 0100 0072 1600 0000 7217 0000  ..r....r....r...
+0000a020: 0072 1200 0000 729a 0000 0029 155a 0543  .r....r....).Z.C
+0000a030: 4c5f 4964 5a06 5374 725f 4964 5a0c 526f  L_IdZ.Str_IdZ.Ro
+0000a040: 7574 696e 675f 696e 666f 5a17 4c61 6b65  uting_infoZ.Lake
+0000a050: 735f 5749 7468 5f4d 756c 7469 5f4f 7574  s_WIth_Multi_Out
+0000a060: 6c65 745a 0a52 656d 6f76 655f 5374 725a  letZ.Remove_StrZ
+0000a070: 0643 4c5f 5374 725a 0d53 7472 5f49 645f  .CL_StrZ.Str_Id_
+0000a080: 756e 6971 7565 5a0c 434c 5f49 645f 756e  uniqueZ.CL_Id_un
+0000a090: 6971 7565 5a0a 4163 635f 5374 725f 434c  iqueZ.Acc_Str_CL
+0000a0a0: 7248 0000 0072 0901 0000 720a 0100 005a  rH...r....r....Z
+0000a0b0: 1172 6f75 7469 6e67 5f69 6e66 6f5f 6f6e  .routing_info_on
+0000a0c0: 6c79 5a07 6c61 6b65 5f69 645a 0869 5f43  lyZ.lake_idZ.i_C
+0000a0d0: 4c5f 5374 725a 0b73 7472 5f6d 6178 5f61  L_StrZ.str_max_a
+0000a0e0: 6363 5a12 7374 725f 746f 5f73 7472 5f6d  ccZ.str_to_str_m
+0000a0f0: 6178 5f61 6363 7223 0000 005a 0c52 656d  ax_accr#...Z.Rem
+0000a100: 6f76 655f 5374 725f 695a 1873 7472 5f6e  ove_Str_iZ.str_n
+0000a110: 6f74 666c 6f77 746f 5f6c 616b 656f 7574  otflowto_lakeout
+0000a120: 6c65 745a 0469 7374 7272 2400 0000 7224  letZ.istrr$...r$
+0000a130: 0000 0072 2500 0000 da1f 4368 6563 6b5f  ...r%.....Check_
+0000a140: 4966 5f4c 616b 655f 4861 7665 5f4d 756c  If_Lake_Have_Mul
+0000a150: 7469 5f4f 7574 4c65 74ef 0a00 0073 4200  ti_OutLet....sB.
+0000a160: 0000 0003 0401 0402 0e02 1002 1003 1601  ................
+0000a170: 1201 0801 1601 02ff 0403 1a01 1003 1803  ................
+0000a180: 1403 1202 0802 1803 0e01 0208 1403 0a08  ................
+0000a190: 1804 0403 2402 1202 1202 0805 0a01 0e05  ....$...........
+0000a1a0: 0801 0c02 720c 0100 0063 0100 0000 0000  ....r....c......
+0000a1b0: 0000 0000 0000 0900 0000 0a00 0000 4300  ..............C.
+0000a1c0: 0000 73ba 0000 0064 017d 017c 006a 0064  ..s....d.}.|.j.d
+0000a1d0: 0264 038d 017d 027c 0264 0119 006a 017c  .d...}.|.d...j.|
+0000a1e0: 0264 043c 007c 0064 0519 006a 017d 037c  .d.<.|.d...j.}.|
+0000a1f0: 037c 0364 066b 0419 007d 0374 02a0 037c  .|.d.k...}.t...|
+0000a200: 03a1 017d 0374 0464 0674 057c 0383 0183  ...}.t.d.t.|....
+0000a210: 0244 005d 687d 047c 037c 0419 007d 057c  .D.]h}.|.|...}.|
+0000a220: 006a 067c 0064 0519 007c 056b 0219 007d  .j.|.d...|.k...}
+0000a230: 067c 066a 0764 0767 0164 0864 098d 027d  .|.j.d.g.d.d...}
+0000a240: 067c 067c 0119 006a 0164 0619 007d 077c  .|.|...j.d...}.|
+0000a250: 067c 0119 006a 017d 0874 057c 0883 0164  .|...j.}.t.|...d
+0000a260: 0a6b 0472 4c74 087c 077c 007c 0264 0a7c  .k.rLt.|.|.|.d.|
+0000a270: 087c 0064 0a64 0b8d 077d 0271 4c7c 0253  .|.d.d...}.qL|.S
+0000a280: 0029 0c72 fd00 0000 7206 0000 0054 7207  .).r....r....Tr.
+0000a290: 0000 0072 8300 0000 7284 0000 0072 0100  ...r....r....r..
+0000a2a0: 0000 7279 0000 0046 727a 0000 0072 2800  ..ry...Frz...r(.
+0000a2b0: 0000 72fb 0000 0029 0972 1400 0000 7213  ..r....).r....r.
+0000a2c0: 0000 0072 1a00 0000 722b 0000 0072 2900  ...r....r+...r).
+0000a2d0: 0000 7215 0000 0072 1900 0000 7241 0000  ..r....r....rA..
+0000a2e0: 0072 a300 0000 72fe 0000 0072 2400 0000  .r....r....r$...
+0000a2f0: 7224 0000 0072 2500 0000 da3b 6368 616e  r$...r%....;chan
+0000a300: 6765 5f61 7474 7269 6275 7465 5f76 616c  ge_attribute_val
+0000a310: 7565 735f 666f 725f 6361 7463 686d 656e  ues_for_catchmen
+0000a320: 7473 5f63 6f76 6572 6564 5f62 795f 7361  ts_covered_by_sa
+0000a330: 6d65 5f6c 616b 6545 0b00 0073 3200 0000  me_lakeE...s2...
+0000a340: 000d 0401 0c01 0e01 0a01 0c01 0a03 1201  ................
+0000a350: 0801 1201 1001 0801 02ff 0403 0a01 0c01  ................
+0000a360: 0201 0201 0201 0201 0201 0201 0201 02f9  ................
+0000a370: 0809 720d 0100 0063 0300 0000 0000 0000  ..r....c........
+0000a380: 0000 0000 0d00 0000 0500 0000 4300 0000  ............C...
+0000a390: 73a8 0200 007c 006a 007d 037c 0264 016b  s....|.j.}.|.d.k
+0000a3a0: 0490 0172 dc74 0164 0174 027c 0383 0183  ...r.t.d.t.|....
+0000a3b0: 0244 005d dc7d 047c 006a 037c 037c 0419  .D.].}.|.j.|.|..
+0000a3c0: 0064 0266 0219 007d 057c 006a 037c 037c  .d.f...}.|.j.|.|
+0000a3d0: 0419 0064 0366 0219 007d 067c 006a 037c  ...d.f...}.|.j.|
+0000a3e0: 037c 0419 0064 0466 0219 007d 077c 006a  .|...d.f...}.|.j
+0000a3f0: 037c 0064 0319 007c 076b 0219 00a0 04a1  .|.d...|.k......
+0000a400: 007d 0874 027c 0883 0164 016b 0472 987c  .}.t.|...d.k.r.|
+0000a410: 0864 0219 006a 0564 0119 007c 006a 037c  .d...j.d...|.j.|
+0000a420: 037c 0419 0064 0566 023c 006e 1264 067c  .|...d.f.<.n.d.|
+0000a430: 006a 037c 037c 0419 0064 0566 023c 007c  .j.|.|...d.f.<.|
+0000a440: 057c 006a 037c 037c 0419 0064 0566 0219  .|.j.|.|...d.f..
+0000a450: 006b 0272 d264 067c 006a 037c 037c 0419  .k.r.d.|.j.|.|..
+0000a460: 0064 0566 023c 007c 057c 006a 037c 037c  .d.f.<.|.|.j.|.|
+0000a470: 0419 0064 0566 0219 006b 0272 1e64 067c  ...d.f...k.r.d.|
+0000a480: 006a 037c 037c 0419 0064 0566 023c 0071  .j.|.|...d.f.<.q
+0000a490: 1e7c 0064 0319 006a 057c 0064 073c 007c  .|.d...j.|.d.<.|
+0000a4a0: 0064 0419 006a 057c 0064 083c 007c 0064  .d...j.|.d.<.|.d
+0000a4b0: 0219 006a 057c 0064 033c 007c 0064 0519  ...j.|.d.<.|.d..
+0000a4c0: 006a 057c 0064 043c 007c 007c 0064 0919  .j.|.d.<.|.|.d..
+0000a4d0: 0064 0a6b 0319 006a 0464 0b64 0c8d 017d  .d.k...j.d.d...}
+0000a4e0: 097c 0064 0319 00a0 067c 0964 0419 00a1  .|.d.....|.d....
+0000a4f0: 010f 007d 0a64 0d7c 006a 0776 0090 0172  ...}.d.|.j.v...r
+0000a500: 8864 0e7c 006a 037c 0a64 0d66 023c 0064  .d.|.j.|.d.f.<.d
+0000a510: 0e7c 006a 037c 0a64 0f66 023c 0064 0e7c  .|.j.|.d.f.<.d.|
+0000a520: 006a 037c 0a64 1066 023c 0064 0e7c 006a  .j.|.d.f.<.d.|.j
+0000a530: 037c 0a64 1166 023c 0064 0e7c 006a 037c  .|.d.f.<.d.|.j.|
+0000a540: 0a64 1266 023c 0064 0e7c 006a 037c 0a64  .d.f.<.d.|.j.|.d
+0000a550: 1366 023c 0064 0e7c 006a 037c 0a64 1466  .f.<.d.|.j.|.d.f
+0000a560: 023c 0064 0e7c 006a 037c 0a64 1566 023c  .<.d.|.j.|.d.f.<
+0000a570: 007c 0164 016b 0090 0172 ea7c 0053 007c  .|.d.k...r.|.S.|
+0000a580: 006a 0864 0364 1664 178d 027d 0b74 097c  .j.d.d.d...}.t.|
+0000a590: 0b83 017d 0b74 0164 0174 027c 0b83 0183  ...}.t.d.t.|....
+0000a5a0: 0244 005d 947d 047c 0b64 0319 006a 057c  .D.].}.|.d...j.|
+0000a5b0: 0419 007d 0c7c 0b64 1819 006a 057c 0419  ...}.|.d...j.|..
+0000a5c0: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
+0000a5d0: 1866 023c 007c 0b64 1919 006a 057c 0419  .f.<.|.d...j.|..
+0000a5e0: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
+0000a5f0: 1966 023c 007c 0b64 1a19 006a 057c 0419  .f.<.|.d...j.|..
+0000a600: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
+0000a610: 1a66 023c 007c 0b64 1b19 006a 057c 0419  .f.<.|.d...j.|..
+0000a620: 007c 006a 037c 0064 0319 007c 0c6b 0264  .|.j.|.d...|.k.d
+0000a630: 1b66 023c 0090 0271 0e7c 0053 0029 1c72  .f.<...q.|.S.).r
+0000a640: a700 0000 7201 0000 0072 8300 0000 7206  ....r....r....r.
+0000a650: 0000 0072 0d00 0000 7285 0000 0072 6b00  ...r....r....rk.
+0000a660: 0000 7286 0000 0072 8700 0000 7264 0000  ..r....r....rd..
+0000a670: 0072 6500 0000 5472 0700 0000 7272 0000  .re...Tr....rr..
+0000a680: 0072 6c00 0000 7273 0000 0072 6800 0000  .rl...rs...rh...
+0000a690: 726d 0000 0072 7100 0000 726e 0000 0072  rm...rq...rn...r
+0000a6a0: 7000 0000 726f 0000 0072 3a00 0000 72a8  p...ro...r:...r.
+0000a6b0: 0000 0072 6900 0000 7266 0000 0072 6a00  ...ri...rf...rj.
+0000a6c0: 0000 7279 0000 0029 0a72 5900 0000 7229  ..ry...).rY...r)
+0000a6d0: 0000 0072 1500 0000 7219 0000 0072 1400  ...r....r....r..
+0000a6e0: 0000 7213 0000 0072 1200 0000 7211 0000  ..r....r....r...
+0000a6f0: 0072 4200 0000 5a1a 5374 7265 616d 6f72  .rB...Z.Streamor
+0000a700: 6465 7261 6e64 6472 6169 6e61 6765 6172  deranddrainagear
+0000a710: 6561 290d 728a 0000 0072 aa00 0000 72ab  ea).r....r....r.
+0000a720: 0000 0072 5f00 0000 7248 0000 0072 8300  ...r_...rH...r..
+0000a730: 0000 7249 0000 0072 ac00 0000 72ad 0000  ..rI...r....r...
+0000a740: 00da 1972 6976 5f70 645f 6e6e 636c 735f  ...riv_pd_nncls_
+0000a750: 726f 7574 696e 675f 696e 666f 7223 0000  routing_infor#..
+0000a760: 0072 ae00 0000 72af 0000 0072 2400 0000  .r....r....r$...
+0000a770: 7224 0000 0072 2500 0000 7222 0000 006f  r$...r%...r"...o
+0000a780: 0b00 0073 7400 0000 000d 0602 0a01 1201  ...st...........
+0000a790: 1201 1201 1202 0401 0aff 0804 0c01 0201  ................
+0000a7a0: 02ff 0402 02fe 1404 1202 1601 1202 1601  ................
+0000a7b0: 1402 0e01 0e01 0e02 0e03 1801 1402 0c01  ................
+0000a7c0: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e03  ................
+0000a7d0: 0a01 0402 0e02 0802 1201 0e03 0cfe 0401  ................
+0000a7e0: 0eff 0205 0cfe 0401 0eff 0205 0cfe 0401  ................
+0000a7f0: 0eff 0205 0cfe 0401 0eff 0604 7222 0000  ............r"..
+0000a800: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
+0000a810: 0000 0300 0000 4300 0000 730c 0000 007c  ......C...s....|
+0000a820: 017c 007c 0213 0014 0053 0029 014e 7224  .|.|.....S.).Nr$
+0000a830: 0000 0029 03da 0141 7261 0000 0072 ca00  ...)...Ara...r..
+0000a840: 0000 7224 0000 0072 2400 0000 7225 0000  ..r$...r$...r%..
+0000a850: 00da 0966 756e 635f 515f 4441 c30b 0000  ...func_Q_DA....
+0000a860: 7302 0000 0000 0172 1001 0000 6301 0000  s......r....c...
+0000a870: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+0000a880: 0043 0000 0073 6400 0000 7a2c 7400 7401  .C...sd...z,t.t.
+0000a890: 7c00 6400 6400 8502 6401 6602 1900 7c00  |.d.d...d.f...|.
+0000a8a0: 6400 6400 8502 6402 6602 1900 8303 5c02  d.d...d.f.....\.
+0000a8b0: 7d01 7d02 5700 6e26 0400 7402 7952 0100  }.}.W.n&..t.yR..
+0000a8c0: 0100 0100 7403 6403 8301 0100 7404 a005  ....t.d.....t...
+0000a8d0: 6404 6405 a102 7d01 5900 6e02 3000 7c01  d.d...}.Y.n.0.|.
+0000a8e0: 6401 1900 7c01 6402 1900 6602 5300 2906  d...|.d...f.S.).
+0000a8f0: 4e72 0100 0000 7228 0000 007a 3723 2323  Nr....r(...z7###
+0000a900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a930: 2323 2323 7265 0000 0072 6b00 0000 2906  ####re...rk...).
+0000a940: 7202 0000 0072 1001 0000 da0c 5275 6e74  r....r......Runt
+0000a950: 696d 6545 7272 6f72 7275 0000 0072 1a00  imeErrorru...r..
+0000a960: 0000 727d 0000 0029 035a 0464 615f 715a  ..r}...).Z.da_qZ
+0000a970: 0570 6f70 7432 5a05 7063 6f76 3272 2400  .popt2Z.pcov2r$.
+0000a980: 0000 7224 0000 0072 2500 0000 da23 7265  ..r$...r%....#re
+0000a990: 7475 726e 5f6b 5f61 6e64 5f63 5f69 6e5f  turn_k_and_c_in_
+0000a9a0: 715f 6461 5f72 656c 6174 696f 6e73 6869  q_da_relationshi
+0000a9b0: 70c7 0b00 0073 0c00 0000 0002 0201 2c01  p....s........,.
+0000a9c0: 0c01 0801 1202 7212 0100 0063 0400 0000  ......r....c....
+0000a9d0: 0000 0000 0000 0000 0d00 0000 0500 0000  ................
+0000a9e0: 4300 0000 73c2 0000 0064 017d 047c 047c  C...s....d.}.|.|
+0000a9f0: 0114 007d 0564 027d 067c 0064 017c 0514  ...}.d.}.|.d.|..
+0000aa00: 0018 007d 077c 0764 036b 0072 4464 047c  ...}.|.d.k.rDd.|
+0000aa10: 0014 007d 0764 057c 0014 007d 057c 007c  ...}.d.|...}.|.|
+0000aa20: 0718 0064 011b 007c 011b 007d 047c 077c  ...d...|...}.|.|
+0000aa30: 0114 0064 017c 0414 007c 0114 007c 0114  ...d.|...|...|..
+0000aa40: 0064 011b 0017 007d 087c 0764 017c 0114  .d.....}.|.d.|..
+0000aa50: 0064 067c 0464 0113 0017 0064 0413 0014  .d.|.d.....d....
+0000aa60: 0017 007d 0974 007c 0883 0174 007c 0983  ...}.t.|...t.|..
+0000aa70: 011b 007d 0a74 007c 0283 0174 007c 0883  ...}.t.|...t.|..
+0000aa80: 011b 007d 0b7c 0b64 036b 0472 ba7c 0a64  ...}.|.d.k.r.|.d
+0000aa90: 0713 007c 0364 0413 0014 007c 0b1b 007d  ...|.d.....|...}
+0000aaa0: 0c6e 0464 087d 0c7c 0c53 0029 094e 7265  .n.d.}.|.S.).Nre
+0000aab0: 0000 007a 0a20 2020 2020 2020 2020 2072  ...z.          r
+0000aac0: 0100 0000 72b1 0000 0067 0000 0000 0000  ....r....g......
+0000aad0: d03f 7228 0000 0067 5555 5555 5555 e53f  .?r(...gUUUUUU.?
+0000aae0: 726c 0000 0029 0172 6300 0000 290d da05  rl...).rc...)...
+0000aaf0: 7769 6474 68da 0564 6570 7468 da01 515a  width..depth..QZ
+0000ab00: 0573 6c6f 7065 5a03 7a63 685a 0573 6964  .slopeZ.zchZ.sid
+0000ab10: 7764 da03 7461 625a 0562 6f74 7764 5a03  wd..tabZ.botwdZ.
+0000ab20: 4163 685a 0350 6368 5a03 5263 68da 0156  AchZ.PchZ.Rch..V
+0000ab30: da01 6e72 2400 0000 7224 0000 0072 2500  ..nr$...r$...r%.
+0000ab40: 0000 da11 6361 6c63 756c 6174 6543 6861  ....calculateCha
+0000ab50: 6e6e 616c 6ed2 0b00 0073 2000 0000 0001  nnaln....s .....
+0000ab60: 0401 0801 0401 0c01 0801 0801 0801 1001  ................
+0000ab70: 1c07 1c01 1001 1001 0801 1602 0401 7219  ..............r.
+0000ab80: 0100 00fa 0123 6303 0000 0000 0000 0000  .....#c.........
+0000ab90: 0000 0010 0000 0007 0000 0043 0000 0073  ...........C...s
+0000aba0: c801 0000 7c01 6401 6b00 720c 7c00 5300  ....|.d.k.r.|.S.
+0000abb0: 7c00 6402 6403 6702 1900 a000 6404 a101  |.d.d.g.....d...
+0000abc0: 6a01 7d03 6405 7d04 6405 7c00 6a02 7601  j.}.d.}.d.|.j.v.
+0000abd0: 7232 6406 7d04 7c02 6407 6b03 9001 7264  r2d.}.|.d.k...rd
+0000abe0: 7403 7c02 8301 6408 1900 6a01 7d05 7404  t.|...d...j.}.t.
+0000abf0: a005 7c05 a101 7d06 7c06 7c06 6401 6b04  ..|...}.|.|.d.k.
+0000ac00: 1900 7d06 7c00 6a06 7c00 7c04 1900 a007  ..}.|.j.|.|.....
+0000ac10: 7c06 a101 1900 7d07 6409 7d08 7c01 6401  |.....}.d.}.|.d.
+0000ac20: 6b00 728c 7408 640a 8301 0100 7c00 5300  k.r.t.d.....|.S.
+0000ac30: 7c00 6a06 7c00 7c04 1900 7c01 6b02 1900  |.j.|.|...|.k...
+0000ac40: 7d09 7409 7c09 8301 6401 6b04 72ba 7c09  }.t.|...d.k.r.|.
+0000ac50: 6402 1900 6a01 6401 1900 7d08 6e0e 7408  d...j.d...}.n.t.
+0000ac60: 640b 7c09 8302 0100 7c00 5300 740a 7c03  d.|.....|.S.t.|.
+0000ac70: 7c08 8302 7d0a 7409 7c07 8301 640c 6b05  |...}.t.|...d.k.
+0000ac80: 9001 7248 740b 6401 7409 7c07 8301 8302  ..rHt.d.t.|.....
+0000ac90: 4400 5d58 7d0b 7c07 6402 1900 6a01 7c0b  D.]X}.|.d...j.|.
+0000aca0: 1900 7d0c 7c0c 7c08 6b02 73ee 7404 a00c  ..}.|.|.k.s.t...
+0000acb0: 7404 a00d 7c0a 7c0c a102 a101 640d 6b00  t...|.|.....d.k.
+0000acc0: 9001 7222 71ee 740a 7c03 7c0c 8302 7d0d  ..r"q.t.|.|...}.
+0000acd0: 7404 a00d 7c0a 7c0d a102 7d0e 7c0a 7404  t...|.|...}.|.t.
+0000ace0: a00e 7c0e a101 1900 7d0a 71ee 7c0a 7d0f  ..|.....}.q.|.}.
+0000acf0: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
+0000ad00: 1900 7d00 7c00 5300 6409 7d08 7c00 6a06  ..}.|.S.d.}.|.j.
+0000ad10: 7c00 7c04 1900 7c01 6b02 1900 7d09 7409  |.|...|.k...}.t.
+0000ad20: 7c09 8301 6401 6b04 9001 72a2 7c09 6402  |...d.k...r.|.d.
+0000ad30: 1900 6a01 6401 1900 7d08 740a 7c03 7c08  ..j.d...}.t.|.|.
+0000ad40: 8302 7d0f 6e0a 7c00 6402 1900 6a01 7d0f  ..}.n.|.d...j.}.
+0000ad50: 7c00 6a06 7c00 6402 1900 a007 7c0f a101  |.j.|.d.....|...
+0000ad60: 1900 7d00 7c00 5300 6400 5300 290e 4e72  ..}.|.S.d.S.).Nr
+0000ad70: 0100 0000 7206 0000 0072 0d00 0000 7263  ....r....r....rc
+0000ad80: 0000 0072 8000 0000 7281 0000 0072 1a01  ...r....r....r..
+0000ad90: 0000 5a09 7265 675f 7375 6269 6472 6b00  ..Z.reg_subidrk.
+0000ada0: 0000 7a41 546f 2075 7365 2073 7562 7265  ..zATo use subre
+0000adb0: 6769 6f6e 2c20 7468 6520 5375 6272 6567  gion, the Subreg
+0000adc0: 696f 6e20 4964 204d 5553 5420 7072 6f76  ion Id MUST prov
+0000add0: 6964 6564 2061 7320 4f75 746c 6574 5f4f  ided as Outlet_O
+0000ade0: 6273 5f49 447a 284e 6f20 4f75 746c 6574  bs_IDz(No Outlet
+0000adf0: 2069 6420 6973 2066 6f75 6e64 6564 2066   id is founded f
+0000ae00: 6f72 2073 7562 7265 6769 6f6e 2020 2072  or subregion   r
+0000ae10: 6500 0000 7228 0000 0029 0f72 1600 0000  e...r(...).r....
+0000ae20: 7213 0000 0072 1100 0000 5a10 4462 665f  r....r....Z.Dbf_
+0000ae30: 546f 5f44 6174 6166 7261 6d65 721a 0000  To_Dataframer...
+0000ae40: 0072 2b00 0000 7219 0000 0072 1200 0000  .r+...r....r....
+0000ae50: 7275 0000 0072 1500 0000 7217 0000 0072  ru...r....r....r
+0000ae60: 2900 0000 723f 0000 0072 2e00 0000 729a  )...r?...r....r.
+0000ae70: 0000 0029 1072 7600 0000 da0d 6f75 746c  ...).rv.....outl
+0000ae80: 6574 5f6f 6273 5f69 64da 1670 6174 685f  et_obs_id..path_
+0000ae90: 7375 625f 7265 675f 6f75 746c 6574 735f  sub_reg_outlets_
+0000aea0: 7672 7700 0000 728c 0000 005a 0f53 7562  vrw...r....Z.Sub
+0000aeb0: 5f72 6567 5f6f 7574 6c65 7473 5a13 5375  _reg_outletsZ.Su
+0000aec0: 625f 7265 675f 6f75 746c 6574 735f 6964  b_reg_outlets_id
+0000aed0: 735a 0f72 6567 5f6f 7574 6c65 745f 696e  sZ.reg_outlet_in
+0000aee0: 666f 72bb 0000 005a 0d6f 7574 6c65 7449  for....Z.outletI
+0000aef0: 445f 696e 666f 7201 0100 0072 4800 0000  D_infor....rH...
+0000af00: 5a07 7570 7265 6769 645a 1248 7964 726f  Z.upregidZ.Hydro
+0000af10: 4261 7369 6e73 5f72 656d 6f76 6572 2300  Basins_remover#.
+0000af20: 0000 7203 0100 0072 2400 0000 7224 0000  ..r....r$...r$..
+0000af30: 0072 2500 0000 da1f 7265 7475 726e 5f69  .r%.....return_i
+0000af40: 6e74 6572 6573 745f 6361 7463 686d 656e  nterest_catchmen
+0000af50: 7473 5f69 6e66 6fec 0b00 0073 5400 0000  ts_info....sT...
+0000af60: 0002 0801 0402 1402 0401 0a01 0402 0a02  ................
+0000af70: 0e01 0a01 0c03 1403 0402 0801 0801 0402  ................
+0000af80: 1201 0c01 1002 0a01 0403 0a04 0e02 1201  ................
+0000af90: 0e02 2001 0201 0a01 0401 04ff 0403 1001  .. .............
+0000afa0: 0402 1401 0403 0401 1201 0e01 0e02 0c02  ................
+0000afb0: 0a02 1401 721d 0100 0063 0200 0000 0000  ....r....c......
+0000afc0: 0000 0000 0000 0c00 0000 0500 0000 0300  ................
+0000afd0: 0000 7352 0100 0067 007d 0288 0164 0119  ..sR...g.}...d..
+0000afe0: 006a 007d 0374 01a0 027c 03a1 017d 0367  .j.}.t...|...}.g
+0000aff0: 007d 0274 03a0 04a1 0074 056a 0664 023c  .}.t.....t.j.d.<
+0000b000: 007c 02a0 0764 03a1 0101 007c 02a0 0764  .|...d.....|...d
+0000b010: 04a1 0101 007c 02a0 0764 05a1 0101 0074  .....|...d.....t
+0000b020: 087c 0383 017d 047c 02a0 0764 0674 097c  .|...}.|...d.t.|
+0000b030: 0483 0117 00a1 0101 0074 0a7c 0164 0719  .........t.|.d..
+0000b040: 006a 0083 0164 0817 0074 0a7c 0164 0919  .j...d...t.|.d..
+0000b050: 006a 0083 0164 0817 0014 007d 057c 02a0  .j...d.....}.|..
+0000b060: 0764 0a74 097c 0583 0117 00a1 0101 007c  .d.t.|.........|
+0000b070: 02a0 0764 0ba1 0101 007c 02a0 0764 0ca1  ...d.....|...d..
+0000b080: 0101 0074 0a7c 0164 0919 006a 0083 0189  ...t.|.d...j....
+0000b090: 027c 0164 0d19 006a 0089 0074 0b74 087c  .|.d...j...t.t.|
+0000b0a0: 0383 0164 0e1b 0083 017d 0674 087c 0383  ...d.....}.t.|..
+0000b0b0: 0164 0f6b 0472 ee74 01a0 0c7c 037c 06a1  .d.k.r.t...|.|..
+0000b0c0: 027d 076e 067c 0367 017d 0774 0d64 1074  .}.n.|.g.}.t.d.t
+0000b0d0: 087c 0783 0183 0244 005d 367d 087c 077c  .|.....D.]6}.|.|
+0000b0e0: 0819 007d 0974 0e64 1164 128d 0187 0087  ...}.t.d.d......
+0000b0f0: 0187 0266 0364 1364 1484 087c 0944 0083  ...f.d.d...|.D..
+0000b100: 0183 017d 0a7c 027c 0a17 007d 0290 0171  ...}.|.|...}...q
+0000b110: 027c 02a0 0764 15a1 0101 0064 16a0 0f7c  .|...d.....d...|
+0000b120: 02a1 017d 0b7c 0b53 0029 174e 72a4 0000  ...}.|.S.).Nr...
+0000b130: 005a 124a 4f42 4c49 425f 5445 4d50 5f46  .Z.JOBLIB_TEMP_F
+0000b140: 4f4c 4445 527a 0c3a 4772 6964 5765 6967  OLDERz.:GridWeig
+0000b150: 6874 737a 0a20 2020 2320 2020 2020 207a  htsz.   #      z
+0000b160: 0d20 2020 2320 5b23 2048 5255 735d 7a15  .   # [# HRUs]z.
+0000b170: 2020 203a 4e75 6d62 6572 4852 5573 2020     :NumberHRUs  
+0000b180: 2020 2020 205a 0352 6f77 7228 0000 00da       Z.Rowr(....
+0000b190: 0343 6f6c 7a15 2020 203a 4e75 6d62 6572  .Colz.   :Number
+0000b1a0: 4772 6964 4365 6c6c 7320 207a 1020 2020  GridCells  z.   
+0000b1b0: 2320 2020 2020 2020 2020 2020 207a 1d20  #            z. 
+0000b1c0: 2020 2320 5b48 5255 2049 445d 205b 4365    # [HRU ID] [Ce
+0000b1d0: 6c6c 2023 5d20 5b77 5f6b 6c5d 5a04 4647  ll #] [w_kl]Z.FG
+0000b1e0: 4944 72cf 0000 0072 7c00 0000 7201 0000  IDr....r|...r...
+0000b1f0: 0072 0601 0000 2901 5a06 6e5f 6a6f 6273  .r....).Z.n_jobs
+0000b200: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+0000b210: 0006 0000 0033 0000 0073 2800 0000 7c00  .....3...s(...|.
+0000b220: 5d20 7d01 7400 7401 8301 7c01 8801 6a02  ] }.t.t...|...j.
+0000b230: 6400 6401 8d01 8800 8802 8304 5600 0100  d.d.........V...
+0000b240: 7102 6402 5300 2903 5472 0700 0000 4e29  q.d.S.).Tr....N)
+0000b250: 0372 0500 0000 da16 6372 6561 7465 5f67  .r......create_g
+0000b260: 7269 645f 7765 6967 6874 5f68 7275 7214  rid_weight_hrur.
+0000b270: 0000 0029 02da 022e 3072 4800 0000 a903  ...)....0rH.....
+0000b280: da07 4176 6166 6769 64da 0a4d 6170 666f  ..Avafgid..Mapfo
+0000b290: 7263 696e 67da 076d 6178 5f63 6f6c 7224  rcing..max_colr$
+0000b2a0: 0000 0072 2500 0000 da09 3c67 656e 6578  ...r%.....<genex
+0000b2b0: 7072 3e55 0c00 00f3 0000 0000 7a2a 6372  pr>U........z*cr
+0000b2c0: 6561 7465 5f67 7269 645f 7765 6967 6874  eate_grid_weight
+0000b2d0: 5f6d 6169 6e2e 3c6c 6f63 616c 733e 2e3c  _main.<locals>.<
+0000b2e0: 6765 6e65 7870 723e 7a0f 3a45 6e64 4772  genexpr>z.:EndGr
+0000b2f0: 6964 5765 6967 6874 73da 010a 2910 7213  idWeights...).r.
+0000b300: 0000 0072 1a00 0000 722b 0000 00da 0874  ...r....r+.....t
+0000b310: 656d 7066 696c 65da 0a67 6574 7465 6d70  empfile..gettemp
+0000b320: 6469 72da 026f 73da 0765 6e76 6972 6f6e  dir..os..environ
+0000b330: 724e 0000 0072 1500 0000 72dc 0000 0072  rN...r....r....r
+0000b340: 7400 0000 722d 0000 00da 0b61 7272 6179  t...r-.....array
+0000b350: 5f73 706c 6974 7229 0000 0072 0400 0000  _splitr)...r....
+0000b360: da04 6a6f 696e 290c 7223 0100 005a 0846  ..join).r#...Z.F
+0000b370: 6f72 6369 6e66 6f5a 1767 7269 645f 7765  orcinfoZ.grid_we
+0000b380: 6967 6874 5f73 7472 696e 675f 6c69 7374  ight_string_list
+0000b390: 5a06 6872 7569 6473 5a05 734e 6872 755a  Z.hruidsZ.sNhruZ
+0000b3a0: 0673 4e63 656c 6c5a 0b6e 5f68 7275 5f67  .sNcellZ.n_hru_g
+0000b3b0: 726f 7570 5a0e 6872 755f 6964 735f 6772  roupZ.hru_ids_gr
+0000b3c0: 6f75 7073 7248 0000 005a 0b69 5f68 7275  oupsrH...Z.i_hru
+0000b3d0: 5f67 726f 7570 5a18 6772 6964 5f77 6569  _groupZ.grid_wei
+0000b3e0: 6768 745f 7374 7269 6e67 5f68 7275 7369  ght_string_hrusi
+0000b3f0: 5a12 6772 6964 5f77 6569 6768 745f 7374  Z.grid_weight_st
+0000b400: 7269 6e67 7224 0000 0072 2101 0000 7225  ringr$...r!...r%
+0000b410: 0000 00da 1763 7265 6174 655f 6772 6964  .....create_grid
+0000b420: 5f77 6569 6768 745f 6d61 696e 310c 0000  _weight_main1...
+0000b430: 7336 0000 0000 0204 010a 010a 0204 020e  s6..............
+0000b440: 030a 010a 010a 0208 0112 0224 0112 010a  ...........$....
+0000b450: 010a 010e 010a 0410 020c 010e 0206 0212  ................
+0000b460: 0108 0120 010c 020a 010a 0172 2e01 0000  ... .......r....
+0000b470: 6304 0000 0000 0000 0000 0000 000e 0000  c...............
+0000b480: 0006 0000 0043 0000 0073 1602 0000 6401  .....C...s....d.
+0000b490: 7d04 7c01 6a00 7c01 6402 1900 7c00 6b02  }.|.j.|.d...|.k.
+0000b4a0: 1900 6a01 6403 6404 8d01 7d05 7402 7c05  ..j.d.d...}.t.|.
+0000b4b0: 8301 6405 6b01 725c 7c01 6a00 7c01 6402  ..d.k.r\|.j.|.d.
+0000b4c0: 1900 7c00 6b02 1900 6a01 6403 6404 8d01  ..|.k...j.d.d...
+0000b4d0: 7d05 7403 6406 8301 0100 7403 7c05 6407  }.t.d.....t.|.d.
+0000b4e0: 1900 8301 0100 7c04 5300 7404 7c05 6408  ......|.S.t.|.d.
+0000b4f0: 1900 6a05 8301 7d06 7c05 6407 1900 6a05  ..j...}.|.d...j.
+0000b500: 7d07 7406 a007 7c07 a101 7d07 6409 7d08  }.t...|...}.d.}.
+0000b510: 7408 6405 7402 7c07 8301 8302 4400 9001  t.d.t.|.....D...
+0000b520: 5d7e 7d09 7c05 7c05 6407 1900 7c07 7c09  ]~}.|.|.d...|.|.
+0000b530: 1900 6b02 1900 7d0a 7c09 7402 7c07 8301  ..k...}.|.t.|...
+0000b540: 640a 1800 6b00 72e2 7404 7c0a 6408 1900  d...k.r.t.|.d...
+0000b550: 6a05 8301 7d0b 7409 7c0b 8301 7409 7c06  j...}.t.|...t.|.
+0000b560: 8301 1b00 7d0c 7c08 7c0c 1700 7d08 6e08  ....}.|.|...}.n.
+0000b570: 640a 7c08 1800 7d0c 7402 7c0a 640b 1900  d.|...}.t.|.d...
+0000b580: 6a05 8301 640a 6b04 9001 7240 7403 740a  j...d.k...r@t.t.
+0000b590: 740b 8301 640c 1700 8301 0100 740a 740c  t...d.......t.t.
+0000b5a0: 7c0a 640b 1900 6a05 6405 1900 7c03 640a  |.d...j.d...|.d.
+0000b5b0: 1700 1400 7c0a 640d 1900 6a05 6405 1900  ....|.d...j.d...
+0000b5c0: 1700 8301 8301 640e 1700 7d0d 6e30 740a  ......d...}.n0t.
+0000b5d0: 740c 7c0a 640b 1900 6a05 6405 1900 7c03  t.|.d...j.d...|.
+0000b5e0: 640a 1700 1400 7c0a 640d 1900 6a05 6405  d.....|.d...j.d.
+0000b5f0: 1900 1700 8301 8301 640e 1700 7d0d 7402  ........d...}.t.
+0000b600: 7c07 8301 640a 6b02 9001 72a8 7c04 640f  |...d.k...r.|.d.
+0000b610: 1700 740a 740c 7c00 8301 8301 1700 6410  ..t.t.|.......d.
+0000b620: 1700 7c0d 1700 640e 1700 740a 7c0c 8301  ..|...d...t.|...
+0000b630: 1700 7d04 7190 7c09 7402 7c07 8301 640a  ..}.q.|.t.|...d.
+0000b640: 1800 6b02 9001 72e4 7c04 640f 1700 740a  ..k...r.|.d...t.
+0000b650: 740c 7c00 8301 8301 1700 6410 1700 7c0d  t.|.......d...|.
+0000b660: 1700 640e 1700 740a 7c0c 8301 1700 7d04  ..d...t.|.....}.
+0000b670: 7190 7c04 640f 1700 740a 740c 7c00 8301  q.|.d...t.t.|...
+0000b680: 8301 1700 6410 1700 7c0d 1700 640e 1700  ....d...|...d...
+0000b690: 740a 7c0c 8301 1700 6411 1700 7d04 7190  t.|.....d...}.q.
+0000b6a0: 7c04 5300 2912 4efa 0120 72a4 0000 0054  |.S.).N.. r....T
+0000b6b0: 7207 0000 0072 0100 0000 7a28 466f 6c6c  r....r....z(Foll
+0000b6c0: 6f77 696e 6720 4772 6964 2068 6173 2074  owing Grid has t
+0000b6d0: 6f20 6265 2069 6e6c 7564 6564 3a2e 2e2e  o be inluded:...
+0000b6e0: 2e2e 2e2e 5a08 4d61 705f 4647 4944 5a06  ....Z.Map_FGIDZ.
+0000b6f0: 735f 6172 6561 7267 0000 0072 2800 0000  s_arearg...r(...
+0000b700: 5a07 4d61 705f 526f 777a 3d65 7272 6f72  Z.Map_Rowz=error
+0000b710: 3a20 3120 6872 752c 2031 2067 7269 642c  : 1 hru, 1 grid,
+0000b720: 2070 726f 6475 6365 206d 7574 6920 706f   produce muti po
+0000b730: 6c79 676f 6e20 6e65 6564 2074 6f20 6265  lygon need to be
+0000b740: 206d 6572 6765 6420 5a07 4d61 705f 436f   merged Z.Map_Co
+0000b750: 6c7a 0620 2020 2020 207a 0420 2020 207a  lz.      z.    z
+0000b760: 0520 2020 2020 7227 0100 0029 0d72 1900  .     r'...).r..
+0000b770: 0000 7214 0000 0072 1500 0000 7275 0000  ..r....r....ru..
+0000b780: 0072 3f00 0000 7213 0000 0072 1a00 0000  .r?...r....r....
+0000b790: 722b 0000 0072 2900 0000 7263 0000 0072  r+...r)...rc...r
+0000b7a0: dc00 0000 72b8 0000 0072 2d00 0000 290e  ....r....r-...).
+0000b7b0: 7260 0000 0072 2301 0000 7222 0100 0072  r`...r#...r"...r
+0000b7c0: 2401 0000 5a16 6772 6964 5f77 6569 6768  $...Z.grid_weigh
+0000b7d0: 745f 7374 7269 6e67 5f68 7275 da04 6361  t_string_hru..ca
+0000b7e0: 7473 5a05 7461 7265 615a 0466 6964 735a  tsZ.tareaZ.fidsZ
+0000b7f0: 0573 756d 7774 725e 0000 005a 0473 6361  .sumwtr^...Z.sca
+0000b800: 745a 0573 6172 6561 da02 7774 5a09 5374  tZ.sarea..wtZ.St
+0000b810: 7263 656c 6c69 6472 2400 0000 7224 0000  rcellidr$...r$..
+0000b820: 0072 2500 0000 721f 0100 005c 0c00 0073  .r%...r....\...s
+0000b830: 6c00 0000 0002 0402 1a04 0c01 1a01 0801  l...............
+0000b840: 0c01 0402 0e01 0a01 0a01 0401 1401 1401  ................
+0000b850: 1001 0e01 1001 0a02 0802 1401 0201 0601  ................
+0000b860: 02ff 02ff 0405 0201 0201 0c01 06ff 0202  ................
+0000b870: 0cfe 02ff 02ff 0207 02f9 02ff 040c 0201  ................
+0000b880: 0201 0c01 06ff 0202 0cfe 02ff 02ff 0207  ................
+0000b890: 02f9 02ff 020a 0e01 2a02 1201 2a02 2e02  ........*...*...
+0000b8a0: 721f 0100 0029 0172 2800 0000 2901 7206  r....).r(...).r.
+0000b8b0: 0000 0029 0272 2800 0000 7228 0000 0029  ...).r(...r(...)
+0000b8c0: 0272 2800 0000 7228 0000 0029 0172 1a01  .r(...r(...).r..
+0000b8d0: 0000 2934 7214 0000 00da 056e 756d 7079  ..)4r......numpy
+0000b8e0: 721a 0000 00da 0670 616e 6461 7372 4000  r......pandasr@.
+0000b8f0: 0000 5a0e 7363 6970 792e 6f70 7469 6d69  ..Z.scipy.optimi
+0000b900: 7a65 7202 0000 005a 1e62 6173 696e 6d61  zer....Z.basinma
+0000b910: 6b65 722e 7574 696c 6974 6965 732e 7574  ker.utilities.ut
+0000b920: 696c 6974 6965 73da 076e 756d 6265 7273  ilities..numbers
+0000b930: 5a06 6a6f 626c 6962 7204 0000 0072 0500  Z.joblibr....r..
+0000b940: 0000 7228 0100 00da 076f 7074 696f 6e73  ..r(.....options
+0000b950: da04 6d6f 6465 da12 6368 6169 6e65 645f  ..mode..chained_
+0000b960: 6173 7369 676e 6d65 6e74 7226 0000 0072  assignmentr&...r
+0000b970: 3200 0000 722a 0000 0072 4c00 0000 7256  2...r*...rL...rV
+0000b980: 0000 0072 6200 0000 7278 0000 0072 7f00  ...rb...rx...r..
+0000b990: 0000 7290 0000 0072 a300 0000 72a6 0000  ..r....r....r...
+0000b9a0: 0072 b000 0000 72b2 0000 0072 a900 0000  .r....r....r....
+0000b9b0: 7217 0000 0072 c700 0000 72cd 0000 0072  r....r....r....r
+0000b9c0: d500 0000 72d9 0000 0072 de00 0000 72ef  ....r....r....r.
+0000b9d0: 0000 0072 f700 0000 72fa 0000 0072 fc00  ...r....r....r..
+0000b9e0: 0000 72ff 0000 0072 0401 0000 720b 0100  ..r....r....r...
+0000b9f0: 0072 0c01 0000 720d 0100 0072 2200 0000  .r....r....r"...
+0000ba00: 7210 0100 0072 1201 0000 7219 0100 0072  r....r....r....r
+0000ba10: 1d01 0000 722e 0100 0072 1f01 0000 7224  ....r....r....r$
+0000ba20: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+0000ba30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+0000ba40: 7378 0000 0008 0208 0108 010c 0108 0108  sx..............
+0000ba50: 0110 0108 010a 0308 2e08 3808 0b08 1e08  ..........8.....
+0000ba60: 1908 5708 5408 580a 7f00 2002 0102 0104  ..W.T.X... .....
+0000ba70: 0104 0102 0102 f70a 7f00 150a 180a 3e08  ..............>.
+0000ba80: 0a08 7f00 7f00 1c08 2a08 6008 7f00 5e08  ........*.`...^.
+0000ba90: 7b08 1308 7f00 7808 7f00 7f00 7f00 2508  {.....x.......%.
+0000baa0: 5a08 6708 6f08 2b08 2008 7f00 0608 5608  Z.g.o.+. .....V.
+0000bab0: 2a0a 5408 0408 0b08 1a0a 4508 2b         *.T.......E.+
```

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/purepy.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/purepy.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Oct 19 23:50:34 2022 UTC, .py size: 16723 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,629 +1,648 @@
-00000000: 610d 0d0a 0000 0000 4a8d 5063 5341 0000  a.......J.PcSA..
+00000000: 610d 0d0a 0000 0000 6bb2 8363 b644 0000  a.......k..c.D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6401 6c06 5a06 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
 00000070: 6401 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
 00000080: 6d0d 5a0d 0100 6400 6404 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
 00000090: 0100 6405 6406 8400 5a10 6407 6408 8400  ..d.d...Z.d.d...
-000000a0: 5a11 641c 640a 640b 8401 5a12 641d 640d  Z.d.d.d...Z.d.d.
+000000a0: 5a11 641e 640a 640b 8401 5a12 641f 640d  Z.d.d.d...Z.d.d.
 000000b0: 640e 8401 5a13 640f 6410 8400 5a14 6411  d...Z.d.d...Z.d.
-000000c0: 6412 8400 5a15 641e 6414 6415 8401 5a16  d...Z.d.d.d...Z.
-000000d0: 6416 6417 8400 5a17 6418 6419 8400 5a18  d.d...Z.d.d...Z.
-000000e0: 641a 641b 8400 5a19 6401 5300 291f e900  d.d...Z.d.S.)...
-000000f0: 0000 004e 2902 da04 6c6f 6164 da0b 4a53  ...N)...load..JS
-00000100: 4f4e 456e 636f 6465 7229 02da 0467 6461  ONEncoder)...gda
-00000110: 6cda 036f 6772 2901 da0b 7a6f 6e61 6c5f  l..ogr)...zonal_
-00000120: 7374 6174 7363 0400 0000 0000 0000 0000  statsc..........
-00000130: 0000 0700 0000 0700 0000 0300 0000 7336  ..............s6
-00000140: 0000 0074 007c 007c 017c 0264 0164 0164  ...t.|.|.|.d.d.d
-00000150: 028d 057d 0474 0174 0287 0066 0164 0364  ...}.t.t...f.d.d
-00000160: 0484 087c 0483 0283 017d 0574 03a0 047c  ...|.....}.t...|
-00000170: 05a1 017d 067c 0653 0029 054e 5429 03da  ...}.|.S.).NT)..
-00000180: 0573 7461 7473 5a0b 6765 6f6a 736f 6e5f  .statsZ.geojson_
-00000190: 6f75 745a 0b61 6c6c 5f74 6f75 6368 6564  outZ.all_touched
-000001a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000001b0: 0005 0000 0013 0000 0073 1c00 0000 8800  .........s......
-000001c0: 7c00 6401 1900 8800 1900 6402 7c00 6401  |.d.......d.|.d.
-000001d0: 1900 6402 1900 6902 5300 2903 4eda 0a70  ..d...i.S.).N..p
-000001e0: 726f 7065 7274 6965 73da 046d 6561 6ea9  roperties..mean.
-000001f0: 0029 01da 0178 a901 da03 6b65 7972 0a00  .)...x....keyr..
-00000200: 0000 fa47 633a 5c75 7365 7273 5c6d 3433  ...Gc:\users\m43
-00000210: 6861 6e5f 325c 646f 6375 6d65 6e74 735c  han_2\documents\
-00000220: 6769 7468 7562 5c62 6173 696e 6d61 6b65  github\basinmake
-00000230: 725c 6261 7369 6e6d 616b 6572 5c66 756e  r\basinmaker\fun
-00000240: 635c 7075 7265 7079 2e70 79da 083c 6c61  c\purepy.py..<la
-00000250: 6d62 6461 3e12 0000 00f3 0000 0000 7a20  mbda>.........z 
-00000260: 7a6f 6e61 6c5f 7374 6174 735f 7064 2e3c  zonal_stats_pd.<
-00000270: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00000280: 2905 7206 0000 00da 046c 6973 74da 036d  ).r......list..m
-00000290: 6170 da02 7064 da09 4461 7461 4672 616d  ap..pd..DataFram
-000002a0: 6529 07da 0773 6870 5f67 7064 da06 7261  e)...shp_gpd..ra
-000002b0: 7374 6572 7207 0000 0072 0d00 0000 da06  sterr....r......
-000002c0: 7265 7375 6c74 5a0f 7265 6175 6c74 5f6c  resultZ.reault_l
-000002d0: 6973 745f 6469 63da 0972 6561 756c 745f  ist_dic..reault_
-000002e0: 7064 720a 0000 0072 0c00 0000 720e 0000  pdr....r....r...
-000002f0: 00da 0e7a 6f6e 616c 5f73 7461 7473 5f70  ...zonal_stats_p
-00000300: 640e 0000 0073 0800 0000 0002 1202 1602  d....s..........
-00000310: 0a02 7219 0000 0063 0500 0000 0000 0000  ..r....c........
-00000320: 0000 0000 0b00 0000 0500 0000 4300 0000  ............C...
-00000330: 73ce 0000 007c 006a 0064 0164 028d 017d  s....|.j.d.d...}
-00000340: 0564 037d 0674 017c 0583 0164 036b 0472  .d.}.t.|...d.k.r
-00000350: a87c 0664 046b 0172 a874 027c 057c 017c  .|.d.k.r.t.|.|.|
-00000360: 027c 0383 047d 077c 077c 0764 0519 0064  .|...}.|.|.d...d
-00000370: 036b 040f 0019 0064 0619 007d 087c 057c  .k.....d...}.|.|
-00000380: 0564 0619 00a0 037c 08a1 0119 006a 0064  .d.....|.....j.d
-00000390: 0164 028d 017d 057c 0664 036b 0272 847c  .d...}.|.d.k.r.|
-000003a0: 077c 0764 0519 0064 036b 0419 007d 097c  .|.d...d.k...}.|
-000003b0: 0664 0717 007d 0671 107c 0664 0717 007d  .d...}.q.|.d...}
-000003c0: 067c 077c 0764 0519 0064 036b 0419 007d  .|.|.d...d.k...}
-000003d0: 0a7c 09a0 047c 0aa1 017d 0971 1074 017c  .|...|...}.q.t.|
-000003e0: 0583 0164 036b 0472 ca7c 057c 0419 007c  ...d.k.r.|.|...|
-000003f0: 0564 053c 007c 09a0 047c 05a1 017d 097c  .d.<.|...|...}.|
-00000400: 0953 0029 084e 54a9 01da 0464 6565 7072  .S.).NT....deepr
-00000410: 0100 0000 e905 0000 0072 0900 0000 5a0a  .........r....Z.
-00000420: 4852 555f 4944 5f4e 6577 e901 0000 0029  HRU_ID_New.....)
-00000430: 05da 0463 6f70 79da 036c 656e 7219 0000  ...copy..lenr...
-00000440: 00da 0469 7369 6eda 0661 7070 656e 6429  ...isin..append)
-00000450: 0b72 1500 0000 7216 0000 0072 0700 0000  .r....r....r....
-00000460: 720d 0000 00da 0363 6f6c 5a09 6e6f 6461  r......colZ.noda
-00000470: 7461 5f70 64da 0169 5a07 7465 6d70 5f70  ta_pd..iZ.temp_p
-00000480: 645a 0e62 6164 5f68 7275 5f76 616c 7565  dZ.bad_hru_value
-00000490: 7372 1800 0000 5a07 676f 6f64 5f70 6472  sr....Z.good_pdr
-000004a0: 0a00 0000 720a 0000 0072 0e00 0000 da0a  ....r....r......
-000004b0: 5a6f 6e61 6c53 7461 7473 1a00 0000 7320  ZonalStats....s 
-000004c0: 0000 0000 060c 0104 0114 010e 0116 011a  ................
-000004d0: 0108 0110 010a 0208 0110 010c 020c 010c  ................
-000004e0: 010a 0272 2400 0000 fa01 2363 0600 0000  ...r$.....#c....
-000004f0: 0000 0000 0000 0000 0d00 0000 0600 0000  ................
-00000500: 4300 0000 730a 0100 007c 036a 007d 0674  C...s....|.j.}.t
-00000510: 01a0 027c 00a1 017d 077c 07a0 037c 06a1  ...|...}.|...|..
-00000520: 017d 087c 086a 0464 0164 028d 017d 087c  .}.|.j.d.d...}.|
-00000530: 08a0 057c 03a1 017d 0974 067c 0964 0383  ...|...}.t.|.d..
-00000540: 027d 0a7c 0464 046b 0390 0172 067c 017c  .}.|.d.k...r.|.|
-00000550: 096a 0776 0172 6074 087c 0164 0583 0201  .j.v.r`t.|.d....
-00000560: 0074 09a0 0aa1 0001 007c 017c 056a 0776  .t.......|.|.j.v
-00000570: 0172 7c74 087c 0164 0683 0201 0074 09a0  .r|t.|.d.....t..
-00000580: 0aa1 0001 007c 047c 056a 0776 0172 9874  .....|.|.j.v.r.t
-00000590: 087c 0464 0683 0201 0074 09a0 0aa1 0001  .|.d.....t......
-000005a0: 007c 056a 0b64 0164 078d 017d 0b7c 0b6a  .|.j.d.d...}.|.j
-000005b0: 0c7c 0467 0164 0864 0164 098d 037d 0b7c  .|.g.d.d.d...}.|
-000005c0: 0b7c 0119 007c 0b64 0a3c 007c 0b7c 0464  .|...|.d.<.|.|.d
-000005d0: 0a67 0219 007d 0b74 0d6a 0e7c 057c 0b64  .g...}.t.j.|.|.d
-000005e0: 0b7c 0464 0c8d 046a 0b64 0164 078d 017d  .|.d...j.d.d...}
-000005f0: 0c74 0d6a 0e7c 0a7c 0c64 0b7c 0164 0c8d  .t.j.|.|.d.|.d..
-00000600: 047d 0a7c 0a64 0a19 007c 0a7c 013c 007c  .}.|.d...|.|.<.|
-00000610: 0a53 0029 0d61 b205 0000 5072 6570 726f  .S.).a....Prepro
-00000620: 6365 7373 2075 7365 7220 7072 6f76 6964  cess user provid
-00000630: 6564 2070 6f6c 7967 6f6e 730a 0a20 2020  ed polygons..   
-00000640: 2046 756e 6374 696f 6e20 7468 6174 2077   Function that w
-00000650: 696c 6c20 7265 7072 6f6a 6563 7420 636c  ill reproject cl
-00000660: 6970 2069 6e70 7574 2070 6f6c 7967 6f6e  ip input polygon
-00000670: 2077 6974 6820 7375 6262 6173 696e 2070   with subbasin p
-00000680: 6f6c 7967 6f6e 0a20 2020 2061 6e64 2077  olygon.    and w
-00000690: 696c 6c20 6469 7373 6f6c 7665 2074 6865  ill dissolve the
-000006a0: 2069 6e70 7574 2070 6f6c 7967 6f6e 2062   input polygon b
-000006b0: 6173 6564 206f 6e20 7468 6569 7220 4944  ased on their ID
-000006c0: 2c20 7375 6368 2061 7320 6c61 6e64 7573  , such as landus
-000006d0: 6520 6964 0a20 2020 206f 7220 736f 696c  e id.    or soil
-000006e0: 2069 642e 0a0a 2020 2020 5061 7261 6d65   id...    Parame
-000006f0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00000700: 2d2d 2d0a 2020 2020 7072 6f63 6573 7369  ---.    processi
-00000710: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
-00000720: 2020 2020 2020 2020 2020 3a20 7167 6973            : qgis
-00000730: 206f 626a 6563 740a 2020 2020 636f 6e74   object.    cont
-00000740: 6578 7420 2020 2020 2020 2020 2020 2020  ext             
-00000750: 2020 2020 2020 2020 2020 2020 2020 3a20                : 
-00000760: 7167 6973 206f 626a 6563 740a 2020 2020  qgis object.    
-00000770: 6c61 7965 725f 7061 7468 2020 2020 2020  layer_path      
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 3a20 7374 7269 6e67 0a20 2020 2020    : string.     
-000007a0: 2020 2054 6865 2070 6174 6820 746f 2061     The path to a
-000007b0: 2073 7065 6369 6669 6320 706f 6c79 676f   specific polygo
-000007c0: 6e2c 2066 6f72 2065 7861 6d70 6c65 2070  n, for example p
-000007d0: 6174 6820 746f 206c 616e 6475 7365 206c  ath to landuse l
-000007e0: 6179 6572 0a20 2020 2050 726f 6a65 6374  ayer.    Project
-000007f0: 5f63 7273 2020 2020 2020 2020 2020 2020  _crs            
-00000800: 2020 2020 2020 2020 2020 203a 2073 7472             : str
-00000810: 696e 670a 2020 2020 2020 2020 7468 6520  ing.        the 
-00000820: 4550 5347 2063 6f64 6520 6f66 2061 2070  EPSG code of a p
-00000830: 726f 6a65 6374 6564 2063 6f6f 6469 6e61  rojected coodina
-00000840: 7465 2073 7973 7465 6d20 7468 6174 2077  te system that w
-00000850: 696c 6c20 6265 2075 7365 6420 746f 0a20  ill be used to. 
-00000860: 2020 2020 2020 2063 616c 6375 6174 6520         calcuate 
-00000870: 4852 5520 6172 6561 2061 6e64 2073 6c6f  HRU area and slo
-00000880: 7065 2e0a 2020 2020 7472 675f 6372 7320  pe..    trg_crs 
-00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008a0: 2020 2020 2020 2020 2020 3a20 7374 7269            : stri
-000008b0: 6e67 0a20 2020 2020 2020 2074 6865 2045  ng.        the E
-000008c0: 5053 4720 636f 6465 206f 6620 6120 2063  PSG code of a  c
-000008d0: 6f6f 6469 6e61 7465 2073 7973 7465 6d20  oodinate system 
-000008e0: 7468 6174 2077 696c 6c20 6265 2075 7365  that will be use
-000008f0: 6420 746f 0a20 2020 2020 2020 2063 616c  d to.        cal
-00000900: 6375 6174 6520 7265 7072 6f6a 6563 7420  cuate reproject 
-00000910: 696e 7075 7420 706f 6c79 676f 6e0a 2020  input polygon.  
-00000920: 2020 436c 6173 735f 436f 6c20 2020 2020    Class_Col     
-00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000940: 2020 2020 3a20 7374 7269 6e67 0a20 2020      : string.   
-00000950: 2020 2020 2074 6865 2063 6f6c 756d 6e20       the column 
-00000960: 6e61 6d65 2069 6e20 7468 6520 696e 7075  name in the inpu
-00000970: 7420 706f 6c79 676f 6e20 286c 6179 6572  t polygon (layer
-00000980: 5f70 6174 6829 2074 6861 7420 636f 6e74  _path) that cont
-00000990: 6169 6e73 0a20 2020 2020 2020 2074 6865  ains.        the
-000009a0: 6972 2049 442c 2066 6f72 2065 7861 6d70  ir ID, for examp
-000009b0: 6c65 206c 616e 6420 7573 6520 4944 206f  le land use ID o
-000009c0: 7220 736f 696c 2049 442e 0a20 2020 204c  r soil ID..    L
-000009d0: 6179 6572 5f63 6c69 7020 2020 2020 2020  ayer_clip       
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 203a 2071 6769 7320 6f62 6a65 6374 0a20   : qgis object. 
-00000a00: 2020 2020 2020 2041 2073 6870 6669 6c65         A shpfile
-00000a10: 2077 6974 6820 6578 7465 6e74 206f 6620   with extent of 
-00000a20: 7468 6520 7761 7465 7273 6865 642c 2077  the watershed, w
-00000a30: 696c 6c20 6265 2075 7365 6420 746f 2063  ill be used to c
-00000a40: 6c69 7020 696e 7075 740a 2020 2020 2020  lip input.      
-00000a50: 2020 696e 7075 7420 706f 6c79 676f 6e0a    input polygon.
-00000a60: 2020 2020 4e6f 7465 730a 2020 2020 2d2d      Notes.    --
-00000a70: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
-00000a80: 544f 444f 3a20 4d61 7920 6265 2061 6464  TODO: May be add
-00000a90: 2073 6f6d 6520 6675 6e63 7469 6f6e 2074   some function t
-00000aa0: 6f20 7369 6d70 6c69 6679 2074 6865 2069  o simplify the i
-00000ab0: 6e70 7574 2070 6f6c 7967 6f6e 730a 2020  nput polygons.  
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00000ad0: 7220 6578 616d 706c 652c 2072 656d 6f76  r example, remov
-00000ae0: 6520 7468 6520 6c61 6e64 7573 6520 7479  e the landuse ty
-00000af0: 7065 2077 6974 6820 736d 616c 6c20 6172  pe with small ar
-00000b00: 6561 730a 2020 2020 2020 2020 2020 2020  eas.            
-00000b10: 2020 2020 6f72 206d 6572 6765 2073 6d61      or merge sma
-00000b20: 6c6c 206c 616e 6475 7365 2070 6f6c 7967  ll landuse polyg
-00000b30: 6f6e 2069 6e74 6f20 7468 6520 7375 7272  on into the surr
-00000b40: 6f75 6e64 696e 6720 706f 6c79 676f 6e0a  ounding polygon.
-00000b50: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00000b60: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00000b70: 2020 6c61 7965 725f 6469 7320 2020 2020    layer_dis     
-00000b80: 2020 2020 2020 2020 2020 2020 203a 2071               : q
-00000b90: 6769 7320 6f62 6a65 6374 0a20 2020 2020  gis object.     
-00000ba0: 2020 2020 2020 2069 7420 6973 2061 2070         it is a p
-00000bb0: 6f6c 7967 6f6e 2061 6674 6572 2070 7265  olygon after pre
-00000bc0: 7072 6f63 6573 730a 2020 2020 5429 01da  process.    T)..
-00000bd0: 0c69 676e 6f72 655f 696e 6465 7872 1d00  .ignore_indexr..
-00000be0: 0000 7225 0000 007a 3120 6e6f 7420 696e  ..r%...z1 not in
-00000bf0: 2074 6865 2061 7474 7269 6275 7465 2074   the attribute t
-00000c00: 6162 6c65 206f 6620 7072 6f76 6964 6564  able of provided
-00000c10: 2073 6861 7065 6669 6c65 7a32 206e 6f74   shapefilez2 not
-00000c20: 2069 6e20 7468 6520 6174 7472 6962 7574   in the attribut
-00000c30: 6520 7461 626c 6520 6f66 2070 726f 7669  e table of provi
-00000c40: 6465 6420 696e 666f 2074 6162 6c65 721a  ded info tabler.
-00000c50: 0000 00da 046c 6173 7429 03da 0673 7562  .....last)...sub
-00000c60: 7365 74da 046b 6565 7072 2600 0000 5a06  set..keepr&...Z.
-00000c70: 4e65 775f 4944 da05 696e 6e65 7229 02da  New_ID..inner)..
-00000c80: 0368 6f77 da02 6f6e 290f da03 6372 73da  .how..on)...crs.
-00000c90: 0967 656f 7061 6e64 6173 da09 7265 6164  .geopandas..read
-00000ca0: 5f66 696c 65da 0674 6f5f 6372 73da 0765  _file..to_crs..e
-00000cb0: 7870 6c6f 6465 da04 636c 6970 da15 636c  xplode..clip..cl
-00000cc0: 6561 6e5f 6765 6f6d 6574 7279 5f70 7572  ean_geometry_pur
-00000cd0: 6570 79da 0763 6f6c 756d 6e73 da05 7072  epy..columns..pr
-00000ce0: 696e 74da 0373 7973 da04 6578 6974 721e  int..sys..exitr.
-00000cf0: 0000 00da 0f64 726f 705f 6475 706c 6963  .....drop_duplic
-00000d00: 6174 6573 7213 0000 00da 056d 6572 6765  atesr......merge
-00000d10: 290d 5a0a 6c61 7965 725f 7061 7468 5a09  ).Z.layer_pathZ.
-00000d20: 436c 6173 735f 436f 6cda 0a74 656d 7066  Class_Col..tempf
-00000d30: 6f6c 6465 725a 0a6d 6173 6b5f 6c61 7965  olderZ.mask_laye
-00000d40: 725a 0c43 6c61 7373 5f4e 4d5f 436f 6c5a  rZ.Class_NM_ColZ
-00000d50: 0a69 6e66 6f5f 7461 626c 655a 076e 6577  .info_tableZ.new
-00000d60: 5f63 7273 da04 6461 7461 5a09 7072 6f6a  _crs..dataZ.proj
-00000d70: 6563 7465 64da 0763 6c69 7070 6564 da07  ected..clipped..
-00000d80: 636c 6561 6e65 645a 0f69 6e66 6f5f 7461  cleanedZ.info_ta
-00000d90: 626c 655f 636f 7079 5a10 696e 666f 5f74  ble_copyZ.info_t
-00000da0: 6162 6c65 5f63 6f70 7932 720a 0000 0072  able_copy2r....r
-00000db0: 0a00 0000 720e 0000 00da 2c52 6570 726f  ....r.....,Repro
-00000dc0: 6a5f 436c 6970 5f44 6973 736f 6c76 655f  j_Clip_Dissolve_
-00000dd0: 5369 6d70 6c69 6679 5f50 6f6c 7967 6f6e  Simplify_Polygon
-00000de0: 5f70 7572 6570 7935 0000 0073 3000 0000  _purepy5...s0...
-00000df0: 0027 0601 0a02 0a01 0c01 0a03 0a01 0a01  .'..............
-00000e00: 0a01 0a01 0801 0a01 0a01 0801 0a01 0a01  ................
-00000e10: 0802 0c01 1201 0c01 0c01 1a02 1201 0c06  ................
-00000e20: 723e 0000 00da 0553 7562 4964 6307 0000  r>.....SubIdc...
-00000e30: 0000 0000 0000 0000 0013 0000 0008 0000  ................
-00000e40: 0043 0000 0073 ee03 0000 6700 6401 a201  .C...s....g.d...
-00000e50: 7d07 6402 7c00 6a00 7600 7218 6403 7d08  }.d.|.j.v.r.d.}.
-00000e60: 6e04 6404 7d08 7401 a002 7c08 a101 7d09  n.d.}.t...|...}.
-00000e70: 7403 7404 6a05 a006 7c02 6405 a102 6406  t.t.j...|.d...d.
-00000e80: 8302 8f1c 7d0a 7c0a a007 7c09 6a08 a101  ....}.|...|.j...
-00000e90: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-00000ea0: 3100 735c 3000 0100 0100 0100 5900 0100  1.s\0.......Y...
-00000eb0: 7c04 6407 6b03 9002 72a8 7c05 6407 6b03  |.d.k...r.|.d.k.
-00000ec0: 728e 7409 a00a 7c05 a101 7d0b 7c0b 6408  r.t...|...}.|.d.
-00000ed0: 1900 7c0b 6409 3c00 7c00 6a0b 640a 640b  ..|.d.<.|.j.d.d.
-00000ee0: 8d01 6a0c 640c 640d 8d01 7d0c 7c05 6407  ..j.d.d...}.|.d.
-00000ef0: 6b03 72d8 7c0b 640a 6409 6702 1900 7d0b  k.r.|.d.d.g...}.
-00000f00: 740d 6a0e 7c0b 7c0c 6409 640e 640f 8d04  t.j.|.|.d.d.d...
-00000f10: 7d0b 7c0b 6a0f 7c06 6410 6411 6412 8d03  }.|.j.|.d.d.d...
-00000f20: 7d0b 7c00 6a0f 7c06 6410 6411 6412 8d03  }.|.j.|.d.d.d...
-00000f30: 7d00 7410 7c00 6413 6414 8303 7d00 7c00  }.t.|.d.d...}.|.
-00000f40: 6414 6413 6702 1900 6a0c 640c 640d 8d01  d.d.g...j.d.d...
-00000f50: 7d0d 7c05 6407 6b03 9001 722c 7c0b 6a0b  }.|.d.k...r,|.j.
-00000f60: 6414 6413 6702 640b 8d01 7d0b 7c0b a006  d.d.g.d...}.|...
-00000f70: 7c0d a101 7d0b 7c00 7c00 6415 1900 6416  |...}.|.|.d...d.
-00000f80: 6b03 1900 6408 6417 6702 1900 6a0c 640c  k...d.d.g...j.d.
-00000f90: 640d 8d01 7d0e 6700 7d0f 7c0e 6408 1900  d...}.g.}.|.d...
-00000fa0: 6a11 4400 5d20 7d10 7c10 7c0e 6417 1900  j.D.] }.|.|.d...
-00000fb0: 6a11 7601 9001 725a 7c0f a012 7c10 a101  j.v...rZ|...|...
-00000fc0: 0100 9001 715a 7c05 6407 6b03 9001 72da  ....qZ|.d.k...r.
-00000fd0: 7c0b 7c0b 6a13 a014 7c0f a101 0f00 1900  |.|.j...|.......
-00000fe0: 7d0b 7c0b 6a00 7d11 7c11 7c11 a014 7c07  }.|.j.}.|.|...|.
-00000ff0: a101 1900 7d12 7c0b 6a0b 7c12 640b 8d01  ....}.|.j.|.d...
-00001000: 7d0b 7415 7c0b 8301 6418 6b04 9001 72da  }.t.|...d.k...r.
-00001010: 7c0b a016 7404 6a05 a006 7c02 7c04 a102  |...t.j...|.|...
-00001020: a101 0100 6419 7c00 6a17 7c00 6a13 a014  ....d.|.j.|.j...
-00001030: 7c0f a101 641a 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
-00001040: 7c00 6a13 a014 7c0f a101 641b 6602 3c00  |.j...|...d.f.<.
-00001050: 6419 7c00 6a17 7c00 6a13 a014 7c0f a101  d.|.j.|.j...|...
-00001060: 641c 6602 3c00 6419 7c00 6a17 7c00 6a13  d.f.<.d.|.j.|.j.
-00001070: a014 7c0f a101 641d 6602 3c00 6419 7c00  ..|...d.f.<.d.|.
-00001080: 6a17 7c00 6a13 a014 7c0f a101 641e 6602  j.|.j...|...d.f.
-00001090: 3c00 6419 7c00 6a17 7c00 6a13 a014 7c0f  <.d.|.j.|.j...|.
-000010a0: a101 641f 6602 3c00 7c00 6a00 7d11 7c11  ..d.f.<.|.j.}.|.
-000010b0: 7c11 a014 7c07 a101 1900 7d12 7c00 6a0b  |...|.....}.|.j.
-000010c0: 7c12 640b 8d01 7d00 7c00 a016 7404 6a05  |.d...}.|...t.j.
-000010d0: a006 7c02 7c03 a102 a101 0100 7418 7404  ..|.|.......t.t.
-000010e0: 6a05 a006 7c02 7c03 a102 8301 0100 9001  j...|.|.........
-000010f0: 6e42 7c00 6a0f 7c06 6410 6411 6412 8d03  nB|.j.|.d.d.d...
-00001100: 7d00 6414 7c00 6a00 7600 9003 72ae 7410  }.d.|.j.v...r.t.
-00001110: 7c00 6413 6414 8303 7d00 7c00 6a19 7c00  |.d.d...}.|.j.|.
-00001120: 6408 3c00 7c00 7c00 6415 1900 6416 6b03  d.<.|.|.d...d.k.
-00001130: 1900 6408 6417 6702 1900 6a0c 640c 640d  ..d.d.g...j.d.d.
-00001140: 8d01 7d0e 6700 7d0f 7c0e 6408 1900 6a11  ..}.g.}.|.d...j.
-00001150: 4400 5d20 7d10 7c10 7c0e 6417 1900 6a11  D.] }.|.|.d...j.
-00001160: 7601 9003 7208 7c0f a012 7c10 a101 0100  v...r.|...|.....
-00001170: 9003 7108 6419 7c00 6a17 7c00 6a13 a014  ..q.d.|.j.|.j...
-00001180: 7c0f a101 641a 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
-00001190: 7c00 6a13 a014 7c0f a101 641b 6602 3c00  |.j...|...d.f.<.
-000011a0: 6419 7c00 6a17 7c00 6a13 a014 7c0f a101  d.|.j.|.j...|...
-000011b0: 641c 6602 3c00 6419 7c00 6a17 7c00 6a13  d.f.<.d.|.j.|.j.
-000011c0: a014 7c0f a101 641d 6602 3c00 6419 7c00  ..|...d.f.<.d.|.
-000011d0: 6a17 7c00 6a13 a014 7c0f a101 641e 6602  j.|.j...|...d.f.
-000011e0: 3c00 6419 7c00 6a17 7c00 6a13 a014 7c0f  <.d.|.j.|.j...|.
-000011f0: a101 641f 6602 3c00 7c00 6a00 7d11 7c11  ..d.f.<.|.j.}.|.
-00001200: 7c11 a014 6700 6420 a201 a101 1900 7d12  |...g.d ......}.
-00001210: 7c00 6a0b 7c12 640b 8d01 7d00 7c00 a016  |.j.|.d...}.|...
-00001220: 7404 6a05 a006 7c02 7c03 a102 a101 0100  t.j...|.|.......
-00001230: 7c00 5300 6400 5300 2921 4e29 10da 0753  |.S.d.S.)!N)...S
-00001240: 7562 4964 5f31 da02 4964 da07 6e73 7562  ubId_1..Id..nsub
-00001250: 6964 32da 066e 7375 6269 64da 0a6e 646f  id2..nsubid..ndo
-00001260: 776e 7375 6269 64da 094f 6c64 5f53 7562  wnsubid..Old_Sub
-00001270: 4964 da0a 4f6c 645f 446f 7753 7562 da0a  Id..Old_DowSub..
-00001280: 4a6f 696e 5f43 6f75 6e74 da0a 5441 5247  Join_Count..TARG
-00001290: 4554 5f46 4944 7241 0000 00da 0a53 7562  ET_FIDrA.....Sub
-000012a0: 4944 5f4f 6c64 72da 0a48 5255 5f49 445f  ID_Oldr..HRU_ID_
-000012b0: 4e5f 31da 0a48 5255 5f49 445f 4e5f 32da  N_1..HRU_ID_N_2.
-000012c0: 0766 6163 7465 7273 da0c 4f6c 645f 446f  .facters..Old_Do
-000012d0: 7753 7562 4964 5a07 5375 6249 6474 325a  wSubIdZ.SubIdt2Z
-000012e0: 0844 415f 4368 6e5f 4c7a 4168 7474 7073  .DA_Chn_LzAhttps
-000012f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
-00001300: 7374 6d69 6e67 2f52 6f75 7469 6e67 546f  stming/RoutingTo
-00001310: 6f6c 2f77 696b 692f 4669 6c65 732f 5245  ol/wiki/Files/RE
-00001320: 4144 4d45 5f4f 4948 2e70 6466 7a40 6874  ADME_OIH.pdfz@ht
-00001330: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001340: 2f64 7573 746d 696e 672f 526f 7574 696e  /dustming/Routin
-00001350: 6754 6f6f 6c2f 7769 6b69 2f46 696c 6573  gTool/wiki/Files
-00001360: 2f52 4541 444d 455f 4e41 2e70 6466 7a0a  /README_NA.pdfz.
-00001370: 5245 4144 4d45 2e70 6466 da02 7762 7225  README.pdf..wbr%
-00001380: 0000 0072 3f00 0000 7245 0000 00da 0867  ...r?...rE.....g
-00001390: 656f 6d65 7472 79a9 0172 3400 0000 5472  eometry..r4...Tr
-000013a0: 1a00 0000 da04 6c65 6674 2902 722c 0000  ......left).r,..
-000013b0: 0072 2b00 0000 da05 6669 7273 7446 2903  .r+.....firstF).
-000013c0: da02 6279 da07 6167 6766 756e 63da 0861  ..by..aggfunc..a
-000013d0: 735f 696e 6465 785a 0a63 656e 7472 6f69  s_indexZ.centroi
-000013e0: 645f 785a 0a63 656e 7472 6f69 645f 79da  d_xZ.centroid_y.
-000013f0: 084c 616b 655f 4361 74e9 0200 0000 da08  .Lake_Cat.......
-00001400: 446f 7753 7562 4964 7201 0000 0067 8d97  DowSubIdr....g..
-00001410: 6e12 83c0 f3bf 5a08 5269 7653 6c6f 7065  n.....Z.RivSlope
-00001420: 5a09 5269 764c 656e 6774 685a 0846 6c6f  Z.RivLengthZ.Flo
-00001430: 6f64 505f 6e5a 0443 685f 6e5a 074d 6178  odP_nZ.Ch_nZ.Max
-00001440: 5f44 454d 5a07 4d69 6e5f 4445 4d29 0f5a  _DEMZ.Min_DEM).Z
-00001450: 0553 4841 5045 7240 0000 0072 4100 0000  .SHAPEr@...rA...
-00001460: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00001470: 4600 0000 7247 0000 0072 4800 0000 7241  F...rG...rH...rA
-00001480: 0000 0072 4900 0000 724a 0000 0072 4b00  ...rI...rJ...rK.
-00001490: 0000 724c 0000 0072 4d00 0000 291a 7234  ..rL...rM...).r4
-000014a0: 0000 00da 0872 6571 7565 7374 73da 0367  .....requests..g
-000014b0: 6574 da04 6f70 656e da02 6f73 da04 7061  et..open..os..pa
-000014c0: 7468 da04 6a6f 696e da05 7772 6974 65da  th..join..write.
-000014d0: 0763 6f6e 7465 6e74 722e 0000 0072 2f00  .contentr....r/.
-000014e0: 0000 da04 6472 6f70 721e 0000 0072 1300  ....dropr....r..
-000014f0: 0000 7239 0000 00da 0864 6973 736f 6c76  ..r9.....dissolv
-00001500: 65da 1561 6464 5f63 656e 7472 6f69 645f  e..add_centroid_
-00001510: 696e 5f77 6773 3834 da06 7661 6c75 6573  in_wgs84..values
-00001520: 7221 0000 0072 3f00 0000 7220 0000 0072  r!...r?...r ...r
-00001530: 1f00 0000 da07 746f 5f66 696c 65da 036c  ......to_file..l
-00001540: 6f63 da15 6372 6561 7465 5f67 656f 5f6a  oc..create_geo_j
-00001550: 6173 6f6e 5f66 696c 65da 0569 6e64 6578  ason_file..index
-00001560: 2913 5a0e 6d61 706f 6c64 6e65 775f 696e  ).Z.mapoldnew_in
-00001570: 666f 723a 0000 00da 0c4f 7574 7075 7446  for:.....OutputF
-00001580: 6f6c 6465 725a 0863 6174 5f6e 616d 655a  olderZ.cat_nameZ
-00001590: 0872 6976 5f6e 616d 65da 0e50 6174 685f  .riv_name..Path_
-000015a0: 6669 6e61 6c5f 7269 765a 0c64 6973 5f63  final_rivZ.dis_c
-000015b0: 6f6c 5f6e 616d 655a 124e 4545 445f 544f  ol_nameZ.NEED_TO
-000015c0: 5f52 454d 4f56 455f 4944 53da 0375 726c  _REMOVE_IDS..url
-000015d0: da08 7265 7370 6f6e 7365 da01 665a 0672  ..response..fZ.r
-000015e0: 6976 5f70 645a 0663 6174 5f70 645a 0963  iv_pdZ.cat_pdZ.c
-000015f0: 6174 5f63 5f78 5f79 5a19 7269 765f 7064  at_c_x_yZ.riv_pd
-00001600: 5f6e 6e63 6c73 5f72 6f75 7469 6e67 5f69  _nncls_routing_i
-00001610: 6e66 6f5a 0e72 656d 6f76 655f 6368 616e  nfoZ.remove_chan
-00001620: 6e65 6cda 0573 7562 6964 5a0a 6361 745f  nel..subidZ.cat_
-00001630: 636f 6c6e 6d73 5a0f 6472 6f70 5f63 6174  colnmsZ.drop_cat
-00001640: 5f63 6f6c 6e6d 7372 0a00 0000 720a 0000  _colnmsr....r...
-00001650: 0072 0e00 0000 da23 7361 7665 5f6d 6f64  .r.....#save_mod
-00001660: 6966 6965 645f 6174 7472 6962 7574 6573  ified_attributes
-00001670: 5f74 6f5f 6f75 7470 7574 7380 0000 0073  _to_outputs....s
-00001680: 8200 0000 0003 0803 0a01 0602 0402 0a01  ................
-00001690: 1601 2a02 0a02 0801 0a01 0c02 1402 0801  ..*.............
-000016a0: 0c01 1201 1003 1001 0c02 1401 0a01 1001  ................
-000016b0: 0a02 2001 0401 0e01 1001 0e01 0a01 1201  .. .............
-000016c0: 0601 0e01 0c01 0e01 1402 1601 1601 1601  ................
-000016d0: 1601 1601 1602 0601 0e01 0c01 1402 1604  ................
-000016e0: 1002 0c02 0c01 0a01 2001 0401 0e01 1001  ........ .......
-000016f0: 0e02 1601 1601 1601 1601 1601 1603 0601  ................
-00001700: 1201 0c01 1401 726f 0000 0063 0200 0000  ......ro...c....
-00001710: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00001720: 4300 0000 7384 0000 0074 00a0 017c 0064  C...s....t...|.d
-00001730: 0119 00a0 027c 01a1 01a1 017d 027c 0064  .....|.....}.|.d
-00001740: 0219 0064 036b 037d 0374 00a0 037c 027c  ...d.k.}.t...|.|
-00001750: 03a1 027d 0464 047c 006a 047c 0464 0166  ...}.d.|.j.|.d.f
-00001760: 023c 0064 047c 006a 047c 0464 0566 023c  .<.d.|.j.|.d.f.<
-00001770: 0064 047c 006a 047c 0464 0666 023c 0064  .d.|.j.|.d.f.<.d
-00001780: 047c 006a 047c 0464 0766 023c 0064 047c  .|.j.|.d.f.<.d.|
-00001790: 006a 047c 0464 0866 023c 0064 047c 006a  .j.|.d.f.<.d.|.j
-000017a0: 047c 0464 0266 023c 007c 0053 0029 097a  .|.d.f.<.|.S.).z
-000017b0: f146 756e 6374 696f 6e73 2077 696c 6c20  .Functions will 
-000017c0: 7365 7420 6c61 6b65 2069 6420 6e6f 7420  set lake id not 
-000017d0: 696e 2043 6f6e 6e5f 4c61 6b65 5f49 6473  in Conn_Lake_Ids
-000017e0: 2074 6f20 2d31 2e32 3334 3520 696e 2061   to -1.2345 in a
-000017f0: 7474 7269 6275 7465 0a20 2020 2020 2020  ttribute.       
-00001800: 2074 6162 6c65 206f 6620 5061 7468 5f46   table of Path_F
-00001810: 696e 616c 6361 7469 6e66 6f0a 2020 2020  inalcatinfo.    
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
-00001830: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d2d  Notes.    ------
-00001840: 2d0a 0a20 2020 2052 6574 7572 6e73 3a0a  -..    Returns:.
-00001850: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00001860: 2020 2020 4e6f 6e65 2c20 7468 6520 6174      None, the at
-00001870: 7472 6962 7574 6520 7461 626c 6520 6f66  tribute table of
-00001880: 2050 6174 685f 7368 7066 696c 6520 7769   Path_shpfile wi
-00001890: 6c6c 2062 6520 7570 6461 7465 640a 2020  ll be updated.  
-000018a0: 2020 da08 4879 4c61 6b65 4964 7256 0000    ..HyLakeIdrV..
-000018b0: 0072 5700 0000 7201 0000 005a 074c 616b  .rW...r....Z.Lak
-000018c0: 6556 6f6c 5a08 4c61 6b65 4172 6561 5a09  eVolZ.LakeAreaZ.
-000018d0: 4c61 6b65 4465 7074 685a 084c 616b 6574  LakeDepthZ.Laket
-000018e0: 7970 6529 05da 026e 70da 0b6c 6f67 6963  ype)...np..logic
-000018f0: 616c 5f6e 6f74 7220 0000 00da 0b6c 6f67  al_notr .....log
-00001900: 6963 616c 5f61 6e64 7266 0000 0029 055a  ical_andrf...).Z
-00001910: 0c66 696e 616c 6361 745f 706c 795a 0d43  .finalcat_plyZ.C
-00001920: 6f6e 6e5f 4c61 6b65 5f49 6473 da05 6d61  onn_Lake_Ids..ma
-00001930: 736b 31da 056d 6173 6b32 da04 6d61 736b  sk1..mask2..mask
-00001940: 720a 0000 0072 0a00 0000 720e 0000 00da  r....r....r.....
-00001950: 3752 656d 6f76 655f 556e 7365 6c65 6374  7Remove_Unselect
-00001960: 6564 5f4c 616b 655f 4174 7472 6962 7574  ed_Lake_Attribut
-00001970: 655f 496e 5f46 696e 616c 6361 7469 6e66  e_In_Finalcatinf
-00001980: 6f5f 7075 7265 7079 dd00 0000 7314 0000  o_purepy....s...
-00001990: 0000 0d14 010c 010c 020e 010e 010e 010e  ................
-000019a0: 010e 010e 0272 7700 0000 6302 0000 0000  .....rw...c.....
-000019b0: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
-000019c0: 0000 0073 2a00 0000 7c00 6a00 7401 a002  ...s*...|.j.t...
-000019d0: 7401 a003 7c00 6a00 7c01 a102 a101 1900  t...|.j.|.......
-000019e0: 7d02 7c00 6a04 7c02 6401 8d01 7d00 7c00  }.|.j.|.d...}.|.
-000019f0: 5300 2902 4e72 5000 0000 2905 7234 0000  S.).NrP...).r4..
-00001a00: 0072 7100 0000 7272 0000 0072 2000 0000  .rq...rr...r ...
-00001a10: 7261 0000 0029 03da 0574 6162 6c65 da05  ra...)...table..
-00001a20: 6e61 6d65 735a 1372 656d 6f76 655f 636f  namesZ.remove_co
-00001a30: 6c75 6d6e 5f6e 616d 6573 720a 0000 0072  lumn_namesr....r
-00001a40: 0a00 0000 720e 0000 00da 1b63 6c65 616e  ....r......clean
-00001a50: 5f61 7474 7269 6275 7465 5f6e 616d 655f  _attribute_name_
-00001a60: 7075 7265 7079 f700 0000 7306 0000 0000  purepy....s.....
-00001a70: 011a 010c 0172 7a00 0000 e9ff ffff ff63  .....rz........c
-00001a80: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00001a90: 0400 0000 4300 0000 73ca 0000 007c 0164  ....C...s....|.d
-00001aa0: 016b 0472 1a7c 0064 0219 00a0 0064 03a1  .k.r.|.d.....d..
-00001ab0: 017c 0064 023c 007c 0064 0219 00a0 01a1  .|.d.<.|.d......
-00001ac0: 000f 007d 027c 006a 020f 007d 037c 006a  ...}.|.j...}.|.j
-00001ad0: 0364 016b 047d 0474 04a0 057c 027c 03a1  .d.k.}.t...|.|..
-00001ae0: 027d 0574 04a0 057c 047c 05a1 027d 067c  .}.t...|.|...}.|
-00001af0: 006a 067c 0619 007d 007c 006a 067c 006a  .j.|...}.|.j.|.j
-00001b00: 0764 046b 0319 007d 0074 087c 006a 067c  .d.k...}.t.|.j.|
-00001b10: 006a 0764 056b 0219 0083 0164 016b 0472  .j.d.k.....d.k.r
-00001b20: b074 0964 0683 0101 0074 0964 0783 0101  .t.d.....t.d....
-00001b30: 0074 097c 006a 067c 006a 0764 056b 0219  .t.|.j.|.j.d.k..
-00001b40: 0083 0101 0074 0964 0683 0101 007c 006a  .....t.d.....|.j
-00001b50: 067c 006a 0764 056b 0319 007d 007c 006a  .|.j.d.k...}.|.j
-00001b60: 0a01 007c 0053 0029 084e 7201 0000 0072  ...|.S.).Nr....r
-00001b70: 4f00 0000 6795 6479 e17f fda5 3dda 0550  O...g.dy....=..P
-00001b80: 6f69 6e74 da12 4765 6f6d 6574 7279 436f  oint..GeometryCo
-00001b90: 6c6c 6563 7469 6f6e 7a1b 2323 2323 2323  llectionz.######
-00001ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001bb0: 2323 2323 237a 1c63 6865 636b 2074 6865  #####z.check the
-00001bc0: 2066 6f6c 6c6f 7769 6e67 2066 6561 7475   following featu
-00001bd0: 7265 7329 0bda 0662 7566 6665 72da 0469  res)...buffer..i
-00001be0: 736e 61da 0869 735f 656d 7074 79da 0461  sna..is_empty..a
-00001bf0: 7265 6172 7100 0000 7273 0000 0072 6600  rearq...rs...rf.
-00001c00: 0000 da09 6765 6f6d 5f74 7970 6572 1f00  ....geom_typer..
-00001c10: 0000 7235 0000 00da 0673 696e 6465 7829  ..r5.....sindex)
-00001c20: 0772 3b00 0000 5a0d 7365 745f 7072 6563  .r;...Z.set_prec
-00001c30: 6973 696f 6e5a 056e 6172 6f77 5a05 656d  isionZ.narowZ.em
-00001c40: 726f 775a 0761 7265 6172 6f77 5a04 726f  rowZ.arearowZ.ro
-00001c50: 7731 5a09 726f 7773 656c 6563 7472 0a00  w1Z.rowselectr..
-00001c60: 0000 720a 0000 0072 0e00 0000 7233 0000  ..r....r....r3..
-00001c70: 00fc 0000 0073 2200 0000 0003 0801 1206  .....s".........
-00001c80: 0e02 0802 0a03 0c01 0c03 0a02 1001 1801  ................
-00001c90: 0801 0801 1401 0802 1001 0602 7233 0000  ............r3..
-00001ca0: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
-00001cb0: 0000 0300 0000 4300 0000 7338 0000 007c  ......C...s8...|
-00001cc0: 006a 007d 037c 00a0 01a1 007d 047c 00a0  .j.}.|.....}.|..
-00001cd0: 027c 01a1 017d 047c 046a 037c 047c 023c  .|...}.|.j.|.|.<
-00001ce0: 007c 046a 0164 0164 028d 01a0 027c 03a1  .|.j.d.d.....|..
-00001cf0: 017d 057c 0553 0029 034e 5472 1a00 0000  .}.|.S.).NTr....
-00001d00: 2904 722d 0000 0072 1e00 0000 7230 0000  ).r-...r....r0..
-00001d10: 0072 8100 0000 2906 723b 0000 005a 0770  .r....).r;...Z.p
-00001d20: 726a 5f63 7273 5a08 6172 6561 5f63 6f6c  rj_crsZ.area_col
-00001d30: da07 7372 635f 7372 63da 0474 6f73 74da  ..src_src..tost.
-00001d40: 036f 7574 720a 0000 0072 0a00 0000 720e  .outr....r....r.
-00001d50: 0000 00da 0e61 6464 5f61 7265 615f 696e  .....add_area_in
-00001d60: 5f6d 321f 0100 0073 0c00 0000 0001 0601  _m2....s........
-00001d70: 0802 0a01 0a02 1202 7287 0000 0063 0300  ........r....c..
-00001d80: 0000 0000 0000 0000 0000 0600 0000 0300  ................
-00001d90: 0000 4300 0000 734a 0000 007c 006a 007d  ..C...sJ...|.j.}
-00001da0: 037c 00a0 01a1 007d 047c 04a0 0264 01a1  .|.....}.|...d..
-00001db0: 017d 047c 046a 036a 046a 057c 047c 023c  .}.|.j.j.j.|.|.<
-00001dc0: 007c 046a 036a 046a 067c 047c 013c 007c  .|.j.j.j.|.|.<.|
-00001dd0: 046a 0164 0264 038d 01a0 027c 03a1 017d  .j.d.d.....|...}
-00001de0: 057c 0553 0029 044e fa09 4550 5347 3a34  .|.S.).N..EPSG:4
-00001df0: 3332 3654 721a 0000 0029 0772 2d00 0000  326Tr....).r-...
-00001e00: 721e 0000 0072 3000 0000 724f 0000 00da  r....r0...rO....
-00001e10: 0863 656e 7472 6f69 64da 0179 720b 0000  .centroid..yr...
-00001e20: 0029 0672 3b00 0000 5a04 636f 6c78 5a04  .).r;...Z.colxZ.
-00001e30: 636f 6c79 7284 0000 0072 8500 0000 7286  colyr....r....r.
-00001e40: 0000 0072 0a00 0000 720a 0000 0072 0e00  ...r....r....r..
-00001e50: 0000 7263 0000 002a 0100 0073 0e00 0000  ..rc...*...s....
-00001e60: 0001 0601 0802 0a02 0e01 0e02 1202 7263  ..............rc
-00001e70: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001e80: 1c00 0000 0800 0000 4300 0000 737e 0300  ........C...s~..
-00001e90: 0064 017c 0076 0172 0c64 0053 0074 006a  .d.|.v.r.d.S.t.j
-00001ea0: 01a0 027c 00a1 017d 0174 006a 01a0 037c  ...|...}.t.j...|
-00001eb0: 00a1 01a0 0464 02a1 017d 0274 057c 0283  .....d...}.t.|..
-00001ec0: 017d 037c 027c 0364 0318 0019 0064 0464  .}.|.|.d.....d.d
-00001ed0: 0585 0219 007d 0467 0064 06a2 017d 0564  .....}.g.d...}.d
-00001ee0: 017d 0664 077d 0764 087d 0864 097d 0967  .}.d.}.d.}.d.}.g
-00001ef0: 007d 0a67 007d 0b64 0a7c 0476 0072 e87c  .}.g.}.d.|.v.r.|
-00001f00: 0664 0217 007c 0417 0064 0b17 007c 0764  .d...|...d...|.d
-00001f10: 0217 007c 0417 0064 0b17 007c 0864 0217  ...|...d...|.d..
-00001f20: 007c 0417 0064 0b17 007c 0964 0217 007c  .|...d...|.d...|
-00001f30: 0417 0064 0b17 0067 047d 0a7c 0664 0217  ...d...g.}.|.d..
-00001f40: 007c 0417 0064 0c17 007c 0764 0217 007c  .|...d...|.d...|
-00001f50: 0417 0064 0c17 007c 0864 0217 007c 0417  ...d...|.d...|..
-00001f60: 0064 0c17 007c 0964 0217 007c 0417 0064  .d...|.d...|...d
-00001f70: 0c17 0067 047d 0b6e 387c 0664 0b17 007c  ...g.}.n8|.d...|
-00001f80: 0764 0b17 007c 0864 0b17 007c 0964 0b17  .d...|.d...|.d..
-00001f90: 0067 047d 0a7c 0664 0c17 007c 0764 0c17  .g.}.|.d...|.d..
-00001fa0: 007c 0864 0c17 007c 0964 0c17 0067 047d  .|.d...|.d...g.}
-00001fb0: 0b67 007d 0c67 007d 0d74 0664 0474 057c  .g.}.g.}.t.d.t.|
-00001fc0: 0a83 0183 0244 0090 015d 2e7d 0e74 006a  .....D...].}.t.j
-00001fd0: 01a0 077c 017c 0a7c 0e19 00a1 027d 0f74  ...|.|.|.....}.t
-00001fe0: 006a 01a0 077c 017c 0b7c 0e19 00a1 027d  .j...|.|.|.....}
-00001ff0: 1074 006a 01a0 087c 0fa1 0190 0173 7290  .t.j...|.....sr.
-00002000: 0171 367c 0ca0 097c 10a1 0101 0064 077c  .q6|...|.....d.|
-00002010: 0a7c 0e19 0076 0090 0173 9864 0d7c 0a7c  .|...v...s.d.|.|
-00002020: 0e19 0076 0090 0172 a27c 0da0 097c 10a1  ...v...r.|...|..
-00002030: 0101 0074 0aa0 0b7c 0fa1 017d 117c 11a0  ...t...|...}.|..
-00002040: 0c64 0ea1 017d 1264 017c 0a7c 0e19 0076  .d...}.d.|.|...v
-00002050: 0090 0173 d264 077c 0a7c 0e19 0076 0090  ...s.d.|.|...v..
-00002060: 0272 147c 1264 0f19 00a0 0d74 0ea1 01a0  .r.|.d.....t....
-00002070: 0d74 0fa1 017c 1264 103c 007c 126a 1044  .t...|.d.<.|.j.D
-00002080: 005d 227d 1364 117c 126a 117c 1364 1066  .]"}.d.|.j.|.d.f
-00002090: 0219 0017 007c 126a 117c 1364 1066 023c  .....|.j.|.d.f.<
-000020a0: 0090 0171 f07c 127d 147c 0544 005d 467d  ...q.|.}.|.D.]F}
-000020b0: 157c 14a0 127c 15a1 017c 1464 123c 007c  .|...|...|.d.<.|
-000020c0: 146a 137c 1064 1364 148d 0201 0074 00a0  .j.|.d.d.....t..
-000020d0: 147c 10a1 016a 1564 151b 0064 151b 007d  .|...j.d...d...}
-000020e0: 167c 1664 166b 0190 0272 1c01 0090 0171  .|.d.k...r.....q
-000020f0: 3690 0271 1c90 0171 3674 057c 0d83 0164  6..q...q6t.|...d
-00002100: 036b 0490 0372 7a74 00a0 1474 006a 01a0  .k...rzt...t.j..
-00002110: 077c 017c 0b64 0419 00a1 02a1 016a 1564  .|.|.d.......j.d
-00002120: 151b 0064 151b 0064 176b 0090 0372 7a74  ...d...d.k...rzt
-00002130: 0664 0474 057c 0d83 0183 0244 005d 807d  .d.t.|.....D.].}
-00002140: 0e74 1674 177c 0d7c 0e19 0083 0183 017d  .t.t.|.|.......}
-00002150: 1764 077c 0d7c 0e19 0076 0090 0372 0667  .d.|.|...v...r.g
-00002160: 007d 187c 1764 1819 0044 005d 227d 197c  .}.|.d...D.]"}.|
-00002170: 1964 1919 0064 1a19 0064 046b 0290 0272  .d...d...d.k...r
-00002180: da7c 18a0 097c 19a1 0101 0090 0271 da7c  .|...|.......q.|
-00002190: 187c 1764 183c 007c 0e64 046b 0290 0372  .|.d.<.|.d.k...r
-000021a0: 167c 177d 1a6e 147c 1a64 1805 0019 007c  .|.}.n.|.d.....|
-000021b0: 1764 1819 0037 0003 003c 0090 0271 ac74  .d...7...<...q.t
-000021c0: 1774 006a 01a0 077c 0164 1ba1 0264 1c64  .t.j...|.d...d.d
-000021d0: 1d64 1e8d 038f 227d 1b74 186a 197c 1a7c  .d...."}.t.j.|.|
-000021e0: 1b64 1f64 0564 208d 0401 0057 0064 0004  .d.d.d ....W.d..
-000021f0: 0004 0083 0301 006e 1231 0090 0373 7030  .......n.1...sp0
-00002200: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00002210: 214e da0d 6669 6e61 6c63 6174 5f69 6e66  !N..finalcat_inf
-00002220: 6fda 015f 721d 0000 0072 0100 0000 e904  o.._r....r......
-00002230: 0000 0029 0667 2d43 1ceb e236 1a3f 67fc  ...).g-C...6.?g.
-00002240: a9f1 d24d 6240 3f67 fca9 f1d2 4d62 503f  ...Mb@?g....MbP?
-00002250: 677b 14ae 47e1 7a74 3f67 7b14 ae47 e17a  g{..G.zt?g{..G.z
-00002260: 843f 679a 9999 9999 99a9 3fda 1166 696e  .?g.......?..fin
-00002270: 616c 6361 745f 696e 666f 5f72 6976 da11  alcat_info_riv..
-00002280: 736c 5f63 6f6e 6e65 6374 6564 5f6c 616b  sl_connected_lak
-00002290: 65da 1573 6c5f 6e6f 6e5f 636f 6e6e 6563  e..sl_non_connec
-000022a0: 7465 645f 6c61 6b65 da01 767a 042e 7368  ted_lake..vz..sh
-000022b0: 707a 082e 6765 6f6a 736f 6e5a 0e63 6f6e  pz..geojsonZ.con
-000022c0: 6e65 6374 6564 5f6c 616b 6572 8800 0000  nected_laker....
-000022d0: 723f 0000 005a 0772 7668 4e61 6d65 da03  r?...Z.rvhName..
-000022e0: 7375 6272 4f00 0000 da07 4765 6f4a 534f  subrO.....GeoJSO
-000022f0: 4e29 01da 0664 7269 7665 7269 0004 0000  N)...driveri....
-00002300: e964 0000 0069 f401 0000 da08 6665 6174  .d...i......feat
-00002310: 7572 6573 7208 0000 0072 5600 0000 7a22  uresr....rV...z"
-00002320: 726f 7574 696e 675f 7072 6f64 7563 745f  routing_product_
-00002330: 6c61 6b65 5f72 6976 6572 2e67 656f 6a73  lake_river.geojs
-00002340: 6f6e da01 777a 0575 7466 2d38 2901 da08  on..wz.utf-8)...
-00002350: 656e 636f 6469 6e67 4629 02da 0c65 6e73  encodingF)...ens
-00002360: 7572 655f 6173 6369 69da 0669 6e64 656e  ure_ascii..inden
-00002370: 7429 1a72 5c00 0000 725d 0000 00da 0764  t).r\...r].....d
-00002380: 6972 6e61 6d65 da08 6261 7365 6e61 6d65  irname..basename
-00002390: da05 7370 6c69 7472 1f00 0000 da05 7261  ..splitr......ra
-000023a0: 6e67 6572 5e00 0000 da06 6578 6973 7473  nger^.....exists
-000023b0: 7221 0000 0072 2e00 0000 722f 0000 0072  r!...r....r/...r
-000023c0: 3000 0000 da06 6173 7479 7065 da03 696e  0.....astype..in
-000023d0: 74da 0373 7472 7268 0000 0072 6600 0000  t..strrh...rf...
-000023e0: da08 7369 6d70 6c69 6679 7265 0000 00da  ..simplifyre....
-000023f0: 0473 7461 74da 0773 745f 7369 7a65 7202  .stat..st_sizer.
-00002400: 0000 0072 5b00 0000 da04 6a73 6f6e da04  ...r[.....json..
-00002410: 6475 6d70 291c 5a12 496e 7075 745f 506f  dump).Z.Input_Po
-00002420: 6c79 676f 6e5f 7061 7468 5a0b 7072 6f64  lygon_pathZ.prod
-00002430: 7563 745f 6469 725a 084e 616d 6573 5f69  uct_dirZ.Names_i
-00002440: 6e5a 076e 5f63 6861 7263 da07 7665 7273  nZ.n_charc..vers
-00002450: 696f 6e5a 0a54 4f4c 4552 414e 4345 735a  ionZ.TOLERANCEsZ
-00002460: 0d68 6561 645f 6e61 6d65 5f63 6174 5a0d  .head_name_catZ.
-00002470: 6865 6164 5f6e 616d 655f 7269 765a 0f68  head_name_rivZ.h
-00002480: 6561 645f 6e61 6d65 5f73 6c61 6b65 5a0f  ead_name_slakeZ.
-00002490: 6865 6164 5f6e 616d 655f 6e6c 616b 655a  head_name_nlakeZ
-000024a0: 0f49 6e70 7574 5f66 696c 655f 6e61 6d65  .Input_file_name
-000024b0: 5a10 4f75 7470 7574 5f66 696c 655f 6e61  Z.Output_file_na
-000024c0: 6d65 5a13 6372 6561 7465 645f 6a61 736f  meZ.created_jaso
-000024d0: 6e5f 6669 6c65 735a 1c63 7265 6174 6564  n_filesZ.created
-000024e0: 5f6a 6173 6f6e 5f66 696c 6573 5f6c 616b  _jason_files_lak
-000024f0: 655f 7269 7672 2300 0000 5a0a 696e 7075  e_rivr#...Z.inpu
-00002500: 745f 7061 7468 5a11 6f75 7470 7574 5f6a  t_pathZ.output_j
-00002510: 6173 6f6e 5f70 6174 685a 0869 6e70 7574  ason_pathZ.input
-00002520: 5f70 645a 0c69 6e70 7574 5f77 6773 5f38  _pdZ.input_wgs_8
-00002530: 34da 0369 6478 5a0c 696e 7075 745f 746f  4..idxZ.input_to
-00002540: 6a73 6f6e 5a09 544f 4c45 5241 4e43 455a  jsonZ.TOLERANCEZ
-00002550: 0e6a 736f 6e5f 6669 6c65 5f73 697a 655a  .json_file_sizeZ
-00002560: 0769 6e6a 736f 6e32 5a0c 6e65 775f 6665  .injson2Z.new_fe
-00002570: 6174 7572 6573 da07 656c 656d 656e 745a  atures..elementZ
-00002580: 156f 7574 7075 745f 6a61 736f 6e5f 6c61  .output_jason_la
-00002590: 6b65 5f72 6976 726d 0000 0072 0a00 0000  ke_rivrm...r....
-000025a0: 720a 0000 0072 0e00 0000 7267 0000 0038  r....r....rg...8
-000025b0: 0100 0073 9000 0000 0002 0802 0402 0c01  ...s............
-000025c0: 1201 0801 1401 0803 0401 0401 0401 0402  ................
-000025d0: 0401 0401 0802 0e01 0e01 0e01 0efc 0407  ................
-000025e0: 0e01 0e01 0e01 0efc 0608 0601 0601 0601  ................
-000025f0: 06fc 0407 0601 0601 0601 06fc 0406 0401  ................
-00002600: 0402 1401 1201 1201 0e01 0401 0a02 1c01  ................
-00002610: 0a03 0a02 0a04 1c01 1801 0a01 2003 0402  ............ ...
-00002620: 0801 0e01 0e02 1401 0a01 0e02 3601 1201  ............6...
-00002630: 1001 0e01 0401 0c01 1201 0e01 0802 0a01  ................
-00002640: 0602 1802 1a01 3202 7267 0000 0029 0272  ......2.rg...).r
-00002650: 2500 0000 7225 0000 0029 0172 3f00 0000  %...r%...).r?...
-00002660: 2901 727b 0000 0029 1a72 2e00 0000 da05  ).r{...).r......
-00002670: 6e75 6d70 7972 7100 0000 725c 0000 00da  numpyrq...r\....
-00002680: 0670 616e 6461 7372 1300 0000 72a6 0000  .pandasr....r...
-00002690: 0072 0200 0000 7203 0000 0072 5900 0000  .r....r....rY...
-000026a0: 7236 0000 005a 056f 7367 656f 7204 0000  r6...Z.osgeor...
-000026b0: 0072 0500 0000 5a0b 7261 7374 6572 7374  .r....Z.rasterst
-000026c0: 6174 7372 0600 0000 7219 0000 0072 2400  atsr....r....r$.
-000026d0: 0000 723e 0000 0072 6f00 0000 7277 0000  ..r>...ro...rw..
-000026e0: 0072 7a00 0000 7233 0000 0072 8700 0000  .rz...r3...r....
-000026f0: 7263 0000 0072 6700 0000 720a 0000 0072  rc...rg...r....r
-00002700: 0a00 0000 720a 0000 0072 0e00 0000 da08  ....r....r......
-00002710: 3c6d 6f64 756c 653e 0100 0000 7328 0000  <module>....s(..
-00002720: 0008 0108 0108 0108 0110 0108 0108 0108  ................
-00002730: 0310 010c 0208 0c08 1c00 ff0a 4b0a 5d08  ............K.].
-00002740: 1a08 050a 2308 0b08 0e                   ....#....
+000000c0: 6412 8400 5a15 6413 6414 8400 5a16 6420  d...Z.d.d...Z.d 
+000000d0: 6416 6417 8401 5a17 6418 6419 8400 5a18  d.d...Z.d.d...Z.
+000000e0: 641a 641b 8400 5a19 641c 641d 8400 5a1a  d.d...Z.d.d...Z.
+000000f0: 6401 5300 2921 e900 0000 004e 2902 da04  d.S.)!.....N)...
+00000100: 6c6f 6164 da0b 4a53 4f4e 456e 636f 6465  load..JSONEncode
+00000110: 7229 02da 0467 6461 6cda 036f 6772 2901  r)...gdal..ogr).
+00000120: da0b 7a6f 6e61 6c5f 7374 6174 7363 0400  ..zonal_statsc..
+00000130: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+00000140: 0000 0300 0000 7336 0000 0074 007c 007c  ......s6...t.|.|
+00000150: 017c 0264 0164 0164 028d 057d 0474 0174  .|.d.d.d...}.t.t
+00000160: 0287 0066 0164 0364 0484 087c 0483 0283  ...f.d.d...|....
+00000170: 017d 0574 03a0 047c 05a1 017d 067c 0653  .}.t...|...}.|.S
+00000180: 0029 054e 5429 03da 0573 7461 7473 5a0b  .).NT)...statsZ.
+00000190: 6765 6f6a 736f 6e5f 6f75 745a 0b61 6c6c  geojson_outZ.all
+000001a0: 5f74 6f75 6368 6564 6301 0000 0000 0000  _touchedc.......
+000001b0: 0000 0000 0001 0000 0005 0000 0013 0000  ................
+000001c0: 0073 1c00 0000 8800 7c00 6401 1900 8800  .s......|.d.....
+000001d0: 1900 6402 7c00 6401 1900 6402 1900 6902  ..d.|.d...d...i.
+000001e0: 5300 2903 4eda 0a70 726f 7065 7274 6965  S.).N..propertie
+000001f0: 73da 046d 6561 6ea9 0029 01da 0178 a901  s..mean..)...x..
+00000200: da03 6b65 7972 0a00 0000 fa47 633a 5c75  ..keyr.....Gc:\u
+00000210: 7365 7273 5c6d 3433 6861 6e5f 325c 646f  sers\m43han_2\do
+00000220: 6375 6d65 6e74 735c 6769 7468 7562 5c62  cuments\github\b
+00000230: 6173 696e 6d61 6b65 725c 6261 7369 6e6d  asinmaker\basinm
+00000240: 616b 6572 5c66 756e 635c 7075 7265 7079  aker\func\purepy
+00000250: 2e70 79da 083c 6c61 6d62 6461 3e12 0000  .py..<lambda>...
+00000260: 00f3 0000 0000 7a20 7a6f 6e61 6c5f 7374  ......z zonal_st
+00000270: 6174 735f 7064 2e3c 6c6f 6361 6c73 3e2e  ats_pd.<locals>.
+00000280: 3c6c 616d 6264 613e 2905 7206 0000 00da  <lambda>).r.....
+00000290: 046c 6973 74da 036d 6170 da02 7064 da09  .list..map..pd..
+000002a0: 4461 7461 4672 616d 6529 07da 0773 6870  DataFrame)...shp
+000002b0: 5f67 7064 da06 7261 7374 6572 7207 0000  _gpd..rasterr...
+000002c0: 0072 0d00 0000 da06 7265 7375 6c74 5a0f  .r......resultZ.
+000002d0: 7265 6175 6c74 5f6c 6973 745f 6469 63da  reault_list_dic.
+000002e0: 0972 6561 756c 745f 7064 720a 0000 0072  .reault_pdr....r
+000002f0: 0c00 0000 720e 0000 00da 0e7a 6f6e 616c  ....r......zonal
+00000300: 5f73 7461 7473 5f70 640e 0000 0073 0800  _stats_pd....s..
+00000310: 0000 0002 1202 1602 0a02 7219 0000 0063  ..........r....c
+00000320: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
+00000330: 0500 0000 4300 0000 73ce 0000 007c 006a  ....C...s....|.j
+00000340: 0064 0164 028d 017d 0564 037d 0674 017c  .d.d...}.d.}.t.|
+00000350: 0583 0164 036b 0472 a87c 0664 046b 0172  ...d.k.r.|.d.k.r
+00000360: a874 027c 057c 017c 027c 0383 047d 077c  .t.|.|.|.|...}.|
+00000370: 077c 0764 0519 0064 036b 040f 0019 0064  .|.d...d.k.....d
+00000380: 0619 007d 087c 057c 0564 0619 00a0 037c  ...}.|.|.d.....|
+00000390: 08a1 0119 006a 0064 0164 028d 017d 057c  .....j.d.d...}.|
+000003a0: 0664 036b 0272 847c 077c 0764 0519 0064  .d.k.r.|.|.d...d
+000003b0: 036b 0419 007d 097c 0664 0717 007d 0671  .k...}.|.d...}.q
+000003c0: 107c 0664 0717 007d 067c 077c 0764 0519  .|.d...}.|.|.d..
+000003d0: 0064 036b 0419 007d 0a7c 09a0 047c 0aa1  .d.k...}.|...|..
+000003e0: 017d 0971 1074 017c 0583 0164 036b 0472  .}.q.t.|...d.k.r
+000003f0: ca7c 057c 0419 007c 0564 053c 007c 09a0  .|.|...|.d.<.|..
+00000400: 047c 05a1 017d 097c 0953 0029 084e 54a9  .|...}.|.S.).NT.
+00000410: 01da 0464 6565 7072 0100 0000 e905 0000  ...deepr........
+00000420: 0072 0900 0000 da0a 4852 555f 4944 5f4e  .r......HRU_ID_N
+00000430: 6577 e901 0000 0029 05da 0463 6f70 79da  ew.....)...copy.
+00000440: 036c 656e 7219 0000 00da 0469 7369 6eda  .lenr......isin.
+00000450: 0661 7070 656e 6429 0b72 1500 0000 7216  .append).r....r.
+00000460: 0000 0072 0700 0000 720d 0000 00da 0363  ...r....r......c
+00000470: 6f6c 5a09 6e6f 6461 7461 5f70 64da 0169  olZ.nodata_pd..i
+00000480: 5a07 7465 6d70 5f70 645a 0e62 6164 5f68  Z.temp_pdZ.bad_h
+00000490: 7275 5f76 616c 7565 7372 1800 0000 5a07  ru_valuesr....Z.
+000004a0: 676f 6f64 5f70 6472 0a00 0000 720a 0000  good_pdr....r...
+000004b0: 0072 0e00 0000 da0a 5a6f 6e61 6c53 7461  .r......ZonalSta
+000004c0: 7473 1a00 0000 7320 0000 0000 060c 0104  ts....s ........
+000004d0: 0114 010e 0116 011a 0108 0110 010a 0208  ................
+000004e0: 0110 010c 020c 010c 010a 0272 2500 0000  ...........r%...
+000004f0: fa01 2363 0600 0000 0000 0000 0000 0000  ..#c............
+00000500: 0d00 0000 0600 0000 4300 0000 730a 0100  ........C...s...
+00000510: 007c 036a 007d 0674 01a0 027c 00a1 017d  .|.j.}.t...|...}
+00000520: 077c 07a0 037c 06a1 017d 087c 086a 0464  .|...|...}.|.j.d
+00000530: 0164 028d 017d 087c 08a0 057c 03a1 017d  .d...}.|...|...}
+00000540: 0974 067c 0964 0383 027d 0a7c 0464 046b  .t.|.d...}.|.d.k
+00000550: 0390 0172 067c 017c 096a 0776 0172 6074  ...r.|.|.j.v.r`t
+00000560: 087c 0164 0583 0201 0074 09a0 0aa1 0001  .|.d.....t......
+00000570: 007c 017c 056a 0776 0172 7c74 087c 0164  .|.|.j.v.r|t.|.d
+00000580: 0683 0201 0074 09a0 0aa1 0001 007c 047c  .....t.......|.|
+00000590: 056a 0776 0172 9874 087c 0464 0683 0201  .j.v.r.t.|.d....
+000005a0: 0074 09a0 0aa1 0001 007c 056a 0b64 0164  .t.......|.j.d.d
+000005b0: 078d 017d 0b7c 0b6a 0c7c 0467 0164 0864  ...}.|.j.|.g.d.d
+000005c0: 0164 098d 037d 0b7c 0b7c 0119 007c 0b64  .d...}.|.|...|.d
+000005d0: 0a3c 007c 0b7c 0464 0a67 0219 007d 0b74  .<.|.|.d.g...}.t
+000005e0: 0d6a 0e7c 057c 0b64 0b7c 0464 0c8d 046a  .j.|.|.d.|.d...j
+000005f0: 0b64 0164 078d 017d 0c74 0d6a 0e7c 0a7c  .d.d...}.t.j.|.|
+00000600: 0c64 0b7c 0164 0c8d 047d 0a7c 0a64 0a19  .d.|.d...}.|.d..
+00000610: 007c 0a7c 013c 007c 0a53 0029 0d61 b205  .|.|.<.|.S.).a..
+00000620: 0000 5072 6570 726f 6365 7373 2075 7365  ..Preprocess use
+00000630: 7220 7072 6f76 6964 6564 2070 6f6c 7967  r provided polyg
+00000640: 6f6e 730a 0a20 2020 2046 756e 6374 696f  ons..    Functio
+00000650: 6e20 7468 6174 2077 696c 6c20 7265 7072  n that will repr
+00000660: 6f6a 6563 7420 636c 6970 2069 6e70 7574  oject clip input
+00000670: 2070 6f6c 7967 6f6e 2077 6974 6820 7375   polygon with su
+00000680: 6262 6173 696e 2070 6f6c 7967 6f6e 0a20  bbasin polygon. 
+00000690: 2020 2061 6e64 2077 696c 6c20 6469 7373     and will diss
+000006a0: 6f6c 7665 2074 6865 2069 6e70 7574 2070  olve the input p
+000006b0: 6f6c 7967 6f6e 2062 6173 6564 206f 6e20  olygon based on 
+000006c0: 7468 6569 7220 4944 2c20 7375 6368 2061  their ID, such a
+000006d0: 7320 6c61 6e64 7573 6520 6964 0a20 2020  s landuse id.   
+000006e0: 206f 7220 736f 696c 2069 642e 0a0a 2020   or soil id...  
+000006f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000700: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000710: 7072 6f63 6573 7369 6e67 2020 2020 2020  processing      
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 2020 3a20 7167 6973 206f 626a 6563 740a    : qgis object.
+00000740: 2020 2020 636f 6e74 6578 7420 2020 2020      context     
+00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000760: 2020 2020 2020 3a20 7167 6973 206f 626a        : qgis obj
+00000770: 6563 740a 2020 2020 6c61 7965 725f 7061  ect.    layer_pa
+00000780: 7468 2020 2020 2020 2020 2020 2020 2020  th              
+00000790: 2020 2020 2020 2020 2020 3a20 7374 7269            : stri
+000007a0: 6e67 0a20 2020 2020 2020 2054 6865 2070  ng.        The p
+000007b0: 6174 6820 746f 2061 2073 7065 6369 6669  ath to a specifi
+000007c0: 6320 706f 6c79 676f 6e2c 2066 6f72 2065  c polygon, for e
+000007d0: 7861 6d70 6c65 2070 6174 6820 746f 206c  xample path to l
+000007e0: 616e 6475 7365 206c 6179 6572 0a20 2020  anduse layer.   
+000007f0: 2050 726f 6a65 6374 5f63 7273 2020 2020   Project_crs    
+00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000810: 2020 203a 2073 7472 696e 670a 2020 2020     : string.    
+00000820: 2020 2020 7468 6520 4550 5347 2063 6f64      the EPSG cod
+00000830: 6520 6f66 2061 2070 726f 6a65 6374 6564  e of a projected
+00000840: 2063 6f6f 6469 6e61 7465 2073 7973 7465   coodinate syste
+00000850: 6d20 7468 6174 2077 696c 6c20 6265 2075  m that will be u
+00000860: 7365 6420 746f 0a20 2020 2020 2020 2063  sed to.        c
+00000870: 616c 6375 6174 6520 4852 5520 6172 6561  alcuate HRU area
+00000880: 2061 6e64 2073 6c6f 7065 2e0a 2020 2020   and slope..    
+00000890: 7472 675f 6372 7320 2020 2020 2020 2020  trg_crs         
+000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008b0: 2020 3a20 7374 7269 6e67 0a20 2020 2020    : string.     
+000008c0: 2020 2074 6865 2045 5053 4720 636f 6465     the EPSG code
+000008d0: 206f 6620 6120 2063 6f6f 6469 6e61 7465   of a  coodinate
+000008e0: 2073 7973 7465 6d20 7468 6174 2077 696c   system that wil
+000008f0: 6c20 6265 2075 7365 6420 746f 0a20 2020  l be used to.   
+00000900: 2020 2020 2063 616c 6375 6174 6520 7265       calcuate re
+00000910: 7072 6f6a 6563 7420 696e 7075 7420 706f  project input po
+00000920: 6c79 676f 6e0a 2020 2020 436c 6173 735f  lygon.    Class_
+00000930: 436f 6c20 2020 2020 2020 2020 2020 2020  Col             
+00000940: 2020 2020 2020 2020 2020 2020 3a20 7374              : st
+00000950: 7269 6e67 0a20 2020 2020 2020 2074 6865  ring.        the
+00000960: 2063 6f6c 756d 6e20 6e61 6d65 2069 6e20   column name in 
+00000970: 7468 6520 696e 7075 7420 706f 6c79 676f  the input polygo
+00000980: 6e20 286c 6179 6572 5f70 6174 6829 2074  n (layer_path) t
+00000990: 6861 7420 636f 6e74 6169 6e73 0a20 2020  hat contains.   
+000009a0: 2020 2020 2074 6865 6972 2049 442c 2066       their ID, f
+000009b0: 6f72 2065 7861 6d70 6c65 206c 616e 6420  or example land 
+000009c0: 7573 6520 4944 206f 7220 736f 696c 2049  use ID or soil I
+000009d0: 442e 0a20 2020 204c 6179 6572 5f63 6c69  D..    Layer_cli
+000009e0: 7020 2020 2020 2020 2020 2020 2020 2020  p               
+000009f0: 2020 2020 2020 2020 203a 2071 6769 7320           : qgis 
+00000a00: 6f62 6a65 6374 0a20 2020 2020 2020 2041  object.        A
+00000a10: 2073 6870 6669 6c65 2077 6974 6820 6578   shpfile with ex
+00000a20: 7465 6e74 206f 6620 7468 6520 7761 7465  tent of the wate
+00000a30: 7273 6865 642c 2077 696c 6c20 6265 2075  rshed, will be u
+00000a40: 7365 6420 746f 2063 6c69 7020 696e 7075  sed to clip inpu
+00000a50: 740a 2020 2020 2020 2020 696e 7075 7420  t.        input 
+00000a60: 706f 6c79 676f 6e0a 2020 2020 4e6f 7465  polygon.    Note
+00000a70: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00000a80: 2020 2020 2020 2320 544f 444f 3a20 4d61        # TODO: Ma
+00000a90: 7920 6265 2061 6464 2073 6f6d 6520 6675  y be add some fu
+00000aa0: 6e63 7469 6f6e 2074 6f20 7369 6d70 6c69  nction to simpli
+00000ab0: 6679 2074 6865 2069 6e70 7574 2070 6f6c  fy the input pol
+00000ac0: 7967 6f6e 730a 2020 2020 2020 2020 2020  ygons.          
+00000ad0: 2020 2020 2020 666f 7220 6578 616d 706c        for exampl
+00000ae0: 652c 2072 656d 6f76 6520 7468 6520 6c61  e, remove the la
+00000af0: 6e64 7573 6520 7479 7065 2077 6974 6820  nduse type with 
+00000b00: 736d 616c 6c20 6172 6561 730a 2020 2020  small areas.    
+00000b10: 2020 2020 2020 2020 2020 2020 6f72 206d              or m
+00000b20: 6572 6765 2073 6d61 6c6c 206c 616e 6475  erge small landu
+00000b30: 7365 2070 6f6c 7967 6f6e 2069 6e74 6f20  se polygon into 
+00000b40: 7468 6520 7375 7272 6f75 6e64 696e 6720  the surrounding 
+00000b50: 706f 6c79 676f 6e0a 0a20 2020 2052 6574  polygon..    Ret
+00000b60: 7572 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d  urns:.    ------
+00000b70: 2d0a 2020 2020 2020 2020 6c61 7965 725f  -.        layer_
+00000b80: 6469 7320 2020 2020 2020 2020 2020 2020  dis             
+00000b90: 2020 2020 203a 2071 6769 7320 6f62 6a65       : qgis obje
+00000ba0: 6374 0a20 2020 2020 2020 2020 2020 2069  ct.            i
+00000bb0: 7420 6973 2061 2070 6f6c 7967 6f6e 2061  t is a polygon a
+00000bc0: 6674 6572 2070 7265 7072 6f63 6573 730a  fter preprocess.
+00000bd0: 2020 2020 5429 01da 0c69 676e 6f72 655f      T)...ignore_
+00000be0: 696e 6465 7872 1e00 0000 7226 0000 007a  indexr....r&...z
+00000bf0: 3120 6e6f 7420 696e 2074 6865 2061 7474  1 not in the att
+00000c00: 7269 6275 7465 2074 6162 6c65 206f 6620  ribute table of 
+00000c10: 7072 6f76 6964 6564 2073 6861 7065 6669  provided shapefi
+00000c20: 6c65 7a32 206e 6f74 2069 6e20 7468 6520  lez2 not in the 
+00000c30: 6174 7472 6962 7574 6520 7461 626c 6520  attribute table 
+00000c40: 6f66 2070 726f 7669 6465 6420 696e 666f  of provided info
+00000c50: 2074 6162 6c65 721a 0000 00da 046c 6173   tabler......las
+00000c60: 7429 03da 0673 7562 7365 74da 046b 6565  t)...subset..kee
+00000c70: 7072 2700 0000 5a06 4e65 775f 4944 da05  pr'...Z.New_ID..
+00000c80: 696e 6e65 7229 02da 0368 6f77 da02 6f6e  inner)...how..on
+00000c90: 290f da03 6372 73da 0967 656f 7061 6e64  )...crs..geopand
+00000ca0: 6173 da09 7265 6164 5f66 696c 65da 0674  as..read_file..t
+00000cb0: 6f5f 6372 73da 0765 7870 6c6f 6465 da04  o_crs..explode..
+00000cc0: 636c 6970 da15 636c 6561 6e5f 6765 6f6d  clip..clean_geom
+00000cd0: 6574 7279 5f70 7572 6570 79da 0763 6f6c  etry_purepy..col
+00000ce0: 756d 6e73 da05 7072 696e 74da 0373 7973  umns..print..sys
+00000cf0: da04 6578 6974 721f 0000 00da 0f64 726f  ..exitr......dro
+00000d00: 705f 6475 706c 6963 6174 6573 7213 0000  p_duplicatesr...
+00000d10: 00da 056d 6572 6765 290d da0a 6c61 7965  ...merge)...laye
+00000d20: 725f 7061 7468 5a09 436c 6173 735f 436f  r_pathZ.Class_Co
+00000d30: 6cda 0a74 656d 7066 6f6c 6465 72da 0a6d  l..tempfolder..m
+00000d40: 6173 6b5f 6c61 7965 725a 0c43 6c61 7373  ask_layerZ.Class
+00000d50: 5f4e 4d5f 436f 6c5a 0a69 6e66 6f5f 7461  _NM_ColZ.info_ta
+00000d60: 626c 655a 076e 6577 5f63 7273 da04 6461  bleZ.new_crs..da
+00000d70: 7461 5a09 7072 6f6a 6563 7465 64da 0763  taZ.projected..c
+00000d80: 6c69 7070 6564 da07 636c 6561 6e65 645a  lipped..cleanedZ
+00000d90: 0f69 6e66 6f5f 7461 626c 655f 636f 7079  .info_table_copy
+00000da0: 5a10 696e 666f 5f74 6162 6c65 5f63 6f70  Z.info_table_cop
+00000db0: 7932 720a 0000 0072 0a00 0000 720e 0000  y2r....r....r...
+00000dc0: 00da 2c52 6570 726f 6a5f 436c 6970 5f44  ..,Reproj_Clip_D
+00000dd0: 6973 736f 6c76 655f 5369 6d70 6c69 6679  issolve_Simplify
+00000de0: 5f50 6f6c 7967 6f6e 5f70 7572 6570 7935  _Polygon_purepy5
+00000df0: 0000 0073 3000 0000 0027 0601 0a02 0a01  ...s0....'......
+00000e00: 0c01 0a03 0a01 0a01 0a01 0a01 0801 0a01  ................
+00000e10: 0a01 0801 0a01 0a01 0802 0c01 1201 0c01  ................
+00000e20: 0c01 1a02 1201 0c06 7241 0000 00da 0553  ........rA.....S
+00000e30: 7562 4964 6307 0000 0000 0000 0000 0000  ubIdc...........
+00000e40: 0014 0000 0008 0000 0043 0000 0073 2604  .........C...s&.
+00000e50: 0000 6700 6401 a201 7d07 6402 7c00 6a00  ..g.d...}.d.|.j.
+00000e60: 7600 7218 6403 7d08 6e04 6404 7d08 7401  v.r.d.}.n.d.}.t.
+00000e70: a002 7c08 a101 7d09 7403 7404 6a05 a006  ..|...}.t.t.j...
+00000e80: 7c02 6405 a102 6406 8302 8f1c 7d0a 7c0a  |.d...d.....}.|.
+00000e90: a007 7c09 6a08 a101 0100 5700 6400 0400  ..|.j.....W.d...
+00000ea0: 0400 8303 0100 6e10 3100 735c 3000 0100  ......n.1.s\0...
+00000eb0: 0100 0100 5900 0100 7c04 6407 6b03 9002  ....Y...|.d.k...
+00000ec0: 72c4 7c05 6407 6b03 728e 7409 a00a 7c05  r.|.d.k.r.t...|.
+00000ed0: a101 7d0b 7c0b 6408 1900 7c0b 6409 3c00  ..}.|.d...|.d.<.
+00000ee0: 7c00 6a0b 640a 640b 8d01 6a0c 640c 640d  |.j.d.d...j.d.d.
+00000ef0: 8d01 7d0c 7c05 6407 6b03 72d8 7c0b 640a  ..}.|.d.k.r.|.d.
+00000f00: 6409 6702 1900 7d0b 740d 6a0e 7c0b 7c0c  d.g...}.t.j.|.|.
+00000f10: 6409 640e 640f 8d04 7d0b 7c0b 6a0f 7c06  d.d.d...}.|.j.|.
+00000f20: 6410 6411 6412 8d03 7d0b 7c00 6a0f 7c06  d.d.d...}.|.j.|.
+00000f30: 6410 6411 6412 8d03 7d00 7410 7c00 6413  d.d.d...}.t.|.d.
+00000f40: 6414 8303 7d00 7c00 6414 6413 6702 1900  d...}.|.d.d.g...
+00000f50: 6a0c 640c 640d 8d01 7d0d 7c05 6407 6b03  j.d.d...}.|.d.k.
+00000f60: 9001 722c 7c0b 6a0b 6414 6413 6702 640b  ..r,|.j.d.d.g.d.
+00000f70: 8d01 7d0b 7c0b a006 7c0d a101 7d0b 7c00  ..}.|...|...}.|.
+00000f80: 7c00 6415 1900 6416 6b03 1900 6408 6417  |.d...d.k...d.d.
+00000f90: 6702 1900 6a0c 640c 640d 8d01 7d0e 6700  g...j.d.d...}.g.
+00000fa0: 7d0f 7c0e 6408 1900 6a11 4400 5d20 7d10  }.|.d...j.D.] }.
+00000fb0: 7c10 7c0e 6417 1900 6a11 7601 9001 725a  |.|.d...j.v...rZ
+00000fc0: 7c0f a012 7c10 a101 0100 9001 715a 7c05  |...|.......qZ|.
+00000fd0: 6407 6b03 9001 72da 7c0b 7c0b 6a13 a014  d.k...r.|.|.j...
+00000fe0: 7c0f a101 0f00 1900 7d0b 7c0b 6a00 7d11  |.......}.|.j.}.
+00000ff0: 7c11 7c11 a014 7c07 a101 1900 7d12 7c0b  |.|...|.....}.|.
+00001000: 6a0b 7c12 640b 8d01 7d0b 7415 7c0b 8301  j.|.d...}.t.|...
+00001010: 6418 6b04 9001 72da 7c0b a016 7404 6a05  d.k...r.|...t.j.
+00001020: a006 7c02 7c04 a102 a101 0100 6419 7c00  ..|.|.......d.|.
+00001030: 6a17 7c00 6a13 a014 7c0f a101 641a 6602  j.|.j...|...d.f.
+00001040: 3c00 6419 7c00 6a17 7c00 6a13 a014 7c0f  <.d.|.j.|.j...|.
+00001050: a101 641b 6602 3c00 6419 7c00 6a17 7c00  ..d.f.<.d.|.j.|.
+00001060: 6a13 a014 7c0f a101 641c 6602 3c00 6419  j...|...d.f.<.d.
+00001070: 7c00 6a17 7c00 6a13 a014 7c0f a101 641d  |.j.|.j...|...d.
+00001080: 6602 3c00 6419 7c00 6a17 7c00 6a13 a014  f.<.d.|.j.|.j...
+00001090: 7c0f a101 641e 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
+000010a0: 7c00 6a13 a014 7c0f a101 641f 6602 3c00  |.j...|...d.f.<.
+000010b0: 7c00 6a00 7d11 7c11 7c11 a014 7c07 a101  |.j.}.|.|...|...
+000010c0: 1900 7d12 7c00 6a0b 7c12 640b 8d01 7d00  ..}.|.j.|.d...}.
+000010d0: 7c00 a016 7404 6a05 a006 7c02 7c03 a102  |...t.j...|.|...
+000010e0: a101 0100 7418 7c00 8301 7d13 7c13 a016  ....t.|...}.|...
+000010f0: 7404 6a05 a006 7c02 6420 a102 a101 0100  t.j...|.d ......
+00001100: 7419 7404 6a05 a006 7c02 7c03 a102 8301  t.t.j...|.|.....
+00001110: 0100 9001 6e5e 7c00 6a0f 7c06 6410 6411  ....n^|.j.|.d.d.
+00001120: 6412 8d03 7d00 6414 7c00 6a00 7600 9003  d...}.d.|.j.v...
+00001130: 72ca 7410 7c00 6413 6414 8303 7d00 7c00  r.t.|.d.d...}.|.
+00001140: 6a1a 7c00 6408 3c00 7c00 7c00 6415 1900  j.|.d.<.|.|.d...
+00001150: 6416 6b03 1900 6408 6417 6702 1900 6a0c  d.k...d.d.g...j.
+00001160: 640c 640d 8d01 7d0e 6700 7d0f 7c0e 6408  d.d...}.g.}.|.d.
+00001170: 1900 6a11 4400 5d20 7d10 7c10 7c0e 6417  ..j.D.] }.|.|.d.
+00001180: 1900 6a11 7601 9003 7224 7c0f a012 7c10  ..j.v...r$|...|.
+00001190: a101 0100 9003 7124 6419 7c00 6a17 7c00  ......q$d.|.j.|.
+000011a0: 6a13 a014 7c0f a101 641a 6602 3c00 6419  j...|...d.f.<.d.
+000011b0: 7c00 6a17 7c00 6a13 a014 7c0f a101 641b  |.j.|.j...|...d.
+000011c0: 6602 3c00 6419 7c00 6a17 7c00 6a13 a014  f.<.d.|.j.|.j...
+000011d0: 7c0f a101 641c 6602 3c00 6419 7c00 6a17  |...d.f.<.d.|.j.
+000011e0: 7c00 6a13 a014 7c0f a101 641d 6602 3c00  |.j...|...d.f.<.
+000011f0: 6419 7c00 6a17 7c00 6a13 a014 7c0f a101  d.|.j.|.j...|...
+00001200: 641e 6602 3c00 6419 7c00 6a17 7c00 6a13  d.f.<.d.|.j.|.j.
+00001210: a014 7c0f a101 641f 6602 3c00 7c00 6a00  ..|...d.f.<.|.j.
+00001220: 7d11 7c11 7c11 a014 6700 6421 a201 a101  }.|.|...g.d!....
+00001230: 1900 7d12 7c00 6a0b 7c12 640b 8d01 7d00  ..}.|.j.|.d...}.
+00001240: 7c00 a016 7404 6a05 a006 7c02 7c03 a102  |...t.j...|.|...
+00001250: a101 0100 7418 7c00 8301 7d13 7c13 a016  ....t.|...}.|...
+00001260: 7404 6a05 a006 7c02 6420 a102 a101 0100  t.j...|.d ......
+00001270: 7c00 5300 6400 5300 2922 4e29 10da 0753  |.S.d.S.)"N)...S
+00001280: 7562 4964 5f31 da02 4964 da07 6e73 7562  ubId_1..Id..nsub
+00001290: 6964 32da 066e 7375 6269 64da 0a6e 646f  id2..nsubid..ndo
+000012a0: 776e 7375 6269 64da 094f 6c64 5f53 7562  wnsubid..Old_Sub
+000012b0: 4964 da0a 4f6c 645f 446f 7753 7562 da0a  Id..Old_DowSub..
+000012c0: 4a6f 696e 5f43 6f75 6e74 da0a 5441 5247  Join_Count..TARG
+000012d0: 4554 5f46 4944 7244 0000 00da 0a53 7562  ET_FIDrD.....Sub
+000012e0: 4944 5f4f 6c64 72da 0a48 5255 5f49 445f  ID_Oldr..HRU_ID_
+000012f0: 4e5f 31da 0a48 5255 5f49 445f 4e5f 32da  N_1..HRU_ID_N_2.
+00001300: 0766 6163 7465 7273 da0c 4f6c 645f 446f  .facters..Old_Do
+00001310: 7753 7562 4964 5a07 5375 6249 6474 32da  wSubIdZ.SubIdt2.
+00001320: 0844 415f 4368 6e5f 4c7a 4168 7474 7073  .DA_Chn_LzAhttps
+00001330: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
+00001340: 7374 6d69 6e67 2f52 6f75 7469 6e67 546f  stming/RoutingTo
+00001350: 6f6c 2f77 696b 692f 4669 6c65 732f 5245  ol/wiki/Files/RE
+00001360: 4144 4d45 5f4f 4948 2e70 6466 7a40 6874  ADME_OIH.pdfz@ht
+00001370: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001380: 2f64 7573 746d 696e 672f 526f 7574 696e  /dustming/Routin
+00001390: 6754 6f6f 6c2f 7769 6b69 2f46 696c 6573  gTool/wiki/Files
+000013a0: 2f52 4541 444d 455f 4e41 2e70 6466 7a0a  /README_NA.pdfz.
+000013b0: 5245 4144 4d45 2e70 6466 da02 7762 7226  README.pdf..wbr&
+000013c0: 0000 0072 4200 0000 7248 0000 00da 0867  ...rB...rH.....g
+000013d0: 656f 6d65 7472 79a9 0172 3500 0000 5472  eometry..r5...Tr
+000013e0: 1a00 0000 da04 6c65 6674 2902 722d 0000  ......left).r-..
+000013f0: 0072 2c00 0000 da05 6669 7273 7446 a903  .r,.....firstF..
+00001400: da02 6279 da07 6167 6766 756e 63da 0861  ..by..aggfunc..a
+00001410: 735f 696e 6465 78da 0a63 656e 7472 6f69  s_index..centroi
+00001420: 645f 78da 0a63 656e 7472 6f69 645f 79da  d_x..centroid_y.
+00001430: 084c 616b 655f 4361 74e9 0200 0000 da08  .Lake_Cat.......
+00001440: 446f 7753 7562 4964 7201 0000 0067 8d97  DowSubIdr....g..
+00001450: 6e12 83c0 f3bf da08 5269 7653 6c6f 7065  n.......RivSlope
+00001460: da09 5269 764c 656e 6774 68da 0846 6c6f  ..RivLength..Flo
+00001470: 6f64 505f 6eda 0443 685f 6eda 074d 6178  odP_n..Ch_n..Max
+00001480: 5f44 454d da07 4d69 6e5f 4445 4d7a 0b6f  _DEM..Min_DEMz.o
+00001490: 7574 6c69 6e65 2e73 6870 290f da05 5348  utline.shp)...SH
+000014a0: 4150 4572 4300 0000 7244 0000 0072 4500  APErC...rD...rE.
+000014b0: 0000 7246 0000 0072 4700 0000 7249 0000  ..rF...rG...rI..
+000014c0: 0072 4a00 0000 724b 0000 0072 4400 0000  .rJ...rK...rD...
+000014d0: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
+000014e0: 4f00 0000 7250 0000 0029 1b72 3500 0000  O...rP...).r5...
+000014f0: da08 7265 7175 6573 7473 da03 6765 74da  ..requests..get.
+00001500: 046f 7065 6eda 026f 73da 0470 6174 68da  .open..os..path.
+00001510: 046a 6f69 6eda 0577 7269 7465 da07 636f  .join..write..co
+00001520: 6e74 656e 7472 2f00 0000 7230 0000 00da  ntentr/...r0....
+00001530: 0464 726f 7072 1f00 0000 7213 0000 0072  .dropr....r....r
+00001540: 3a00 0000 da08 6469 7373 6f6c 7665 da15  :.....dissolve..
+00001550: 6164 645f 6365 6e74 726f 6964 5f69 6e5f  add_centroid_in_
+00001560: 7767 7338 34da 0676 616c 7565 7372 2200  wgs84..valuesr".
+00001570: 0000 7242 0000 0072 2100 0000 7220 0000  ..rB...r!...r ..
+00001580: 00da 0774 6f5f 6669 6c65 da03 6c6f 63da  ...to_file..loc.
+00001590: 1963 7265 6174 655f 7761 7465 7273 6865  .create_watershe
+000015a0: 645f 626f 756e 6461 7279 da15 6372 6561  d_boundary..crea
+000015b0: 7465 5f67 656f 5f6a 6173 6f6e 5f66 696c  te_geo_jason_fil
+000015c0: 65da 0569 6e64 6578 2914 da0e 6d61 706f  e..index)...mapo
+000015d0: 6c64 6e65 775f 696e 666f 723c 0000 00da  ldnew_infor<....
+000015e0: 0c4f 7574 7075 7446 6f6c 6465 72da 0863  .OutputFolder..c
+000015f0: 6174 5f6e 616d 65da 0872 6976 5f6e 616d  at_name..riv_nam
+00001600: 65da 0e50 6174 685f 6669 6e61 6c5f 7269  e..Path_final_ri
+00001610: 765a 0c64 6973 5f63 6f6c 5f6e 616d 655a  vZ.dis_col_nameZ
+00001620: 124e 4545 445f 544f 5f52 454d 4f56 455f  .NEED_TO_REMOVE_
+00001630: 4944 53da 0375 726c da08 7265 7370 6f6e  IDS..url..respon
+00001640: 7365 da01 665a 0672 6976 5f70 645a 0663  se..fZ.riv_pdZ.c
+00001650: 6174 5f70 645a 0963 6174 5f63 5f78 5f79  at_pdZ.cat_c_x_y
+00001660: da19 7269 765f 7064 5f6e 6e63 6c73 5f72  ..riv_pd_nncls_r
+00001670: 6f75 7469 6e67 5f69 6e66 6f5a 0e72 656d  outing_infoZ.rem
+00001680: 6f76 655f 6368 616e 6e65 6cda 0573 7562  ove_channel..sub
+00001690: 6964 5a0a 6361 745f 636f 6c6e 6d73 5a0f  idZ.cat_colnmsZ.
+000016a0: 6472 6f70 5f63 6174 5f63 6f6c 6e6d 73da  drop_cat_colnms.
+000016b0: 076f 7574 6c69 6e65 720a 0000 0072 0a00  .outliner....r..
+000016c0: 0000 720e 0000 00da 2373 6176 655f 6d6f  ..r.....#save_mo
+000016d0: 6469 6669 6564 5f61 7474 7269 6275 7465  dified_attribute
+000016e0: 735f 746f 5f6f 7574 7075 7473 8000 0000  s_to_outputs....
+000016f0: 738a 0000 0000 0308 030a 0106 0204 020a  s...............
+00001700: 0116 012a 020a 0208 010a 010c 0214 0208  ...*............
+00001710: 010c 0112 0110 0310 010c 0214 010a 0110  ................
+00001720: 010a 0220 0104 010e 0110 010e 010a 0112  ... ............
+00001730: 0106 010e 010c 010e 0114 0216 0116 0116  ................
+00001740: 0116 0116 0116 0206 010e 010c 0114 0208  ................
+00001750: 0114 0116 0410 020c 020c 010a 0120 0104  ............. ..
+00001760: 010e 0110 010e 0216 0116 0116 0116 0116  ................
+00001770: 0116 0306 0112 010c 0114 0108 0114 0172  ...............r
+00001780: 8300 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001790: 0002 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
+000017a0: 0000 7c00 6a00 6401 6402 8d01 6403 6701  ..|.j.d.d...d.g.
+000017b0: 1900 7d01 6404 7c01 6405 3c00 7c01 6a01  ..}.d.|.d.<.|.j.
+000017c0: 6405 6406 6407 6408 8d03 7d01 7c01 5300  d.d.d.d...}.|.S.
+000017d0: 2909 4e54 721a 0000 0072 5300 0000 721e  ).NTr....rS...r.
+000017e0: 0000 00da 0249 4472 5600 0000 4672 5700  .....IDrV...FrW.
+000017f0: 0000 2902 721f 0000 0072 7000 0000 2902  ..).r....rp...).
+00001800: 7278 0000 0072 5200 0000 720a 0000 0072  rx...rR...r....r
+00001810: 0a00 0000 720e 0000 0072 7500 0000 e000  ....r....ru.....
+00001820: 0000 7308 0000 0000 0112 0108 0110 0172  ..s............r
+00001830: 7500 0000 6302 0000 0000 0000 0000 0000  u...c...........
+00001840: 0005 0000 0005 0000 0043 0000 0073 8400  .........C...s..
+00001850: 0000 7400 a001 7c00 6401 1900 a002 7c01  ..t...|.d.....|.
+00001860: a101 a101 7d02 7c00 6402 1900 6403 6b03  ....}.|.d...d.k.
+00001870: 7d03 7400 a003 7c02 7c03 a102 7d04 6404  }.t...|.|...}.d.
+00001880: 7c00 6a04 7c04 6401 6602 3c00 6404 7c00  |.j.|.d.f.<.d.|.
+00001890: 6a04 7c04 6405 6602 3c00 6404 7c00 6a04  j.|.d.f.<.d.|.j.
+000018a0: 7c04 6406 6602 3c00 6404 7c00 6a04 7c04  |.d.f.<.d.|.j.|.
+000018b0: 6407 6602 3c00 6404 7c00 6a04 7c04 6408  d.f.<.d.|.j.|.d.
+000018c0: 6602 3c00 6404 7c00 6a04 7c04 6402 6602  f.<.d.|.j.|.d.f.
+000018d0: 3c00 7c00 5300 2909 7af1 4675 6e63 7469  <.|.S.).z.Functi
+000018e0: 6f6e 7320 7769 6c6c 2073 6574 206c 616b  ons will set lak
+000018f0: 6520 6964 206e 6f74 2069 6e20 436f 6e6e  e id not in Conn
+00001900: 5f4c 616b 655f 4964 7320 746f 202d 312e  _Lake_Ids to -1.
+00001910: 3233 3435 2069 6e20 6174 7472 6962 7574  2345 in attribut
+00001920: 650a 2020 2020 2020 2020 7461 626c 6520  e.        table 
+00001930: 6f66 2050 6174 685f 4669 6e61 6c63 6174  of Path_Finalcat
+00001940: 696e 666f 0a20 2020 202d 2d2d 2d2d 2d2d  info.    -------
+00001950: 2d2d 2d0a 0a20 2020 204e 6f74 6573 0a20  ---..    Notes. 
+00001960: 2020 202d 2d2d 2d2d 2d2d 0a0a 2020 2020     -------..    
+00001970: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
+00001980: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00001990: 652c 2074 6865 2061 7474 7269 6275 7465  e, the attribute
+000019a0: 2074 6162 6c65 206f 6620 5061 7468 5f73   table of Path_s
+000019b0: 6870 6669 6c65 2077 696c 6c20 6265 2075  hpfile will be u
+000019c0: 7064 6174 6564 0a20 2020 20da 0848 794c  pdated.    ..HyL
+000019d0: 616b 6549 6472 5d00 0000 725e 0000 0072  akeIdr]...r^...r
+000019e0: 0100 0000 da07 4c61 6b65 566f 6cda 084c  ......LakeVol..L
+000019f0: 616b 6541 7265 61da 094c 616b 6544 6570  akeArea..LakeDep
+00001a00: 7468 da08 4c61 6b65 7479 7065 2905 da02  th..Laketype)...
+00001a10: 6e70 da0b 6c6f 6769 6361 6c5f 6e6f 7472  np..logical_notr
+00001a20: 2100 0000 da0b 6c6f 6769 6361 6c5f 616e  !.....logical_an
+00001a30: 6472 7400 0000 2905 5a0c 6669 6e61 6c63  drt...).Z.finalc
+00001a40: 6174 5f70 6c79 da0d 436f 6e6e 5f4c 616b  at_ply..Conn_Lak
+00001a50: 655f 4964 73da 056d 6173 6b31 da05 6d61  e_Ids..mask1..ma
+00001a60: 736b 32da 046d 6173 6b72 0a00 0000 720a  sk2..maskr....r.
+00001a70: 0000 0072 0e00 0000 da37 5265 6d6f 7665  ...r.....7Remove
+00001a80: 5f55 6e73 656c 6563 7465 645f 4c61 6b65  _Unselected_Lake
+00001a90: 5f41 7474 7269 6275 7465 5f49 6e5f 4669  _Attribute_In_Fi
+00001aa0: 6e61 6c63 6174 696e 666f 5f70 7572 6570  nalcatinfo_purep
+00001ab0: 79e6 0000 0073 1400 0000 000d 1401 0c01  y....s..........
+00001ac0: 0c02 0e01 0e01 0e01 0e01 0e01 0e02 7291  ..............r.
+00001ad0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001ae0: 0300 0000 0700 0000 4300 0000 732a 0000  ........C...s*..
+00001af0: 007c 006a 0074 01a0 0274 01a0 037c 006a  .|.j.t...t...|.j
+00001b00: 007c 01a1 02a1 0119 007d 027c 006a 047c  .|.......}.|.j.|
+00001b10: 0264 018d 017d 007c 0053 0029 024e 7254  .d...}.|.S.).NrT
+00001b20: 0000 0029 0572 3500 0000 728a 0000 0072  ...).r5...r....r
+00001b30: 8b00 0000 7221 0000 0072 6f00 0000 2903  ....r!...ro...).
+00001b40: da05 7461 626c 65da 056e 616d 6573 5a13  ..table..namesZ.
+00001b50: 7265 6d6f 7665 5f63 6f6c 756d 6e5f 6e61  remove_column_na
+00001b60: 6d65 7372 0a00 0000 720a 0000 0072 0e00  mesr....r....r..
+00001b70: 0000 da1b 636c 6561 6e5f 6174 7472 6962  ....clean_attrib
+00001b80: 7574 655f 6e61 6d65 5f70 7572 6570 7900  ute_name_purepy.
+00001b90: 0100 0073 0600 0000 0001 1a01 0c01 7294  ...s..........r.
+00001ba0: 0000 00e9 ffff ffff 6302 0000 0000 0000  ........c.......
+00001bb0: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
+00001bc0: 0073 ca00 0000 7c01 6401 6b04 721a 7c00  .s....|.d.k.r.|.
+00001bd0: 6402 1900 a000 6403 a101 7c00 6402 3c00  d.....d...|.d.<.
+00001be0: 7c00 6402 1900 a001 a100 0f00 7d02 7c00  |.d.........}.|.
+00001bf0: 6a02 0f00 7d03 7c00 6a03 6401 6b04 7d04  j...}.|.j.d.k.}.
+00001c00: 7404 a005 7c02 7c03 a102 7d05 7404 a005  t...|.|...}.t...
+00001c10: 7c04 7c05 a102 7d06 7c00 6a06 7c06 1900  |.|...}.|.j.|...
+00001c20: 7d00 7c00 6a06 7c00 6a07 6404 6b03 1900  }.|.j.|.j.d.k...
+00001c30: 7d00 7408 7c00 6a06 7c00 6a07 6405 6b02  }.t.|.j.|.j.d.k.
+00001c40: 1900 8301 6401 6b04 72b0 7409 6406 8301  ....d.k.r.t.d...
+00001c50: 0100 7409 6407 8301 0100 7409 7c00 6a06  ..t.d.....t.|.j.
+00001c60: 7c00 6a07 6405 6b02 1900 8301 0100 7409  |.j.d.k.......t.
+00001c70: 6406 8301 0100 7c00 6a06 7c00 6a07 6405  d.....|.j.|.j.d.
+00001c80: 6b03 1900 7d00 7c00 6a0a 0100 7c00 5300  k...}.|.j...|.S.
+00001c90: 2908 4e72 0100 0000 7253 0000 0067 9564  ).Nr....rS...g.d
+00001ca0: 79e1 7ffd a53d da05 506f 696e 74da 1247  y....=..Point..G
+00001cb0: 656f 6d65 7472 7943 6f6c 6c65 6374 696f  eometryCollectio
+00001cc0: 6e7a 1b23 2323 2323 2323 2323 2323 2323  nz.#############
+00001cd0: 2323 2323 2323 2323 2323 2323 2323 7a1c  ##############z.
+00001ce0: 6368 6563 6b20 7468 6520 666f 6c6c 6f77  check the follow
+00001cf0: 696e 6720 6665 6174 7572 6573 290b da06  ing features)...
+00001d00: 6275 6666 6572 da04 6973 6e61 da08 6973  buffer..isna..is
+00001d10: 5f65 6d70 7479 da04 6172 6561 728a 0000  _empty..arear...
+00001d20: 0072 8c00 0000 7274 0000 00da 0967 656f  .r....rt.....geo
+00001d30: 6d5f 7479 7065 7220 0000 0072 3600 0000  m_typer ...r6...
+00001d40: da06 7369 6e64 6578 2907 723e 0000 005a  ..sindex).r>...Z
+00001d50: 0d73 6574 5f70 7265 6369 7369 6f6e 5a05  .set_precisionZ.
+00001d60: 6e61 726f 775a 0565 6d72 6f77 5a07 6172  narowZ.emrowZ.ar
+00001d70: 6561 726f 775a 0472 6f77 315a 0972 6f77  earowZ.row1Z.row
+00001d80: 7365 6c65 6374 720a 0000 0072 0a00 0000  selectr....r....
+00001d90: 720e 0000 0072 3400 0000 0501 0000 7322  r....r4.......s"
+00001da0: 0000 0000 0308 0112 060e 0208 020a 030c  ................
+00001db0: 010c 030a 0210 0118 0108 0108 0114 0108  ................
+00001dc0: 0210 0106 0272 3400 0000 6303 0000 0000  .....r4...c.....
+00001dd0: 0000 0000 0000 0006 0000 0003 0000 0043  ...............C
+00001de0: 0000 0073 3800 0000 7c00 6a00 7d03 7c00  ...s8...|.j.}.|.
+00001df0: a001 a100 7d04 7c00 a002 7c01 a101 7d04  ....}.|...|...}.
+00001e00: 7c04 6a03 7c04 7c02 3c00 7c04 6a01 6401  |.j.|.|.<.|.j.d.
+00001e10: 6402 8d01 a002 7c03 a101 7d05 7c05 5300  d.....|...}.|.S.
+00001e20: 2903 4e54 721a 0000 0029 0472 2e00 0000  ).NTr....).r....
+00001e30: 721f 0000 0072 3100 0000 729b 0000 0029  r....r1...r....)
+00001e40: 0672 3e00 0000 5a07 7072 6a5f 6372 735a  .r>...Z.prj_crsZ
+00001e50: 0861 7265 615f 636f 6cda 0773 7263 5f73  .area_col..src_s
+00001e60: 7263 da04 746f 7374 da03 6f75 7472 0a00  rc..tost..outr..
+00001e70: 0000 720a 0000 0072 0e00 0000 da0e 6164  ..r....r......ad
+00001e80: 645f 6172 6561 5f69 6e5f 6d32 2801 0000  d_area_in_m2(...
+00001e90: 730c 0000 0000 0106 0108 020a 010a 0212  s...............
+00001ea0: 0272 a100 0000 6303 0000 0000 0000 0000  .r....c.........
+00001eb0: 0000 0006 0000 0003 0000 0043 0000 0073  ...........C...s
+00001ec0: 4a00 0000 7c00 6a00 7d03 7c00 a001 a100  J...|.j.}.|.....
+00001ed0: 7d04 7c04 a002 6401 a101 7d04 7c04 6a03  }.|...d...}.|.j.
+00001ee0: 6a04 6a05 7c04 7c02 3c00 7c04 6a03 6a04  j.j.|.|.<.|.j.j.
+00001ef0: 6a06 7c04 7c01 3c00 7c04 6a01 6402 6403  j.|.|.<.|.j.d.d.
+00001f00: 8d01 a002 7c03 a101 7d05 7c05 5300 2904  ....|...}.|.S.).
+00001f10: 4efa 0945 5053 473a 3433 3236 5472 1a00  N..EPSG:4326Tr..
+00001f20: 0000 2907 722e 0000 0072 1f00 0000 7231  ..).r....r....r1
+00001f30: 0000 0072 5300 0000 da08 6365 6e74 726f  ...rS.....centro
+00001f40: 6964 da01 7972 0b00 0000 2906 723e 0000  id..yr....).r>..
+00001f50: 005a 0463 6f6c 785a 0463 6f6c 7972 9e00  .Z.colxZ.colyr..
+00001f60: 0000 729f 0000 0072 a000 0000 720a 0000  ..r....r....r...
+00001f70: 0072 0a00 0000 720e 0000 0072 7100 0000  .r....r....rq...
+00001f80: 3301 0000 730e 0000 0000 0106 0108 020a  3...s...........
+00001f90: 020e 010e 0212 0272 7100 0000 6301 0000  .......rq...c...
+00001fa0: 0000 0000 0000 0000 001c 0000 0008 0000  ................
+00001fb0: 0043 0000 0073 7e03 0000 6401 7c00 7601  .C...s~...d.|.v.
+00001fc0: 720c 6400 5300 7400 6a01 a002 7c00 a101  r.d.S.t.j...|...
+00001fd0: 7d01 7400 6a01 a003 7c00 a101 a004 6402  }.t.j...|.....d.
+00001fe0: a101 7d02 7405 7c02 8301 7d03 7c02 7c03  ..}.t.|...}.|.|.
+00001ff0: 6403 1800 1900 6404 6405 8502 1900 7d04  d.....d.d.....}.
+00002000: 6700 6406 a201 7d05 6401 7d06 6407 7d07  g.d...}.d.}.d.}.
+00002010: 6408 7d08 6409 7d09 6700 7d0a 6700 7d0b  d.}.d.}.g.}.g.}.
+00002020: 640a 7c04 7600 72e8 7c06 6402 1700 7c04  d.|.v.r.|.d...|.
+00002030: 1700 640b 1700 7c07 6402 1700 7c04 1700  ..d...|.d...|...
+00002040: 640b 1700 7c08 6402 1700 7c04 1700 640b  d...|.d...|...d.
+00002050: 1700 7c09 6402 1700 7c04 1700 640b 1700  ..|.d...|...d...
+00002060: 6704 7d0a 7c06 6402 1700 7c04 1700 640c  g.}.|.d...|...d.
+00002070: 1700 7c07 6402 1700 7c04 1700 640c 1700  ..|.d...|...d...
+00002080: 7c08 6402 1700 7c04 1700 640c 1700 7c09  |.d...|...d...|.
+00002090: 6402 1700 7c04 1700 640c 1700 6704 7d0b  d...|...d...g.}.
+000020a0: 6e38 7c06 640b 1700 7c07 640b 1700 7c08  n8|.d...|.d...|.
+000020b0: 640b 1700 7c09 640b 1700 6704 7d0a 7c06  d...|.d...g.}.|.
+000020c0: 640c 1700 7c07 640c 1700 7c08 640c 1700  d...|.d...|.d...
+000020d0: 7c09 640c 1700 6704 7d0b 6700 7d0c 6700  |.d...g.}.g.}.g.
+000020e0: 7d0d 7406 6404 7405 7c0a 8301 8302 4400  }.t.d.t.|.....D.
+000020f0: 9001 5d2e 7d0e 7400 6a01 a007 7c01 7c0a  ..].}.t.j...|.|.
+00002100: 7c0e 1900 a102 7d0f 7400 6a01 a007 7c01  |.....}.t.j...|.
+00002110: 7c0b 7c0e 1900 a102 7d10 7400 6a01 a008  |.|.....}.t.j...
+00002120: 7c0f a101 9001 7372 9001 7136 7c0c a009  |.....sr..q6|...
+00002130: 7c10 a101 0100 6407 7c0a 7c0e 1900 7600  |.....d.|.|...v.
+00002140: 9001 7398 640d 7c0a 7c0e 1900 7600 9001  ..s.d.|.|...v...
+00002150: 72a2 7c0d a009 7c10 a101 0100 740a a00b  r.|...|.....t...
+00002160: 7c0f a101 7d11 7c11 a00c 640e a101 7d12  |...}.|...d...}.
+00002170: 6401 7c0a 7c0e 1900 7600 9001 73d2 6407  d.|.|...v...s.d.
+00002180: 7c0a 7c0e 1900 7600 9002 7214 7c12 640f  |.|...v...r.|.d.
+00002190: 1900 a00d 740e a101 a00d 740f a101 7c12  ....t.....t...|.
+000021a0: 6410 3c00 7c12 6a10 4400 5d22 7d13 6411  d.<.|.j.D.]"}.d.
+000021b0: 7c12 6a11 7c13 6410 6602 1900 1700 7c12  |.j.|.d.f.....|.
+000021c0: 6a11 7c13 6410 6602 3c00 9001 71f0 7c12  j.|.d.f.<...q.|.
+000021d0: 7d14 7c05 4400 5d46 7d15 7c14 a012 7c15  }.|.D.]F}.|...|.
+000021e0: a101 7c14 6412 3c00 7c14 6a13 7c10 6413  ..|.d.<.|.j.|.d.
+000021f0: 6414 8d02 0100 7400 a014 7c10 a101 6a15  d.....t...|...j.
+00002200: 6415 1b00 6415 1b00 7d16 7c16 6416 6b01  d...d...}.|.d.k.
+00002210: 9002 721c 0100 9001 7136 9002 711c 9001  ..r.....q6..q...
+00002220: 7136 7405 7c0d 8301 6403 6b04 9003 727a  q6t.|...d.k...rz
+00002230: 7400 a014 7400 6a01 a007 7c01 7c0b 6404  t...t.j...|.|.d.
+00002240: 1900 a102 a101 6a15 6415 1b00 6415 1b00  ......j.d...d...
+00002250: 6417 6b00 9003 727a 7406 6404 7405 7c0d  d.k...rzt.d.t.|.
+00002260: 8301 8302 4400 5d80 7d0e 7416 7417 7c0d  ....D.].}.t.t.|.
+00002270: 7c0e 1900 8301 8301 7d17 6407 7c0d 7c0e  |.......}.d.|.|.
+00002280: 1900 7600 9003 7206 6700 7d18 7c17 6418  ..v...r.g.}.|.d.
+00002290: 1900 4400 5d22 7d19 7c19 6419 1900 641a  ..D.]"}.|.d...d.
+000022a0: 1900 6404 6b02 9002 72da 7c18 a009 7c19  ..d.k...r.|...|.
+000022b0: a101 0100 9002 71da 7c18 7c17 6418 3c00  ......q.|.|.d.<.
+000022c0: 7c0e 6404 6b02 9003 7216 7c17 7d1a 6e14  |.d.k...r.|.}.n.
+000022d0: 7c1a 6418 0500 1900 7c17 6418 1900 3700  |.d.....|.d...7.
+000022e0: 0300 3c00 9002 71ac 7417 7400 6a01 a007  ..<...q.t.t.j...
+000022f0: 7c01 641b a102 641c 641d 641e 8d03 8f22  |.d...d.d.d...."
+00002300: 7d1b 7418 6a19 7c1a 7c1b 641f 6405 6420  }.t.j.|.|.d.d.d 
+00002310: 8d04 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00002320: 6e12 3100 9003 7370 3000 0100 0100 0100  n.1...sp0.......
+00002330: 5900 0100 6400 5300 2921 4eda 0d66 696e  Y...d.S.)!N..fin
+00002340: 616c 6361 745f 696e 666f da01 5f72 1e00  alcat_info.._r..
+00002350: 0000 7201 0000 00e9 0400 0000 2906 672d  ..r.........).g-
+00002360: 431c ebe2 361a 3f67 fca9 f1d2 4d62 403f  C...6.?g....Mb@?
+00002370: 67fc a9f1 d24d 6250 3f67 7b14 ae47 e17a  g....MbP?g{..G.z
+00002380: 743f 677b 14ae 47e1 7a84 3f67 9a99 9999  t?g{..G.z.?g....
+00002390: 9999 a93f da11 6669 6e61 6c63 6174 5f69  ...?..finalcat_i
+000023a0: 6e66 6f5f 7269 76da 1173 6c5f 636f 6e6e  nfo_riv..sl_conn
+000023b0: 6563 7465 645f 6c61 6b65 da15 736c 5f6e  ected_lake..sl_n
+000023c0: 6f6e 5f63 6f6e 6e65 6374 6564 5f6c 616b  on_connected_lak
+000023d0: 65da 0176 7a04 2e73 6870 7a08 2e67 656f  e..vz..shpz..geo
+000023e0: 6a73 6f6e da0e 636f 6e6e 6563 7465 645f  json..connected_
+000023f0: 6c61 6b65 72a2 0000 0072 4200 0000 da07  laker....rB.....
+00002400: 7276 684e 616d 65da 0373 7562 7253 0000  rvhName..subrS..
+00002410: 00da 0747 656f 4a53 4f4e 2901 da06 6472  ...GeoJSON)...dr
+00002420: 6976 6572 6900 0400 00e9 6400 0000 69f4  iveri.....d...i.
+00002430: 0100 00da 0866 6561 7475 7265 7372 0800  .....featuresr..
+00002440: 0000 725d 0000 007a 2272 6f75 7469 6e67  ..r]...z"routing
+00002450: 5f70 726f 6475 6374 5f6c 616b 655f 7269  _product_lake_ri
+00002460: 7665 722e 6765 6f6a 736f 6eda 0177 7a05  ver.geojson..wz.
+00002470: 7574 662d 3829 01da 0865 6e63 6f64 696e  utf-8)...encodin
+00002480: 6746 2902 da0c 656e 7375 7265 5f61 7363  gF)...ensure_asc
+00002490: 6969 da06 696e 6465 6e74 291a 726a 0000  ii..indent).rj..
+000024a0: 0072 6b00 0000 da07 6469 726e 616d 65da  .rk.....dirname.
+000024b0: 0862 6173 656e 616d 65da 0573 706c 6974  .basename..split
+000024c0: 7220 0000 00da 0572 616e 6765 726c 0000  r .....rangerl..
+000024d0: 00da 0665 7869 7374 7372 2200 0000 722f  ...existsr"...r/
+000024e0: 0000 0072 3000 0000 7231 0000 00da 0661  ...r0...r1.....a
+000024f0: 7374 7970 65da 0369 6e74 da03 7374 7272  stype..int..strr
+00002500: 7700 0000 7274 0000 00da 0873 696d 706c  w...rt.....simpl
+00002510: 6966 7972 7300 0000 da04 7374 6174 da07  ifyrs.....stat..
+00002520: 7374 5f73 697a 6572 0200 0000 7269 0000  st_sizer....ri..
+00002530: 00da 046a 736f 6eda 0464 756d 7029 1cda  ...json..dump)..
+00002540: 1249 6e70 7574 5f50 6f6c 7967 6f6e 5f70  .Input_Polygon_p
+00002550: 6174 68da 0b70 726f 6475 6374 5f64 6972  ath..product_dir
+00002560: da08 4e61 6d65 735f 696e da07 6e5f 6368  ..Names_in..n_ch
+00002570: 6172 63da 0776 6572 7369 6f6e da0a 544f  arc..version..TO
+00002580: 4c45 5241 4e43 4573 da0d 6865 6164 5f6e  LERANCEs..head_n
+00002590: 616d 655f 6361 74da 0d68 6561 645f 6e61  ame_cat..head_na
+000025a0: 6d65 5f72 6976 da0f 6865 6164 5f6e 616d  me_riv..head_nam
+000025b0: 655f 736c 616b 65da 0f68 6561 645f 6e61  e_slake..head_na
+000025c0: 6d65 5f6e 6c61 6b65 da0f 496e 7075 745f  me_nlake..Input_
+000025d0: 6669 6c65 5f6e 616d 65da 104f 7574 7075  file_name..Outpu
+000025e0: 745f 6669 6c65 5f6e 616d 65da 1363 7265  t_file_name..cre
+000025f0: 6174 6564 5f6a 6173 6f6e 5f66 696c 6573  ated_jason_files
+00002600: da1c 6372 6561 7465 645f 6a61 736f 6e5f  ..created_jason_
+00002610: 6669 6c65 735f 6c61 6b65 5f72 6976 7224  files_lake_rivr$
+00002620: 0000 00da 0a69 6e70 7574 5f70 6174 68da  .....input_path.
+00002630: 116f 7574 7075 745f 6a61 736f 6e5f 7061  .output_jason_pa
+00002640: 7468 5a08 696e 7075 745f 7064 da0c 696e  thZ.input_pd..in
+00002650: 7075 745f 7767 735f 3834 da03 6964 78da  put_wgs_84..idx.
+00002660: 0c69 6e70 7574 5f74 6f6a 736f 6eda 0954  .input_tojson..T
+00002670: 4f4c 4552 414e 4345 da0e 6a73 6f6e 5f66  OLERANCE..json_f
+00002680: 696c 655f 7369 7a65 da07 696e 6a73 6f6e  ile_size..injson
+00002690: 32da 0c6e 6577 5f66 6561 7475 7265 73da  2..new_features.
+000026a0: 0765 6c65 6d65 6e74 da15 6f75 7470 7574  .element..output
+000026b0: 5f6a 6173 6f6e 5f6c 616b 655f 7269 7672  _jason_lake_rivr
+000026c0: 7f00 0000 720a 0000 0072 0a00 0000 720e  ....r....r....r.
+000026d0: 0000 0072 7600 0000 4101 0000 7390 0000  ...rv...A...s...
+000026e0: 0000 0208 0204 020c 0112 0108 0114 0108  ................
+000026f0: 0304 0104 0104 0104 0204 0104 0108 020e  ................
+00002700: 010e 010e 010e fc04 070e 010e 010e 010e  ................
+00002710: fc06 0806 0106 0106 0106 fc04 0706 0106  ................
+00002720: 0106 0106 fc04 0604 0104 0214 0112 0112  ................
+00002730: 010e 0104 010a 021c 010a 030a 020a 041c  ................
+00002740: 0118 010a 0120 0304 0208 010e 010e 0214  ..... ..........
+00002750: 010a 010e 0236 0112 0110 010e 0104 010c  .....6..........
+00002760: 0112 010e 0108 020a 0106 0218 021a 0132  ...............2
+00002770: 0272 7600 0000 2902 7226 0000 0072 2600  .rv...).r&...r&.
+00002780: 0000 2901 7242 0000 0029 0172 9500 0000  ..).rB...).r....
+00002790: 291b 722f 0000 00da 056e 756d 7079 728a  ).r/.....numpyr.
+000027a0: 0000 0072 6a00 0000 da06 7061 6e64 6173  ...rj.....pandas
+000027b0: 7213 0000 0072 c200 0000 7202 0000 0072  r....r....r....r
+000027c0: 0300 0000 7267 0000 0072 3700 0000 da05  ....rg...r7.....
+000027d0: 6f73 6765 6f72 0400 0000 7205 0000 005a  osgeor....r....Z
+000027e0: 0b72 6173 7465 7273 7461 7473 7206 0000  .rasterstatsr...
+000027f0: 0072 1900 0000 7225 0000 0072 4100 0000  .r....r%...rA...
+00002800: 7283 0000 0072 7500 0000 7291 0000 0072  r....ru...r....r
+00002810: 9400 0000 7234 0000 0072 a100 0000 7271  ....r4...r....rq
+00002820: 0000 0072 7600 0000 720a 0000 0072 0a00  ...rv...r....r..
+00002830: 0000 720a 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+00002840: 6f64 756c 653e 0100 0000 732a 0000 0008  odule>....s*....
+00002850: 0108 0108 0108 0110 0108 0108 0108 0310  ................
+00002860: 010c 0208 0c08 1c00 ff0a 4b0a 6008 0608  ..........K.`...
+00002870: 1a08 050a 2308 0b08 0e                   ....#....
```

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/qgis.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/qgis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/__pycache__/rarray.cpython-39.pyc` & `basinmaker-3.0.3/basinmaker/func/__pycache__/rarray.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/fgdal.py` & `basinmaker-3.0.3/basinmaker/func/fgdal.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/grassgis.py` & `basinmaker-3.0.3/basinmaker/func/grassgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/pdtable.py` & `basinmaker-3.0.3/basinmaker/func/pdtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,129 @@
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 from basinmaker.utilities.utilities import *
 import numbers
 from joblib import Parallel, delayed
 import tempfile
+pd.options.mode.chained_assignment = None
+
+
+def update_selected_subid_using_sec_downsubid(sec_down_subinfo,upstream_subs,cat_ply,hyshdinfo):
+    is_sec_down_subid_in_selected_subid = False
+    is_subid_of_sec_downsubid_in_selected_subid = False
+    update_downsubids_using_sec_downsubid = False
+    update_topology = False
+    # identify sec_down_subinfo subbains that downsubid is not in the subid list
+    sec_down_subinfo_mostdown = sec_down_subinfo[~sec_down_subinfo['Sec_DowSubId'].isin(sec_down_subinfo['SubId'].values)]
+    sec_down_subid_in_selected_subid = sec_down_subinfo_mostdown['Sec_DowSubId'].isin(upstream_subs).copy(deep=True)
+
+    # check if downsubid in the secondary downsubid list exist in the selected subbasin
+    # if not means the secondary downsubid has no impact on this area
+    # return the input directly
+    sec_down_subinfo_downsub_in_selected = sec_down_subinfo_mostdown[sec_down_subid_in_selected_subid]
+
+    if len(sec_down_subinfo_downsub_in_selected) <= 0:
+        return upstream_subs,cat_ply,update_topology
+
+    # check subid of secondary downsub id that are in the selected subids
+    # is in the selected subid or not
+    # if they all inlucded in the selected subid
+    # means the secondary downsubid has no impact on this area
+    # return the input directly
+    missing_subid_in_sec_table = sec_down_subinfo_downsub_in_selected[~sec_down_subinfo_downsub_in_selected['SubId'].isin(upstream_subs)].copy(deep=True)
+
+    if len(missing_subid_in_sec_table) <= 0:
+        return upstream_subs,cat_ply,update_topology
+
+    # obtain routing topology for secondary table
+    hyshdinfo_sec = sec_down_subinfo[['SubId', 'Sec_DowSubId']].astype("int32").values
+    for subid_sec in missing_subid_in_sec_table['SubId'].values:
+        #obtain subids in the sec_down_subinfo drainage to this  subid_sec
+        upstream_subs_sec = defcat(hyshdinfo_sec, subid_sec)
+        sec_down_subinfoselect = sec_down_subinfo[sec_down_subinfo['SubId'].isin(upstream_subs_sec)]
+        # update the DownSubId in the cat_ply using using Sec_DowSubId for upstream_subs
+        cat_ply = cat_ply.merge(sec_down_subinfoselect,on='SubId',how='left')
+        mask = cat_ply['SubId'].isin(upstream_subs_sec)
+        cat_ply.loc[mask,'DowSubId'] = cat_ply.loc[mask,'Sec_DowSubId'].values
+        # update the routing topology and get the subbasin drainage to this subid_sec
+        hyshdinfo = cat_ply[['SubId', 'DowSubId']].astype("int32").values
+        upstream_subs_new_sub_sec = defcat(hyshdinfo, subid_sec)
+        # add the new subids into the eixisting upstream subids
+        upstream_subs = np.concatenate((upstream_subs, upstream_subs_new_sub_sec), axis=0)
+        cat_ply = cat_ply.drop(columns='Sec_DowSubId')
+    update_topology = True
+    return upstream_subs,cat_ply,update_topology
+
+def return_extracted_subids(cat_ply,mostdownid,mostupstreamid,sec_down_subinfo):
+
+    # flags for sec down subid
+    has_sec_downsub = False
+    update_downsubids_using_sec_downsubid = False
+
+    hyshdinfo = cat_ply[['SubId', 'DowSubId']].astype("int32").values
+    sum_update_topology = 0
+    update_topology = 0
+    ## find all subid control by this subid
+    for i_down in range(0,len(mostdownid)):
+        ### Loop for each downstream id
+        tar_subid = mostdownid[i_down]
+
+        upstream_subs,cat_ply,update_topology = return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply)
+        sum_update_topology = sum_update_topology + update_topology
+        if i_down == 0:
+            selected_subs = upstream_subs
+        else:
+            selected_subs = np.concatenate((selected_subs, upstream_subs), axis=0)
+
+    selected_subs = np.unique(selected_subs)
+
+    ## find all subid control by this subid
+    remove_subs = np.empty(0, dtype=int)
+
+    for i_up in range(0,len(mostupstreamid)):
+        ### Loop for each downstream id
+        tar_subid = mostupstreamid[i_up]
+
+        if tar_subid < 0:
+            continue
+
+        upstream_subs,cat_ply,update_topology = return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply)
+
+        if i_up == 0:
+            remove_subs = upstream_subs
+        else:
+            remove_subs = np.concatenate((remove_subs, upstream_subs), axis=0)
+
+    if len(remove_subs) > 0:
+        remove_subs = np.unique(remove_subs)
+
+        mask = ~np.in1d(selected_subs, remove_subs)
+
+        selected_subs = selected_subs[mask]
+    if sum_update_topology >= 1:
+        update_topology = True
+    else:
+        update_topology = False
+    return selected_subs,cat_ply,update_topology
+
+
+
+
+
+def return_subids_drainage_to_subid(tar_subid,hyshdinfo,sec_down_subinfo,cat_ply):
+
+    ## find all subid control by this subid
+    upstream_subs = defcat(hyshdinfo, tar_subid)
+    update_topology = 0
+    # check if has sencondary down subid
+    if len(sec_down_subinfo) > 0:
+        upstream_subs,cat_ply,update_topology = update_selected_subid_using_sec_downsubid(sec_down_subinfo,upstream_subs,cat_ply,hyshdinfo)
+
+    return upstream_subs,cat_ply,update_topology
 
 def remove_landuse_type_input_based_on_area(landuse_thres,hruinfo,sub_area,Landuse_ID):
 
     if landuse_thres <= 0:
         return hruinfo
     # calculate the landuse area of each landuse group in each subbasin
     subinfo_lu = hruinfo[['SubId',Landuse_ID,'HRU_Area']].copy(deep=True)
@@ -151,15 +266,15 @@
 
 
 def update_non_connected_catchment_info(catinfo):
     routing_info = catinfo[["SubId", "DowSubId"]].astype("float").values
     catinfo_non_connected = catinfo.loc[catinfo["Lake_Cat"] == 2].copy()
 
     catids_nc = catinfo_non_connected["SubId"].copy()
-
+    max_seg_id = catinfo["Seg_ID"].max()
     catinfo.loc[
         catinfo["SubId"].isin(catids_nc), "RivLength"
     ] = 0.0  ## no reiver length since not connected.
 
     for i in range(0, len(catinfo_non_connected)):
         c_subid = catinfo_non_connected["SubId"].values[i]
         d_subid = catinfo_non_connected["DowSubId"].values[i]
@@ -172,28 +287,34 @@
         # Up_cat_info = catinfo.loc[catinfo["SubId"].isin(Upstreamcats)].copy()
         #
         # DA = sum(Up_cat_info["BasArea"].values)
         #
         # catinfo.loc[catinfo["SubId"] == c_subid, "DrainArea"] = DA
 
         if len(d_sub_info) < 1:
+            catinfo.loc[catinfo["SubId"] == c_subid, "Strahler"] = 1
+            catinfo.loc[catinfo["SubId"] == c_subid, "Seg_ID"] = max_seg_id + i + 1
+            catinfo.loc[catinfo["SubId"] == c_subid, "Seg_order"] = 1
             continue
 
         ## add nonconnected lake catchment area to downsubbasin drinage area
         #        if d_sub_info['Lake_Cat'].values[0]  != 2:
         #            catinfo.loc[catinfo['SubId'] == d_subid,'DA'] = d_sub_info['DA'].values[0] + DA
 
         while d_sub_info["Lake_Cat"].values[0] == 2:
-
             lc_subid_info = catinfo.loc[catinfo["SubId"] == lc_subid].copy()
             d_subid = lc_subid_info["DowSubId"].values[0]
             d_sub_info = catinfo.loc[catinfo["SubId"] == d_subid].copy()
             if len(d_sub_info) < 1:
                 lc_subid = -1
                 break
+            if lc_subid == d_sub_info['DowSubId'].values[0]:
+                print(lc_subid,d_subid)
+                lc_subid = -1
+                break
             lc_subid = d_subid
 
         if lc_subid == -1:
             continue
 
         catinfo.loc[catinfo["SubId"] == c_subid, "RivSlope"] = -1.2345
         catinfo.loc[catinfo["SubId"] == c_subid, "Ch_n"] = -1.2345
@@ -315,24 +436,26 @@
     Longestpath = max(longest_flow_pathes)
 
     return Longestpath
 
 def remove_possible_small_subbasins(mapoldnew_info, area_thresthold = 1):
     mapoldnew_info_new = mapoldnew_info.copy(deep=True)
 
-    # get small subbasin that is not lake
-    small_sub_non_lake = mapoldnew_info[mapoldnew_info['BasArea']/1000/1000 < area_thresthold].copy(deep=True)
-    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake['Lake_Cat'] == 0].copy(deep=True)
-    small_sub_non_lake_subid =small_sub_non_lake['SubId'].values
-
     # check the gauge column name, in case it is v2.1 using Has_Gauge
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in mapoldnew_info.columns:
         Gauge_col_Name = "Has_Gauge"
 
+    # get small subbasin that is not lake
+    small_sub_non_lake = mapoldnew_info[mapoldnew_info['BasArea']/1000/1000 < area_thresthold].copy(deep=True)
+    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake['Lake_Cat'] == 0].copy(deep=True)
+    small_sub_non_lake = small_sub_non_lake[small_sub_non_lake[Gauge_col_Name] == 0].copy(deep=True)
+
+    small_sub_non_lake_subid =small_sub_non_lake['SubId'].values
+
     ### process connected lakes  merge polygons
     for i in range(0, len(small_sub_non_lake)):
         small_sub_id = small_sub_non_lake['SubId'].values[i]
         small_downsub_id = small_sub_non_lake['DowSubId'].values[i]
         small_sub_seg_id = small_sub_non_lake['Seg_ID'].values[i]
 
         small_sub_is_head_water_sub = len(mapoldnew_info[mapoldnew_info['DowSubId'] == small_sub_id]) == 0
@@ -356,15 +479,15 @@
             has_down_sub = False
             down_sub_has_same_seg_id = False
 
         # check if it has the same segment id with upstream subbasin
         if len(upstream_sub_info) > 0:
             has_upstream = True
 
-            if len(upstream_sub_info_same_seg) > 0:
+            if len(upstream_sub_info_same_seg) > 0 and upstream_sub_info_same_seg[Gauge_col_Name].values[0] == 0:
                 up_sub_has_same_seg_id = True
             else:
                 up_sub_has_same_seg_id = False
 
         else:
             has_upstream = False
             up_sub_has_same_seg_id = False
@@ -725,35 +848,29 @@
     -------
         catinfoall
     """
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in catinfoall.columns:
         Gauge_col_Name = "Has_Gauge"
 
-    catinfo = catinfoall.loc[
-        catinfoall["Lake_Cat"] != 2
-    ].copy()  ### remove none connected lake catchments, which do not connected to the river system
+    catinfo = catinfoall.loc[catinfoall["Lake_Cat"] != 2].copy()  ### remove none connected lake catchments, which do not connected to the river system
     catinfo_ncl = catinfoall.loc[catinfoall["Lake_Cat"] == 2].copy()
     routing_ncl = catinfo_ncl[["SubId", "DowSubId"]].astype("float").values
 
     catlist = np.full((len(catinfo)), -9)
     icat = 0
     iseg = 1
     ### find first segments of all reaches, no upstream reaches
     for i in range(0, len(catinfo)):
         idx = catinfo.index[i]
         if catinfo["SubId"].values[i] == catinfo["DowSubId"].values[i]:
             catinfo.loc[idx, "DowSubId"] = -1
         catid = catinfo["SubId"].values[i]
-        if (
-            len(catinfo[catinfo["DowSubId"] == catid]) == 0
-        ):  ### the river seg has no upstream segment
-            catlist[icat] = int(
-                catinfo["DowSubId"].values[i]
-            )  #### store next reach segment
+        if (len(catinfo[catinfo["DowSubId"] == catid]) == 0):  ### the river seg has no upstream segment
+            catlist[icat] = int(catinfo["DowSubId"].values[i])  #### store next reach segment
 
             #### calculate DA of head watershed include None connected lakes
             if len(routing_ncl) == 0:
                 DA_ncl = 0.0
                 slp_ncl = 0.0
             else:
                 Upstreamcats = defcat(routing_ncl, catid)  ### alll subuds
@@ -849,18 +966,19 @@
                     Up_Reaches_info["Seg_order"].values[0] + 1
                 )
 
 
                 catinfo.loc[curcat_idx, "Seg_ID"] = Up_Reaches_info["Seg_ID"].values[0]
 
                 if "DA_Chn_L" in catinfo.columns:
-                    catinfo.loc[curcat_idx, "DA_Chn_L"] = np.max(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
+                    catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
 
-                    catinfo.loc[curcat_idx, "DA_Chn_Slp"] = (cur_Reach_info["RivSlope"].values[0] * np.max(Up_Reaches_info["DA_Chn_L"].values[0],0)
-                                                           + Up_Reaches_info["DA_Chn_L"].values[0]*Up_Reaches_info["DA_Chn_Slp"].values[0])/catinfo.loc[curcat_idx, "DA_Chn_L"]
+                    catinfo.loc[curcat_idx, "DA_Chn_Slp"] = ( cur_Reach_info["RivSlope"].values[0]  * np.maximum(cur_Reach_info["RivLength"].values[0],0)
+                                                           +  Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(Up_Reaches_info["DA_Chn_Slp"].values[0],0)
+                                                             ) / catinfo.loc[curcat_idx, "DA_Chn_L"]
 
                     catinfo.loc[curcat_idx, "DA_Slope"] = (cur_Reach_info["BasSlope"].values[0]*cur_Reach_info["BasArea"].values[0]
                                                            + DA_ncl * slp_ncl
                                                            + Up_Reaches_info["DA_Slope"].values[0] * Up_Reaches_info["DrainArea"].values[0]
                                                            )/catinfo.loc[curcat_idx, "DrainArea"]
 
 
@@ -872,32 +990,32 @@
                 # catinfo.loc[curcat_idx, "Tc_4"] = TC_4
                 # catinfo.loc[curcat_idx, "Tc_5"] = TC_5
 
 
                 #                print('1',catid,catinfo.loc[curcat_idx,'DA'].values,catinfo.loc[curcat_idx,'Strahler'].values,catinfo.loc[curcat_idx,'Sub_order'].values)
                 catid = int(cur_Reach_info["DowSubId"].values[0])
             else:  ### has mutiple upstram
-                if (
-                    np.min(Up_Reaches_info["Strahler"].values) > 0
-                ):  ### all upstream has been processed
+                if (np.min(Up_Reaches_info["Strahler"].values) > 0):  ### all upstream has been processed
 
                     if 'DA_Chn_L' in Up_Reaches_info.columns:
                         Up_Reaches_info = Up_Reaches_info.sort_values(by='DA_Chn_L', ascending=False)
 
                     catinfo.loc[curcat_idx, "DrainArea"] = (
                         cur_Reach_info["BasArea"].values[0]
                         + np.sum(Up_Reaches_info["DrainArea"].values)
                         + DA_ncl
                     )
 
                     if "DA_Chn_L" in catinfo.columns:
-                        catinfo.loc[curcat_idx, "DA_Chn_L"] = np.max(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
+                        catinfo.loc[curcat_idx, "DA_Chn_L"] = np.maximum(Up_Reaches_info["DA_Chn_L"].values[0],0) + cur_Reach_info["RivLength"].values[0]
+
+                        catinfo.loc[curcat_idx, "DA_Chn_Slp"] = ( cur_Reach_info["RivSlope"].values[0]  * np.maximum(cur_Reach_info["RivLength"].values[0],0)
+                                                               +  Up_Reaches_info["DA_Chn_L"].values[0] * np.maximum(Up_Reaches_info["DA_Chn_Slp"].values[0],0)
+                                                                 ) /catinfo.loc[curcat_idx, "DA_Chn_L"]
 
-                        catinfo.loc[curcat_idx, "DA_Chn_Slp"] = (cur_Reach_info["RivSlope"].values[0] * np.max(Up_Reaches_info["DA_Chn_L"].values[0],0)
-                                                               + Up_Reaches_info["DA_Chn_L"].values[0]*Up_Reaches_info["DA_Chn_Slp"].values[0])/catinfo.loc[curcat_idx, "DA_Chn_L"]
 
                         catinfo.loc[curcat_idx, "DA_Slope"] = (cur_Reach_info["BasSlope"].values[0]*cur_Reach_info["BasArea"].values[0]
                                                                + DA_ncl * slp_ncl
                                                                + Up_Reaches_info["DA_Slope"].values[0] * Up_Reaches_info["DrainArea"].values[0]
                                                                )/catinfo.loc[curcat_idx, "DrainArea"]
 
 
@@ -1159,16 +1277,14 @@
 
     Returns:
     -------
     AllCatinfo           : dataframe
         Downstream DA and strahler order of each subregion along the flow
         pathway between subregions will be updated.
     """
-    min_manning_n = 0.01
-    max_manning_n = 0.15
     ### start from head subregions with no upstream subregion
     Subregion_list = Sub_Region_info[Sub_Region_info["N_Up_SubRegion"] == 1][
         "Sub_Reg_ID"
     ].values
     Subregion_list = np.unique(Subregion_list)
     Subregion_list = Subregion_list.tolist()
 
@@ -1990,40 +2106,40 @@
                 # if not havve the same attribute with upstream lake
                 con_lake_up = i_seg_info["HyLakeId"].values[iorder - 1] != i_seg_info["HyLakeId"].values[iorder]
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] <= 0
 
-                con_area_lake = i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                con_area_lake = False #i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
 
             if iorder == 0 and iorder < len(i_seg_info) - 1:
                 # if not havve the same attribute with upstream lake
                 con_lake_up = True
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] <= 0
 
-                con_area_lake = i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
+                con_area_lake = False #i_seg_info["BasArea"].values[iorder] < 10 * 1000 * 1000
 
             if iorder == len(i_seg_info) - 2 and i_seg_info["HyLakeId"].values[iorder] > 0:
                 # if not havve the same attribute with upstream lake
                 con_lake_up = True
                 # if not havve the same attribute with down lake
                 con_lake_down = i_seg_info["HyLakeId"].values[iorder] != i_seg_info["HyLakeId"].values[iorder + 1]
                 # if this is not a lake subbasin
                 is_lake = i_seg_info["HyLakeId"].values[iorder] > 0
 
                 # if tsubid == 9023607:
                 #     print(con_lake_up,con_lake_down,is_lake,iorder,len(i_seg_info) - 2,i_seg_info["HyLakeId"].values[iorder] > 0)
                 # change add lake to downstream info
                 downsubid = i_seg_info["DowSubId"].values[iorder]
 
-                con_area_lake = i_seg_info["BasArea"].values[iorder +1] < 10 * 1000 * 1000
+                con_area_lake = False #i_seg_info["BasArea"].values[iorder +1] < 10 * 1000 * 1000
 
                 if con_area_lake and con_lake_down:
                     finalriv_info.loc[
                         finalriv_info["SubId"] == downsubid,'HyLakeId'] = i_seg_info["HyLakeId"].values[iorder]
                     finalriv_info.loc[
                         finalriv_info["SubId"] == downsubid,'Lake_Cat'] = i_seg_info["Lake_Cat"].values[iorder]
                     finalriv_info.loc[
@@ -2187,27 +2303,37 @@
     finalcat_info["LakeArea"] = finalcat_info["LakeArea"].astype(float)
     finalcat_info["HyLakeId"] = finalcat_info["HyLakeId"].astype(int)
     finalcat_info["Seg_ID"] = finalcat_info["Seg_ID"].astype(int)
 
     Non_ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 2].copy(deep=True)
     ConnL_info = finalcat_info.loc[finalcat_info["Lake_Cat"] == 1].copy(deep=True)
 
+    if "Has_POI" in finalcat_info.columns:
+        Gauge_col_Name = "Has_POI"
+    else:
+        Gauge_col_Name = "Has_Gauge"
     # first obtain selected lakes based on lake area
     ### process connected lakes first
+    mask1 = ConnL_info["LakeArea"] >= Thres_Area_Conn_Lakes
+    mask2 = ConnL_info[Gauge_col_Name] == 1
+    mask = np.logical_or(mask1,mask2)
     Selected_ConnLakes = ConnL_info.loc[
-       (ConnL_info["LakeArea"] >= Thres_Area_Conn_Lakes)
+       mask
     ]["HyLakeId"].values
 
     Selected_ConnLakes = Selected_ConnLakes[Selected_ConnLakes > 0]
     Selected_ConnLakes = np.unique(Selected_ConnLakes)
 
 
+    mask1 = Non_ConnL_info["LakeArea"] >= Thres_Area_Non_Conn_Lakes
+    mask2 = Non_ConnL_info[Gauge_col_Name] == 1
+    mask = np.logical_or(mask1,mask2)
     ### process non connected selected lakes
     Selected_Non_ConnLakes = Non_ConnL_info[
-        (Non_ConnL_info["LakeArea"] >= Thres_Area_Non_Conn_Lakes)
+        mask
     ]["HyLakeId"].values
     Selected_Non_ConnLakes = Selected_Non_ConnLakes[Selected_Non_ConnLakes > 0]
     Selected_Non_ConnLakes = np.unique(Selected_Non_ConnLakes)
 
 
     # selecte lake by list
     if len(Selected_Lake_List_in) > 0:
@@ -2552,14 +2678,16 @@
     # assign acc for each row
     str_id_unique = np.unique(np.array(riv_lake[:, 1]))
     cl_id_unique = np.unique(np.array(riv_lake[:, 3]))
 
     acc_str_cl = np.full((len(riv_lake), 1), np.nan)
     for i in range(0, len(str_id_unique)):
         strid = str_id_unique[i]
+        # print(strid)
+        # print(routing_info.loc[routing_info["SubId"] == strid])
         maxacc = routing_info.loc[routing_info["SubId"] == strid]["MaxAcc_cat"].values[
             0
         ]
         acc_str_cl[riv_lake[:, 1] == strid] = maxacc
     riv_lake = np.append(riv_lake, acc_str_cl, axis=1)
 
     ## loop for each lake, identify, outlet seg, and inlet segs
```

### Comparing `basinmaker-3.0.1/basinmaker/func/purepy.py` & `basinmaker-3.0.3/basinmaker/func/purepy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,412 +1,421 @@
-import geopandas
-import numpy as np
-import os
-import pandas as pd
-from json import load, JSONEncoder
-import json
-import requests
-import sys
-#import shapely.wkt
-#import pygeos as pg
-from osgeo import gdal, ogr
-from rasterstats import zonal_stats
-
-def zonal_stats_pd(shp_gpd,raster,stats,key):
-
-    result = zonal_stats(shp_gpd, raster, stats = stats,geojson_out=True,all_touched=True)
-
-    reault_list_dic = list(map(lambda x : {key:x['properties'][key],'mean':x['properties']['mean']}, result))
-
-    reault_pd = pd.DataFrame(reault_list_dic)
-
-    return reault_pd
-
-
-
-def ZonalStats(shp_gpd, raster, stats,key,col):
-    # shape - shapefile path
-    # raster - raster path
-    # stats - stats as list, f.e. 'min mean max' ; 'min'
-    # the result is final_gdf as GeoDataFrame
-
-    nodata_pd = shp_gpd.copy(deep=True)
-    i = 0
-    while len(nodata_pd) >0 and i <=5:
-        temp_pd = zonal_stats_pd(nodata_pd,raster,stats,key)
-        bad_hru_values = temp_pd[~(temp_pd['mean'] > 0)]['HRU_ID_New']
-        nodata_pd = nodata_pd[nodata_pd['HRU_ID_New'].isin(bad_hru_values)].copy(deep=True)
-        if i == 0:
-            reault_pd = temp_pd[temp_pd['mean'] > 0]
-            i = i + 1
-        else:
-            i = i + 1
-            good_pd = temp_pd[temp_pd['mean'] > 0]
-            reault_pd = reault_pd.append(good_pd)
-
-    if len(nodata_pd) > 0:
-        nodata_pd['mean'] = nodata_pd[col]
-        reault_pd = reault_pd.append(nodata_pd)
-#    print(len(shp_gpd),len(nodata_pd),len(reault_pd))
-    return reault_pd
-
-
-def Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-    layer_path, Class_Col, tempfolder,mask_layer,Class_NM_Col = '#',info_table = '#'
-):
-    """Preprocess user provided polygons
-
-    Function that will reproject clip input polygon with subbasin polygon
-    and will dissolve the input polygon based on their ID, such as landuse id
-    or soil id.
-
-    Parameters
-    ----------
-    processing                        : qgis object
-    context                           : qgis object
-    layer_path                        : string
-        The path to a specific polygon, for example path to landuse layer
-    Project_crs                       : string
-        the EPSG code of a projected coodinate system that will be used to
-        calcuate HRU area and slope.
-    trg_crs                           : string
-        the EPSG code of a  coodinate system that will be used to
-        calcuate reproject input polygon
-    Class_Col                         : string
-        the column name in the input polygon (layer_path) that contains
-        their ID, for example land use ID or soil ID.
-    Layer_clip                        : qgis object
-        A shpfile with extent of the watershed, will be used to clip input
-        input polygon
-    Notes
-    -------
-        # TODO: May be add some function to simplify the input polygons
-                for example, remove the landuse type with small areas
-                or merge small landuse polygon into the surrounding polygon
-
-    Returns:
-    -------
-        layer_dis                  : qgis object
-            it is a polygon after preprocess
-    """
-
-    new_crs = mask_layer.crs
-    data = geopandas.read_file(layer_path)
-
-    projected = data.to_crs(new_crs)
-    projected = projected.explode(ignore_index=True)
-    clipped = projected.clip(mask_layer)
-#    dissolved = clipped.dissolve(by=[Class_Col], aggfunc='first',as_index=False)
-#    print(Class_Col,new_crs,clipped.crs)
-    cleaned = clean_geometry_purepy(clipped,1)
-    if Class_NM_Col != '#':
-        if Class_Col not in clipped.columns:
-            print(Class_Col," not in the attribute table of provided shapefile")
-            sys.exit()
-        if Class_Col not in info_table.columns:
-            print(Class_Col," not in the attribute table of provided info table")
-            sys.exit()
-        if Class_NM_Col not in info_table.columns:
-            print(Class_NM_Col," not in the attribute table of provided info table")
-            sys.exit()
-
-        info_table_copy = info_table.copy(deep=True)
-        info_table_copy = info_table_copy.drop_duplicates(subset=[Class_NM_Col], keep='last',ignore_index=True)
-        info_table_copy['New_ID'] = info_table_copy[Class_Col]
-        info_table_copy = info_table_copy[[Class_NM_Col,'New_ID']]
-        info_table_copy2 = pd.merge(info_table, info_table_copy, how='inner', on = Class_NM_Col).copy(deep=True)
-
-        cleaned = pd.merge(cleaned, info_table_copy2, how='inner', on = Class_Col)
-        cleaned[Class_Col] = cleaned['New_ID']
-        #update
-    #    clipped Class_Col based on the Class_NM_Col
-    #    arcpy.RepairGeometry_management(os.path.join(tempfolder,Class_Col+"_dislve.shp"))
-
-    #    arcpy.AddSpatialIndex_management(os.path.join(tempfolder,Class_Col+"_dislve.shp"))
-    return cleaned
-
-
-def save_modified_attributes_to_outputs(mapoldnew_info,tempfolder,OutputFolder,cat_name,riv_name,Path_final_riv,dis_col_name='SubId'):
-
-
-    NEED_TO_REMOVE_IDS = ["SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_SubId","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId","SubIdt2"]
-
-    #obtain readme file
-    if "DA_Chn_L" in  mapoldnew_info.columns:
-        url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_OIH.pdf'
-    else:
-        url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_NA.pdf'
-
-    response = requests.get(url)
-    with open(os.path.join(OutputFolder,"README.pdf"), 'wb') as f:
-        f.write(response.content)
-
-    if riv_name != '#':
-
-        if Path_final_riv != '#':
-            riv_pd = geopandas.read_file(Path_final_riv)
-            riv_pd['Old_SubId'] = riv_pd['SubId']
-
-        cat_pd = mapoldnew_info.drop(columns = 'geometry').copy(deep=True)
-        # remove all columns
-        if Path_final_riv != '#':
-            riv_pd = riv_pd[['geometry','Old_SubId']]
-            riv_pd = pd.merge(riv_pd, cat_pd, on='Old_SubId', how='left')
-            riv_pd = riv_pd.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
-
-
-        mapoldnew_info = mapoldnew_info.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
-        mapoldnew_info = add_centroid_in_wgs84(mapoldnew_info,"centroid_x","centroid_y")
-
-        cat_c_x_y = mapoldnew_info[["centroid_y","centroid_x"]].copy(deep=True)
-        if Path_final_riv != '#':
-            riv_pd = riv_pd.drop(columns = ["centroid_y","centroid_x"])
-            riv_pd = riv_pd.join(cat_c_x_y)
-
-        riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2][['SubId','DowSubId']].copy(deep=True)
-        remove_channel = []
-        for subid in riv_pd_nncls_routing_info['SubId'].values:
-            if subid not in riv_pd_nncls_routing_info['DowSubId'].values:
-                remove_channel.append(subid)
-        if Path_final_riv != '#':
-            riv_pd = riv_pd[~riv_pd.SubId.isin(remove_channel)]
-            cat_colnms = riv_pd.columns
-            drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
-            riv_pd = riv_pd.drop(columns=drop_cat_colnms)
-            if len(riv_pd) > 0:
-                riv_pd.to_file(os.path.join(OutputFolder,riv_name))
-
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
-        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
-
-        cat_colnms = mapoldnew_info.columns
-        drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
-        mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
-        mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
-
-        create_geo_jason_file(os.path.join(OutputFolder,cat_name))
-
-    else:
-
-        mapoldnew_info = mapoldnew_info.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
-
-        if "centroid_y" in mapoldnew_info.columns:
-
-            mapoldnew_info = add_centroid_in_wgs84(mapoldnew_info,"centroid_x","centroid_y")
-            mapoldnew_info["SubId"] = mapoldnew_info.index
-            riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2][['SubId','DowSubId']].copy(deep=True)
-            remove_channel = []
-            for subid in riv_pd_nncls_routing_info['SubId'].values:
-                if subid not in riv_pd_nncls_routing_info['DowSubId'].values:
-                    remove_channel.append(subid)
-
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
-            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
-
-
-        cat_colnms = mapoldnew_info.columns
-        drop_cat_colnms = cat_colnms[cat_colnms.isin(["SHAPE","SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId"])]
-        mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
-        mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
-        return mapoldnew_info
-
-
-def Remove_Unselected_Lake_Attribute_In_Finalcatinfo_purepy(finalcat_ply, Conn_Lake_Ids):
-    """Functions will set lake id not in Conn_Lake_Ids to -1.2345 in attribute
-        table of Path_Finalcatinfo
-    ----------
-
-    Notes
-    -------
-
-    Returns:
-    -------
-        None, the attribute table of Path_shpfile will be updated
-    """
-
-    mask1 = np.logical_not(finalcat_ply['HyLakeId'].isin(Conn_Lake_Ids))
-    mask2 = finalcat_ply['Lake_Cat'] != 2
-    mask = np.logical_and(mask1,mask2)
-
-    finalcat_ply.loc[mask,'HyLakeId'] = 0
-    finalcat_ply.loc[mask,'LakeVol'] = 0
-    finalcat_ply.loc[mask,'LakeArea'] = 0
-    finalcat_ply.loc[mask,'LakeDepth'] = 0
-    finalcat_ply.loc[mask,'Laketype'] =0
-    finalcat_ply.loc[mask,'Lake_Cat'] = 0
-
-    return finalcat_ply
-
-def clean_attribute_name_purepy(table,names):
-    remove_column_names = table.columns[np.logical_not(np.isin(table.columns,names))]
-    table = table.drop(columns=remove_column_names)
-    return table
-
-def clean_geometry_purepy(data,set_precision = -1):
-
-#    data["geometry"] = data["geometry"].apply(lambda x: shapely.wkt.loads(shapely.wkt.dumps(x, rounding_precision=4)))
-    if set_precision > 0:
-        data['geometry'] = data['geometry'].buffer(0.00000000001)
-
-#        data.geometry = pg.set_precision(data.geometry.values.data, 1e-6)
-#        data["geometry"] = data["geometry"].apply(lambda x: shapely.wkt.loads(shapely.wkt.dumps(x, rounding_precision=4)))
-#        data['geometry'] = data['geometry'].buffer(0)
-#    print("aaaa")
-    narow = ~data['geometry'].isna()
-#    print("a1",len(data.loc[narow]))
-    emrow = ~data.is_empty
-#    print("a2",len(data.loc[emrow]))
-    arearow = data.area > 0
-#    print("a3",len(data.loc[arearow]))
-#    arevalid = data.is_valid
-    row1 = np.logical_and(narow,emrow)
-    rowselect = np.logical_and(arearow,row1)
-#    print("a",len(data))
-#    rowselect = np.logical_and(rowselect,arevalid)
-    data = data.loc[rowselect]
-#    print("b",len(data))
-    data = data.loc[data.geom_type != 'Point']
-    if len(data.loc[data.geom_type == 'GeometryCollection']) > 0:
-        print("###########################")
-        print("check the following features")
-        print(data.loc[data.geom_type == 'GeometryCollection'])
-        print("###########################")
-
-    data = data.loc[data.geom_type != 'GeometryCollection']
-    data.sindex
-#    print("c",len(data))
-    return data
-
-def add_area_in_m2(data,prj_crs,area_col):
-    src_src = data.crs
-    tost = data.copy()
-
-    tost= data.to_crs(prj_crs)
-    tost[area_col] = tost.area
-
-    out= tost.copy(deep=True).to_crs(src_src)
-
-    return out
-
-def add_centroid_in_wgs84(data,colx,coly):
-    src_src = data.crs
-    tost = data.copy()
-
-    tost= tost.to_crs('EPSG:4326')
-
-    tost[coly] = tost.geometry.centroid.y
-    tost[colx] = tost.geometry.centroid.x
-
-    out= tost.copy(deep=True).to_crs(src_src)
-
-    return out
-
-
-def create_geo_jason_file(Input_Polygon_path):
-
-    if "finalcat_info" not in Input_Polygon_path:
-#        print(Input_Polygon_path)
-        return
-
-    product_dir = os.path.dirname(Input_Polygon_path)
-    Names_in = os.path.basename(Input_Polygon_path).split('_')
-    n_charc = len(Names_in)
-    version  = Names_in[n_charc - 1][0:4]
-    TOLERANCEs = [0.0001,0.0005,0.001,0.005,0.01,0.05]
-
-
-    head_name_cat = "finalcat_info"
-    head_name_riv = "finalcat_info_riv"
-    head_name_slake = "sl_connected_lake"
-    head_name_nlake = "sl_non_connected_lake"
-
-    Input_file_name = []
-    Output_file_name = []
-    if 'v' in version:
-        Input_file_name = [
-                           head_name_cat + "_"+version+'.shp',
-                           head_name_riv + "_"+version+'.shp',
-                           head_name_slake + "_"+version+'.shp',
-                           head_name_nlake + "_"+version+'.shp',
-                           ]
-        Output_file_name = [
-                           head_name_cat + "_"+version+'.geojson',
-                           head_name_riv + "_"+version+'.geojson',
-                           head_name_slake + "_"+version+'.geojson',
-                           head_name_nlake + "_"+version+'.geojson',
-                           ]
-    else:
-        Input_file_name = [
-                           head_name_cat +'.shp',
-                           head_name_riv +'.shp',
-                           head_name_slake +'.shp',
-                           head_name_nlake +'.shp',
-                           ]
-        Output_file_name = [
-                           head_name_cat +'.geojson',
-                           head_name_riv +'.geojson',
-                           head_name_slake +'.geojson',
-                           head_name_nlake +'.geojson',
-                           ]
-    created_jason_files = []
-    created_jason_files_lake_riv = []
-
-    for i  in  range(0,len(Input_file_name)):
-        input_path = os.path.join(product_dir,Input_file_name[i])
-        output_jason_path = os.path.join(product_dir,Output_file_name[i])
-        if not os.path.exists(input_path):
-            continue
-        created_jason_files.append(output_jason_path)
-
-        if 'finalcat_info_riv' in Input_file_name[i] or 'connected_lake' in Input_file_name[i]:
-            created_jason_files_lake_riv.append(output_jason_path)
-
-        # reproject to WGS84
-        input_pd = geopandas.read_file(input_path)
-
-        input_wgs_84 = input_pd.to_crs('EPSG:4326')
-
-
-
-        if 'finalcat_info' in Input_file_name[i] or "finalcat_info_riv" in Input_file_name[i]:
-            input_wgs_84['rvhName'] = input_wgs_84['SubId'].astype(int).astype(str)
-            for idx in input_wgs_84.index:
-                input_wgs_84.loc[idx,'rvhName'] = 'sub' + input_wgs_84.loc[idx,'rvhName']
-
-
-        input_tojson = input_wgs_84
-
-        for TOLERANCE in TOLERANCEs:
-            input_tojson['geometry'] = input_tojson.simplify(TOLERANCE)
-            input_tojson.to_file(output_jason_path, driver="GeoJSON")
-
-            json_file_size = os.stat(output_jason_path).st_size/1024/1024 #to MB
-            if json_file_size <= 100:
-                break
-
-    if len(created_jason_files_lake_riv) > 1 and os.stat(os.path.join(product_dir,Output_file_name[0])).st_size/1024/1024 < 500:
-        for i in range(0,len(created_jason_files_lake_riv)):
-            injson2 = load(open(created_jason_files_lake_riv[i]))
-            if 'finalcat_info_riv' in created_jason_files_lake_riv[i]:
-                new_features = []
-                for element in injson2["features"]:
-                    if element["properties"]["Lake_Cat"] == 0:
-                        new_features.append(element)
-                injson2["features"] = new_features
-
-            if i == 0:
-                output_jason_lake_riv = injson2
-            else:
-                output_jason_lake_riv['features'] += injson2['features']
-
-        with open(os.path.join(product_dir,'routing_product_lake_river.geojson'), 'w', encoding='utf-8') as f:
-            json.dump(output_jason_lake_riv, f, ensure_ascii=False, indent=4)
-
-    return
+import geopandas
+import numpy as np
+import os
+import pandas as pd
+from json import load, JSONEncoder
+import json
+import requests
+import sys
+#import shapely.wkt
+#import pygeos as pg
+from osgeo import gdal, ogr
+from rasterstats import zonal_stats
+
+def zonal_stats_pd(shp_gpd,raster,stats,key):
+
+    result = zonal_stats(shp_gpd, raster, stats = stats,geojson_out=True,all_touched=True)
+
+    reault_list_dic = list(map(lambda x : {key:x['properties'][key],'mean':x['properties']['mean']}, result))
+
+    reault_pd = pd.DataFrame(reault_list_dic)
+
+    return reault_pd
+
+
+
+def ZonalStats(shp_gpd, raster, stats,key,col):
+    # shape - shapefile path
+    # raster - raster path
+    # stats - stats as list, f.e. 'min mean max' ; 'min'
+    # the result is final_gdf as GeoDataFrame
+
+    nodata_pd = shp_gpd.copy(deep=True)
+    i = 0
+    while len(nodata_pd) >0 and i <=5:
+        temp_pd = zonal_stats_pd(nodata_pd,raster,stats,key)
+        bad_hru_values = temp_pd[~(temp_pd['mean'] > 0)]['HRU_ID_New']
+        nodata_pd = nodata_pd[nodata_pd['HRU_ID_New'].isin(bad_hru_values)].copy(deep=True)
+        if i == 0:
+            reault_pd = temp_pd[temp_pd['mean'] > 0]
+            i = i + 1
+        else:
+            i = i + 1
+            good_pd = temp_pd[temp_pd['mean'] > 0]
+            reault_pd = reault_pd.append(good_pd)
+
+    if len(nodata_pd) > 0:
+        nodata_pd['mean'] = nodata_pd[col]
+        reault_pd = reault_pd.append(nodata_pd)
+#    print(len(shp_gpd),len(nodata_pd),len(reault_pd))
+    return reault_pd
+
+
+def Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+    layer_path, Class_Col, tempfolder,mask_layer,Class_NM_Col = '#',info_table = '#'
+):
+    """Preprocess user provided polygons
+
+    Function that will reproject clip input polygon with subbasin polygon
+    and will dissolve the input polygon based on their ID, such as landuse id
+    or soil id.
+
+    Parameters
+    ----------
+    processing                        : qgis object
+    context                           : qgis object
+    layer_path                        : string
+        The path to a specific polygon, for example path to landuse layer
+    Project_crs                       : string
+        the EPSG code of a projected coodinate system that will be used to
+        calcuate HRU area and slope.
+    trg_crs                           : string
+        the EPSG code of a  coodinate system that will be used to
+        calcuate reproject input polygon
+    Class_Col                         : string
+        the column name in the input polygon (layer_path) that contains
+        their ID, for example land use ID or soil ID.
+    Layer_clip                        : qgis object
+        A shpfile with extent of the watershed, will be used to clip input
+        input polygon
+    Notes
+    -------
+        # TODO: May be add some function to simplify the input polygons
+                for example, remove the landuse type with small areas
+                or merge small landuse polygon into the surrounding polygon
+
+    Returns:
+    -------
+        layer_dis                  : qgis object
+            it is a polygon after preprocess
+    """
+
+    new_crs = mask_layer.crs
+    data = geopandas.read_file(layer_path)
+
+    projected = data.to_crs(new_crs)
+    projected = projected.explode(ignore_index=True)
+    clipped = projected.clip(mask_layer)
+#    dissolved = clipped.dissolve(by=[Class_Col], aggfunc='first',as_index=False)
+#    print(Class_Col,new_crs,clipped.crs)
+    cleaned = clean_geometry_purepy(clipped,1)
+    if Class_NM_Col != '#':
+        if Class_Col not in clipped.columns:
+            print(Class_Col," not in the attribute table of provided shapefile")
+            sys.exit()
+        if Class_Col not in info_table.columns:
+            print(Class_Col," not in the attribute table of provided info table")
+            sys.exit()
+        if Class_NM_Col not in info_table.columns:
+            print(Class_NM_Col," not in the attribute table of provided info table")
+            sys.exit()
+
+        info_table_copy = info_table.copy(deep=True)
+        info_table_copy = info_table_copy.drop_duplicates(subset=[Class_NM_Col], keep='last',ignore_index=True)
+        info_table_copy['New_ID'] = info_table_copy[Class_Col]
+        info_table_copy = info_table_copy[[Class_NM_Col,'New_ID']]
+        info_table_copy2 = pd.merge(info_table, info_table_copy, how='inner', on = Class_NM_Col).copy(deep=True)
+
+        cleaned = pd.merge(cleaned, info_table_copy2, how='inner', on = Class_Col)
+        cleaned[Class_Col] = cleaned['New_ID']
+        #update
+    #    clipped Class_Col based on the Class_NM_Col
+    #    arcpy.RepairGeometry_management(os.path.join(tempfolder,Class_Col+"_dislve.shp"))
+
+    #    arcpy.AddSpatialIndex_management(os.path.join(tempfolder,Class_Col+"_dislve.shp"))
+    return cleaned
+
+
+def save_modified_attributes_to_outputs(mapoldnew_info,tempfolder,OutputFolder,cat_name,riv_name,Path_final_riv,dis_col_name='SubId'):
+
+
+    NEED_TO_REMOVE_IDS = ["SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_SubId","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId","SubIdt2"]
+
+    #obtain readme file
+    if "DA_Chn_L" in  mapoldnew_info.columns:
+        url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_OIH.pdf'
+    else:
+        url = 'https://github.com/dustming/RoutingTool/wiki/Files/README_NA.pdf'
+
+    response = requests.get(url)
+    with open(os.path.join(OutputFolder,"README.pdf"), 'wb') as f:
+        f.write(response.content)
+
+    if riv_name != '#':
+
+        if Path_final_riv != '#':
+            riv_pd = geopandas.read_file(Path_final_riv)
+            riv_pd['Old_SubId'] = riv_pd['SubId']
+
+        cat_pd = mapoldnew_info.drop(columns = 'geometry').copy(deep=True)
+        # remove all columns
+        if Path_final_riv != '#':
+            riv_pd = riv_pd[['geometry','Old_SubId']]
+            riv_pd = pd.merge(riv_pd, cat_pd, on='Old_SubId', how='left')
+            riv_pd = riv_pd.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
+
+
+        mapoldnew_info = mapoldnew_info.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
+        mapoldnew_info = add_centroid_in_wgs84(mapoldnew_info,"centroid_x","centroid_y")
+
+        cat_c_x_y = mapoldnew_info[["centroid_y","centroid_x"]].copy(deep=True)
+        if Path_final_riv != '#':
+            riv_pd = riv_pd.drop(columns = ["centroid_y","centroid_x"])
+            riv_pd = riv_pd.join(cat_c_x_y)
+
+        riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2][['SubId','DowSubId']].copy(deep=True)
+        remove_channel = []
+        for subid in riv_pd_nncls_routing_info['SubId'].values:
+            if subid not in riv_pd_nncls_routing_info['DowSubId'].values:
+                remove_channel.append(subid)
+        if Path_final_riv != '#':
+            riv_pd = riv_pd[~riv_pd.SubId.isin(remove_channel)]
+            cat_colnms = riv_pd.columns
+            drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
+            riv_pd = riv_pd.drop(columns=drop_cat_colnms)
+            if len(riv_pd) > 0:
+                riv_pd.to_file(os.path.join(OutputFolder,riv_name))
+
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
+        mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
+
+        cat_colnms = mapoldnew_info.columns
+        drop_cat_colnms = cat_colnms[cat_colnms.isin(NEED_TO_REMOVE_IDS)]
+        mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
+        mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
+
+        outline = create_watershed_boundary(mapoldnew_info)
+        outline.to_file(os.path.join(OutputFolder,"outline.shp"))
+        create_geo_jason_file(os.path.join(OutputFolder,cat_name))
+
+    else:
+
+        mapoldnew_info = mapoldnew_info.dissolve(by=dis_col_name, aggfunc='first',as_index=False)
+
+        if "centroid_y" in mapoldnew_info.columns:
+
+            mapoldnew_info = add_centroid_in_wgs84(mapoldnew_info,"centroid_x","centroid_y")
+            mapoldnew_info["SubId"] = mapoldnew_info.index
+            riv_pd_nncls_routing_info = mapoldnew_info[mapoldnew_info['Lake_Cat'] != 2][['SubId','DowSubId']].copy(deep=True)
+            remove_channel = []
+            for subid in riv_pd_nncls_routing_info['SubId'].values:
+                if subid not in riv_pd_nncls_routing_info['DowSubId'].values:
+                    remove_channel.append(subid)
+
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivSlope'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'RivLength'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'FloodP_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Ch_n'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Max_DEM'] = -1.2345
+            mapoldnew_info.loc[mapoldnew_info.SubId.isin(remove_channel),'Min_DEM'] = -1.2345
+
+
+        cat_colnms = mapoldnew_info.columns
+        drop_cat_colnms = cat_colnms[cat_colnms.isin(["SHAPE","SubId_1", "Id","nsubid2", "nsubid","ndownsubid","Old_DowSub","Join_Count","TARGET_FID","Id","SubID_Oldr","HRU_ID_N_1","HRU_ID_N_2","facters","Old_DowSubId"])]
+        mapoldnew_info = mapoldnew_info.drop(columns=drop_cat_colnms)
+        mapoldnew_info.to_file(os.path.join(OutputFolder,cat_name))
+        outline = create_watershed_boundary(mapoldnew_info)
+        outline.to_file(os.path.join(OutputFolder,"outline.shp"))
+        return mapoldnew_info
+
+def create_watershed_boundary(mapoldnew_info):
+    wb = mapoldnew_info.copy(deep=True)[['geometry']]
+    wb["ID"] = 1
+    wb = wb.dissolve(by="ID", aggfunc='first',as_index=False)
+    return wb
+
+def Remove_Unselected_Lake_Attribute_In_Finalcatinfo_purepy(finalcat_ply, Conn_Lake_Ids):
+    """Functions will set lake id not in Conn_Lake_Ids to -1.2345 in attribute
+        table of Path_Finalcatinfo
+    ----------
+
+    Notes
+    -------
+
+    Returns:
+    -------
+        None, the attribute table of Path_shpfile will be updated
+    """
+
+    mask1 = np.logical_not(finalcat_ply['HyLakeId'].isin(Conn_Lake_Ids))
+    mask2 = finalcat_ply['Lake_Cat'] != 2
+    mask = np.logical_and(mask1,mask2)
+
+    finalcat_ply.loc[mask,'HyLakeId'] = 0
+    finalcat_ply.loc[mask,'LakeVol'] = 0
+    finalcat_ply.loc[mask,'LakeArea'] = 0
+    finalcat_ply.loc[mask,'LakeDepth'] = 0
+    finalcat_ply.loc[mask,'Laketype'] =0
+    finalcat_ply.loc[mask,'Lake_Cat'] = 0
+
+    return finalcat_ply
+
+def clean_attribute_name_purepy(table,names):
+    remove_column_names = table.columns[np.logical_not(np.isin(table.columns,names))]
+    table = table.drop(columns=remove_column_names)
+    return table
+
+def clean_geometry_purepy(data,set_precision = -1):
+
+#    data["geometry"] = data["geometry"].apply(lambda x: shapely.wkt.loads(shapely.wkt.dumps(x, rounding_precision=4)))
+    if set_precision > 0:
+        data['geometry'] = data['geometry'].buffer(0.00000000001)
+
+#        data.geometry = pg.set_precision(data.geometry.values.data, 1e-6)
+#        data["geometry"] = data["geometry"].apply(lambda x: shapely.wkt.loads(shapely.wkt.dumps(x, rounding_precision=4)))
+#        data['geometry'] = data['geometry'].buffer(0)
+#    print("aaaa")
+    narow = ~data['geometry'].isna()
+#    print("a1",len(data.loc[narow]))
+    emrow = ~data.is_empty
+#    print("a2",len(data.loc[emrow]))
+    arearow = data.area > 0
+#    print("a3",len(data.loc[arearow]))
+#    arevalid = data.is_valid
+    row1 = np.logical_and(narow,emrow)
+    rowselect = np.logical_and(arearow,row1)
+#    print("a",len(data))
+#    rowselect = np.logical_and(rowselect,arevalid)
+    data = data.loc[rowselect]
+#    print("b",len(data))
+    data = data.loc[data.geom_type != 'Point']
+    if len(data.loc[data.geom_type == 'GeometryCollection']) > 0:
+        print("###########################")
+        print("check the following features")
+        print(data.loc[data.geom_type == 'GeometryCollection'])
+        print("###########################")
+
+    data = data.loc[data.geom_type != 'GeometryCollection']
+    data.sindex
+#    print("c",len(data))
+    return data
+
+def add_area_in_m2(data,prj_crs,area_col):
+    src_src = data.crs
+    tost = data.copy()
+
+    tost= data.to_crs(prj_crs)
+    tost[area_col] = tost.area
+
+    out= tost.copy(deep=True).to_crs(src_src)
+
+    return out
+
+def add_centroid_in_wgs84(data,colx,coly):
+    src_src = data.crs
+    tost = data.copy()
+
+    tost= tost.to_crs('EPSG:4326')
+
+    tost[coly] = tost.geometry.centroid.y
+    tost[colx] = tost.geometry.centroid.x
+
+    out= tost.copy(deep=True).to_crs(src_src)
+
+    return out
+
+
+def create_geo_jason_file(Input_Polygon_path):
+
+    if "finalcat_info" not in Input_Polygon_path:
+#        print(Input_Polygon_path)
+        return
+
+    product_dir = os.path.dirname(Input_Polygon_path)
+    Names_in = os.path.basename(Input_Polygon_path).split('_')
+    n_charc = len(Names_in)
+    version  = Names_in[n_charc - 1][0:4]
+    TOLERANCEs = [0.0001,0.005]
+
+
+    head_name_cat = "finalcat_info"
+    head_name_riv = "finalcat_info_riv"
+    head_name_slake = "sl_connected_lake"
+    head_name_nlake = "sl_non_connected_lake"
+
+    Input_file_name = []
+    Output_file_name = []
+    if 'v' in version:
+        Input_file_name = [
+                           head_name_cat + "_"+version+'.shp',
+                           head_name_riv + "_"+version+'.shp',
+                           head_name_slake + "_"+version+'.shp',
+                           head_name_nlake + "_"+version+'.shp',
+                           ]
+        Output_file_name = [
+                           head_name_cat + "_"+version+'.geojson',
+                           head_name_riv + "_"+version+'.geojson',
+                           head_name_slake + "_"+version+'.geojson',
+                           head_name_nlake + "_"+version+'.geojson',
+                           ]
+    else:
+        Input_file_name = [
+                           head_name_cat +'.shp',
+                           head_name_riv +'.shp',
+                           head_name_slake +'.shp',
+                           head_name_nlake +'.shp',
+                           ]
+        Output_file_name = [
+                           head_name_cat +'.geojson',
+                           head_name_riv +'.geojson',
+                           head_name_slake +'.geojson',
+                           head_name_nlake +'.geojson',
+                           ]
+    created_jason_files = []
+    created_jason_files_lake_riv = []
+
+    for i  in  range(0,len(Input_file_name)):
+        input_path = os.path.join(product_dir,Input_file_name[i])
+        output_jason_path = os.path.join(product_dir,Output_file_name[i])
+        if not os.path.exists(input_path):
+            continue
+        created_jason_files.append(output_jason_path)
+
+        if 'finalcat_info_riv' in Input_file_name[i] or 'connected_lake' in Input_file_name[i]:
+            created_jason_files_lake_riv.append(output_jason_path)
+
+        # reproject to WGS84
+        input_pd = geopandas.read_file(input_path)
+
+        input_wgs_84 = input_pd.to_crs('EPSG:4326')
+
+
+
+        if 'finalcat_info' in Input_file_name[i] or "finalcat_info_riv" in Input_file_name[i]:
+            input_wgs_84['rvhName'] = input_wgs_84['SubId'].astype(int).astype(str)
+            for idx in input_wgs_84.index:
+                input_wgs_84.loc[idx,'rvhName'] = 'sub' + input_wgs_84.loc[idx,'rvhName']
+
+
+        input_tojson = input_wgs_84
+
+        for TOLERANCE in TOLERANCEs:
+            input_tojson['geometry'] = input_tojson.simplify(TOLERANCE)
+            input_tojson.to_file(output_jason_path, driver="GeoJSON")
+
+            json_file_size = os.stat(output_jason_path).st_size/1024/1024 #to MB
+            if json_file_size <= 100:
+                break
+
+    if len(created_jason_files_lake_riv) > 1 and os.stat(os.path.join(product_dir,Output_file_name[0])).st_size/1024/1024 < 500:
+        for i in range(0,len(created_jason_files_lake_riv)):
+            injson2 = load(open(created_jason_files_lake_riv[i]))
+            if 'finalcat_info_riv' in created_jason_files_lake_riv[i]:
+                new_features = []
+                for element in injson2["features"]:
+                    if element["properties"]["Lake_Cat"] == 0:
+                        new_features.append(element)
+                injson2["features"] = new_features
+
+            if i == 0:
+                output_jason_lake_riv = injson2
+            else:
+                output_jason_lake_riv['features'] += injson2['features']
+
+        with open(os.path.join(product_dir,'routing_product_lake_river.geojson'), 'w', encoding='utf-8') as f:
+            json.dump(output_jason_lake_riv, f, ensure_ascii=False, indent=4)
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/func/qgis.py` & `basinmaker-3.0.3/basinmaker/func/qgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/func/rarray.py` & `basinmaker-3.0.3/basinmaker/func/rarray.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/hymodin/raveninput.py` & `basinmaker-3.0.3/basinmaker/hymodin/raveninput.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     Examples
     -------
 
     """
 
     Raveinputsfolder = os.path.join(OutputFolder, "RavenInput")
     Obs_Folder = os.path.join(Raveinputsfolder, "obs")
+    Json_Folder = os.path.join(Raveinputsfolder, "geojsons")
 
     if not os.path.exists(OutputFolder):
         os.makedirs(OutputFolder)
 
     shutil.rmtree(Raveinputsfolder, ignore_errors=True)
 
     ### check if there is a model input template provided
@@ -199,30 +200,34 @@
         toDirectory = Raveinputsfolder
         copy_tree(fromDirectory, toDirectory)
 
     if not os.path.exists(Raveinputsfolder):
         os.makedirs(Raveinputsfolder)
     if not os.path.exists(Obs_Folder):
         os.makedirs(Obs_Folder)
+    if not os.path.exists(Json_Folder):
+        os.makedirs(Json_Folder)
+
+    copy_files_with_extension(os.path.dirname(Path_final_hru_info),Json_Folder,"*.geojson")
 
     if Forcing_Input_File != "#":
         fromDirectory = Forcing_Input_File
         toDirectory = os.path.join(Raveinputsfolder, "GriddedForcings2.txt")
         copyfile(fromDirectory, toDirectory)
 
     finalcatchpath = Path_final_hru_info
 
     tempinfo = Dbf5(finalcatchpath[:-3] + "dbf")
     ncatinfo = tempinfo.to_dataframe()
     ncatinfo2 = ncatinfo.drop_duplicates("HRU_ID", keep="first")
     ncatinfo2 = ncatinfo2.loc[(ncatinfo2["HRU_ID"] > 0) & (ncatinfo2["SubId"] > 0)]
-    
+
     if 'DrainArea' in ncatinfo2.columns:
         ncatinfo2 = ncatinfo2.sort_values(by=['DrainArea','HRU_ID'])
-    
+
     if 'Rivlen' in ncatinfo2.columns:
         ncatinfo2["RivLength"] = ncatinfo2["Rivlen"].values
     #            ncatinfo2['RivSlope'] = ncatinfo2['Rivlen'].values
     #            ncatinfo2['RivLength'] = ncatinfo2['Rivlen'].values
     #            ncatinfo2['RivLength'] = ncatinfo2['Rivlen'].values
     #            ncatinfo2['RivLength'] = ncatinfo2['Rivlen'].values
     (
@@ -245,19 +250,19 @@
         SubBasinGroup_Length_Channel,
         time_step,
         aspect_from_gis
     )
     WriteStringToFile(Channel_rvp_string + '\n \n', Channel_rvp_file_path, "w")
     WriteStringToFile(Model_rvh_string + '\n \n', Model_rvh_file_path, "w")
     WriteStringToFile(Model_rvp_string_modify + '\n \n', Model_rvp_file_path, "a")
-    
+
     Lake_rvh_string, Lake_rvh_file_path = Generate_Raven_Lake_rvh_String(
         ncatinfo2, Raveinputsfolder, Model_Name,lake_out_flow_method
     )
-            
+
     WriteStringToFile(Lake_rvh_string, Lake_rvh_file_path, "w")
 
     if WriteObsrvt > 0:
         (
             obs_rvt_file_path_gauge_list,
             obs_rvt_file_string_gauge_list,
             Model_rvt_file_path,
@@ -281,14 +286,19 @@
             )
             WriteStringToFile(
                 Model_rvt_file_string_modify_gauge_list[i] + '\n \n', Model_rvt_file_path, "a"
             )
         obsnms.to_csv(os.path.join(Obs_Folder, "obsinfo.csv"))
 
 
+    src_geojson = os.path.join(os.path.dirname(Path_final_hru_info),"finalcat_info.geojson")
+    tar_geojson = os.path.join(Raveinputsfolder,"finalcat_info.geojson")
+    if os.path.exists(src_geojson):
+        shutil.copyfile(src_geojson, tar_geojson)
+
 ####
 # Inputs
 ####
 def DownloadStreamflowdata_CA(Station_NM, CA_HYDAT, StartYear, EndYear):
     """Return streamflow data from HYDAT
 
     Function that used to obtain streamflow data of certain gauge from HYDAT database
@@ -461,15 +471,15 @@
     else:
         try:
             obs_DA = (
                 float(station_info_value[len(station_info_value) - 1].decode("utf-8"))
                 * 2.58999
             )  # square miles to square km
         except:
-            try: 
+            try:
                 obs_DA = (
                     float(station_info_value[len(station_info_value) - 2].decode("utf-8"))
                     * 2.58999
                 )  # square miles to square km
             except:
                 obs_DA = -1.2345
 
@@ -491,15 +501,15 @@
 
     ##obtain start of the data rows
     datarow = -1
     for i in range(0, len(stlistdata)):
         istlistdata = stlistdata[i].split()
         if len(istlistdata) == 0:
             return -1.2345,-1.2345, False
-            
+
         if istlistdata[0] == "#" or len(istlistdata) != 5:
             continue
         if istlistdata[1].decode("utf-8") == str(int(Station_NM)).zfill(8):
             datarow = i
             break
     Date_ini = stlistdata[datarow].split()[2].decode("utf-8")
     Date_end = stlistdata[len(stlistdata) - 1].split()[2].decode("utf-8")
@@ -787,17 +797,17 @@
     >>>
 
 
     """
 
     obsnms = catinfo[["Obs_NM", "SRC_obs", "SubId", "DrainArea"]]
     obsnms = obsnms.drop_duplicates("Obs_NM", keep="first")
-    obsnms = obsnms.replace(np.nan, '-9999.0', regex=True)    
+    obsnms = obsnms.replace(np.nan, '-9999.0', regex=True)
     obsnms = obsnms.loc[obsnms["Obs_NM"] != "-9999.0"]
-    
+
     obsnms.loc[:, "DrainArea"] = obsnms["DrainArea"].values / 1000 / 1000  # m2 to km2
     index = obsnms.index
     Date = pd.date_range(
         start=str(startyear) + "-" + "01" + "-" + "01",
         end=str(endyear) + "-" + "12" + "-" + "31",
         freq="D",
     )
@@ -1044,15 +1054,15 @@
     Lake_rvh_string_list.append("# This is a Raven lake rvh file generated")
     Lake_rvh_string_list.append("# by BasinMaker v2.0")
     Lake_rvh_string_list.append("#----------------------------------------------")
 
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in catinfo.columns:
         Gauge_col_Name = "Has_Gauge"
-        
+
     for i in range(0, len(catinfo.index)):
         if catinfo.iloc[i]["HRU_IsLake"] > 0:  ## lake hru
             lakeid = int(catinfo.iloc[i]["HyLakeId"])
             catid = catinfo.iloc[i]["SubId"]
             A = catinfo.iloc[i]["HRU_Area"]  ### in meters
             h0 = catinfo.iloc[i]["LakeDepth"]  ## m
             WeirCoe = 0.6
@@ -1094,16 +1104,16 @@
                 )  # f2.write("  :MaxDepth "+str(h0)+ "\n")
                 Lake_rvh_string_list.append(
                     "  :LakeArea    " + str(A)
                 )  # f2.write("  :LakeArea    "+str(A)+ "\n")
 
                 Lake_rvh_string_list.append(
                     "  :SeepageParameters   0   0 "
-                )  # f2.write("  :LakeArea    "+str(A)+ "\n")            
-                
+                )  # f2.write("  :LakeArea    "+str(A)+ "\n")
+
                 Lake_rvh_string_list.append(
                     ":EndReservoir   "
                 )  # f2.write(":EndReservoir   "+"\n")
             elif has_obs >= 1 and lake_out_flow_method == 'power_law':
                 Lake_rvh_string_list.append(
                     "#############################################"
                 )  # f2.write("#############################################"+"\n")
@@ -1127,59 +1137,59 @@
                     "  :Type RESROUTE_STANDARD   "
                 )  # f2.write("  :Type RESROUTE_STANDARD   "+"\n")
                 Lake_rvh_string_list.append(
                     "  :MaxDepth " + str(h0)
                 )  # f2.write("  :MaxDepth "+str(h0)+ "\n")
                 Lake_rvh_string_list.append(
                     "  :SeepageParameters   0   0 "
-                )  # f2.write("  :LakeArea    "+str(A)+ "\n")            
+                )  # f2.write("  :LakeArea    "+str(A)+ "\n")
 
                 Lake_rvh_string_list.append(
                     "  :OutflowStageRelation POWER_LAW "
-                )           
+                )
 
                 Lake_rvh_string_list.append(
                     "  %s   %s " %(str(Crewd*2/3*(9.80616**(0.5))),str(1.5))
-                ) 
-                
+                )
+
                 Lake_rvh_string_list.append(
                     "  :EndOutflowStageRelation "
-                ) 
-                            
+                )
+
 
                 Lake_rvh_string_list.append(
                     "  :VolumeStageRelation POWER_LAW "
-                )           
+                )
 
                 Lake_rvh_string_list.append(
                     "  %s   %s " %(str(A),str(1))
-                ) 
-                
+                )
+
                 Lake_rvh_string_list.append(
                     "  :EndVolumeStageRelation "
-                ) 
-                
-                
+                )
+
+
                 Lake_rvh_string_list.append(
                     "  :AreaStageRelation POWER_LAW "
-                )           
+                )
 
                 Lake_rvh_string_list.append(
                     "  %s   %s " %(str(A),str(0))
-                ) 
-                
+                )
+
                 Lake_rvh_string_list.append(
                     "  :EndAreaStageRelation "
-                ) 
-                            
-                            
+                )
+
+
                 Lake_rvh_string_list.append(
                     ":EndReservoir   "
                 )  # f2.write(":EndReservoir   "+"\n")
-                
+
     Lake_rvh_string = "\n".join(Lake_rvh_string_list)
     return Lake_rvh_string, Lake_rvh_file_path
     #### write lake input files for different lake zone
 
 
 #########################
 def Return_Group_Name_Based_On_Value(value, GroupNames, Group_Thresthold_Values):
@@ -1338,15 +1348,15 @@
     >>> ncatinfo2 = ncatinfo.drop_duplicates('HRU_ID', keep='first')
     >>> Channel_rvp_file_path,Channel_rvp_string,Model_rvh_file_path,Model_rvh_string,Model_rvp_file_path,Model_rvp_string_modify = Generate_Raven_Channel_rvp_rvh_String(ncatinfo2,Raveinputsfolder,lenThres,
     ...                                                                                                                                                                   iscalmanningn,Lake_As_Gauge,Model_Name
     ...                                                                                                                                                                   )
     >>>
 
     """
-        
+
     Channel_rvp_file_path = os.path.join(Raveinputsfolder, "channel_properties.rvp")
     Channel_rvp_string_list = []
     Model_rvh_file_path = os.path.join(Raveinputsfolder, Model_Name + ".rvh")
     Model_rvh_string_list = []
     Model_rvp_file_path = os.path.join(Raveinputsfolder, Model_Name + ".rvp")
     Model_rvp_string_modify = (
         "\n" + ":RedirectToFile " + "channel_properties.rvp" + "\n"
@@ -1399,15 +1409,15 @@
     )
     not_write_default_channel = True
     for i in range(0, len(catinfo_sub)):
         ### Get catchment width and dpeth
         catid = int(catinfo_sub["SubId"].values[i])
         downcatid = int(catinfo_sub["DowSubId"].values[i])
         temp = catinfo_sub["RivLength"].values[i]
-        
+
         if float(temp) > lenThres:
             catlen = float(temp) / 1000  #### in km
             strRlen = '{:>10.4f}'.format(catlen) #str(catlen)
         else:
             catlen = -9999
             strRlen = "ZERO-"
         if (
@@ -1427,15 +1437,15 @@
         GroupName = Return_Group_Name_Based_On_Value(
             catinfo_sub["RivLength"].values[i],
             SubBasinGroup_NM_Channel,
             SubBasinGroup_Length_Channel,
         )
         SubBasin_Group_Channel.loc[i, "SubId"] = catid
         SubBasin_Group_Channel.loc[i, "SubBasin_Group_NM"] = GroupName
-        
+
         if strRlen != "ZERO-":
             pronam = "Chn_" + Strcat
         else:
             pronam = "Chn_ZERO_LENGTH"
 
         if strRlen != "ZERO-":
             chslope = max(catinfo_sub["RivSlope"].values[i], min_riv_slope)
@@ -1447,22 +1457,22 @@
         else:
             nchn = 0.12345
 
         if strRlen != "ZERO-":
             floodn = catinfo_sub["FloodP_n"].values[i]
         else:
             floodn = 0.12345
-        
+
         if strRlen != "ZERO-":
             bkf_width = max(catinfo_sub["BkfWidth"].values[i], 1)
             bkf_depth = max(catinfo_sub["BkfDepth"].values[i], 1)
         else:
             bkf_width = 0.12345
             bkf_depth = 0.12345
-        
+
         if strRlen != "ZERO-":
             output_string_chn_rvp_sub = Generate_Raven_Channel_rvp_string_sub(
                 pronam,
                 bkf_width,
                 bkf_depth,
                 chslope,
                 catinfo_sub["MeanElev"].values[i],
@@ -1479,81 +1489,81 @@
                 catinfo_sub["MeanElev"].values[i],
                 floodn,
                 nchn,
                 iscalmanningn,
             )
             not_write_default_channel = False
         else:
-            output_string_chn_rvp_sub = [] 
+            output_string_chn_rvp_sub = []
             output_string_chn_rvp_sub.append("#   Sub "+ Strcat + "  refer to  Chn_ZERO_LENGTH ")
             output_string_chn_rvp_sub.append("##############new channel ##############################")
             output_string_chn_rvp_sub = "\n".join(output_string_chn_rvp_sub)
-            
+
         Channel_rvp_string_list.append(output_string_chn_rvp_sub)
 
         Gauge_col_Name = "Has_POI"
         if "Has_POI" not in catinfo_sub.columns:
             Gauge_col_Name = "Has_Gauge"
-        
+
         if catinfo_sub[Gauge_col_Name].values[i] > 0:
             Guage = "1"
         elif (
             catinfo_sub["Lake_Cat"].values[i] > 0 and Lake_As_Gauge == True
-        ): 
+        ):
             Guage = "1"
         else:
             Guage = "0"
-        
+
         Model_rvh_string_list.append(
             "  "
             + Strcat
             + tab
             + "sub"
             + Strcat
             + tab
             + StrDid
             + tab
             + pronam
             + tab
             + strRlen
             + tab
             + Guage
-        )  
+        )
 
     Model_rvh_string_list.append(":EndSubBasins")  # orvh.write(":EndSubBasins"+"\n")
     Model_rvh_string_list.append("\n")  # orvh.write("\n")
     ##########################################
-    
+
     # Model_rvh_string_list.append(":SubBasinProperties")
     # Model_rvh_string_list.append(":Parameters,  TIME_TO_PEAK,  TIME_CONC,   TIME_LAG,")
     # Model_rvh_string_list.append(":Units     ,  d           ,          d,          d,")
-    # 
-    # 
+    #
+    #
     # for i in range(0, len(catinfo_sub)):
     #     ### Get catchment width and dpeth
     #     catid = int(catinfo_sub["SubId"].values[i])
     #     subarea = int(catinfo_sub["BasArea"].values[i]/1000/1000)
-    #     if (catinfo_sub["Lake_Cat"].values[i] <= 0):  
+    #     if (catinfo_sub["Lake_Cat"].values[i] <= 0):
     #         routing_area = subarea
     #     else:
     #         routing_area = max(0.0001,subarea - catinfo_sub["LakeArea"].values[i]/1000/1000)
-    # 
+    #
     #     Tc = max(0.01,0.76*routing_area**0.38/24)
     #     Tl = 0.6*Tc
     #     Tp = Tr/2 +Tl
-    # 
+    #
     #     Tc = '{:>10.4f}'.format(Tc)  + "," + tab
-    #     Tl = '{:>10.4f}'.format(Tl)  + "," + tab 
-    #     Tp = '{:>10.4f}'.format(Tp)  + "," + tab 
+    #     Tl = '{:>10.4f}'.format(Tl)  + "," + tab
+    #     Tp = '{:>10.4f}'.format(Tp)  + "," + tab
     #     Model_rvh_string_list.append(tab + str(catid) + "," + tab + Tp + Tc + Tl)
-    # 
+    #
     # Model_rvh_string_list.append(":EndSubBasinProperties")
-    # 
+    #
     # Model_rvh_string_list.append("\n")  # orvh.write("\n")
-        
+
     ##########################################
     Model_rvh_string_list.append(":HRUs")  # orvh.write(":HRUs"+"\n")
     Model_rvh_string_list.append(
         "  :Attributes AREA ELEVATION  LATITUDE  LONGITUDE   BASIN_ID  LAND_USE_CLASS  VEG_CLASS   SOIL_PROFILE  AQUIFER_PROFILE   TERRAIN_CLASS   SLOPE   ASPECT"
     )  # orvh.write("  :Attributes AREA ELEVATION  LATITUDE  LONGITUDE   BASIN_ID  LAND_USE_CLASS  VEG_CLASS   SOIL_PROFILE  AQUIFER_PROFILE   TERRAIN_CLASS   SLOPE   ASPECT"+"\n")
     Model_rvh_string_list.append(
         "  :Units       km2         m       deg        deg       none            none       none           none             none            none     deg      deg"
@@ -1580,32 +1590,32 @@
         LAND_USE_CLASS = catinfo_hru["LAND_USE_C"].values[i] + tab
         VEG_CLASS = catinfo_hru["VEG_C"].values[i] + tab
         SOIL_PROFILE = catinfo_hru["SOIL_PROF"].values[i] + tab
         AQUIFER_PROFILE = "[NONE]" + tab
         TERRAIN_CLASS = "[NONE]" + tab
 
         SLOPE = '{:>10.6f}'.format(catslope)  + tab #str(catslope) + tab
-        
+
         if aspect_from_gis == 'grass':
             asp_temp = 270 + cataspect
             if asp_temp > 360:
                 asp_temp = asp_temp - 360
             ASPECT = '{:>10.4f}'.format(asp_temp)  + tab # str(asp_temp) + tab
-            
+
         elif aspect_from_gis == 'arcgis' or aspect_from_gis == 'qgis':
             asp_temp = -(-360 + cataspect)
             if asp_temp > 360:
                 asp_temp = asp_temp - 360
             ASPECT = str(asp_temp) + tab
         elif aspect_from_gis == 'purepy':
             asp_temp = 360 - cataspect
-            ASPECT = str(asp_temp) + tab            
+            ASPECT = str(asp_temp) + tab
         else:
             ASPECT = '{:>10.4f}'.format(cataspect)  + tab #str(cataspect) + tab
-            
+
         Model_rvh_string_list.append(
             "  "
             + StrGid
             + tab
             + StrGidarea
             + StrGidelev
             + lat
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/combine.py` & `basinmaker-3.0.3/basinmaker/postprocessing/combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import pandas as pd
 import numpy as np
 import tempfile
 from joblib import Parallel, delayed
 
 
 def combine_catchments_covered_by_the_same_lake_qgis(
-    # OutputFolder, 
-    # Path_final_rivply="#", 
-    # Path_final_riv="#", 
+    # OutputFolder,
+    # Path_final_rivply="#",
+    # Path_final_riv="#",
     Routing_Product_Folder = '#',
     qgis_prefix_path="#"
 ):
     """Define final lake river routing structure
 
     Generate the final lake river routing structure by merging subbasin
     polygons that are covered by the same lake.
@@ -78,31 +78,31 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
 
     OutputFolder = Routing_Product_Folder
 
@@ -147,29 +147,29 @@
     finalrivply_info = Dbf_To_Dataframe(Path_Temp_final_rviply).drop_duplicates(
         "SubId", keep="first"
     )
     # change attribute table for lake covered catchments,
     mapoldnew_info = change_attribute_values_for_catchments_covered_by_same_lake(
         finalrivply_info
     )
-    
+
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivLength'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivSlope'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'FloodP_n'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Ch_n'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Max_DEM'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Min_DEM'] = -1.2345
-    
+
     if 'DA_Chn_L' in mapoldnew_info.columns:
         mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'DA_Chn_L'] = -1.2345
         mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'DA_Chn_Slp'] = -1.2345
 
     # update topology for new attribute table
     update_topology(mapoldnew_info, UpdateStreamorder=-1)
 
     # copy new attribute table to shpfile
     all_subids = finalrivply_info['SubId'].values
-    
+
     copy_data_and_dissolve(all_subids,tempfolder,processing,Path_Temp_final_rviply,Path_Temp_final_rvi,
         mapoldnew_info,COLUMN_NAMES_CONSTANT_CLEAN,OutputFolder,Path_Catchment_Polygon,context)
-        
-    return 
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/combinearcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/combinearcgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import sys
 import os
 import csv
-import tempfile 
-import copy 
+import tempfile
+import copy
 import pandas as pd
 from arcgis.features import GeoAccessor, GeoSeriesAccessor
 import arcpy
 from arcpy import env
 from arcpy.sa import *
 
 
@@ -74,57 +74,57 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
-    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
+    if Path_Catchment_Polygon == '#':
         print("Invalid routing product folder ")
 
 
     OutputFolder = Routing_Product_Folder
 
 
     Path_final_rivply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
     if not os.path.exists(OutputFolder):
         os.makedirs(OutputFolder)
-        
+
     tempfolder = os.path.join(
         tempfile.gettempdir(), "basinmaker_" + str(np.random.randint(1, 10000 + 1))
     )
     if not os.path.exists(tempfolder):
         os.makedirs(tempfolder)
     arcpy.env.workspace = tempfolder
 
     ### create a copy of shapfiles in temp folder
     Path_Temp_final_rviply = os.path.join(OutputFolder,"temp_finalriv_ply" + str(np.random.randint(1, 10000 + 1)) + ".shp")
-    
+
     Path_Temp_final_rvi = os.path.join(OutputFolder,"temp_finalriv_riv" + str(np.random.randint(1, 10000 + 1)) + ".shp")
-    
+
     ### read riv ply info
     ### read attribute table
     finalrivply_info = pd.DataFrame.spatial.from_featureclass(Path_final_rivply)
     # change attribute table for lake covered catchments,
     finalrivply_info['SubId'] = finalrivply_info['SubId'].astype('int32')
     finalrivply_info['DowSubId'] = finalrivply_info['DowSubId'].astype('int32')
     finalrivply_info['HyLakeId'] = finalrivply_info['HyLakeId'].astype('int32')
@@ -132,39 +132,39 @@
 
     mapoldnew_info = change_attribute_values_for_catchments_covered_by_same_lake(
         finalrivply_info
     )
 
     mapoldnew_info = remove_possible_small_subbasins(mapoldnew_info = mapoldnew_info, area_thresthold = 10*30*30/1000/1000)
     # update topology for new attribute table
-    
+
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivLength'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivSlope'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'FloodP_n'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Ch_n'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Max_DEM'] = -1.2345
     mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'Min_DEM'] = -1.2345
-    
+
     if 'DA_Chn_L' in mapoldnew_info.columns:
         mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivLength'] = -1.2345
         mapoldnew_info.loc[mapoldnew_info['Lake_Cat'] > 0,'RivLength'] = -1.2345
-            
-    mapoldnew_info = update_topology(mapoldnew_info, UpdateStreamorder=-1)    
-    
+
+    mapoldnew_info = update_topology(mapoldnew_info, UpdateStreamorder=-1)
+
     mapoldnew_info['DowSubId'] = mapoldnew_info['DowSubId'].astype('int32')
-    
+
     if len(os.path.basename(Path_Catchment_Polygon).split('_')) == 5:
         cat_name = "finalcat_info_"+os.path.basename(Path_Catchment_Polygon).split('_')[4]
         riv_name = "finalcat_info_riv_"+os.path.basename(Path_Catchment_Polygon).split('_')[4]
     else:
         cat_name =  "finalcat_info.shp"
         riv_name =  "finalcat_info_riv.shp"
-              
+
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=cat_name,
         riv_name =riv_name,
         Path_final_riv = Path_final_riv,
     )
-    return 
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/combinepurepy.py` & `basinmaker-3.0.3/basinmaker/postprocessing/combinepurepy.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,22 +80,22 @@
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
                 Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
-    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
+    if Path_Catchment_Polygon == '#':
         print("Invalid routing product folder ")
 
 
     OutputFolder = Routing_Product_Folder
 
 
     Path_final_rivply = Path_Catchment_Polygon
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/downloadpd.py` & `basinmaker-3.0.3/basinmaker/postprocessing/downloadpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import wget
 import pandas as pd
 import numpy as np
 import gdown
 # define function two download routing product for a given gauge
-def Download_Routing_Product_For_One_Gauge(gauge_name,product_name,region='#',subreg = '#'):
+def Download_Routing_Product_For_One_Gauge(product_name,gauge_name = "#",region='#',subreg = '#'):
     if product_name == 'NALRP':
         version = 'v2-1'
         if gauge_name != '#':
             gauge_info = pd.read_csv("https://github.com/dustming/RoutingTool/wiki/Files/obs_gauges_NA_v2-1.csv")
             gauge_info_sl = gauge_info[gauge_info['Obs_NM'] == gauge_name]
             if len(gauge_info_sl) < 1:
                 print("The gauge ",gauge_name,"is not included in the routing product ")
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/downloadpdptspurepy.py` & `basinmaker-3.0.3/basinmaker/postprocessing/downloadpdptspurepy.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/gridweight.py` & `basinmaker-3.0.3/basinmaker/postprocessing/gridweight.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/gridweightarcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/gridweightarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/hru.py` & `basinmaker-3.0.3/basinmaker/postprocessing/hru.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/hruarcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/hruarcgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/hrupurepy.py` & `basinmaker-3.0.3/basinmaker/postprocessing/hrupurepy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,883 +1,886 @@
-import numpy as np
-import sys
-import os
-import csv
-import tempfile
-import copy
-import pandas as pd
-import geopandas
-import sys, os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from basinmaker.func.purepy import *
-from basinmaker.func.pdtable import *
-from osgeo import gdal, ogr
-from basinmaker.func.fgdal import *
-
-def GenerateHRUS_purepy(
-    Path_Subbasin_Ply,
-    Landuse_info,
-    Soil_info,
-    Veg_info,
-    Inmportance_order,
-    min_hru_area_pct_sub,
-    Sub_Lake_ID="HyLakeId",
-    Sub_ID="SubId",
-    Path_Connect_Lake_ply="#",
-    Path_Non_Connect_Lake_ply="#",
-    Lake_Id="Hylak_id",
-    Path_Landuse_Ply="#",
-    Landuse_ID="Landuse_ID",
-    Path_Soil_Ply="#",
-    Soil_ID="Soil_ID",
-    Path_Veg_Ply="#",
-    Veg_ID="Veg_ID",
-    Path_Other_Ply_1="#",
-    Other_Ply_ID_1="O_ID_1",
-    Path_Other_Ply_2="#",
-    Other_Ply_ID_2="O_ID_2",
-    DEM="#",
-    Project_crs = '3573',
-    OutputFolder="#",
-    pixel_size = 30,
-    area_ratio_thresholds = [0,0,0],
-):
-    """Generate HRU polygons and their attributes needed by hydrological model
-
-    Function that be used to overlay: subbasin polygon, lake polygon (optional)
-    , Land use polygon (optional), soil type polygon(optional),
-    vegetation polygon (optional), and two other user defined polygons
-    (optional).
-    Non-lake HRU polygons in a subbasin is defined by an unique
-    combination of all user provided datasets.
-    A lake HRU polygon is defined the same as the provided lake polygon.
-    All value of landuse and Veg polygon covered by lake will
-    be changed to 1, indicating it is a covered by lake.
-    All value of the soil polygon covered by the lake will be change to
-    the soil id of the polygon covered by the lake with largest area.
-
-    Parameters
-    ----------
-    Path_Subbasin_Ply                 : string
-        It is the path of the subbasin polygon, which is generated by
-        toolbox. if not generated by toolbox, the attribute table should
-        including following attribute.
-        ##############Subbasin related attributes###########################
-        SubID           - integer, The subbasin Id
-        DowSubId        - integer, The downstream subbasin ID of this
-                                   subbasin
-        IsLake          - integer, If the subbasin is a lake / reservior
-                                   subbasin. 1 yes, <0, no
-        IsObs           - integer, If the subbasin contains a observation
-                                   gauge. 1 yes, < 0 no.
-        RivLength       - float,   The length of the river in current
-                                   subbasin in m
-        RivSlope        - float,   The slope of the river path in
-                                   current subbasin, in m/m
-        FloodP_n        - float,   Flood plain manning's coefficient, in -
-        Ch_n            - float,   main channel manning's coefficient, in -
-        BkfWidth        - float,   the bankfull width of the main channel
-                                   in m
-        BkfDepth        - float,   the bankfull depth of the main channel
-                                   in m
-        HyLakeId        - integer, the lake id
-        LakeVol         - float,   the Volume of the lake in km3
-        LakeDepth       - float,   the average depth of the lake m
-        LakeArea        - float,   the area of the lake in m2
-    Landuse_info                      : string
-        Path to a csv file that contains landuse information, including
-        following attributes:
-        Landuse_ID (can be any string)  - integer, the landuse ID in the
-                                                   landuse polygon
-        LAND_USE_C                      - string,  the landuse class name
-                                                   for each landuse Type
-    Soil_info                        : string
-        Path to a csv file that contains soil information, including
-        following attributes:
-        Soil_ID (can be any string)     - integer, the Soil ID in the
-                                                   soil polygon
-        SOIL_PROF                       - string,  the Soil profile name
-                                                   for each soil type
-    Veg_info                         : string
-        Path to a csv file that contains vegetation information, including
-        following attributes:
-        Veg_ID (can be any string)      - integer, the vegetation ID in the
-                                                   vegetation polygon
-        VEG_C                           - string,  the vegetation class name
-                                                   for each vegetation Type
-    Sub_Lake_ID                      : string (optional)
-        The column name of the lake id in the subbasin polygon
-    Sub_ID                           : string (optional)
-        The column name of the subbasin id in the subbasin polygon
-    Path_Connect_Lake_ply            : string (Optional)
-        Path to the connected lake's polygon
-    Path_Non_Connect_Lake_ply        : string (Optional)
-        Path to the non connected lake's polygon
-    Lake_Id                          : string (Optional)
-        The the column name in lake polygon indicate the lake ID.
-    Path_Landuse_Ply                 : string (Optional)
-        Path to the landuse polygon. when Path_Landuse_Ply is not
-        provided. The Landuse ID in Landuse_info should be
-        1: land, -1: lake
-    Landuse_ID                       : string (Optional)
-        the the column name in landuse polygon and Landuse_info csv
-        indicate the landuse ID. when Path_Landuse_Ply is not
-        provided. The Landuse ID should be
-        1: land, -1: lake.
-    Path_Soil_Ply                    : string (Optional)
-        Path to the soil polygon. when soil polygon is not
-        provided. The Soil ID in Soil_info should be the same
-        as Landuse ID.
-    Soil_ID                          : string (Optional)
-        the the column name in soil polygon and soil_info csv
-        indicate the soil ID. when soil polygon is not
-        provided. The Soil ID in Soil_info should be the same
-        as Landuse ID.
-    Path_Veg_Ply                     : string (Optional)
-        Path to the vegetation polygon. when Veg polygon is not
-        provided. The Veg ID in Veg_info should be the same
-        as Landuse ID.
-    Veg_ID                           : string (Optional)
-        the the column name in vegetation polygon and veg_info csv
-        indicate the vegetation ID. when Veg polygon is not
-        provided. The Veg ID in Veg_info should be the same
-        as Landuse ID.
-    Path_Other_Ply_1                 : string (Optional)
-        Path to the other polygon that will be used to define HRU,
-        such as elevation band, or aspect.
-    Other_Ply_ID_1                   : string (Optional)
-        the the column name in Other_Ply_1 polygon
-        indicate the landuse ID.
-    Path_Other_Ply_2                 : string (Optional)
-        Path to the other polygon that will be used to define HRU,
-        such as elevation band, or aspect.
-    Other_Ply_ID_2                   : string (Optional)
-        the the column name in Other_Ply_2 polygon
-        indicate the landuse ID.
-    DEM                              : string (optional)
-        the path to a raster elevation dataset, that will be used to
-        calcuate average apspect, elevation and slope within each HRU.
-        if no data is provided, basin average value will be used for
-        each HRU.
-    Project_crs                      : string
-        the EPSG code of a projected coodinate system that will be used to
-        calcuate HRU area and slope.
-    OutputFolder                     : string
-        The path to the folder that will save output HRU polygon.
-
-    Notes
-    -------
-    Following ouput files will be generated in "<OutputFolder>/"
-    'finalcat_hru_info.shp'              - HRU polygon and it's attributes
-
-
-    Returns:
-    -------
-       None
-
-    Examples
-    -------
-    >>> from ToolboxClass import LRRT
-    >>> import pandas as pd
-    >>> DataFolder = "C:/Path_to_foldr_of_example_dataset_provided_in_Github_wiki/"
-    >>> RTtool=LRRT()
-    >>> RTtool.GenerateHRUS(OutputFolder = DataFolder,
-                           Path_Subbasin_Ply = os.path.join(DataFolder,"finalcat_info.shp"),
-                           Path_Connect_Lake_ply = os.path.join(DataFolder,'Con_Lake_Ply.shp'),
-                           Path_Non_Connect_Lake_ply = os.path.join(DataFolder,'Non_Con_Lake_Ply.shp'),
-                           Path_Landuse_Ply = os.path.join(DataFolder,'modislanduse_exp_lg_pre.shp'),
-                           Landuse_ID = 'gridcode',
-                           Path_Soil_Ply = os.path.join(DataFolder,'ca_all_slc_v3r2_exp_lg.shp'),
-                           Soil_ID = 'POLY_ID',
-                           Landuse_info=os.path.join(DataFolder,'landuse_info.csv'),
-                           Soil_info=os.path.join(DataFolder,'soil_info.csv'),
-                           Veg_info=os.path.join(DataFolder,'veg_info.csv'),
-                           DEM = os.path.join(DataFolder,'na_dem_15s_1.tif')
-                           )
-
-    """
-
-    if not os.path.exists(OutputFolder):
-        os.makedirs(OutputFolder)
-
-    tempfolder = os.path.join(
-        OutputFolder, "HRU_TEMP" + str(np.random.randint(1, 10000 + 1))
-    )
-    if not os.path.exists(tempfolder):
-        os.makedirs(tempfolder)
-
-    prj_crs = Project_crs
-    Merge_layer_list = []
-    Merge_layer_raster_list = []
-    Merge_layer_shp_list = []
-    Merge_ID_list = []
-
-
-    Sub_Lake_HRU_Layer, trg_crs, fieldnames_list = GeneratelandandlakeHRUS(
-        OutputFolder,
-        tempfolder,
-        Path_Subbasin_ply=Path_Subbasin_Ply,
-        Path_Connect_Lake_ply=Path_Connect_Lake_ply,
-        Path_Non_Connect_Lake_ply=Path_Non_Connect_Lake_ply,
-        Sub_ID=Sub_ID,
-        Sub_Lake_ID=Sub_Lake_ID,
-        Lake_Id=Lake_Id,
-        prj_crs = prj_crs,
-    )
-
-    lakehruinfo = geopandas.read_file(Sub_Lake_HRU_Layer)
-    hru_lake_info = lakehruinfo.loc[lakehruinfo['HRU_IsLake'] > 0].copy()
-    lakehruinfo_landhrus = lakehruinfo.loc[lakehruinfo['HRU_IsLake'] <= 0].copy()
-
-    hru_lake_info = hru_lake_info.to_crs(prj_crs)
-    lakehruinfo_landhrus = lakehruinfo_landhrus.to_crs(prj_crs)
-    lakehruinfo = lakehruinfo.to_crs(prj_crs)
-
-    hru_lake_info = clean_geometry_purepy(hru_lake_info)
-    lakehruinfo_landhrus = clean_geometry_purepy(lakehruinfo_landhrus)
-
-    path_to_landhru_shp= os.path.join(tempfolder,'land_hru.shp')
-    path_to_lakehru_shp= os.path.join(tempfolder,'lake_hru.shp')
-    path_to_landuse_shp = os.path.join(tempfolder,'landuse.shp')
-    path_to_soil_shp = os.path.join(tempfolder,'soil.shp')
-    path_to_veg_shp = os.path.join(tempfolder,'veg.shp')
-    path_to_other1_shp = os.path.join(tempfolder,'o1.shp')
-    path_to_other2_shp = os.path.join(tempfolder,'o2.shp')
-
-
-#    lakehruinfo_landhrus.to_file(path_to_landhru_shp)
-    if len(hru_lake_info) > 0:
-        hru_lake_info.to_file(path_to_lakehru_shp)
-
-    if len(lakehruinfo_landhrus) > 0:
-        lakehruinfo_landhrus.to_file(path_to_landhru_shp)
-
-    fieldnames_list.extend(
-        [
-            Landuse_ID,
-            Soil_ID,
-            Veg_ID,
-            Other_Ply_ID_1,
-            Other_Ply_ID_2,
-            "LAND_USE_C",
-            "VEG_C",
-            "SOIL_PROF",
-            "HRU_Slope",
-            "HRU_Area",
-            "HRU_Aspect",
-            "geometry",
-        ]
-    )
-    dissolve_filedname_list = ["HRULake_ID"]
-
-    Merge_layer_list.append(lakehruinfo_landhrus)
-
-    Landuse_info_data = pd.read_csv(Landuse_info)
-    Soil_info_data = pd.read_csv(Soil_info)
-    Veg_info_data = pd.read_csv(Veg_info)
-
-
-    #### check which data will be inlucded to determine HRU
-    if Path_Landuse_Ply != "#":
-        land_landuse_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-            layer_path = Path_Landuse_Ply,
-            Class_Col = Landuse_ID,
-            tempfolder = tempfolder,
-            mask_layer = lakehruinfo,
-            Class_NM_Col = "LAND_USE_C",
-            info_table = Landuse_info_data,
-        )
-
-        if Landuse_ID not in land_landuse_clean.columns:
-            print("Landuse polygon attribute table do not contain: ",Landuse_ID)
-            sys.exit()
-        land_landuse_clean.to_file(path_to_landuse_shp)
-
-        dissolve_filedname_list.append(Landuse_ID)
-        Merge_layer_shp_list.append(path_to_landuse_shp)
-        Merge_ID_list.append(Landuse_ID)
-
-    if Path_Soil_Ply != "#":
-        land_soil_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-            layer_path = Path_Soil_Ply,
-            Class_Col = Soil_ID,
-            tempfolder = tempfolder,
-            mask_layer = lakehruinfo,
-            Class_NM_Col = "SOIL_PROF",
-            info_table = Soil_info_data,
-        )
-
-        if Soil_ID not in land_soil_clean.columns:
-            print("Soil polygon attribute table do not contain: ",Soil_ID)
-            sys.exit()
-        land_soil_clean.to_file(path_to_soil_shp)
-        dissolve_filedname_list.append(Soil_ID)
-        Merge_layer_shp_list.append(path_to_soil_shp)
-        Merge_ID_list.append(Soil_ID)
-
-    if Path_Veg_Ply != "#":
-        land_veg_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-            layer_path = Path_Veg_Ply,
-            Class_Col = Veg_ID,
-            tempfolder = tempfolder,
-            mask_layer = lakehruinfo
-        )
-
-        if Veg_ID not in land_veg_clean.columns:
-            print("Veg polygon attribute table do not contain: ",Veg_ID)
-            sys.exit()
-        land_veg_clean.to_file(path_to_veg_shp)
-        dissolve_filedname_list.append(Veg_ID)
-        Merge_layer_shp_list.append(path_to_veg_shp)
-        Merge_ID_list.append(Veg_ID)
-
-
-    if Path_Other_Ply_1 != "#":
-        land_o1_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-            layer_path = Path_Other_Ply_1,
-            Class_Col = Other_Ply_ID_1,
-            tempfolder = tempfolder,
-            mask_layer = lakehruinfo
-        )
-
-        if Other_Ply_ID_1 not in land_o1_clean.columns:
-            print("Other_Ply_1 polygon attribute table do not contain: ",Other_Ply_ID_1)
-            sys.exit()
-        land_o1_clean.to_file(path_to_other1_shp)
-        dissolve_filedname_list.append(Other_Ply_ID_1)
-        Merge_layer_shp_list.append(path_to_other1_shp)
-        Merge_ID_list.append(Other_Ply_ID_1)
-
-    if Path_Other_Ply_2 != "#":
-        land_o2_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
-            layer_path = Path_Other_Ply_2,
-            Class_Col = Other_Ply_ID_2,
-            tempfolder = tempfolder,
-            mask_layer = lakehruinfo
-        )
-
-        if Other_Ply_ID_2 not in land_o2_clean.columns:
-            print("Other_Ply_1 polygon attribute table do not contain: ",Other_Ply_ID_2)
-            sys.exit()
-        land_o2_clean.to_file(path_to_other2_shp)
-        dissolve_filedname_list.append(Other_Ply_ID_2)
-        Merge_layer_shp_list.append(path_to_other2_shp)
-        Merge_ID_list.append(Other_Ply_ID_2)
-
-    fieldnames = np.array(fieldnames_list)
-
-
-    path_to_hru_temp_shp = RasterHRUUnionInt32(OutputFolder,tempfolder,Merge_layer_shp_list,
-                            Merge_ID_list,Sub_Lake_HRU_Layer,Sub_ID,
-                            Landuse_ID,Soil_ID,Veg_ID,Other_Ply_ID_1,
-                            Other_Ply_ID_2,pixel_size,lakehruinfo)
-
-    HRU_temp1 = geopandas.read_file(path_to_hru_temp_shp)
-
-    HRU_temp1 = decode_hru_attri_ids(HRU_temp1,lakehruinfo,Landuse_ID,Soil_ID,
-                                     Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2)
-
-    HRU_temp1.to_file(os.path.join(tempfolder,'HRU_DEDOCE.shp'))
-    #####
-    hru_lake_info = HRU_temp1.loc[HRU_temp1['HRU_IsLake'] > 0].copy()
-    hru_land_info = HRU_temp1.loc[HRU_temp1['HRU_IsLake'] <= 0].copy()
-
-    # landuse polygon is not provided,landused id the same as IS_lake
-    if Path_Landuse_Ply == "#":
-        hru_land_info[Landuse_ID] = -hru_land_info['HRU_IsLake']
-    hru_lake_info[Landuse_ID] = -1
-    # if soil is not provied, it the value,will be the same as land use
-    if Path_Soil_Ply == "#":
-        hru_land_info[Soil_ID] = -hru_land_info['HRU_IsLake']
-    hru_lake_info[Soil_ID] = -1
-    # if no vegetation polygon is provide vegetation, will be the same as landuse
-    if Path_Veg_Ply == "#":
-        hru_land_info[Veg_ID] = hru_land_info[Landuse_ID]
-    hru_lake_info[Veg_ID] = -1
-    if Path_Other_Ply_1 == "#":
-        hru_land_info[Other_Ply_ID_1] = -hru_land_info['HRU_IsLake']
-    hru_lake_info[Other_Ply_ID_1] = -1
-    if Path_Other_Ply_2 == "#":
-        hru_land_info[Other_Ply_ID_2] = -hru_land_info['HRU_IsLake']
-    hru_lake_info[Other_Ply_ID_2] = -1
-
-    hru_lake_info = clean_attribute_name_purepy(hru_lake_info,fieldnames)
-    hru_land_info = clean_attribute_name_purepy(hru_land_info,fieldnames)
-
-
-    hruinfo = hru_lake_info.append(hru_land_info)
-
-    hruinfo.to_file(os.path.join(tempfolder,'HRU_with_attributes.shp'))
-
-
-    HRU_draf_final = Define_HRU_Attributes_purepy(
-        prj_crs = prj_crs,
-        trg_crs = trg_crs,
-        hruinfo = hruinfo,
-        dissolve_filedname_list = dissolve_filedname_list,
-        Sub_ID = Sub_ID,
-        Landuse_ID = Landuse_ID,
-        Soil_ID = Soil_ID,
-        Veg_ID = Veg_ID,
-        Other_Ply_ID_1 = Other_Ply_ID_1,
-        Other_Ply_ID_2 = Other_Ply_ID_2,
-        Landuse_info_data = Landuse_info_data,
-        Soil_info_data = Soil_info_data,
-        Veg_info_data = Veg_info_data,
-        DEM = DEM,
-        Path_Subbasin_Ply = Path_Subbasin_Ply,
-        min_hru_area_pct_sub = min_hru_area_pct_sub,
-        Inmportance_order = Inmportance_order,
-        OutputFolder = OutputFolder,
-        tempfolder = tempfolder,
-        area_ratio_thresholds = area_ratio_thresholds,
-    )
-
-    COLUMN_NAMES_CONSTANT_HRU_extend = COLUMN_NAMES_CONSTANT_HRU.extend(
-        [
-            Landuse_ID,
-            Soil_ID,
-            Veg_ID,
-            Other_Ply_ID_1,
-            Other_Ply_ID_2,
-            'geometry',
-            'HRU_A_G'
-        ]
-    )
-    HRU_draf_final = clean_attribute_name_purepy(HRU_draf_final,COLUMN_NAMES_CONSTANT_HRU)
-    for col in [Landuse_ID,Soil_ID,Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2,'SubId']:
-        HRU_draf_final = HRU_draf_final.loc[HRU_draf_final[col] != 0]
-
-    HRU_draf_final.to_crs(trg_crs)
-    HRU_draf_final.to_file(os.path.join(OutputFolder,'finalcat_hru_info.shp'))
-    HRU_draf_final_wgs_84 = HRU_draf_final.to_crs('EPSG:4326')
-#    HRU_draf_final_wgs_84 = HRU_draf_final_wgs_84[['HRU_ID','geometry']]
-    TOLERANCEs = [0.0001,0.0005,0.001,0.005,0.01,0.05]
-    output_jason_path = os.path.join(OutputFolder,'finalcat_hru_info.geojson')
-    for TOLERANCE in TOLERANCEs:
-        HRU_draf_final_wgs_84['geometry'] = HRU_draf_final_wgs_84.simplify(TOLERANCE)
-        HRU_draf_final_wgs_84.to_file(output_jason_path,driver="GeoJSON")
-
-        json_file_size = os.stat(output_jason_path).st_size/1024/1024 #to MB
-        if json_file_size <= 100:
-            break
-
-def GeneratelandandlakeHRUS(
-    OutputFolder,
-    tempfolder,
-    Path_Subbasin_ply,
-    Path_Connect_Lake_ply="#",
-    Path_Non_Connect_Lake_ply="#",
-    Sub_ID="SubId",
-    Sub_Lake_ID="HyLakeId",
-    Lake_Id="Hylak_id",
-    prj_crs = "EPSG:3161",
-):
-
-    """Overlay subbasin polygon and lake polygons
-
-    Function that will overlay subbasin polygon and lake polygon
-
-    Parameters
-    ----------
-    processing                        : qgis object
-    context                           : qgis object
-    OutputFolder                     : string
-        The path to the folder that will save output HRU polygon.
-
-    Path_Subbasin_Ply                 : string
-        It is the path of the subbasin polygon, which is generated by
-        toolbox. if not generated by toolbox, the attribute table should
-        including following attribute.
-        ##############Subbasin related attributes###########################
-        SubID           - integer, The subbasin Id
-        DowSubId        - integer, The downstream subbasin ID of this
-                                   subbasin
-        IsLake          - integer, If the subbasin is a lake / reservior
-                                   subbasin. 1 yes, <0, no
-        IsObs           - integer, If the subbasin contains a observation
-                                   gauge. 1 yes, < 0 no.
-        RivLength       - float,   The length of the river in current
-                                   subbasin in m
-        RivSlope        - float,   The slope of the river path in
-                                   current subbasin, in m/m
-        FloodP_n        - float,   Flood plain manning's coefficient, in -
-        Ch_n            - float,   main channel manning's coefficient, in -
-        BkfWidth        - float,   the bankfull width of the main channel
-                                   in m
-        BkfDepth        - float,   the bankfull depth of the main channel
-                                   in m
-        HyLakeId        - integer, the lake id
-        LakeVol         - float,   the Volume of the lake in km3
-        LakeDepth       - float,   the average depth of the lake m
-        LakeArea        - float,   the area of the lake in m2
-    Path_Connect_Lake_ply            : string (Optional)
-        Path to the connected lake's polygon
-    Path_Non_Connect_Lake_ply        : string (Optional)
-        Path to the non connected lake's polygon
-    Sub_ID                           : string (optional)
-        The column name of the subbasin id in the subbasin polygon
-    Sub_Lake_ID                      : string (optional)
-        The column name of the lake id in the subbasin polygon
-    Lake_Id                          : string (Optional)
-        The the column name in lake polygon indicate the lake ID.
-
-
-    Notes
-    -------
-        None
-
-    Returns:
-    -------
-        Sub_Lake_HRU['OUTPUT']                   : qgis object
-            it is a polygon after overlay between subbasin polygon and
-            lake polygon
-        Sub_Lake_HRU['OUTPUT'].crs().authid()    : string
-            it is a string indicate the geospatial reference used by SubBasin
-            polygon
-        ['HRULake_ID','HRU_IsLake',Sub_ID]       : list
-            it is a string list
-    """
-
-    # Fix geometry errors in subbasin polygon
-#    arcpy.RepairGeometry_management(Path_Subbasin_ply)
-
-    # Create a file name list that will be strored in output attribute table
-    fieldnames_list = [
-        "HRULake_ID",
-        "HRU_IsLake",
-        Lake_Id,
-        Sub_ID,
-        Sub_Lake_ID,
-        "geometry"
-    ]  ### attribubte name in the need to be saved
-    fieldnames = np.array(fieldnames_list)
-
-    # if no lake polygon is provided, use subId as HRULake_ID.
-    if Path_Connect_Lake_ply == "#" and Path_Non_Connect_Lake_ply == "#":
-
-        cat_info = geopandas.read_file(Path_Subbasin_ply)
-        cat_info['Hylak_id'] = -1
-        cat_info['HRULake_ID'] = cat_info.index +1
-        cat_info['HRU_IsLake'] = -1
-
-        # remove column not in fieldnames
-        cat_info = clean_attribute_name_purepy(cat_info,fieldnames)
-        crs_id = cat_info.crs
-        cat_info = cat_info.to_crs(prj_crs)
-        cat_info.to_file(os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'))
-        return os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'), crs_id, ["HRULake_ID", "HRU_IsLake", Sub_ID]
-    else:
-        cat_info = geopandas.read_file(Path_Subbasin_ply)
-
-    # fix lake polygon  geometry
-    if Path_Connect_Lake_ply != "#":
-#        arcpy.RepairGeometry_management(Path_Connect_Lake_ply)
-        cl_lake = geopandas.read_file(Path_Connect_Lake_ply)
-    # fix lake polygon geometry
-    if Path_Non_Connect_Lake_ply != "#":
-#        arcpy.RepairGeometry_management(Path_Non_Connect_Lake_ply)
-        ncl_lake = geopandas.read_file(Path_Non_Connect_Lake_ply)
-
-    # Merge connected and non connected lake polygons first
-    if Path_Connect_Lake_ply != "#" and Path_Non_Connect_Lake_ply != "#":
-        merged_lake_ply = cl_lake.append(ncl_lake)
-#        arcpy.Merge_management([Path_Connect_Lake_ply, Path_Non_Connect_Lake_ply], os.path.join(tempfolder,'merged_lake_ply.shp'))
-    elif Path_Connect_Lake_ply != "#" and Path_Non_Connect_Lake_ply == "#":
-#        arcpy.CopyFeatures_management(Path_Connect_Lake_ply, os.path.join(tempfolder,'merged_lake_ply.shp'))
-        merged_lake_ply = cl_lake
-    elif Path_Connect_Lake_ply == "#" and Path_Non_Connect_Lake_ply != "#":
-#        arcpy.CopyFeatures_management(Path_Non_Connect_Lake_ply, os.path.join(tempfolder,'merged_lake_ply.shp'))
-        merged_lake_ply = ncl_lake
-    else:
-        print("should never happened......")
-
-    # union merged polygon and subbasin polygon
-#    cat_info.spatial.to_featureclass(location=os.path.join(tempfolder,'cat_ply.shp'))
-#    arcpy.RepairGeometry_management(os.path.join(tempfolder,'cat_ply.shp'))
-
-    inFeatures = [[Path_Subbasin_ply, 1], [os.path.join(tempfolder,'merged_lake_ply.shp'), 2]]
-
-    cat_lake_union = geopandas.overlay(cat_info, merged_lake_ply, how='union',make_valid = True,keep_geom_type = True)
-
-#    cat_lake_union.to_file(os.path.join(tempfolder,'cat_lake_union.shp'))
-
-
-#    arcpy.Union_analysis(inFeatures, os.path.join(tempfolder,'cat_lake_union.shp'))
-#    arcpy.RepairGeometry_management(os.path.join(tempfolder,'cat_lake_union.shp'))
-    cat_lake_union = clean_geometry_purepy(cat_lake_union)
-
-    sub_lake_info = cat_lake_union.copy(deep=True)
-    sub_lake_info['HRULake_ID'] = -9999
-    sub_lake_info['HRU_IsLake'] = -9999
-
-    sub_lake_info = sub_lake_info.sort_values(by=['SubId',Lake_Id]).copy(deep=True).reset_index()
-
-    sub_lake_info['HRU_ID_Temp'] = sub_lake_info.index + 1
-
-    sub_lake_info = Determine_Lake_HRU_Id(sub_lake_info)
-    # copy determined lake hru id to vector
-    sub_lake_info = clean_attribute_name_purepy(sub_lake_info,fieldnames)
-    crs_id = sub_lake_info.crs
-    sub_lake_info = sub_lake_info.to_crs(prj_crs)
-    save_modified_attributes_to_outputs(
-        mapoldnew_info = sub_lake_info,
-        tempfolder = tempfolder,
-        OutputFolder = OutputFolder,
-        cat_name = 'finalcat_hru_lake_info.shp',
-        riv_name = '#',
-        Path_final_riv = '#',
-        dis_col_name='HRULake_ID'
-    )
-    return os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'), crs_id, ["HRULake_ID", "HRU_IsLake", Sub_ID]
-
-
-############
-
-
-def Define_HRU_Attributes_purepy(
-    prj_crs,
-    trg_crs,
-    hruinfo,
-    dissolve_filedname_list,
-    Sub_ID,
-    Landuse_ID,
-    Soil_ID,
-    Veg_ID,
-    Other_Ply_ID_1,
-    Other_Ply_ID_2,
-    Landuse_info_data,
-    Soil_info_data,
-    Veg_info_data,
-    DEM,
-    Path_Subbasin_Ply,
-    Inmportance_order,
-    min_hru_area_pct_sub,
-    OutputFolder,
-    tempfolder,
-    area_ratio_thresholds,
-):
-
-    """Generate attributes of each HRU
-
-    Function will generate attributes that are needed by Raven and
-    other hydrological models for each HRU
-
-    Parameters
-    ----------
-    processing                        : qgis object
-    context                           : qgis object
-    Project_crs                       : string
-        the EPSG code of a projected coodinate system that will be used to
-        calcuate HRU area and slope.
-    hru_layer                         : qgis object
-        a polygon layer generated by overlay all input polygons
-    dissolve_filedname_list           : list
-        a list contain column name of ID in each polygon layer
-        in Merge_layer_list
-    Sub_ID                            : string
-        The column name of the subbasin id in the subbasin polygon
-    Landuse_ID                        : string
-        the the column name in landuse polygon and Landuse_info csv
-        indicate the landuse ID. when Path_Landuse_Ply is not
-        provided. The Landuse ID should be
-        1: land, -1: lake.
-    Soil_ID                           : string
-        the the column name in soil polygon and soil_info csv
-        indicate the soil ID. when soil polygon is not
-        provided. The Soil ID in Soil_info should be the same
-        as Landuse ID.
-    Veg_ID                            : string
-        the the column name in vegetation polygon and veg_info csv
-        indicate the vegetation ID. when Veg polygon is not
-        provided. The Veg ID in Veg_info should be the same
-        as Landuse ID.
-
-    Landuse_info                      : Dataframe
-        a dataframe that contains landuse information, including
-        following attributes:
-        Landuse_ID (can be any string)  - integer, the landuse ID in the
-                                                   landuse polygon
-        LAND_USE_C                      - string,  the landuse class name
-                                                   for each landuse Type
-    Soil_info                         : Dataframe
-        a dataframe that contains soil information, including
-        following attributes:
-        Soil_ID (can be any string)     - integer, the Soil ID in the
-                                                   soil polygon
-        SOIL_PROF                       - string,  the Soil profile name
-                                                   for each soil type
-    Veg_info                          : Dataframe
-        a dataframe file that contains vegetation information, including
-        following attributes:
-        Veg_ID (can be any string)      - integer, the vegetation ID in the
-                                                   vegetation polygon
-        VEG_C                           - string,  the vegetation class name
-                                                   for each vegetation Type
-    DEM                               : string (optional)
-        the path to a raster elevation dataset, that will be used to
-        calcuate average apspect, elevation and slope within each HRU.
-        if no data is provided, basin average value will be used for
-        each HRU.
-    Path_Subbasin_Ply                 : string
-        It is the path of the subbasin polygon, which is generated by
-        toolbox. if not generated by toolbox, the attribute table should
-        including following attribute.
-        ##############Subbasin related attributes###########################
-        SubID           - integer, The subbasin Id
-        DowSubId        - integer, The downstream subbasin ID of this
-                                   subbasin
-        IsLake          - integer, If the subbasin is a lake / reservior
-                                   subbasin. 1 yes, <0, no
-        IsObs           - integer, If the subbasin contains a observation
-                                   gauge. 1 yes, < 0 no.
-        RivLength       - float,   The length of the river in current
-                                   subbasin in m
-        RivSlope        - float,   The slope of the river path in
-                                   current subbasin, in m/m
-        FloodP_n        - float,   Flood plain manning's coefficient, in -
-        Ch_n            - float,   main channel manning's coefficient, in -
-        BkfWidth        - float,   the bankfull width of the main channel
-                                   in m
-        BkfDepth        - float,   the bankfull depth of the main channel
-                                   in m
-        HyLakeId        - integer, the lake id
-        LakeVol         - float,   the Volume of the lake in km3
-        LakeDepth       - float,   the average depth of the lake m
-        LakeArea        - float,   the area of the lake in m2
-    OutputFolder                      : String
-        The path to a folder to save result during the processing
-
-    Returns:
-    -------
-    HRU_draf_final                  : qgis object
-        it is a polygon object that generated by overlay all input
-        layers and inlcude all needed attribue for hydrological model
-        like RAVEN
-    """
-    num = str(np.random.randint(1, 10000 + 1))
-    hruinfo["LAND_USE_C"] = '-9999'
-    hruinfo["VEG_C"] = '-9999'
-    hruinfo["SOIL_PROF"] = '-9999'
-    hruinfo["HRU_CenX"] = -9999.9999
-    hruinfo["HRU_CenY"] = -9999.9999
-    hruinfo["HRU_ID_New"] = -9999
-    hruinfo["HRU_Area"] = -9999.99
-
-    hruinfo_area = add_area_in_m2(hruinfo,prj_crs,'HRU_Area')
-
-    hruinfo_area = simplify_hrus_method2(area_ratio_thresholds,hruinfo_area, Landuse_ID,
-                          Soil_ID,Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2)
-
-    hruinfo_area = hruinfo_area.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
-
-
-    hruinfo_area['HRU_ID'] = hruinfo_area.index + 1
-    hruinfo_area["HRU_ID_New"] = hruinfo_area.index + 1
-
-    hruinfo_area_update_attribute = Determine_HRU_Attributes(
-        hruinfo_area,
-        Sub_ID,
-        Landuse_ID,
-        Soil_ID,
-        Veg_ID,
-        Other_Ply_ID_1,
-        Other_Ply_ID_2,
-        Landuse_info_data,
-        Soil_info_data,
-        Veg_info_data,
-    )
-
-    hruinfo_new = save_modified_attributes_to_outputs(
-        mapoldnew_info = hruinfo_area_update_attribute,
-        tempfolder = tempfolder,
-        OutputFolder = tempfolder,
-        cat_name = 'finalcat_hru_info.shp',
-        riv_name = '#',
-        Path_final_riv = '#',
-        dis_col_name='HRU_ID_New'
-    )
-    hruinfo_new = add_area_in_m2(hruinfo_new,prj_crs,'HRU_Area')
-#    print(len(hruinfo_area_update_attribute),len(hruinfo_new))
-    hruinfo_simple = hruinfo_new
-    # if len(Inmportance_order) > 0:
-    #     hruinfo_simple = simplidfy_hrus(
-    #         min_hru_pct_sub_area = min_hru_area_pct_sub,
-    #         hruinfo = hruinfo_new,
-    #         importance_order = Inmportance_order,
-    #     )
-    # else:
-    #     hruinfo_simple = hruinfo_new
-    #
-    # hruinfo_simple = clean_geometry_purepy(hruinfo_simple,set_precision = -1)
-    #
-    # hruinfo_simple = save_modified_attributes_to_outputs(
-    #     mapoldnew_info = hruinfo_simple,
-    #     tempfolder = tempfolder,
-    #     OutputFolder = tempfolder,
-    #     cat_name = 'hru_simple.shp',
-    #     riv_name = '#',
-    #     Path_final_riv = '#',
-    #     dis_col_name='HRU_ID_New'
-    # )
-
-    hruinfo_simple = add_centroid_in_wgs84(hruinfo_simple,"HRU_CenX","HRU_CenY")
-
-    cat_info = geopandas.read_file(Path_Subbasin_Ply)
-    cat_info = cat_info.drop(columns = 'geometry').copy(deep=True)
-
-    hruinfo_simple = pd.merge(hruinfo_simple, cat_info, on='SubId', how='left')
-
-    hruinfo_simple = add_area_in_m2(hruinfo_simple,prj_crs,'HRU_Area')
-#    print(len(hruinfo_simple))
-    if DEM != "#":
-
-        hru_proj= hruinfo_simple.to_crs(prj_crs)
-        hru_proj.to_file(os.path.join(tempfolder,"hru_proj.shp"))
-        proj_clip_raster(DEM,os.path.join(tempfolder,"demproj.tif"),prj_crs)
-#        proj_clip_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demclip.tif"),prj_crs,os.path.join(tempfolder,"hru_proj.shp"))
-        gdal_slope_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demslope.tif"))
-        gdal_aspect_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demaspect.tif"))
-
-        table_elv = ZonalStats(hru_proj, os.path.join(tempfolder,"demproj.tif"), 'mean','HRU_ID_New','MeanElev')
-        table_asp = ZonalStats(hru_proj, os.path.join(tempfolder,"demaspect.tif"), 'mean','HRU_ID_New','BasAspect')
-        table_slp = ZonalStats(hru_proj, os.path.join(tempfolder,"demslope.tif"), 'mean','HRU_ID_New','BasSlope')
-
-        table_slp['HRU_S_mean'] = table_slp['mean']
-        table_slp = table_slp[['HRU_ID_New','HRU_S_mean']]
-        table_asp['HRU_A_mean'] = table_asp['mean']
-        table_asp = table_asp[['HRU_ID_New','HRU_A_mean']]
-        table_elv['HRU_E_mean'] = table_elv['mean']
-        table_elv = table_elv[['HRU_ID_New','HRU_E_mean']]
-        hru_proj = pd.merge(hru_proj, table_slp, on='HRU_ID_New')
-        hru_proj = pd.merge(hru_proj, table_asp, on='HRU_ID_New')
-        hru_proj = pd.merge(hru_proj, table_elv, on='HRU_ID_New')
-        hruinfo_add_slp_asp = hru_proj.to_crs(trg_crs)
-        hruinfo_add_slp_asp = hruinfo_add_slp_asp.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
-        hruinfo_add_slp_asp['HRU_ID'] = hruinfo_add_slp_asp.index + 1
-#        print(len(hruinfo_add_slp_asp))
-    else:
-
-        hruinfo_add_slp_asp = hruinfo_simple.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
-        hruinfo_add_slp_asp['HRU_ID'] = hruinfo_add_slp_asp.index + 1
-        hruinfo_add_slp_asp['HRU_S_mean'] = hruinfo_add_slp_asp['BasSlope']
-        hruinfo_add_slp_asp['HRU_A_mean'] = hruinfo_add_slp_asp['BasAspect']
-        hruinfo_add_slp_asp['HRU_E_mean'] = hruinfo_add_slp_asp['MeanElev']
-
-    hruinfo_add_slp_asp = adjust_HRUs_area_based_on_ply_sub_area(hruinfo_add_slp_asp)
-
-    hruinfo_add_slp_asp = clean_geometry_purepy(hruinfo_add_slp_asp,set_precision = 1)
-#    print(len(hruinfo_add_slp_asp))
-    return hruinfo_add_slp_asp
-
-def adjust_HRUs_area_based_on_ply_sub_area(hruinfo):
-    hruinfo['HRU_A_G'] =hruinfo ['HRU_Area']
-    subinfo = hruinfo[['SubId','HRU_Area']].copy(deep=True)
-    subinfo = subinfo.rename(columns={"HRU_Area": "Bas_A_G"})
-
-    subinfo = subinfo.groupby(['SubId'],as_index = False).sum()
-    hruinfo = pd.merge(hruinfo, subinfo, on='SubId')
-    hruinfo['Ratio_A'] = hruinfo['BasArea']/hruinfo['Bas_A_G']
-    hruinfo['HRU_Area'] = hruinfo['HRU_A_G'] * hruinfo['Ratio_A']
-
-    return hruinfo
+import numpy as np
+import sys
+import os
+import csv
+import tempfile
+import copy
+import pandas as pd
+import geopandas
+import sys, os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from basinmaker.func.purepy import *
+from basinmaker.func.pdtable import *
+from osgeo import gdal, ogr
+from basinmaker.func.fgdal import *
+from basinmaker.utilities.utilities import *
+
+def GenerateHRUS_purepy(
+    Path_Subbasin_Ply,
+    Landuse_info,
+    Soil_info,
+    Veg_info,
+    Inmportance_order,
+    min_hru_area_pct_sub,
+    Sub_Lake_ID="HyLakeId",
+    Sub_ID="SubId",
+    Path_Connect_Lake_ply="#",
+    Path_Non_Connect_Lake_ply="#",
+    Lake_Id="Hylak_id",
+    Path_Landuse_Ply="#",
+    Landuse_ID="Landuse_ID",
+    Path_Soil_Ply="#",
+    Soil_ID="Soil_ID",
+    Path_Veg_Ply="#",
+    Veg_ID="Veg_ID",
+    Path_Other_Ply_1="#",
+    Other_Ply_ID_1="O_ID_1",
+    Path_Other_Ply_2="#",
+    Other_Ply_ID_2="O_ID_2",
+    DEM="#",
+    Project_crs = '3573',
+    OutputFolder="#",
+    pixel_size = 30,
+    area_ratio_thresholds = [0,0,0],
+):
+    """Generate HRU polygons and their attributes needed by hydrological model
+
+    Function that be used to overlay: subbasin polygon, lake polygon (optional)
+    , Land use polygon (optional), soil type polygon(optional),
+    vegetation polygon (optional), and two other user defined polygons
+    (optional).
+    Non-lake HRU polygons in a subbasin is defined by an unique
+    combination of all user provided datasets.
+    A lake HRU polygon is defined the same as the provided lake polygon.
+    All value of landuse and Veg polygon covered by lake will
+    be changed to 1, indicating it is a covered by lake.
+    All value of the soil polygon covered by the lake will be change to
+    the soil id of the polygon covered by the lake with largest area.
+
+    Parameters
+    ----------
+    Path_Subbasin_Ply                 : string
+        It is the path of the subbasin polygon, which is generated by
+        toolbox. if not generated by toolbox, the attribute table should
+        including following attribute.
+        ##############Subbasin related attributes###########################
+        SubID           - integer, The subbasin Id
+        DowSubId        - integer, The downstream subbasin ID of this
+                                   subbasin
+        IsLake          - integer, If the subbasin is a lake / reservior
+                                   subbasin. 1 yes, <0, no
+        IsObs           - integer, If the subbasin contains a observation
+                                   gauge. 1 yes, < 0 no.
+        RivLength       - float,   The length of the river in current
+                                   subbasin in m
+        RivSlope        - float,   The slope of the river path in
+                                   current subbasin, in m/m
+        FloodP_n        - float,   Flood plain manning's coefficient, in -
+        Ch_n            - float,   main channel manning's coefficient, in -
+        BkfWidth        - float,   the bankfull width of the main channel
+                                   in m
+        BkfDepth        - float,   the bankfull depth of the main channel
+                                   in m
+        HyLakeId        - integer, the lake id
+        LakeVol         - float,   the Volume of the lake in km3
+        LakeDepth       - float,   the average depth of the lake m
+        LakeArea        - float,   the area of the lake in m2
+    Landuse_info                      : string
+        Path to a csv file that contains landuse information, including
+        following attributes:
+        Landuse_ID (can be any string)  - integer, the landuse ID in the
+                                                   landuse polygon
+        LAND_USE_C                      - string,  the landuse class name
+                                                   for each landuse Type
+    Soil_info                        : string
+        Path to a csv file that contains soil information, including
+        following attributes:
+        Soil_ID (can be any string)     - integer, the Soil ID in the
+                                                   soil polygon
+        SOIL_PROF                       - string,  the Soil profile name
+                                                   for each soil type
+    Veg_info                         : string
+        Path to a csv file that contains vegetation information, including
+        following attributes:
+        Veg_ID (can be any string)      - integer, the vegetation ID in the
+                                                   vegetation polygon
+        VEG_C                           - string,  the vegetation class name
+                                                   for each vegetation Type
+    Sub_Lake_ID                      : string (optional)
+        The column name of the lake id in the subbasin polygon
+    Sub_ID                           : string (optional)
+        The column name of the subbasin id in the subbasin polygon
+    Path_Connect_Lake_ply            : string (Optional)
+        Path to the connected lake's polygon
+    Path_Non_Connect_Lake_ply        : string (Optional)
+        Path to the non connected lake's polygon
+    Lake_Id                          : string (Optional)
+        The the column name in lake polygon indicate the lake ID.
+    Path_Landuse_Ply                 : string (Optional)
+        Path to the landuse polygon. when Path_Landuse_Ply is not
+        provided. The Landuse ID in Landuse_info should be
+        1: land, -1: lake
+    Landuse_ID                       : string (Optional)
+        the the column name in landuse polygon and Landuse_info csv
+        indicate the landuse ID. when Path_Landuse_Ply is not
+        provided. The Landuse ID should be
+        1: land, -1: lake.
+    Path_Soil_Ply                    : string (Optional)
+        Path to the soil polygon. when soil polygon is not
+        provided. The Soil ID in Soil_info should be the same
+        as Landuse ID.
+    Soil_ID                          : string (Optional)
+        the the column name in soil polygon and soil_info csv
+        indicate the soil ID. when soil polygon is not
+        provided. The Soil ID in Soil_info should be the same
+        as Landuse ID.
+    Path_Veg_Ply                     : string (Optional)
+        Path to the vegetation polygon. when Veg polygon is not
+        provided. The Veg ID in Veg_info should be the same
+        as Landuse ID.
+    Veg_ID                           : string (Optional)
+        the the column name in vegetation polygon and veg_info csv
+        indicate the vegetation ID. when Veg polygon is not
+        provided. The Veg ID in Veg_info should be the same
+        as Landuse ID.
+    Path_Other_Ply_1                 : string (Optional)
+        Path to the other polygon that will be used to define HRU,
+        such as elevation band, or aspect.
+    Other_Ply_ID_1                   : string (Optional)
+        the the column name in Other_Ply_1 polygon
+        indicate the landuse ID.
+    Path_Other_Ply_2                 : string (Optional)
+        Path to the other polygon that will be used to define HRU,
+        such as elevation band, or aspect.
+    Other_Ply_ID_2                   : string (Optional)
+        the the column name in Other_Ply_2 polygon
+        indicate the landuse ID.
+    DEM                              : string (optional)
+        the path to a raster elevation dataset, that will be used to
+        calcuate average apspect, elevation and slope within each HRU.
+        if no data is provided, basin average value will be used for
+        each HRU.
+    Project_crs                      : string
+        the EPSG code of a projected coodinate system that will be used to
+        calcuate HRU area and slope.
+    OutputFolder                     : string
+        The path to the folder that will save output HRU polygon.
+
+    Notes
+    -------
+    Following ouput files will be generated in "<OutputFolder>/"
+    'finalcat_hru_info.shp'              - HRU polygon and it's attributes
+
+
+    Returns:
+    -------
+       None
+
+    Examples
+    -------
+    >>> from ToolboxClass import LRRT
+    >>> import pandas as pd
+    >>> DataFolder = "C:/Path_to_foldr_of_example_dataset_provided_in_Github_wiki/"
+    >>> RTtool=LRRT()
+    >>> RTtool.GenerateHRUS(OutputFolder = DataFolder,
+                           Path_Subbasin_Ply = os.path.join(DataFolder,"finalcat_info.shp"),
+                           Path_Connect_Lake_ply = os.path.join(DataFolder,'Con_Lake_Ply.shp'),
+                           Path_Non_Connect_Lake_ply = os.path.join(DataFolder,'Non_Con_Lake_Ply.shp'),
+                           Path_Landuse_Ply = os.path.join(DataFolder,'modislanduse_exp_lg_pre.shp'),
+                           Landuse_ID = 'gridcode',
+                           Path_Soil_Ply = os.path.join(DataFolder,'ca_all_slc_v3r2_exp_lg.shp'),
+                           Soil_ID = 'POLY_ID',
+                           Landuse_info=os.path.join(DataFolder,'landuse_info.csv'),
+                           Soil_info=os.path.join(DataFolder,'soil_info.csv'),
+                           Veg_info=os.path.join(DataFolder,'veg_info.csv'),
+                           DEM = os.path.join(DataFolder,'na_dem_15s_1.tif')
+                           )
+
+    """
+
+    if not os.path.exists(OutputFolder):
+        os.makedirs(OutputFolder)
+
+    tempfolder = os.path.join(
+        OutputFolder, "HRU_TEMP" + str(np.random.randint(1, 10000 + 1))
+    )
+    if not os.path.exists(tempfolder):
+        os.makedirs(tempfolder)
+
+    prj_crs = Project_crs
+    Merge_layer_list = []
+    Merge_layer_raster_list = []
+    Merge_layer_shp_list = []
+    Merge_ID_list = []
+
+    copy_files_with_extension(os.path.dirname(Path_Subbasin_Ply),OutputFolder,"*.geojson")
+
+    Sub_Lake_HRU_Layer, trg_crs, fieldnames_list = GeneratelandandlakeHRUS(
+        OutputFolder,
+        tempfolder,
+        Path_Subbasin_ply=Path_Subbasin_Ply,
+        Path_Connect_Lake_ply=Path_Connect_Lake_ply,
+        Path_Non_Connect_Lake_ply=Path_Non_Connect_Lake_ply,
+        Sub_ID=Sub_ID,
+        Sub_Lake_ID=Sub_Lake_ID,
+        Lake_Id=Lake_Id,
+        prj_crs = prj_crs,
+    )
+
+    lakehruinfo = geopandas.read_file(Sub_Lake_HRU_Layer)
+    hru_lake_info = lakehruinfo.loc[lakehruinfo['HRU_IsLake'] > 0].copy()
+    lakehruinfo_landhrus = lakehruinfo.loc[lakehruinfo['HRU_IsLake'] <= 0].copy()
+
+    hru_lake_info = hru_lake_info.to_crs(prj_crs)
+    lakehruinfo_landhrus = lakehruinfo_landhrus.to_crs(prj_crs)
+    lakehruinfo = lakehruinfo.to_crs(prj_crs)
+
+    hru_lake_info = clean_geometry_purepy(hru_lake_info)
+    lakehruinfo_landhrus = clean_geometry_purepy(lakehruinfo_landhrus)
+
+    path_to_landhru_shp= os.path.join(tempfolder,'land_hru.shp')
+    path_to_lakehru_shp= os.path.join(tempfolder,'lake_hru.shp')
+    path_to_landuse_shp = os.path.join(tempfolder,'landuse.shp')
+    path_to_soil_shp = os.path.join(tempfolder,'soil.shp')
+    path_to_veg_shp = os.path.join(tempfolder,'veg.shp')
+    path_to_other1_shp = os.path.join(tempfolder,'o1.shp')
+    path_to_other2_shp = os.path.join(tempfolder,'o2.shp')
+
+
+#    lakehruinfo_landhrus.to_file(path_to_landhru_shp)
+    if len(hru_lake_info) > 0:
+        hru_lake_info.to_file(path_to_lakehru_shp)
+
+    if len(lakehruinfo_landhrus) > 0:
+        lakehruinfo_landhrus.to_file(path_to_landhru_shp)
+
+    fieldnames_list.extend(
+        [
+            Landuse_ID,
+            Soil_ID,
+            Veg_ID,
+            Other_Ply_ID_1,
+            Other_Ply_ID_2,
+            "LAND_USE_C",
+            "VEG_C",
+            "SOIL_PROF",
+            "HRU_Slope",
+            "HRU_Area",
+            "HRU_Aspect",
+            "geometry",
+        ]
+    )
+    dissolve_filedname_list = ["HRULake_ID"]
+
+    Merge_layer_list.append(lakehruinfo_landhrus)
+
+    Landuse_info_data = pd.read_csv(Landuse_info)
+    Soil_info_data = pd.read_csv(Soil_info)
+    Veg_info_data = pd.read_csv(Veg_info)
+
+
+    #### check which data will be inlucded to determine HRU
+    if Path_Landuse_Ply != "#":
+        land_landuse_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+            layer_path = Path_Landuse_Ply,
+            Class_Col = Landuse_ID,
+            tempfolder = tempfolder,
+            mask_layer = lakehruinfo,
+            Class_NM_Col = "LAND_USE_C",
+            info_table = Landuse_info_data,
+        )
+
+        if Landuse_ID not in land_landuse_clean.columns:
+            print("Landuse polygon attribute table do not contain: ",Landuse_ID)
+            sys.exit()
+        land_landuse_clean.to_file(path_to_landuse_shp)
+
+        dissolve_filedname_list.append(Landuse_ID)
+        Merge_layer_shp_list.append(path_to_landuse_shp)
+        Merge_ID_list.append(Landuse_ID)
+
+    if Path_Soil_Ply != "#":
+        land_soil_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+            layer_path = Path_Soil_Ply,
+            Class_Col = Soil_ID,
+            tempfolder = tempfolder,
+            mask_layer = lakehruinfo,
+            Class_NM_Col = "SOIL_PROF",
+            info_table = Soil_info_data,
+        )
+
+        if Soil_ID not in land_soil_clean.columns:
+            print("Soil polygon attribute table do not contain: ",Soil_ID)
+            sys.exit()
+        land_soil_clean.to_file(path_to_soil_shp)
+        dissolve_filedname_list.append(Soil_ID)
+        Merge_layer_shp_list.append(path_to_soil_shp)
+        Merge_ID_list.append(Soil_ID)
+
+    if Path_Veg_Ply != "#":
+        land_veg_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+            layer_path = Path_Veg_Ply,
+            Class_Col = Veg_ID,
+            tempfolder = tempfolder,
+            mask_layer = lakehruinfo
+        )
+
+        if Veg_ID not in land_veg_clean.columns:
+            print("Veg polygon attribute table do not contain: ",Veg_ID)
+            sys.exit()
+        land_veg_clean.to_file(path_to_veg_shp)
+        dissolve_filedname_list.append(Veg_ID)
+        Merge_layer_shp_list.append(path_to_veg_shp)
+        Merge_ID_list.append(Veg_ID)
+
+
+    if Path_Other_Ply_1 != "#":
+        land_o1_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+            layer_path = Path_Other_Ply_1,
+            Class_Col = Other_Ply_ID_1,
+            tempfolder = tempfolder,
+            mask_layer = lakehruinfo
+        )
+
+        if Other_Ply_ID_1 not in land_o1_clean.columns:
+            print("Other_Ply_1 polygon attribute table do not contain: ",Other_Ply_ID_1)
+            sys.exit()
+        land_o1_clean.to_file(path_to_other1_shp)
+        dissolve_filedname_list.append(Other_Ply_ID_1)
+        Merge_layer_shp_list.append(path_to_other1_shp)
+        Merge_ID_list.append(Other_Ply_ID_1)
+
+    if Path_Other_Ply_2 != "#":
+        land_o2_clean = Reproj_Clip_Dissolve_Simplify_Polygon_purepy(
+            layer_path = Path_Other_Ply_2,
+            Class_Col = Other_Ply_ID_2,
+            tempfolder = tempfolder,
+            mask_layer = lakehruinfo
+        )
+
+        if Other_Ply_ID_2 not in land_o2_clean.columns:
+            print("Other_Ply_1 polygon attribute table do not contain: ",Other_Ply_ID_2)
+            sys.exit()
+        land_o2_clean.to_file(path_to_other2_shp)
+        dissolve_filedname_list.append(Other_Ply_ID_2)
+        Merge_layer_shp_list.append(path_to_other2_shp)
+        Merge_ID_list.append(Other_Ply_ID_2)
+
+    fieldnames = np.array(fieldnames_list)
+
+
+    path_to_hru_temp_shp = RasterHRUUnionInt32(OutputFolder,tempfolder,Merge_layer_shp_list,
+                            Merge_ID_list,Sub_Lake_HRU_Layer,Sub_ID,
+                            Landuse_ID,Soil_ID,Veg_ID,Other_Ply_ID_1,
+                            Other_Ply_ID_2,pixel_size,lakehruinfo)
+
+    HRU_temp1 = geopandas.read_file(path_to_hru_temp_shp)
+
+    HRU_temp1 = decode_hru_attri_ids(HRU_temp1,lakehruinfo,Landuse_ID,Soil_ID,
+                                     Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2)
+
+    HRU_temp1.to_file(os.path.join(tempfolder,'HRU_DEDOCE.shp'))
+    #####
+    hru_lake_info = HRU_temp1.loc[HRU_temp1['HRU_IsLake'] > 0].copy()
+    hru_land_info = HRU_temp1.loc[HRU_temp1['HRU_IsLake'] <= 0].copy()
+
+    # landuse polygon is not provided,landused id the same as IS_lake
+    if Path_Landuse_Ply == "#":
+        hru_land_info[Landuse_ID] = -hru_land_info['HRU_IsLake']
+    hru_lake_info[Landuse_ID] = -1
+    # if soil is not provied, it the value,will be the same as land use
+    if Path_Soil_Ply == "#":
+        hru_land_info[Soil_ID] = -hru_land_info['HRU_IsLake']
+    hru_lake_info[Soil_ID] = -1
+    # if no vegetation polygon is provide vegetation, will be the same as landuse
+    if Path_Veg_Ply == "#":
+        hru_land_info[Veg_ID] = hru_land_info[Landuse_ID]
+    hru_lake_info[Veg_ID] = -1
+    if Path_Other_Ply_1 == "#":
+        hru_land_info[Other_Ply_ID_1] = -hru_land_info['HRU_IsLake']
+    hru_lake_info[Other_Ply_ID_1] = -1
+    if Path_Other_Ply_2 == "#":
+        hru_land_info[Other_Ply_ID_2] = -hru_land_info['HRU_IsLake']
+    hru_lake_info[Other_Ply_ID_2] = -1
+
+    hru_lake_info = clean_attribute_name_purepy(hru_lake_info,fieldnames)
+    hru_land_info = clean_attribute_name_purepy(hru_land_info,fieldnames)
+
+
+    hruinfo = hru_lake_info.append(hru_land_info)
+
+    hruinfo.to_file(os.path.join(tempfolder,'HRU_with_attributes.shp'))
+
+
+    HRU_draf_final = Define_HRU_Attributes_purepy(
+        prj_crs = prj_crs,
+        trg_crs = trg_crs,
+        hruinfo = hruinfo,
+        dissolve_filedname_list = dissolve_filedname_list,
+        Sub_ID = Sub_ID,
+        Landuse_ID = Landuse_ID,
+        Soil_ID = Soil_ID,
+        Veg_ID = Veg_ID,
+        Other_Ply_ID_1 = Other_Ply_ID_1,
+        Other_Ply_ID_2 = Other_Ply_ID_2,
+        Landuse_info_data = Landuse_info_data,
+        Soil_info_data = Soil_info_data,
+        Veg_info_data = Veg_info_data,
+        DEM = DEM,
+        Path_Subbasin_Ply = Path_Subbasin_Ply,
+        min_hru_area_pct_sub = min_hru_area_pct_sub,
+        Inmportance_order = Inmportance_order,
+        OutputFolder = OutputFolder,
+        tempfolder = tempfolder,
+        area_ratio_thresholds = area_ratio_thresholds,
+    )
+
+    COLUMN_NAMES_CONSTANT_HRU_extend = COLUMN_NAMES_CONSTANT_HRU.extend(
+        [
+            Landuse_ID,
+            Soil_ID,
+            Veg_ID,
+            Other_Ply_ID_1,
+            Other_Ply_ID_2,
+            'geometry',
+            'HRU_A_G'
+        ]
+    )
+    HRU_draf_final = clean_attribute_name_purepy(HRU_draf_final,COLUMN_NAMES_CONSTANT_HRU)
+    for col in [Landuse_ID,Soil_ID,Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2,'SubId']:
+        HRU_draf_final = HRU_draf_final.loc[HRU_draf_final[col] != 0]
+
+    HRU_draf_final.to_crs(trg_crs)
+    HRU_draf_final.to_file(os.path.join(OutputFolder,'finalcat_hru_info.shp'))
+    HRU_draf_final_wgs_84 = HRU_draf_final.to_crs('EPSG:4326')
+#    HRU_draf_final_wgs_84 = HRU_draf_final_wgs_84[['HRU_ID','geometry']]
+    TOLERANCEs = [0.0001,0.0005,0.001,0.005,0.01,0.05]
+    output_jason_path = os.path.join(OutputFolder,'finalcat_hru_info.geojson')
+    for TOLERANCE in TOLERANCEs:
+        HRU_draf_final_wgs_84['geometry'] = HRU_draf_final_wgs_84.simplify(TOLERANCE)
+        HRU_draf_final_wgs_84.to_file(output_jason_path,driver="GeoJSON")
+
+        json_file_size = os.stat(output_jason_path).st_size/1024/1024 #to MB
+        if json_file_size <= 100:
+            break
+
+
+def GeneratelandandlakeHRUS(
+    OutputFolder,
+    tempfolder,
+    Path_Subbasin_ply,
+    Path_Connect_Lake_ply="#",
+    Path_Non_Connect_Lake_ply="#",
+    Sub_ID="SubId",
+    Sub_Lake_ID="HyLakeId",
+    Lake_Id="Hylak_id",
+    prj_crs = "EPSG:3161",
+):
+
+    """Overlay subbasin polygon and lake polygons
+
+    Function that will overlay subbasin polygon and lake polygon
+
+    Parameters
+    ----------
+    processing                        : qgis object
+    context                           : qgis object
+    OutputFolder                     : string
+        The path to the folder that will save output HRU polygon.
+
+    Path_Subbasin_Ply                 : string
+        It is the path of the subbasin polygon, which is generated by
+        toolbox. if not generated by toolbox, the attribute table should
+        including following attribute.
+        ##############Subbasin related attributes###########################
+        SubID           - integer, The subbasin Id
+        DowSubId        - integer, The downstream subbasin ID of this
+                                   subbasin
+        IsLake          - integer, If the subbasin is a lake / reservior
+                                   subbasin. 1 yes, <0, no
+        IsObs           - integer, If the subbasin contains a observation
+                                   gauge. 1 yes, < 0 no.
+        RivLength       - float,   The length of the river in current
+                                   subbasin in m
+        RivSlope        - float,   The slope of the river path in
+                                   current subbasin, in m/m
+        FloodP_n        - float,   Flood plain manning's coefficient, in -
+        Ch_n            - float,   main channel manning's coefficient, in -
+        BkfWidth        - float,   the bankfull width of the main channel
+                                   in m
+        BkfDepth        - float,   the bankfull depth of the main channel
+                                   in m
+        HyLakeId        - integer, the lake id
+        LakeVol         - float,   the Volume of the lake in km3
+        LakeDepth       - float,   the average depth of the lake m
+        LakeArea        - float,   the area of the lake in m2
+    Path_Connect_Lake_ply            : string (Optional)
+        Path to the connected lake's polygon
+    Path_Non_Connect_Lake_ply        : string (Optional)
+        Path to the non connected lake's polygon
+    Sub_ID                           : string (optional)
+        The column name of the subbasin id in the subbasin polygon
+    Sub_Lake_ID                      : string (optional)
+        The column name of the lake id in the subbasin polygon
+    Lake_Id                          : string (Optional)
+        The the column name in lake polygon indicate the lake ID.
+
+
+    Notes
+    -------
+        None
+
+    Returns:
+    -------
+        Sub_Lake_HRU['OUTPUT']                   : qgis object
+            it is a polygon after overlay between subbasin polygon and
+            lake polygon
+        Sub_Lake_HRU['OUTPUT'].crs().authid()    : string
+            it is a string indicate the geospatial reference used by SubBasin
+            polygon
+        ['HRULake_ID','HRU_IsLake',Sub_ID]       : list
+            it is a string list
+    """
+
+    # Fix geometry errors in subbasin polygon
+#    arcpy.RepairGeometry_management(Path_Subbasin_ply)
+
+    # Create a file name list that will be strored in output attribute table
+    fieldnames_list = [
+        "HRULake_ID",
+        "HRU_IsLake",
+        Lake_Id,
+        Sub_ID,
+        Sub_Lake_ID,
+        "geometry"
+    ]  ### attribubte name in the need to be saved
+    fieldnames = np.array(fieldnames_list)
+
+    # if no lake polygon is provided, use subId as HRULake_ID.
+    if Path_Connect_Lake_ply == "#" and Path_Non_Connect_Lake_ply == "#":
+
+        cat_info = geopandas.read_file(Path_Subbasin_ply)
+        cat_info['Hylak_id'] = -1
+        cat_info['HRULake_ID'] = cat_info.index +1
+        cat_info['HRU_IsLake'] = -1
+
+        # remove column not in fieldnames
+        cat_info = clean_attribute_name_purepy(cat_info,fieldnames)
+        crs_id = cat_info.crs
+        cat_info = cat_info.to_crs(prj_crs)
+        cat_info.to_file(os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'))
+        return os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'), crs_id, ["HRULake_ID", "HRU_IsLake", Sub_ID]
+    else:
+        cat_info = geopandas.read_file(Path_Subbasin_ply)
+
+    # fix lake polygon  geometry
+    if Path_Connect_Lake_ply != "#":
+#        arcpy.RepairGeometry_management(Path_Connect_Lake_ply)
+        cl_lake = geopandas.read_file(Path_Connect_Lake_ply)
+    # fix lake polygon geometry
+    if Path_Non_Connect_Lake_ply != "#":
+#        arcpy.RepairGeometry_management(Path_Non_Connect_Lake_ply)
+        ncl_lake = geopandas.read_file(Path_Non_Connect_Lake_ply)
+
+    # Merge connected and non connected lake polygons first
+    if Path_Connect_Lake_ply != "#" and Path_Non_Connect_Lake_ply != "#":
+        merged_lake_ply = cl_lake.append(ncl_lake)
+#        arcpy.Merge_management([Path_Connect_Lake_ply, Path_Non_Connect_Lake_ply], os.path.join(tempfolder,'merged_lake_ply.shp'))
+    elif Path_Connect_Lake_ply != "#" and Path_Non_Connect_Lake_ply == "#":
+#        arcpy.CopyFeatures_management(Path_Connect_Lake_ply, os.path.join(tempfolder,'merged_lake_ply.shp'))
+        merged_lake_ply = cl_lake
+    elif Path_Connect_Lake_ply == "#" and Path_Non_Connect_Lake_ply != "#":
+#        arcpy.CopyFeatures_management(Path_Non_Connect_Lake_ply, os.path.join(tempfolder,'merged_lake_ply.shp'))
+        merged_lake_ply = ncl_lake
+    else:
+        print("should never happened......")
+
+    # union merged polygon and subbasin polygon
+#    cat_info.spatial.to_featureclass(location=os.path.join(tempfolder,'cat_ply.shp'))
+#    arcpy.RepairGeometry_management(os.path.join(tempfolder,'cat_ply.shp'))
+
+    inFeatures = [[Path_Subbasin_ply, 1], [os.path.join(tempfolder,'merged_lake_ply.shp'), 2]]
+
+    cat_lake_union = geopandas.overlay(cat_info, merged_lake_ply, how='union',make_valid = True,keep_geom_type = True)
+
+#    cat_lake_union.to_file(os.path.join(tempfolder,'cat_lake_union.shp'))
+
+
+#    arcpy.Union_analysis(inFeatures, os.path.join(tempfolder,'cat_lake_union.shp'))
+#    arcpy.RepairGeometry_management(os.path.join(tempfolder,'cat_lake_union.shp'))
+    cat_lake_union = clean_geometry_purepy(cat_lake_union)
+
+    sub_lake_info = cat_lake_union.copy(deep=True)
+    sub_lake_info['HRULake_ID'] = -9999
+    sub_lake_info['HRU_IsLake'] = -9999
+
+    sub_lake_info = sub_lake_info.sort_values(by=['SubId',Lake_Id]).copy(deep=True).reset_index()
+
+    sub_lake_info['HRU_ID_Temp'] = sub_lake_info.index + 1
+
+    sub_lake_info = Determine_Lake_HRU_Id(sub_lake_info)
+    # copy determined lake hru id to vector
+    sub_lake_info = clean_attribute_name_purepy(sub_lake_info,fieldnames)
+    crs_id = sub_lake_info.crs
+    sub_lake_info = sub_lake_info.to_crs(prj_crs)
+    save_modified_attributes_to_outputs(
+        mapoldnew_info = sub_lake_info,
+        tempfolder = tempfolder,
+        OutputFolder = OutputFolder,
+        cat_name = 'finalcat_hru_lake_info.shp',
+        riv_name = '#',
+        Path_final_riv = '#',
+        dis_col_name='HRULake_ID'
+    )
+    return os.path.join(OutputFolder,'finalcat_hru_lake_info.shp'), crs_id, ["HRULake_ID", "HRU_IsLake", Sub_ID]
+
+
+############
+
+
+def Define_HRU_Attributes_purepy(
+    prj_crs,
+    trg_crs,
+    hruinfo,
+    dissolve_filedname_list,
+    Sub_ID,
+    Landuse_ID,
+    Soil_ID,
+    Veg_ID,
+    Other_Ply_ID_1,
+    Other_Ply_ID_2,
+    Landuse_info_data,
+    Soil_info_data,
+    Veg_info_data,
+    DEM,
+    Path_Subbasin_Ply,
+    Inmportance_order,
+    min_hru_area_pct_sub,
+    OutputFolder,
+    tempfolder,
+    area_ratio_thresholds,
+):
+
+    """Generate attributes of each HRU
+
+    Function will generate attributes that are needed by Raven and
+    other hydrological models for each HRU
+
+    Parameters
+    ----------
+    processing                        : qgis object
+    context                           : qgis object
+    Project_crs                       : string
+        the EPSG code of a projected coodinate system that will be used to
+        calcuate HRU area and slope.
+    hru_layer                         : qgis object
+        a polygon layer generated by overlay all input polygons
+    dissolve_filedname_list           : list
+        a list contain column name of ID in each polygon layer
+        in Merge_layer_list
+    Sub_ID                            : string
+        The column name of the subbasin id in the subbasin polygon
+    Landuse_ID                        : string
+        the the column name in landuse polygon and Landuse_info csv
+        indicate the landuse ID. when Path_Landuse_Ply is not
+        provided. The Landuse ID should be
+        1: land, -1: lake.
+    Soil_ID                           : string
+        the the column name in soil polygon and soil_info csv
+        indicate the soil ID. when soil polygon is not
+        provided. The Soil ID in Soil_info should be the same
+        as Landuse ID.
+    Veg_ID                            : string
+        the the column name in vegetation polygon and veg_info csv
+        indicate the vegetation ID. when Veg polygon is not
+        provided. The Veg ID in Veg_info should be the same
+        as Landuse ID.
+
+    Landuse_info                      : Dataframe
+        a dataframe that contains landuse information, including
+        following attributes:
+        Landuse_ID (can be any string)  - integer, the landuse ID in the
+                                                   landuse polygon
+        LAND_USE_C                      - string,  the landuse class name
+                                                   for each landuse Type
+    Soil_info                         : Dataframe
+        a dataframe that contains soil information, including
+        following attributes:
+        Soil_ID (can be any string)     - integer, the Soil ID in the
+                                                   soil polygon
+        SOIL_PROF                       - string,  the Soil profile name
+                                                   for each soil type
+    Veg_info                          : Dataframe
+        a dataframe file that contains vegetation information, including
+        following attributes:
+        Veg_ID (can be any string)      - integer, the vegetation ID in the
+                                                   vegetation polygon
+        VEG_C                           - string,  the vegetation class name
+                                                   for each vegetation Type
+    DEM                               : string (optional)
+        the path to a raster elevation dataset, that will be used to
+        calcuate average apspect, elevation and slope within each HRU.
+        if no data is provided, basin average value will be used for
+        each HRU.
+    Path_Subbasin_Ply                 : string
+        It is the path of the subbasin polygon, which is generated by
+        toolbox. if not generated by toolbox, the attribute table should
+        including following attribute.
+        ##############Subbasin related attributes###########################
+        SubID           - integer, The subbasin Id
+        DowSubId        - integer, The downstream subbasin ID of this
+                                   subbasin
+        IsLake          - integer, If the subbasin is a lake / reservior
+                                   subbasin. 1 yes, <0, no
+        IsObs           - integer, If the subbasin contains a observation
+                                   gauge. 1 yes, < 0 no.
+        RivLength       - float,   The length of the river in current
+                                   subbasin in m
+        RivSlope        - float,   The slope of the river path in
+                                   current subbasin, in m/m
+        FloodP_n        - float,   Flood plain manning's coefficient, in -
+        Ch_n            - float,   main channel manning's coefficient, in -
+        BkfWidth        - float,   the bankfull width of the main channel
+                                   in m
+        BkfDepth        - float,   the bankfull depth of the main channel
+                                   in m
+        HyLakeId        - integer, the lake id
+        LakeVol         - float,   the Volume of the lake in km3
+        LakeDepth       - float,   the average depth of the lake m
+        LakeArea        - float,   the area of the lake in m2
+    OutputFolder                      : String
+        The path to a folder to save result during the processing
+
+    Returns:
+    -------
+    HRU_draf_final                  : qgis object
+        it is a polygon object that generated by overlay all input
+        layers and inlcude all needed attribue for hydrological model
+        like RAVEN
+    """
+    num = str(np.random.randint(1, 10000 + 1))
+    hruinfo["LAND_USE_C"] = '-9999'
+    hruinfo["VEG_C"] = '-9999'
+    hruinfo["SOIL_PROF"] = '-9999'
+    hruinfo["HRU_CenX"] = -9999.9999
+    hruinfo["HRU_CenY"] = -9999.9999
+    hruinfo["HRU_ID_New"] = -9999
+    hruinfo["HRU_Area"] = -9999.99
+
+    hruinfo_area = add_area_in_m2(hruinfo,prj_crs,'HRU_Area')
+
+    hruinfo_area = simplify_hrus_method2(area_ratio_thresholds,hruinfo_area, Landuse_ID,
+                          Soil_ID,Veg_ID,Other_Ply_ID_1,Other_Ply_ID_2)
+
+    hruinfo_area = hruinfo_area.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
+
+
+    hruinfo_area['HRU_ID'] = hruinfo_area.index + 1
+    hruinfo_area["HRU_ID_New"] = hruinfo_area.index + 1
+
+    hruinfo_area_update_attribute = Determine_HRU_Attributes(
+        hruinfo_area,
+        Sub_ID,
+        Landuse_ID,
+        Soil_ID,
+        Veg_ID,
+        Other_Ply_ID_1,
+        Other_Ply_ID_2,
+        Landuse_info_data,
+        Soil_info_data,
+        Veg_info_data,
+    )
+    hruinfo_area_update_attribute = clean_geometry_purepy(hruinfo_area_update_attribute,set_precision = 1)
+    hruinfo_new = save_modified_attributes_to_outputs(
+        mapoldnew_info = hruinfo_area_update_attribute,
+        tempfolder = tempfolder,
+        OutputFolder = tempfolder,
+        cat_name = 'finalcat_hru_info.shp',
+        riv_name = '#',
+        Path_final_riv = '#',
+        dis_col_name='HRU_ID_New'
+    )
+    hruinfo_new = add_area_in_m2(hruinfo_new,prj_crs,'HRU_Area')
+#    print(len(hruinfo_area_update_attribute),len(hruinfo_new))
+    hruinfo_simple = hruinfo_new
+    # if len(Inmportance_order) > 0:
+    #     hruinfo_simple = simplidfy_hrus(
+    #         min_hru_pct_sub_area = min_hru_area_pct_sub,
+    #         hruinfo = hruinfo_new,
+    #         importance_order = Inmportance_order,
+    #     )
+    # else:
+    #     hruinfo_simple = hruinfo_new
+    #
+    # hruinfo_simple = clean_geometry_purepy(hruinfo_simple,set_precision = -1)
+    #
+    # hruinfo_simple = save_modified_attributes_to_outputs(
+    #     mapoldnew_info = hruinfo_simple,
+    #     tempfolder = tempfolder,
+    #     OutputFolder = tempfolder,
+    #     cat_name = 'hru_simple.shp',
+    #     riv_name = '#',
+    #     Path_final_riv = '#',
+    #     dis_col_name='HRU_ID_New'
+    # )
+
+    hruinfo_simple = add_centroid_in_wgs84(hruinfo_simple,"HRU_CenX","HRU_CenY")
+
+    cat_info = geopandas.read_file(Path_Subbasin_Ply)
+    cat_info = cat_info.drop(columns = 'geometry').copy(deep=True)
+
+    hruinfo_simple = pd.merge(hruinfo_simple, cat_info, on='SubId', how='left')
+
+    hruinfo_simple = add_area_in_m2(hruinfo_simple,prj_crs,'HRU_Area')
+#    print(len(hruinfo_simple))
+    if DEM != "#":
+
+        hru_proj= hruinfo_simple.to_crs(prj_crs)
+        hru_proj.to_file(os.path.join(tempfolder,"hru_proj.shp"))
+        proj_clip_raster(DEM,os.path.join(tempfolder,"demproj.tif"),prj_crs)
+#        proj_clip_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demclip.tif"),prj_crs,os.path.join(tempfolder,"hru_proj.shp"))
+        gdal_slope_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demslope.tif"))
+        gdal_aspect_raster(os.path.join(tempfolder,"demproj.tif"),os.path.join(tempfolder,"demaspect.tif"))
+
+        table_elv = ZonalStats(hru_proj, os.path.join(tempfolder,"demproj.tif"), 'mean','HRU_ID_New','MeanElev')
+        table_asp = ZonalStats(hru_proj, os.path.join(tempfolder,"demaspect.tif"), 'mean','HRU_ID_New','BasAspect')
+        table_slp = ZonalStats(hru_proj, os.path.join(tempfolder,"demslope.tif"), 'mean','HRU_ID_New','BasSlope')
+
+        table_slp['HRU_S_mean'] = table_slp['mean']
+        table_slp = table_slp[['HRU_ID_New','HRU_S_mean']]
+        table_asp['HRU_A_mean'] = table_asp['mean']
+        table_asp = table_asp[['HRU_ID_New','HRU_A_mean']]
+        table_elv['HRU_E_mean'] = table_elv['mean']
+        table_elv = table_elv[['HRU_ID_New','HRU_E_mean']]
+        hru_proj = pd.merge(hru_proj, table_slp, on='HRU_ID_New')
+        hru_proj = pd.merge(hru_proj, table_asp, on='HRU_ID_New')
+        hru_proj = pd.merge(hru_proj, table_elv, on='HRU_ID_New')
+        hruinfo_add_slp_asp = hru_proj.to_crs(trg_crs)
+        hruinfo_add_slp_asp = hruinfo_add_slp_asp.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
+        hruinfo_add_slp_asp['HRU_ID'] = hruinfo_add_slp_asp.index + 1
+#        print(len(hruinfo_add_slp_asp))
+    else:
+
+        hruinfo_add_slp_asp = hruinfo_simple.sort_values(by=[Sub_ID,Soil_ID,Landuse_ID]).copy(deep=True).reset_index()
+        hruinfo_add_slp_asp['HRU_ID'] = hruinfo_add_slp_asp.index + 1
+        hruinfo_add_slp_asp['HRU_S_mean'] = hruinfo_add_slp_asp['BasSlope']
+        hruinfo_add_slp_asp['HRU_A_mean'] = hruinfo_add_slp_asp['BasAspect']
+        hruinfo_add_slp_asp['HRU_E_mean'] = hruinfo_add_slp_asp['MeanElev']
+
+    hruinfo_add_slp_asp = adjust_HRUs_area_based_on_ply_sub_area(hruinfo_add_slp_asp)
+
+    hruinfo_add_slp_asp = clean_geometry_purepy(hruinfo_add_slp_asp,set_precision = 1)
+#    print(len(hruinfo_add_slp_asp))
+    return hruinfo_add_slp_asp
+
+def adjust_HRUs_area_based_on_ply_sub_area(hruinfo):
+    hruinfo['HRU_A_G'] =hruinfo ['HRU_Area']
+    subinfo = hruinfo[['SubId','HRU_Area']].copy(deep=True)
+    subinfo = subinfo.rename(columns={"HRU_Area": "Bas_A_G"})
+
+    subinfo = subinfo.groupby(['SubId'],as_index = False).sum()
+    hruinfo = pd.merge(hruinfo, subinfo, on='SubId')
+    hruinfo['Ratio_A'] = hruinfo['BasArea']/hruinfo['Bas_A_G']
+    hruinfo['HRU_Area'] = hruinfo['HRU_A_G'] * hruinfo['Ratio_A']
+
+    return hruinfo
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/increaseda.py` & `basinmaker-3.0.3/basinmaker/postprocessing/increaseda.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,41 +103,41 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
-    ## copy obs_gauges to output folder 
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
 
 
     # overall procedure,
     # 1. first get product attribute table
     # 2. determine which features needs to be merged together to increage
@@ -157,15 +157,15 @@
         sub_colnm, keep="first"
     )
 
     if Path_Conl_ply != '#':
         Conn_Lakes_ply = Dbf_To_Dataframe(Path_Conl_ply).drop_duplicates(
             "Hylak_id", keep="first"
         )
-    else: 
+    else:
         Conn_Lakes_ply = pd.DataFrame(np.full((10,1),-9999),columns=["Hylak_id"])
     # change attribute table
     (
         mapoldnew_info,
         Selected_riv_ids,
         Connected_Lake_Mainriv,
         Old_Non_Connect_LakeIds,
@@ -196,22 +196,22 @@
     UpdateTopology(mapoldnew_info)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
     # create output folder
     outputfolder_subid = OutputFolder
     if not os.path.exists(outputfolder_subid):
         os.makedirs(outputfolder_subid)
-        
+
     all_subids = finalriv_info['SubId'].values
-    
+
     copy_data_and_dissolve(all_subids,tempfolder,processing,Path_Temp_final_rviply,Path_Temp_final_rvi,
         mapoldnew_info,COLUMN_NAMES_CONSTANT_CLEAN,OutputFolder,Path_Catchment_Polygon,context,
         Path_final_rviply,Path_final_riv)
-        
-        
+
+
     # # copy new attribute table to subbasin polyline and polygon
     # Copy_Pddataframe_to_shpfile(
     #     Path_Temp_final_rviply,
     #     mapoldnew_info,
     #     link_col_nm_shp="SubId",
     #     link_col_nm_df="Old_SubId",
     #     UpdateColNM=["#"],
@@ -266,36 +266,36 @@
             Selectfeatureattributes(
                 processing,
                 Input=Path_Conl_ply,
                 Output=os.path.join(outputfolder_subid, outlake_name),
                 Attri_NM="Hylak_id",
                 Values=Conn_To_NonConlakeids,
             )
-                    
+
     # # dissolve subbasin polygon based on new subbasin id
     # Path_out_final_rviply = os.path.join(
     #     outputfolder_subid, os.path.basename(Path_final_riv_ply)
     # )
     # Path_out_final_rvi = os.path.join(
     #     outputfolder_subid, os.path.basename(Path_final_riv)
     # )
-    # 
+    #
     # qgis_vector_dissolve(
     #     processing,
     #     context,
     #     INPUT=Path_Temp_final_rviply,
     #     FIELD=["SubId"],
     #     OUTPUT=Path_out_final_rviply,
     # )
     # qgis_vector_dissolve(
     #     processing,
     #     context,
     #     INPUT=Path_Temp_final_rvi,
     #     FIELD=["SubId"],
     #     OUTPUT=Path_out_final_rvi,
     # )
-    # 
+    #
     # # clean attribute table and done
     # Clean_Attribute_Name(Path_out_final_rviply, COLUMN_NAMES_CONSTANT_CLEAN)
     # Clean_Attribute_Name(Path_out_final_rvi, COLUMN_NAMES_CONSTANT_CLEAN)
 
     Qgs.exit()
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/increasedaarcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/increasedaarcgis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import sys
 import os
 import csv
-import tempfile 
-import copy 
+import tempfile
+import copy
 import pandas as pd
 from arcgis.features import GeoAccessor, GeoSeriesAccessor
 import arcpy
 from arcpy import env
 from arcpy.sa import *
 import shutil
 
@@ -102,41 +102,41 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
-    ## copy obs_gauges to output folder 
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
 
     # overall procedure,
     # 1. first get product attribute table
     # 2. determine which features needs to be merged together to increage
     #    drainage area of the sub basin, for example sub a, b c needs to be merged
@@ -167,53 +167,53 @@
         Conn_To_NonConlakeids,
     ) = Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Increase_DA(
         finalriv_infoply, Conn_Lakes_ply, Area_Min
     )
 
     finalriv_inforiv_main = finalriv_inforiv.loc[finalriv_inforiv['SubId'].isin(Selected_riv_ids)]
     finalriv_inforiv_main.spatial.to_featureclass(location=os.path.join(tempfolder,'selected_riv.shp'),overwrite=True,sanitize_columns=False)
-    
+
     UpdateTopology(mapoldnew_info)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=os.path.basename(Path_final_riv_ply),
         riv_name = os.path.basename(Path_final_riv),
         Path_final_riv = os.path.join(tempfolder,'selected_riv.shp'),
     )
-   
-    # export lakes 
+
+    # export lakes
     if Path_Conl_ply == '#':
         Conn_Lakes_ply_select = []
         Conn_Lakes_ply_not_select = []
-    else:     
-        Conn_Lakes_ply = pd.DataFrame.spatial.from_featureclass(Path_Conl_ply)    
+    else:
+        Conn_Lakes_ply = pd.DataFrame.spatial.from_featureclass(Path_Conl_ply)
         lake_mask = Conn_Lakes_ply['Hylak_id'].isin(Connected_Lake_Mainriv)
         Conn_Lakes_ply_select = Conn_Lakes_ply.loc[lake_mask].copy()
         Conn_Lakes_ply_not_select = Conn_Lakes_ply.loc[np.logical_not(lake_mask)].copy()
 
     # export lake polygons
     # export connected lake polygon
     if len(Conn_Lakes_ply_select) > 0:
         Conn_Lakes_ply_select.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_Conl_ply)),overwrite=True,sanitize_columns=False)
-    
-    # export non connected polygon 
+
+    # export non connected polygon
     if len(Conn_Lakes_ply_not_select) >0 and Path_NonCon_Lake_ply != '#':
-        non_conn_Lakes_ply = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)  
+        non_conn_Lakes_ply = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)
         new_non_connected_lake = pd.concat([non_conn_Lakes_ply, Conn_Lakes_ply_not_select], ignore_index=True)
         new_non_connected_lake.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)),overwrite=True,sanitize_columns=False)
     if len(Conn_Lakes_ply_not_select) <= 0 and Path_NonCon_Lake_ply != '#':
         non_conn_Lakes_ply = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)
         non_conn_Lakes_ply.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)),overwrite=True,sanitize_columns=False)
     if len(Conn_Lakes_ply_not_select) > 0 and Path_NonCon_Lake_ply == '#':
-       
+
         if len(os.path.basename(Path_Conl_ply).split('_')) == 4:
             outlake_name = 'sl_non_connected_lake_' + os.path.basename(Path_Conl_ply).split('_')[3]
         else:
             outlake_name = 'sl_non_connected_lake.shp'
-            
+
         Conn_Lakes_ply_not_select.spatial.to_featureclass(location=os.path.join(OutputFolder,outlake_name),overwrite=True,sanitize_columns=False)
-        
-    return 
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/increasedapurepy.py` & `basinmaker-3.0.3/basinmaker/postprocessing/increasedapurepy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import sys
 import os
 import csv
-import tempfile 
-import copy 
+import tempfile
+import copy
 import pandas as pd
 import shutil
 import geopandas
 
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
@@ -97,41 +97,41 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
 
-    ## copy obs_gauges to output folder 
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
 
     # overall procedure,
     # 1. first get product attribute table
     # 2. determine which features needs to be merged together to increage
     #    drainage area of the sub basin, for example sub a, b c needs to be merged
@@ -144,20 +144,20 @@
     Path_final_rviply = Path_final_riv_ply
     Path_final_riv = Path_final_riv
     Path_Conl_ply = Path_Con_Lake_ply
     Path_Non_ConL_ply = Path_NonCon_Lake_ply
 
     finalriv_infoply = geopandas.read_file(Path_final_rviply)
     finalriv_inforiv = geopandas.read_file(Path_final_riv)
-    
+
     if Path_Conl_ply != '#':
         Conn_Lakes_ply = geopandas.read_file(Path_Conl_ply)
-    else: 
+    else:
         Conn_Lakes_ply = pd.DataFrame(np.full((10,1),-9999),columns=["Hylak_id"])
-                
+
 
 
     # change attribute table
     (
         mapoldnew_info,
         Selected_riv_ids,
         Connected_Lake_Mainriv,
@@ -165,52 +165,52 @@
         Conn_To_NonConlakeids,
     ) = Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Increase_DA(
         finalriv_infoply, Conn_Lakes_ply, Area_Min
     )
 
     finalriv_inforiv_main = finalriv_inforiv.loc[finalriv_inforiv['SubId'].isin(Selected_riv_ids)]
     finalriv_inforiv_main.to_file(os.path.join(tempfolder,'selected_riv.shp'))
-    
+
     UpdateTopology(mapoldnew_info)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=os.path.basename(Path_final_riv_ply),
         riv_name = os.path.basename(Path_final_riv),
         Path_final_riv = os.path.join(tempfolder,'selected_riv.shp'),
     )
-   
-    # export lakes 
+
+    # export lakes
     if Path_Conl_ply == '#':
         Conn_Lakes_ply_select = []
         Conn_Lakes_ply_not_select = []
-    else:     
-        Conn_Lakes_ply = geopandas.read_file(Path_Conl_ply)    
+    else:
+        Conn_Lakes_ply = geopandas.read_file(Path_Conl_ply)
         lake_mask = Conn_Lakes_ply['Hylak_id'].isin(Connected_Lake_Mainriv)
         Conn_Lakes_ply_select = Conn_Lakes_ply.loc[lake_mask].copy()
         Conn_Lakes_ply_not_select = Conn_Lakes_ply.loc[np.logical_not(lake_mask)].copy()
 
     # export lake polygons
     # export connected lake polygon
     if len(Conn_Lakes_ply_select) > 0:
         Conn_Lakes_ply_select.to_file(os.path.join(OutputFolder,os.path.basename(Path_Conl_ply)))
-    
-    # export non connected polygon 
+
+    # export non connected polygon
     if len(Conn_Lakes_ply_not_select) >0 and Path_NonCon_Lake_ply != '#':
-        non_conn_Lakes_ply = geopandas.read_file(Path_NonCon_Lake_ply)  
+        non_conn_Lakes_ply = geopandas.read_file(Path_NonCon_Lake_ply)
         new_non_connected_lake = pd.concat([non_conn_Lakes_ply, Conn_Lakes_ply_not_select], ignore_index=True)
         new_non_connected_lake.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
     if len(Conn_Lakes_ply_not_select) <= 0 and Path_NonCon_Lake_ply != '#':
         non_conn_Lakes_ply = geopandas.read_file(Path_NonCon_Lake_ply)
         non_conn_Lakes_ply.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
     if len(Conn_Lakes_ply_not_select) > 0 and Path_NonCon_Lake_ply == '#':
         if len(os.path.basename(Path_Conl_ply).split('_')) == 4:
             outlake_name = 'sl_non_connected_lake_' + os.path.basename(Path_Conl_ply).split('_')[3]
         else:
             outlake_name = 'sl_non_connected_lake.shp'
-            
+
         Conn_Lakes_ply_not_select.to_file(os.path.join(OutputFolder,outlake_name))
-        
-    return 
+
+    return
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/inversetopology.py` & `basinmaker-3.0.3/basinmaker/postprocessing/inversetopology.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/plotleaflet.py` & `basinmaker-3.0.3/basinmaker/postprocessing/plotleaflet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-import os
-import geopandas
-import matplotlib.pyplot as plt ## only needed to plot figures
-from ipywidgets import HTML,Layout,IntSlider, ColorPicker, jslink ## only needed to plot figures
-from ipyleaflet import Map, GeoData, basemaps, LayersControl,Popup,Marker,Polygon,Choropleth,WidgetControl## only needed to plot figures
-#import leafmap.foliumap  as leafmap
-
-def plot_routing_product_with_ipyleaflet(path_to_product_folder,version_number = ''):
-    product_folder = path_to_product_folder
-    if version_number != '':
-        version_number = '_'+version_number
-    path_subbasin = os.path.join(product_folder,'finalcat_info'+version_number+'.shp')
-    path_river = os.path.join(product_folder,'finalcat_info_riv'+version_number+'.shp')
-    path_cllake = os.path.join(product_folder,'sl_connected_lake'+version_number+'.shp')
-    path_ncllake = os.path.join(product_folder,'sl_non_connected_lake'+version_number+'.shp')
-
-    subbasin = geopandas.read_file(path_subbasin)
-    subbasin = subbasin.to_crs("EPSG:4326")
-
-    if os.path.exists(path_river):
-        river = geopandas.read_file(path_river)
-        river = river.to_crs("EPSG:4326")
-
-
-    if os.path.exists(path_cllake):
-        cllake = geopandas.read_file(path_cllake)
-        cllake = cllake.to_crs("EPSG:4326")
-    if os.path.exists(path_ncllake):
-        ncllake = geopandas.read_file(path_ncllake)
-        ncllake = ncllake.to_crs("EPSG:4326")
-
-    cx = subbasin['centroid_x'].mean()
-    cy = subbasin['centroid_y'].mean()
-    m = Map(center=(cy,cx), zoom = 9, basemap= basemaps.Esri.WorldTopoMap)
-
-    subnolake = subbasin[subbasin['Lake_Cat'] == 0].copy(deep=True)
-    sub_nolake_map = GeoData(geo_dataframe = subnolake,
-                      style={'color': '#6E6E6E', 'fillColor': '#89CD66', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
-                      name = 'Subbasin without lakes')
-    subcllake = subbasin[subbasin['Lake_Cat'] == 1].copy(deep=True)
-    if len(subcllake) > 0:
-        sub_cllake_map = GeoData(geo_dataframe = subcllake,
-                          style={'color': '#6E6E6E', 'fillColor': '#CDE389', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
-                          name = 'Subbasin with connected lakes')
-    subncllake = subbasin[subbasin['Lake_Cat'] == 2].copy(deep=True)
-    if len(subncllake) > 0:
-        sub_ncllake_map = GeoData(geo_dataframe = subncllake,
-                          style={'color': '#6E6E6E', 'fillColor': '#F5F57A', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
-                          name = 'Subbasin with connected lakes')
-    if os.path.exists(path_river):
-        river_map = GeoData(geo_dataframe = river,
-                          style={'color': '#0070FF', 'fillColor': '#0070FF', 'opacity':1, 'weight':2, 'dashArray':'2', 'fillOpacity':1},
-                          name = 'River')
-    if os.path.exists(path_cllake):
-        cllake_map = GeoData(geo_dataframe = cllake,
-                            style={'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
-                            name = 'Non connected lakes')
-    if os.path.exists(path_ncllake):
-        ncllake_map = GeoData(geo_dataframe = ncllake,
-                             style={'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':0, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
-                             name = 'Connected lakes')
-
-    m.add_layer(sub_nolake_map)
-    if len(subcllake) > 0:
-        m.add_layer(sub_cllake_map)
-    if len(subncllake) > 0:
-        m.add_layer(sub_ncllake_map)
-    if os.path.exists(path_river):
-        m.add_layer(river_map)
-    if os.path.exists(path_cllake):
-        m.add_layer(cllake_map)
-    if os.path.exists(path_ncllake):
-        m.add_layer(ncllake_map)
-
-    m.add_control(LayersControl())
-    m.layout.height="700px"
-
-    return m
-
-# def plot_routing_product_with_leafmap(path_to_product_folder,version_number = ''):
-#     product_folder = path_to_product_folder
-#     if version_number != '':
-#         version_number = '_'+version_number
-#     path_subbasin = os.path.join(product_folder,'finalcat_info'+version_number+'.shp')
-#     path_river = os.path.join(product_folder,'finalcat_info_riv'+version_number+'.shp')
-#     path_cllake = os.path.join(product_folder,'sl_connected_lake'+version_number+'.shp')
-#     path_ncllake = os.path.join(product_folder,'sl_non_connected_lake'+version_number+'.shp')
-#
-#     subbasin = geopandas.read_file(path_subbasin)
-#     subbasin = subbasin.to_crs("EPSG:4326")
-#
-#     if os.path.exists(path_river):
-#         river = geopandas.read_file(path_river)
-#         river = river.to_crs("EPSG:4326")
-#
-#
-#     if os.path.exists(path_cllake):
-#         cllake = geopandas.read_file(path_cllake)
-#         cllake = cllake.to_crs("EPSG:4326")
-#     if os.path.exists(path_ncllake):
-#         ncllake = geopandas.read_file(path_ncllake)
-#         ncllake = ncllake.to_crs("EPSG:4326")
-#
-#     subcol_olrrp = ['SubId','geometry','DowSubId','BasArea','Lake_Cat','DrainArea','DA_Chn_L','DA_Slope','DA_Chn_Slp','BasSlope']
-#     subcol_na = ['SubId','geometry','DowSubId','BasArea','Lake_Cat','DrainArea','BasSlope']
-#
-#     rivcol = ['geometry','RivSlope','RivLength','BkfWidth','BkfDepth','Strahler','Q_Mean','FloodP_n','Ch_n']
-#     lake_col =  ['geometry','Hylak_id','Lake_type','Lake_area','Vol_total','Depth_avg']
-#
-#     if version_number == 'v1-0':
-#         subcol = subcol_olrrp
-#     else:
-#         subcol = subcol_na
-#
-#     subnolake = subbasin[subbasin['Lake_Cat'] == 0].copy(deep=True)
-#
-#     m = leafmap.Map(
-#         draw_control=False,
-#         measure_control=False,
-#         fullscreen_control=False,
-#         attribution_control=True,
-#     )
-#
-#
-#     m.add_gdf(subnolake[subcol], layer_name="Subbasin without lakes",style = {'color': '#6E6E6E', 'fillColor': '#89CD66', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1})
-#     labels = ["Subbasin without lakes"]
-#     colors = ["#89CD66"]
-#
-#     subcllake = subbasin[subbasin['Lake_Cat'] == 1].copy(deep=True)
-#     if len(subcllake) > 0:
-#         style = {'color': '#6E6E6E', 'fillColor': '#CDE389', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
-#         name = 'Subbasin with connected lakes'
-#         m.add_gdf(subcllake[subcol], layer_name=name,style = style)
-#         labels = labels + ['Subbasin with connected lakes']
-#         colors = colors + ['#CDE389']
-#
-#
-#     subncllake = subbasin[subbasin['Lake_Cat'] == 2].copy(deep=True)
-#     if len(subncllake) > 0:
-#         style = {'color': '#6E6E6E', 'fillColor': '#F5F57A', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
-#         name = 'Subbasin with non connected lakes'
-#         m.add_gdf(subncllake[subcol], layer_name=name,style = style)
-#         labels = labels + ['Subbasin with non connected lakes']
-#         colors = colors + ['#F5F57A']
-#
-#     if os.path.exists(path_river):
-#         style = {'color': '#0070FF', 'fillColor': '#0070FF', 'opacity':1, 'weight':2, 'dashArray':'2', 'fillOpacity':1}
-#         name = 'River'
-#         m.add_gdf(river[rivcol], layer_name=name,style = style)
-#         labels = labels + ['River/Lakes']
-#         colors = colors + ['#0070FF']
-#
-#     if os.path.exists(path_cllake):
-#         style = {'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
-#         name = 'Non connected lakes'
-#         m.add_gdf(cllake[lake_col], layer_name=name,style = style)
-#
-#
-#     if os.path.exists(path_ncllake):
-#         style = {'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
-#         name = 'Cconnected lakes'
-#         m.add_gdf(ncllake[lake_col], layer_name=name,style = style)
-#
-#     m.add_legend(title='Legend', labels=labels, colors=colors)
-#     return m
+import os
+import geopandas
+import matplotlib.pyplot as plt ## only needed to plot figures
+from ipywidgets import HTML,Layout,IntSlider, ColorPicker, jslink ## only needed to plot figures
+from ipyleaflet import Map, GeoData, basemaps, LayersControl,Popup,Marker,Polygon,Choropleth,WidgetControl## only needed to plot figures
+#import leafmap.foliumap  as leafmap
+
+def plot_routing_product_with_ipyleaflet(path_to_product_folder,version_number = ''):
+    product_folder = path_to_product_folder
+    if version_number != '':
+        version_number = '_'+version_number
+    path_subbasin = os.path.join(product_folder,'finalcat_info'+version_number+'.shp')
+    path_river = os.path.join(product_folder,'finalcat_info_riv'+version_number+'.shp')
+    path_cllake = os.path.join(product_folder,'sl_connected_lake'+version_number+'.shp')
+    path_ncllake = os.path.join(product_folder,'sl_non_connected_lake'+version_number+'.shp')
+
+    subbasin = geopandas.read_file(path_subbasin)
+    subbasin = subbasin.to_crs("EPSG:4326")
+
+    if os.path.exists(path_river):
+        river = geopandas.read_file(path_river)
+        river = river.to_crs("EPSG:4326")
+
+
+    if os.path.exists(path_cllake):
+        cllake = geopandas.read_file(path_cllake)
+        cllake = cllake.to_crs("EPSG:4326")
+    if os.path.exists(path_ncllake):
+        ncllake = geopandas.read_file(path_ncllake)
+        ncllake = ncllake.to_crs("EPSG:4326")
+
+    cx = subbasin['centroid_x'].mean()
+    cy = subbasin['centroid_y'].mean()
+    m = Map(center=(cy,cx), zoom = 9, basemap= basemaps.Esri.WorldTopoMap)
+
+    subnolake = subbasin[subbasin['Lake_Cat'] == 0].copy(deep=True)
+    sub_nolake_map = GeoData(geo_dataframe = subnolake,
+                      style={'color': '#6E6E6E', 'fillColor': '#89CD66', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
+                      name = 'Subbasin without lakes')
+    subcllake = subbasin[subbasin['Lake_Cat'] == 1].copy(deep=True)
+    if len(subcllake) > 0:
+        sub_cllake_map = GeoData(geo_dataframe = subcllake,
+                          style={'color': '#6E6E6E', 'fillColor': '#CDE389', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
+                          name = 'Subbasin with connected lakes')
+    subncllake = subbasin[subbasin['Lake_Cat'] == 2].copy(deep=True)
+    if len(subncllake) > 0:
+        sub_ncllake_map = GeoData(geo_dataframe = subncllake,
+                          style={'color': '#6E6E6E', 'fillColor': '#F5F57A', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
+                          name = 'Subbasin with connected lakes')
+    if os.path.exists(path_river):
+        river_map = GeoData(geo_dataframe = river,
+                          style={'color': '#0070FF', 'fillColor': '#0070FF', 'opacity':1, 'weight':2, 'dashArray':'2', 'fillOpacity':1},
+                          name = 'River')
+    if os.path.exists(path_cllake):
+        cllake_map = GeoData(geo_dataframe = cllake,
+                            style={'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
+                            name = 'Connected lakes')
+    if os.path.exists(path_ncllake):
+        ncllake_map = GeoData(geo_dataframe = ncllake,
+                             style={'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':0, 'weight':1, 'dashArray':'2', 'fillOpacity':1},
+                             name = 'Non connected lakes')
+    
+    m.add_layer(sub_nolake_map)
+    if len(subcllake) > 0:
+        m.add_layer(sub_cllake_map)
+    if len(subncllake) > 0:
+        m.add_layer(sub_ncllake_map)
+    if os.path.exists(path_river):
+        m.add_layer(river_map)
+    if os.path.exists(path_cllake):
+        m.add_layer(cllake_map)
+    if os.path.exists(path_ncllake):
+        m.add_layer(ncllake_map)
+
+    m.add_control(LayersControl())
+    m.layout.height="700px"
+
+    return m
+
+# def plot_routing_product_with_leafmap(path_to_product_folder,version_number = ''):
+#     product_folder = path_to_product_folder
+#     if version_number != '':
+#         version_number = '_'+version_number
+#     path_subbasin = os.path.join(product_folder,'finalcat_info'+version_number+'.shp')
+#     path_river = os.path.join(product_folder,'finalcat_info_riv'+version_number+'.shp')
+#     path_cllake = os.path.join(product_folder,'sl_connected_lake'+version_number+'.shp')
+#     path_ncllake = os.path.join(product_folder,'sl_non_connected_lake'+version_number+'.shp')
+#
+#     subbasin = geopandas.read_file(path_subbasin)
+#     subbasin = subbasin.to_crs("EPSG:4326")
+#
+#     if os.path.exists(path_river):
+#         river = geopandas.read_file(path_river)
+#         river = river.to_crs("EPSG:4326")
+#
+#
+#     if os.path.exists(path_cllake):
+#         cllake = geopandas.read_file(path_cllake)
+#         cllake = cllake.to_crs("EPSG:4326")
+#     if os.path.exists(path_ncllake):
+#         ncllake = geopandas.read_file(path_ncllake)
+#         ncllake = ncllake.to_crs("EPSG:4326")
+#
+#     subcol_olrrp = ['SubId','geometry','DowSubId','BasArea','Lake_Cat','DrainArea','DA_Chn_L','DA_Slope','DA_Chn_Slp','BasSlope']
+#     subcol_na = ['SubId','geometry','DowSubId','BasArea','Lake_Cat','DrainArea','BasSlope']
+#
+#     rivcol = ['geometry','RivSlope','RivLength','BkfWidth','BkfDepth','Strahler','Q_Mean','FloodP_n','Ch_n']
+#     lake_col =  ['geometry','Hylak_id','Lake_type','Lake_area','Vol_total','Depth_avg']
+#
+#     if version_number == 'v1-0':
+#         subcol = subcol_olrrp
+#     else:
+#         subcol = subcol_na
+#
+#     subnolake = subbasin[subbasin['Lake_Cat'] == 0].copy(deep=True)
+#
+#     m = leafmap.Map(
+#         draw_control=False,
+#         measure_control=False,
+#         fullscreen_control=False,
+#         attribution_control=True,
+#     )
+#
+#
+#     m.add_gdf(subnolake[subcol], layer_name="Subbasin without lakes",style = {'color': '#6E6E6E', 'fillColor': '#89CD66', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1})
+#     labels = ["Subbasin without lakes"]
+#     colors = ["#89CD66"]
+#
+#     subcllake = subbasin[subbasin['Lake_Cat'] == 1].copy(deep=True)
+#     if len(subcllake) > 0:
+#         style = {'color': '#6E6E6E', 'fillColor': '#CDE389', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
+#         name = 'Subbasin with connected lakes'
+#         m.add_gdf(subcllake[subcol], layer_name=name,style = style)
+#         labels = labels + ['Subbasin with connected lakes']
+#         colors = colors + ['#CDE389']
+#
+#
+#     subncllake = subbasin[subbasin['Lake_Cat'] == 2].copy(deep=True)
+#     if len(subncllake) > 0:
+#         style = {'color': '#6E6E6E', 'fillColor': '#F5F57A', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
+#         name = 'Subbasin with non connected lakes'
+#         m.add_gdf(subncllake[subcol], layer_name=name,style = style)
+#         labels = labels + ['Subbasin with non connected lakes']
+#         colors = colors + ['#F5F57A']
+#
+#     if os.path.exists(path_river):
+#         style = {'color': '#0070FF', 'fillColor': '#0070FF', 'opacity':1, 'weight':2, 'dashArray':'2', 'fillOpacity':1}
+#         name = 'River'
+#         m.add_gdf(river[rivcol], layer_name=name,style = style)
+#         labels = labels + ['River/Lakes']
+#         colors = colors + ['#0070FF']
+#
+#     if os.path.exists(path_cllake):
+#         style = {'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
+#         name = 'Non connected lakes'
+#         m.add_gdf(cllake[lake_col], layer_name=name,style = style)
+#
+#
+#     if os.path.exists(path_ncllake):
+#         style = {'color': '#6E6E6E', 'fillColor': '#0070FF', 'opacity':1, 'weight':1, 'dashArray':'2', 'fillOpacity':1}
+#         name = 'Cconnected lakes'
+#         m.add_gdf(ncllake[lake_col], layer_name=name,style = style)
+#
+#     m.add_legend(title='Legend', labels=labels, colors=colors)
+#     return m
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/selectlake.py` & `basinmaker-3.0.3/basinmaker/postprocessing/selectlake.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     feedback = QgsProcessingFeedback()
     Processing.initialize()
     QgsApplication.processingRegistry().addProvider(QgsNativeAlgorithms())
     context = dataobjects.createContext()
     context.setInvalidGeometryCheck(QgsFeatureRequest.GeometryNoCheck)
 
-    
+
     if not os.path.exists(OutputFolder):
         os.makedirs(OutputFolder)
 
     tempfolder = os.path.join(
         tempfile.gettempdir(),
         "basinmaker_sllake_" + str(np.random.randint(1, 10000 + 1)),
     )
@@ -113,44 +113,44 @@
     Path_Catchment_Polygon="#"
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
-    
-    ## copy obs_gauges to output folder 
+
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
-    
+
     ### read attribute table
     finalcat_info = Dbf_To_Dataframe(Path_final_riv_ply)
     finalcat_info = finalcat_info.fillna(-9999)
 
     ### Obtain selected lake's attribute info
     (
         Selected_Non_ConnLakes,
@@ -222,34 +222,34 @@
     )
     # change attribute for catchment due to remove of non connected lakes
     mapoldnew_info = (
         Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_NCL(
             mapoldnew_info, finalcat_info_temp, Un_Selected_Non_ConnL_info
         )
     )
-    
+
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'HyLakeId'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Lake_Cat'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeVol'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeDepth'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeArea'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Laketype'] = 0
-    
+
     # update topology for new attribute table
     UpdateTopology(mapoldnew_info, UpdateStreamorder=-1)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
 
 
     all_subids = finalcat_info_temp['SubId'].values
-    
+
     copy_data_and_dissolve(all_subids,tempfolder,processing,Path_Temp_final_rviply,Path_Temp_final_rvi,
         mapoldnew_info,COLUMN_NAMES_CONSTANT_CLEAN,OutputFolder,Path_Catchment_Polygon,context,
         Path_final_riv_ply,Path_final_riv)
-        
-        
+
+
     # # copy new attribute table to shpfiles
     # Copy_Pddataframe_to_shpfile(
     #     Path_Temp_final_rviply,
     #     mapoldnew_info,
     #     link_col_nm_shp="SubId",
     #     link_col_nm_df="Old_SubId",
     #     UpdateColNM=["#"],
@@ -257,15 +257,15 @@
     # Copy_Pddataframe_to_shpfile(
     #     Path_Temp_final_rvi,
     #     mapoldnew_info,
     #     link_col_nm_shp="SubId",
     #     link_col_nm_df="Old_SubId",
     #     UpdateColNM=["#"],
     # )
-    # 
+    #
     # # disslove line and polygon based on new subid
     # qgis_vector_dissolve(
     #     processing,
     #     context,
     #     INPUT=Path_Temp_final_rvi,
     #     FIELD=["SubId"],
     #     OUTPUT=os.path.join(OutputFolder, os.path.basename(Path_final_riv)),
@@ -273,15 +273,15 @@
     # qgis_vector_dissolve(
     #     processing,
     #     context,
     #     INPUT=Path_Temp_final_rviply,
     #     FIELD=["SubId"],
     #     OUTPUT=os.path.join(OutputFolder, os.path.basename(Path_final_riv_ply)),
     # )
-    # 
+    #
     # # clean attribute table
     # Clean_Attribute_Name(
     #     os.path.join(OutputFolder, os.path.basename(Path_final_riv)),
     #     COLUMN_NAMES_CONSTANT,
     # )
     # Clean_Attribute_Name(
     #     os.path.join(OutputFolder, os.path.basename(Path_final_riv_ply)),
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/selectlakearcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/selectlakearcgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import sys
 import os
 import csv
-import tempfile 
-import copy 
+import tempfile
+import copy
 import pandas as pd
 from arcgis.features import GeoAccessor, GeoSeriesAccessor
 import arcpy
 from arcpy import env
 from arcpy.sa import *
 import shutil
 
@@ -101,49 +101,49 @@
 
     tempfolder = os.path.join(
         tempfile.gettempdir(),
         "basinmaker_sllake_" + str(np.random.randint(1, 10000 + 1)),
     )
     if not os.path.exists(tempfolder):
         os.makedirs(tempfolder)
-        
+
     Path_Catchment_Polygon="#"
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
-    
-    ## copy obs_gauges to output folder 
+
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
 
     ### read attribute table
     finalcat_info = pd.DataFrame.spatial.from_featureclass(Path_final_riv_ply)
 
     ### Obtain selected lake's attribute info
@@ -155,37 +155,37 @@
         Un_Selected_Non_ConnL_info,
     ) = Return_Selected_Lakes_Attribute_Table_And_Id(
         finalcat_info,
         Thres_Area_Conn_Lakes*1000*1000,
         Thres_Area_Non_Conn_Lakes*1000*1000,
         Selected_Lake_List_in,
     )
-    
+
     ### Extract lake polygons
     if len(Selected_Non_ConnLakes) > 0:
         sl_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)
         sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_Non_ConnLakes)]
         sl_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)),overwrite=True,sanitize_columns=False)
 
     if len(Selected_ConnLakes) > 0:
         sl_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_Con_Lake_ply)
         sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_ConnLakes)]
         sl_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply)),overwrite=True,sanitize_columns=False)
 
     print(" Obtain selected Lake IDs done")
 
-   
+
     finalcat_ply = pd.DataFrame.spatial.from_featureclass(Path_final_riv_ply)
     # change lake related attribute for un selected connected lake
     # catchment to -1.2345
     finalcat_ply = Remove_Unselected_Lake_Attribute_In_Finalcatinfo_Arcgis(
         finalcat_ply, Selected_ConnLakes
     )
     # remove lake attribute
-        
+
     # Modify attribute table to merge un selected lake catchment if needed
     # change attributes for catchment due to remove of connected lakes
     mapoldnew_info = (
         Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_CL(
             finalcat_ply, Un_Selected_ConnLakes_info
         )
     )
@@ -198,19 +198,19 @@
 
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'HyLakeId'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Lake_Cat'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeVol'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeDepth'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'LakeArea'] = 0
     mapoldnew_info.loc[mapoldnew_info['HyLakeId'] <= 0,'Laketype'] = 0
-        
+
     # update topology for new attribute table
     mapoldnew_info = UpdateTopology(mapoldnew_info, UpdateStreamorder=-1)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
-    
+
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=os.path.basename(Path_final_riv_ply),
         riv_name = os.path.basename(Path_final_riv),
         Path_final_riv = Path_final_riv,
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/selectlakepurepy.py` & `basinmaker-3.0.3/basinmaker/postprocessing/selectlakepurepy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import sys
 import os
 import csv
-import tempfile 
-import copy 
+import tempfile
+import copy
 import pandas as pd
 import shutil
 import geopandas
 
 import sys, os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
@@ -96,49 +96,49 @@
 
     tempfolder = os.path.join(
         tempfile.gettempdir(),
         "basinmaker_sllake_" + str(np.random.randint(1, 10000 + 1)),
     )
     if not os.path.exists(tempfolder):
         os.makedirs(tempfolder)
-        
+
     Path_Catchment_Polygon="#"
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
 
     Path_final_riv_ply = Path_Catchment_Polygon
     Path_final_riv = Path_River_Polyline
-    
-    ## copy obs_gauges to output folder 
+
+    ## copy obs_gauges to output folder
     for file in os.listdir(Routing_Product_Folder):
-        if 'obs_gauges' in file:
+        if 'obs_gauges' in file or 'poi' in file:
             shutil.copy(os.path.join(Routing_Product_Folder, file), os.path.join(OutputFolder, file))
 
 
     ### read attribute table
     finalcat_info = geopandas.read_file(Path_final_riv_ply)
 
     ### Obtain selected lake's attribute info
@@ -150,54 +150,54 @@
         Un_Selected_Non_ConnL_info,
     ) = Return_Selected_Lakes_Attribute_Table_And_Id(
         finalcat_info,
         Thres_Area_Conn_Lakes*1000*1000,
         Thres_Area_Non_Conn_Lakes*1000*1000,
         Selected_Lake_List_in,
     )
-    
+
     ### Extract lake polygons
     if len(Selected_Non_ConnLakes) > 0:
         sl_con_lakes = geopandas.read_file(Path_NonCon_Lake_ply)
         sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_Non_ConnLakes)]
         sl_con_lakes.to_file(os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)))
 
     if len(Selected_ConnLakes) > 0:
         sl_con_lakes = geopandas.read_file(Path_Con_Lake_ply)
         sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Selected_ConnLakes)]
         sl_con_lakes.to_file(os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply)))
 
     print(" Obtain selected Lake IDs done")
- 
+
     finalcat_ply = geopandas.read_file(Path_final_riv_ply)
     # change lake related attribute for un selected connected lake
     # catchment to -1.2345
     finalcat_ply = Remove_Unselected_Lake_Attribute_In_Finalcatinfo_purepy(
         finalcat_ply, Selected_ConnLakes
     )
     # remove lake attribute
-        
+
     # Modify attribute table to merge un selected lake catchment if needed
     # change attributes for catchment due to remove of connected lakes
     mapoldnew_info = (
         Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_CL(
             finalcat_ply, Un_Selected_ConnLakes_info
         )
     )
     # change attribute for catchment due to remove of non connected lakes
     mapoldnew_info = (
         Change_Attribute_Values_For_Catchments_Need_To_Be_Merged_By_Remove_NCL(
             mapoldnew_info, finalcat_ply, Un_Selected_Non_ConnL_info
         )
     )
-    
+
     # update topology for new attribute table
     mapoldnew_info = UpdateTopology(mapoldnew_info, UpdateStreamorder=-1)
     mapoldnew_info = update_non_connected_catchment_info(mapoldnew_info)
-    
+
     save_modified_attributes_to_outputs(
         mapoldnew_info=mapoldnew_info,
         tempfolder=tempfolder,
         OutputFolder=OutputFolder,
         cat_name=os.path.basename(Path_final_riv_ply),
         riv_name = os.path.basename(Path_final_riv),
         Path_final_riv = Path_final_riv,
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/selectprod.py` & `basinmaker-3.0.3/basinmaker/postprocessing/selectprod.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,56 +199,56 @@
     Path_River_Polyline="#"
     Path_Con_Lake_ply="#"
     Path_NonCon_Lake_ply="#"
     Path_obs_gauge_point="#"
     Path_final_cat_ply="#"
     Path_final_cat_riv="#"
 
-    ##define input files from routing prodcut 
+    ##define input files from routing prodcut
     for file in os.listdir(Routing_Product_Folder):
         if file.endswith(".shp"):
             if 'catchment_without_merging_lakes' in file:
                 Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
             if 'river_without_merging_lakes' in file:
                 Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
             if 'sl_connected_lake' in file:
                 Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
             if 'sl_non_connected_lake' in file:
                 Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
+            if 'obs_gauges' in file or 'poi' in file:
                 Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info' in file:
                 Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
             if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
 
     if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
         print("Invalid routing product folder ")
-    
+
     sub_colnm = "SubId"
     down_colnm = "DowSubId"
     ##3
     hyshdinfo2 = Dbf_To_Dataframe(Path_Catchment_Polygon).drop_duplicates(
         sub_colnm, keep="first"
     )
     hyshdinfo = hyshdinfo2[[sub_colnm, down_colnm]].astype("int32").values
 
 
     Gauge_col_Name = "Has_POI"
     if "Has_POI" not in hyshdinfo2.columns:
         Gauge_col_Name = "Has_Gauge"
-        
+
     if not os.path.exists(OutputFolder):
         os.makedirs(OutputFolder)
-        
+
     for i_down in range(0,len(mostdownid)):
         ### Loop for each downstream id
         OutHyID = mostdownid[i_down]
         OutHyID2 = mostupstreamid[i_down]
-            
+
         ## find all subid control by this subid
         HydroBasins1 = defcat(hyshdinfo, OutHyID)
         if OutHyID2 > 0:
             HydroBasins2 = defcat(hyshdinfo, OutHyID2)
             ###  exculde the Ids in HydroBasins2 from HydroBasins1
             for i in range(len(HydroBasins2)):
                 rows = np.argwhere(HydroBasins1 == HydroBasins2[i])
@@ -324,9 +324,9 @@
             processing,
             Input=Path_obs_gauge_point,
             Output=os.path.join(OutputFolder, os.path.basename(Path_obs_gauge_point)),
             Attri_NM="Obs_NM",
             Values=Gauge_NMs,
             Is_str = True,
         )
-    
+
     Qgs.exit()
```

### Comparing `basinmaker-3.0.1/basinmaker/postprocessing/selectprodarcgis.py` & `basinmaker-3.0.3/basinmaker/postprocessing/selectprodarcgis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,291 +1,293 @@
-
-import numpy as np
-import arcpy
-from arcpy import env
-from arcpy.sa import *
-from arcgis.features import GeoAccessor, GeoSeriesAccessor
-import sys
-import os
-import csv
-import pandas as pd
-import tempfile 
-import copy 
-
-import sys, os
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from basinmaker.func.arcgis import *
-from basinmaker.func.pdtable import *
-
-arcpy.env.overwriteOutput = True
-arcpy.CheckOutExtension("Spatial")
-
-
-def Locate_subid_needsbyuser_arcgis(
-    Path_Points="#", Gauge_NMS="#", Path_products="#"
-):
-    """Get Subbasin Ids
-
-    Function that used to obtain subbasin ID of certain gauge.
-    or subbasin ID of the polygon that includes the given point
-    shapefile.
-
-    Parameters
-    ----------
-    Path_Points      : string (Optional)
-        It is the path of the point shapefile. If the point shapefile is
-        provided. The function will return subids of those catchment
-        polygons that includes these point in the point shapefile
-
-    Gauge_NMS        : list
-        Name of the streamflow gauges, such as ['09PC019'], if the gauge
-        name is provided, the subbasin ID that contain this gauge will be
-        returned
-    Path_products    : string
-        The path of the subbasin polygon shapefile.
-        The shapefile should at least contains following columns
-        ##############Subbasin related attributes###########################
-        SubID           - integer, The subbasin Id
-        DowSubId        - integer, The downstream subbasin ID of this
-                                   subbasin
-        Obs_NM          - The streamflow obervation gauge name.
-
-    Notes
-    -------
-    Path_Points or Gauge_NMS should only provide one each time
-    to use this function
-
-    Returns:
-    -------
-    SubId_Selected  : list
-        It is a list contains the selected subid based on provided
-        streamflow gauge name or provided point shapefile
-
-    Examples
-    -------
-
-    """
-
-    tempfolder = os.path.join(
-        tempfile.gettempdir(),
-        "basinmaker_locsubid" + str(np.random.randint(1, 10000 + 1)),
-    )
-    if not os.path.exists(tempfolder):
-        os.makedirs(tempfolder)
-    arcpy.env.workspace = tempfolder
-
-    SubId_Selected = -1
-    if Gauge_NMS[0] != "#":
-
-        hyshdinfo2 = pd.DataFrame.spatial.from_featureclass(Path_products)
-        hyshdinfo2 = hyshdinfo2.loc[hyshdinfo2["Obs_NM"] != "-9999.0"]
-        hyshdinfo2 = hyshdinfo2.loc[hyshdinfo2["Obs_NM"].isin(Gauge_NMS)]
-        hyshdinfo2 = hyshdinfo2[["Obs_NM", "SubId"]]
-        #            hyshdinfo2.to_csv(os.path.join(self.OutputFolder,'SubIds_Selected.csv'),sep=',', index = None)
-        SubId_Selected = hyshdinfo2["SubId"].values
-
-    if Path_Points != "#":
-        SpRef_in = arcpy.Describe(Path_products).spatialReference
-
-        arcpy.Project_management(Path_products,"Obspoint_project2.shp", out_coordinate_system)
-
-
-
-        arcpy.SpatialJoin_analysis("Obspoint_project2.shp", Path_products, 'Sub_Selected_by_Points')
-
-        hyshdinfo2 = Outputfilename_cat(os.path.join(tempfolder, "Sub_Selected_by_Points.shp"))
-
-        SubId_Selected = hyshdinfo2["SubId"].values
-        SubId_Selected = SubId_Selected[SubId_Selected > 0]
-
-    return SubId_Selected
-
-
-def Select_Routing_product_based_SubId_arcgis(
-    OutputFolder,
-    Routing_Product_Folder,
-    mostdownid=-1,
-    mostupstreamid=-1,
-):
-    """Extract region of interest based on provided Subid
-
-    Function that used to obtain the region of interest from routing
-    product based on given SubId
-
-    Parameters
-    ----------
-    OutputFolder                   : string
-        Folder path that stores extracted routing product
-    Path_Catchment_Polygon         : string
-        Path to the catchment polygon
-    Path_River_Polyline            : string (optional)
-        Path to the river polyline
-    Path_Con_Lake_ply              : string (optional)
-        Path to a connected lake polygon. Connected lakes are lakes that
-        are connected by Path_final_cat_riv or Path_final_riv.
-    Path_NonCon_Lake_ply           : string (optional)
-        Path to a non connected lake polygon. Connected lakes are lakes
-        that are not connected by Path_final_cat_riv or Path_final_riv.
-    mostdownid                     : integer
-        It is the most downstream subbasin ID in the region of interest
-    mostupstreamid                 : integer (optional)
-        It is the most upstream subbasin ID in the region of interest.
-        Normally it is -1, indicating all subbasin drainage to mostdownid
-        is needed. In some case, if not all subbasin drainage to mostdownid
-        is needed, then the most upstream subbsin ID need to be provided
-        here.
-
-
-    Notes
-    -------
-    This function has no return values, instead following fiels will be
-    generated. The output files have are same as inputs expect the extent
-    are different.
-
-    os.path.join(OutputFolder,os.path.basename(Path_Catchment_Polygon))
-    os.path.join(OutputFolder,os.path.basename(Path_River_Polyline))
-    os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply))
-    os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply))
-
-    Returns:
-    -------
-    None
-
-    Examples
-    -------
-
-    """
-    tempfolder = os.path.join(
-        tempfile.gettempdir(),
-        "basinmaker_locsubid" + str(101),#np.random.randint(1, 10000 + 1)),
-    )
-    if not os.path.exists(tempfolder):
-        os.makedirs(tempfolder)
-    arcpy.env.workspace = tempfolder
-
-
-    Path_Catchment_Polygon="#"
-    Path_River_Polyline="#"
-    Path_Con_Lake_ply="#"
-    Path_NonCon_Lake_ply="#"
-    Path_obs_gauge_point="#"
-    Path_final_cat_ply="#"
-    Path_final_cat_riv="#"
-
-    ##define input files from routing prodcut 
-    for file in os.listdir(Routing_Product_Folder):
-        if file.endswith(".shp"):
-            if 'catchment_without_merging_lakes' in file:
-                Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
-            if 'river_without_merging_lakes' in file:
-                Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
-            if 'sl_connected_lake' in file:
-                Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'sl_non_connected_lake' in file:
-                Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
-            if 'obs_gauges' in file:
-                Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
-            if 'finalcat_info' in file:
-                Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
-            if 'finalcat_info_riv' in file:
-                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)                
-
-    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
-        print("Invalid routing product folder ")
-        arcpy.AddMessage(Path_Catchment_Polygon)
-        return()
-
-
-
-    sub_colnm = "SubId"
-    down_colnm = "DowSubId"
-
-    ##3
-    
-    cat_ply = pd.DataFrame.spatial.from_featureclass(Path_Catchment_Polygon)
-
-    hyshdinfo = cat_ply[[sub_colnm, down_colnm]].astype("int32").values
-
-    Gauge_col_Name = "Has_POI"
-    if "Has_POI" not in cat_ply.columns:
-        Gauge_col_Name = "Has_Gauge"
-        
-    ### Loop for each downstream id
-
-    if not os.path.exists(OutputFolder):
-        os.makedirs(OutputFolder)
-
-    ## find all subid control by this subid
-    for i_down in range(0,len(mostdownid)):
-        ### Loop for each downstream id
-        OutHyID = mostdownid[i_down]
-        OutHyID2 = mostupstreamid[i_down]
-            
-        ## find all subid control by this subid
-        HydroBasins1 = defcat(hyshdinfo, OutHyID)
-        if OutHyID2 > 0:
-            HydroBasins2 = defcat(hyshdinfo, OutHyID2)
-            ###  exculde the Ids in HydroBasins2 from HydroBasins1
-            for i in range(len(HydroBasins2)):
-                rows = np.argwhere(HydroBasins1 == HydroBasins2[i])
-                HydroBasins1 = np.delete(HydroBasins1, rows)
-            HydroBasins = HydroBasins1
-        else:
-            HydroBasins = HydroBasins1
-
-        if i_down == 0:
-            HydroBasins_All = HydroBasins
-        else:
-            HydroBasins_All = np.concatenate((HydroBasins_All, HydroBasins), axis=0)
-
-    Outputfilename_cat = os.path.join(
-        OutputFolder, os.path.basename(Path_Catchment_Polygon)
-    )
-
-    cat_ply_select = cat_ply.loc[cat_ply['SubId'].isin(HydroBasins_All)]
-
-    cat_ply_select.spatial.to_featureclass(location=Outputfilename_cat,overwrite=True,sanitize_columns=False) 
-    Outputfilename_cat_riv = os.path.join(
-        OutputFolder, os.path.basename(Path_River_Polyline)
-    )
-
-    cat_riv = pd.DataFrame.spatial.from_featureclass(Path_River_Polyline)
-    
-
-    cat_riv_select = cat_riv.loc[cat_riv['SubId'].isin(HydroBasins)]
-    
-    cat_riv_select.spatial.to_featureclass(location=Outputfilename_cat_riv,overwrite=True,sanitize_columns=False) 
-    
-    cat_ply_select = pd.DataFrame.spatial.from_featureclass(Outputfilename_cat)
-    Connect_Lake_info = cat_ply_select.loc[cat_ply_select["Lake_Cat"] == 1]
-    Connect_Lakeids = np.unique(Connect_Lake_info["HyLakeId"].values)
-    Connect_Lakeids = Connect_Lakeids[Connect_Lakeids > 0]
-    
-    NConnect_Lake_info = cat_ply_select.loc[cat_ply_select["Lake_Cat"] == 2]
-    NonCL_Lakeids = np.unique(NConnect_Lake_info["HyLakeId"].values)
-    NonCL_Lakeids = NonCL_Lakeids[NonCL_Lakeids > 0]
-
-    if len(Connect_Lakeids) > 0 and Path_Con_Lake_ply != "#":
-
-        sl_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_Con_Lake_ply)
-        sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Connect_Lakeids)]
-        sl_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply)),overwrite=True,sanitize_columns=False)
-
-
-    if len(NonCL_Lakeids) > 0 and Path_NonCon_Lake_ply != "#":
-        sl_non_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)
-        sl_non_con_lakes = sl_non_con_lakes.loc[sl_non_con_lakes['Hylak_id'].isin(NonCL_Lakeids)]
-        sl_non_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)),overwrite=True,sanitize_columns=False)
-    
-    sl_gauge_info = cat_ply_select.loc[cat_ply_select[Gauge_col_Name] > 0]
-    sl_gauge_nm = np.unique(sl_gauge_info["Obs_NM"].values)
-    sl_gauge_nm = sl_gauge_nm[sl_gauge_nm != 'nan']
-    if len(sl_gauge_nm) > 0 and Path_obs_gauge_point !='#':
-        all_gauge = pd.DataFrame.spatial.from_featureclass(Path_obs_gauge_point)
-        sl_gauge = all_gauge.loc[all_gauge['Obs_NM'].isin(sl_gauge_nm)]
-        sl_gauge.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_obs_gauge_point)),overwrite=True,sanitize_columns=False)
-    
-    return 
-
-
-################################################################
+
+import numpy as np
+import arcpy
+from arcpy import env
+from arcpy.sa import *
+from arcgis.features import GeoAccessor, GeoSeriesAccessor
+import sys
+import os
+import csv
+import pandas as pd
+import tempfile
+import copy
+
+import sys, os
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from basinmaker.func.arcgis import *
+from basinmaker.func.pdtable import *
+
+arcpy.env.overwriteOutput = True
+arcpy.CheckOutExtension("Spatial")
+
+
+def Locate_subid_needsbyuser_arcgis(
+    Path_Points="#", Gauge_NMS="#", Path_products="#"
+):
+    """Get Subbasin Ids
+
+    Function that used to obtain subbasin ID of certain gauge.
+    or subbasin ID of the polygon that includes the given point
+    shapefile.
+
+    Parameters
+    ----------
+    Path_Points      : string (Optional)
+        It is the path of the point shapefile. If the point shapefile is
+        provided. The function will return subids of those catchment
+        polygons that includes these point in the point shapefile
+
+    Gauge_NMS        : list
+        Name of the streamflow gauges, such as ['09PC019'], if the gauge
+        name is provided, the subbasin ID that contain this gauge will be
+        returned
+    Path_products    : string
+        The path of the subbasin polygon shapefile.
+        The shapefile should at least contains following columns
+        ##############Subbasin related attributes###########################
+        SubID           - integer, The subbasin Id
+        DowSubId        - integer, The downstream subbasin ID of this
+                                   subbasin
+        Obs_NM          - The streamflow obervation gauge name.
+
+    Notes
+    -------
+    Path_Points or Gauge_NMS should only provide one each time
+    to use this function
+
+    Returns:
+    -------
+    SubId_Selected  : list
+        It is a list contains the selected subid based on provided
+        streamflow gauge name or provided point shapefile
+
+    Examples
+    -------
+
+    """
+
+    tempfolder = os.path.join(
+        tempfile.gettempdir(),
+        "basinmaker_locsubid" + str(np.random.randint(1, 10000 + 1)),
+    )
+    if not os.path.exists(tempfolder):
+        os.makedirs(tempfolder)
+    arcpy.env.workspace = tempfolder
+
+    SubId_Selected = -1
+    if Gauge_NMS[0] != "#":
+
+        hyshdinfo2 = pd.DataFrame.spatial.from_featureclass(Path_products)
+        hyshdinfo2 = hyshdinfo2.loc[hyshdinfo2["Obs_NM"] != "-9999.0"]
+        hyshdinfo2 = hyshdinfo2.loc[hyshdinfo2["Obs_NM"].isin(Gauge_NMS)]
+        hyshdinfo2 = hyshdinfo2[["Obs_NM", "SubId"]]
+        #            hyshdinfo2.to_csv(os.path.join(self.OutputFolder,'SubIds_Selected.csv'),sep=',', index = None)
+        SubId_Selected = hyshdinfo2["SubId"].values
+
+    if Path_Points != "#":
+        SpRef_in = arcpy.Describe(Path_products).spatialReference
+
+        arcpy.Project_management(Path_products,"Obspoint_project2.shp", out_coordinate_system)
+
+
+
+        arcpy.SpatialJoin_analysis("Obspoint_project2.shp", Path_products, 'Sub_Selected_by_Points')
+
+        hyshdinfo2 = Outputfilename_cat(os.path.join(tempfolder, "Sub_Selected_by_Points.shp"))
+
+        SubId_Selected = hyshdinfo2["SubId"].values
+        SubId_Selected = SubId_Selected[SubId_Selected > 0]
+
+    return SubId_Selected
+
+
+def Select_Routing_product_based_SubId_arcgis(
+    OutputFolder,
+    Routing_Product_Folder,
+    mostdownid=-1,
+    mostupstreamid=-1,
+):
+    """Extract region of interest based on provided Subid
+
+    Function that used to obtain the region of interest from routing
+    product based on given SubId
+
+    Parameters
+    ----------
+    OutputFolder                   : string
+        Folder path that stores extracted routing product
+    Path_Catchment_Polygon         : string
+        Path to the catchment polygon
+    Path_River_Polyline            : string (optional)
+        Path to the river polyline
+    Path_Con_Lake_ply              : string (optional)
+        Path to a connected lake polygon. Connected lakes are lakes that
+        are connected by Path_final_cat_riv or Path_final_riv.
+    Path_NonCon_Lake_ply           : string (optional)
+        Path to a non connected lake polygon. Connected lakes are lakes
+        that are not connected by Path_final_cat_riv or Path_final_riv.
+    mostdownid                     : integer
+        It is the most downstream subbasin ID in the region of interest
+    mostupstreamid                 : integer (optional)
+        It is the most upstream subbasin ID in the region of interest.
+        Normally it is -1, indicating all subbasin drainage to mostdownid
+        is needed. In some case, if not all subbasin drainage to mostdownid
+        is needed, then the most upstream subbsin ID need to be provided
+        here.
+
+
+    Notes
+    -------
+    This function has no return values, instead following fiels will be
+    generated. The output files have are same as inputs expect the extent
+    are different.
+
+    os.path.join(OutputFolder,os.path.basename(Path_Catchment_Polygon))
+    os.path.join(OutputFolder,os.path.basename(Path_River_Polyline))
+    os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply))
+    os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply))
+
+    Returns:
+    -------
+    None
+
+    Examples
+    -------
+
+    """
+    tempfolder = os.path.join(
+        tempfile.gettempdir(),
+        "basinmaker_locsubid" + str(101),#np.random.randint(1, 10000 + 1)),
+    )
+    if not os.path.exists(tempfolder):
+        os.makedirs(tempfolder)
+    arcpy.env.workspace = tempfolder
+
+
+    Path_Catchment_Polygon="#"
+    Path_River_Polyline="#"
+    Path_Con_Lake_ply="#"
+    Path_NonCon_Lake_ply="#"
+    Path_obs_gauge_point="#"
+    Path_final_cat_ply="#"
+    Path_final_cat_riv="#"
+
+    ##define input files from routing prodcut
+    for file in os.listdir(Routing_Product_Folder):
+        if file.endswith(".shp"):
+            if 'catchment_without_merging_lakes' in file:
+                Path_Catchment_Polygon = os.path.join(Routing_Product_Folder, file)
+            if 'river_without_merging_lakes' in file:
+                Path_River_Polyline = os.path.join(Routing_Product_Folder, file)
+            if 'sl_connected_lake' in file:
+                Path_Con_Lake_ply = os.path.join(Routing_Product_Folder, file)
+            if 'sl_non_connected_lake' in file:
+                Path_NonCon_Lake_ply = os.path.join(Routing_Product_Folder, file)
+            if 'obs_gauges' in file or 'poi' in file:
+                Path_obs_gauge_point = os.path.join(Routing_Product_Folder, file)
+            if 'finalcat_info' in file:
+                Path_final_cat_ply = os.path.join(Routing_Product_Folder, file)
+            if 'finalcat_info_riv' in file:
+                Path_final_cat_riv = os.path.join(Routing_Product_Folder, file)
+
+    if Path_Catchment_Polygon == '#' or  Path_River_Polyline =='#':
+        print("Invalid routing product folder ")
+        arcpy.AddMessage(Path_Catchment_Polygon)
+        return()
+
+
+
+    sub_colnm = "SubId"
+    down_colnm = "DowSubId"
+
+    ##3
+
+    cat_ply = pd.DataFrame.spatial.from_featureclass(Path_Catchment_Polygon)
+
+    hyshdinfo = cat_ply[[sub_colnm, down_colnm]].astype("int32").values
+
+    Gauge_col_Name = "Has_POI"
+    if "Has_POI" not in cat_ply.columns:
+        Gauge_col_Name = "Has_Gauge"
+
+    ### Loop for each downstream id
+
+    if not os.path.exists(OutputFolder):
+        os.makedirs(OutputFolder)
+
+    ## find all subid control by this subid
+    for i_down in range(0,len(mostdownid)):
+        ### Loop for each downstream id
+        OutHyID = mostdownid[i_down]
+        OutHyID2 = mostupstreamid[i_down]
+
+        ## find all subid control by this subid
+        HydroBasins1 = defcat(hyshdinfo, OutHyID)
+        if OutHyID2 > 0:
+            HydroBasins2 = defcat(hyshdinfo, OutHyID2)
+            ###  exculde the Ids in HydroBasins2 from HydroBasins1
+            for i in range(len(HydroBasins2)):
+                rows = np.argwhere(HydroBasins1 == HydroBasins2[i])
+                HydroBasins1 = np.delete(HydroBasins1, rows)
+            HydroBasins = HydroBasins1
+        else:
+            HydroBasins = HydroBasins1
+
+        if i_down == 0:
+            HydroBasins_All = HydroBasins
+        else:
+            HydroBasins_All = np.concatenate((HydroBasins_All, HydroBasins), axis=0)
+
+    Outputfilename_cat = os.path.join(
+        OutputFolder, os.path.basename(Path_Catchment_Polygon)
+    )
+
+    cat_ply_select = cat_ply.loc[cat_ply['SubId'].isin(HydroBasins_All)]
+
+    cat_ply_select.spatial.to_featureclass(location=Outputfilename_cat,overwrite=True,sanitize_columns=False)
+    Outputfilename_cat_riv = os.path.join(
+        OutputFolder, os.path.basename(Path_River_Polyline)
+    )
+
+    cat_riv = pd.DataFrame.spatial.from_featureclass(Path_River_Polyline)
+
+
+    cat_riv_select = cat_riv.loc[cat_riv['SubId'].isin(HydroBasins_All)]
+
+    cat_riv_select.spatial.to_featureclass(location=Outputfilename_cat_riv,overwrite=True,sanitize_columns=False)
+
+    cat_ply_select = pd.DataFrame.spatial.from_featureclass(Outputfilename_cat)
+    Connect_Lake_info = cat_ply_select.loc[cat_ply_select["Lake_Cat"] == 1]
+    Connect_Lakeids = np.unique(Connect_Lake_info["HyLakeId"].values)
+    Connect_Lakeids = Connect_Lakeids[Connect_Lakeids > 0]
+
+    NConnect_Lake_info = cat_ply_select.loc[cat_ply_select["Lake_Cat"] == 2]
+    NonCL_Lakeids = np.unique(NConnect_Lake_info["HyLakeId"].values)
+    NonCL_Lakeids = NonCL_Lakeids[NonCL_Lakeids > 0]
+
+    if len(Connect_Lakeids) > 0 and Path_Con_Lake_ply != "#":
+
+        sl_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_Con_Lake_ply)
+        sl_con_lakes = sl_con_lakes.loc[sl_con_lakes['Hylak_id'].isin(Connect_Lakeids)]
+        if len(sl_con_lakes) > 0:
+            sl_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_Con_Lake_ply)),overwrite=True,sanitize_columns=False)
+
+
+    if len(NonCL_Lakeids) > 0 and Path_NonCon_Lake_ply != "#":
+        sl_non_con_lakes = pd.DataFrame.spatial.from_featureclass(Path_NonCon_Lake_ply)
+        sl_non_con_lakes = sl_non_con_lakes.loc[sl_non_con_lakes['Hylak_id'].isin(NonCL_Lakeids)]
+        if len(sl_non_con_lakes) > 0:
+            sl_non_con_lakes.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_NonCon_Lake_ply)),overwrite=True,sanitize_columns=False)
+
+    sl_gauge_info = cat_ply_select.loc[cat_ply_select[Gauge_col_Name] > 0]
+    sl_gauge_nm = np.unique(sl_gauge_info["Obs_NM"].values)
+    sl_gauge_nm = sl_gauge_nm[sl_gauge_nm != 'nan']
+    if len(sl_gauge_nm) > 0 and Path_obs_gauge_point !='#':
+        all_gauge = pd.DataFrame.spatial.from_featureclass(Path_obs_gauge_point)
+        sl_gauge = all_gauge.loc[all_gauge['Obs_NM'].isin(sl_gauge_nm)]
+        sl_gauge.spatial.to_featureclass(location=os.path.join(OutputFolder,os.path.basename(Path_obs_gauge_point)),overwrite=True,sanitize_columns=False)
+
+    return
+
+
+################################################################
```

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/preinputpolygonqgis.py` & `basinmaker-3.0.3/basinmaker/preprocessing/preinputpolygonqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/preprocessinglakeply.py` & `basinmaker-3.0.3/basinmaker/preprocessing/preprocessinglakeply.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/preprocessingobs.py` & `basinmaker-3.0.3/basinmaker/preprocessing/preprocessingobs.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/preprocessrasterqgis.py` & `basinmaker-3.0.3/basinmaker/preprocessing/preprocessrasterqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py` & `basinmaker-3.0.3/basinmaker/preprocessing/rasterizevectorsandloadtodbqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py` & `basinmaker-3.0.3/basinmaker/preprocessing/reprojectandclipvectorbyplyqgis.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/subreg/defsubreg.py` & `basinmaker-3.0.3/basinmaker/subreg/defsubreg.py`

 * *Files identical despite different names*

### Comparing `basinmaker-3.0.1/basinmaker/utilities/utilities.py` & `basinmaker-3.0.3/basinmaker/utilities/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import os
-
+import glob,shutil
 from simpledbf import Dbf5
 
 # define internal file names
+def copy_files_with_extension(src_folder,tar_folder,ext):
+
+    files = glob.iglob(os.path.join(src_folder, ext))
+    for file in files:
+        if os.path.isfile(file):
+            t = shutil.copy2(file, tar_folder)
+
 Internal_Constant_Names = {
     "cat_add_lake_old_fdr": "cat_add_lake_old_fdr",
     "cat_add_lake": "cat_add_lake",
     "pourpoints_add_obs": "pourpoints_add_obs",
     "all_lakes": "all_lakes",
     "lake_boundary": "lake_boundary",
     "connect_lake": "connect_lake",
@@ -76,14 +83,16 @@
     "centroid_x",
     "centroid_y",
     "DA_Chn_L",
     "DA_Slope",
     "DA_Chn_Slp",
     "outletLat",
     "outletLng",
+    "k",
+    "c",
 ]
 
 COLUMN_NAMES_CONSTANT_CLEAN = [
     "SubId",
     "DowSubId",
     "RivSlope",
     "RivLength",
@@ -116,15 +125,17 @@
     "centroid_x",
     "centroid_y",
     "DA_Chn_L",
     "DA_Slope",
     "DA_Chn_Slp",
     "outletLat",
     "outletLng",
-    "Has_Gauge"
+    "Has_Gauge",
+    "k",
+    "c",
 ]
 
 
 COLUMN_NAMES_With_NULL_Values = [
     "Lake_Cat",
     "HyLakeId",
     "LakeVol",
@@ -186,15 +197,15 @@
     "HRU_S_mean",
     "HRU_A_mean",
     "HRU_E_mean",
     "SHAPE",
     "DA_Chn_L",
     "DA_Slope",
     "DA_Chn_Slp",
-    "Has_Gauge" ,   
+    "Has_Gauge" ,
 ]
 
 
 COLUMN_TYPES_CONSTANT = [
     "Integer",
     "Integer",
     "Real",
@@ -228,25 +239,27 @@
     "Real",
     "Real",
     "Real",
     "Real",
     "Real",
     "Real",
     "Real",
+    "Real",
+    "Real",
 ]
 
 DEFALUT_FLOOD_N = 0.09
 min_manning_n = 0.025
 max_manning_n = 0.15
 min_riv_slope = 0.000001
 max_riv_slope = 1
 min_bkf_width = 0.1
 min_bkf_depth = 0.1
 min_riv_lenth = 90
-    
+
 def Dbf_To_Dataframe(file_path):
     """Transfer an input dbf file to dataframe
 
     Parameters
     ----------
     file_path   : string
     Full path to a shapefile
```

### Comparing `basinmaker-3.0.1/basinmaker.egg-info/PKG-INFO` & `basinmaker-3.0.3/basinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basinmaker
-Version: 3.0.1
+Version: 3.0.3
 Summary: An automated GIS toolbox for watershed delineation with lakes
 Home-page: https://github.com/dustming/basinmaker
 Author: basinmaker development team
 Author-email: m43han@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `basinmaker-3.0.1/setup.py` & `basinmaker-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="basinmaker",
-    version="3.0.1",
+    version="3.0.3",
     author="basinmaker development team",
     author_email="m43han@uwaterloo.ca",
     description="An automated GIS toolbox for watershed delineation with lakes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dustming/basinmaker",
     packages = setuptools.find_packages(
```

