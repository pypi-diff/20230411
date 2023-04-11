# Comparing `tmp/pyfmtools-0.80.tar.gz` & `tmp/pyfmtools-0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmtools-0.80.tar", last modified: Mon Mar 27 07:12:44 2023, max compression
+gzip compressed data, was "pyfmtools-0.81.tar", last modified: Tue Apr 11 01:52:08 2023, max compression
```

## Comparing `pyfmtools-0.80.tar` & `pyfmtools-0.81.tar`

### file list

```diff
@@ -1,110 +1,112 @@
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-03-27 07:12:44.184169 pyfmtools-0.80/
--rw-r--r--   0 nhenseler   (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-0.80/LICENSE.txt
--rw-rw-r--   0 nhenseler   (501) staff       (20)      211 2022-06-27 07:31:35.000000 pyfmtools-0.80/MANIFEST.in
--rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-03-27 07:12:44.183657 pyfmtools-0.80/PKG-INFO
--rw-rw-r--   0 nhenseler   (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-0.80/README.md
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-03-27 07:12:43.709676 pyfmtools-0.80/dist/
--rw-r--r--   0 nhenseler   (501) staff       (20)   435980 2023-03-27 07:12:43.000000 pyfmtools-0.80/dist/pyfmtools-0.80-cp39-cp39-macosx_10_9_x86_64.whl
--rw-r--r--   0 nhenseler   (501) staff       (20)       38 2023-03-27 07:12:44.184290 pyfmtools-0.80/setup.cfg
--rw-r--r--   0 nhenseler   (501) staff       (20)      946 2023-03-27 07:09:03.000000 pyfmtools-0.80/setup.py
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-03-27 07:12:44.176225 pyfmtools-0.80/src/
--rw-------   0 nhenseler   (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-0.80/src/binarylattice.h
--rw-r--r--   0 nhenseler   (501) staff       (20)    10148 2022-05-23 02:31:18.000000 pyfmtools-0.80/src/buildPyfmtools.py
--rw-------   0 nhenseler   (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-0.80/src/colamd.c
--rw-------   0 nhenseler   (501) staff       (20)     9804 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/colamd.h
--rw-------   0 nhenseler   (501) staff       (20)    19373 2020-04-28 01:07:53.000000 pyfmtools-0.80/src/commonlib.c
--rw-------   0 nhenseler   (501) staff       (20)     8894 2020-04-28 01:28:51.000000 pyfmtools-0.80/src/commonlib.h
--rw-------   0 nhenseler   (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/declare.h
--rw-------   0 nhenseler   (501) staff       (20)    26583 2021-02-16 05:37:08.000000 pyfmtools-0.80/src/fmrandom.cpp
--rw-------   0 nhenseler   (501) staff       (20)     6042 2021-02-15 23:08:21.000000 pyfmtools-0.80/src/fmrandom.h
--rw-------   0 nhenseler   (501) staff       (20)     7326 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/fortify.h
--rw-------   0 nhenseler   (501) staff       (20)    42931 2021-06-26 11:56:42.000000 pyfmtools-0.80/src/fuzzymeasurefit.cpp
--rw-------   0 nhenseler   (501) staff       (20)    10458 2020-09-15 03:02:02.000000 pyfmtools-0.80/src/fuzzymeasurefit.h
--rw-------   0 nhenseler   (501) staff       (20)    46580 2021-02-12 00:35:43.000000 pyfmtools-0.80/src/fuzzymeasurefit3.cpp
--rw-------   0 nhenseler   (501) staff       (20)    53584 2022-03-23 22:37:43.000000 pyfmtools-0.80/src/fuzzymeasuretools.cpp
--rw-------   0 nhenseler   (501) staff       (20)    19772 2022-05-19 03:16:38.000000 pyfmtools-0.80/src/fuzzymeasuretools.h
--rw-------   0 nhenseler   (501) staff       (20)      750 2022-04-13 06:22:25.000000 pyfmtools-0.80/src/generaldefs.h
--rw-------   0 nhenseler   (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-0.80/src/hbio.h
--rw-------   0 nhenseler   (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-0.80/src/ini.c
--rw-------   0 nhenseler   (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/ini.h
--rw-------   0 nhenseler   (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-0.80/src/isfixedvar.c
--rw-------   0 nhenseler   (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_BFP.h
--rw-------   0 nhenseler   (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_BFP1.h
--rw-------   0 nhenseler   (501) staff       (20)     4444 2021-02-16 05:56:16.000000 pyfmtools-0.80/src/lp_BFP2.h
--rw-------   0 nhenseler   (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-0.80/src/lp_Hash.c
--rw-------   0 nhenseler   (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_Hash.h
--rw-------   0 nhenseler   (501) staff       (20)    23763 2020-09-15 01:45:42.000000 pyfmtools-0.80/src/lp_LUSOL.c
--rw-------   0 nhenseler   (501) staff       (20)     2818 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_LUSOL.h
--rw-------   0 nhenseler   (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_MDO.c
--rw-------   0 nhenseler   (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_MDO.h
--rw-------   0 nhenseler   (501) staff       (20)    53842 2021-02-16 06:53:34.000000 pyfmtools-0.80/src/lp_MPS.c
--rw-------   0 nhenseler   (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_MPS.h
--rw-------   0 nhenseler   (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-0.80/src/lp_SOS.c
--rw-------   0 nhenseler   (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_SOS.h
--rw-------   0 nhenseler   (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_crash.c
--rw-------   0 nhenseler   (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_crash.h
--rw-------   0 nhenseler   (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-0.80/src/lp_etaPFI.h
--rw-------   0 nhenseler   (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_explicit.h
--rw-------   0 nhenseler   (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_fortify.h
--rw-------   0 nhenseler   (501) staff       (20)   286090 2022-05-23 02:33:29.000000 pyfmtools-0.80/src/lp_lib.c
--rw-------   0 nhenseler   (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-0.80/src/lp_lib.h
--rw-------   0 nhenseler   (501) staff       (20)    96546 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_matrix.c
--rw-------   0 nhenseler   (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_matrix.h
--rw-------   0 nhenseler   (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-0.80/src/lp_mipbb.c
--rw-------   0 nhenseler   (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_mipbb.h
--rw-------   0 nhenseler   (501) staff       (20)    23491 2021-02-12 00:36:06.000000 pyfmtools-0.80/src/lp_params.c
--rw-------   0 nhenseler   (501) staff       (20)   184143 2021-07-24 00:59:10.000000 pyfmtools-0.80/src/lp_presolve.c
--rw-------   0 nhenseler   (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_presolve.h
--rw-------   0 nhenseler   (501) staff       (20)    68918 2020-09-24 08:24:57.000000 pyfmtools-0.80/src/lp_price.c
--rw-------   0 nhenseler   (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_price.h
--rw-------   0 nhenseler   (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_pricePSE.c
--rw-------   0 nhenseler   (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_pricePSE.h
--rw-------   0 nhenseler   (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-0.80/src/lp_report.c
--rw-------   0 nhenseler   (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_report.h
--rw-------   0 nhenseler   (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-0.80/src/lp_rlp.h
--rw-------   0 nhenseler   (501) staff       (20)    29508 2017-12-15 12:16:42.000000 pyfmtools-0.80/src/lp_scale.c
--rw-------   0 nhenseler   (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_scale.h
--rw-------   0 nhenseler   (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-0.80/src/lp_simplex.c
--rw-------   0 nhenseler   (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_simplex.h
--rw-------   0 nhenseler   (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-0.80/src/lp_types.h
--rw-------   0 nhenseler   (501) staff       (20)    26914 2020-09-24 08:01:30.000000 pyfmtools-0.80/src/lp_utils.c
--rw-------   0 nhenseler   (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_utils.h
--rw-------   0 nhenseler   (501) staff       (20)    11210 2020-04-28 01:15:38.000000 pyfmtools-0.80/src/lp_wlp.c
--rw-------   0 nhenseler   (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lp_wlp.h
--rw-------   0 nhenseler   (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-0.80/src/lpkit.h
--rw-------   0 nhenseler   (501) staff       (20)    21870 2020-09-24 08:24:40.000000 pyfmtools-0.80/src/lpslink56.c
--rw-------   0 nhenseler   (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lpsolve.h
--rw-------   0 nhenseler   (501) staff       (20)    24934 2020-04-28 01:21:09.000000 pyfmtools-0.80/src/lusol.c
--rw-------   0 nhenseler   (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol.h
--rw-------   0 nhenseler   (501) staff       (20)   135944 2017-12-15 11:57:34.000000 pyfmtools-0.80/src/lusol1.h
--rw-------   0 nhenseler   (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol2.h
--rw-------   0 nhenseler   (501) staff       (20)    28424 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol6a.h
--rw-------   0 nhenseler   (501) staff       (20)     4498 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol6l0.h
--rw-------   0 nhenseler   (501) staff       (20)     4899 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol6u.h
--rw-------   0 nhenseler   (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol7a.h
--rw-------   0 nhenseler   (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusol8a.h
--rw-------   0 nhenseler   (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-0.80/src/lusolio.c
--rw-------   0 nhenseler   (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/lusolio.h
--rw-------   0 nhenseler   (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-0.80/src/minimalsplus.h
--rw-------   0 nhenseler   (501) staff       (20)    13025 2020-04-28 01:15:38.000000 pyfmtools-0.80/src/mmio.c
--rw-------   0 nhenseler   (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/mmio.h
--rw-------   0 nhenseler   (501) staff       (20)    19312 2020-04-28 01:22:16.000000 pyfmtools-0.80/src/myblas.c
--rw-------   0 nhenseler   (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-0.80/src/myblas.h
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-03-27 07:12:44.180709 pyfmtools-0.80/src/pyfmtools.egg-info/
--rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-03-27 07:12:42.000000 pyfmtools-0.80/src/pyfmtools.egg-info/PKG-INFO
--rw-r--r--   0 nhenseler   (501) staff       (20)     1718 2023-03-27 07:12:42.000000 pyfmtools-0.80/src/pyfmtools.egg-info/SOURCES.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)        1 2023-03-27 07:12:42.000000 pyfmtools-0.80/src/pyfmtools.egg-info/dependency_links.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       12 2023-03-27 07:12:42.000000 pyfmtools-0.80/src/pyfmtools.egg-info/requires.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)       21 2023-03-27 07:12:42.000000 pyfmtools-0.80/src/pyfmtools.egg-info/top_level.txt
--rw-r--r--   0 nhenseler   (501) staff       (20)    48236 2023-03-27 07:08:40.000000 pyfmtools-0.80/src/pyfmtools.py
--rw-------   0 nhenseler   (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-0.80/src/sparselib.c
--rw-------   0 nhenseler   (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/sparselib.h
--rw-------   0 nhenseler   (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-0.80/src/stdafx.h
--rw-------   0 nhenseler   (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-0.80/src/ufortify.h
--rw-------   0 nhenseler   (501) staff       (20)    87216 2022-05-23 02:18:42.000000 pyfmtools-0.80/src/wrapperpy.cpp
--rw-------   0 nhenseler   (501) staff       (20)    14390 2022-05-20 09:48:18.000000 pyfmtools-0.80/src/wrapperpy.h
--rw-------   0 nhenseler   (501) staff       (20)    28266 2020-09-24 07:46:24.000000 pyfmtools-0.80/src/yacc_read.c
--rw-------   0 nhenseler   (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-0.80/src/yacc_read.h
-drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-03-27 07:12:44.183092 pyfmtools-0.80/tests/
--rw-------   0 nhenseler   (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-0.80/tests/test_no_wrapper.py
--rw-r--r--   0 nhenseler   (501) staff       (20)    27771 2022-06-28 04:36:04.000000 pyfmtools-0.80/tests/test_wrapper.py
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.689706 pyfmtools-0.81/
+-rw-r--r--   0 nhenseler   (501) staff       (20)     7652 2022-04-26 03:16:57.000000 pyfmtools-0.81/LICENSE.txt
+-rw-rw-r--   0 nhenseler   (501) staff       (20)      211 2022-06-27 07:31:35.000000 pyfmtools-0.81/MANIFEST.in
+-rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-04-11 01:52:08.689284 pyfmtools-0.81/PKG-INFO
+-rw-rw-r--   0 nhenseler   (501) staff       (20)     5026 2022-06-20 10:01:16.000000 pyfmtools-0.81/README.md
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.423642 pyfmtools-0.81/dist/
+-rw-r--r--   0 nhenseler   (501) staff       (20)   436101 2023-04-11 01:52:07.000000 pyfmtools-0.81/dist/pyfmtools-0.81-cp39-cp39-macosx_10_9_x86_64.whl
+-rw-r--r--   0 nhenseler   (501) staff       (20)       38 2023-04-11 01:52:08.689870 pyfmtools-0.81/setup.cfg
+-rw-r--r--   0 nhenseler   (501) staff       (20)      946 2023-04-11 01:47:13.000000 pyfmtools-0.81/setup.py
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.681332 pyfmtools-0.81/src/
+-rw-------   0 nhenseler   (501) staff       (20)     1933 2021-02-16 05:49:22.000000 pyfmtools-0.81/src/binarylattice.h
+-rw-r--r--   0 nhenseler   (501) staff       (20)    10148 2022-05-23 02:31:18.000000 pyfmtools-0.81/src/buildPyfmtools.py
+-rw-------   0 nhenseler   (501) staff       (20)   103132 2020-04-28 00:59:43.000000 pyfmtools-0.81/src/colamd.c
+-rw-------   0 nhenseler   (501) staff       (20)     9804 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/colamd.h
+-rw-------   0 nhenseler   (501) staff       (20)    19373 2020-04-28 01:07:53.000000 pyfmtools-0.81/src/commonlib.c
+-rw-------   0 nhenseler   (501) staff       (20)     8894 2020-04-28 01:28:51.000000 pyfmtools-0.81/src/commonlib.h
+-rw-------   0 nhenseler   (501) staff       (20)      389 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/declare.h
+-rw-------   0 nhenseler   (501) staff       (20)    26583 2021-02-16 05:37:08.000000 pyfmtools-0.81/src/fmrandom.cpp
+-rw-------   0 nhenseler   (501) staff       (20)     6042 2021-02-15 23:08:21.000000 pyfmtools-0.81/src/fmrandom.h
+-rw-------   0 nhenseler   (501) staff       (20)     7326 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/fortify.h
+-rw-------   0 nhenseler   (501) staff       (20)    42931 2021-06-26 11:56:42.000000 pyfmtools-0.81/src/fuzzymeasurefit.cpp
+-rw-------   0 nhenseler   (501) staff       (20)    10458 2020-09-15 03:02:02.000000 pyfmtools-0.81/src/fuzzymeasurefit.h
+-rw-------   0 nhenseler   (501) staff       (20)    46580 2021-02-12 00:35:43.000000 pyfmtools-0.81/src/fuzzymeasurefit3.cpp
+-rw-------   0 nhenseler   (501) staff       (20)    53584 2022-03-23 22:37:43.000000 pyfmtools-0.81/src/fuzzymeasuretools.bak.cpp
+-rw-------   0 nhenseler   (501) staff       (20)    19772 2022-05-19 03:16:38.000000 pyfmtools-0.81/src/fuzzymeasuretools.bak.h
+-rw-------   0 nhenseler   (501) staff       (20)    53591 2023-04-11 01:38:11.000000 pyfmtools-0.81/src/fuzzymeasuretools.cpp
+-rw-------   0 nhenseler   (501) staff       (20)    19220 2023-04-11 01:38:11.000000 pyfmtools-0.81/src/fuzzymeasuretools.h
+-rw-------   0 nhenseler   (501) staff       (20)      750 2022-04-13 06:22:25.000000 pyfmtools-0.81/src/generaldefs.h
+-rw-------   0 nhenseler   (501) staff       (20)     2822 2018-03-02 10:06:22.000000 pyfmtools-0.81/src/hbio.h
+-rw-------   0 nhenseler   (501) staff       (20)     1216 2020-09-03 10:46:28.000000 pyfmtools-0.81/src/ini.c
+-rw-------   0 nhenseler   (501) staff       (20)      394 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/ini.h
+-rw-------   0 nhenseler   (501) staff       (20)      496 2020-09-15 01:44:59.000000 pyfmtools-0.81/src/isfixedvar.c
+-rw-------   0 nhenseler   (501) staff       (20)     4588 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_BFP.h
+-rw-------   0 nhenseler   (501) staff       (20)     5569 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_BFP1.h
+-rw-------   0 nhenseler   (501) staff       (20)     4444 2021-02-16 05:56:16.000000 pyfmtools-0.81/src/lp_BFP2.h
+-rw-------   0 nhenseler   (501) staff       (20)     5516 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_Hash.c
+-rw-------   0 nhenseler   (501) staff       (20)     1135 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_Hash.h
+-rw-------   0 nhenseler   (501) staff       (20)    23763 2020-09-15 01:45:42.000000 pyfmtools-0.81/src/lp_LUSOL.c
+-rw-------   0 nhenseler   (501) staff       (20)     2818 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_LUSOL.h
+-rw-------   0 nhenseler   (501) staff       (20)     6986 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MDO.c
+-rw-------   0 nhenseler   (501) staff       (20)      252 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MDO.h
+-rw-------   0 nhenseler   (501) staff       (20)    53842 2021-02-16 06:53:34.000000 pyfmtools-0.81/src/lp_MPS.c
+-rw-------   0 nhenseler   (501) staff       (20)      926 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_MPS.h
+-rw-------   0 nhenseler   (501) staff       (20)    40253 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_SOS.c
+-rw-------   0 nhenseler   (501) staff       (20)     4627 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_SOS.h
+-rw-------   0 nhenseler   (501) staff       (20)    12381 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_crash.c
+-rw-------   0 nhenseler   (501) staff       (20)      484 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_crash.h
+-rw-------   0 nhenseler   (501) staff       (20)     3916 2021-02-12 00:36:00.000000 pyfmtools-0.81/src/lp_etaPFI.h
+-rw-------   0 nhenseler   (501) staff       (20)    47660 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_explicit.h
+-rw-------   0 nhenseler   (501) staff       (20)       45 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_fortify.h
+-rw-------   0 nhenseler   (501) staff       (20)   286090 2022-05-23 02:33:29.000000 pyfmtools-0.81/src/lp_lib.c
+-rw-------   0 nhenseler   (501) staff       (20)   118585 2022-05-23 02:33:57.000000 pyfmtools-0.81/src/lp_lib.h
+-rw-------   0 nhenseler   (501) staff       (20)    96546 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_matrix.c
+-rw-------   0 nhenseler   (501) staff       (20)    12184 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_matrix.h
+-rw-------   0 nhenseler   (501) staff       (20)    46309 2021-04-07 03:10:58.000000 pyfmtools-0.81/src/lp_mipbb.c
+-rw-------   0 nhenseler   (501) staff       (20)     2128 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_mipbb.h
+-rw-------   0 nhenseler   (501) staff       (20)    23491 2021-02-12 00:36:06.000000 pyfmtools-0.81/src/lp_params.c
+-rw-------   0 nhenseler   (501) staff       (20)   184143 2021-07-24 00:59:10.000000 pyfmtools-0.81/src/lp_presolve.c
+-rw-------   0 nhenseler   (501) staff       (20)     4190 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_presolve.h
+-rw-------   0 nhenseler   (501) staff       (20)    68918 2020-09-24 08:24:57.000000 pyfmtools-0.81/src/lp_price.c
+-rw-------   0 nhenseler   (501) staff       (20)     5141 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_price.h
+-rw-------   0 nhenseler   (501) staff       (20)    13780 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_pricePSE.c
+-rw-------   0 nhenseler   (501) staff       (20)      712 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_pricePSE.h
+-rw-------   0 nhenseler   (501) staff       (20)    24951 2020-04-28 01:15:06.000000 pyfmtools-0.81/src/lp_report.c
+-rw-------   0 nhenseler   (501) staff       (20)     1436 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_report.h
+-rw-------   0 nhenseler   (501) staff       (20)    51050 2021-02-12 00:36:10.000000 pyfmtools-0.81/src/lp_rlp.h
+-rw-------   0 nhenseler   (501) staff       (20)    29508 2017-12-15 12:16:42.000000 pyfmtools-0.81/src/lp_scale.c
+-rw-------   0 nhenseler   (501) staff       (20)     1008 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_scale.h
+-rw-------   0 nhenseler   (501) staff       (20)    75069 2020-04-28 01:17:20.000000 pyfmtools-0.81/src/lp_simplex.c
+-rw-------   0 nhenseler   (501) staff       (20)     1057 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_simplex.h
+-rw-------   0 nhenseler   (501) staff       (20)     9717 2020-09-08 02:31:35.000000 pyfmtools-0.81/src/lp_types.h
+-rw-------   0 nhenseler   (501) staff       (20)    26914 2020-09-24 08:01:30.000000 pyfmtools-0.81/src/lp_utils.c
+-rw-------   0 nhenseler   (501) staff       (20)     6125 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_utils.h
+-rw-------   0 nhenseler   (501) staff       (20)    11210 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/lp_wlp.c
+-rw-------   0 nhenseler   (501) staff       (20)      294 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lp_wlp.h
+-rw-------   0 nhenseler   (501) staff       (20)     1307 2018-03-02 10:29:08.000000 pyfmtools-0.81/src/lpkit.h
+-rw-------   0 nhenseler   (501) staff       (20)    21870 2020-09-24 08:24:40.000000 pyfmtools-0.81/src/lpslink56.c
+-rw-------   0 nhenseler   (501) staff       (20)      778 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lpsolve.h
+-rw-------   0 nhenseler   (501) staff       (20)    24934 2020-04-28 01:21:09.000000 pyfmtools-0.81/src/lusol.c
+-rw-------   0 nhenseler   (501) staff       (20)    14037 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol.h
+-rw-------   0 nhenseler   (501) staff       (20)   135944 2017-12-15 11:57:34.000000 pyfmtools-0.81/src/lusol1.h
+-rw-------   0 nhenseler   (501) staff       (20)     6437 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol2.h
+-rw-------   0 nhenseler   (501) staff       (20)    28424 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6a.h
+-rw-------   0 nhenseler   (501) staff       (20)     4498 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6l0.h
+-rw-------   0 nhenseler   (501) staff       (20)     4899 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol6u.h
+-rw-------   0 nhenseler   (501) staff       (20)    22181 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol7a.h
+-rw-------   0 nhenseler   (501) staff       (20)    11175 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusol8a.h
+-rw-------   0 nhenseler   (501) staff       (20)     7376 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/lusolio.c
+-rw-------   0 nhenseler   (501) staff       (20)     1014 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/lusolio.h
+-rw-------   0 nhenseler   (501) staff       (20)     7757 2020-12-16 09:23:48.000000 pyfmtools-0.81/src/minimalsplus.h
+-rw-------   0 nhenseler   (501) staff       (20)    13025 2020-04-28 01:15:38.000000 pyfmtools-0.81/src/mmio.c
+-rw-------   0 nhenseler   (501) staff       (20)     4320 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/mmio.h
+-rw-------   0 nhenseler   (501) staff       (20)    19312 2020-04-28 01:22:16.000000 pyfmtools-0.81/src/myblas.c
+-rw-------   0 nhenseler   (501) staff       (20)     5651 2021-02-12 08:29:12.000000 pyfmtools-0.81/src/myblas.h
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.685625 pyfmtools-0.81/src/pyfmtools.egg-info/
+-rw-r--r--   0 nhenseler   (501) staff       (20)     5372 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/PKG-INFO
+-rw-r--r--   0 nhenseler   (501) staff       (20)     1776 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)        1 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)       12 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/requires.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)       21 2023-04-11 01:52:07.000000 pyfmtools-0.81/src/pyfmtools.egg-info/top_level.txt
+-rw-r--r--   0 nhenseler   (501) staff       (20)    48236 2023-03-27 07:08:40.000000 pyfmtools-0.81/src/pyfmtools.py
+-rw-------   0 nhenseler   (501) staff       (20)    21684 2021-04-07 03:11:24.000000 pyfmtools-0.81/src/sparselib.c
+-rw-------   0 nhenseler   (501) staff       (20)     2975 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/sparselib.h
+-rw-------   0 nhenseler   (501) staff       (20)      396 2020-04-28 00:33:49.000000 pyfmtools-0.81/src/stdafx.h
+-rw-------   0 nhenseler   (501) staff       (20)     1822 2015-09-18 14:53:52.000000 pyfmtools-0.81/src/ufortify.h
+-rw-------   0 nhenseler   (501) staff       (20)    87216 2022-05-23 02:18:42.000000 pyfmtools-0.81/src/wrapperpy.cpp
+-rw-------   0 nhenseler   (501) staff       (20)    14390 2022-05-20 09:48:18.000000 pyfmtools-0.81/src/wrapperpy.h
+-rw-------   0 nhenseler   (501) staff       (20)    28266 2020-09-24 07:46:24.000000 pyfmtools-0.81/src/yacc_read.c
+-rw-------   0 nhenseler   (501) staff       (20)      918 2017-11-28 12:18:32.000000 pyfmtools-0.81/src/yacc_read.h
+drwxr-xr-x   0 nhenseler   (501) staff       (20)        0 2023-04-11 01:52:08.688521 pyfmtools-0.81/tests/
+-rw-------   0 nhenseler   (501) staff       (20)     3508 2022-05-24 07:38:34.000000 pyfmtools-0.81/tests/test_no_wrapper.py
+-rw-r--r--   0 nhenseler   (501) staff       (20)    27771 2022-06-28 04:36:04.000000 pyfmtools-0.81/tests/test_wrapper.py
```

### Comparing `pyfmtools-0.80/LICENSE.txt` & `pyfmtools-0.81/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/PKG-INFO` & `pyfmtools-0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 0.80
+Version: 0.81
 Summary: Library for handling and fitting fuzzy measures
 Home-page: UNKNOWN
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyfmtools-0.80/README.md` & `pyfmtools-0.81/README.md`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/setup.py` & `pyfmtools-0.81/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup( 
     name="pyfmtools",
-    version="0.80",
+    version="0.81",
     description="Library for handling and fitting fuzzy measures",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="",
     author='Gleb Beliakov, Norbert Henseler',
     author_email='gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au',
     license_file='LICENSE.txt',
```

### Comparing `pyfmtools-0.80/src/binarylattice.h` & `pyfmtools-0.81/src/binarylattice.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/buildPyfmtools.py` & `pyfmtools-0.81/src/buildPyfmtools.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/colamd.c` & `pyfmtools-0.81/src/colamd.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/colamd.h` & `pyfmtools-0.81/src/colamd.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/commonlib.c` & `pyfmtools-0.81/src/commonlib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/commonlib.h` & `pyfmtools-0.81/src/commonlib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fmrandom.cpp` & `pyfmtools-0.81/src/fmrandom.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fmrandom.h` & `pyfmtools-0.81/src/fmrandom.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fortify.h` & `pyfmtools-0.81/src/fortify.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fuzzymeasurefit.cpp` & `pyfmtools-0.81/src/fuzzymeasurefit.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fuzzymeasurefit.h` & `pyfmtools-0.81/src/fuzzymeasurefit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fuzzymeasurefit3.cpp` & `pyfmtools-0.81/src/fuzzymeasurefit3.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fuzzymeasuretools.cpp` & `pyfmtools-0.81/src/fuzzymeasuretools.bak.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/fuzzymeasuretools.h` & `pyfmtools-0.81/src/fuzzymeasuretools.bak.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/generaldefs.h` & `pyfmtools-0.81/src/generaldefs.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/hbio.h` & `pyfmtools-0.81/src/hbio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/ini.c` & `pyfmtools-0.81/src/ini.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_BFP.h` & `pyfmtools-0.81/src/lp_BFP.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_BFP1.h` & `pyfmtools-0.81/src/lp_BFP1.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_BFP2.h` & `pyfmtools-0.81/src/lp_BFP2.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_Hash.c` & `pyfmtools-0.81/src/lp_Hash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_Hash.h` & `pyfmtools-0.81/src/lp_Hash.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_LUSOL.c` & `pyfmtools-0.81/src/lp_LUSOL.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_LUSOL.h` & `pyfmtools-0.81/src/lp_LUSOL.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_MDO.c` & `pyfmtools-0.81/src/lp_MDO.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_MPS.c` & `pyfmtools-0.81/src/lp_MPS.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_MPS.h` & `pyfmtools-0.81/src/lp_MPS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_SOS.c` & `pyfmtools-0.81/src/lp_SOS.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_SOS.h` & `pyfmtools-0.81/src/lp_SOS.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_crash.c` & `pyfmtools-0.81/src/lp_crash.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_etaPFI.h` & `pyfmtools-0.81/src/lp_etaPFI.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_explicit.h` & `pyfmtools-0.81/src/lp_explicit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_lib.c` & `pyfmtools-0.81/src/lp_lib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_lib.h` & `pyfmtools-0.81/src/lp_lib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_matrix.c` & `pyfmtools-0.81/src/lp_matrix.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_matrix.h` & `pyfmtools-0.81/src/lp_matrix.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_mipbb.c` & `pyfmtools-0.81/src/lp_mipbb.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_mipbb.h` & `pyfmtools-0.81/src/lp_mipbb.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_params.c` & `pyfmtools-0.81/src/lp_params.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_presolve.c` & `pyfmtools-0.81/src/lp_presolve.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_presolve.h` & `pyfmtools-0.81/src/lp_presolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_price.c` & `pyfmtools-0.81/src/lp_price.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_price.h` & `pyfmtools-0.81/src/lp_price.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_pricePSE.c` & `pyfmtools-0.81/src/lp_pricePSE.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_pricePSE.h` & `pyfmtools-0.81/src/lp_pricePSE.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_report.c` & `pyfmtools-0.81/src/lp_report.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_report.h` & `pyfmtools-0.81/src/lp_report.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_rlp.h` & `pyfmtools-0.81/src/lp_rlp.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_scale.c` & `pyfmtools-0.81/src/lp_scale.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_scale.h` & `pyfmtools-0.81/src/lp_scale.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_simplex.c` & `pyfmtools-0.81/src/lp_simplex.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_simplex.h` & `pyfmtools-0.81/src/lp_simplex.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_types.h` & `pyfmtools-0.81/src/lp_types.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_utils.c` & `pyfmtools-0.81/src/lp_utils.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_utils.h` & `pyfmtools-0.81/src/lp_utils.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lp_wlp.c` & `pyfmtools-0.81/src/lp_wlp.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lpkit.h` & `pyfmtools-0.81/src/lpkit.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lpslink56.c` & `pyfmtools-0.81/src/lpslink56.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lpsolve.h` & `pyfmtools-0.81/src/lpsolve.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol.c` & `pyfmtools-0.81/src/lusol.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol.h` & `pyfmtools-0.81/src/lusol.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol1.h` & `pyfmtools-0.81/src/lusol1.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol2.h` & `pyfmtools-0.81/src/lusol2.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol6a.h` & `pyfmtools-0.81/src/lusol6a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol6l0.h` & `pyfmtools-0.81/src/lusol6l0.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol6u.h` & `pyfmtools-0.81/src/lusol6u.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol7a.h` & `pyfmtools-0.81/src/lusol7a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusol8a.h` & `pyfmtools-0.81/src/lusol8a.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusolio.c` & `pyfmtools-0.81/src/lusolio.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/lusolio.h` & `pyfmtools-0.81/src/lusolio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/minimalsplus.h` & `pyfmtools-0.81/src/minimalsplus.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/mmio.c` & `pyfmtools-0.81/src/mmio.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/mmio.h` & `pyfmtools-0.81/src/mmio.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/myblas.c` & `pyfmtools-0.81/src/myblas.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/myblas.h` & `pyfmtools-0.81/src/myblas.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/pyfmtools.egg-info/PKG-INFO` & `pyfmtools-0.81/src/pyfmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmtools
-Version: 0.80
+Version: 0.81
 Summary: Library for handling and fitting fuzzy measures
 Home-page: UNKNOWN
 Author: Gleb Beliakov, Norbert Henseler
 Author-email: gleb.beliakov@deakin.edu.au, norbert.henseler@deakin.edu.au
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyfmtools-0.80/src/pyfmtools.egg-info/SOURCES.txt` & `pyfmtools-0.81/src/pyfmtools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
-dist/pyfmtools-0.80-cp39-cp39-macosx_10_9_x86_64.whl
+dist/pyfmtools-0.81-cp39-cp39-macosx_10_9_x86_64.whl
 src/binarylattice.h
 src/buildPyfmtools.py
 src/colamd.c
 src/colamd.h
 src/commonlib.c
 src/commonlib.h
 src/declare.h
 src/fmrandom.cpp
 src/fmrandom.h
 src/fortify.h
 src/fuzzymeasurefit.cpp
 src/fuzzymeasurefit.h
 src/fuzzymeasurefit3.cpp
+src/fuzzymeasuretools.bak.cpp
+src/fuzzymeasuretools.bak.h
 src/fuzzymeasuretools.cpp
 src/fuzzymeasuretools.h
 src/generaldefs.h
 src/hbio.h
 src/ini.c
 src/ini.h
 src/isfixedvar.c
```

### Comparing `pyfmtools-0.80/src/pyfmtools.py` & `pyfmtools-0.81/src/pyfmtools.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/sparselib.c` & `pyfmtools-0.81/src/sparselib.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/sparselib.h` & `pyfmtools-0.81/src/sparselib.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/ufortify.h` & `pyfmtools-0.81/src/ufortify.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/wrapperpy.cpp` & `pyfmtools-0.81/src/wrapperpy.cpp`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/wrapperpy.h` & `pyfmtools-0.81/src/wrapperpy.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/yacc_read.c` & `pyfmtools-0.81/src/yacc_read.c`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/src/yacc_read.h` & `pyfmtools-0.81/src/yacc_read.h`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/tests/test_no_wrapper.py` & `pyfmtools-0.81/tests/test_no_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyfmtools-0.80/tests/test_wrapper.py` & `pyfmtools-0.81/tests/test_wrapper.py`

 * *Files identical despite different names*

