# Comparing `tmp/usgs-strec-2.2.4.tar.gz` & `tmp/usgs-strec-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-strec-2.2.4.tar", last modified: Mon Feb 27 22:03:40 2023, max compression
+gzip compressed data, was "usgs-strec-2.2.5.tar", last modified: Tue Apr 11 14:37:20 2023, max compression
```

## Comparing `usgs-strec-2.2.4.tar` & `usgs-strec-2.2.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.203455 usgs-strec-2.2.4/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/.gitlab-ci.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/.travis.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/CONTRIBUTING.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-02-27 22:03:40.203455 usgs-strec-2.2.4/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8570 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/README.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/code.json
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2609 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/install.sh
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/license.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/select_regions.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-02-27 22:03:40.203455 usgs-strec-2.2.4/setup.cfg
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.183456 usgs-strec-2.2.4/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.183456 usgs-strec-2.2.4/src/strec/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/__init__.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.183456 usgs-strec-2.2.4/src/strec/bin/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7030 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/bin/regcalc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8008 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/src/strec/bin/strec_cfg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9227 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/calc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/cmt.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.193455 usgs-strec-2.2.4/src/strec/data/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/REGION_GRIDS_README.txt
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/active.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/domains.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/land.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/maximum_interface_depths.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/moment_tensors.db
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/ocean.geojson
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/stable.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/strec.ini
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/subduction.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/data/volcanic.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5373 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/database.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/distance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/gcmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/gmreg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/kagan.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5818 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/ngasub.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/slab.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13046 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/sm_probs.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/subduction.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    20965 2023-02-27 20:47:29.000000 usgs-strec-2.2.4/src/strec/subtype.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7962 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/src/strec/utils.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.193455 usgs-strec-2.2.4/src/usgs_strec.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2194 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-02-27 22:03:40.000000 usgs-strec-2.2.4/src/usgs_strec.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.183456 usgs-strec-2.2.4/test/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.183456 usgs-strec-2.2.4/test/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.193455 usgs-strec-2.2.4/test/src/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/data/AMlvPS_trench.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/data/large_events.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/data/strec.db
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/data/test.ndk
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/data/test_regimes.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.193455 usgs-strec-2.2.4/test/src/strec/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     9985 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/calc_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/cmt_test.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 22:03:40.203455 usgs-strec-2.2.4/test/src/strec/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/big_focals.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/comcatid_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/focal_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/hypocols_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/id_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/moment_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/nga_matched.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10011 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/simple_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/data/subsampled_nga_results.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/data/van_slab2_dep_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/data/van_slab2_dip_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/data/van_slab2_str_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/data/van_slab2_thk_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/data/van_slab2_unc_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/database_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/distance_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/gcmt_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/gmreg_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/kagan_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2116 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/ngasub_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      746 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/probs_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.4/test/src/strec/slab_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/subduction_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7886 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/subtype_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3530 2023-02-27 20:02:06.000000 usgs-strec-2.2.4/test/src/strec/utils_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/.gitignore
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/.gitlab-ci.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/.travis.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/CONTRIBUTING.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/DISCLAIMER.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/LICENSE.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8570 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/README.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/code.json
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 14:19:05.000000 usgs-strec-2.2.5/install.sh
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/license.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-11 14:16:44.000000 usgs-strec-2.2.5/pyproject.toml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/select_regions.png
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/setup.cfg
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.437297 usgs-strec-2.2.5/src/strec/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/__init__.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.437297 usgs-strec-2.2.5/src/strec/bin/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7030 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/bin/regcalc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8008 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/src/strec/bin/strec_cfg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9227 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/calc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/cmt.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.457298 usgs-strec-2.2.5/src/strec/data/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/REGION_GRIDS_README.txt
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/active.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/domains.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/land.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/maximum_interface_depths.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/moment_tensors.db
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/ocean.geojson
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/stable.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/strec.ini
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/subduction.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/volcanic.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5373 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/database.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/distance.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/gcmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/gmreg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/kagan.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5818 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/ngasub.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/slab.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13046 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/sm_probs.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/subduction.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    20965 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/subtype.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7962 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/utils.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.457298 usgs-strec-2.2.5/src/usgs_strec.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2194 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/SOURCES.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/test/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/test/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.467298 usgs-strec-2.2.5/test/src/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/AMlvPS_trench.json
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/large_events.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/strec.db
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/test.ndk
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/test_regimes.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.467298 usgs-strec-2.2.5/test/src/strec/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     9985 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/calc_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/cmt_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/test/src/strec/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/big_focals.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/comcatid_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/focal_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/hypocols_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/id_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/moment_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/nga_matched.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10011 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/data/simple_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/subsampled_nga_results.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_dep_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_dip_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_str_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_thk_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_unc_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/database_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/distance_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/gcmt_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/gmreg_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/kagan_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2116 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/ngasub_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      746 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/probs_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/slab_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/subduction_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7886 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/subtype_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3530 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/utils_test.py
```

### Comparing `usgs-strec-2.2.4/.gitlab-ci.yml` & `usgs-strec-2.2.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/.travis.yml` & `usgs-strec-2.2.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/CONTRIBUTING.md` & `usgs-strec-2.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/DISCLAIMER.md` & `usgs-strec-2.2.5/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/LICENSE.md` & `usgs-strec-2.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/PKG-INFO` & `usgs-strec-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.4
+Version: 2.2.5
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -16,15 +16,15 @@
         revision. It is being provided to meet the need for timely best
         science. The information has not received final approval by the USGS
         and is provided on the condition that neither the USGS nor the
         U.S. Government shall be held liable for any damages resulting from
         the authorized or unauthorized use of the information.
         
 Keywords: comcat,earthquake
-Requires-Python: <=3.10
+Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.md
 
 # Table of Contents
 - [Table of Contents](#table-of-contents)
```

### Comparing `usgs-strec-2.2.4/README.md` & `usgs-strec-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/code.json` & `usgs-strec-2.2.5/code.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/install.sh` & `usgs-strec-2.2.5/install.sh`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 source $prof
 
 echo "Path:"
 echo $PATH
 
 VENV=strecenv
-PYVER=3.9
+PYVER=3.10
 
 # Is conda installed?
 conda --version
 if [ $? -ne 0 ]; then
     echo "No conda detected, installing miniconda from ${mini_conda_url}..."
 
     curl -L $mini_conda_url -o miniconda.sh;
```

### Comparing `usgs-strec-2.2.4/pyproject.toml` & `usgs-strec-2.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "usgs-strec"
-version = "2.2.4"
+version = "2.2.5"
 description = "USGS SeismoTectonic Regime Earthquake Calculator (STREC)"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
 ]
 
 license = {file = "LICENSE.md"}
 readme = "README.md"
-requires-python = "<=3.10"
+requires-python = "<=3.11"
 
 keywords = ["comcat", "earthquake"]
 
 
 dependencies = [
     "configobj>=5.0.6",
     "esi-utils-rupture",
```

### Comparing `usgs-strec-2.2.4/select_regions.png` & `usgs-strec-2.2.5/select_regions.png`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/bin/regcalc.py` & `usgs-strec-2.2.5/src/strec/bin/regcalc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/bin/strec_cfg.py` & `usgs-strec-2.2.5/src/strec/bin/strec_cfg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/calc.py` & `usgs-strec-2.2.5/src/strec/calc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/cmt.py` & `usgs-strec-2.2.5/src/strec/cmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/REGION_GRIDS_README.txt` & `usgs-strec-2.2.5/src/strec/data/REGION_GRIDS_README.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/active.geojson` & `usgs-strec-2.2.5/src/strec/data/active.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/domains.xlsx` & `usgs-strec-2.2.5/src/strec/data/domains.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/land.geojson` & `usgs-strec-2.2.5/src/strec/data/land.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/moment_tensors.db` & `usgs-strec-2.2.5/src/strec/data/moment_tensors.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/ocean.geojson` & `usgs-strec-2.2.5/src/strec/data/ocean.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/stable.geojson` & `usgs-strec-2.2.5/src/strec/data/stable.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/strec.ini` & `usgs-strec-2.2.5/src/strec/data/strec.ini`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/subduction.geojson` & `usgs-strec-2.2.5/src/strec/data/subduction.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/data/volcanic.geojson` & `usgs-strec-2.2.5/src/strec/data/volcanic.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/database.py` & `usgs-strec-2.2.5/src/strec/database.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/distance.py` & `usgs-strec-2.2.5/src/strec/distance.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/gcmt.py` & `usgs-strec-2.2.5/src/strec/gcmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/gmreg.py` & `usgs-strec-2.2.5/src/strec/gmreg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/kagan.py` & `usgs-strec-2.2.5/src/strec/kagan.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/ngasub.py` & `usgs-strec-2.2.5/src/strec/ngasub.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/slab.py` & `usgs-strec-2.2.5/src/strec/slab.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/sm_probs.py` & `usgs-strec-2.2.5/src/strec/sm_probs.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/subduction.py` & `usgs-strec-2.2.5/src/strec/subduction.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/subtype.py` & `usgs-strec-2.2.5/src/strec/subtype.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/strec/utils.py` & `usgs-strec-2.2.5/src/strec/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/src/usgs_strec.egg-info/PKG-INFO` & `usgs-strec-2.2.5/src/usgs_strec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.4
+Version: 2.2.5
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -16,15 +16,15 @@
         revision. It is being provided to meet the need for timely best
         science. The information has not received final approval by the USGS
         and is provided on the condition that neither the USGS nor the
         U.S. Government shall be held liable for any damages resulting from
         the authorized or unauthorized use of the information.
         
 Keywords: comcat,earthquake
-Requires-Python: <=3.10
+Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.md
 
 # Table of Contents
 - [Table of Contents](#table-of-contents)
```

### Comparing `usgs-strec-2.2.4/src/usgs_strec.egg-info/SOURCES.txt` & `usgs-strec-2.2.5/src/usgs_strec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/data/AMlvPS_trench.json` & `usgs-strec-2.2.5/test/src/data/AMlvPS_trench.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/data/large_events.xlsx` & `usgs-strec-2.2.5/test/src/data/large_events.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/data/strec.db` & `usgs-strec-2.2.5/test/src/data/strec.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/data/test_regimes.xlsx` & `usgs-strec-2.2.5/test/src/data/test_regimes.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/calc_test.py` & `usgs-strec-2.2.5/test/src/strec/calc_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/cmt_test.py` & `usgs-strec-2.2.5/test/src/strec/cmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/big_focals.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/big_focals.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/comcatid_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/comcatid_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/focal_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/focal_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/hypocols_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/hypocols_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/id_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/id_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/moment_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/moment_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/nga_matched.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/nga_matched.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/simple_catalog.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/simple_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/subsampled_nga_results.xlsx` & `usgs-strec-2.2.5/test/src/strec/data/subsampled_nga_results.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/van_slab2_dep_02.23.18.grd` & `usgs-strec-2.2.5/test/src/strec/data/van_slab2_dep_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/van_slab2_dip_02.23.18.grd` & `usgs-strec-2.2.5/test/src/strec/data/van_slab2_dip_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/van_slab2_str_02.23.18.grd` & `usgs-strec-2.2.5/test/src/strec/data/van_slab2_str_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/van_slab2_thk_02.23.18.grd` & `usgs-strec-2.2.5/test/src/strec/data/van_slab2_thk_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/data/van_slab2_unc_02.23.18.grd` & `usgs-strec-2.2.5/test/src/strec/data/van_slab2_unc_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/database_test.py` & `usgs-strec-2.2.5/test/src/strec/database_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/distance_test.py` & `usgs-strec-2.2.5/test/src/strec/distance_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/gcmt_test.py` & `usgs-strec-2.2.5/test/src/strec/gcmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/gmreg_test.py` & `usgs-strec-2.2.5/test/src/strec/gmreg_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/kagan_test.py` & `usgs-strec-2.2.5/test/src/strec/kagan_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/ngasub_test.py` & `usgs-strec-2.2.5/test/src/strec/ngasub_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/probs_test.py` & `usgs-strec-2.2.5/test/src/strec/probs_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/slab_test.py` & `usgs-strec-2.2.5/test/src/strec/slab_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/subduction_test.py` & `usgs-strec-2.2.5/test/src/strec/subduction_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/subtype_test.py` & `usgs-strec-2.2.5/test/src/strec/subtype_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.4/test/src/strec/utils_test.py` & `usgs-strec-2.2.5/test/src/strec/utils_test.py`

 * *Files identical despite different names*

