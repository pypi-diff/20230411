# Comparing `tmp/usgs-strec-2.2.5.tar.gz` & `tmp/usgs-strec-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-strec-2.2.5.tar", last modified: Tue Apr 11 14:37:20 2023, max compression
+gzip compressed data, was "usgs-strec-2.2.6.tar", last modified: Tue Apr 11 15:46:07 2023, max compression
```

## Comparing `usgs-strec-2.2.5.tar` & `usgs-strec-2.2.6.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/.gitlab-ci.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/.travis.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/CONTRIBUTING.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8570 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/README.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/code.json
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 14:19:05.000000 usgs-strec-2.2.5/install.sh
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/license.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-11 14:16:44.000000 usgs-strec-2.2.5/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/select_regions.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/setup.cfg
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.437297 usgs-strec-2.2.5/src/strec/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/__init__.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.437297 usgs-strec-2.2.5/src/strec/bin/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7030 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/bin/regcalc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8008 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/src/strec/bin/strec_cfg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9227 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/calc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/cmt.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.457298 usgs-strec-2.2.5/src/strec/data/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/REGION_GRIDS_README.txt
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/active.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/domains.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/land.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/maximum_interface_depths.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/moment_tensors.db
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/ocean.geojson
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/stable.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/strec.ini
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/subduction.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/data/volcanic.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5373 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/database.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/distance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/gcmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/gmreg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/kagan.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5818 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/ngasub.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/slab.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13046 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/sm_probs.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/src/strec/subduction.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    20965 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/subtype.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7962 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/src/strec/utils.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.457298 usgs-strec-2.2.5/src/usgs_strec.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9815 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2194 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-11 14:37:20.000000 usgs-strec-2.2.5/src/usgs_strec.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/test/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.427297 usgs-strec-2.2.5/test/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.467298 usgs-strec-2.2.5/test/src/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/AMlvPS_trench.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/large_events.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/strec.db
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/test.ndk
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/data/test_regimes.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.467298 usgs-strec-2.2.5/test/src/strec/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     9985 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/calc_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/cmt_test.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 14:37:20.477298 usgs-strec-2.2.5/test/src/strec/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/big_focals.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/comcatid_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/focal_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/hypocols_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/id_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/moment_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/nga_matched.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10011 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/data/simple_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/data/subsampled_nga_results.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_dep_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_dip_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_str_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_thk_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/data/van_slab2_unc_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/database_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/distance_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/gcmt_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/gmreg_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/kagan_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2116 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/ngasub_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      746 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/probs_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.5/test/src/strec/slab_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.5/test/src/strec/subduction_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     7886 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/subtype_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3530 2023-04-11 14:16:15.000000 usgs-strec-2.2.5/test/src/strec/utils_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/.gitignore
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/.gitlab-ci.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/.travis.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/CONTRIBUTING.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/DISCLAIMER.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/LICENSE.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10781 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/README.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/code.json
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/install.sh
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/license.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-11 15:45:56.000000 usgs-strec-2.2.6/pyproject.toml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/select_regions.png
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/setup.cfg
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/strec/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/__init__.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/strec/bin/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8371 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/bin/regcalc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8008 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/src/strec/bin/strec_cfg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9523 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/calc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/cmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4869 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/config.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/src/strec/data/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/REGION_GRIDS_README.txt
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/active.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/domains.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/land.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/maximum_interface_depths.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/moment_tensors.db
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/ocean.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6153 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/data/select.conf
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1753 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/data/selectspec.conf
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/stable.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/strec.ini
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/subduction.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/volcanic.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5373 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/database.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/distance.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/gcmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/gmreg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/kagan.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/slab.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13185 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/sm_probs.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/subduction.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23230 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/subtype.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8163 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/utils.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/src/usgs_strec.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2222 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/SOURCES.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/test/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/test/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/AMlvPS_trench.json
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/large_events.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/strec.db
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/test.ndk
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/test_regimes.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/strec/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10144 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/calc_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/cmt_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/strec/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/big_focals.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/comcatid_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/focal_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/hypocols_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/id_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/moment_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/nga_matched.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10154 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/data/simple_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/subsampled_nga_results.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_dep_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_dip_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_str_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_thk_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_unc_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/database_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/distance_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/gcmt_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/gmreg_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/kagan_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8109 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/probs_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/slab_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/subduction_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8116 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/subtype_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/utils_test.py
```

### Comparing `usgs-strec-2.2.5/.gitlab-ci.yml` & `usgs-strec-2.2.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/.travis.yml` & `usgs-strec-2.2.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/CONTRIBUTING.md` & `usgs-strec-2.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/DISCLAIMER.md` & `usgs-strec-2.2.6/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/LICENSE.md` & `usgs-strec-2.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/PKG-INFO` & `usgs-strec-2.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,614 +1,674 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7573 6773  : 2.1.Name: usgs
-00000020: 2d73 7472 6563 0a56 6572 7369 6f6e 3a20  -strec.Version: 
-00000030: 322e 322e 350a 5375 6d6d 6172 793a 2055  2.2.5.Summary: U
-00000040: 5347 5320 5365 6973 6d6f 5465 6374 6f6e  SGS SeismoTecton
-00000050: 6963 2052 6567 696d 6520 4561 7274 6871  ic Regime Earthq
-00000060: 7561 6b65 2043 616c 6375 6c61 746f 7220  uake Calculator 
-00000070: 2853 5452 4543 290a 4175 7468 6f72 2d65  (STREC).Author-e
-00000080: 6d61 696c 3a20 4d69 6b65 2048 6561 726e  mail: Mike Hearn
-00000090: 6520 3c6d 6865 6172 6e65 4075 7367 732e  e <mhearne@usgs.
-000000a0: 676f 763e 2c20 4572 6963 2054 686f 6d70  gov>, Eric Thomp
-000000b0: 736f 6e20 3c65 7468 6f6d 7073 6f6e 4075  son <ethompson@u
-000000c0: 7367 732e 676f 763e 0a4c 6963 656e 7365  sgs.gov>.License
-000000d0: 3a20 4c69 6365 6e73 650a 2020 2020 2020  : License.      
-000000e0: 2020 3d3d 3d3d 3d3d 3d0a 2020 2020 2020    =======.      
-000000f0: 2020 0a20 2020 2020 2020 2055 6e6c 6573    .        Unles
-00000100: 7320 6f74 6865 7277 6973 6520 6e6f 7465  s otherwise note
-00000110: 642c 2054 6869 7320 7072 6f6a 6563 7420  d, This project 
-00000120: 6973 2069 6e20 7468 6520 7075 626c 6963  is in the public
-00000130: 2064 6f6d 6169 6e20 696e 2074 6865 2055   domain in the U
-00000140: 6e69 7465 640a 2020 2020 2020 2020 5374  nited.        St
-00000150: 6174 6573 2062 6563 6175 7365 2069 7420  ates because it 
-00000160: 636f 6e74 6169 6e73 206d 6174 6572 6961  contains materia
-00000170: 6c73 2074 6861 7420 6f72 6967 696e 616c  ls that original
-00000180: 6c79 2063 616d 6520 6672 6f6d 2074 6865  ly came from the
-00000190: 2055 6e69 7465 640a 2020 2020 2020 2020   United.        
-000001a0: 5374 6174 6573 2047 656f 6c6f 6769 6361  States Geologica
-000001b0: 6c20 5375 7276 6579 2c20 616e 2061 6765  l Survey, an age
-000001c0: 6e63 7920 6f66 2074 6865 2055 6e69 7465  ncy of the Unite
-000001d0: 6420 5374 6174 6573 2044 6570 6172 746d  d States Departm
-000001e0: 656e 7420 6f66 0a20 2020 2020 2020 2049  ent of.        I
-000001f0: 6e74 6572 696f 722e 2046 6f72 206d 6f72  nterior. For mor
-00000200: 6520 696e 666f 726d 6174 696f 6e2c 2073  e information, s
-00000210: 6565 2074 6865 206f 6666 6963 6961 6c20  ee the official 
-00000220: 5553 4753 2063 6f70 7972 6967 6874 2070  USGS copyright p
-00000230: 6f6c 6963 7920 6174 0a20 2020 2020 2020  olicy at.       
-00000240: 2068 7474 7073 3a2f 2f77 7777 322e 7573   https://www2.us
-00000250: 6773 2e67 6f76 2f76 6973 7561 6c2d 6964  gs.gov/visual-id
-00000260: 2f63 7265 6469 745f 7573 6773 2e68 746d  /credit_usgs.htm
-00000270: 6c23 636f 7079 7269 6768 740a 2020 2020  l#copyright.    
-00000280: 2020 2020 0a20 2020 2020 2020 2054 6869      .        Thi
-00000290: 7320 696e 666f 726d 6174 696f 6e20 6973  s information is
-000002a0: 2070 7265 6c69 6d69 6e61 7279 206f 7220   preliminary or 
-000002b0: 7072 6f76 6973 696f 6e61 6c20 616e 6420  provisional and 
-000002c0: 6973 2073 7562 6a65 6374 2074 6f0a 2020  is subject to.  
-000002d0: 2020 2020 2020 7265 7669 7369 6f6e 2e20        revision. 
-000002e0: 4974 2069 7320 6265 696e 6720 7072 6f76  It is being prov
-000002f0: 6964 6564 2074 6f20 6d65 6574 2074 6865  ided to meet the
-00000300: 206e 6565 6420 666f 7220 7469 6d65 6c79   need for timely
-00000310: 2062 6573 740a 2020 2020 2020 2020 7363   best.        sc
-00000320: 6965 6e63 652e 2054 6865 2069 6e66 6f72  ience. The infor
-00000330: 6d61 7469 6f6e 2068 6173 206e 6f74 2072  mation has not r
-00000340: 6563 6569 7665 6420 6669 6e61 6c20 6170  eceived final ap
-00000350: 7072 6f76 616c 2062 7920 7468 6520 5553  proval by the US
-00000360: 4753 0a20 2020 2020 2020 2061 6e64 2069  GS.        and i
-00000370: 7320 7072 6f76 6964 6564 206f 6e20 7468  s provided on th
-00000380: 6520 636f 6e64 6974 696f 6e20 7468 6174  e condition that
-00000390: 206e 6569 7468 6572 2074 6865 2055 5347   neither the USG
-000003a0: 5320 6e6f 7220 7468 650a 2020 2020 2020  S nor the.      
-000003b0: 2020 552e 532e 2047 6f76 6572 6e6d 656e    U.S. Governmen
-000003c0: 7420 7368 616c 6c20 6265 2068 656c 6420  t shall be held 
-000003d0: 6c69 6162 6c65 2066 6f72 2061 6e79 2064  liable for any d
-000003e0: 616d 6167 6573 2072 6573 756c 7469 6e67  amages resulting
-000003f0: 2066 726f 6d0a 2020 2020 2020 2020 7468   from.        th
-00000400: 6520 6175 7468 6f72 697a 6564 206f 7220  e authorized or 
-00000410: 756e 6175 7468 6f72 697a 6564 2075 7365  unauthorized use
-00000420: 206f 6620 7468 6520 696e 666f 726d 6174   of the informat
-00000430: 696f 6e2e 0a20 2020 2020 2020 200a 4b65  ion..        .Ke
-00000440: 7977 6f72 6473 3a20 636f 6d63 6174 2c65  ywords: comcat,e
-00000450: 6172 7468 7175 616b 650a 5265 7175 6972  arthquake.Requir
-00000460: 6573 2d50 7974 686f 6e3a 203c 3d33 2e31  es-Python: <=3.1
-00000470: 310a 4465 7363 7269 7074 696f 6e2d 436f  1.Description-Co
-00000480: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000490: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
-000004a0: 6573 2d45 7874 7261 3a20 6465 760a 5072  es-Extra: dev.Pr
-000004b0: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
-000004c0: 7374 0a4c 6963 656e 7365 2d46 696c 653a  st.License-File:
-000004d0: 204c 4943 454e 5345 2e6d 640a 0a23 2054   LICENSE.md..# T
-000004e0: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
-000004f0: 0a2d 205b 5461 626c 6520 6f66 2043 6f6e  .- [Table of Con
-00000500: 7465 6e74 735d 2823 7461 626c 652d 6f66  tents](#table-of
-00000510: 2d63 6f6e 7465 6e74 7329 0a2d 205b 496e  -contents).- [In
-00000520: 7472 6f64 7563 7469 6f6e 5d28 2369 6e74  troduction](#int
-00000530: 726f 6475 6374 696f 6e29 0a2d 205b 496e  roduction).- [In
-00000540: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
-00000550: 7461 6c6c 6174 696f 6e29 0a2d 205b 5570  tallation).- [Up
-00000560: 6772 6164 655d 2823 7570 6772 6164 6529  grade](#upgrade)
-00000570: 0a2d 205b 436f 6e66 6967 7572 6174 696f  .- [Configuratio
-00000580: 6e5d 2823 636f 6e66 6967 7572 6174 696f  n](#configuratio
-00000590: 6e29 0a2d 205b 5573 6167 655d 2823 7573  n).- [Usage](#us
-000005a0: 6167 6529 0a2d 205b 476c 6f73 7361 7279  age).- [Glossary
-000005b0: 5d28 2367 6c6f 7373 6172 7929 0a0a 2320  ](#glossary)..# 
-000005c0: 496e 7472 6f64 7563 7469 6f6e 0a0a 5468  Introduction..Th
-000005d0: 6973 206c 6962 7261 7279 2061 6e64 2073  is library and s
-000005e0: 6574 206f 6620 746f 6f6c 7320 7761 7320  et of tools was 
-000005f0: 6372 6561 7465 6420 746f 2070 726f 7669  created to provi
-00000600: 6465 2066 756e 6374 696f 6e61 6c69 7479  de functionality
-00000610: 2074 6f0a 6175 746f 6d61 7469 6361 6c6c   to.automaticall
-00000620: 7920 6465 7465 726d 696e 6520 7468 6520  y determine the 
-00000630: 7465 6374 6f6e 6963 2072 6567 696f 6e20  tectonic region 
-00000640: 6f66 2061 6e20 6561 7274 6871 7561 6b65  of an earthquake
-00000650: 0a28 5375 6264 7563 7469 6f6e 2c20 4163  .(Subduction, Ac
-00000660: 7469 7665 2c20 486f 7453 706f 742c 2053  tive, HotSpot, S
-00000670: 7461 626c 6529 2c20 616e 6420 7468 6520  table), and the 
-00000680: 6469 7374 616e 6365 2074 6f20 7468 6520  distance to the 
-00000690: 7465 6374 6f6e 6963 0a72 6567 696f 6e73  tectonic.regions
-000006a0: 2074 6f20 7768 6963 6820 6974 2064 6f65   to which it doe
-000006b0: 7320 2a6e 6f74 2a20 6265 6c6f 6e67 2e0a  s *not* belong..
-000006c0: 0a49 6e20 6164 6469 7469 6f6e 2c20 5365  .In addition, Se
-000006d0: 6973 6d6f 5465 6374 6f6e 6963 2052 6567  ismoTectonic Reg
-000006e0: 696d 6520 4561 7274 6871 7561 6b65 2043  ime Earthquake C
-000006f0: 616c 6375 6c61 746f 7220 2853 5452 4543  alculator (STREC
-00000700: 2920 7072 6f76 6964 6573 2061 2074 6f6f  ) provides a too
-00000710: 6c20 7468 6174 2c20 0a69 6e20 7375 6264  l that, .in subd
-00000720: 7563 7469 6f6e 207a 6f6e 6573 2c20 7265  uction zones, re
-00000730: 7475 726e 7320 696e 666f 726d 6174 696f  turns informatio
-00000740: 6e20 6162 6f75 7420 7468 6520 7375 6264  n about the subd
-00000750: 7563 7469 6f6e 207a 6f6e 652c 2075 7369  uction zone, usi
-00000760: 6e67 2074 6865 200a 5553 4753 2053 6c61  ng the .USGS Sla
-00000770: 6232 206d 6f64 656c 732e 0a0a 2868 7474  b2 models...(htt
-00000780: 7073 3a2f 2f77 7777 2e73 6369 656e 6365  ps://www.science
-00000790: 6261 7365 2e67 6f76 2f63 6174 616c 6f67  base.gov/catalog
-000007a0: 2f69 7465 6d2f 3561 6131 6230 3065 6534  /item/5aa1b00ee4
-000007b0: 6230 6231 6333 3932 6538 3634 3637 2f29  b0b1c392e86467/)
-000007c0: 2e0a 0a0a 5468 6973 2063 6f64 6520 7761  ....This code wa
-000007d0: 7320 6261 7365 6420 6f6e 2074 6865 205b  s based on the [
-000007e0: 7061 7065 725d 2868 7474 7073 3a2f 2f64  paper](https://d
-000007f0: 6f69 2e6f 7267 2f31 302e 3137 3835 2f30  oi.org/10.1785/0
-00000800: 3132 3031 3130 3132 3429 3a0a 0a60 6060  120110124):..```
-00000810: 0a41 2047 6c6f 6261 6c20 4561 7274 6871  .A Global Earthq
-00000820: 7561 6b65 2044 6973 6372 696d 696e 6174  uake Discriminat
-00000830: 696f 6e20 5363 6865 6d65 2074 6f20 4f70  ion Scheme to Op
-00000840: 7469 6d69 7a65 2047 726f 756e 64e2 8090  timize Ground...
-00000850: 4d6f 7469 6f6e 2050 7265 6469 6374 696f  Motion Predictio
-00000860: 6e20 4571 7561 7469 6f6e 2053 656c 6563  n Equation Selec
-00000870: 7469 6f6e 0a44 2e20 4761 7263 c3ad 613b  tion.D. Garc..a;
-00000880: 2044 2e20 4a2e 2057 616c 643b 204d 2e20   D. J. Wald; M. 
-00000890: 472e 2048 6561 726e 650a 4275 6c6c 6574  G. Hearne.Bullet
-000008a0: 696e 206f 6620 7468 6520 5365 6973 6d6f  in of the Seismo
-000008b0: 6c6f 6769 6361 6c20 536f 6369 6574 7920  logical Society 
-000008c0: 6f66 2041 6d65 7269 6361 2028 3230 3132  of America (2012
-000008d0: 2920 3130 3220 2831 293a 2031 3835 e280  ) 102 (1): 185..
-000008e0: 9332 3033 2e0a 6060 600a 0a0a 2320 496e  .203..```...# In
-000008f0: 7374 616c 6c61 7469 6f6e 0a0a 6070 6970  stallation..`pip
-00000900: 2069 6e73 7461 6c6c 2075 7367 732d 7374   install usgs-st
-00000910: 7265 6360 0a0a 2320 5570 6772 6164 650a  rec`..# Upgrade.
-00000920: 0a60 7069 7020 696e 7374 616c 6c20 2d2d  .`pip install --
-00000930: 7570 6772 6164 6520 7573 6773 2d73 7472  upgrade usgs-str
-00000940: 6563 600a 0a23 2043 6f6e 6669 6775 7261  ec`..# Configura
-00000950: 7469 6f6e 0a0a 496e 206f 7264 6572 2074  tion..In order t
-00000960: 6f20 7573 6520 5354 5245 4320 796f 7520  o use STREC you 
-00000970: 7769 6c6c 206e 6565 6420 746f 3a0a 0a20  will need to:.. 
-00000980: 2d20 646f 776e 6c6f 6164 2055 5347 5320  - download USGS 
-00000990: 536c 6162 2032 2e30 206d 6f64 656c 732c  Slab 2.0 models,
-000009a0: 2064 6573 6372 6962 6564 2061 7420 7468   described at th
-000009b0: 6520 5363 6965 6e63 6520 4261 7365 200a  e Science Base .
-000009c0: 2020 206c 696e 6b20 6162 6f76 652e 200a     link above. .
-000009d0: 202d 2063 7265 6174 6520 6120 6461 7461   - create a data
-000009e0: 6261 7365 206f 6620 6d6f 6d65 6e74 2074  base of moment t
-000009f0: 656e 736f 7273 2c20 6569 7468 6572 206d  ensors, either m
-00000a00: 616e 7561 6c6c 7920 6672 6f6d 2061 200a  anually from a .
-00000a10: 2020 2073 7072 6561 6473 6865 6574 2f43     spreadsheet/C
-00000a20: 5356 2066 696c 6520 2864 6573 6372 6962  SV file (describ
-00000a30: 6564 2062 656c 6f77 292c 206f 7220 6279  ed below), or by
-00000a40: 2064 6f77 6e6c 6f61 6469 6e67 200a 2020   downloading .  
-00000a50: 2061 2064 6566 6175 6c74 2064 6174 6162   a default datab
-00000a60: 6173 6520 6f66 206d 6f6d 656e 7420 7465  ase of moment te
-00000a70: 6e73 6f72 7320 6672 6f6d 2074 6865 200a  nsors from the .
-00000a80: 2020 205b 476c 6f62 616c 2043 656e 7472     [Global Centr
-00000a90: 6f69 6420 4d6f 6d65 6e74 2054 656e 736f  oid Moment Tenso
-00000aa0: 7220 2847 434d 5429 2063 6174 616c 6f67  r (GCMT) catalog
-00000ab0: 5d28 6874 7470 733a 2f2f 7777 772e 676c  ](https://www.gl
-00000ac0: 6f62 616c 636d 742e 6f72 672f 290a 202d  obalcmt.org/). -
-00000ad0: 2043 7265 6174 6520 6120 636f 6e66 6967   Create a config
-00000ae0: 7572 6174 696f 6e20 6669 6c65 2064 6573  uration file des
-00000af0: 6372 6962 696e 6720 7468 6520 6c6f 6361  cribing the loca
-00000b00: 7469 6f6e 7320 6f66 2074 6865 7365 2066  tions of these f
-00000b10: 696c 6573 2e0a 0a54 6f20 6d61 6b65 2074  iles...To make t
-00000b20: 6869 7320 6561 7369 6572 2c20 6120 636f  his easier, a co
-00000b30: 6e66 6967 7572 6174 696f 6e20 7072 6f67  nfiguration prog
-00000b40: 7261 6e20 6361 6c6c 6564 2060 7374 7265  ran called `stre
-00000b50: 635f 6366 6760 2069 7320 7072 6f76 6964  c_cfg` is provid
-00000b60: 6564 2077 6869 6368 2061 7574 6f6d 6174  ed which automat
-00000b70: 6573 200a 616c 6c20 6f66 2074 6865 7365  es .all of these
-00000b80: 2070 726f 6365 7373 6573 2e20 5468 6973   processes. This
-00000b90: 2070 726f 6772 616d 2063 6f6d 6573 2077   program comes w
-00000ba0: 6974 6820 7477 6f20 2a73 7562 2d63 6f6d  ith two *sub-com
-00000bb0: 6d61 6e64 732a 2063 616c 6c65 6420 6069  mands* called `i
-00000bc0: 6e66 6f60 2061 6e64 2060 7570 6461 7465  nfo` and `update
-00000bd0: 602e 200a 546f 2069 6e69 7469 616c 697a  `. .To initializ
-00000be0: 6520 7468 6520 7379 7374 656d 2077 6974  e the system wit
-00000bf0: 6820 7468 6520 536c 6162 2032 2e30 2067  h the Slab 2.0 g
-00000c00: 7269 6473 2061 6e64 2047 434d 5420 6d6f  rids and GCMT mo
-00000c10: 6d65 6e74 2074 656e 736f 7220 6461 7461  ment tensor data
-00000c20: 6261 7365 3a0a 0a60 7374 7265 635f 6366  base:..`strec_cf
-00000c30: 6720 7570 6461 7465 202d 2d64 6174 6166  g update --dataf
-00000c40: 6f6c 6465 7220 3c70 6174 682f 746f 2f64  older <path/to/d
-00000c50: 6174 612f 666f 6c64 6572 3e20 2d2d 736c  ata/folder> --sl
-00000c60: 6162 202d 2d67 636d 7460 0a0a 466f 7220  ab --gcmt`..For 
-00000c70: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
-00000c80: 7365 7420 7468 6520 5354 5245 4320 6461  set the STREC da
-00000c90: 7461 2066 6f6c 6465 7220 746f 2062 6520  ta folder to be 
-00000ca0: 2a2f 6461 7461 2f73 7472 6563 2a3a 0a0a  */data/strec*:..
-00000cb0: 6073 7472 6563 5f63 6667 2075 7064 6174  `strec_cfg updat
-00000cc0: 6520 2d2d 6461 7461 666f 6c64 6572 202f  e --datafolder /
-00000cd0: 6461 7461 2f73 7472 6563 202d 2d73 6c61  data/strec --sla
-00000ce0: 6220 2d2d 6763 6d74 600a 0a61 6e64 2074  b --gcmt`..and t
-00000cf0: 6865 6e20 7573 6520 7468 6520 666f 6c6c  hen use the foll
-00000d00: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
-00000d10: 2073 6565 2074 6865 2072 6573 756c 7469   see the resulti
-00000d20: 6e67 2063 6f6e 6669 6775 7261 7469 6f6e  ng configuration
-00000d30: 3a0a 0a60 7374 7265 635f 6366 6720 696e  :..`strec_cfg in
-00000d40: 666f 600a 0a54 6865 206f 7574 7075 7420  fo`..The output 
-00000d50: 7368 6f75 6c64 206c 6f6f 6b20 736f 6d65  should look some
-00000d60: 7468 696e 6720 6c69 6b65 2074 6865 2066  thing like the f
-00000d70: 6f6c 6c6f 7769 6e67 3a0a 0a60 6060 0a43  ollowing:..```.C
-00000d80: 6f6e 6669 6720 6669 6c65 202f 686f 6d65  onfig file /home
-00000d90: 2f75 7365 722f 2e73 7472 6563 2f63 6f6e  /user/.strec/con
-00000da0: 6669 672e 696e 693a 0a2d 2d2d 2d2d 2d2d  fig.ini:.-------
-00000db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000dc0: 2d0a 5b44 4154 415d 0a66 6f6c 6465 7220  -.[DATA].folder 
-00000dd0: 3d20 2f64 6174 612f 7374 7265 630a 736c  = /data/strec.sl
-00000de0: 6162 666f 6c64 6572 203d 202f 6461 7461  abfolder = /data
-00000df0: 2f73 7472 6563 2f73 6c61 6273 0a64 6266  /strec/slabs.dbf
-00000e00: 696c 6520 3d20 2f64 6174 612f 7374 7265  ile = /data/stre
-00000e10: 632f 6d6f 6d65 6e74 5f74 656e 736f 7273  c/moment_tensors
-00000e20: 2e64 620a 0a5b 434f 4e53 5441 4e54 535d  .db..[CONSTANTS]
-00000e30: 0a6d 696e 7261 6469 616c 5f64 6973 7468  .minradial_disth
-00000e40: 6973 7420 3d20 302e 3031 0a6d 6178 7261  ist = 0.01.maxra
-00000e50: 6469 616c 5f64 6973 7468 6973 7420 3d20  dial_disthist = 
-00000e60: 312e 300a 6d69 6e72 6164 6961 6c5f 6469  1.0.minradial_di
-00000e70: 7374 636f 6d70 203d 2030 2e35 0a6d 6178  stcomp = 0.5.max
-00000e80: 7261 6469 616c 5f64 6973 7463 6f6d 7020  radial_distcomp 
-00000e90: 3d20 312e 300a 7374 6570 5f64 6973 7463  = 1.0.step_distc
-00000ea0: 6f6d 7020 3d20 302e 310a 6465 7074 685f  omp = 0.1.depth_
-00000eb0: 7261 6e67 6563 6f6d 7020 3d20 3130 0a6d  rangecomp = 10.m
-00000ec0: 696e 6e6f 5f63 6f6d 7020 3d20 330a 6465  inno_comp = 3.de
-00000ed0: 6661 756c 745f 737a 6469 7020 3d20 3137  fault_szdip = 17
-00000ee0: 0a64 7374 7269 6b65 5f69 6e74 6572 6620  .dstrike_interf 
-00000ef0: 3d20 3330 0a64 6469 705f 696e 7465 7266  = 30.ddip_interf
-00000f00: 203d 2033 300a 646c 616d 6264 6120 3d20   = 30.dlambda = 
-00000f10: 3630 0a64 6465 7074 685f 696e 7465 7266  60.ddepth_interf
-00000f20: 203d 2032 300a 6464 6570 7468 5f69 6e74   = 20.ddepth_int
-00000f30: 7261 203d 2031 300a 2d2d 2d2d 2d2d 2d2d  ra = 10.--------
-00000f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f50: 0a0a 4d6f 6d65 6e74 2054 656e 736f 7220  ..Moment Tensor 
-00000f60: 4461 7461 6261 7365 2028 2f64 6174 612f  Database (/data/
-00000f70: 7374 7265 632f 6d6f 6d65 6e74 5f74 656e  strec/moment_ten
-00000f80: 736f 7273 2e64 6229 2063 6f6e 7461 696e  sors.db) contain
-00000f90: 7320 3630 3533 3520 6576 656e 7473 2066  s 60535 events f
-00000fa0: 726f 6d20 3120 736f 7572 6365 732e 0a0a  rom 1 sources...
-00000fb0: 5468 6572 6520 6172 6520 3133 3520 736c  There are 135 sl
-00000fc0: 6162 2067 7269 6473 2066 726f 6d20 3237  ab grids from 27
-00000fd0: 2075 6e69 7175 6520 736c 6162 206d 6f64   unique slab mod
-00000fe0: 656c 7320 6c6f 6361 7465 6420 696e 202f  els located in /
-00000ff0: 6461 7461 2f73 7472 6563 2f73 6c61 6273  data/strec/slabs
-00001000: 2e0a 6060 600a 0a23 2055 7361 6765 0a0a  ..```..# Usage..
-00001010: 6072 6567 6361 6c63 6020 6973 2074 6865  `regcalc` is the
-00001020: 2070 726f 6772 616d 2075 7365 6420 746f   program used to
-00001030: 2063 616c 6375 6c61 7465 2072 6567 696f   calculate regio
-00001040: 6e20 7061 7261 6d65 7465 7273 2e0a 0a54  n parameters...T
-00001050: 6865 2064 6574 6169 6c73 206f 6620 7468  he details of th
-00001060: 6520 6f70 7469 6f6e 7320 6172 6520 7669  e options are vi
-00001070: 7369 626c 6520 6279 2072 756e 6e69 6e67  sible by running
-00001080: 2060 7265 6763 616c 6320 2d2d 6865 6c70   `regcalc --help
-00001090: 602e 0a0a 5468 6520 7468 7265 6520 6d6f  `...The three mo
-000010a0: 7374 2062 6173 6963 2075 7365 2063 6173  st basic use cas
-000010b0: 6573 2061 7265 3a0a 0a20 2d20 4765 7474  es are:.. - Gett
-000010c0: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-000010d0: 6162 6f75 7420 616e 2065 7665 6e74 2062  about an event b
-000010e0: 7920 436f 6d43 6174 2049 443a 2060 7265  y ComCat ID: `re
-000010f0: 6763 616c 6320 2d64 2075 7336 3030 3069  gcalc -d us6000i
-00001100: 6430 7460 0a20 2d20 4765 7474 696e 6720  d0t`. - Getting 
-00001110: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-00001120: 7420 6120 2870 6f73 7369 626c 7920 7468  t a (possibly th
-00001130: 656f 7265 7469 6361 6c29 2065 7665 6e74  eoretical) event
-00001140: 2062 7920 7072 6f76 6964 696e 6720 6879   by providing hy
-00001150: 706f 6365 6e74 6572 2069 6e66 6f72 6d61  pocenter informa
-00001160: 7469 6f6e 3a20 6072 6567 6361 6c63 202d  tion: `regcalc -
-00001170: 6520 2d35 2e30 3733 3520 3130 332e 3038  e -5.0735 103.08
-00001180: 3236 2035 302e 3560 0a20 2d20 4765 7474  26 50.5`. - Gett
-00001190: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-000011a0: 6162 6f75 7420 6d6f 7265 2074 6861 6e20  about more than 
-000011b0: 6f6e 6520 6576 656e 742c 2077 6974 6820  one event, with 
-000011c0: 696e 7075 7420 6c69 6b65 2062 656c 6f77  input like below
-000011d0: 2061 7320 4578 6365 6c20 6f72 2043 5356   as Excel or CSV
-000011e0: 3a0a 0a3c 7461 626c 653e 0a3c 7472 3e20  :..<table>.<tr> 
-000011f0: 0a20 203c 7468 3e4c 6174 6974 7564 653c  .  <th>Latitude<
-00001200: 2f74 683e 0a20 203c 7468 3e4c 6f6e 6769  /th>.  <th>Longi
-00001210: 7475 6465 3c2f 7468 3e0a 2020 3c74 683e  tude</th>.  <th>
-00001220: 4465 7074 683c 2f74 683e 0a3c 2f74 723e  Depth</th>.</tr>
-00001230: 0a3c 7472 3e0a 2020 3c74 643e 2d35 2e30  .<tr>.  <td>-5.0
-00001240: 3734 3c2f 7464 3e0a 2020 3c74 643e 3130  74</td>.  <td>10
-00001250: 332e 3038 333c 2f74 643e 0a20 203c 7464  3.083</td>.  <td
-00001260: 3e35 302e 353c 2f74 643e 0a3c 2f74 723e  >50.5</td>.</tr>
-00001270: 0a3c 7472 3e0a 2020 3c74 643e 2d31 2e30  .<tr>.  <td>-1.0
-00001280: 3038 3c2f 7464 3e0a 2020 3c74 643e 3938  08</td>.  <td>98
-00001290: 2e36 3432 3c2f 7464 3e0a 2020 3c74 643e  .642</td>.  <td>
-000012a0: 3137 2e36 3c2f 7464 3e0a 3c2f 7472 3e0a  17.6</td>.</tr>.
-000012b0: 3c2f 7461 626c 653e 0a0a 6072 6567 6361  </table>..`regca
-000012c0: 6c63 202d 6920 696e 7075 745f 6669 6c65  lc -i input_file
-000012d0: 2e78 6c73 7860 0a0a 596f 7520 6361 6e20  .xlsx`..You can 
-000012e0: 6164 6420 6120 436f 6d43 6174 2049 4420  add a ComCat ID 
-000012f0: 636f 6c75 6d6e 2074 6f20 7468 6973 202d  column to this -
-00001300: 2074 6865 206e 616d 6520 7768 6963 6820   the name which 
-00001310: 7769 6c6c 2062 6520 6175 746f 6d61 7469  will be automati
-00001320: 6361 6c6c 7920 6465 7465 6374 6564 2069  cally detected i
-00001330: 7320 2a45 7665 6e74 4944 2a20 2863 6173  s *EventID* (cas
-00001340: 6520 646f 6573 206e 6f74 206d 6174 7465  e does not matte
-00001350: 7229 2e20 4966 2074 6865 2066 696c 6520  r). If the file 
-00001360: 6861 7320 616e 6f74 6865 7220 6e61 6d65  has another name
-00001370: 2066 6f72 2074 6865 2073 616d 6520 636f   for the same co
-00001380: 6c75 6d6e 2079 6f75 2063 616e 2073 7570  lumn you can sup
-00001390: 706c 7920 7468 6174 2077 6974 6820 7468  ply that with th
-000013a0: 6520 2d2d 6964 2d63 6f6c 756d 6e20 636f  e --id-column co
-000013b0: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
-000013c0: 6e3a 0a0a 6072 6567 6361 6c63 202d 6920  n:..`regcalc -i 
-000013d0: 696e 7075 745f 6669 6c65 2e78 6c73 7820  input_file.xlsx 
-000013e0: 2d2d 6964 2d63 6f6c 756d 6e20 6964 600a  --id-column id`.
-000013f0: 0a49 6620 7468 6520 6669 6c65 2063 6f6e  .If the file con
-00001400: 7461 696e 7320 636f 6c75 6d6e 206e 616d  tains column nam
-00001410: 6573 2066 6f72 206c 6174 6974 7564 652c  es for latitude,
-00001420: 206c 6f6e 6769 7475 6465 2061 6e64 2064   longitude and d
-00001430: 6570 7468 2074 6861 7420 646f 206e 6f74  epth that do not
-00001440: 206d 6174 6368 2074 6865 2072 6567 756c   match the regul
-00001450: 6172 2065 7870 7265 7373 696f 6e20 7061  ar expression pa
-00001460: 7474 6572 6e73 2022 5e6c 6174 222c 2022  tterns "^lat", "
-00001470: 5e6c 6f6e 222c 2022 5e64 6570 2220 2869  ^lon", "^dep" (i
-00001480: 676e 6f72 696e 6720 6361 7365 2920 7468  gnoring case) th
-00001490: 656e 2079 6f75 2063 616e 2073 7570 706c  en you can suppl
-000014a0: 7920 7468 6f73 6520 636f 6c75 6d6e 206e  y those column n
-000014b0: 616d 6573 2061 7320 7765 6c6c 2075 7369  ames as well usi
-000014c0: 6e67 2074 6865 202d 2d68 7970 6f2d 636f  ng the --hypo-co
-000014d0: 6c75 6d6e 7320 636f 6d6d 616e 6420 6c69  lumns command li
-000014e0: 6e65 206f 7074 696f 6e3a 0a0a 6072 6567  ne option:..`reg
-000014f0: 6361 6c63 202d 6920 696e 7075 745f 6669  calc -i input_fi
-00001500: 6c65 2e78 6c73 7820 2d2d 6879 706f 2d63  le.xlsx --hypo-c
-00001510: 6f6c 756d 6e73 2045 7665 6e74 4c61 7469  olumns EventLati
-00001520: 7475 6465 2045 7665 6e74 4c6f 6e67 6974  tude EventLongit
-00001530: 7564 6520 4576 656e 7444 6570 7468 600a  ude EventDepth`.
-00001540: 0a49 6620 616e 2069 6e70 7574 2073 7072  .If an input spr
-00001550: 6561 6473 6865 6574 2068 6173 206d 6f6d  eadsheet has mom
-00001560: 656e 7420 7465 6e73 6f72 2063 6f6c 756d  ent tensor colum
-00001570: 6e73 206e 616d 6564 204d 7272 2c20 4d74  ns named Mrr, Mt
-00001580: 742c 204d 7070 2c20 6574 632e 2028 6361  t, Mpp, etc. (ca
-00001590: 7365 2064 6f65 7320 6e6f 7420 6d61 7474  se does not matt
-000015a0: 6572 2920 7468 656e 2074 686f 7365 2076  er) then those v
-000015b0: 616c 7565 7320 7769 6c6c 2062 6520 7573  alues will be us
-000015c0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-000015d0: 7468 6520 4b61 6761 6e20 616e 676c 6520  the Kagan angle 
-000015e0: 616e 6420 6465 7465 726d 696e 6520 7468  and determine th
-000015f0: 6520 666f 6361 6c20 6d65 6368 616e 6973  e focal mechanis
-00001600: 6d2e 0a0a 596f 7520 6361 6e20 616c 736f  m...You can also
-00001610: 206f 7074 696f 6e61 6c6c 7920 7370 6563   optionally spec
-00001620: 6966 7920 6d6f 6d65 6e74 2074 656e 736f  ify moment tenso
-00001630: 7220 696e 666f 726d 6174 696f 6e20 666f  r information fo
-00001640: 7220 6120 7369 6e67 6c65 2065 7665 6e74  r a single event
-00001650: 2069 6e20 7468 6520 666f 726d 206f 6620   in the form of 
-00001660: 7374 7269 6b65 2f64 6970 2f72 616b 6520  strike/dip/rake 
-00001670: 616e 676c 6573 2061 6e64 2061 206d 6167  angles and a mag
-00001680: 6e69 7475 6465 2c20 7573 696e 6720 7468  nitude, using th
-00001690: 6520 2d2d 6d6f 6d65 6e74 2d69 6e66 6f20  e --moment-info 
-000016a0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-000016b0: 696f 6e3a 0a0a 6072 6567 6361 6c63 202d  ion:..`regcalc -
-000016c0: 6520 2d30 2e39 3530 202d 3231 2e37 3235  e -0.950 -21.725
-000016d0: 2031 302e 3020 2d6d 2032 3630 2038 3420   10.0 -m 260 84 
-000016e0: 3136 3920 362e 3960 0a0a 2a4e 6f74 653a  169 6.9`..*Note:
-000016f0: 2055 7365 7273 206d 6179 206e 6f74 6963   Users may notic
-00001700: 6520 7468 6174 2064 6973 7461 6e63 6573  e that distances
-00001710: 2074 6f20 7465 6374 6f6e 6963 2072 6567   to tectonic reg
-00001720: 696f 6e73 2074 6865 2065 6172 7468 7175  ions the earthqu
-00001730: 616b 6520 6973 204e 4f54 2069 6e20 6d61  ake is NOT in ma
-00001740: 7920 6265 2075 6e72 6561 736f 6e61 626c  y be unreasonabl
-00001750: 7920 6c61 7267 6520 7661 6c75 6573 2e20  y large values. 
-00001760: 5468 6520 7265 6173 6f6e 200a 666f 7220  The reason .for 
-00001770: 7265 7475 726e 696e 6720 7468 6520 6469  returning the di
-00001780: 7374 616e 6365 7320 746f 206f 7468 6572  stances to other
-00001790: 2072 6567 696f 6e73 2069 7320 746f 2068   regions is to h
-000017a0: 656c 7020 696e 666f 726d 2074 6865 2075  elp inform the u
-000017b0: 7365 7220 7768 656e 2074 6865 2065 6172  ser when the ear
-000017c0: 7468 7175 616b 6520 6973 2063 6c6f 7365  thquake is close
-000017d0: 2074 6f20 616e 6f74 6865 7220 7265 6769   to another regi
-000017e0: 6f6e 2e0a 5768 656e 2053 5452 4543 206f  on..When STREC o
-000017f0: 7574 7075 7473 2074 6865 7365 206c 6172  utputs these lar
-00001800: 6765 206e 756d 6265 7273 2069 7420 696e  ge numbers it in
-00001810: 6469 6361 7465 7320 7468 6174 2074 6865  dicates that the
-00001820: 2064 6973 7461 6e63 6520 746f 2074 6861   distance to tha
-00001830: 7420 6f74 6865 7220 7265 6769 6f6e 2069  t other region i
-00001840: 7320 6e6f 7420 636c 6f73 6520 656e 6f75  s not close enou
-00001850: 6768 2074 6f20 6166 6665 6374 0a74 6865  gh to affect.the
-00001860: 2070 726f 7065 7274 6965 7320 6f66 2074   properties of t
-00001870: 6865 2065 6172 7468 7175 616b 652e 2a0a  he earthquake.*.
-00001880: 0a0a 2320 476c 6f73 7361 7279 0a0a 5354  ..# Glossary..ST
-00001890: 5245 4320 6465 6669 6e65 7320 6120 6e75  REC defines a nu
-000018a0: 6d62 6572 206f 6620 7465 726d 7320 7468  mber of terms th
-000018b0: 6174 206d 6179 206e 6f74 2062 6520 636f  at may not be co
-000018c0: 6d6d 6f6e 6c79 0a75 6e64 6572 7374 6f6f  mmonly.understoo
-000018d0: 642c 2073 6f20 7468 6579 2061 7265 2065  d, so they are e
-000018e0: 7870 6c61 696e 6564 2068 6572 652e 2020  xplained here.  
-000018f0: 5468 6573 6520 7465 726d 7320 6d61 7920  These terms may 
-00001900: 6265 2064 6966 6665 7265 6e74 0a66 726f  be different.fro
-00001910: 6d20 7468 6520 4761 7263 6961 2070 6170  m the Garcia pap
-00001920: 6572 2075 706f 6e20 7768 6963 6820 7468  er upon which th
-00001930: 6973 2073 6f66 7477 6172 6520 6973 206f  is software is o
-00001940: 7269 6769 6e61 6c6c 7920 6261 7365 642e  riginally based.
-00001950: 0a0a 202d 202a 5465 6374 6f6e 6963 2052  .. - *Tectonic R
-00001960: 6567 696f 6e2a 3a20 4f6e 6520 6f66 2053  egion*: One of S
-00001970: 7562 6475 6374 696f 6e2c 2041 6374 6976  ubduction, Activ
-00001980: 652c 2048 6f74 5370 6f74 2c20 6f72 2053  e, HotSpot, or S
-00001990: 7461 626c 652e 0a20 2020 5765 2068 6176  table..   We hav
-000019a0: 6520 7370 6c69 7420 7570 2074 6865 2067  e split up the g
-000019b0: 6c6f 6265 2069 6e74 6f20 7468 6573 6520  lobe into these 
-000019c0: 666f 7572 2072 6567 696f 6e73 2c20 7375  four regions, su
-000019d0: 6368 2074 6861 7420 616e 790a 2020 2070  ch that any.   p
-000019e0: 6f69 6e74 206f 6e20 7468 6520 676c 6f62  oint on the glob
-000019f0: 6520 7368 6f75 6c64 2066 616c 6c20 696e  e should fall in
-00001a00: 746f 206f 6e65 2061 6e64 206f 6e6c 7920  to one and only 
-00001a10: 6f6e 6520 6f66 2074 6865 7365 0a20 2020  one of these.   
-00001a20: 7265 6769 6f6e 732e 0a20 2020 0a20 2020  regions..   .   
-00001a30: 2020 2a20 2a53 7562 6475 6374 696f 6e2a    * *Subduction*
-00001a40: 3a20 4120 7465 6374 6f6e 6963 2072 6567  : A tectonic reg
-00001a50: 696f 6e20 6465 6669 6e65 6420 6279 206f  ion defined by o
-00001a60: 6e65 2070 6c61 7465 2064 6573 6365 6e64  ne plate descend
-00001a70: 696e 6720 6265 6c6f 770a 2020 2020 2061  ing below.     a
-00001a80: 6e6f 7468 6572 2028 652e 672e 2c20 7468  nother (e.g., th
-00001a90: 6520 7765 7374 6572 6e20 706f 7274 696f  e western portio
-00001aa0: 6e20 6f66 2074 6865 2055 6e69 7465 6420  n of the United 
-00001ab0: 5374 6174 6573 292c 206d 6f72 6520 7370  States), more sp
-00001ac0: 6563 6966 6963 616c 6c79 0a20 2020 2020  ecifically.     
-00001ad0: 6279 2074 686f 7365 206c 6f63 6174 696f  by those locatio
-00001ae0: 6e73 2061 626f 7665 2074 6865 2053 6c61  ns above the Sla
-00001af0: 6232 2e30 2067 7269 6473 2e0a 0a20 2020  b2.0 grids...   
-00001b00: 2020 2a20 2a41 6374 6976 652a 3a20 4120    * *Active*: A 
-00001b10: 7465 6374 6f6e 6963 2072 6567 696f 6e20  tectonic region 
-00001b20: 7768 6963 6820 6578 7065 7269 656e 6365  which experience
-00001b30: 7320 6372 7573 7461 6c20 6465 666f 726d  s crustal deform
-00001b40: 6174 696f 6e20 6475 650a 2020 2020 2074  ation due.     t
-00001b50: 6f20 706c 6174 6520 7465 6374 6f6e 6963  o plate tectonic
-00001b60: 732e 0a0a 2020 2020 202a 202a 486f 7453  s...     * *HotS
-00001b70: 706f 742a 3a20 4120 7465 6374 6f6e 6963  pot*: A tectonic
-00001b80: 2072 6567 696f 6e20 7768 6963 6820 6973   region which is
-00001b90: 2073 6974 7469 6e67 2061 626f 7665 206d   sitting above m
-00001ba0: 616e 746c 6520 706c 756d 6573 2c20 0a20  antle plumes, . 
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2077 6865 7265 206d 6167 6d61 2070 7573   where magma pus
-00001bd0: 6865 7320 7468 726f 7567 6820 6372 6163  hes through crac
-00001be0: 6b73 2069 6e20 7468 6520 6372 7573 742e  ks in the crust.
-00001bf0: 0a0a 2020 2020 202a 202a 5374 6162 6c65  ..     * *Stable
-00001c00: 2a3a 2054 6563 746f 6e69 6320 7265 6769  *: Tectonic regi
-00001c10: 6f6e 7320 7768 6963 6820 756e 6c69 6b65  ons which unlike
-00001c20: 2041 6374 6976 6520 7265 6769 6f6e 732c   Active regions,
-00001c30: 2064 6f20 6e6f 740a 2020 2020 2065 7870   do not.     exp
-00001c40: 6572 6965 6e63 6520 6372 7573 7461 6c20  erience crustal 
-00001c50: 6465 666f 726d 6174 696f 6e20 2865 2e67  deformation (e.g
-00001c60: 2e2c 2074 6865 2069 6e74 6572 696f 7220  ., the interior 
-00001c70: 6f66 2074 6865 0a20 2020 2020 4175 7374  of the.     Aust
-00001c80: 7261 6c69 616e 2063 6f6e 7469 6e65 6e74  ralian continent
-00001c90: 2e29 0a0a 215b 4d61 7020 7368 6f77 696e  .)..![Map showin
-00001ca0: 6720 7465 6374 6f6e 6963 2072 6567 696f  g tectonic regio
-00001cb0: 6e73 5d28 7365 6c65 6374 5f72 6567 696f  ns](select_regio
-00001cc0: 6e73 2e70 6e67 2022 4d61 7020 5368 6f77  ns.png "Map Show
-00001cd0: 696e 6720 5465 6374 6f6e 6963 2052 6567  ing Tectonic Reg
-00001ce0: 696f 6e73 2229 0a2a 4669 6720 3120 2d20  ions").*Fig 1 - 
-00001cf0: 4d61 7020 7368 6f77 696e 6720 7465 6374  Map showing tect
-00001d00: 6f6e 6963 2072 6567 696f 6e73 2e20 4143  onic regions. AC
-00001d10: 523d 4163 7469 7665 2043 7275 7374 616c  R=Active Crustal
-00001d20: 2052 6567 696f 6e2c 2053 5542 3d53 7562   Region, SUB=Sub
-00001d30: 6475 6374 696f 6e20 5a6f 6e65 2c20 564f  duction Zone, VO
-00001d40: 4c3d 486f 7453 706f 7420 5265 6769 6f6e  L=HotSpot Region
-00001d50: 2c20 5343 523d 5374 6162 6c65 2043 6f6e  , SCR=Stable Con
-00001d60: 7469 6e65 6e74 616c 2052 6567 696f 6e2a  tinental Region*
-00001d70: 200a 0a20 2d20 2a4f 6365 616e 6963 2a3a   .. - *Oceanic*:
-00001d80: 2041 6e6f 7468 6572 2072 6567 696f 6e2c   Another region,
-00001d90: 206e 6f74 2065 7863 6c75 7369 7665 2077   not exclusive w
-00001da0: 6974 6820 7468 6520 666f 7572 2054 6563  ith the four Tec
-00001db0: 746f 6e69 630a 2020 2052 6567 696f 6e73  tonic.   Regions
-00001dc0: 2c20 7468 6174 2069 6e64 6963 6174 6573  , that indicates
-00001dd0: 2077 6865 7468 6572 2074 6865 2070 6f69   whether the poi
-00001de0: 6e74 2073 7570 706c 6965 6420 6973 2069  nt supplied is i
-00001df0: 6e20 7468 6520 6f63 6561 6e0a 2020 2028  n the ocean.   (
-00001e00: 692e 652e 2c20 6e6f 7420 636f 6e74 696e  i.e., not contin
-00001e10: 656e 7461 6c29 2e0a 0a20 2d20 2a43 6f6e  ental)... - *Con
-00001e20: 7469 6e65 6e74 616c 2a3a 2054 6865 206f  tinental*: The o
-00001e30: 7070 6f73 6974 6520 6f66 204f 6365 616e  pposite of Ocean
-00001e40: 6963 2e0a 0a20 2d20 2a46 6f63 616c 204d  ic... - *Focal M
-00001e50: 6563 6861 6e69 736d 2a3a 2041 2073 6574  echanism*: A set
-00001e60: 206f 6620 7061 7261 6d65 7465 7273 2074   of parameters t
-00001e70: 6861 7420 6465 6669 6e65 2074 6865 2064  hat define the d
-00001e80: 6566 6f72 6d61 7469 6f6e 2069 6e0a 2020  eformation in.  
-00001e90: 2074 6865 2073 6f75 7263 6520 7265 6769   the source regi
-00001ea0: 6f6e 2074 6861 7420 6765 6e65 7261 7465  on that generate
-00001eb0: 7320 7468 6520 7365 6973 6d69 6320 7761  s the seismic wa
-00001ec0: 7665 7320 6f66 2061 6e20 6561 7274 6871  ves of an earthq
-00001ed0: 7561 6b65 2e0a 0a20 2d20 2a54 656e 736f  uake... - *Tenso
-00001ee0: 7220 5479 7065 2a3a 2054 6865 2073 686f  r Type*: The sho
-00001ef0: 7274 206e 616d 6520 666f 7220 7468 6520  rt name for the 
-00001f00: 616c 676f 7269 7468 6d20 7573 6564 2074  algorithm used t
-00001f10: 6f20 6765 6e65 7261 7465 0a20 2020 7468  o generate.   th
-00001f20: 6520 6d6f 6d65 6e74 2074 656e 736f 7220  e moment tensor 
-00001f30: 7573 6564 2074 6f20 6465 7465 726d 696e  used to determin
-00001f40: 6520 666f 6361 6c20 6d65 6368 616e 6973  e focal mechanis
-00001f50: 6d2c 204b 6167 616e 2061 6e67 6c65 2c0a  m, Kagan angle,.
-00001f60: 2020 2065 7463 2e20 2054 6869 7320 6973     etc.  This is
-00001f70: 2075 7375 616c 6c79 2061 2073 686f 7274   usually a short
-00001f80: 2063 6f64 6520 6c69 6b65 202a 4d77 772a   code like *Mww*
-00001f90: 2028 572d 7068 6173 6529 2c20 2a4d 7772   (W-phase), *Mwr
-00001fa0: 2a0a 2020 2028 7265 6769 6f6e 616c 292c  *.   (regional),
-00001fb0: 202a 4d77 622a 2028 626f 6479 2077 6176   *Mwb* (body wav
-00001fc0: 6529 2c20 6f72 202a 636f 6d70 6f73 6974  e), or *composit
-00001fd0: 652a 2c20 7768 6963 6820 696e 6469 6361  e*, which indica
-00001fe0: 7465 7320 7468 6174 0a20 2020 7468 6572  tes that.   ther
-00001ff0: 6520 6973 206e 6f20 636f 6d70 7574 6564  e is no computed
-00002000: 206d 6f6d 656e 7420 7465 6e73 6f72 2c20   moment tensor, 
-00002010: 736f 2061 2063 6f6d 706f 7369 7465 206f  so a composite o
-00002020: 6620 6869 7374 6f72 6963 616c 0a20 2020  f historical.   
-00002030: 6d6f 6d65 6e74 2074 656e 736f 7273 2061  moment tensors a
-00002040: 726f 756e 6420 7468 6520 696e 7075 7420  round the input 
-00002050: 636f 6f72 6469 6e61 7465 7320 6973 2075  coordinates is u
-00002060: 7365 6420 696e 7374 6561 642e 0a0a 202d  sed instead... -
-00002070: 202a 5465 6e73 6f72 2053 6f75 7263 652a   *Tensor Source*
-00002080: 3a20 5768 656e 2061 7661 696c 6162 6c65  : When available
-00002090: 2c20 7468 6973 2069 7320 7573 7561 6c6c  , this is usuall
-000020a0: 7920 7468 6520 6e65 7477 6f72 6b20 7468  y the network th
-000020b0: 6174 0a20 2020 636f 6e74 7269 6275 7465  at.   contribute
-000020c0: 6420 7468 6520 6d6f 6d65 6e74 2074 656e  d the moment ten
-000020d0: 736f 722c 2066 6f6c 6c6f 7765 6420 6279  sor, followed by
-000020e0: 2074 6865 2049 4420 7573 6564 2062 7920   the ID used by 
-000020f0: 7468 6174 0a20 2020 6e65 7477 6f72 6b20  that.   network 
-00002100: 2865 2e67 2e2c 2075 735f 3230 3030 626d  (e.g., us_2000bm
-00002110: 6367 292e 0a0a 202d 202a 4b61 6761 6e20  cg)... - *Kagan 
-00002120: 416e 676c 652a 3a20 416e 2073 696e 676c  Angle*: An singl
-00002130: 6520 616e 676c 6520 6265 7477 6565 6e20  e angle between 
-00002140: 616e 7920 7477 6f20 6d6f 6d65 6e74 2074  any two moment t
-00002150: 656e 736f 7273 206f 7220 696e 0a20 2020  ensors or in.   
-00002160: 206f 7572 2063 6173 652c 2062 6574 7765   our case, betwe
-00002170: 656e 2061 206d 6f6d 656e 7420 7465 6e73  en a moment tens
-00002180: 6f72 2061 6e64 2061 2073 7562 6475 6374  or and a subduct
-00002190: 696e 6720 736c 6162 2e0a 0a20 2d20 2a43  ing slab... - *C
-000021a0: 6f6d 706f 7369 7465 204d 6f6d 656e 7420  omposite Moment 
-000021b0: 5465 6e73 6f72 2a3a 2057 6865 6e20 6d6f  Tensor*: When mo
-000021c0: 6d65 6e74 2074 656e 736f 7273 2061 7265  ment tensors are
-000021d0: 206e 6f74 2061 7661 696c 6162 6c65 200a   not available .
-000021e0: 2020 2020 666f 7220 6120 6769 7665 6e20      for a given 
-000021f0: 6576 656e 742c 2061 2063 6f6d 706f 7369  event, a composi
-00002200: 7465 206d 6f6d 656e 7420 7465 6e73 6f72  te moment tensor
-00002210: 2069 7320 6361 6c63 756c 6174 6564 2062   is calculated b
-00002220: 7920 0a20 2020 2065 7373 656e 7469 616c  y .    essential
-00002230: 6c79 2074 616b 696e 6720 7468 6520 6d65  ly taking the me
-00002240: 616e 206f 6620 6174 206c 6561 7374 2074  an of at least t
-00002250: 6872 6565 206d 6f6d 656e 7420 7465 6e73  hree moment tens
-00002260: 6f72 7320 696e 2061 2030 2e31 200a 2020  ors in a 0.1 .  
-00002270: 2020 6465 6772 6565 2062 6f78 2073 7572    degree box sur
-00002280: 726f 756e 6469 6e67 2074 6865 2065 6172  rounding the ear
-00002290: 7468 7175 616b 6520 6879 706f 6365 6e74  thquake hypocent
-000022a0: 6572 2e0a 0a20 2d20 2a43 6f6d 706f 7369  er... - *Composi
-000022b0: 7465 2056 6172 6961 6269 6c69 7479 2a3a  te Variability*:
-000022c0: 2057 6865 6e20 7468 6520 6d6f 6d65 6e74   When the moment
-000022d0: 2074 656e 736f 7220 736f 6c75 7469 6f6e   tensor solution
-000022e0: 2069 7320 6f66 2074 7970 650a 202a 636f   is of type. *co
-000022f0: 6d70 6f73 6974 652a 2c20 6120 7363 616c  mposite*, a scal
-00002300: 6172 2076 616c 7565 2064 6573 6372 6962  ar value describ
-00002310: 696e 6720 7468 6520 7661 7269 6162 696c  ing the variabil
-00002320: 6974 7920 6f66 2074 6865 206d 6f6d 656e  ity of the momen
-00002330: 740a 2074 656e 736f 7273 2075 7365 6420  t. tensors used 
-00002340: 746f 2064 6574 6572 6d69 6e65 2074 6865  to determine the
-00002350: 2063 6f6d 706f 7369 7465 2e0a 0a20 2d20   composite... - 
-00002360: 2a44 6973 7461 6e63 6520 746f 205b 5265  *Distance to [Re
-00002370: 6769 6f6e 5d2a 3a20 5468 6520 6772 6561  gion]*: The grea
-00002380: 7420 6369 7263 6c65 2064 6973 7461 6e63  t circle distanc
-00002390: 6520 6672 6f6d 2074 6865 2069 6e70 7574  e from the input
-000023a0: 0a20 2020 636f 6f72 6469 6e61 7465 7320  .   coordinates 
-000023b0: 746f 2074 6865 206e 6561 7265 7374 2076  to the nearest v
-000023c0: 6572 7465 7820 6f66 205b 5265 6769 6f6e  ertex of [Region
-000023d0: 5d20 706f 6c79 676f 6e2e 0a0a 202d 202a  ] polygon... - *
-000023e0: 536c 6162 204d 6f64 656c 2052 6567 696f  Slab Model Regio
-000023f0: 6e2a 3a20 5765 2063 7572 7265 6e74 6c79  n*: We currently
-00002400: 2075 7365 2053 6c61 6220 322e 3020 7375   use Slab 2.0 su
-00002410: 6264 7563 7469 6f6e 206d 6f64 656c 730a  bduction models.
-00002420: 2020 2028 4861 7965 7320 3230 3132 292c     (Hayes 2012),
-00002430: 2077 6869 6368 2061 7265 2063 7572 7265   which are curre
-00002440: 6e74 6c79 2070 726f 7669 6465 6420 666f  ntly provided fo
-00002450: 7220 3237 2072 6567 696f 6e73 2061 726f  r 27 regions aro
-00002460: 756e 640a 2020 2074 6865 2067 6c6f 6265  und.   the globe
-00002470: 2e20 2054 6865 7365 2072 6567 696f 6e73  .  These regions
-00002480: 2061 7265 2064 6573 6372 6962 6564 2069   are described i
-00002490: 6e20 6465 7461 696c 2068 6572 653a 0a20  n detail here:. 
-000024a0: 2020 6874 7470 733a 2f2f 7777 772e 7363    https://www.sc
-000024b0: 6965 6e63 6562 6173 652e 676f 762f 6361  iencebase.gov/ca
-000024c0: 7461 6c6f 672f 6974 656d 2f35 6161 3162  talog/item/5aa1b
-000024d0: 3030 6565 3462 3062 3163 3339 3265 3836  00ee4b0b1c392e86
-000024e0: 3436 372f 0a0a 202d 202a 536c 6162 204d  467/.. - *Slab M
-000024f0: 6f64 656c 2044 6570 7468 2a3a 2054 6865  odel Depth*: The
-00002500: 2062 6573 7420 6573 7469 6d61 7465 206f   best estimate o
-00002510: 6620 6465 7074 6820 746f 2073 7562 6475  f depth to subdu
-00002520: 6374 696f 6e0a 2020 2069 6e74 6572 6661  ction.   interfa
-00002530: 6365 2e0a 0a20 2d20 2a53 6c61 6220 4d6f  ce... - *Slab Mo
-00002540: 6465 6c20 4465 7074 6820 556e 6365 7274  del Depth Uncert
-00002550: 6169 6e74 792a 3a20 5468 6520 6265 7374  ainty*: The best
-00002560: 2065 7374 696d 6174 6520 6f66 2074 6865   estimate of the
-00002570: 2075 6e63 6572 7461 696e 7479 0a20 2020   uncertainty.   
-00002580: 6f66 2074 6865 2064 6570 7468 2074 6f20  of the depth to 
-00002590: 7375 6264 7563 7469 6f6e 2069 6e74 6572  subduction inter
-000025a0: 6661 6365 2e0a 0a20 2d20 2a53 6c61 6220  face... - *Slab 
-000025b0: 4d6f 6465 6c20 4469 702a 3a20 5468 6520  Model Dip*: The 
-000025c0: 6265 7374 2065 7374 696d 6174 6520 6f66  best estimate of
-000025d0: 2074 6865 2064 6970 2061 6e67 6c65 206f   the dip angle o
-000025e0: 6620 7468 650a 2020 2073 7562 6475 6374  f the.   subduct
-000025f0: 696e 6720 706c 6174 652e 0a0a 202d 202a  ing plate... - *
-00002600: 536c 6162 204d 6f64 656c 2053 7472 696b  Slab Model Strik
-00002610: 652a 3a20 5468 6520 6265 7374 2065 7374  e*: The best est
-00002620: 696d 6174 6520 6f66 2074 6865 2073 7472  imate of the str
-00002630: 696b 6520 616e 676c 6520 6f66 2074 6865  ike angle of the
-00002640: 0a20 2020 7375 6264 7563 7469 6e67 2070  .   subducting p
-00002650: 6c61 7465 2e0a 0a                        late...
+00000000: 2320 5461 626c 6520 6f66 2043 6f6e 7465  # Table of Conte
+00000010: 6e74 730a 2d20 5b54 6162 6c65 206f 6620  nts.- [Table of 
+00000020: 436f 6e74 656e 7473 5d28 2374 6162 6c65  Contents](#table
+00000030: 2d6f 662d 636f 6e74 656e 7473 290a 2d20  -of-contents).- 
+00000040: 5b49 6e74 726f 6475 6374 696f 6e5d 2823  [Introduction](#
+00000050: 696e 7472 6f64 7563 7469 6f6e 290a 2d20  introduction).- 
+00000060: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00000070: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+00000080: 5b55 7067 7261 6465 5d28 2375 7067 7261  [Upgrade](#upgra
+00000090: 6465 290a 2d20 5b43 6f6e 6669 6775 7261  de).- [Configura
+000000a0: 7469 6f6e 5d28 2363 6f6e 6669 6775 7261  tion](#configura
+000000b0: 7469 6f6e 290a 2d20 5b55 7361 6765 5d28  tion).- [Usage](
+000000c0: 2375 7361 6765 290a 2d20 5b50 726f 6261  #usage).- [Proba
+000000d0: 6269 6c69 7469 6573 5d20 2823 7072 6f62  bilities] (#prob
+000000e0: 6162 696c 6974 6965 7329 0a2d 205b 476c  abilities).- [Gl
+000000f0: 6f73 7361 7279 5d28 2367 6c6f 7373 6172  ossary](#glossar
+00000100: 7929 0a0a 2320 496e 7472 6f64 7563 7469  y)..# Introducti
+00000110: 6f6e 0a0a 5468 6973 206c 6962 7261 7279  on..This library
+00000120: 2061 6e64 2073 6574 206f 6620 746f 6f6c   and set of tool
+00000130: 7320 7761 7320 6372 6561 7465 6420 746f  s was created to
+00000140: 2070 726f 7669 6465 2066 756e 6374 696f   provide functio
+00000150: 6e61 6c69 7479 2074 6f0a 6175 746f 6d61  nality to.automa
+00000160: 7469 6361 6c6c 7920 6465 7465 726d 696e  tically determin
+00000170: 6520 7468 6520 7465 6374 6f6e 6963 2072  e the tectonic r
+00000180: 6567 696f 6e20 6f66 2061 6e20 6561 7274  egion of an eart
+00000190: 6871 7561 6b65 0a28 5375 6264 7563 7469  hquake.(Subducti
+000001a0: 6f6e 2c20 4163 7469 7665 2c20 486f 7453  on, Active, HotS
+000001b0: 706f 742c 2053 7461 626c 6529 2c20 616e  pot, Stable), an
+000001c0: 6420 7468 6520 6469 7374 616e 6365 2074  d the distance t
+000001d0: 6f20 7468 6520 7465 6374 6f6e 6963 0a72  o the tectonic.r
+000001e0: 6567 696f 6e73 2074 6f20 7768 6963 6820  egions to which 
+000001f0: 6974 2064 6f65 7320 2a6e 6f74 2a20 6265  it does *not* be
+00000200: 6c6f 6e67 2e0a 0a49 6e20 6164 6469 7469  long...In additi
+00000210: 6f6e 2c20 5365 6973 6d6f 5465 6374 6f6e  on, SeismoTecton
+00000220: 6963 2052 6567 696d 6520 4561 7274 6871  ic Regime Earthq
+00000230: 7561 6b65 2043 616c 6375 6c61 746f 7220  uake Calculator 
+00000240: 2853 5452 4543 2920 7072 6f76 6964 6573  (STREC) provides
+00000250: 2061 2074 6f6f 6c20 7468 6174 2c20 0a69   a tool that, .i
+00000260: 6e20 7375 6264 7563 7469 6f6e 207a 6f6e  n subduction zon
+00000270: 6573 2c20 7265 7475 726e 7320 696e 666f  es, returns info
+00000280: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+00000290: 6520 7375 6264 7563 7469 6f6e 207a 6f6e  e subduction zon
+000002a0: 652c 2075 7369 6e67 2074 6865 200a 5553  e, using the .US
+000002b0: 4753 2053 6c61 6232 206d 6f64 656c 732e  GS Slab2 models.
+000002c0: 0a0a 2868 7474 7073 3a2f 2f77 7777 2e73  ..(https://www.s
+000002d0: 6369 656e 6365 6261 7365 2e67 6f76 2f63  ciencebase.gov/c
+000002e0: 6174 616c 6f67 2f69 7465 6d2f 3561 6131  atalog/item/5aa1
+000002f0: 6230 3065 6534 6230 6231 6333 3932 6538  b00ee4b0b1c392e8
+00000300: 3634 3637 2f29 2e0a 0a0a 5468 6973 2063  6467/)....This c
+00000310: 6f64 6520 7761 7320 6261 7365 6420 6f6e  ode was based on
+00000320: 2074 6865 205b 7061 7065 725d 2868 7474   the [paper](htt
+00000330: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00000340: 3137 3835 2f30 3132 3031 3130 3132 3429  1785/0120110124)
+00000350: 3a0a 0a60 6060 0a41 2047 6c6f 6261 6c20  :..```.A Global 
+00000360: 4561 7274 6871 7561 6b65 2044 6973 6372  Earthquake Discr
+00000370: 696d 696e 6174 696f 6e20 5363 6865 6d65  imination Scheme
+00000380: 2074 6f20 4f70 7469 6d69 7a65 2047 726f   to Optimize Gro
+00000390: 756e 64e2 8090 4d6f 7469 6f6e 2050 7265  und...Motion Pre
+000003a0: 6469 6374 696f 6e20 4571 7561 7469 6f6e  diction Equation
+000003b0: 2053 656c 6563 7469 6f6e 0a44 2e20 4761   Selection.D. Ga
+000003c0: 7263 c3ad 613b 2044 2e20 4a2e 2057 616c  rc..a; D. J. Wal
+000003d0: 643b 204d 2e20 472e 2048 6561 726e 650a  d; M. G. Hearne.
+000003e0: 4275 6c6c 6574 696e 206f 6620 7468 6520  Bulletin of the 
+000003f0: 5365 6973 6d6f 6c6f 6769 6361 6c20 536f  Seismological So
+00000400: 6369 6574 7920 6f66 2041 6d65 7269 6361  ciety of America
+00000410: 2028 3230 3132 2920 3130 3220 2831 293a   (2012) 102 (1):
+00000420: 2031 3835 e280 9332 3033 2e0a 6060 600a   185...203..```.
+00000430: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
+00000440: 0a0a 6070 6970 2069 6e73 7461 6c6c 2075  ..`pip install u
+00000450: 7367 732d 7374 7265 6360 0a0a 2320 5570  sgs-strec`..# Up
+00000460: 6772 6164 650a 0a60 7069 7020 696e 7374  grade..`pip inst
+00000470: 616c 6c20 2d2d 7570 6772 6164 6520 7573  all --upgrade us
+00000480: 6773 2d73 7472 6563 600a 0a23 2043 6f6e  gs-strec`..# Con
+00000490: 6669 6775 7261 7469 6f6e 0a0a 496e 206f  figuration..In o
+000004a0: 7264 6572 2074 6f20 7573 6520 5354 5245  rder to use STRE
+000004b0: 4320 796f 7520 7769 6c6c 206e 6565 6420  C you will need 
+000004c0: 746f 3a0a 0a20 2d20 646f 776e 6c6f 6164  to:.. - download
+000004d0: 2055 5347 5320 536c 6162 2032 2e30 206d   USGS Slab 2.0 m
+000004e0: 6f64 656c 732c 2064 6573 6372 6962 6564  odels, described
+000004f0: 2061 7420 7468 6520 5363 6965 6e63 6520   at the Science 
+00000500: 4261 7365 200a 2020 206c 696e 6b20 6162  Base .   link ab
+00000510: 6f76 652e 200a 202d 2063 7265 6174 6520  ove. . - create 
+00000520: 6120 6461 7461 6261 7365 206f 6620 6d6f  a database of mo
+00000530: 6d65 6e74 2074 656e 736f 7273 2c20 6569  ment tensors, ei
+00000540: 7468 6572 206d 616e 7561 6c6c 7920 6672  ther manually fr
+00000550: 6f6d 2061 200a 2020 2073 7072 6561 6473  om a .   spreads
+00000560: 6865 6574 2f43 5356 2066 696c 6520 2864  heet/CSV file (d
+00000570: 6573 6372 6962 6564 2062 656c 6f77 292c  escribed below),
+00000580: 206f 7220 6279 2064 6f77 6e6c 6f61 6469   or by downloadi
+00000590: 6e67 200a 2020 2061 2064 6566 6175 6c74  ng .   a default
+000005a0: 2064 6174 6162 6173 6520 6f66 206d 6f6d   database of mom
+000005b0: 656e 7420 7465 6e73 6f72 7320 6672 6f6d  ent tensors from
+000005c0: 2074 6865 200a 2020 205b 476c 6f62 616c   the .   [Global
+000005d0: 2043 656e 7472 6f69 6420 4d6f 6d65 6e74   Centroid Moment
+000005e0: 2054 656e 736f 7220 2847 434d 5429 2063   Tensor (GCMT) c
+000005f0: 6174 616c 6f67 5d28 6874 7470 733a 2f2f  atalog](https://
+00000600: 7777 772e 676c 6f62 616c 636d 742e 6f72  www.globalcmt.or
+00000610: 672f 290a 202d 2043 7265 6174 6520 6120  g/). - Create a 
+00000620: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00000630: 6c65 2064 6573 6372 6962 696e 6720 7468  le describing th
+00000640: 6520 6c6f 6361 7469 6f6e 7320 6f66 2074  e locations of t
+00000650: 6865 7365 2066 696c 6573 2e0a 0a54 6f20  hese files...To 
+00000660: 6d61 6b65 2074 6869 7320 6561 7369 6572  make this easier
+00000670: 2c20 6120 636f 6e66 6967 7572 6174 696f  , a configuratio
+00000680: 6e20 7072 6f67 7261 6e20 6361 6c6c 6564  n progran called
+00000690: 2060 7374 7265 635f 6366 6760 2069 7320   `strec_cfg` is 
+000006a0: 7072 6f76 6964 6564 2077 6869 6368 2061  provided which a
+000006b0: 7574 6f6d 6174 6573 200a 616c 6c20 6f66  utomates .all of
+000006c0: 2074 6865 7365 2070 726f 6365 7373 6573   these processes
+000006d0: 2e20 5468 6973 2070 726f 6772 616d 2063  . This program c
+000006e0: 6f6d 6573 2077 6974 6820 7477 6f20 2a73  omes with two *s
+000006f0: 7562 2d63 6f6d 6d61 6e64 732a 2063 616c  ub-commands* cal
+00000700: 6c65 6420 6069 6e66 6f60 2061 6e64 2060  led `info` and `
+00000710: 7570 6461 7465 602e 200a 546f 2069 6e69  update`. .To ini
+00000720: 7469 616c 697a 6520 7468 6520 7379 7374  tialize the syst
+00000730: 656d 2077 6974 6820 7468 6520 536c 6162  em with the Slab
+00000740: 2032 2e30 2067 7269 6473 2061 6e64 2047   2.0 grids and G
+00000750: 434d 5420 6d6f 6d65 6e74 2074 656e 736f  CMT moment tenso
+00000760: 7220 6461 7461 6261 7365 3a0a 0a60 7374  r database:..`st
+00000770: 7265 635f 6366 6720 7570 6461 7465 202d  rec_cfg update -
+00000780: 2d64 6174 6166 6f6c 6465 7220 3c70 6174  -datafolder <pat
+00000790: 682f 746f 2f64 6174 612f 666f 6c64 6572  h/to/data/folder
+000007a0: 3e20 2d2d 736c 6162 202d 2d67 636d 7460  > --slab --gcmt`
+000007b0: 0a0a 466f 7220 6578 616d 706c 652c 2069  ..For example, i
+000007c0: 6620 796f 7520 7365 7420 7468 6520 5354  f you set the ST
+000007d0: 5245 4320 6461 7461 2066 6f6c 6465 7220  REC data folder 
+000007e0: 746f 2062 6520 2a2f 6461 7461 2f73 7472  to be */data/str
+000007f0: 6563 2a3a 0a0a 6073 7472 6563 5f63 6667  ec*:..`strec_cfg
+00000800: 2075 7064 6174 6520 2d2d 6461 7461 666f   update --datafo
+00000810: 6c64 6572 202f 6461 7461 2f73 7472 6563  lder /data/strec
+00000820: 202d 2d73 6c61 6220 2d2d 6763 6d74 600a   --slab --gcmt`.
+00000830: 0a61 6e64 2074 6865 6e20 7573 6520 7468  .and then use th
+00000840: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00000850: 616e 6420 746f 2073 6565 2074 6865 2072  and to see the r
+00000860: 6573 756c 7469 6e67 2063 6f6e 6669 6775  esulting configu
+00000870: 7261 7469 6f6e 3a0a 0a60 7374 7265 635f  ration:..`strec_
+00000880: 6366 6720 696e 666f 600a 0a54 6865 206f  cfg info`..The o
+00000890: 7574 7075 7420 7368 6f75 6c64 206c 6f6f  utput should loo
+000008a0: 6b20 736f 6d65 7468 696e 6720 6c69 6b65  k something like
+000008b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+000008c0: 0a60 6060 0a43 6f6e 6669 6720 6669 6c65  .```.Config file
+000008d0: 202f 686f 6d65 2f75 7365 722f 2e73 7472   /home/user/.str
+000008e0: 6563 2f63 6f6e 6669 672e 696e 693a 0a2d  ec/config.ini:.-
+000008f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000900: 2d2d 2d2d 2d2d 2d0a 5b44 4154 415d 0a66  -------.[DATA].f
+00000910: 6f6c 6465 7220 3d20 2f64 6174 612f 7374  older = /data/st
+00000920: 7265 630a 736c 6162 666f 6c64 6572 203d  rec.slabfolder =
+00000930: 202f 6461 7461 2f73 7472 6563 2f73 6c61   /data/strec/sla
+00000940: 6273 0a64 6266 696c 6520 3d20 2f64 6174  bs.dbfile = /dat
+00000950: 612f 7374 7265 632f 6d6f 6d65 6e74 5f74  a/strec/moment_t
+00000960: 656e 736f 7273 2e64 620a 0a5b 434f 4e53  ensors.db..[CONS
+00000970: 5441 4e54 535d 0a6d 696e 7261 6469 616c  TANTS].minradial
+00000980: 5f64 6973 7468 6973 7420 3d20 302e 3031  _disthist = 0.01
+00000990: 0a6d 6178 7261 6469 616c 5f64 6973 7468  .maxradial_disth
+000009a0: 6973 7420 3d20 312e 300a 6d69 6e72 6164  ist = 1.0.minrad
+000009b0: 6961 6c5f 6469 7374 636f 6d70 203d 2030  ial_distcomp = 0
+000009c0: 2e35 0a6d 6178 7261 6469 616c 5f64 6973  .5.maxradial_dis
+000009d0: 7463 6f6d 7020 3d20 312e 300a 7374 6570  tcomp = 1.0.step
+000009e0: 5f64 6973 7463 6f6d 7020 3d20 302e 310a  _distcomp = 0.1.
+000009f0: 6465 7074 685f 7261 6e67 6563 6f6d 7020  depth_rangecomp 
+00000a00: 3d20 3130 0a6d 696e 6e6f 5f63 6f6d 7020  = 10.minno_comp 
+00000a10: 3d20 330a 6465 6661 756c 745f 737a 6469  = 3.default_szdi
+00000a20: 7020 3d20 3137 0a64 7374 7269 6b65 5f69  p = 17.dstrike_i
+00000a30: 6e74 6572 6620 3d20 3330 0a64 6469 705f  nterf = 30.ddip_
+00000a40: 696e 7465 7266 203d 2033 300a 646c 616d  interf = 30.dlam
+00000a50: 6264 6120 3d20 3630 0a64 6465 7074 685f  bda = 60.ddepth_
+00000a60: 696e 7465 7266 203d 2032 300a 6464 6570  interf = 20.ddep
+00000a70: 7468 5f69 6e74 7261 203d 2031 300a 2d2d  th_intra = 10.--
+00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a90: 2d2d 2d2d 2d2d 0a0a 4d6f 6d65 6e74 2054  ------..Moment T
+00000aa0: 656e 736f 7220 4461 7461 6261 7365 2028  ensor Database (
+00000ab0: 2f64 6174 612f 7374 7265 632f 6d6f 6d65  /data/strec/mome
+00000ac0: 6e74 5f74 656e 736f 7273 2e64 6229 2063  nt_tensors.db) c
+00000ad0: 6f6e 7461 696e 7320 3630 3533 3520 6576  ontains 60535 ev
+00000ae0: 656e 7473 2066 726f 6d20 3120 736f 7572  ents from 1 sour
+00000af0: 6365 732e 0a0a 5468 6572 6520 6172 6520  ces...There are 
+00000b00: 3133 3520 736c 6162 2067 7269 6473 2066  135 slab grids f
+00000b10: 726f 6d20 3237 2075 6e69 7175 6520 736c  rom 27 unique sl
+00000b20: 6162 206d 6f64 656c 7320 6c6f 6361 7465  ab models locate
+00000b30: 6420 696e 202f 6461 7461 2f73 7472 6563  d in /data/strec
+00000b40: 2f73 6c61 6273 2e0a 6060 600a 0a23 2055  /slabs..```..# U
+00000b50: 7361 6765 0a0a 6072 6567 6361 6c63 6020  sage..`regcalc` 
+00000b60: 6973 2074 6865 2070 726f 6772 616d 2075  is the program u
+00000b70: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+00000b80: 2072 6567 696f 6e20 7061 7261 6d65 7465   region paramete
+00000b90: 7273 2e0a 0a54 6865 2064 6574 6169 6c73  rs...The details
+00000ba0: 206f 6620 7468 6520 6f70 7469 6f6e 7320   of the options 
+00000bb0: 6172 6520 7669 7369 626c 6520 6279 2072  are visible by r
+00000bc0: 756e 6e69 6e67 2060 7265 6763 616c 6320  unning `regcalc 
+00000bd0: 2d2d 6865 6c70 602e 0a0a 5468 6520 7468  --help`...The th
+00000be0: 7265 6520 6d6f 7374 2062 6173 6963 2075  ree most basic u
+00000bf0: 7365 2063 6173 6573 2061 7265 3a0a 0a20  se cases are:.. 
+00000c00: 2d20 4765 7474 696e 6720 696e 666f 726d  - Getting inform
+00000c10: 6174 696f 6e20 6162 6f75 7420 616e 2065  ation about an e
+00000c20: 7665 6e74 2062 7920 436f 6d43 6174 2049  vent by ComCat I
+00000c30: 443a 2060 7265 6763 616c 6320 2d64 2075  D: `regcalc -d u
+00000c40: 7336 3030 3069 6430 7460 0a20 2d20 4765  s6000id0t`. - Ge
+00000c50: 7474 696e 6720 696e 666f 726d 6174 696f  tting informatio
+00000c60: 6e20 6162 6f75 7420 6120 2870 6f73 7369  n about a (possi
+00000c70: 626c 7920 7468 656f 7265 7469 6361 6c29  bly theoretical)
+00000c80: 2065 7665 6e74 2062 7920 7072 6f76 6964   event by provid
+00000c90: 696e 6720 6879 706f 6365 6e74 6572 2069  ing hypocenter i
+00000ca0: 6e66 6f72 6d61 7469 6f6e 3a20 6072 6567  nformation: `reg
+00000cb0: 6361 6c63 202d 6520 2d35 2e30 3733 3520  calc -e -5.0735 
+00000cc0: 3130 332e 3038 3236 2035 302e 3560 0a20  103.0826 50.5`. 
+00000cd0: 2d20 4765 7474 696e 6720 696e 666f 726d  - Getting inform
+00000ce0: 6174 696f 6e20 6162 6f75 7420 6d6f 7265  ation about more
+00000cf0: 2074 6861 6e20 6f6e 6520 6576 656e 742c   than one event,
+00000d00: 2077 6974 6820 696e 7075 7420 6c69 6b65   with input like
+00000d10: 2062 656c 6f77 2061 7320 4578 6365 6c20   below as Excel 
+00000d20: 6f72 2043 5356 3a0a 0a3c 7461 626c 653e  or CSV:..<table>
+00000d30: 0a3c 7472 3e20 0a20 203c 7468 3e4c 6174  .<tr> .  <th>Lat
+00000d40: 6974 7564 653c 2f74 683e 0a20 203c 7468  itude</th>.  <th
+00000d50: 3e4c 6f6e 6769 7475 6465 3c2f 7468 3e0a  >Longitude</th>.
+00000d60: 2020 3c74 683e 4465 7074 683c 2f74 683e    <th>Depth</th>
+00000d70: 0a3c 2f74 723e 0a3c 7472 3e0a 2020 3c74  .</tr>.<tr>.  <t
+00000d80: 643e 2d35 2e30 3734 3c2f 7464 3e0a 2020  d>-5.074</td>.  
+00000d90: 3c74 643e 3130 332e 3038 333c 2f74 643e  <td>103.083</td>
+00000da0: 0a20 203c 7464 3e35 302e 353c 2f74 643e  .  <td>50.5</td>
+00000db0: 0a3c 2f74 723e 0a3c 7472 3e0a 2020 3c74  .</tr>.<tr>.  <t
+00000dc0: 643e 2d31 2e30 3038 3c2f 7464 3e0a 2020  d>-1.008</td>.  
+00000dd0: 3c74 643e 3938 2e36 3432 3c2f 7464 3e0a  <td>98.642</td>.
+00000de0: 2020 3c74 643e 3137 2e36 3c2f 7464 3e0a    <td>17.6</td>.
+00000df0: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
+00000e00: 6072 6567 6361 6c63 202d 6920 696e 7075  `regcalc -i inpu
+00000e10: 745f 6669 6c65 2e78 6c73 7860 0a0a 596f  t_file.xlsx`..Yo
+00000e20: 7520 6361 6e20 6164 6420 6120 436f 6d43  u can add a ComC
+00000e30: 6174 2049 4420 636f 6c75 6d6e 2074 6f20  at ID column to 
+00000e40: 7468 6973 202d 2074 6865 206e 616d 6520  this - the name 
+00000e50: 7768 6963 6820 7769 6c6c 2062 6520 6175  which will be au
+00000e60: 746f 6d61 7469 6361 6c6c 7920 6465 7465  tomatically dete
+00000e70: 6374 6564 2069 7320 2a45 7665 6e74 4944  cted is *EventID
+00000e80: 2a20 2863 6173 6520 646f 6573 206e 6f74  * (case does not
+00000e90: 206d 6174 7465 7229 2e20 4966 2074 6865   matter). If the
+00000ea0: 2066 696c 6520 6861 7320 616e 6f74 6865   file has anothe
+00000eb0: 7220 6e61 6d65 2066 6f72 2074 6865 2073  r name for the s
+00000ec0: 616d 6520 636f 6c75 6d6e 2079 6f75 2063  ame column you c
+00000ed0: 616e 2073 7570 706c 7920 7468 6174 2077  an supply that w
+00000ee0: 6974 6820 7468 6520 2d2d 6964 2d63 6f6c  ith the --id-col
+00000ef0: 756d 6e20 636f 6d6d 616e 6420 6c69 6e65  umn command line
+00000f00: 206f 7074 696f 6e3a 0a0a 6072 6567 6361   option:..`regca
+00000f10: 6c63 202d 6920 696e 7075 745f 6669 6c65  lc -i input_file
+00000f20: 2e78 6c73 7820 2d2d 6964 2d63 6f6c 756d  .xlsx --id-colum
+00000f30: 6e20 6964 600a 0a49 6620 7468 6520 6669  n id`..If the fi
+00000f40: 6c65 2063 6f6e 7461 696e 7320 636f 6c75  le contains colu
+00000f50: 6d6e 206e 616d 6573 2066 6f72 206c 6174  mn names for lat
+00000f60: 6974 7564 652c 206c 6f6e 6769 7475 6465  itude, longitude
+00000f70: 2061 6e64 2064 6570 7468 2074 6861 7420   and depth that 
+00000f80: 646f 206e 6f74 206d 6174 6368 2074 6865  do not match the
+00000f90: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
+00000fa0: 696f 6e20 7061 7474 6572 6e73 2022 5e6c  ion patterns "^l
+00000fb0: 6174 222c 2022 5e6c 6f6e 222c 2022 5e64  at", "^lon", "^d
+00000fc0: 6570 2220 2869 676e 6f72 696e 6720 6361  ep" (ignoring ca
+00000fd0: 7365 2920 7468 656e 2079 6f75 2063 616e  se) then you can
+00000fe0: 2073 7570 706c 7920 7468 6f73 6520 636f   supply those co
+00000ff0: 6c75 6d6e 206e 616d 6573 2061 7320 7765  lumn names as we
+00001000: 6c6c 2075 7369 6e67 2074 6865 202d 2d68  ll using the --h
+00001010: 7970 6f2d 636f 6c75 6d6e 7320 636f 6d6d  ypo-columns comm
+00001020: 616e 6420 6c69 6e65 206f 7074 696f 6e3a  and line option:
+00001030: 0a0a 6072 6567 6361 6c63 202d 6920 696e  ..`regcalc -i in
+00001040: 7075 745f 6669 6c65 2e78 6c73 7820 2d2d  put_file.xlsx --
+00001050: 6879 706f 2d63 6f6c 756d 6e73 2045 7665  hypo-columns Eve
+00001060: 6e74 4c61 7469 7475 6465 2045 7665 6e74  ntLatitude Event
+00001070: 4c6f 6e67 6974 7564 6520 4576 656e 7444  Longitude EventD
+00001080: 6570 7468 600a 0a49 6620 616e 2069 6e70  epth`..If an inp
+00001090: 7574 2073 7072 6561 6473 6865 6574 2068  ut spreadsheet h
+000010a0: 6173 206d 6f6d 656e 7420 7465 6e73 6f72  as moment tensor
+000010b0: 2063 6f6c 756d 6e73 206e 616d 6564 204d   columns named M
+000010c0: 7272 2c20 4d74 742c 204d 7070 2c20 6574  rr, Mtt, Mpp, et
+000010d0: 632e 2028 6361 7365 2064 6f65 7320 6e6f  c. (case does no
+000010e0: 7420 6d61 7474 6572 2920 7468 656e 2074  t matter) then t
+000010f0: 686f 7365 2076 616c 7565 7320 7769 6c6c  hose values will
+00001100: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
+00001110: 756c 6174 6520 7468 6520 4b61 6761 6e20  ulate the Kagan 
+00001120: 616e 676c 6520 616e 6420 6465 7465 726d  angle and determ
+00001130: 696e 6520 7468 6520 666f 6361 6c20 6d65  ine the focal me
+00001140: 6368 616e 6973 6d2e 0a0a 596f 7520 6361  chanism...You ca
+00001150: 6e20 616c 736f 206f 7074 696f 6e61 6c6c  n also optionall
+00001160: 7920 7370 6563 6966 7920 6d6f 6d65 6e74  y specify moment
+00001170: 2074 656e 736f 7220 696e 666f 726d 6174   tensor informat
+00001180: 696f 6e20 666f 7220 6120 7369 6e67 6c65  ion for a single
+00001190: 2065 7665 6e74 2069 6e20 7468 6520 666f   event in the fo
+000011a0: 726d 206f 6620 7374 7269 6b65 2f64 6970  rm of strike/dip
+000011b0: 2f72 616b 6520 616e 676c 6573 2061 6e64  /rake angles and
+000011c0: 2061 206d 6167 6e69 7475 6465 2c20 7573   a magnitude, us
+000011d0: 696e 6720 7468 6520 2d2d 6d6f 6d65 6e74  ing the --moment
+000011e0: 2d69 6e66 6f20 636f 6d6d 616e 6420 6c69  -info command li
+000011f0: 6e65 206f 7074 696f 6e3a 0a0a 6072 6567  ne option:..`reg
+00001200: 6361 6c63 202d 6520 2d30 2e39 3530 202d  calc -e -0.950 -
+00001210: 3231 2e37 3235 2031 302e 3020 2d6d 2032  21.725 10.0 -m 2
+00001220: 3630 2038 3420 3136 3920 362e 3960 0a0a  60 84 169 6.9`..
+00001230: 2a4e 6f74 653a 2055 7365 7273 206d 6179  *Note: Users may
+00001240: 206e 6f74 6963 6520 7468 6174 2064 6973   notice that dis
+00001250: 7461 6e63 6573 2074 6f20 7465 6374 6f6e  tances to tecton
+00001260: 6963 2072 6567 696f 6e73 2074 6865 2065  ic regions the e
+00001270: 6172 7468 7175 616b 6520 6973 204e 4f54  arthquake is NOT
+00001280: 2069 6e20 6d61 7920 6265 2075 6e72 6561   in may be unrea
+00001290: 736f 6e61 626c 7920 6c61 7267 6520 7661  sonably large va
+000012a0: 6c75 6573 2e20 5468 6520 7265 6173 6f6e  lues. The reason
+000012b0: 200a 666f 7220 7265 7475 726e 696e 6720   .for returning 
+000012c0: 7468 6520 6469 7374 616e 6365 7320 746f  the distances to
+000012d0: 206f 7468 6572 2072 6567 696f 6e73 2069   other regions i
+000012e0: 7320 746f 2068 656c 7020 696e 666f 726d  s to help inform
+000012f0: 2074 6865 2075 7365 7220 7768 656e 2074   the user when t
+00001300: 6865 2065 6172 7468 7175 616b 6520 6973  he earthquake is
+00001310: 2063 6c6f 7365 2074 6f20 616e 6f74 6865   close to anothe
+00001320: 7220 7265 6769 6f6e 2e0a 5768 656e 2053  r region..When S
+00001330: 5452 4543 206f 7574 7075 7473 2074 6865  TREC outputs the
+00001340: 7365 206c 6172 6765 206e 756d 6265 7273  se large numbers
+00001350: 2069 7420 696e 6469 6361 7465 7320 7468   it indicates th
+00001360: 6174 2074 6865 2064 6973 7461 6e63 6520  at the distance 
+00001370: 746f 2074 6861 7420 6f74 6865 7220 7265  to that other re
+00001380: 6769 6f6e 2069 7320 6e6f 7420 636c 6f73  gion is not clos
+00001390: 6520 656e 6f75 6768 2074 6f20 6166 6665  e enough to affe
+000013a0: 6374 0a74 6865 2070 726f 7065 7274 6965  ct.the propertie
+000013b0: 7320 6f66 2074 6865 2065 6172 7468 7175  s of the earthqu
+000013c0: 616b 652e 2a0a 0a23 2050 726f 6261 6269  ake.*..# Probabi
+000013d0: 6c69 7469 6573 0a0a 5354 5245 4320 6e6f  lities..STREC no
+000013e0: 7720 6361 6c63 756c 6174 6573 2074 6865  w calculates the
+000013f0: 2070 726f 6261 6269 6c69 7469 6573 206f   probabilities o
+00001400: 6620 616e 2065 6172 7468 7175 616b 6520  f an earthquake 
+00001410: 6265 696e 6720 696e 2061 6e79 206f 6620  being in any of 
+00001420: 7468 6520 7465 6374 6f6e 6963 2072 6567  the tectonic reg
+00001430: 696f 6e73 2c20 616e 6420 616c 736f 2069  ions, and also i
+00001440: 6e0a 616e 7920 6f66 2074 6865 2076 6172  n.any of the var
+00001450: 696f 7573 2064 6566 696e 6564 2064 6570  ious defined dep
+00001460: 7468 2063 6174 6567 6f72 6965 732e 2046  th categories. F
+00001470: 6f72 2073 7562 6475 6374 696f 6e20 7265  or subduction re
+00001480: 6769 6f6e 7320 7468 6573 6520 6172 6520  gions these are 
+00001490: 6861 7264 636f 6465 6420 6173 200a 6372  hardcoded as .cr
+000014a0: 7573 7461 6c2c 2069 6e74 6572 6661 6365  ustal, interface
+000014b0: 2c20 616e 6420 696e 7472 6173 6c61 622e  , and intraslab.
+000014c0: 2046 6f72 206f 7468 6572 2072 6567 696f   For other regio
+000014d0: 6e73 2c20 7468 6520 2a64 6566 6175 6c74  ns, the *default
+000014e0: 2a20 636f 6e66 6967 7572 6174 696f 6e20  * configuration 
+000014f0: 696e 636c 7564 6573 2074 6865 2066 6f6c  includes the fol
+00001500: 6c6f 7769 6e67 3a0a 0a20 2d20 6163 725f  lowing:.. - acr_
+00001510: 7368 616c 6c6f 7720 3a20 6163 7469 7665  shallow : active
+00001520: 2065 6172 7468 7175 616b 6573 206f 6363   earthquakes occ
+00001530: 7572 7269 6e67 2061 626f 7665 2033 3020  urring above 30 
+00001540: 6b6d 0a20 2d20 6163 725f 6465 6570 202d  km. - acr_deep -
+00001550: 2061 6374 6976 6520 6561 7274 6871 7561   active earthqua
+00001560: 6b65 7320 6f63 6375 7272 696e 6720 6265  kes occurring be
+00001570: 6c6f 7720 3330 206b 6d0a 202d 2073 6372  low 30 km. - scr
+00001580: 5f73 6861 6c6c 6f77 202d 2073 7461 626c  _shallow - stabl
+00001590: 6520 6561 7274 6871 7561 6b65 7320 6174  e earthquakes at
+000015a0: 2061 6e79 2064 6570 7468 0a20 2d20 766f   any depth. - vo
+000015b0: 6c63 616e 6963 5f73 6861 6c6c 6f77 202d  lcanic_shallow -
+000015c0: 2076 6f6c 6361 6e69 6320 6561 7274 6871   volcanic earthq
+000015d0: 7561 6b65 7320 6174 2061 6e79 2064 6570  uakes at any dep
+000015e0: 7468 0a0a 2323 2050 726f 6261 6269 6c69  th..## Probabili
+000015f0: 7479 2063 6f6e 6669 6775 7261 7469 6f6e  ty configuration
+00001600: 0a0a 5573 6572 7320 6361 6e20 636f 6e66  ..Users can conf
+00001610: 6967 7572 6520 7468 6520 7072 6f62 6162  igure the probab
+00001620: 696c 6974 7920 7365 7474 696e 6773 2074  ility settings t
+00001630: 6f20 696e 636c 7564 6520 6d6f 7265 2066  o include more f
+00001640: 696e 656c 7920 6772 6169 6e65 6420 6465  inely grained de
+00001650: 7074 6820 7a6f 6e65 7320 666f 7220 6163  pth zones for ac
+00001660: 7469 7665 2c20 0a73 7461 626c 652c 2061  tive, .stable, a
+00001670: 6e64 2076 6f6c 6361 6e69 6320 7265 6769  nd volcanic regi
+00001680: 6f6e 732e 2054 6865 2064 6566 6175 6c74  ons. The default
+00001690: 2063 6f6e 6669 6720 6669 6c65 2069 7320   config file is 
+000016a0: 6c6f 6361 7465 6420 696e 2074 6865 205b  located in the [
+000016b0: 7265 706f 7369 746f 7279 5d20 0a28 6874  repository] .(ht
+000016c0: 7470 733a 2f2f 636f 6465 2e75 7367 732e  tps://code.usgs.
+000016d0: 676f 762f 6768 7363 2f65 7369 2f73 7472  gov/ghsc/esi/str
+000016e0: 6563 2f2d 2f62 6c6f 622f 6d61 696e 2f73  ec/-/blob/main/s
+000016f0: 7263 2f73 7472 6563 2f64 6174 612f 7365  rc/strec/data/se
+00001700: 6c65 6374 2e63 6f6e 6629 2061 6e64 200a  lect.conf) and .
+00001710: 696e 7374 616c 6c65 6420 7769 7468 2074  installed with t
+00001720: 6865 2073 6f66 7477 6172 652e 2054 6f20  he software. To 
+00001730: 6375 7374 6f6d 697a 6520 7468 6520 7072  customize the pr
+00001740: 6f62 6162 696c 6974 7920 6465 7074 6820  obability depth 
+00001750: 7a6f 6e65 732c 2064 6f77 6e6c 6f61 6420  zones, download 
+00001760: 6120 636f 7079 206f 6620 7468 6520 6669  a copy of the fi
+00001770: 6c65 2066 726f 6d20 0a74 6865 2072 6570  le from .the rep
+00001780: 6f73 6974 6f72 7920 616e 6420 7361 7665  ository and save
+00001790: 2069 7420 696e 2074 6865 205b 4441 5441   it in the [DATA
+000017a0: 5d2d 3e66 6f6c 6465 7220 696e 2074 6865  ]->folder in the
+000017b0: 2063 6f6e 6669 672e 696e 6920 6669 6c65   config.ini file
+000017c0: 2064 6573 6372 6962 6564 2061 626f 7665   described above
+000017d0: 2e0a 0a60 6060 0a5b 4441 5441 5d0a 666f  ...```.[DATA].fo
+000017e0: 6c64 6572 203d 202f 6461 7461 2f73 7472  lder = /data/str
+000017f0: 6563 0a60 6060 0a0a 5468 6520 7265 6c65  ec.```..The rele
+00001800: 7661 6e74 2073 6563 7469 6f6e 206f 6620  vant section of 
+00001810: 7468 6520 7365 6c65 6374 2e63 6f6e 6620  the select.conf 
+00001820: 6669 6c65 2074 6f20 6d6f 6469 6679 206c  file to modify l
+00001830: 6f6f 6b73 206c 696b 6520 7468 6520 666f  ooks like the fo
+00001840: 6c6c 6f77 696e 673a 0a0a 6060 600a 5b74  llowing:..```.[t
+00001850: 6563 746f 6e69 635f 7265 6769 6f6e 735d  ectonic_regions]
+00001860: 0a20 2020 205b 5b61 6372 5d5d 0a20 2020  .    [[acr]].   
+00001870: 2020 2020 2068 6f72 697a 6f6e 7461 6c5f       horizontal_
+00001880: 6275 6666 6572 203d 2031 3030 0a20 2020  buffer = 100.   
+00001890: 2020 2020 2076 6572 7469 6361 6c5f 6275       vertical_bu
+000018a0: 6666 6572 203d 2035 0a20 2020 2020 2020  ffer = 5.       
+000018b0: 2064 6570 7468 5f6c 6162 656c 7320 3d20   depth_labels = 
+000018c0: 7368 616c 6c6f 772c 2064 6565 700a 2020  shallow, deep.  
+000018d0: 2020 2020 2020 6d69 6e5f 6465 7074 6820        min_depth 
+000018e0: 3d20 2d49 6e66 2c20 3330 0a20 2020 2020  = -Inf, 30.     
+000018f0: 2020 206d 6178 5f64 6570 7468 203d 2033     max_depth = 3
+00001900: 302c 2049 6e66 0a20 2020 205b 5b73 6372  0, Inf.    [[scr
+00001910: 5d5d 0a20 2020 2020 2020 2068 6f72 697a  ]].        horiz
+00001920: 6f6e 7461 6c5f 6275 6666 6572 203d 2031  ontal_buffer = 1
+00001930: 3030 0a20 2020 2020 2020 2076 6572 7469  00.        verti
+00001940: 6361 6c5f 6275 6666 6572 203d 2035 0a20  cal_buffer = 5. 
+00001950: 2020 2020 2020 2064 6570 7468 5f6c 6162         depth_lab
+00001960: 656c 7320 3d20 7368 616c 6c6f 770a 2020  els = shallow.  
+00001970: 2020 2020 2020 6d69 6e5f 6465 7074 6820        min_depth 
+00001980: 3d20 2d49 6e66 0a20 2020 2020 2020 206d  = -Inf.        m
+00001990: 6178 5f64 6570 7468 203d 2049 6e66 0a20  ax_depth = Inf. 
+000019a0: 2020 205b 5b73 7562 6475 6374 696f 6e5d     [[subduction]
+000019b0: 5d0a 2020 2020 2020 2020 686f 7269 7a6f  ].        horizo
+000019c0: 6e74 616c 5f62 7566 6665 7220 3d20 3130  ntal_buffer = 10
+000019d0: 300a 2020 2020 2020 2020 7665 7274 6963  0.        vertic
+000019e0: 616c 5f62 7566 6665 7220 3d20 350a 2020  al_buffer = 5.  
+000019f0: 2020 2020 2020 6465 7074 685f 6c61 6265        depth_labe
+00001a00: 6c73 203d 2063 7275 7374 616c 2c20 696e  ls = crustal, in
+00001a10: 7465 7266 6163 652c 2069 6e74 7261 736c  terface, intrasl
+00001a20: 6162 0a20 2020 2020 2020 206d 696e 5f64  ab.        min_d
+00001a30: 6570 7468 203d 202d 496e 662c 2031 352c  epth = -Inf, 15,
+00001a40: 2037 300a 2020 2020 2020 2020 6d61 785f   70.        max_
+00001a50: 6465 7074 6820 3d20 3135 2c20 3730 2c20  depth = 15, 70, 
+00001a60: 496e 660a 2020 2020 2020 2020 7573 655f  Inf.        use_
+00001a70: 736c 6162 203d 2054 7275 650a 2020 2020  slab = True.    
+00001a80: 5b5b 766f 6c63 616e 6963 5d5d 0a20 2020  [[volcanic]].   
+00001a90: 2020 2020 2068 6f72 697a 6f6e 7461 6c5f       horizontal_
+00001aa0: 6275 6666 6572 203d 2031 300a 2020 2020  buffer = 10.    
+00001ab0: 2020 2020 7665 7274 6963 616c 5f62 7566      vertical_buf
+00001ac0: 6665 7220 3d20 350a 2020 2020 2020 2020  fer = 5.        
+00001ad0: 6465 7074 685f 6c61 6265 6c73 203d 2073  depth_labels = s
+00001ae0: 6861 6c6c 6f77 0a20 2020 2020 2020 206d  hallow.        m
+00001af0: 696e 5f64 6570 7468 203d 202d 496e 660a  in_depth = -Inf.
+00001b00: 2020 2020 2020 2020 6d61 785f 6465 7074          max_dept
+00001b10: 6820 3d20 496e 660a 6060 600a 0a54 6f20  h = Inf.```..To 
+00001b20: 6164 6420 6120 2264 6565 7022 2028 3130  add a "deep" (10
+00001b30: 206b 6d20 6f72 2064 6565 7065 7229 2063   km or deeper) c
+00001b40: 6174 6567 6f72 7920 746f 2074 6865 2073  ategory to the s
+00001b50: 6372 2073 6563 7469 6f6e 2c20 796f 7520  cr section, you 
+00001b60: 776f 756c 6420 6d6f 6469 6679 2074 6861  would modify tha
+00001b70: 7420 0a73 6563 7469 6f6e 2074 6f20 6c6f  t .section to lo
+00001b80: 6f6b 206c 696b 6520 7468 6520 666f 6c6c  ok like the foll
+00001b90: 6f77 696e 673a 0a0a 6060 600a 2020 2020  owing:..```.    
+00001ba0: 5b5b 7363 725d 5d0a 2020 2020 2020 2020  [[scr]].        
+00001bb0: 686f 7269 7a6f 6e74 616c 5f62 7566 6665  horizontal_buffe
+00001bc0: 7220 3d20 3130 300a 2020 2020 2020 2020  r = 100.        
+00001bd0: 7665 7274 6963 616c 5f62 7566 6665 7220  vertical_buffer 
+00001be0: 3d20 350a 2020 2020 2020 2020 6465 7074  = 5.        dept
+00001bf0: 685f 6c61 6265 6c73 203d 2073 6861 6c6c  h_labels = shall
+00001c00: 6f77 2c20 6465 6570 0a20 2020 2020 2020  ow, deep.       
+00001c10: 206d 696e 5f64 6570 7468 203d 202d 496e   min_depth = -In
+00001c20: 662c 2031 300a 2020 2020 2020 2020 6d61  f, 10.        ma
+00001c30: 785f 6465 7074 6820 3d20 3130 2c20 496e  x_depth = 10, In
+00001c40: 660a 6060 600a 0a0a 2320 476c 6f73 7361  f.```...# Glossa
+00001c50: 7279 0a0a 5354 5245 4320 6465 6669 6e65  ry..STREC define
+00001c60: 7320 6120 6e75 6d62 6572 206f 6620 7465  s a number of te
+00001c70: 726d 7320 7468 6174 206d 6179 206e 6f74  rms that may not
+00001c80: 2062 6520 636f 6d6d 6f6e 6c79 0a75 6e64   be commonly.und
+00001c90: 6572 7374 6f6f 642c 2073 6f20 7468 6579  erstood, so they
+00001ca0: 2061 7265 2065 7870 6c61 696e 6564 2068   are explained h
+00001cb0: 6572 652e 2020 5468 6573 6520 7465 726d  ere.  These term
+00001cc0: 7320 6d61 7920 6265 2064 6966 6665 7265  s may be differe
+00001cd0: 6e74 0a66 726f 6d20 7468 6520 4761 7263  nt.from the Garc
+00001ce0: 6961 2070 6170 6572 2075 706f 6e20 7768  ia paper upon wh
+00001cf0: 6963 6820 7468 6973 2073 6f66 7477 6172  ich this softwar
+00001d00: 6520 6973 206f 7269 6769 6e61 6c6c 7920  e is originally 
+00001d10: 6261 7365 642e 0a0a 202d 202a 5465 6374  based... - *Tect
+00001d20: 6f6e 6963 2052 6567 696f 6e2a 3a20 4f6e  onic Region*: On
+00001d30: 6520 6f66 2053 7562 6475 6374 696f 6e2c  e of Subduction,
+00001d40: 2041 6374 6976 652c 2048 6f74 5370 6f74   Active, HotSpot
+00001d50: 2c20 6f72 2053 7461 626c 652e 0a20 2020  , or Stable..   
+00001d60: 5765 2068 6176 6520 7370 6c69 7420 7570  We have split up
+00001d70: 2074 6865 2067 6c6f 6265 2069 6e74 6f20   the globe into 
+00001d80: 7468 6573 6520 666f 7572 2072 6567 696f  these four regio
+00001d90: 6e73 2c20 7375 6368 2074 6861 7420 616e  ns, such that an
+00001da0: 790a 2020 2070 6f69 6e74 206f 6e20 7468  y.   point on th
+00001db0: 6520 676c 6f62 6520 7368 6f75 6c64 2066  e globe should f
+00001dc0: 616c 6c20 696e 746f 206f 6e65 2061 6e64  all into one and
+00001dd0: 206f 6e6c 7920 6f6e 6520 6f66 2074 6865   only one of the
+00001de0: 7365 0a20 2020 7265 6769 6f6e 732e 0a20  se.   regions.. 
+00001df0: 2020 0a20 2020 2020 2a20 2a53 7562 6475    .     * *Subdu
+00001e00: 6374 696f 6e2a 3a20 4120 7465 6374 6f6e  ction*: A tecton
+00001e10: 6963 2072 6567 696f 6e20 6465 6669 6e65  ic region define
+00001e20: 6420 6279 206f 6e65 2070 6c61 7465 2064  d by one plate d
+00001e30: 6573 6365 6e64 696e 6720 6265 6c6f 770a  escending below.
+00001e40: 2020 2020 2061 6e6f 7468 6572 2028 652e       another (e.
+00001e50: 672e 2c20 7468 6520 7765 7374 6572 6e20  g., the western 
+00001e60: 706f 7274 696f 6e20 6f66 2074 6865 2055  portion of the U
+00001e70: 6e69 7465 6420 5374 6174 6573 292c 206d  nited States), m
+00001e80: 6f72 6520 7370 6563 6966 6963 616c 6c79  ore specifically
+00001e90: 0a20 2020 2020 6279 2074 686f 7365 206c  .     by those l
+00001ea0: 6f63 6174 696f 6e73 2061 626f 7665 2074  ocations above t
+00001eb0: 6865 2053 6c61 6232 2e30 2067 7269 6473  he Slab2.0 grids
+00001ec0: 2e0a 0a20 2020 2020 2a20 2a41 6374 6976  ...     * *Activ
+00001ed0: 652a 3a20 4120 7465 6374 6f6e 6963 2072  e*: A tectonic r
+00001ee0: 6567 696f 6e20 7768 6963 6820 6578 7065  egion which expe
+00001ef0: 7269 656e 6365 7320 6372 7573 7461 6c20  riences crustal 
+00001f00: 6465 666f 726d 6174 696f 6e20 6475 650a  deformation due.
+00001f10: 2020 2020 2074 6f20 706c 6174 6520 7465       to plate te
+00001f20: 6374 6f6e 6963 732e 0a0a 2020 2020 202a  ctonics...     *
+00001f30: 202a 486f 7453 706f 742a 3a20 4120 7465   *HotSpot*: A te
+00001f40: 6374 6f6e 6963 2072 6567 696f 6e20 7768  ctonic region wh
+00001f50: 6963 6820 6973 2073 6974 7469 6e67 2061  ich is sitting a
+00001f60: 626f 7665 206d 616e 746c 6520 706c 756d  bove mantle plum
+00001f70: 6573 2c20 0a20 2020 2020 2020 2020 2020  es, .           
+00001f80: 2020 2020 2020 2077 6865 7265 206d 6167         where mag
+00001f90: 6d61 2070 7573 6865 7320 7468 726f 7567  ma pushes throug
+00001fa0: 6820 6372 6163 6b73 2069 6e20 7468 6520  h cracks in the 
+00001fb0: 6372 7573 742e 0a0a 2020 2020 202a 202a  crust...     * *
+00001fc0: 5374 6162 6c65 2a3a 2054 6563 746f 6e69  Stable*: Tectoni
+00001fd0: 6320 7265 6769 6f6e 7320 7768 6963 6820  c regions which 
+00001fe0: 756e 6c69 6b65 2041 6374 6976 6520 7265  unlike Active re
+00001ff0: 6769 6f6e 732c 2064 6f20 6e6f 740a 2020  gions, do not.  
+00002000: 2020 2065 7870 6572 6965 6e63 6520 6372     experience cr
+00002010: 7573 7461 6c20 6465 666f 726d 6174 696f  ustal deformatio
+00002020: 6e20 2865 2e67 2e2c 2074 6865 2069 6e74  n (e.g., the int
+00002030: 6572 696f 7220 6f66 2074 6865 0a20 2020  erior of the.   
+00002040: 2020 4175 7374 7261 6c69 616e 2063 6f6e    Australian con
+00002050: 7469 6e65 6e74 2e29 0a0a 215b 4d61 7020  tinent.)..![Map 
+00002060: 7368 6f77 696e 6720 7465 6374 6f6e 6963  showing tectonic
+00002070: 2072 6567 696f 6e73 5d28 7365 6c65 6374   regions](select
+00002080: 5f72 6567 696f 6e73 2e70 6e67 2022 4d61  _regions.png "Ma
+00002090: 7020 5368 6f77 696e 6720 5465 6374 6f6e  p Showing Tecton
+000020a0: 6963 2052 6567 696f 6e73 2229 0a2a 4669  ic Regions").*Fi
+000020b0: 6720 3120 2d20 4d61 7020 7368 6f77 696e  g 1 - Map showin
+000020c0: 6720 7465 6374 6f6e 6963 2072 6567 696f  g tectonic regio
+000020d0: 6e73 2e20 4143 523d 4163 7469 7665 2043  ns. ACR=Active C
+000020e0: 7275 7374 616c 2052 6567 696f 6e2c 2053  rustal Region, S
+000020f0: 5542 3d53 7562 6475 6374 696f 6e20 5a6f  UB=Subduction Zo
+00002100: 6e65 2c20 564f 4c3d 486f 7453 706f 7420  ne, VOL=HotSpot 
+00002110: 5265 6769 6f6e 2c20 5343 523d 5374 6162  Region, SCR=Stab
+00002120: 6c65 2043 6f6e 7469 6e65 6e74 616c 2052  le Continental R
+00002130: 6567 696f 6e2a 200a 0a20 2d20 2a4f 6365  egion* .. - *Oce
+00002140: 616e 6963 2a3a 2041 6e6f 7468 6572 2072  anic*: Another r
+00002150: 6567 696f 6e2c 206e 6f74 2065 7863 6c75  egion, not exclu
+00002160: 7369 7665 2077 6974 6820 7468 6520 666f  sive with the fo
+00002170: 7572 2054 6563 746f 6e69 630a 2020 2052  ur Tectonic.   R
+00002180: 6567 696f 6e73 2c20 7468 6174 2069 6e64  egions, that ind
+00002190: 6963 6174 6573 2077 6865 7468 6572 2074  icates whether t
+000021a0: 6865 2070 6f69 6e74 2073 7570 706c 6965  he point supplie
+000021b0: 6420 6973 2069 6e20 7468 6520 6f63 6561  d is in the ocea
+000021c0: 6e0a 2020 2028 692e 652e 2c20 6e6f 7420  n.   (i.e., not 
+000021d0: 636f 6e74 696e 656e 7461 6c29 2e0a 0a20  continental)... 
+000021e0: 2d20 2a43 6f6e 7469 6e65 6e74 616c 2a3a  - *Continental*:
+000021f0: 2054 6865 206f 7070 6f73 6974 6520 6f66   The opposite of
+00002200: 204f 6365 616e 6963 2e0a 0a20 2d20 2a46   Oceanic... - *F
+00002210: 6f63 616c 204d 6563 6861 6e69 736d 2a3a  ocal Mechanism*:
+00002220: 2041 2073 6574 206f 6620 7061 7261 6d65   A set of parame
+00002230: 7465 7273 2074 6861 7420 6465 6669 6e65  ters that define
+00002240: 2074 6865 2064 6566 6f72 6d61 7469 6f6e   the deformation
+00002250: 2069 6e0a 2020 2074 6865 2073 6f75 7263   in.   the sourc
+00002260: 6520 7265 6769 6f6e 2074 6861 7420 6765  e region that ge
+00002270: 6e65 7261 7465 7320 7468 6520 7365 6973  nerates the seis
+00002280: 6d69 6320 7761 7665 7320 6f66 2061 6e20  mic waves of an 
+00002290: 6561 7274 6871 7561 6b65 2e0a 0a20 2d20  earthquake... - 
+000022a0: 2a54 656e 736f 7220 5479 7065 2a3a 2054  *Tensor Type*: T
+000022b0: 6865 2073 686f 7274 206e 616d 6520 666f  he short name fo
+000022c0: 7220 7468 6520 616c 676f 7269 7468 6d20  r the algorithm 
+000022d0: 7573 6564 2074 6f20 6765 6e65 7261 7465  used to generate
+000022e0: 0a20 2020 7468 6520 6d6f 6d65 6e74 2074  .   the moment t
+000022f0: 656e 736f 7220 7573 6564 2074 6f20 6465  ensor used to de
+00002300: 7465 726d 696e 6520 666f 6361 6c20 6d65  termine focal me
+00002310: 6368 616e 6973 6d2c 204b 6167 616e 2061  chanism, Kagan a
+00002320: 6e67 6c65 2c0a 2020 2065 7463 2e20 2054  ngle,.   etc.  T
+00002330: 6869 7320 6973 2075 7375 616c 6c79 2061  his is usually a
+00002340: 2073 686f 7274 2063 6f64 6520 6c69 6b65   short code like
+00002350: 202a 4d77 772a 2028 572d 7068 6173 6529   *Mww* (W-phase)
+00002360: 2c20 2a4d 7772 2a0a 2020 2028 7265 6769  , *Mwr*.   (regi
+00002370: 6f6e 616c 292c 202a 4d77 622a 2028 626f  onal), *Mwb* (bo
+00002380: 6479 2077 6176 6529 2c20 6f72 202a 636f  dy wave), or *co
+00002390: 6d70 6f73 6974 652a 2c20 7768 6963 6820  mposite*, which 
+000023a0: 696e 6469 6361 7465 7320 7468 6174 0a20  indicates that. 
+000023b0: 2020 7468 6572 6520 6973 206e 6f20 636f    there is no co
+000023c0: 6d70 7574 6564 206d 6f6d 656e 7420 7465  mputed moment te
+000023d0: 6e73 6f72 2c20 736f 2061 2063 6f6d 706f  nsor, so a compo
+000023e0: 7369 7465 206f 6620 6869 7374 6f72 6963  site of historic
+000023f0: 616c 0a20 2020 6d6f 6d65 6e74 2074 656e  al.   moment ten
+00002400: 736f 7273 2061 726f 756e 6420 7468 6520  sors around the 
+00002410: 696e 7075 7420 636f 6f72 6469 6e61 7465  input coordinate
+00002420: 7320 6973 2075 7365 6420 696e 7374 6561  s is used instea
+00002430: 642e 0a0a 202d 202a 5465 6e73 6f72 2053  d... - *Tensor S
+00002440: 6f75 7263 652a 3a20 5768 656e 2061 7661  ource*: When ava
+00002450: 696c 6162 6c65 2c20 7468 6973 2069 7320  ilable, this is 
+00002460: 7573 7561 6c6c 7920 7468 6520 6e65 7477  usually the netw
+00002470: 6f72 6b20 7468 6174 0a20 2020 636f 6e74  ork that.   cont
+00002480: 7269 6275 7465 6420 7468 6520 6d6f 6d65  ributed the mome
+00002490: 6e74 2074 656e 736f 722c 2066 6f6c 6c6f  nt tensor, follo
+000024a0: 7765 6420 6279 2074 6865 2049 4420 7573  wed by the ID us
+000024b0: 6564 2062 7920 7468 6174 0a20 2020 6e65  ed by that.   ne
+000024c0: 7477 6f72 6b20 2865 2e67 2e2c 2075 735f  twork (e.g., us_
+000024d0: 3230 3030 626d 6367 292e 0a0a 202d 202a  2000bmcg)... - *
+000024e0: 4b61 6761 6e20 416e 676c 652a 3a20 416e  Kagan Angle*: An
+000024f0: 2073 696e 676c 6520 616e 676c 6520 6265   single angle be
+00002500: 7477 6565 6e20 616e 7920 7477 6f20 6d6f  tween any two mo
+00002510: 6d65 6e74 2074 656e 736f 7273 206f 7220  ment tensors or 
+00002520: 696e 0a20 2020 206f 7572 2063 6173 652c  in.    our case,
+00002530: 2062 6574 7765 656e 2061 206d 6f6d 656e   between a momen
+00002540: 7420 7465 6e73 6f72 2061 6e64 2061 2073  t tensor and a s
+00002550: 7562 6475 6374 696e 6720 736c 6162 2e0a  ubducting slab..
+00002560: 0a20 2d20 2a43 6f6d 706f 7369 7465 204d  . - *Composite M
+00002570: 6f6d 656e 7420 5465 6e73 6f72 2a3a 2057  oment Tensor*: W
+00002580: 6865 6e20 6d6f 6d65 6e74 2074 656e 736f  hen moment tenso
+00002590: 7273 2061 7265 206e 6f74 2061 7661 696c  rs are not avail
+000025a0: 6162 6c65 200a 2020 2020 666f 7220 6120  able .    for a 
+000025b0: 6769 7665 6e20 6576 656e 742c 2061 2063  given event, a c
+000025c0: 6f6d 706f 7369 7465 206d 6f6d 656e 7420  omposite moment 
+000025d0: 7465 6e73 6f72 2069 7320 6361 6c63 756c  tensor is calcul
+000025e0: 6174 6564 2062 7920 0a20 2020 2065 7373  ated by .    ess
+000025f0: 656e 7469 616c 6c79 2074 616b 696e 6720  entially taking 
+00002600: 7468 6520 6d65 616e 206f 6620 6174 206c  the mean of at l
+00002610: 6561 7374 2074 6872 6565 206d 6f6d 656e  east three momen
+00002620: 7420 7465 6e73 6f72 7320 696e 2061 2030  t tensors in a 0
+00002630: 2e31 200a 2020 2020 6465 6772 6565 2062  .1 .    degree b
+00002640: 6f78 2073 7572 726f 756e 6469 6e67 2074  ox surrounding t
+00002650: 6865 2065 6172 7468 7175 616b 6520 6879  he earthquake hy
+00002660: 706f 6365 6e74 6572 2e0a 0a20 2d20 2a43  pocenter... - *C
+00002670: 6f6d 706f 7369 7465 2056 6172 6961 6269  omposite Variabi
+00002680: 6c69 7479 2a3a 2057 6865 6e20 7468 6520  lity*: When the 
+00002690: 6d6f 6d65 6e74 2074 656e 736f 7220 736f  moment tensor so
+000026a0: 6c75 7469 6f6e 2069 7320 6f66 2074 7970  lution is of typ
+000026b0: 650a 202a 636f 6d70 6f73 6974 652a 2c20  e. *composite*, 
+000026c0: 6120 7363 616c 6172 2076 616c 7565 2064  a scalar value d
+000026d0: 6573 6372 6962 696e 6720 7468 6520 7661  escribing the va
+000026e0: 7269 6162 696c 6974 7920 6f66 2074 6865  riability of the
+000026f0: 206d 6f6d 656e 740a 2074 656e 736f 7273   moment. tensors
+00002700: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
+00002710: 6e65 2074 6865 2063 6f6d 706f 7369 7465  ne the composite
+00002720: 2e0a 0a20 2d20 2a44 6973 7461 6e63 6520  ... - *Distance 
+00002730: 746f 205b 5265 6769 6f6e 5d2a 3a20 5468  to [Region]*: Th
+00002740: 6520 6772 6561 7420 6369 7263 6c65 2064  e great circle d
+00002750: 6973 7461 6e63 6520 6672 6f6d 2074 6865  istance from the
+00002760: 2069 6e70 7574 0a20 2020 636f 6f72 6469   input.   coordi
+00002770: 6e61 7465 7320 746f 2074 6865 206e 6561  nates to the nea
+00002780: 7265 7374 2076 6572 7465 7820 6f66 205b  rest vertex of [
+00002790: 5265 6769 6f6e 5d20 706f 6c79 676f 6e2e  Region] polygon.
+000027a0: 0a0a 202d 202a 536c 6162 204d 6f64 656c  .. - *Slab Model
+000027b0: 2052 6567 696f 6e2a 3a20 5765 2063 7572   Region*: We cur
+000027c0: 7265 6e74 6c79 2075 7365 2053 6c61 6220  rently use Slab 
+000027d0: 322e 3020 7375 6264 7563 7469 6f6e 206d  2.0 subduction m
+000027e0: 6f64 656c 730a 2020 2028 4861 7965 7320  odels.   (Hayes 
+000027f0: 3230 3132 292c 2077 6869 6368 2061 7265  2012), which are
+00002800: 2063 7572 7265 6e74 6c79 2070 726f 7669   currently provi
+00002810: 6465 6420 666f 7220 3237 2072 6567 696f  ded for 27 regio
+00002820: 6e73 2061 726f 756e 640a 2020 2074 6865  ns around.   the
+00002830: 2067 6c6f 6265 2e20 2054 6865 7365 2072   globe.  These r
+00002840: 6567 696f 6e73 2061 7265 2064 6573 6372  egions are descr
+00002850: 6962 6564 2069 6e20 6465 7461 696c 2068  ibed in detail h
+00002860: 6572 653a 0a20 2020 6874 7470 733a 2f2f  ere:.   https://
+00002870: 7777 772e 7363 6965 6e63 6562 6173 652e  www.sciencebase.
+00002880: 676f 762f 6361 7461 6c6f 672f 6974 656d  gov/catalog/item
+00002890: 2f35 6161 3162 3030 6565 3462 3062 3163  /5aa1b00ee4b0b1c
+000028a0: 3339 3265 3836 3436 372f 0a0a 202d 202a  392e86467/.. - *
+000028b0: 536c 6162 204d 6f64 656c 2044 6570 7468  Slab Model Depth
+000028c0: 2a3a 2054 6865 2062 6573 7420 6573 7469  *: The best esti
+000028d0: 6d61 7465 206f 6620 6465 7074 6820 746f  mate of depth to
+000028e0: 2073 7562 6475 6374 696f 6e0a 2020 2069   subduction.   i
+000028f0: 6e74 6572 6661 6365 2e0a 0a20 2d20 2a53  nterface... - *S
+00002900: 6c61 6220 4d6f 6465 6c20 4465 7074 6820  lab Model Depth 
+00002910: 556e 6365 7274 6169 6e74 792a 3a20 5468  Uncertainty*: Th
+00002920: 6520 6265 7374 2065 7374 696d 6174 6520  e best estimate 
+00002930: 6f66 2074 6865 2075 6e63 6572 7461 696e  of the uncertain
+00002940: 7479 0a20 2020 6f66 2074 6865 2064 6570  ty.   of the dep
+00002950: 7468 2074 6f20 7375 6264 7563 7469 6f6e  th to subduction
+00002960: 2069 6e74 6572 6661 6365 2e0a 0a20 2d20   interface... - 
+00002970: 2a53 6c61 6220 4d6f 6465 6c20 4469 702a  *Slab Model Dip*
+00002980: 3a20 5468 6520 6265 7374 2065 7374 696d  : The best estim
+00002990: 6174 6520 6f66 2074 6865 2064 6970 2061  ate of the dip a
+000029a0: 6e67 6c65 206f 6620 7468 650a 2020 2073  ngle of the.   s
+000029b0: 7562 6475 6374 696e 6720 706c 6174 652e  ubducting plate.
+000029c0: 0a0a 202d 202a 536c 6162 204d 6f64 656c  .. - *Slab Model
+000029d0: 2053 7472 696b 652a 3a20 5468 6520 6265   Strike*: The be
+000029e0: 7374 2065 7374 696d 6174 6520 6f66 2074  st estimate of t
+000029f0: 6865 2073 7472 696b 6520 616e 676c 6520  he strike angle 
+00002a00: 6f66 2074 6865 0a20 2020 7375 6264 7563  of the.   subduc
+00002a10: 7469 6e67 2070 6c61 7465 2e0a 0a         ting plate...
```

### Comparing `usgs-strec-2.2.5/README.md` & `usgs-strec-2.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,536 +1,752 @@
-00000000: 2320 5461 626c 6520 6f66 2043 6f6e 7465  # Table of Conte
-00000010: 6e74 730a 2d20 5b54 6162 6c65 206f 6620  nts.- [Table of 
-00000020: 436f 6e74 656e 7473 5d28 2374 6162 6c65  Contents](#table
-00000030: 2d6f 662d 636f 6e74 656e 7473 290a 2d20  -of-contents).- 
-00000040: 5b49 6e74 726f 6475 6374 696f 6e5d 2823  [Introduction](#
-00000050: 696e 7472 6f64 7563 7469 6f6e 290a 2d20  introduction).- 
-00000060: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
-00000070: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
-00000080: 5b55 7067 7261 6465 5d28 2375 7067 7261  [Upgrade](#upgra
-00000090: 6465 290a 2d20 5b43 6f6e 6669 6775 7261  de).- [Configura
-000000a0: 7469 6f6e 5d28 2363 6f6e 6669 6775 7261  tion](#configura
-000000b0: 7469 6f6e 290a 2d20 5b55 7361 6765 5d28  tion).- [Usage](
-000000c0: 2375 7361 6765 290a 2d20 5b47 6c6f 7373  #usage).- [Gloss
-000000d0: 6172 795d 2823 676c 6f73 7361 7279 290a  ary](#glossary).
-000000e0: 0a23 2049 6e74 726f 6475 6374 696f 6e0a  .# Introduction.
-000000f0: 0a54 6869 7320 6c69 6272 6172 7920 616e  .This library an
-00000100: 6420 7365 7420 6f66 2074 6f6f 6c73 2077  d set of tools w
-00000110: 6173 2063 7265 6174 6564 2074 6f20 7072  as created to pr
-00000120: 6f76 6964 6520 6675 6e63 7469 6f6e 616c  ovide functional
-00000130: 6974 7920 746f 0a61 7574 6f6d 6174 6963  ity to.automatic
-00000140: 616c 6c79 2064 6574 6572 6d69 6e65 2074  ally determine t
-00000150: 6865 2074 6563 746f 6e69 6320 7265 6769  he tectonic regi
-00000160: 6f6e 206f 6620 616e 2065 6172 7468 7175  on of an earthqu
-00000170: 616b 650a 2853 7562 6475 6374 696f 6e2c  ake.(Subduction,
-00000180: 2041 6374 6976 652c 2048 6f74 5370 6f74   Active, HotSpot
-00000190: 2c20 5374 6162 6c65 292c 2061 6e64 2074  , Stable), and t
-000001a0: 6865 2064 6973 7461 6e63 6520 746f 2074  he distance to t
-000001b0: 6865 2074 6563 746f 6e69 630a 7265 6769  he tectonic.regi
-000001c0: 6f6e 7320 746f 2077 6869 6368 2069 7420  ons to which it 
-000001d0: 646f 6573 202a 6e6f 742a 2062 656c 6f6e  does *not* belon
-000001e0: 672e 0a0a 496e 2061 6464 6974 696f 6e2c  g...In addition,
-000001f0: 2053 6569 736d 6f54 6563 746f 6e69 6320   SeismoTectonic 
-00000200: 5265 6769 6d65 2045 6172 7468 7175 616b  Regime Earthquak
-00000210: 6520 4361 6c63 756c 6174 6f72 2028 5354  e Calculator (ST
-00000220: 5245 4329 2070 726f 7669 6465 7320 6120  REC) provides a 
-00000230: 746f 6f6c 2074 6861 742c 200a 696e 2073  tool that, .in s
-00000240: 7562 6475 6374 696f 6e20 7a6f 6e65 732c  ubduction zones,
-00000250: 2072 6574 7572 6e73 2069 6e66 6f72 6d61   returns informa
-00000260: 7469 6f6e 2061 626f 7574 2074 6865 2073  tion about the s
-00000270: 7562 6475 6374 696f 6e20 7a6f 6e65 2c20  ubduction zone, 
-00000280: 7573 696e 6720 7468 6520 0a55 5347 5320  using the .USGS 
-00000290: 536c 6162 3220 6d6f 6465 6c73 2e0a 0a28  Slab2 models...(
-000002a0: 6874 7470 733a 2f2f 7777 772e 7363 6965  https://www.scie
-000002b0: 6e63 6562 6173 652e 676f 762f 6361 7461  ncebase.gov/cata
-000002c0: 6c6f 672f 6974 656d 2f35 6161 3162 3030  log/item/5aa1b00
-000002d0: 6565 3462 3062 3163 3339 3265 3836 3436  ee4b0b1c392e8646
-000002e0: 372f 292e 0a0a 0a54 6869 7320 636f 6465  7/)....This code
-000002f0: 2077 6173 2062 6173 6564 206f 6e20 7468   was based on th
-00000300: 6520 5b70 6170 6572 5d28 6874 7470 733a  e [paper](https:
-00000310: 2f2f 646f 692e 6f72 672f 3130 2e31 3738  //doi.org/10.178
-00000320: 352f 3031 3230 3131 3031 3234 293a 0a0a  5/0120110124):..
-00000330: 6060 600a 4120 476c 6f62 616c 2045 6172  ```.A Global Ear
-00000340: 7468 7175 616b 6520 4469 7363 7269 6d69  thquake Discrimi
-00000350: 6e61 7469 6f6e 2053 6368 656d 6520 746f  nation Scheme to
-00000360: 204f 7074 696d 697a 6520 4772 6f75 6e64   Optimize Ground
-00000370: e280 904d 6f74 696f 6e20 5072 6564 6963  ...Motion Predic
-00000380: 7469 6f6e 2045 7175 6174 696f 6e20 5365  tion Equation Se
-00000390: 6c65 6374 696f 6e0a 442e 2047 6172 63c3  lection.D. Garc.
-000003a0: ad61 3b20 442e 204a 2e20 5761 6c64 3b20  .a; D. J. Wald; 
-000003b0: 4d2e 2047 2e20 4865 6172 6e65 0a42 756c  M. G. Hearne.Bul
-000003c0: 6c65 7469 6e20 6f66 2074 6865 2053 6569  letin of the Sei
-000003d0: 736d 6f6c 6f67 6963 616c 2053 6f63 6965  smological Socie
-000003e0: 7479 206f 6620 416d 6572 6963 6120 2832  ty of America (2
-000003f0: 3031 3229 2031 3032 2028 3129 3a20 3138  012) 102 (1): 18
-00000400: 35e2 8093 3230 332e 0a60 6060 0a0a 0a23  5...203..```...#
-00000410: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
-00000420: 7069 7020 696e 7374 616c 6c20 7573 6773  pip install usgs
-00000430: 2d73 7472 6563 600a 0a23 2055 7067 7261  -strec`..# Upgra
-00000440: 6465 0a0a 6070 6970 2069 6e73 7461 6c6c  de..`pip install
-00000450: 202d 2d75 7067 7261 6465 2075 7367 732d   --upgrade usgs-
-00000460: 7374 7265 6360 0a0a 2320 436f 6e66 6967  strec`..# Config
-00000470: 7572 6174 696f 6e0a 0a49 6e20 6f72 6465  uration..In orde
-00000480: 7220 746f 2075 7365 2053 5452 4543 2079  r to use STREC y
-00000490: 6f75 2077 696c 6c20 6e65 6564 2074 6f3a  ou will need to:
-000004a0: 0a0a 202d 2064 6f77 6e6c 6f61 6420 5553  .. - download US
-000004b0: 4753 2053 6c61 6220 322e 3020 6d6f 6465  GS Slab 2.0 mode
-000004c0: 6c73 2c20 6465 7363 7269 6265 6420 6174  ls, described at
-000004d0: 2074 6865 2053 6369 656e 6365 2042 6173   the Science Bas
-000004e0: 6520 0a20 2020 6c69 6e6b 2061 626f 7665  e .   link above
-000004f0: 2e20 0a20 2d20 6372 6561 7465 2061 2064  . . - create a d
-00000500: 6174 6162 6173 6520 6f66 206d 6f6d 656e  atabase of momen
-00000510: 7420 7465 6e73 6f72 732c 2065 6974 6865  t tensors, eithe
-00000520: 7220 6d61 6e75 616c 6c79 2066 726f 6d20  r manually from 
-00000530: 6120 0a20 2020 7370 7265 6164 7368 6565  a .   spreadshee
-00000540: 742f 4353 5620 6669 6c65 2028 6465 7363  t/CSV file (desc
-00000550: 7269 6265 6420 6265 6c6f 7729 2c20 6f72  ribed below), or
-00000560: 2062 7920 646f 776e 6c6f 6164 696e 6720   by downloading 
-00000570: 0a20 2020 6120 6465 6661 756c 7420 6461  .   a default da
-00000580: 7461 6261 7365 206f 6620 6d6f 6d65 6e74  tabase of moment
-00000590: 2074 656e 736f 7273 2066 726f 6d20 7468   tensors from th
-000005a0: 6520 0a20 2020 5b47 6c6f 6261 6c20 4365  e .   [Global Ce
-000005b0: 6e74 726f 6964 204d 6f6d 656e 7420 5465  ntroid Moment Te
-000005c0: 6e73 6f72 2028 4743 4d54 2920 6361 7461  nsor (GCMT) cata
-000005d0: 6c6f 675d 2868 7474 7073 3a2f 2f77 7777  log](https://www
-000005e0: 2e67 6c6f 6261 6c63 6d74 2e6f 7267 2f29  .globalcmt.org/)
-000005f0: 0a20 2d20 4372 6561 7465 2061 2063 6f6e  . - Create a con
-00000600: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00000610: 6465 7363 7269 6269 6e67 2074 6865 206c  describing the l
-00000620: 6f63 6174 696f 6e73 206f 6620 7468 6573  ocations of thes
-00000630: 6520 6669 6c65 732e 0a0a 546f 206d 616b  e files...To mak
-00000640: 6520 7468 6973 2065 6173 6965 722c 2061  e this easier, a
-00000650: 2063 6f6e 6669 6775 7261 7469 6f6e 2070   configuration p
-00000660: 726f 6772 616e 2063 616c 6c65 6420 6073  rogran called `s
-00000670: 7472 6563 5f63 6667 6020 6973 2070 726f  trec_cfg` is pro
-00000680: 7669 6465 6420 7768 6963 6820 6175 746f  vided which auto
-00000690: 6d61 7465 7320 0a61 6c6c 206f 6620 7468  mates .all of th
-000006a0: 6573 6520 7072 6f63 6573 7365 732e 2054  ese processes. T
-000006b0: 6869 7320 7072 6f67 7261 6d20 636f 6d65  his program come
-000006c0: 7320 7769 7468 2074 776f 202a 7375 622d  s with two *sub-
-000006d0: 636f 6d6d 616e 6473 2a20 6361 6c6c 6564  commands* called
-000006e0: 2060 696e 666f 6020 616e 6420 6075 7064   `info` and `upd
-000006f0: 6174 6560 2e20 0a54 6f20 696e 6974 6961  ate`. .To initia
-00000700: 6c69 7a65 2074 6865 2073 7973 7465 6d20  lize the system 
-00000710: 7769 7468 2074 6865 2053 6c61 6220 322e  with the Slab 2.
-00000720: 3020 6772 6964 7320 616e 6420 4743 4d54  0 grids and GCMT
-00000730: 206d 6f6d 656e 7420 7465 6e73 6f72 2064   moment tensor d
-00000740: 6174 6162 6173 653a 0a0a 6073 7472 6563  atabase:..`strec
-00000750: 5f63 6667 2075 7064 6174 6520 2d2d 6461  _cfg update --da
-00000760: 7461 666f 6c64 6572 203c 7061 7468 2f74  tafolder <path/t
-00000770: 6f2f 6461 7461 2f66 6f6c 6465 723e 202d  o/data/folder> -
-00000780: 2d73 6c61 6220 2d2d 6763 6d74 600a 0a46  -slab --gcmt`..F
-00000790: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-000007a0: 6f75 2073 6574 2074 6865 2053 5452 4543  ou set the STREC
-000007b0: 2064 6174 6120 666f 6c64 6572 2074 6f20   data folder to 
-000007c0: 6265 202a 2f64 6174 612f 7374 7265 632a  be */data/strec*
-000007d0: 3a0a 0a60 7374 7265 635f 6366 6720 7570  :..`strec_cfg up
-000007e0: 6461 7465 202d 2d64 6174 6166 6f6c 6465  date --datafolde
-000007f0: 7220 2f64 6174 612f 7374 7265 6320 2d2d  r /data/strec --
-00000800: 736c 6162 202d 2d67 636d 7460 0a0a 616e  slab --gcmt`..an
-00000810: 6420 7468 656e 2075 7365 2074 6865 2066  d then use the f
-00000820: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000830: 2074 6f20 7365 6520 7468 6520 7265 7375   to see the resu
-00000840: 6c74 696e 6720 636f 6e66 6967 7572 6174  lting configurat
-00000850: 696f 6e3a 0a0a 6073 7472 6563 5f63 6667  ion:..`strec_cfg
-00000860: 2069 6e66 6f60 0a0a 5468 6520 6f75 7470   info`..The outp
-00000870: 7574 2073 686f 756c 6420 6c6f 6f6b 2073  ut should look s
-00000880: 6f6d 6574 6869 6e67 206c 696b 6520 7468  omething like th
-00000890: 6520 666f 6c6c 6f77 696e 673a 0a0a 6060  e following:..``
-000008a0: 600a 436f 6e66 6967 2066 696c 6520 2f68  `.Config file /h
-000008b0: 6f6d 652f 7573 6572 2f2e 7374 7265 632f  ome/user/.strec/
-000008c0: 636f 6e66 6967 2e69 6e69 3a0a 2d2d 2d2d  config.ini:.----
-000008d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000008e0: 2d2d 2d2d 0a5b 4441 5441 5d0a 666f 6c64  ----.[DATA].fold
-000008f0: 6572 203d 202f 6461 7461 2f73 7472 6563  er = /data/strec
-00000900: 0a73 6c61 6266 6f6c 6465 7220 3d20 2f64  .slabfolder = /d
-00000910: 6174 612f 7374 7265 632f 736c 6162 730a  ata/strec/slabs.
-00000920: 6462 6669 6c65 203d 202f 6461 7461 2f73  dbfile = /data/s
-00000930: 7472 6563 2f6d 6f6d 656e 745f 7465 6e73  trec/moment_tens
-00000940: 6f72 732e 6462 0a0a 5b43 4f4e 5354 414e  ors.db..[CONSTAN
-00000950: 5453 5d0a 6d69 6e72 6164 6961 6c5f 6469  TS].minradial_di
-00000960: 7374 6869 7374 203d 2030 2e30 310a 6d61  sthist = 0.01.ma
-00000970: 7872 6164 6961 6c5f 6469 7374 6869 7374  xradial_disthist
-00000980: 203d 2031 2e30 0a6d 696e 7261 6469 616c   = 1.0.minradial
-00000990: 5f64 6973 7463 6f6d 7020 3d20 302e 350a  _distcomp = 0.5.
-000009a0: 6d61 7872 6164 6961 6c5f 6469 7374 636f  maxradial_distco
-000009b0: 6d70 203d 2031 2e30 0a73 7465 705f 6469  mp = 1.0.step_di
-000009c0: 7374 636f 6d70 203d 2030 2e31 0a64 6570  stcomp = 0.1.dep
-000009d0: 7468 5f72 616e 6765 636f 6d70 203d 2031  th_rangecomp = 1
-000009e0: 300a 6d69 6e6e 6f5f 636f 6d70 203d 2033  0.minno_comp = 3
-000009f0: 0a64 6566 6175 6c74 5f73 7a64 6970 203d  .default_szdip =
-00000a00: 2031 370a 6473 7472 696b 655f 696e 7465   17.dstrike_inte
-00000a10: 7266 203d 2033 300a 6464 6970 5f69 6e74  rf = 30.ddip_int
-00000a20: 6572 6620 3d20 3330 0a64 6c61 6d62 6461  erf = 30.dlambda
-00000a30: 203d 2036 300a 6464 6570 7468 5f69 6e74   = 60.ddepth_int
-00000a40: 6572 6620 3d20 3230 0a64 6465 7074 685f  erf = 20.ddepth_
-00000a50: 696e 7472 6120 3d20 3130 0a2d 2d2d 2d2d  intra = 10.-----
-00000a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a70: 2d2d 2d0a 0a4d 6f6d 656e 7420 5465 6e73  ---..Moment Tens
-00000a80: 6f72 2044 6174 6162 6173 6520 282f 6461  or Database (/da
-00000a90: 7461 2f73 7472 6563 2f6d 6f6d 656e 745f  ta/strec/moment_
-00000aa0: 7465 6e73 6f72 732e 6462 2920 636f 6e74  tensors.db) cont
-00000ab0: 6169 6e73 2036 3035 3335 2065 7665 6e74  ains 60535 event
-00000ac0: 7320 6672 6f6d 2031 2073 6f75 7263 6573  s from 1 sources
-00000ad0: 2e0a 0a54 6865 7265 2061 7265 2031 3335  ...There are 135
-00000ae0: 2073 6c61 6220 6772 6964 7320 6672 6f6d   slab grids from
-00000af0: 2032 3720 756e 6971 7565 2073 6c61 6220   27 unique slab 
-00000b00: 6d6f 6465 6c73 206c 6f63 6174 6564 2069  models located i
-00000b10: 6e20 2f64 6174 612f 7374 7265 632f 736c  n /data/strec/sl
-00000b20: 6162 732e 0a60 6060 0a0a 2320 5573 6167  abs..```..# Usag
-00000b30: 650a 0a60 7265 6763 616c 6360 2069 7320  e..`regcalc` is 
-00000b40: 7468 6520 7072 6f67 7261 6d20 7573 6564  the program used
-00000b50: 2074 6f20 6361 6c63 756c 6174 6520 7265   to calculate re
-00000b60: 6769 6f6e 2070 6172 616d 6574 6572 732e  gion parameters.
-00000b70: 0a0a 5468 6520 6465 7461 696c 7320 6f66  ..The details of
-00000b80: 2074 6865 206f 7074 696f 6e73 2061 7265   the options are
-00000b90: 2076 6973 6962 6c65 2062 7920 7275 6e6e   visible by runn
-00000ba0: 696e 6720 6072 6567 6361 6c63 202d 2d68  ing `regcalc --h
-00000bb0: 656c 7060 2e0a 0a54 6865 2074 6872 6565  elp`...The three
-00000bc0: 206d 6f73 7420 6261 7369 6320 7573 6520   most basic use 
-00000bd0: 6361 7365 7320 6172 653a 0a0a 202d 2047  cases are:.. - G
-00000be0: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
-00000bf0: 6f6e 2061 626f 7574 2061 6e20 6576 656e  on about an even
-00000c00: 7420 6279 2043 6f6d 4361 7420 4944 3a20  t by ComCat ID: 
-00000c10: 6072 6567 6361 6c63 202d 6420 7573 3630  `regcalc -d us60
-00000c20: 3030 6964 3074 600a 202d 2047 6574 7469  00id0t`. - Getti
-00000c30: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2061  ng information a
-00000c40: 626f 7574 2061 2028 706f 7373 6962 6c79  bout a (possibly
-00000c50: 2074 6865 6f72 6574 6963 616c 2920 6576   theoretical) ev
-00000c60: 656e 7420 6279 2070 726f 7669 6469 6e67  ent by providing
-00000c70: 2068 7970 6f63 656e 7465 7220 696e 666f   hypocenter info
-00000c80: 726d 6174 696f 6e3a 2060 7265 6763 616c  rmation: `regcal
-00000c90: 6320 2d65 202d 352e 3037 3335 2031 3033  c -e -5.0735 103
-00000ca0: 2e30 3832 3620 3530 2e35 600a 202d 2047  .0826 50.5`. - G
-00000cb0: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
-00000cc0: 6f6e 2061 626f 7574 206d 6f72 6520 7468  on about more th
-00000cd0: 616e 206f 6e65 2065 7665 6e74 2c20 7769  an one event, wi
-00000ce0: 7468 2069 6e70 7574 206c 696b 6520 6265  th input like be
-00000cf0: 6c6f 7720 6173 2045 7863 656c 206f 7220  low as Excel or 
-00000d00: 4353 563a 0a0a 3c74 6162 6c65 3e0a 3c74  CSV:..<table>.<t
-00000d10: 723e 200a 2020 3c74 683e 4c61 7469 7475  r> .  <th>Latitu
-00000d20: 6465 3c2f 7468 3e0a 2020 3c74 683e 4c6f  de</th>.  <th>Lo
-00000d30: 6e67 6974 7564 653c 2f74 683e 0a20 203c  ngitude</th>.  <
-00000d40: 7468 3e44 6570 7468 3c2f 7468 3e0a 3c2f  th>Depth</th>.</
-00000d50: 7472 3e0a 3c74 723e 0a20 203c 7464 3e2d  tr>.<tr>.  <td>-
-00000d60: 352e 3037 343c 2f74 643e 0a20 203c 7464  5.074</td>.  <td
-00000d70: 3e31 3033 2e30 3833 3c2f 7464 3e0a 2020  >103.083</td>.  
-00000d80: 3c74 643e 3530 2e35 3c2f 7464 3e0a 3c2f  <td>50.5</td>.</
-00000d90: 7472 3e0a 3c74 723e 0a20 203c 7464 3e2d  tr>.<tr>.  <td>-
-00000da0: 312e 3030 383c 2f74 643e 0a20 203c 7464  1.008</td>.  <td
-00000db0: 3e39 382e 3634 323c 2f74 643e 0a20 203c  >98.642</td>.  <
-00000dc0: 7464 3e31 372e 363c 2f74 643e 0a3c 2f74  td>17.6</td>.</t
-00000dd0: 723e 0a3c 2f74 6162 6c65 3e0a 0a60 7265  r>.</table>..`re
-00000de0: 6763 616c 6320 2d69 2069 6e70 7574 5f66  gcalc -i input_f
-00000df0: 696c 652e 786c 7378 600a 0a59 6f75 2063  ile.xlsx`..You c
-00000e00: 616e 2061 6464 2061 2043 6f6d 4361 7420  an add a ComCat 
-00000e10: 4944 2063 6f6c 756d 6e20 746f 2074 6869  ID column to thi
-00000e20: 7320 2d20 7468 6520 6e61 6d65 2077 6869  s - the name whi
-00000e30: 6368 2077 696c 6c20 6265 2061 7574 6f6d  ch will be autom
-00000e40: 6174 6963 616c 6c79 2064 6574 6563 7465  atically detecte
-00000e50: 6420 6973 202a 4576 656e 7449 442a 2028  d is *EventID* (
-00000e60: 6361 7365 2064 6f65 7320 6e6f 7420 6d61  case does not ma
-00000e70: 7474 6572 292e 2049 6620 7468 6520 6669  tter). If the fi
-00000e80: 6c65 2068 6173 2061 6e6f 7468 6572 206e  le has another n
-00000e90: 616d 6520 666f 7220 7468 6520 7361 6d65  ame for the same
-00000ea0: 2063 6f6c 756d 6e20 796f 7520 6361 6e20   column you can 
-00000eb0: 7375 7070 6c79 2074 6861 7420 7769 7468  supply that with
-00000ec0: 2074 6865 202d 2d69 642d 636f 6c75 6d6e   the --id-column
-00000ed0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
-00000ee0: 7469 6f6e 3a0a 0a60 7265 6763 616c 6320  tion:..`regcalc 
-00000ef0: 2d69 2069 6e70 7574 5f66 696c 652e 786c  -i input_file.xl
-00000f00: 7378 202d 2d69 642d 636f 6c75 6d6e 2069  sx --id-column i
-00000f10: 6460 0a0a 4966 2074 6865 2066 696c 6520  d`..If the file 
-00000f20: 636f 6e74 6169 6e73 2063 6f6c 756d 6e20  contains column 
-00000f30: 6e61 6d65 7320 666f 7220 6c61 7469 7475  names for latitu
-00000f40: 6465 2c20 6c6f 6e67 6974 7564 6520 616e  de, longitude an
-00000f50: 6420 6465 7074 6820 7468 6174 2064 6f20  d depth that do 
-00000f60: 6e6f 7420 6d61 7463 6820 7468 6520 7265  not match the re
-00000f70: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
-00000f80: 2070 6174 7465 726e 7320 225e 6c61 7422   patterns "^lat"
-00000f90: 2c20 225e 6c6f 6e22 2c20 225e 6465 7022  , "^lon", "^dep"
-00000fa0: 2028 6967 6e6f 7269 6e67 2063 6173 6529   (ignoring case)
-00000fb0: 2074 6865 6e20 796f 7520 6361 6e20 7375   then you can su
-00000fc0: 7070 6c79 2074 686f 7365 2063 6f6c 756d  pply those colum
-00000fd0: 6e20 6e61 6d65 7320 6173 2077 656c 6c20  n names as well 
-00000fe0: 7573 696e 6720 7468 6520 2d2d 6879 706f  using the --hypo
-00000ff0: 2d63 6f6c 756d 6e73 2063 6f6d 6d61 6e64  -columns command
-00001000: 206c 696e 6520 6f70 7469 6f6e 3a0a 0a60   line option:..`
-00001010: 7265 6763 616c 6320 2d69 2069 6e70 7574  regcalc -i input
-00001020: 5f66 696c 652e 786c 7378 202d 2d68 7970  _file.xlsx --hyp
-00001030: 6f2d 636f 6c75 6d6e 7320 4576 656e 744c  o-columns EventL
-00001040: 6174 6974 7564 6520 4576 656e 744c 6f6e  atitude EventLon
-00001050: 6769 7475 6465 2045 7665 6e74 4465 7074  gitude EventDept
-00001060: 6860 0a0a 4966 2061 6e20 696e 7075 7420  h`..If an input 
-00001070: 7370 7265 6164 7368 6565 7420 6861 7320  spreadsheet has 
-00001080: 6d6f 6d65 6e74 2074 656e 736f 7220 636f  moment tensor co
-00001090: 6c75 6d6e 7320 6e61 6d65 6420 4d72 722c  lumns named Mrr,
-000010a0: 204d 7474 2c20 4d70 702c 2065 7463 2e20   Mtt, Mpp, etc. 
-000010b0: 2863 6173 6520 646f 6573 206e 6f74 206d  (case does not m
-000010c0: 6174 7465 7229 2074 6865 6e20 7468 6f73  atter) then thos
-000010d0: 6520 7661 6c75 6573 2077 696c 6c20 6265  e values will be
-000010e0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-000010f0: 7465 2074 6865 204b 6167 616e 2061 6e67  te the Kagan ang
-00001100: 6c65 2061 6e64 2064 6574 6572 6d69 6e65  le and determine
-00001110: 2074 6865 2066 6f63 616c 206d 6563 6861   the focal mecha
-00001120: 6e69 736d 2e0a 0a59 6f75 2063 616e 2061  nism...You can a
-00001130: 6c73 6f20 6f70 7469 6f6e 616c 6c79 2073  lso optionally s
-00001140: 7065 6369 6679 206d 6f6d 656e 7420 7465  pecify moment te
-00001150: 6e73 6f72 2069 6e66 6f72 6d61 7469 6f6e  nsor information
-00001160: 2066 6f72 2061 2073 696e 676c 6520 6576   for a single ev
-00001170: 656e 7420 696e 2074 6865 2066 6f72 6d20  ent in the form 
-00001180: 6f66 2073 7472 696b 652f 6469 702f 7261  of strike/dip/ra
-00001190: 6b65 2061 6e67 6c65 7320 616e 6420 6120  ke angles and a 
-000011a0: 6d61 676e 6974 7564 652c 2075 7369 6e67  magnitude, using
-000011b0: 2074 6865 202d 2d6d 6f6d 656e 742d 696e   the --moment-in
-000011c0: 666f 2063 6f6d 6d61 6e64 206c 696e 6520  fo command line 
-000011d0: 6f70 7469 6f6e 3a0a 0a60 7265 6763 616c  option:..`regcal
-000011e0: 6320 2d65 202d 302e 3935 3020 2d32 312e  c -e -0.950 -21.
-000011f0: 3732 3520 3130 2e30 202d 6d20 3236 3020  725 10.0 -m 260 
-00001200: 3834 2031 3639 2036 2e39 600a 0a2a 4e6f  84 169 6.9`..*No
-00001210: 7465 3a20 5573 6572 7320 6d61 7920 6e6f  te: Users may no
-00001220: 7469 6365 2074 6861 7420 6469 7374 616e  tice that distan
-00001230: 6365 7320 746f 2074 6563 746f 6e69 6320  ces to tectonic 
-00001240: 7265 6769 6f6e 7320 7468 6520 6561 7274  regions the eart
-00001250: 6871 7561 6b65 2069 7320 4e4f 5420 696e  hquake is NOT in
-00001260: 206d 6179 2062 6520 756e 7265 6173 6f6e   may be unreason
-00001270: 6162 6c79 206c 6172 6765 2076 616c 7565  ably large value
-00001280: 732e 2054 6865 2072 6561 736f 6e20 0a66  s. The reason .f
-00001290: 6f72 2072 6574 7572 6e69 6e67 2074 6865  or returning the
-000012a0: 2064 6973 7461 6e63 6573 2074 6f20 6f74   distances to ot
-000012b0: 6865 7220 7265 6769 6f6e 7320 6973 2074  her regions is t
-000012c0: 6f20 6865 6c70 2069 6e66 6f72 6d20 7468  o help inform th
-000012d0: 6520 7573 6572 2077 6865 6e20 7468 6520  e user when the 
-000012e0: 6561 7274 6871 7561 6b65 2069 7320 636c  earthquake is cl
-000012f0: 6f73 6520 746f 2061 6e6f 7468 6572 2072  ose to another r
-00001300: 6567 696f 6e2e 0a57 6865 6e20 5354 5245  egion..When STRE
-00001310: 4320 6f75 7470 7574 7320 7468 6573 6520  C outputs these 
-00001320: 6c61 7267 6520 6e75 6d62 6572 7320 6974  large numbers it
-00001330: 2069 6e64 6963 6174 6573 2074 6861 7420   indicates that 
-00001340: 7468 6520 6469 7374 616e 6365 2074 6f20  the distance to 
-00001350: 7468 6174 206f 7468 6572 2072 6567 696f  that other regio
-00001360: 6e20 6973 206e 6f74 2063 6c6f 7365 2065  n is not close e
-00001370: 6e6f 7567 6820 746f 2061 6666 6563 740a  nough to affect.
-00001380: 7468 6520 7072 6f70 6572 7469 6573 206f  the properties o
-00001390: 6620 7468 6520 6561 7274 6871 7561 6b65  f the earthquake
-000013a0: 2e2a 0a0a 0a23 2047 6c6f 7373 6172 790a  .*...# Glossary.
-000013b0: 0a53 5452 4543 2064 6566 696e 6573 2061  .STREC defines a
-000013c0: 206e 756d 6265 7220 6f66 2074 6572 6d73   number of terms
-000013d0: 2074 6861 7420 6d61 7920 6e6f 7420 6265   that may not be
-000013e0: 2063 6f6d 6d6f 6e6c 790a 756e 6465 7273   commonly.unders
-000013f0: 746f 6f64 2c20 736f 2074 6865 7920 6172  tood, so they ar
-00001400: 6520 6578 706c 6169 6e65 6420 6865 7265  e explained here
-00001410: 2e20 2054 6865 7365 2074 6572 6d73 206d  .  These terms m
-00001420: 6179 2062 6520 6469 6666 6572 656e 740a  ay be different.
-00001430: 6672 6f6d 2074 6865 2047 6172 6369 6120  from the Garcia 
-00001440: 7061 7065 7220 7570 6f6e 2077 6869 6368  paper upon which
-00001450: 2074 6869 7320 736f 6674 7761 7265 2069   this software i
-00001460: 7320 6f72 6967 696e 616c 6c79 2062 6173  s originally bas
-00001470: 6564 2e0a 0a20 2d20 2a54 6563 746f 6e69  ed... - *Tectoni
-00001480: 6320 5265 6769 6f6e 2a3a 204f 6e65 206f  c Region*: One o
-00001490: 6620 5375 6264 7563 7469 6f6e 2c20 4163  f Subduction, Ac
-000014a0: 7469 7665 2c20 486f 7453 706f 742c 206f  tive, HotSpot, o
-000014b0: 7220 5374 6162 6c65 2e0a 2020 2057 6520  r Stable..   We 
-000014c0: 6861 7665 2073 706c 6974 2075 7020 7468  have split up th
-000014d0: 6520 676c 6f62 6520 696e 746f 2074 6865  e globe into the
-000014e0: 7365 2066 6f75 7220 7265 6769 6f6e 732c  se four regions,
-000014f0: 2073 7563 6820 7468 6174 2061 6e79 0a20   such that any. 
-00001500: 2020 706f 696e 7420 6f6e 2074 6865 2067    point on the g
-00001510: 6c6f 6265 2073 686f 756c 6420 6661 6c6c  lobe should fall
-00001520: 2069 6e74 6f20 6f6e 6520 616e 6420 6f6e   into one and on
-00001530: 6c79 206f 6e65 206f 6620 7468 6573 650a  ly one of these.
-00001540: 2020 2072 6567 696f 6e73 2e0a 2020 200a     regions..   .
-00001550: 2020 2020 202a 202a 5375 6264 7563 7469       * *Subducti
-00001560: 6f6e 2a3a 2041 2074 6563 746f 6e69 6320  on*: A tectonic 
-00001570: 7265 6769 6f6e 2064 6566 696e 6564 2062  region defined b
-00001580: 7920 6f6e 6520 706c 6174 6520 6465 7363  y one plate desc
-00001590: 656e 6469 6e67 2062 656c 6f77 0a20 2020  ending below.   
-000015a0: 2020 616e 6f74 6865 7220 2865 2e67 2e2c    another (e.g.,
-000015b0: 2074 6865 2077 6573 7465 726e 2070 6f72   the western por
-000015c0: 7469 6f6e 206f 6620 7468 6520 556e 6974  tion of the Unit
-000015d0: 6564 2053 7461 7465 7329 2c20 6d6f 7265  ed States), more
-000015e0: 2073 7065 6369 6669 6361 6c6c 790a 2020   specifically.  
-000015f0: 2020 2062 7920 7468 6f73 6520 6c6f 6361     by those loca
-00001600: 7469 6f6e 7320 6162 6f76 6520 7468 6520  tions above the 
-00001610: 536c 6162 322e 3020 6772 6964 732e 0a0a  Slab2.0 grids...
-00001620: 2020 2020 202a 202a 4163 7469 7665 2a3a       * *Active*:
-00001630: 2041 2074 6563 746f 6e69 6320 7265 6769   A tectonic regi
-00001640: 6f6e 2077 6869 6368 2065 7870 6572 6965  on which experie
-00001650: 6e63 6573 2063 7275 7374 616c 2064 6566  nces crustal def
-00001660: 6f72 6d61 7469 6f6e 2064 7565 0a20 2020  ormation due.   
-00001670: 2020 746f 2070 6c61 7465 2074 6563 746f    to plate tecto
-00001680: 6e69 6373 2e0a 0a20 2020 2020 2a20 2a48  nics...     * *H
-00001690: 6f74 5370 6f74 2a3a 2041 2074 6563 746f  otSpot*: A tecto
-000016a0: 6e69 6320 7265 6769 6f6e 2077 6869 6368  nic region which
-000016b0: 2069 7320 7369 7474 696e 6720 6162 6f76   is sitting abov
-000016c0: 6520 6d61 6e74 6c65 2070 6c75 6d65 732c  e mantle plumes,
-000016d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000016e0: 2020 2020 7768 6572 6520 6d61 676d 6120      where magma 
-000016f0: 7075 7368 6573 2074 6872 6f75 6768 2063  pushes through c
-00001700: 7261 636b 7320 696e 2074 6865 2063 7275  racks in the cru
-00001710: 7374 2e0a 0a20 2020 2020 2a20 2a53 7461  st...     * *Sta
-00001720: 626c 652a 3a20 5465 6374 6f6e 6963 2072  ble*: Tectonic r
-00001730: 6567 696f 6e73 2077 6869 6368 2075 6e6c  egions which unl
-00001740: 696b 6520 4163 7469 7665 2072 6567 696f  ike Active regio
-00001750: 6e73 2c20 646f 206e 6f74 0a20 2020 2020  ns, do not.     
-00001760: 6578 7065 7269 656e 6365 2063 7275 7374  experience crust
-00001770: 616c 2064 6566 6f72 6d61 7469 6f6e 2028  al deformation (
-00001780: 652e 672e 2c20 7468 6520 696e 7465 7269  e.g., the interi
-00001790: 6f72 206f 6620 7468 650a 2020 2020 2041  or of the.     A
-000017a0: 7573 7472 616c 6961 6e20 636f 6e74 696e  ustralian contin
-000017b0: 656e 742e 290a 0a21 5b4d 6170 2073 686f  ent.)..![Map sho
-000017c0: 7769 6e67 2074 6563 746f 6e69 6320 7265  wing tectonic re
-000017d0: 6769 6f6e 735d 2873 656c 6563 745f 7265  gions](select_re
-000017e0: 6769 6f6e 732e 706e 6720 224d 6170 2053  gions.png "Map S
-000017f0: 686f 7769 6e67 2054 6563 746f 6e69 6320  howing Tectonic 
-00001800: 5265 6769 6f6e 7322 290a 2a46 6967 2031  Regions").*Fig 1
-00001810: 202d 204d 6170 2073 686f 7769 6e67 2074   - Map showing t
-00001820: 6563 746f 6e69 6320 7265 6769 6f6e 732e  ectonic regions.
-00001830: 2041 4352 3d41 6374 6976 6520 4372 7573   ACR=Active Crus
-00001840: 7461 6c20 5265 6769 6f6e 2c20 5355 423d  tal Region, SUB=
-00001850: 5375 6264 7563 7469 6f6e 205a 6f6e 652c  Subduction Zone,
-00001860: 2056 4f4c 3d48 6f74 5370 6f74 2052 6567   VOL=HotSpot Reg
-00001870: 696f 6e2c 2053 4352 3d53 7461 626c 6520  ion, SCR=Stable 
-00001880: 436f 6e74 696e 656e 7461 6c20 5265 6769  Continental Regi
-00001890: 6f6e 2a20 0a0a 202d 202a 4f63 6561 6e69  on* .. - *Oceani
-000018a0: 632a 3a20 416e 6f74 6865 7220 7265 6769  c*: Another regi
-000018b0: 6f6e 2c20 6e6f 7420 6578 636c 7573 6976  on, not exclusiv
-000018c0: 6520 7769 7468 2074 6865 2066 6f75 7220  e with the four 
-000018d0: 5465 6374 6f6e 6963 0a20 2020 5265 6769  Tectonic.   Regi
-000018e0: 6f6e 732c 2074 6861 7420 696e 6469 6361  ons, that indica
-000018f0: 7465 7320 7768 6574 6865 7220 7468 6520  tes whether the 
-00001900: 706f 696e 7420 7375 7070 6c69 6564 2069  point supplied i
-00001910: 7320 696e 2074 6865 206f 6365 616e 0a20  s in the ocean. 
-00001920: 2020 2869 2e65 2e2c 206e 6f74 2063 6f6e    (i.e., not con
-00001930: 7469 6e65 6e74 616c 292e 0a0a 202d 202a  tinental)... - *
-00001940: 436f 6e74 696e 656e 7461 6c2a 3a20 5468  Continental*: Th
-00001950: 6520 6f70 706f 7369 7465 206f 6620 4f63  e opposite of Oc
-00001960: 6561 6e69 632e 0a0a 202d 202a 466f 6361  eanic... - *Foca
-00001970: 6c20 4d65 6368 616e 6973 6d2a 3a20 4120  l Mechanism*: A 
-00001980: 7365 7420 6f66 2070 6172 616d 6574 6572  set of parameter
-00001990: 7320 7468 6174 2064 6566 696e 6520 7468  s that define th
-000019a0: 6520 6465 666f 726d 6174 696f 6e20 696e  e deformation in
-000019b0: 0a20 2020 7468 6520 736f 7572 6365 2072  .   the source r
-000019c0: 6567 696f 6e20 7468 6174 2067 656e 6572  egion that gener
-000019d0: 6174 6573 2074 6865 2073 6569 736d 6963  ates the seismic
-000019e0: 2077 6176 6573 206f 6620 616e 2065 6172   waves of an ear
-000019f0: 7468 7175 616b 652e 0a0a 202d 202a 5465  thquake... - *Te
-00001a00: 6e73 6f72 2054 7970 652a 3a20 5468 6520  nsor Type*: The 
-00001a10: 7368 6f72 7420 6e61 6d65 2066 6f72 2074  short name for t
-00001a20: 6865 2061 6c67 6f72 6974 686d 2075 7365  he algorithm use
-00001a30: 6420 746f 2067 656e 6572 6174 650a 2020  d to generate.  
-00001a40: 2074 6865 206d 6f6d 656e 7420 7465 6e73   the moment tens
-00001a50: 6f72 2075 7365 6420 746f 2064 6574 6572  or used to deter
-00001a60: 6d69 6e65 2066 6f63 616c 206d 6563 6861  mine focal mecha
-00001a70: 6e69 736d 2c20 4b61 6761 6e20 616e 676c  nism, Kagan angl
-00001a80: 652c 0a20 2020 6574 632e 2020 5468 6973  e,.   etc.  This
-00001a90: 2069 7320 7573 7561 6c6c 7920 6120 7368   is usually a sh
-00001aa0: 6f72 7420 636f 6465 206c 696b 6520 2a4d  ort code like *M
-00001ab0: 7777 2a20 2857 2d70 6861 7365 292c 202a  ww* (W-phase), *
-00001ac0: 4d77 722a 0a20 2020 2872 6567 696f 6e61  Mwr*.   (regiona
-00001ad0: 6c29 2c20 2a4d 7762 2a20 2862 6f64 7920  l), *Mwb* (body 
-00001ae0: 7761 7665 292c 206f 7220 2a63 6f6d 706f  wave), or *compo
-00001af0: 7369 7465 2a2c 2077 6869 6368 2069 6e64  site*, which ind
-00001b00: 6963 6174 6573 2074 6861 740a 2020 2074  icates that.   t
-00001b10: 6865 7265 2069 7320 6e6f 2063 6f6d 7075  here is no compu
-00001b20: 7465 6420 6d6f 6d65 6e74 2074 656e 736f  ted moment tenso
-00001b30: 722c 2073 6f20 6120 636f 6d70 6f73 6974  r, so a composit
-00001b40: 6520 6f66 2068 6973 746f 7269 6361 6c0a  e of historical.
-00001b50: 2020 206d 6f6d 656e 7420 7465 6e73 6f72     moment tensor
-00001b60: 7320 6172 6f75 6e64 2074 6865 2069 6e70  s around the inp
-00001b70: 7574 2063 6f6f 7264 696e 6174 6573 2069  ut coordinates i
-00001b80: 7320 7573 6564 2069 6e73 7465 6164 2e0a  s used instead..
-00001b90: 0a20 2d20 2a54 656e 736f 7220 536f 7572  . - *Tensor Sour
-00001ba0: 6365 2a3a 2057 6865 6e20 6176 6169 6c61  ce*: When availa
-00001bb0: 626c 652c 2074 6869 7320 6973 2075 7375  ble, this is usu
-00001bc0: 616c 6c79 2074 6865 206e 6574 776f 726b  ally the network
-00001bd0: 2074 6861 740a 2020 2063 6f6e 7472 6962   that.   contrib
-00001be0: 7574 6564 2074 6865 206d 6f6d 656e 7420  uted the moment 
-00001bf0: 7465 6e73 6f72 2c20 666f 6c6c 6f77 6564  tensor, followed
-00001c00: 2062 7920 7468 6520 4944 2075 7365 6420   by the ID used 
-00001c10: 6279 2074 6861 740a 2020 206e 6574 776f  by that.   netwo
-00001c20: 726b 2028 652e 672e 2c20 7573 5f32 3030  rk (e.g., us_200
-00001c30: 3062 6d63 6729 2e0a 0a20 2d20 2a4b 6167  0bmcg)... - *Kag
-00001c40: 616e 2041 6e67 6c65 2a3a 2041 6e20 7369  an Angle*: An si
-00001c50: 6e67 6c65 2061 6e67 6c65 2062 6574 7765  ngle angle betwe
-00001c60: 656e 2061 6e79 2074 776f 206d 6f6d 656e  en any two momen
-00001c70: 7420 7465 6e73 6f72 7320 6f72 2069 6e0a  t tensors or in.
-00001c80: 2020 2020 6f75 7220 6361 7365 2c20 6265      our case, be
-00001c90: 7477 6565 6e20 6120 6d6f 6d65 6e74 2074  tween a moment t
-00001ca0: 656e 736f 7220 616e 6420 6120 7375 6264  ensor and a subd
-00001cb0: 7563 7469 6e67 2073 6c61 622e 0a0a 202d  ucting slab... -
-00001cc0: 202a 436f 6d70 6f73 6974 6520 4d6f 6d65   *Composite Mome
-00001cd0: 6e74 2054 656e 736f 722a 3a20 5768 656e  nt Tensor*: When
-00001ce0: 206d 6f6d 656e 7420 7465 6e73 6f72 7320   moment tensors 
-00001cf0: 6172 6520 6e6f 7420 6176 6169 6c61 626c  are not availabl
-00001d00: 6520 0a20 2020 2066 6f72 2061 2067 6976  e .    for a giv
-00001d10: 656e 2065 7665 6e74 2c20 6120 636f 6d70  en event, a comp
-00001d20: 6f73 6974 6520 6d6f 6d65 6e74 2074 656e  osite moment ten
-00001d30: 736f 7220 6973 2063 616c 6375 6c61 7465  sor is calculate
-00001d40: 6420 6279 200a 2020 2020 6573 7365 6e74  d by .    essent
-00001d50: 6961 6c6c 7920 7461 6b69 6e67 2074 6865  ially taking the
-00001d60: 206d 6561 6e20 6f66 2061 7420 6c65 6173   mean of at leas
-00001d70: 7420 7468 7265 6520 6d6f 6d65 6e74 2074  t three moment t
-00001d80: 656e 736f 7273 2069 6e20 6120 302e 3120  ensors in a 0.1 
-00001d90: 0a20 2020 2064 6567 7265 6520 626f 7820  .    degree box 
-00001da0: 7375 7272 6f75 6e64 696e 6720 7468 6520  surrounding the 
-00001db0: 6561 7274 6871 7561 6b65 2068 7970 6f63  earthquake hypoc
-00001dc0: 656e 7465 722e 0a0a 202d 202a 436f 6d70  enter... - *Comp
-00001dd0: 6f73 6974 6520 5661 7269 6162 696c 6974  osite Variabilit
-00001de0: 792a 3a20 5768 656e 2074 6865 206d 6f6d  y*: When the mom
-00001df0: 656e 7420 7465 6e73 6f72 2073 6f6c 7574  ent tensor solut
-00001e00: 696f 6e20 6973 206f 6620 7479 7065 0a20  ion is of type. 
-00001e10: 2a63 6f6d 706f 7369 7465 2a2c 2061 2073  *composite*, a s
-00001e20: 6361 6c61 7220 7661 6c75 6520 6465 7363  calar value desc
-00001e30: 7269 6269 6e67 2074 6865 2076 6172 6961  ribing the varia
-00001e40: 6269 6c69 7479 206f 6620 7468 6520 6d6f  bility of the mo
-00001e50: 6d65 6e74 0a20 7465 6e73 6f72 7320 7573  ment. tensors us
-00001e60: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
-00001e70: 7468 6520 636f 6d70 6f73 6974 652e 0a0a  the composite...
-00001e80: 202d 202a 4469 7374 616e 6365 2074 6f20   - *Distance to 
-00001e90: 5b52 6567 696f 6e5d 2a3a 2054 6865 2067  [Region]*: The g
-00001ea0: 7265 6174 2063 6972 636c 6520 6469 7374  reat circle dist
-00001eb0: 616e 6365 2066 726f 6d20 7468 6520 696e  ance from the in
-00001ec0: 7075 740a 2020 2063 6f6f 7264 696e 6174  put.   coordinat
-00001ed0: 6573 2074 6f20 7468 6520 6e65 6172 6573  es to the neares
-00001ee0: 7420 7665 7274 6578 206f 6620 5b52 6567  t vertex of [Reg
-00001ef0: 696f 6e5d 2070 6f6c 7967 6f6e 2e0a 0a20  ion] polygon... 
-00001f00: 2d20 2a53 6c61 6220 4d6f 6465 6c20 5265  - *Slab Model Re
-00001f10: 6769 6f6e 2a3a 2057 6520 6375 7272 656e  gion*: We curren
-00001f20: 746c 7920 7573 6520 536c 6162 2032 2e30  tly use Slab 2.0
-00001f30: 2073 7562 6475 6374 696f 6e20 6d6f 6465   subduction mode
-00001f40: 6c73 0a20 2020 2848 6179 6573 2032 3031  ls.   (Hayes 201
-00001f50: 3229 2c20 7768 6963 6820 6172 6520 6375  2), which are cu
-00001f60: 7272 656e 746c 7920 7072 6f76 6964 6564  rrently provided
-00001f70: 2066 6f72 2032 3720 7265 6769 6f6e 7320   for 27 regions 
-00001f80: 6172 6f75 6e64 0a20 2020 7468 6520 676c  around.   the gl
-00001f90: 6f62 652e 2020 5468 6573 6520 7265 6769  obe.  These regi
-00001fa0: 6f6e 7320 6172 6520 6465 7363 7269 6265  ons are describe
-00001fb0: 6420 696e 2064 6574 6169 6c20 6865 7265  d in detail here
-00001fc0: 3a0a 2020 2068 7474 7073 3a2f 2f77 7777  :.   https://www
-00001fd0: 2e73 6369 656e 6365 6261 7365 2e67 6f76  .sciencebase.gov
-00001fe0: 2f63 6174 616c 6f67 2f69 7465 6d2f 3561  /catalog/item/5a
-00001ff0: 6131 6230 3065 6534 6230 6231 6333 3932  a1b00ee4b0b1c392
-00002000: 6538 3634 3637 2f0a 0a20 2d20 2a53 6c61  e86467/.. - *Sla
-00002010: 6220 4d6f 6465 6c20 4465 7074 682a 3a20  b Model Depth*: 
-00002020: 5468 6520 6265 7374 2065 7374 696d 6174  The best estimat
-00002030: 6520 6f66 2064 6570 7468 2074 6f20 7375  e of depth to su
-00002040: 6264 7563 7469 6f6e 0a20 2020 696e 7465  bduction.   inte
-00002050: 7266 6163 652e 0a0a 202d 202a 536c 6162  rface... - *Slab
-00002060: 204d 6f64 656c 2044 6570 7468 2055 6e63   Model Depth Unc
-00002070: 6572 7461 696e 7479 2a3a 2054 6865 2062  ertainty*: The b
-00002080: 6573 7420 6573 7469 6d61 7465 206f 6620  est estimate of 
-00002090: 7468 6520 756e 6365 7274 6169 6e74 790a  the uncertainty.
-000020a0: 2020 206f 6620 7468 6520 6465 7074 6820     of the depth 
-000020b0: 746f 2073 7562 6475 6374 696f 6e20 696e  to subduction in
-000020c0: 7465 7266 6163 652e 0a0a 202d 202a 536c  terface... - *Sl
-000020d0: 6162 204d 6f64 656c 2044 6970 2a3a 2054  ab Model Dip*: T
-000020e0: 6865 2062 6573 7420 6573 7469 6d61 7465  he best estimate
-000020f0: 206f 6620 7468 6520 6469 7020 616e 676c   of the dip angl
-00002100: 6520 6f66 2074 6865 0a20 2020 7375 6264  e of the.   subd
-00002110: 7563 7469 6e67 2070 6c61 7465 2e0a 0a20  ucting plate... 
-00002120: 2d20 2a53 6c61 6220 4d6f 6465 6c20 5374  - *Slab Model St
-00002130: 7269 6b65 2a3a 2054 6865 2062 6573 7420  rike*: The best 
-00002140: 6573 7469 6d61 7465 206f 6620 7468 6520  estimate of the 
-00002150: 7374 7269 6b65 2061 6e67 6c65 206f 6620  strike angle of 
-00002160: 7468 650a 2020 2073 7562 6475 6374 696e  the.   subductin
-00002170: 6720 706c 6174 652e 0a0a                 g plate...
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7573 6773  : 2.1.Name: usgs
+00000020: 2d73 7472 6563 0a56 6572 7369 6f6e 3a20  -strec.Version: 
+00000030: 322e 322e 360a 5375 6d6d 6172 793a 2055  2.2.6.Summary: U
+00000040: 5347 5320 5365 6973 6d6f 5465 6374 6f6e  SGS SeismoTecton
+00000050: 6963 2052 6567 696d 6520 4561 7274 6871  ic Regime Earthq
+00000060: 7561 6b65 2043 616c 6375 6c61 746f 7220  uake Calculator 
+00000070: 2853 5452 4543 290a 4175 7468 6f72 2d65  (STREC).Author-e
+00000080: 6d61 696c 3a20 4d69 6b65 2048 6561 726e  mail: Mike Hearn
+00000090: 6520 3c6d 6865 6172 6e65 4075 7367 732e  e <mhearne@usgs.
+000000a0: 676f 763e 2c20 4572 6963 2054 686f 6d70  gov>, Eric Thomp
+000000b0: 736f 6e20 3c65 7468 6f6d 7073 6f6e 4075  son <ethompson@u
+000000c0: 7367 732e 676f 763e 0a4c 6963 656e 7365  sgs.gov>.License
+000000d0: 3a20 4c69 6365 6e73 650a 2020 2020 2020  : License.      
+000000e0: 2020 3d3d 3d3d 3d3d 3d0a 2020 2020 2020    =======.      
+000000f0: 2020 0a20 2020 2020 2020 2055 6e6c 6573    .        Unles
+00000100: 7320 6f74 6865 7277 6973 6520 6e6f 7465  s otherwise note
+00000110: 642c 2054 6869 7320 7072 6f6a 6563 7420  d, This project 
+00000120: 6973 2069 6e20 7468 6520 7075 626c 6963  is in the public
+00000130: 2064 6f6d 6169 6e20 696e 2074 6865 2055   domain in the U
+00000140: 6e69 7465 640a 2020 2020 2020 2020 5374  nited.        St
+00000150: 6174 6573 2062 6563 6175 7365 2069 7420  ates because it 
+00000160: 636f 6e74 6169 6e73 206d 6174 6572 6961  contains materia
+00000170: 6c73 2074 6861 7420 6f72 6967 696e 616c  ls that original
+00000180: 6c79 2063 616d 6520 6672 6f6d 2074 6865  ly came from the
+00000190: 2055 6e69 7465 640a 2020 2020 2020 2020   United.        
+000001a0: 5374 6174 6573 2047 656f 6c6f 6769 6361  States Geologica
+000001b0: 6c20 5375 7276 6579 2c20 616e 2061 6765  l Survey, an age
+000001c0: 6e63 7920 6f66 2074 6865 2055 6e69 7465  ncy of the Unite
+000001d0: 6420 5374 6174 6573 2044 6570 6172 746d  d States Departm
+000001e0: 656e 7420 6f66 0a20 2020 2020 2020 2049  ent of.        I
+000001f0: 6e74 6572 696f 722e 2046 6f72 206d 6f72  nterior. For mor
+00000200: 6520 696e 666f 726d 6174 696f 6e2c 2073  e information, s
+00000210: 6565 2074 6865 206f 6666 6963 6961 6c20  ee the official 
+00000220: 5553 4753 2063 6f70 7972 6967 6874 2070  USGS copyright p
+00000230: 6f6c 6963 7920 6174 0a20 2020 2020 2020  olicy at.       
+00000240: 2068 7474 7073 3a2f 2f77 7777 322e 7573   https://www2.us
+00000250: 6773 2e67 6f76 2f76 6973 7561 6c2d 6964  gs.gov/visual-id
+00000260: 2f63 7265 6469 745f 7573 6773 2e68 746d  /credit_usgs.htm
+00000270: 6c23 636f 7079 7269 6768 740a 2020 2020  l#copyright.    
+00000280: 2020 2020 0a20 2020 2020 2020 2054 6869      .        Thi
+00000290: 7320 696e 666f 726d 6174 696f 6e20 6973  s information is
+000002a0: 2070 7265 6c69 6d69 6e61 7279 206f 7220   preliminary or 
+000002b0: 7072 6f76 6973 696f 6e61 6c20 616e 6420  provisional and 
+000002c0: 6973 2073 7562 6a65 6374 2074 6f0a 2020  is subject to.  
+000002d0: 2020 2020 2020 7265 7669 7369 6f6e 2e20        revision. 
+000002e0: 4974 2069 7320 6265 696e 6720 7072 6f76  It is being prov
+000002f0: 6964 6564 2074 6f20 6d65 6574 2074 6865  ided to meet the
+00000300: 206e 6565 6420 666f 7220 7469 6d65 6c79   need for timely
+00000310: 2062 6573 740a 2020 2020 2020 2020 7363   best.        sc
+00000320: 6965 6e63 652e 2054 6865 2069 6e66 6f72  ience. The infor
+00000330: 6d61 7469 6f6e 2068 6173 206e 6f74 2072  mation has not r
+00000340: 6563 6569 7665 6420 6669 6e61 6c20 6170  eceived final ap
+00000350: 7072 6f76 616c 2062 7920 7468 6520 5553  proval by the US
+00000360: 4753 0a20 2020 2020 2020 2061 6e64 2069  GS.        and i
+00000370: 7320 7072 6f76 6964 6564 206f 6e20 7468  s provided on th
+00000380: 6520 636f 6e64 6974 696f 6e20 7468 6174  e condition that
+00000390: 206e 6569 7468 6572 2074 6865 2055 5347   neither the USG
+000003a0: 5320 6e6f 7220 7468 650a 2020 2020 2020  S nor the.      
+000003b0: 2020 552e 532e 2047 6f76 6572 6e6d 656e    U.S. Governmen
+000003c0: 7420 7368 616c 6c20 6265 2068 656c 6420  t shall be held 
+000003d0: 6c69 6162 6c65 2066 6f72 2061 6e79 2064  liable for any d
+000003e0: 616d 6167 6573 2072 6573 756c 7469 6e67  amages resulting
+000003f0: 2066 726f 6d0a 2020 2020 2020 2020 7468   from.        th
+00000400: 6520 6175 7468 6f72 697a 6564 206f 7220  e authorized or 
+00000410: 756e 6175 7468 6f72 697a 6564 2075 7365  unauthorized use
+00000420: 206f 6620 7468 6520 696e 666f 726d 6174   of the informat
+00000430: 696f 6e2e 0a20 2020 2020 2020 200a 4b65  ion..        .Ke
+00000440: 7977 6f72 6473 3a20 636f 6d63 6174 2c65  ywords: comcat,e
+00000450: 6172 7468 7175 616b 650a 5265 7175 6972  arthquake.Requir
+00000460: 6573 2d50 7974 686f 6e3a 203c 3d33 2e31  es-Python: <=3.1
+00000470: 310a 4465 7363 7269 7074 696f 6e2d 436f  1.Description-Co
+00000480: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000490: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
+000004a0: 6573 2d45 7874 7261 3a20 6465 760a 5072  es-Extra: dev.Pr
+000004b0: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
+000004c0: 7374 0a4c 6963 656e 7365 2d46 696c 653a  st.License-File:
+000004d0: 204c 4943 454e 5345 2e6d 640a 0a23 2054   LICENSE.md..# T
+000004e0: 6162 6c65 206f 6620 436f 6e74 656e 7473  able of Contents
+000004f0: 0a2d 205b 5461 626c 6520 6f66 2043 6f6e  .- [Table of Con
+00000500: 7465 6e74 735d 2823 7461 626c 652d 6f66  tents](#table-of
+00000510: 2d63 6f6e 7465 6e74 7329 0a2d 205b 496e  -contents).- [In
+00000520: 7472 6f64 7563 7469 6f6e 5d28 2369 6e74  troduction](#int
+00000530: 726f 6475 6374 696f 6e29 0a2d 205b 496e  roduction).- [In
+00000540: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
+00000550: 7461 6c6c 6174 696f 6e29 0a2d 205b 5570  tallation).- [Up
+00000560: 6772 6164 655d 2823 7570 6772 6164 6529  grade](#upgrade)
+00000570: 0a2d 205b 436f 6e66 6967 7572 6174 696f  .- [Configuratio
+00000580: 6e5d 2823 636f 6e66 6967 7572 6174 696f  n](#configuratio
+00000590: 6e29 0a2d 205b 5573 6167 655d 2823 7573  n).- [Usage](#us
+000005a0: 6167 6529 0a2d 205b 5072 6f62 6162 696c  age).- [Probabil
+000005b0: 6974 6965 735d 2028 2370 726f 6261 6269  ities] (#probabi
+000005c0: 6c69 7469 6573 290a 2d20 5b47 6c6f 7373  lities).- [Gloss
+000005d0: 6172 795d 2823 676c 6f73 7361 7279 290a  ary](#glossary).
+000005e0: 0a23 2049 6e74 726f 6475 6374 696f 6e0a  .# Introduction.
+000005f0: 0a54 6869 7320 6c69 6272 6172 7920 616e  .This library an
+00000600: 6420 7365 7420 6f66 2074 6f6f 6c73 2077  d set of tools w
+00000610: 6173 2063 7265 6174 6564 2074 6f20 7072  as created to pr
+00000620: 6f76 6964 6520 6675 6e63 7469 6f6e 616c  ovide functional
+00000630: 6974 7920 746f 0a61 7574 6f6d 6174 6963  ity to.automatic
+00000640: 616c 6c79 2064 6574 6572 6d69 6e65 2074  ally determine t
+00000650: 6865 2074 6563 746f 6e69 6320 7265 6769  he tectonic regi
+00000660: 6f6e 206f 6620 616e 2065 6172 7468 7175  on of an earthqu
+00000670: 616b 650a 2853 7562 6475 6374 696f 6e2c  ake.(Subduction,
+00000680: 2041 6374 6976 652c 2048 6f74 5370 6f74   Active, HotSpot
+00000690: 2c20 5374 6162 6c65 292c 2061 6e64 2074  , Stable), and t
+000006a0: 6865 2064 6973 7461 6e63 6520 746f 2074  he distance to t
+000006b0: 6865 2074 6563 746f 6e69 630a 7265 6769  he tectonic.regi
+000006c0: 6f6e 7320 746f 2077 6869 6368 2069 7420  ons to which it 
+000006d0: 646f 6573 202a 6e6f 742a 2062 656c 6f6e  does *not* belon
+000006e0: 672e 0a0a 496e 2061 6464 6974 696f 6e2c  g...In addition,
+000006f0: 2053 6569 736d 6f54 6563 746f 6e69 6320   SeismoTectonic 
+00000700: 5265 6769 6d65 2045 6172 7468 7175 616b  Regime Earthquak
+00000710: 6520 4361 6c63 756c 6174 6f72 2028 5354  e Calculator (ST
+00000720: 5245 4329 2070 726f 7669 6465 7320 6120  REC) provides a 
+00000730: 746f 6f6c 2074 6861 742c 200a 696e 2073  tool that, .in s
+00000740: 7562 6475 6374 696f 6e20 7a6f 6e65 732c  ubduction zones,
+00000750: 2072 6574 7572 6e73 2069 6e66 6f72 6d61   returns informa
+00000760: 7469 6f6e 2061 626f 7574 2074 6865 2073  tion about the s
+00000770: 7562 6475 6374 696f 6e20 7a6f 6e65 2c20  ubduction zone, 
+00000780: 7573 696e 6720 7468 6520 0a55 5347 5320  using the .USGS 
+00000790: 536c 6162 3220 6d6f 6465 6c73 2e0a 0a28  Slab2 models...(
+000007a0: 6874 7470 733a 2f2f 7777 772e 7363 6965  https://www.scie
+000007b0: 6e63 6562 6173 652e 676f 762f 6361 7461  ncebase.gov/cata
+000007c0: 6c6f 672f 6974 656d 2f35 6161 3162 3030  log/item/5aa1b00
+000007d0: 6565 3462 3062 3163 3339 3265 3836 3436  ee4b0b1c392e8646
+000007e0: 372f 292e 0a0a 0a54 6869 7320 636f 6465  7/)....This code
+000007f0: 2077 6173 2062 6173 6564 206f 6e20 7468   was based on th
+00000800: 6520 5b70 6170 6572 5d28 6874 7470 733a  e [paper](https:
+00000810: 2f2f 646f 692e 6f72 672f 3130 2e31 3738  //doi.org/10.178
+00000820: 352f 3031 3230 3131 3031 3234 293a 0a0a  5/0120110124):..
+00000830: 6060 600a 4120 476c 6f62 616c 2045 6172  ```.A Global Ear
+00000840: 7468 7175 616b 6520 4469 7363 7269 6d69  thquake Discrimi
+00000850: 6e61 7469 6f6e 2053 6368 656d 6520 746f  nation Scheme to
+00000860: 204f 7074 696d 697a 6520 4772 6f75 6e64   Optimize Ground
+00000870: e280 904d 6f74 696f 6e20 5072 6564 6963  ...Motion Predic
+00000880: 7469 6f6e 2045 7175 6174 696f 6e20 5365  tion Equation Se
+00000890: 6c65 6374 696f 6e0a 442e 2047 6172 63c3  lection.D. Garc.
+000008a0: ad61 3b20 442e 204a 2e20 5761 6c64 3b20  .a; D. J. Wald; 
+000008b0: 4d2e 2047 2e20 4865 6172 6e65 0a42 756c  M. G. Hearne.Bul
+000008c0: 6c65 7469 6e20 6f66 2074 6865 2053 6569  letin of the Sei
+000008d0: 736d 6f6c 6f67 6963 616c 2053 6f63 6965  smological Socie
+000008e0: 7479 206f 6620 416d 6572 6963 6120 2832  ty of America (2
+000008f0: 3031 3229 2031 3032 2028 3129 3a20 3138  012) 102 (1): 18
+00000900: 35e2 8093 3230 332e 0a60 6060 0a0a 0a23  5...203..```...#
+00000910: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
+00000920: 7069 7020 696e 7374 616c 6c20 7573 6773  pip install usgs
+00000930: 2d73 7472 6563 600a 0a23 2055 7067 7261  -strec`..# Upgra
+00000940: 6465 0a0a 6070 6970 2069 6e73 7461 6c6c  de..`pip install
+00000950: 202d 2d75 7067 7261 6465 2075 7367 732d   --upgrade usgs-
+00000960: 7374 7265 6360 0a0a 2320 436f 6e66 6967  strec`..# Config
+00000970: 7572 6174 696f 6e0a 0a49 6e20 6f72 6465  uration..In orde
+00000980: 7220 746f 2075 7365 2053 5452 4543 2079  r to use STREC y
+00000990: 6f75 2077 696c 6c20 6e65 6564 2074 6f3a  ou will need to:
+000009a0: 0a0a 202d 2064 6f77 6e6c 6f61 6420 5553  .. - download US
+000009b0: 4753 2053 6c61 6220 322e 3020 6d6f 6465  GS Slab 2.0 mode
+000009c0: 6c73 2c20 6465 7363 7269 6265 6420 6174  ls, described at
+000009d0: 2074 6865 2053 6369 656e 6365 2042 6173   the Science Bas
+000009e0: 6520 0a20 2020 6c69 6e6b 2061 626f 7665  e .   link above
+000009f0: 2e20 0a20 2d20 6372 6561 7465 2061 2064  . . - create a d
+00000a00: 6174 6162 6173 6520 6f66 206d 6f6d 656e  atabase of momen
+00000a10: 7420 7465 6e73 6f72 732c 2065 6974 6865  t tensors, eithe
+00000a20: 7220 6d61 6e75 616c 6c79 2066 726f 6d20  r manually from 
+00000a30: 6120 0a20 2020 7370 7265 6164 7368 6565  a .   spreadshee
+00000a40: 742f 4353 5620 6669 6c65 2028 6465 7363  t/CSV file (desc
+00000a50: 7269 6265 6420 6265 6c6f 7729 2c20 6f72  ribed below), or
+00000a60: 2062 7920 646f 776e 6c6f 6164 696e 6720   by downloading 
+00000a70: 0a20 2020 6120 6465 6661 756c 7420 6461  .   a default da
+00000a80: 7461 6261 7365 206f 6620 6d6f 6d65 6e74  tabase of moment
+00000a90: 2074 656e 736f 7273 2066 726f 6d20 7468   tensors from th
+00000aa0: 6520 0a20 2020 5b47 6c6f 6261 6c20 4365  e .   [Global Ce
+00000ab0: 6e74 726f 6964 204d 6f6d 656e 7420 5465  ntroid Moment Te
+00000ac0: 6e73 6f72 2028 4743 4d54 2920 6361 7461  nsor (GCMT) cata
+00000ad0: 6c6f 675d 2868 7474 7073 3a2f 2f77 7777  log](https://www
+00000ae0: 2e67 6c6f 6261 6c63 6d74 2e6f 7267 2f29  .globalcmt.org/)
+00000af0: 0a20 2d20 4372 6561 7465 2061 2063 6f6e  . - Create a con
+00000b00: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+00000b10: 6465 7363 7269 6269 6e67 2074 6865 206c  describing the l
+00000b20: 6f63 6174 696f 6e73 206f 6620 7468 6573  ocations of thes
+00000b30: 6520 6669 6c65 732e 0a0a 546f 206d 616b  e files...To mak
+00000b40: 6520 7468 6973 2065 6173 6965 722c 2061  e this easier, a
+00000b50: 2063 6f6e 6669 6775 7261 7469 6f6e 2070   configuration p
+00000b60: 726f 6772 616e 2063 616c 6c65 6420 6073  rogran called `s
+00000b70: 7472 6563 5f63 6667 6020 6973 2070 726f  trec_cfg` is pro
+00000b80: 7669 6465 6420 7768 6963 6820 6175 746f  vided which auto
+00000b90: 6d61 7465 7320 0a61 6c6c 206f 6620 7468  mates .all of th
+00000ba0: 6573 6520 7072 6f63 6573 7365 732e 2054  ese processes. T
+00000bb0: 6869 7320 7072 6f67 7261 6d20 636f 6d65  his program come
+00000bc0: 7320 7769 7468 2074 776f 202a 7375 622d  s with two *sub-
+00000bd0: 636f 6d6d 616e 6473 2a20 6361 6c6c 6564  commands* called
+00000be0: 2060 696e 666f 6020 616e 6420 6075 7064   `info` and `upd
+00000bf0: 6174 6560 2e20 0a54 6f20 696e 6974 6961  ate`. .To initia
+00000c00: 6c69 7a65 2074 6865 2073 7973 7465 6d20  lize the system 
+00000c10: 7769 7468 2074 6865 2053 6c61 6220 322e  with the Slab 2.
+00000c20: 3020 6772 6964 7320 616e 6420 4743 4d54  0 grids and GCMT
+00000c30: 206d 6f6d 656e 7420 7465 6e73 6f72 2064   moment tensor d
+00000c40: 6174 6162 6173 653a 0a0a 6073 7472 6563  atabase:..`strec
+00000c50: 5f63 6667 2075 7064 6174 6520 2d2d 6461  _cfg update --da
+00000c60: 7461 666f 6c64 6572 203c 7061 7468 2f74  tafolder <path/t
+00000c70: 6f2f 6461 7461 2f66 6f6c 6465 723e 202d  o/data/folder> -
+00000c80: 2d73 6c61 6220 2d2d 6763 6d74 600a 0a46  -slab --gcmt`..F
+00000c90: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
+00000ca0: 6f75 2073 6574 2074 6865 2053 5452 4543  ou set the STREC
+00000cb0: 2064 6174 6120 666f 6c64 6572 2074 6f20   data folder to 
+00000cc0: 6265 202a 2f64 6174 612f 7374 7265 632a  be */data/strec*
+00000cd0: 3a0a 0a60 7374 7265 635f 6366 6720 7570  :..`strec_cfg up
+00000ce0: 6461 7465 202d 2d64 6174 6166 6f6c 6465  date --datafolde
+00000cf0: 7220 2f64 6174 612f 7374 7265 6320 2d2d  r /data/strec --
+00000d00: 736c 6162 202d 2d67 636d 7460 0a0a 616e  slab --gcmt`..an
+00000d10: 6420 7468 656e 2075 7365 2074 6865 2066  d then use the f
+00000d20: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000d30: 2074 6f20 7365 6520 7468 6520 7265 7375   to see the resu
+00000d40: 6c74 696e 6720 636f 6e66 6967 7572 6174  lting configurat
+00000d50: 696f 6e3a 0a0a 6073 7472 6563 5f63 6667  ion:..`strec_cfg
+00000d60: 2069 6e66 6f60 0a0a 5468 6520 6f75 7470   info`..The outp
+00000d70: 7574 2073 686f 756c 6420 6c6f 6f6b 2073  ut should look s
+00000d80: 6f6d 6574 6869 6e67 206c 696b 6520 7468  omething like th
+00000d90: 6520 666f 6c6c 6f77 696e 673a 0a0a 6060  e following:..``
+00000da0: 600a 436f 6e66 6967 2066 696c 6520 2f68  `.Config file /h
+00000db0: 6f6d 652f 7573 6572 2f2e 7374 7265 632f  ome/user/.strec/
+00000dc0: 636f 6e66 6967 2e69 6e69 3a0a 2d2d 2d2d  config.ini:.----
+00000dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000de0: 2d2d 2d2d 0a5b 4441 5441 5d0a 666f 6c64  ----.[DATA].fold
+00000df0: 6572 203d 202f 6461 7461 2f73 7472 6563  er = /data/strec
+00000e00: 0a73 6c61 6266 6f6c 6465 7220 3d20 2f64  .slabfolder = /d
+00000e10: 6174 612f 7374 7265 632f 736c 6162 730a  ata/strec/slabs.
+00000e20: 6462 6669 6c65 203d 202f 6461 7461 2f73  dbfile = /data/s
+00000e30: 7472 6563 2f6d 6f6d 656e 745f 7465 6e73  trec/moment_tens
+00000e40: 6f72 732e 6462 0a0a 5b43 4f4e 5354 414e  ors.db..[CONSTAN
+00000e50: 5453 5d0a 6d69 6e72 6164 6961 6c5f 6469  TS].minradial_di
+00000e60: 7374 6869 7374 203d 2030 2e30 310a 6d61  sthist = 0.01.ma
+00000e70: 7872 6164 6961 6c5f 6469 7374 6869 7374  xradial_disthist
+00000e80: 203d 2031 2e30 0a6d 696e 7261 6469 616c   = 1.0.minradial
+00000e90: 5f64 6973 7463 6f6d 7020 3d20 302e 350a  _distcomp = 0.5.
+00000ea0: 6d61 7872 6164 6961 6c5f 6469 7374 636f  maxradial_distco
+00000eb0: 6d70 203d 2031 2e30 0a73 7465 705f 6469  mp = 1.0.step_di
+00000ec0: 7374 636f 6d70 203d 2030 2e31 0a64 6570  stcomp = 0.1.dep
+00000ed0: 7468 5f72 616e 6765 636f 6d70 203d 2031  th_rangecomp = 1
+00000ee0: 300a 6d69 6e6e 6f5f 636f 6d70 203d 2033  0.minno_comp = 3
+00000ef0: 0a64 6566 6175 6c74 5f73 7a64 6970 203d  .default_szdip =
+00000f00: 2031 370a 6473 7472 696b 655f 696e 7465   17.dstrike_inte
+00000f10: 7266 203d 2033 300a 6464 6970 5f69 6e74  rf = 30.ddip_int
+00000f20: 6572 6620 3d20 3330 0a64 6c61 6d62 6461  erf = 30.dlambda
+00000f30: 203d 2036 300a 6464 6570 7468 5f69 6e74   = 60.ddepth_int
+00000f40: 6572 6620 3d20 3230 0a64 6465 7074 685f  erf = 20.ddepth_
+00000f50: 696e 7472 6120 3d20 3130 0a2d 2d2d 2d2d  intra = 10.-----
+00000f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000f70: 2d2d 2d0a 0a4d 6f6d 656e 7420 5465 6e73  ---..Moment Tens
+00000f80: 6f72 2044 6174 6162 6173 6520 282f 6461  or Database (/da
+00000f90: 7461 2f73 7472 6563 2f6d 6f6d 656e 745f  ta/strec/moment_
+00000fa0: 7465 6e73 6f72 732e 6462 2920 636f 6e74  tensors.db) cont
+00000fb0: 6169 6e73 2036 3035 3335 2065 7665 6e74  ains 60535 event
+00000fc0: 7320 6672 6f6d 2031 2073 6f75 7263 6573  s from 1 sources
+00000fd0: 2e0a 0a54 6865 7265 2061 7265 2031 3335  ...There are 135
+00000fe0: 2073 6c61 6220 6772 6964 7320 6672 6f6d   slab grids from
+00000ff0: 2032 3720 756e 6971 7565 2073 6c61 6220   27 unique slab 
+00001000: 6d6f 6465 6c73 206c 6f63 6174 6564 2069  models located i
+00001010: 6e20 2f64 6174 612f 7374 7265 632f 736c  n /data/strec/sl
+00001020: 6162 732e 0a60 6060 0a0a 2320 5573 6167  abs..```..# Usag
+00001030: 650a 0a60 7265 6763 616c 6360 2069 7320  e..`regcalc` is 
+00001040: 7468 6520 7072 6f67 7261 6d20 7573 6564  the program used
+00001050: 2074 6f20 6361 6c63 756c 6174 6520 7265   to calculate re
+00001060: 6769 6f6e 2070 6172 616d 6574 6572 732e  gion parameters.
+00001070: 0a0a 5468 6520 6465 7461 696c 7320 6f66  ..The details of
+00001080: 2074 6865 206f 7074 696f 6e73 2061 7265   the options are
+00001090: 2076 6973 6962 6c65 2062 7920 7275 6e6e   visible by runn
+000010a0: 696e 6720 6072 6567 6361 6c63 202d 2d68  ing `regcalc --h
+000010b0: 656c 7060 2e0a 0a54 6865 2074 6872 6565  elp`...The three
+000010c0: 206d 6f73 7420 6261 7369 6320 7573 6520   most basic use 
+000010d0: 6361 7365 7320 6172 653a 0a0a 202d 2047  cases are:.. - G
+000010e0: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
+000010f0: 6f6e 2061 626f 7574 2061 6e20 6576 656e  on about an even
+00001100: 7420 6279 2043 6f6d 4361 7420 4944 3a20  t by ComCat ID: 
+00001110: 6072 6567 6361 6c63 202d 6420 7573 3630  `regcalc -d us60
+00001120: 3030 6964 3074 600a 202d 2047 6574 7469  00id0t`. - Getti
+00001130: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2061  ng information a
+00001140: 626f 7574 2061 2028 706f 7373 6962 6c79  bout a (possibly
+00001150: 2074 6865 6f72 6574 6963 616c 2920 6576   theoretical) ev
+00001160: 656e 7420 6279 2070 726f 7669 6469 6e67  ent by providing
+00001170: 2068 7970 6f63 656e 7465 7220 696e 666f   hypocenter info
+00001180: 726d 6174 696f 6e3a 2060 7265 6763 616c  rmation: `regcal
+00001190: 6320 2d65 202d 352e 3037 3335 2031 3033  c -e -5.0735 103
+000011a0: 2e30 3832 3620 3530 2e35 600a 202d 2047  .0826 50.5`. - G
+000011b0: 6574 7469 6e67 2069 6e66 6f72 6d61 7469  etting informati
+000011c0: 6f6e 2061 626f 7574 206d 6f72 6520 7468  on about more th
+000011d0: 616e 206f 6e65 2065 7665 6e74 2c20 7769  an one event, wi
+000011e0: 7468 2069 6e70 7574 206c 696b 6520 6265  th input like be
+000011f0: 6c6f 7720 6173 2045 7863 656c 206f 7220  low as Excel or 
+00001200: 4353 563a 0a0a 3c74 6162 6c65 3e0a 3c74  CSV:..<table>.<t
+00001210: 723e 200a 2020 3c74 683e 4c61 7469 7475  r> .  <th>Latitu
+00001220: 6465 3c2f 7468 3e0a 2020 3c74 683e 4c6f  de</th>.  <th>Lo
+00001230: 6e67 6974 7564 653c 2f74 683e 0a20 203c  ngitude</th>.  <
+00001240: 7468 3e44 6570 7468 3c2f 7468 3e0a 3c2f  th>Depth</th>.</
+00001250: 7472 3e0a 3c74 723e 0a20 203c 7464 3e2d  tr>.<tr>.  <td>-
+00001260: 352e 3037 343c 2f74 643e 0a20 203c 7464  5.074</td>.  <td
+00001270: 3e31 3033 2e30 3833 3c2f 7464 3e0a 2020  >103.083</td>.  
+00001280: 3c74 643e 3530 2e35 3c2f 7464 3e0a 3c2f  <td>50.5</td>.</
+00001290: 7472 3e0a 3c74 723e 0a20 203c 7464 3e2d  tr>.<tr>.  <td>-
+000012a0: 312e 3030 383c 2f74 643e 0a20 203c 7464  1.008</td>.  <td
+000012b0: 3e39 382e 3634 323c 2f74 643e 0a20 203c  >98.642</td>.  <
+000012c0: 7464 3e31 372e 363c 2f74 643e 0a3c 2f74  td>17.6</td>.</t
+000012d0: 723e 0a3c 2f74 6162 6c65 3e0a 0a60 7265  r>.</table>..`re
+000012e0: 6763 616c 6320 2d69 2069 6e70 7574 5f66  gcalc -i input_f
+000012f0: 696c 652e 786c 7378 600a 0a59 6f75 2063  ile.xlsx`..You c
+00001300: 616e 2061 6464 2061 2043 6f6d 4361 7420  an add a ComCat 
+00001310: 4944 2063 6f6c 756d 6e20 746f 2074 6869  ID column to thi
+00001320: 7320 2d20 7468 6520 6e61 6d65 2077 6869  s - the name whi
+00001330: 6368 2077 696c 6c20 6265 2061 7574 6f6d  ch will be autom
+00001340: 6174 6963 616c 6c79 2064 6574 6563 7465  atically detecte
+00001350: 6420 6973 202a 4576 656e 7449 442a 2028  d is *EventID* (
+00001360: 6361 7365 2064 6f65 7320 6e6f 7420 6d61  case does not ma
+00001370: 7474 6572 292e 2049 6620 7468 6520 6669  tter). If the fi
+00001380: 6c65 2068 6173 2061 6e6f 7468 6572 206e  le has another n
+00001390: 616d 6520 666f 7220 7468 6520 7361 6d65  ame for the same
+000013a0: 2063 6f6c 756d 6e20 796f 7520 6361 6e20   column you can 
+000013b0: 7375 7070 6c79 2074 6861 7420 7769 7468  supply that with
+000013c0: 2074 6865 202d 2d69 642d 636f 6c75 6d6e   the --id-column
+000013d0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
+000013e0: 7469 6f6e 3a0a 0a60 7265 6763 616c 6320  tion:..`regcalc 
+000013f0: 2d69 2069 6e70 7574 5f66 696c 652e 786c  -i input_file.xl
+00001400: 7378 202d 2d69 642d 636f 6c75 6d6e 2069  sx --id-column i
+00001410: 6460 0a0a 4966 2074 6865 2066 696c 6520  d`..If the file 
+00001420: 636f 6e74 6169 6e73 2063 6f6c 756d 6e20  contains column 
+00001430: 6e61 6d65 7320 666f 7220 6c61 7469 7475  names for latitu
+00001440: 6465 2c20 6c6f 6e67 6974 7564 6520 616e  de, longitude an
+00001450: 6420 6465 7074 6820 7468 6174 2064 6f20  d depth that do 
+00001460: 6e6f 7420 6d61 7463 6820 7468 6520 7265  not match the re
+00001470: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00001480: 2070 6174 7465 726e 7320 225e 6c61 7422   patterns "^lat"
+00001490: 2c20 225e 6c6f 6e22 2c20 225e 6465 7022  , "^lon", "^dep"
+000014a0: 2028 6967 6e6f 7269 6e67 2063 6173 6529   (ignoring case)
+000014b0: 2074 6865 6e20 796f 7520 6361 6e20 7375   then you can su
+000014c0: 7070 6c79 2074 686f 7365 2063 6f6c 756d  pply those colum
+000014d0: 6e20 6e61 6d65 7320 6173 2077 656c 6c20  n names as well 
+000014e0: 7573 696e 6720 7468 6520 2d2d 6879 706f  using the --hypo
+000014f0: 2d63 6f6c 756d 6e73 2063 6f6d 6d61 6e64  -columns command
+00001500: 206c 696e 6520 6f70 7469 6f6e 3a0a 0a60   line option:..`
+00001510: 7265 6763 616c 6320 2d69 2069 6e70 7574  regcalc -i input
+00001520: 5f66 696c 652e 786c 7378 202d 2d68 7970  _file.xlsx --hyp
+00001530: 6f2d 636f 6c75 6d6e 7320 4576 656e 744c  o-columns EventL
+00001540: 6174 6974 7564 6520 4576 656e 744c 6f6e  atitude EventLon
+00001550: 6769 7475 6465 2045 7665 6e74 4465 7074  gitude EventDept
+00001560: 6860 0a0a 4966 2061 6e20 696e 7075 7420  h`..If an input 
+00001570: 7370 7265 6164 7368 6565 7420 6861 7320  spreadsheet has 
+00001580: 6d6f 6d65 6e74 2074 656e 736f 7220 636f  moment tensor co
+00001590: 6c75 6d6e 7320 6e61 6d65 6420 4d72 722c  lumns named Mrr,
+000015a0: 204d 7474 2c20 4d70 702c 2065 7463 2e20   Mtt, Mpp, etc. 
+000015b0: 2863 6173 6520 646f 6573 206e 6f74 206d  (case does not m
+000015c0: 6174 7465 7229 2074 6865 6e20 7468 6f73  atter) then thos
+000015d0: 6520 7661 6c75 6573 2077 696c 6c20 6265  e values will be
+000015e0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+000015f0: 7465 2074 6865 204b 6167 616e 2061 6e67  te the Kagan ang
+00001600: 6c65 2061 6e64 2064 6574 6572 6d69 6e65  le and determine
+00001610: 2074 6865 2066 6f63 616c 206d 6563 6861   the focal mecha
+00001620: 6e69 736d 2e0a 0a59 6f75 2063 616e 2061  nism...You can a
+00001630: 6c73 6f20 6f70 7469 6f6e 616c 6c79 2073  lso optionally s
+00001640: 7065 6369 6679 206d 6f6d 656e 7420 7465  pecify moment te
+00001650: 6e73 6f72 2069 6e66 6f72 6d61 7469 6f6e  nsor information
+00001660: 2066 6f72 2061 2073 696e 676c 6520 6576   for a single ev
+00001670: 656e 7420 696e 2074 6865 2066 6f72 6d20  ent in the form 
+00001680: 6f66 2073 7472 696b 652f 6469 702f 7261  of strike/dip/ra
+00001690: 6b65 2061 6e67 6c65 7320 616e 6420 6120  ke angles and a 
+000016a0: 6d61 676e 6974 7564 652c 2075 7369 6e67  magnitude, using
+000016b0: 2074 6865 202d 2d6d 6f6d 656e 742d 696e   the --moment-in
+000016c0: 666f 2063 6f6d 6d61 6e64 206c 696e 6520  fo command line 
+000016d0: 6f70 7469 6f6e 3a0a 0a60 7265 6763 616c  option:..`regcal
+000016e0: 6320 2d65 202d 302e 3935 3020 2d32 312e  c -e -0.950 -21.
+000016f0: 3732 3520 3130 2e30 202d 6d20 3236 3020  725 10.0 -m 260 
+00001700: 3834 2031 3639 2036 2e39 600a 0a2a 4e6f  84 169 6.9`..*No
+00001710: 7465 3a20 5573 6572 7320 6d61 7920 6e6f  te: Users may no
+00001720: 7469 6365 2074 6861 7420 6469 7374 616e  tice that distan
+00001730: 6365 7320 746f 2074 6563 746f 6e69 6320  ces to tectonic 
+00001740: 7265 6769 6f6e 7320 7468 6520 6561 7274  regions the eart
+00001750: 6871 7561 6b65 2069 7320 4e4f 5420 696e  hquake is NOT in
+00001760: 206d 6179 2062 6520 756e 7265 6173 6f6e   may be unreason
+00001770: 6162 6c79 206c 6172 6765 2076 616c 7565  ably large value
+00001780: 732e 2054 6865 2072 6561 736f 6e20 0a66  s. The reason .f
+00001790: 6f72 2072 6574 7572 6e69 6e67 2074 6865  or returning the
+000017a0: 2064 6973 7461 6e63 6573 2074 6f20 6f74   distances to ot
+000017b0: 6865 7220 7265 6769 6f6e 7320 6973 2074  her regions is t
+000017c0: 6f20 6865 6c70 2069 6e66 6f72 6d20 7468  o help inform th
+000017d0: 6520 7573 6572 2077 6865 6e20 7468 6520  e user when the 
+000017e0: 6561 7274 6871 7561 6b65 2069 7320 636c  earthquake is cl
+000017f0: 6f73 6520 746f 2061 6e6f 7468 6572 2072  ose to another r
+00001800: 6567 696f 6e2e 0a57 6865 6e20 5354 5245  egion..When STRE
+00001810: 4320 6f75 7470 7574 7320 7468 6573 6520  C outputs these 
+00001820: 6c61 7267 6520 6e75 6d62 6572 7320 6974  large numbers it
+00001830: 2069 6e64 6963 6174 6573 2074 6861 7420   indicates that 
+00001840: 7468 6520 6469 7374 616e 6365 2074 6f20  the distance to 
+00001850: 7468 6174 206f 7468 6572 2072 6567 696f  that other regio
+00001860: 6e20 6973 206e 6f74 2063 6c6f 7365 2065  n is not close e
+00001870: 6e6f 7567 6820 746f 2061 6666 6563 740a  nough to affect.
+00001880: 7468 6520 7072 6f70 6572 7469 6573 206f  the properties o
+00001890: 6620 7468 6520 6561 7274 6871 7561 6b65  f the earthquake
+000018a0: 2e2a 0a0a 2320 5072 6f62 6162 696c 6974  .*..# Probabilit
+000018b0: 6965 730a 0a53 5452 4543 206e 6f77 2063  ies..STREC now c
+000018c0: 616c 6375 6c61 7465 7320 7468 6520 7072  alculates the pr
+000018d0: 6f62 6162 696c 6974 6965 7320 6f66 2061  obabilities of a
+000018e0: 6e20 6561 7274 6871 7561 6b65 2062 6569  n earthquake bei
+000018f0: 6e67 2069 6e20 616e 7920 6f66 2074 6865  ng in any of the
+00001900: 2074 6563 746f 6e69 6320 7265 6769 6f6e   tectonic region
+00001910: 732c 2061 6e64 2061 6c73 6f20 696e 0a61  s, and also in.a
+00001920: 6e79 206f 6620 7468 6520 7661 7269 6f75  ny of the variou
+00001930: 7320 6465 6669 6e65 6420 6465 7074 6820  s defined depth 
+00001940: 6361 7465 676f 7269 6573 2e20 466f 7220  categories. For 
+00001950: 7375 6264 7563 7469 6f6e 2072 6567 696f  subduction regio
+00001960: 6e73 2074 6865 7365 2061 7265 2068 6172  ns these are har
+00001970: 6463 6f64 6564 2061 7320 0a63 7275 7374  dcoded as .crust
+00001980: 616c 2c20 696e 7465 7266 6163 652c 2061  al, interface, a
+00001990: 6e64 2069 6e74 7261 736c 6162 2e20 466f  nd intraslab. Fo
+000019a0: 7220 6f74 6865 7220 7265 6769 6f6e 732c  r other regions,
+000019b0: 2074 6865 202a 6465 6661 756c 742a 2063   the *default* c
+000019c0: 6f6e 6669 6775 7261 7469 6f6e 2069 6e63  onfiguration inc
+000019d0: 6c75 6465 7320 7468 6520 666f 6c6c 6f77  ludes the follow
+000019e0: 696e 673a 0a0a 202d 2061 6372 5f73 6861  ing:.. - acr_sha
+000019f0: 6c6c 6f77 203a 2061 6374 6976 6520 6561  llow : active ea
+00001a00: 7274 6871 7561 6b65 7320 6f63 6375 7272  rthquakes occurr
+00001a10: 696e 6720 6162 6f76 6520 3330 206b 6d0a  ing above 30 km.
+00001a20: 202d 2061 6372 5f64 6565 7020 2d20 6163   - acr_deep - ac
+00001a30: 7469 7665 2065 6172 7468 7175 616b 6573  tive earthquakes
+00001a40: 206f 6363 7572 7269 6e67 2062 656c 6f77   occurring below
+00001a50: 2033 3020 6b6d 0a20 2d20 7363 725f 7368   30 km. - scr_sh
+00001a60: 616c 6c6f 7720 2d20 7374 6162 6c65 2065  allow - stable e
+00001a70: 6172 7468 7175 616b 6573 2061 7420 616e  arthquakes at an
+00001a80: 7920 6465 7074 680a 202d 2076 6f6c 6361  y depth. - volca
+00001a90: 6e69 635f 7368 616c 6c6f 7720 2d20 766f  nic_shallow - vo
+00001aa0: 6c63 616e 6963 2065 6172 7468 7175 616b  lcanic earthquak
+00001ab0: 6573 2061 7420 616e 7920 6465 7074 680a  es at any depth.
+00001ac0: 0a23 2320 5072 6f62 6162 696c 6974 7920  .## Probability 
+00001ad0: 636f 6e66 6967 7572 6174 696f 6e0a 0a55  configuration..U
+00001ae0: 7365 7273 2063 616e 2063 6f6e 6669 6775  sers can configu
+00001af0: 7265 2074 6865 2070 726f 6261 6269 6c69  re the probabili
+00001b00: 7479 2073 6574 7469 6e67 7320 746f 2069  ty settings to i
+00001b10: 6e63 6c75 6465 206d 6f72 6520 6669 6e65  nclude more fine
+00001b20: 6c79 2067 7261 696e 6564 2064 6570 7468  ly grained depth
+00001b30: 207a 6f6e 6573 2066 6f72 2061 6374 6976   zones for activ
+00001b40: 652c 200a 7374 6162 6c65 2c20 616e 6420  e, .stable, and 
+00001b50: 766f 6c63 616e 6963 2072 6567 696f 6e73  volcanic regions
+00001b60: 2e20 5468 6520 6465 6661 756c 7420 636f  . The default co
+00001b70: 6e66 6967 2066 696c 6520 6973 206c 6f63  nfig file is loc
+00001b80: 6174 6564 2069 6e20 7468 6520 5b72 6570  ated in the [rep
+00001b90: 6f73 6974 6f72 795d 200a 2868 7474 7073  ository] .(https
+00001ba0: 3a2f 2f63 6f64 652e 7573 6773 2e67 6f76  ://code.usgs.gov
+00001bb0: 2f67 6873 632f 6573 692f 7374 7265 632f  /ghsc/esi/strec/
+00001bc0: 2d2f 626c 6f62 2f6d 6169 6e2f 7372 632f  -/blob/main/src/
+00001bd0: 7374 7265 632f 6461 7461 2f73 656c 6563  strec/data/selec
+00001be0: 742e 636f 6e66 2920 616e 6420 0a69 6e73  t.conf) and .ins
+00001bf0: 7461 6c6c 6564 2077 6974 6820 7468 6520  talled with the 
+00001c00: 736f 6674 7761 7265 2e20 546f 2063 7573  software. To cus
+00001c10: 746f 6d69 7a65 2074 6865 2070 726f 6261  tomize the proba
+00001c20: 6269 6c69 7479 2064 6570 7468 207a 6f6e  bility depth zon
+00001c30: 6573 2c20 646f 776e 6c6f 6164 2061 2063  es, download a c
+00001c40: 6f70 7920 6f66 2074 6865 2066 696c 6520  opy of the file 
+00001c50: 6672 6f6d 200a 7468 6520 7265 706f 7369  from .the reposi
+00001c60: 746f 7279 2061 6e64 2073 6176 6520 6974  tory and save it
+00001c70: 2069 6e20 7468 6520 5b44 4154 415d 2d3e   in the [DATA]->
+00001c80: 666f 6c64 6572 2069 6e20 7468 6520 636f  folder in the co
+00001c90: 6e66 6967 2e69 6e69 2066 696c 6520 6465  nfig.ini file de
+00001ca0: 7363 7269 6265 6420 6162 6f76 652e 0a0a  scribed above...
+00001cb0: 6060 600a 5b44 4154 415d 0a66 6f6c 6465  ```.[DATA].folde
+00001cc0: 7220 3d20 2f64 6174 612f 7374 7265 630a  r = /data/strec.
+00001cd0: 6060 600a 0a54 6865 2072 656c 6576 616e  ```..The relevan
+00001ce0: 7420 7365 6374 696f 6e20 6f66 2074 6865  t section of the
+00001cf0: 2073 656c 6563 742e 636f 6e66 2066 696c   select.conf fil
+00001d00: 6520 746f 206d 6f64 6966 7920 6c6f 6f6b  e to modify look
+00001d10: 7320 6c69 6b65 2074 6865 2066 6f6c 6c6f  s like the follo
+00001d20: 7769 6e67 3a0a 0a60 6060 0a5b 7465 6374  wing:..```.[tect
+00001d30: 6f6e 6963 5f72 6567 696f 6e73 5d0a 2020  onic_regions].  
+00001d40: 2020 5b5b 6163 725d 5d0a 2020 2020 2020    [[acr]].      
+00001d50: 2020 686f 7269 7a6f 6e74 616c 5f62 7566    horizontal_buf
+00001d60: 6665 7220 3d20 3130 300a 2020 2020 2020  fer = 100.      
+00001d70: 2020 7665 7274 6963 616c 5f62 7566 6665    vertical_buffe
+00001d80: 7220 3d20 350a 2020 2020 2020 2020 6465  r = 5.        de
+00001d90: 7074 685f 6c61 6265 6c73 203d 2073 6861  pth_labels = sha
+00001da0: 6c6c 6f77 2c20 6465 6570 0a20 2020 2020  llow, deep.     
+00001db0: 2020 206d 696e 5f64 6570 7468 203d 202d     min_depth = -
+00001dc0: 496e 662c 2033 300a 2020 2020 2020 2020  Inf, 30.        
+00001dd0: 6d61 785f 6465 7074 6820 3d20 3330 2c20  max_depth = 30, 
+00001de0: 496e 660a 2020 2020 5b5b 7363 725d 5d0a  Inf.    [[scr]].
+00001df0: 2020 2020 2020 2020 686f 7269 7a6f 6e74          horizont
+00001e00: 616c 5f62 7566 6665 7220 3d20 3130 300a  al_buffer = 100.
+00001e10: 2020 2020 2020 2020 7665 7274 6963 616c          vertical
+00001e20: 5f62 7566 6665 7220 3d20 350a 2020 2020  _buffer = 5.    
+00001e30: 2020 2020 6465 7074 685f 6c61 6265 6c73      depth_labels
+00001e40: 203d 2073 6861 6c6c 6f77 0a20 2020 2020   = shallow.     
+00001e50: 2020 206d 696e 5f64 6570 7468 203d 202d     min_depth = -
+00001e60: 496e 660a 2020 2020 2020 2020 6d61 785f  Inf.        max_
+00001e70: 6465 7074 6820 3d20 496e 660a 2020 2020  depth = Inf.    
+00001e80: 5b5b 7375 6264 7563 7469 6f6e 5d5d 0a20  [[subduction]]. 
+00001e90: 2020 2020 2020 2068 6f72 697a 6f6e 7461         horizonta
+00001ea0: 6c5f 6275 6666 6572 203d 2031 3030 0a20  l_buffer = 100. 
+00001eb0: 2020 2020 2020 2076 6572 7469 6361 6c5f         vertical_
+00001ec0: 6275 6666 6572 203d 2035 0a20 2020 2020  buffer = 5.     
+00001ed0: 2020 2064 6570 7468 5f6c 6162 656c 7320     depth_labels 
+00001ee0: 3d20 6372 7573 7461 6c2c 2069 6e74 6572  = crustal, inter
+00001ef0: 6661 6365 2c20 696e 7472 6173 6c61 620a  face, intraslab.
+00001f00: 2020 2020 2020 2020 6d69 6e5f 6465 7074          min_dept
+00001f10: 6820 3d20 2d49 6e66 2c20 3135 2c20 3730  h = -Inf, 15, 70
+00001f20: 0a20 2020 2020 2020 206d 6178 5f64 6570  .        max_dep
+00001f30: 7468 203d 2031 352c 2037 302c 2049 6e66  th = 15, 70, Inf
+00001f40: 0a20 2020 2020 2020 2075 7365 5f73 6c61  .        use_sla
+00001f50: 6220 3d20 5472 7565 0a20 2020 205b 5b76  b = True.    [[v
+00001f60: 6f6c 6361 6e69 635d 5d0a 2020 2020 2020  olcanic]].      
+00001f70: 2020 686f 7269 7a6f 6e74 616c 5f62 7566    horizontal_buf
+00001f80: 6665 7220 3d20 3130 0a20 2020 2020 2020  fer = 10.       
+00001f90: 2076 6572 7469 6361 6c5f 6275 6666 6572   vertical_buffer
+00001fa0: 203d 2035 0a20 2020 2020 2020 2064 6570   = 5.        dep
+00001fb0: 7468 5f6c 6162 656c 7320 3d20 7368 616c  th_labels = shal
+00001fc0: 6c6f 770a 2020 2020 2020 2020 6d69 6e5f  low.        min_
+00001fd0: 6465 7074 6820 3d20 2d49 6e66 0a20 2020  depth = -Inf.   
+00001fe0: 2020 2020 206d 6178 5f64 6570 7468 203d       max_depth =
+00001ff0: 2049 6e66 0a60 6060 0a0a 546f 2061 6464   Inf.```..To add
+00002000: 2061 2022 6465 6570 2220 2831 3020 6b6d   a "deep" (10 km
+00002010: 206f 7220 6465 6570 6572 2920 6361 7465   or deeper) cate
+00002020: 676f 7279 2074 6f20 7468 6520 7363 7220  gory to the scr 
+00002030: 7365 6374 696f 6e2c 2079 6f75 2077 6f75  section, you wou
+00002040: 6c64 206d 6f64 6966 7920 7468 6174 200a  ld modify that .
+00002050: 7365 6374 696f 6e20 746f 206c 6f6f 6b20  section to look 
+00002060: 6c69 6b65 2074 6865 2066 6f6c 6c6f 7769  like the followi
+00002070: 6e67 3a0a 0a60 6060 0a20 2020 205b 5b73  ng:..```.    [[s
+00002080: 6372 5d5d 0a20 2020 2020 2020 2068 6f72  cr]].        hor
+00002090: 697a 6f6e 7461 6c5f 6275 6666 6572 203d  izontal_buffer =
+000020a0: 2031 3030 0a20 2020 2020 2020 2076 6572   100.        ver
+000020b0: 7469 6361 6c5f 6275 6666 6572 203d 2035  tical_buffer = 5
+000020c0: 0a20 2020 2020 2020 2064 6570 7468 5f6c  .        depth_l
+000020d0: 6162 656c 7320 3d20 7368 616c 6c6f 772c  abels = shallow,
+000020e0: 2064 6565 700a 2020 2020 2020 2020 6d69   deep.        mi
+000020f0: 6e5f 6465 7074 6820 3d20 2d49 6e66 2c20  n_depth = -Inf, 
+00002100: 3130 0a20 2020 2020 2020 206d 6178 5f64  10.        max_d
+00002110: 6570 7468 203d 2031 302c 2049 6e66 0a60  epth = 10, Inf.`
+00002120: 6060 0a0a 0a23 2047 6c6f 7373 6172 790a  ``...# Glossary.
+00002130: 0a53 5452 4543 2064 6566 696e 6573 2061  .STREC defines a
+00002140: 206e 756d 6265 7220 6f66 2074 6572 6d73   number of terms
+00002150: 2074 6861 7420 6d61 7920 6e6f 7420 6265   that may not be
+00002160: 2063 6f6d 6d6f 6e6c 790a 756e 6465 7273   commonly.unders
+00002170: 746f 6f64 2c20 736f 2074 6865 7920 6172  tood, so they ar
+00002180: 6520 6578 706c 6169 6e65 6420 6865 7265  e explained here
+00002190: 2e20 2054 6865 7365 2074 6572 6d73 206d  .  These terms m
+000021a0: 6179 2062 6520 6469 6666 6572 656e 740a  ay be different.
+000021b0: 6672 6f6d 2074 6865 2047 6172 6369 6120  from the Garcia 
+000021c0: 7061 7065 7220 7570 6f6e 2077 6869 6368  paper upon which
+000021d0: 2074 6869 7320 736f 6674 7761 7265 2069   this software i
+000021e0: 7320 6f72 6967 696e 616c 6c79 2062 6173  s originally bas
+000021f0: 6564 2e0a 0a20 2d20 2a54 6563 746f 6e69  ed... - *Tectoni
+00002200: 6320 5265 6769 6f6e 2a3a 204f 6e65 206f  c Region*: One o
+00002210: 6620 5375 6264 7563 7469 6f6e 2c20 4163  f Subduction, Ac
+00002220: 7469 7665 2c20 486f 7453 706f 742c 206f  tive, HotSpot, o
+00002230: 7220 5374 6162 6c65 2e0a 2020 2057 6520  r Stable..   We 
+00002240: 6861 7665 2073 706c 6974 2075 7020 7468  have split up th
+00002250: 6520 676c 6f62 6520 696e 746f 2074 6865  e globe into the
+00002260: 7365 2066 6f75 7220 7265 6769 6f6e 732c  se four regions,
+00002270: 2073 7563 6820 7468 6174 2061 6e79 0a20   such that any. 
+00002280: 2020 706f 696e 7420 6f6e 2074 6865 2067    point on the g
+00002290: 6c6f 6265 2073 686f 756c 6420 6661 6c6c  lobe should fall
+000022a0: 2069 6e74 6f20 6f6e 6520 616e 6420 6f6e   into one and on
+000022b0: 6c79 206f 6e65 206f 6620 7468 6573 650a  ly one of these.
+000022c0: 2020 2072 6567 696f 6e73 2e0a 2020 200a     regions..   .
+000022d0: 2020 2020 202a 202a 5375 6264 7563 7469       * *Subducti
+000022e0: 6f6e 2a3a 2041 2074 6563 746f 6e69 6320  on*: A tectonic 
+000022f0: 7265 6769 6f6e 2064 6566 696e 6564 2062  region defined b
+00002300: 7920 6f6e 6520 706c 6174 6520 6465 7363  y one plate desc
+00002310: 656e 6469 6e67 2062 656c 6f77 0a20 2020  ending below.   
+00002320: 2020 616e 6f74 6865 7220 2865 2e67 2e2c    another (e.g.,
+00002330: 2074 6865 2077 6573 7465 726e 2070 6f72   the western por
+00002340: 7469 6f6e 206f 6620 7468 6520 556e 6974  tion of the Unit
+00002350: 6564 2053 7461 7465 7329 2c20 6d6f 7265  ed States), more
+00002360: 2073 7065 6369 6669 6361 6c6c 790a 2020   specifically.  
+00002370: 2020 2062 7920 7468 6f73 6520 6c6f 6361     by those loca
+00002380: 7469 6f6e 7320 6162 6f76 6520 7468 6520  tions above the 
+00002390: 536c 6162 322e 3020 6772 6964 732e 0a0a  Slab2.0 grids...
+000023a0: 2020 2020 202a 202a 4163 7469 7665 2a3a       * *Active*:
+000023b0: 2041 2074 6563 746f 6e69 6320 7265 6769   A tectonic regi
+000023c0: 6f6e 2077 6869 6368 2065 7870 6572 6965  on which experie
+000023d0: 6e63 6573 2063 7275 7374 616c 2064 6566  nces crustal def
+000023e0: 6f72 6d61 7469 6f6e 2064 7565 0a20 2020  ormation due.   
+000023f0: 2020 746f 2070 6c61 7465 2074 6563 746f    to plate tecto
+00002400: 6e69 6373 2e0a 0a20 2020 2020 2a20 2a48  nics...     * *H
+00002410: 6f74 5370 6f74 2a3a 2041 2074 6563 746f  otSpot*: A tecto
+00002420: 6e69 6320 7265 6769 6f6e 2077 6869 6368  nic region which
+00002430: 2069 7320 7369 7474 696e 6720 6162 6f76   is sitting abov
+00002440: 6520 6d61 6e74 6c65 2070 6c75 6d65 732c  e mantle plumes,
+00002450: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002460: 2020 2020 7768 6572 6520 6d61 676d 6120      where magma 
+00002470: 7075 7368 6573 2074 6872 6f75 6768 2063  pushes through c
+00002480: 7261 636b 7320 696e 2074 6865 2063 7275  racks in the cru
+00002490: 7374 2e0a 0a20 2020 2020 2a20 2a53 7461  st...     * *Sta
+000024a0: 626c 652a 3a20 5465 6374 6f6e 6963 2072  ble*: Tectonic r
+000024b0: 6567 696f 6e73 2077 6869 6368 2075 6e6c  egions which unl
+000024c0: 696b 6520 4163 7469 7665 2072 6567 696f  ike Active regio
+000024d0: 6e73 2c20 646f 206e 6f74 0a20 2020 2020  ns, do not.     
+000024e0: 6578 7065 7269 656e 6365 2063 7275 7374  experience crust
+000024f0: 616c 2064 6566 6f72 6d61 7469 6f6e 2028  al deformation (
+00002500: 652e 672e 2c20 7468 6520 696e 7465 7269  e.g., the interi
+00002510: 6f72 206f 6620 7468 650a 2020 2020 2041  or of the.     A
+00002520: 7573 7472 616c 6961 6e20 636f 6e74 696e  ustralian contin
+00002530: 656e 742e 290a 0a21 5b4d 6170 2073 686f  ent.)..![Map sho
+00002540: 7769 6e67 2074 6563 746f 6e69 6320 7265  wing tectonic re
+00002550: 6769 6f6e 735d 2873 656c 6563 745f 7265  gions](select_re
+00002560: 6769 6f6e 732e 706e 6720 224d 6170 2053  gions.png "Map S
+00002570: 686f 7769 6e67 2054 6563 746f 6e69 6320  howing Tectonic 
+00002580: 5265 6769 6f6e 7322 290a 2a46 6967 2031  Regions").*Fig 1
+00002590: 202d 204d 6170 2073 686f 7769 6e67 2074   - Map showing t
+000025a0: 6563 746f 6e69 6320 7265 6769 6f6e 732e  ectonic regions.
+000025b0: 2041 4352 3d41 6374 6976 6520 4372 7573   ACR=Active Crus
+000025c0: 7461 6c20 5265 6769 6f6e 2c20 5355 423d  tal Region, SUB=
+000025d0: 5375 6264 7563 7469 6f6e 205a 6f6e 652c  Subduction Zone,
+000025e0: 2056 4f4c 3d48 6f74 5370 6f74 2052 6567   VOL=HotSpot Reg
+000025f0: 696f 6e2c 2053 4352 3d53 7461 626c 6520  ion, SCR=Stable 
+00002600: 436f 6e74 696e 656e 7461 6c20 5265 6769  Continental Regi
+00002610: 6f6e 2a20 0a0a 202d 202a 4f63 6561 6e69  on* .. - *Oceani
+00002620: 632a 3a20 416e 6f74 6865 7220 7265 6769  c*: Another regi
+00002630: 6f6e 2c20 6e6f 7420 6578 636c 7573 6976  on, not exclusiv
+00002640: 6520 7769 7468 2074 6865 2066 6f75 7220  e with the four 
+00002650: 5465 6374 6f6e 6963 0a20 2020 5265 6769  Tectonic.   Regi
+00002660: 6f6e 732c 2074 6861 7420 696e 6469 6361  ons, that indica
+00002670: 7465 7320 7768 6574 6865 7220 7468 6520  tes whether the 
+00002680: 706f 696e 7420 7375 7070 6c69 6564 2069  point supplied i
+00002690: 7320 696e 2074 6865 206f 6365 616e 0a20  s in the ocean. 
+000026a0: 2020 2869 2e65 2e2c 206e 6f74 2063 6f6e    (i.e., not con
+000026b0: 7469 6e65 6e74 616c 292e 0a0a 202d 202a  tinental)... - *
+000026c0: 436f 6e74 696e 656e 7461 6c2a 3a20 5468  Continental*: Th
+000026d0: 6520 6f70 706f 7369 7465 206f 6620 4f63  e opposite of Oc
+000026e0: 6561 6e69 632e 0a0a 202d 202a 466f 6361  eanic... - *Foca
+000026f0: 6c20 4d65 6368 616e 6973 6d2a 3a20 4120  l Mechanism*: A 
+00002700: 7365 7420 6f66 2070 6172 616d 6574 6572  set of parameter
+00002710: 7320 7468 6174 2064 6566 696e 6520 7468  s that define th
+00002720: 6520 6465 666f 726d 6174 696f 6e20 696e  e deformation in
+00002730: 0a20 2020 7468 6520 736f 7572 6365 2072  .   the source r
+00002740: 6567 696f 6e20 7468 6174 2067 656e 6572  egion that gener
+00002750: 6174 6573 2074 6865 2073 6569 736d 6963  ates the seismic
+00002760: 2077 6176 6573 206f 6620 616e 2065 6172   waves of an ear
+00002770: 7468 7175 616b 652e 0a0a 202d 202a 5465  thquake... - *Te
+00002780: 6e73 6f72 2054 7970 652a 3a20 5468 6520  nsor Type*: The 
+00002790: 7368 6f72 7420 6e61 6d65 2066 6f72 2074  short name for t
+000027a0: 6865 2061 6c67 6f72 6974 686d 2075 7365  he algorithm use
+000027b0: 6420 746f 2067 656e 6572 6174 650a 2020  d to generate.  
+000027c0: 2074 6865 206d 6f6d 656e 7420 7465 6e73   the moment tens
+000027d0: 6f72 2075 7365 6420 746f 2064 6574 6572  or used to deter
+000027e0: 6d69 6e65 2066 6f63 616c 206d 6563 6861  mine focal mecha
+000027f0: 6e69 736d 2c20 4b61 6761 6e20 616e 676c  nism, Kagan angl
+00002800: 652c 0a20 2020 6574 632e 2020 5468 6973  e,.   etc.  This
+00002810: 2069 7320 7573 7561 6c6c 7920 6120 7368   is usually a sh
+00002820: 6f72 7420 636f 6465 206c 696b 6520 2a4d  ort code like *M
+00002830: 7777 2a20 2857 2d70 6861 7365 292c 202a  ww* (W-phase), *
+00002840: 4d77 722a 0a20 2020 2872 6567 696f 6e61  Mwr*.   (regiona
+00002850: 6c29 2c20 2a4d 7762 2a20 2862 6f64 7920  l), *Mwb* (body 
+00002860: 7761 7665 292c 206f 7220 2a63 6f6d 706f  wave), or *compo
+00002870: 7369 7465 2a2c 2077 6869 6368 2069 6e64  site*, which ind
+00002880: 6963 6174 6573 2074 6861 740a 2020 2074  icates that.   t
+00002890: 6865 7265 2069 7320 6e6f 2063 6f6d 7075  here is no compu
+000028a0: 7465 6420 6d6f 6d65 6e74 2074 656e 736f  ted moment tenso
+000028b0: 722c 2073 6f20 6120 636f 6d70 6f73 6974  r, so a composit
+000028c0: 6520 6f66 2068 6973 746f 7269 6361 6c0a  e of historical.
+000028d0: 2020 206d 6f6d 656e 7420 7465 6e73 6f72     moment tensor
+000028e0: 7320 6172 6f75 6e64 2074 6865 2069 6e70  s around the inp
+000028f0: 7574 2063 6f6f 7264 696e 6174 6573 2069  ut coordinates i
+00002900: 7320 7573 6564 2069 6e73 7465 6164 2e0a  s used instead..
+00002910: 0a20 2d20 2a54 656e 736f 7220 536f 7572  . - *Tensor Sour
+00002920: 6365 2a3a 2057 6865 6e20 6176 6169 6c61  ce*: When availa
+00002930: 626c 652c 2074 6869 7320 6973 2075 7375  ble, this is usu
+00002940: 616c 6c79 2074 6865 206e 6574 776f 726b  ally the network
+00002950: 2074 6861 740a 2020 2063 6f6e 7472 6962   that.   contrib
+00002960: 7574 6564 2074 6865 206d 6f6d 656e 7420  uted the moment 
+00002970: 7465 6e73 6f72 2c20 666f 6c6c 6f77 6564  tensor, followed
+00002980: 2062 7920 7468 6520 4944 2075 7365 6420   by the ID used 
+00002990: 6279 2074 6861 740a 2020 206e 6574 776f  by that.   netwo
+000029a0: 726b 2028 652e 672e 2c20 7573 5f32 3030  rk (e.g., us_200
+000029b0: 3062 6d63 6729 2e0a 0a20 2d20 2a4b 6167  0bmcg)... - *Kag
+000029c0: 616e 2041 6e67 6c65 2a3a 2041 6e20 7369  an Angle*: An si
+000029d0: 6e67 6c65 2061 6e67 6c65 2062 6574 7765  ngle angle betwe
+000029e0: 656e 2061 6e79 2074 776f 206d 6f6d 656e  en any two momen
+000029f0: 7420 7465 6e73 6f72 7320 6f72 2069 6e0a  t tensors or in.
+00002a00: 2020 2020 6f75 7220 6361 7365 2c20 6265      our case, be
+00002a10: 7477 6565 6e20 6120 6d6f 6d65 6e74 2074  tween a moment t
+00002a20: 656e 736f 7220 616e 6420 6120 7375 6264  ensor and a subd
+00002a30: 7563 7469 6e67 2073 6c61 622e 0a0a 202d  ucting slab... -
+00002a40: 202a 436f 6d70 6f73 6974 6520 4d6f 6d65   *Composite Mome
+00002a50: 6e74 2054 656e 736f 722a 3a20 5768 656e  nt Tensor*: When
+00002a60: 206d 6f6d 656e 7420 7465 6e73 6f72 7320   moment tensors 
+00002a70: 6172 6520 6e6f 7420 6176 6169 6c61 626c  are not availabl
+00002a80: 6520 0a20 2020 2066 6f72 2061 2067 6976  e .    for a giv
+00002a90: 656e 2065 7665 6e74 2c20 6120 636f 6d70  en event, a comp
+00002aa0: 6f73 6974 6520 6d6f 6d65 6e74 2074 656e  osite moment ten
+00002ab0: 736f 7220 6973 2063 616c 6375 6c61 7465  sor is calculate
+00002ac0: 6420 6279 200a 2020 2020 6573 7365 6e74  d by .    essent
+00002ad0: 6961 6c6c 7920 7461 6b69 6e67 2074 6865  ially taking the
+00002ae0: 206d 6561 6e20 6f66 2061 7420 6c65 6173   mean of at leas
+00002af0: 7420 7468 7265 6520 6d6f 6d65 6e74 2074  t three moment t
+00002b00: 656e 736f 7273 2069 6e20 6120 302e 3120  ensors in a 0.1 
+00002b10: 0a20 2020 2064 6567 7265 6520 626f 7820  .    degree box 
+00002b20: 7375 7272 6f75 6e64 696e 6720 7468 6520  surrounding the 
+00002b30: 6561 7274 6871 7561 6b65 2068 7970 6f63  earthquake hypoc
+00002b40: 656e 7465 722e 0a0a 202d 202a 436f 6d70  enter... - *Comp
+00002b50: 6f73 6974 6520 5661 7269 6162 696c 6974  osite Variabilit
+00002b60: 792a 3a20 5768 656e 2074 6865 206d 6f6d  y*: When the mom
+00002b70: 656e 7420 7465 6e73 6f72 2073 6f6c 7574  ent tensor solut
+00002b80: 696f 6e20 6973 206f 6620 7479 7065 0a20  ion is of type. 
+00002b90: 2a63 6f6d 706f 7369 7465 2a2c 2061 2073  *composite*, a s
+00002ba0: 6361 6c61 7220 7661 6c75 6520 6465 7363  calar value desc
+00002bb0: 7269 6269 6e67 2074 6865 2076 6172 6961  ribing the varia
+00002bc0: 6269 6c69 7479 206f 6620 7468 6520 6d6f  bility of the mo
+00002bd0: 6d65 6e74 0a20 7465 6e73 6f72 7320 7573  ment. tensors us
+00002be0: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
+00002bf0: 7468 6520 636f 6d70 6f73 6974 652e 0a0a  the composite...
+00002c00: 202d 202a 4469 7374 616e 6365 2074 6f20   - *Distance to 
+00002c10: 5b52 6567 696f 6e5d 2a3a 2054 6865 2067  [Region]*: The g
+00002c20: 7265 6174 2063 6972 636c 6520 6469 7374  reat circle dist
+00002c30: 616e 6365 2066 726f 6d20 7468 6520 696e  ance from the in
+00002c40: 7075 740a 2020 2063 6f6f 7264 696e 6174  put.   coordinat
+00002c50: 6573 2074 6f20 7468 6520 6e65 6172 6573  es to the neares
+00002c60: 7420 7665 7274 6578 206f 6620 5b52 6567  t vertex of [Reg
+00002c70: 696f 6e5d 2070 6f6c 7967 6f6e 2e0a 0a20  ion] polygon... 
+00002c80: 2d20 2a53 6c61 6220 4d6f 6465 6c20 5265  - *Slab Model Re
+00002c90: 6769 6f6e 2a3a 2057 6520 6375 7272 656e  gion*: We curren
+00002ca0: 746c 7920 7573 6520 536c 6162 2032 2e30  tly use Slab 2.0
+00002cb0: 2073 7562 6475 6374 696f 6e20 6d6f 6465   subduction mode
+00002cc0: 6c73 0a20 2020 2848 6179 6573 2032 3031  ls.   (Hayes 201
+00002cd0: 3229 2c20 7768 6963 6820 6172 6520 6375  2), which are cu
+00002ce0: 7272 656e 746c 7920 7072 6f76 6964 6564  rrently provided
+00002cf0: 2066 6f72 2032 3720 7265 6769 6f6e 7320   for 27 regions 
+00002d00: 6172 6f75 6e64 0a20 2020 7468 6520 676c  around.   the gl
+00002d10: 6f62 652e 2020 5468 6573 6520 7265 6769  obe.  These regi
+00002d20: 6f6e 7320 6172 6520 6465 7363 7269 6265  ons are describe
+00002d30: 6420 696e 2064 6574 6169 6c20 6865 7265  d in detail here
+00002d40: 3a0a 2020 2068 7474 7073 3a2f 2f77 7777  :.   https://www
+00002d50: 2e73 6369 656e 6365 6261 7365 2e67 6f76  .sciencebase.gov
+00002d60: 2f63 6174 616c 6f67 2f69 7465 6d2f 3561  /catalog/item/5a
+00002d70: 6131 6230 3065 6534 6230 6231 6333 3932  a1b00ee4b0b1c392
+00002d80: 6538 3634 3637 2f0a 0a20 2d20 2a53 6c61  e86467/.. - *Sla
+00002d90: 6220 4d6f 6465 6c20 4465 7074 682a 3a20  b Model Depth*: 
+00002da0: 5468 6520 6265 7374 2065 7374 696d 6174  The best estimat
+00002db0: 6520 6f66 2064 6570 7468 2074 6f20 7375  e of depth to su
+00002dc0: 6264 7563 7469 6f6e 0a20 2020 696e 7465  bduction.   inte
+00002dd0: 7266 6163 652e 0a0a 202d 202a 536c 6162  rface... - *Slab
+00002de0: 204d 6f64 656c 2044 6570 7468 2055 6e63   Model Depth Unc
+00002df0: 6572 7461 696e 7479 2a3a 2054 6865 2062  ertainty*: The b
+00002e00: 6573 7420 6573 7469 6d61 7465 206f 6620  est estimate of 
+00002e10: 7468 6520 756e 6365 7274 6169 6e74 790a  the uncertainty.
+00002e20: 2020 206f 6620 7468 6520 6465 7074 6820     of the depth 
+00002e30: 746f 2073 7562 6475 6374 696f 6e20 696e  to subduction in
+00002e40: 7465 7266 6163 652e 0a0a 202d 202a 536c  terface... - *Sl
+00002e50: 6162 204d 6f64 656c 2044 6970 2a3a 2054  ab Model Dip*: T
+00002e60: 6865 2062 6573 7420 6573 7469 6d61 7465  he best estimate
+00002e70: 206f 6620 7468 6520 6469 7020 616e 676c   of the dip angl
+00002e80: 6520 6f66 2074 6865 0a20 2020 7375 6264  e of the.   subd
+00002e90: 7563 7469 6e67 2070 6c61 7465 2e0a 0a20  ucting plate... 
+00002ea0: 2d20 2a53 6c61 6220 4d6f 6465 6c20 5374  - *Slab Model St
+00002eb0: 7269 6b65 2a3a 2054 6865 2062 6573 7420  rike*: The best 
+00002ec0: 6573 7469 6d61 7465 206f 6620 7468 6520  estimate of the 
+00002ed0: 7374 7269 6b65 2061 6e67 6c65 206f 6620  strike angle of 
+00002ee0: 7468 650a 2020 2073 7562 6475 6374 696e  the.   subductin
+00002ef0: 6720 706c 6174 652e 0a0a                 g plate...
```

### Comparing `usgs-strec-2.2.5/code.json` & `usgs-strec-2.2.6/code.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/install.sh` & `usgs-strec-2.2.6/install.sh`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/pyproject.toml` & `usgs-strec-2.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "usgs-strec"
-version = "2.2.5"
+version = "2.2.6"
 description = "USGS SeismoTectonic Regime Earthquake Calculator (STREC)"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
 ]
 
 license = {file = "LICENSE.md"}
```

### Comparing `usgs-strec-2.2.5/select_regions.png` & `usgs-strec-2.2.6/select_regions.png`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/bin/regcalc.py` & `usgs-strec-2.2.6/src/strec/bin/regcalc.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,40 +20,40 @@
     csv = "csv"
     excel = "excel"
     json = "json"
 
 
 @app.command()
 def main(
-    eqinfo: Tuple[float, float, float] = typer.Option(
-        (None, None, None),
+    eqinfo: Tuple[float, float, float, float] = typer.Option(
+        (None, None, None, None),
         "--eqinfo",
         "-e",
-        help=("Calculate region based on lat, lon, depth of earthquake"),
+        help=("Calculate region based on lat, lon, depth, magnitude of earthquake"),
     ),
     event_id: str = typer.Option(
         None,
         "--event-id",
         "-d",
         help=("Calculate region based on ComCat event id (i.e., us6000iasi)."),
     ),
     input_file: str = typer.Option(
         None,
         "--input-file",
         "-i",
         help="Calculate region for events specified in input file.",
     ),
-    hypo_columns: Tuple[str, str, str] = typer.Option(
-        (None, None, None),
+    hypo_columns: Tuple[str, str, str, str] = typer.Option(
+        (None, None, None, None),
         "--hypo_columns",
         "-c",
         help=(
             (
                 "When used with -i/--input-file, specify the columns "
-                "that should be used for Latitude, Longitude, Depth."
+                "that should be used for Latitude, Longitude, Depth and Magnitude."
             )
         ),
     ),
     id_column: str = typer.Option(
         None,
         "--id-column",
         help=(
@@ -71,19 +71,19 @@
     ),
     output_file: str = typer.Option(
         None,
         "--output-file",
         "-o",
         help="Specify output filename for results (see --format).",
     ),
-    moment_info: Tuple[float, float, float, float] = typer.Option(
-        (None, None, None, None),
+    moment_info: Tuple[float, float, float] = typer.Option(
+        (None, None, None),
         "--moment-info",
         "-m",
-        help="Specify strike, dip, rake and magnitude for single earthquake.",
+        help="Specify strike, dip, rake for single earthquake.",
     ),
     verbose: bool = typer.Option(
         False,
         "--verbose",
         "-v",
         help="Print out more verbose output.",
     ),
@@ -111,25 +111,45 @@
      - DistanceToContinental : Distance in km to nearest continental polygon.
      - SlabModelRegion : Subduction region.
      - SlabModelDepth : Depth of slab2.0 grid at earthquake location.
      - SlabModelDepthUncertainty : Uncertainty of depth to slab.
      - SlabModelDip : Dip of slab at earthquake location.
      - SlabModelStrike : Strike of slab at earthquake location.
      - SlabModelMaximumDepth : Maximum depth of seismogenic zone.
-     - NGACategory: Subduction category, one of ["interface", "slab", "crustal",
-                    "outer rise", "undetermined", "crustal uncertain",
-                    "interface uncertain", "slab uncertain", "outer rise uncertain"]
+     - ProbabilityActive: Probability that event occurred in an active region.
+     - ProbabilityStable: Probability that event occurred in an stable region.
+     - ProbabilityVolcanic: Probability that event occurred in a volcanic region.
+     - ProbabilitySubduction: Probability that event occurred in a subduction region.
+     - ProbabilityCrustal: Probability that event occurred in a subduction
+                           crustal depth zone.
+     - ProbabilityInterface: Probability that event occurred in a subduction
+                             interface depth zone.
+     - ProbabilityIntraslab: Probability that event occurred in a subduction
+                             intraslab depth zone.
+     - ProbabilityActiveShallow: When specified, the probability that event occurred
+                                 in a configurable shallow zone in an active tectonic
+                                 region.
+     - ProbabilityActiveDeep: When specified, the probability that event occurred
+                              in a configurable deep zone in an active tectonic
+                              region.
+     - ProbabilityStableShallow: When specified, the probability that event occurred
+                                 in a configurable shallow zone in a stable tectonic
+                                 region.
+     - ProbabilityVolcanicShallow: When specified, the probability that event occurred
+                                   in a configurable shallow zone in a volcanic tectonic
+                                   region.
 
     where:
         - Active regions are boundaries between two plates that are colliding,
           sliding past each other, or pulling apart.
         - Stable regions are regions where those things are not happening.
         - Subduction regions are those that are above the Slab2.0 grids.
         - HotSpot regions are those that sit above mantle plumes
         - ALL FocalMechanisms that are some combination of the other types
+        -
 
 
     Input files can be CSV or Excel format (regcalc will
     attempt to determine format automatically) and MUST include columns
     beginning with (case insensitive):
 
         Lat - Numeric latitude of input earthquake.
```

### Comparing `usgs-strec-2.2.5/src/strec/bin/strec_cfg.py` & `usgs-strec-2.2.6/src/strec/bin/strec_cfg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/calc.py` & `usgs-strec-2.2.6/src/strec/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def get_input_dataframe(input_file, eqinfo, event_id, hypo_columns, id_column):
     """Create a dataframe of events (possibly only one).
 
     Args:
         input_file (str or None):  Name of input CSV/Excel file or None.
-        eqinfo (tuple or None): Tuple of (lat, lon, depth) or None.
+        eqinfo (tuple or None): Tuple of (lat, lon, depth, magnitude) or None.
         event_id (str or None): ComCat Event ID or None.
         hypo_columns (tuple or None): Tuple of hypocenter column names in input_file or
                                       None.
         id_column (str or None): Name of column in input_file containing ComCat Event
                                  ID or None.
 
     Returns:
@@ -35,30 +35,42 @@
             - Name of latitude column
             - Name of longitude column
             - Name of depth column
     """
     latcol = "lat"
     loncol = "lon"
     depcol = "depth"
+    magcol = "mag"
     idcol = None
     if input_file is not None:
-        df, idcol, latcol, loncol, depcol = read_input_file(
+        df, idcol, latcol, loncol, depcol, magcol = read_input_file(
             input_file, hypo_columns, id_column
         )
     elif eqinfo is not None:
-        lat, lon, depth = eqinfo
-        d = {"lat": [lat], "lon": [lon], "depth": [depth]}
+        lat, lon, depth, mag = eqinfo
+        d = {"lat": [lat], "lon": [lon], "depth": [depth], "mag": [mag]}
         df = pd.DataFrame(d)
     if event_id is not None:
         detail = get_event_details(event_id)
         idcol = "ComCatID"
-        lat, lon, depth = detail["latitude"], detail["longitude"], detail["depth"]
-        d = {"ComCatID": event_id, "lat": [lat], "lon": [lon], "depth": [depth]}
+        lat, lon, depth, mag = (
+            detail["latitude"],
+            detail["longitude"],
+            detail["depth"],
+            detail["magnitude"],
+        )
+        d = {
+            "ComCatID": event_id,
+            "lat": [lat],
+            "lon": [lon],
+            "depth": [depth],
+            "mag": [mag],
+        }
         df = pd.DataFrame(d)
-    return (df, idcol, latcol, loncol, depcol)
+    return (df, idcol, latcol, loncol, depcol, magcol)
 
 
 def get_moment_columns(row):
     """Return focal mechanism/moment tensor parameters from MT components or focal angles.
 
     Args:
         row (pandas Series): Contains moment tensor components (mtt, mpp, etc) OR
@@ -175,16 +187,16 @@
     id_column,
     verbose,
 ):
     """Output full range of seismotectonic information.
 
     Args:
         input_file (str or None):  Name of input CSV/Excel file or None.
-        eqinfo (tuple or None): Tuple of (lat, lon, depth) or None.
-        moment_info (tuple or None): Tuple of (strike, dip, rake, magnitude) or None.
+        eqinfo (tuple or None): Tuple of (lat, lon, depth, magnitude) or None.
+        moment_info (tuple or None): Tuple of (strike, dip, rake) or None.
         event_id (str or None): ComCat Event ID or None.
         hypo_columns (tuple or None): Tuple of hypocenter column names in input_file
                                       or None.
         id_column (str or None): Name of column in input_file containing ComCat
                                  Event ID or None.
         verbose (bool): Turn verbose debugging on/off.
     Returns:
@@ -211,21 +223,21 @@
             - SlabModelType : (grid,trench)
             - SlabModelDepth : Depth to slab interface at epicenter.
             - SlabModelDepthUncertainty : Uncertainty of depth to slab interface.
             - SlabModelDip : Dip of slab at epicenter.
             - SlabModelStrike : Strike of slab at epicenter.
     """
     selector = SubductionSelector(verbose=verbose, prefix=LOGGER)
-    dataframe, idcol, latcol, loncol, depcol = get_input_dataframe(
+    dataframe, idcol, latcol, loncol, depcol, magcol = get_input_dataframe(
         input_file, eqinfo, event_id, hypo_columns, id_column
     )
     tensor_params = None
     if moment_info[0] is not None:
-        strike, dip, rake, mag = moment_info
-        tensor_params = fill_tensor_from_angles(strike, dip, rake, mag)
+        strike, dip, rake = moment_info
+        tensor_params = fill_tensor_from_angles(strike, dip, rake, dataframe[magcol])
     has_tensor = check_moment_row(dataframe.iloc[0]) or tensor_params is not None
     rows = []
     ic = 0
     inc = min(100, np.power(10, np.floor(np.log10(len(dataframe))) - 1))
     for _, row in dataframe.iterrows():
         if ic % inc == 0 and verbose:
             msg = "Getting detailed information for %i of %i events.\n"
@@ -237,19 +249,20 @@
 
         lat = row[latcol]
         lon = row[loncol]
         # for the cases where lon goes from 0-360
         if lon > 180:
             lon -= 360
         depth = row[depcol]
-
+        mag = row[magcol]
         result = selector.getSubductionType(
             lat,
             lon,
             depth,
+            mag,
             eventid=event_id,
             tensor_params=tensor_params,
         )
 
         tensor_params = None
         row = pd.concat([row, result])
         rows.append(row)
```

### Comparing `usgs-strec-2.2.5/src/strec/cmt.py` & `usgs-strec-2.2.6/src/strec/cmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/REGION_GRIDS_README.txt` & `usgs-strec-2.2.6/src/strec/data/REGION_GRIDS_README.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/active.geojson` & `usgs-strec-2.2.6/src/strec/data/active.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/domains.xlsx` & `usgs-strec-2.2.6/src/strec/data/domains.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/land.geojson` & `usgs-strec-2.2.6/src/strec/data/land.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/moment_tensors.db` & `usgs-strec-2.2.6/src/strec/data/moment_tensors.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/ocean.geojson` & `usgs-strec-2.2.6/src/strec/data/ocean.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/stable.geojson` & `usgs-strec-2.2.6/src/strec/data/stable.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/strec.ini` & `usgs-strec-2.2.6/src/strec/data/strec.ini`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/subduction.geojson` & `usgs-strec-2.2.6/src/strec/data/subduction.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/data/volcanic.geojson` & `usgs-strec-2.2.6/src/strec/data/volcanic.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/database.py` & `usgs-strec-2.2.6/src/strec/database.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/distance.py` & `usgs-strec-2.2.6/src/strec/distance.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/gcmt.py` & `usgs-strec-2.2.6/src/strec/gcmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/gmreg.py` & `usgs-strec-2.2.6/src/strec/gmreg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/kagan.py` & `usgs-strec-2.2.6/src/strec/kagan.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/slab.py` & `usgs-strec-2.2.6/src/strec/slab.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/sm_probs.py` & `usgs-strec-2.2.6/src/strec/sm_probs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,30 +65,30 @@
             for key, value in subduction_probs.items():
                 subduction_probs[key] = value * region_probs["subduction"]
 
             # If we are in a subduction zone then we don't want the
             # keys for subduction_0, 1, 2 (which are the generic vertical
             # subduction subtypes that are not informed by the slab model because
             # it isn't available)
-            if "subduction_0" in region_probs:
-                del region_probs["subduction_0"]
-            if "subduction_1" in region_probs:
-                del region_probs["subduction_1"]
-            if "subduction_2" in region_probs:
-                del region_probs["subduction_2"]
+            if "subduction_crustal" in region_probs:
+                del region_probs["subduction_crustal"]
+            if "subduction_interface" in region_probs:
+                del region_probs["subduction_interface"]
+            if "subduction_intraslab" in region_probs:
+                del region_probs["subduction_intraslab"]
 
         else:
             # If we are NOT in a subduction zone we may or may not need subduction
             # probabilities (depending on distance and the configured taper). But
             # either way, we will not have access to the slab model and so we have
             # to use the generic vertical subtypes
             subduction_probs = {
-                "crustal": region_probs["subduction_0"],
-                "interface": region_probs["subduction_1"],
-                "intraslab": region_probs["subduction_2"],
+                "crustal": region_probs["subduction_crustal"],
+                "interface": region_probs["subduction_interface"],
+                "intraslab": region_probs["subduction_intraslab"],
             }
         region_probs.update(subduction_probs)
     else:
         logging.info('"use_slab" is False so no slab used in finding GMPE ' "weights.")
 
     return region_probs
 
@@ -140,29 +140,31 @@
         x2 = rdict["horizontal_buffer"]
 
         region_prob = get_probability(distance, x1, p1, x2, p2)
         region_probs[region] = region_prob
 
         region_layer_probs = {}
         # now do the weights for each depth zone
+        labels = rdict["depth_labels"]
         for i in range(0, len(rdict["min_depth"])):
             # First, taper from -1 to 0 for the lower end
             x1 = rdict["min_depth"][i] - rdict["vertical_buffer"] / 2
             p1 = -1.0
             x2 = rdict["min_depth"][i]
             p2 = 0.0
             p_layer1 = get_probability(depth, x1, p1, x2, p2)
             # Then, taper from 0 to -1 for the higher end
             x1 = rdict["max_depth"][i]
             p1 = 0.0
             x2 = rdict["max_depth"][i] + rdict["vertical_buffer"] / 2
             p2 = -1.0
             p_layer2 = get_probability(depth, x1, p1, x2, p2)
             # Lastly, combine to get probability curve for layer i
-            region_layer_probs["%s_%i" % (region, i)] = 1 + p_layer1 + p_layer2
+            label = labels[i]
+            region_layer_probs["%s_%s" % (region, label)] = 1 + p_layer1 + p_layer2
         probsum = sum([lp for lp in list(region_layer_probs.values())])
         if probsum > 0:
             for key, value in region_layer_probs.items():
                 region_layer_probs[key] = value / probsum
 
         # running list of all region layer probabilities
         layer_probs.update(region_layer_probs)
```

### Comparing `usgs-strec-2.2.5/src/strec/subduction.py` & `usgs-strec-2.2.6/src/strec/subduction.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/src/strec/subtype.py` & `usgs-strec-2.2.6/src/strec/subtype.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 # third party imports
 import numpy as np
 import requests
 from esi_utils_rupture.tensor import fill_tensor_from_components
 
 # local imports
 from strec.cmt import getCompositeCMT
+from strec.config import get_select_config
 from strec.gmreg import Regionalizer
 from strec.kagan import get_kagan_angle
 from strec.slab import SlabCollection
+from strec.sm_probs import get_probs
 from strec.utils import get_config
 
 EVENT_URL = (
     "https://earthquake.usgs.gov/fdsnws/event/1/query?eventid=EVENTID&format=geojson"
 )
 SLAB_RAKE = 90  # presumed rake angle of slabs
 
@@ -61,14 +63,24 @@
     "delplunge_ss": 20,
 }
 
 COMCAT_TEMPLATE = (
     "https://earthquake.usgs.gov/earthquakes/feed/v1.0/detail/[EVENTID].geojson"
 )
 
+PROB_TRANSLATOR = {
+    "acr": "ProbabilityActive",
+    "scr": "ProbabilityStable",
+    "subduction": "ProbabilitySubduction",
+    "volcanic": "ProbabilityVolcanic",
+    "crustal": "ProbabilitySubductionCrustal",
+    "interface": "ProbabilitySubductionInterface",
+    "intraslab": "ProbabilitySubductionIntraslab",
+}
+
 
 def fill_axis(axis, tensor_props):
     axis_dict = {}
     if f"{axis.lower()}-axis-plunge" in tensor_props:
         axis_dict[f"{axis.upper()}"] = {
             "azimuth": float(tensor_props[f"{axis.lower()}-axis-azimuth"]),
             "plunge": float(tensor_props[f"{axis.lower()}-axis-plunge"]),
@@ -201,23 +213,25 @@
                 interface.
                 - IsInSlab : Boolean indicating whether depth is within the slab.
         Raises:
             AttributeError if the eventid is not found in ComCat.
         """
         if self.verbose:
             self.logger.info("Inside getSubductionTypeByID...")
-        lat, lon, depth, tensor_params = self.getOnlineTensor(eventid)
+        lat, lon, depth, magnitude, tensor_params = self.getOnlineTensor(eventid)
         if self.verbose:
             self.logger.info("Tensor Parameters: %s" % str(tensor_params))
         if lat is None:
             raise AttributeError("Event %s is not found in ComCat." % eventid)
 
         lat = float(lat)
         lon = float(lon)
-        results = self.getSubductionType(lat, lon, depth, tensor_params=tensor_params)
+        results = self.getSubductionType(
+            lat, lon, depth, magnitude, tensor_params=tensor_params
+        )
         return results
 
     def getOnlineTensor(self, eventid):
         """Get tensor parameters from preferred ComCat moment tensor.
 
         Args:
             eventid (str): ComCat EventID (Sumatra is official20041226005853450_30).
@@ -248,29 +262,30 @@
             self.logger.info("Inside getOnlineTensor")
         try:
             detail = get_event_details(eventid)
         except Exception as e:
             msg = 'Failed to get event information for %s - error "%s"'
             tpl = (eventid, str(e))
             self.logger.warn(msg % tpl)
-            return (None, None, None, None)
+            return (None, None, None, None, None)
         lat = detail["latitude"]
         lon = detail["longitude"]
         depth = detail["depth"]
+        magnitude = detail["magnitude"]
         if "tensor" not in detail:
             self.logger.info("No moment tensor available for %s" % eventid)
-            return lat, lon, depth, None
+            return (lat, lon, depth, magnitude, None)
 
         if self.verbose:
             self.logger.info("Getting tensor components...")
         tensor_params = detail["tensor"]
 
         # if no tensor, bail out
         if tensor_params is None:
-            lat, lon, depth, tensor_params
+            return (lat, lon, depth, magnitude, tensor_params)
 
         if self.verbose:
             self.logger.info("Getting tensor axes...")
         # sometimes the online MT is missing properties
 
         if "T" not in tensor_params and "mrr" in tensor_params:
             if self.verbose:
@@ -299,17 +314,19 @@
                 tensor_params["mrt"],
                 tensor_params["mrp"],
                 tensor_params["mtp"],
             )
             tensor_params["NP1"] = tensor2["NP1"].copy()
             tensor_params["NP2"] = tensor2["NP2"].copy()
 
-        return lat, lon, depth, tensor_params
+        return (lat, lon, depth, magnitude, tensor_params)
 
-    def getSubductionType(self, lat, lon, depth, eventid=None, tensor_params=None):
+    def getSubductionType(
+        self, lat, lon, depth, magnitude, eventid=None, tensor_params=None
+    ):
         """Given a event hypocenter, determine the subduction zone information.
 
         Args:
             lat (float): Epicentral latitude.
             lon (float): Epicentral longitude.
             depth (float): Epicentral depth.
             eventid (float): ComCat EventID (Sumatra is official20041226005853450_30).
@@ -374,15 +391,15 @@
         data_folder = pathlib.Path(config["DATA"]["folder"])
         tensor_type = None
         tensor_source = None
         similarity = np.nan
         nevents = 0
         if tensor_params is None:
             if eventid is not None:
-                _, _, _, tensor_params = self.getOnlineTensor(eventid)
+                _, _, _, _, tensor_params = self.getOnlineTensor(eventid)
                 if tensor_params is not None:
                     tensor_type = tensor_params["type"]
                     tensor_source = tensor_params["source"]
 
             if tensor_params is None:
                 dbfile = data_folder / config["DATA"]["dbfile"]
                 minboxcomp = float(config["CONSTANTS"]["minradial_distcomp"])
@@ -418,14 +435,19 @@
         results["CompositeVariability"] = similarity
         results["NComposite"] = nevents
         results["FocalMechanism"] = get_focal_mechanism(tensor_params)
         if len(slab_params):
             if np.isnan(slab_params["depth"]):
                 results["SlabModelRegion"] = SLAB_REGIONS[slab_params["region"]]
                 results["KaganAngle"] = np.nan
+                results["SlabModelDepth"] = np.nan
+                results["SlabModelDepthUncertainty"] = np.nan
+                results["SlabModelDip"] = np.nan
+                results["SlabModelStrike"] = np.nan
+                results["SlabModelMaximumDepth"] = np.nan
             else:
                 results["SlabModelRegion"] = SLAB_REGIONS[slab_params["region"]]
                 results["SlabModelDepth"] = slab_params["depth"]
                 results["SlabModelDepthUncertainty"] = slab_params["depth_uncertainty"]
                 results["SlabModelDip"] = slab_params["dip"]
                 results["SlabModelStrike"] = slab_params["strike"]
                 results["SlabModelMaximumDepth"] = slab_params[
@@ -449,38 +471,68 @@
             results["SlabModelDepth"] = np.nan
             results["SlabModelDepthUncertainty"] = np.nan
             results["SlabModelDip"] = np.nan
             results["SlabModelStrike"] = np.nan
             results["SlabModelMaximumDepth"] = np.nan
             results["KaganAngle"] = np.nan
 
-        results = results.reindex(
-            index=[
-                "TectonicRegion",
-                "FocalMechanism",
-                "TensorType",
-                "TensorSource",
-                "KaganAngle",
-                "CompositeVariability",
-                "NComposite",
-                "DistanceToStable",
-                "DistanceToActive",
-                "DistanceToSubduction",
-                "DistanceToHotSpot",
-                "Oceanic",
-                "DistanceToOceanic",
-                "DistanceToContinental",
-                "SlabModelRegion",
-                "SlabModelDepth",
-                "SlabModelDepthUncertainty",
-                "SlabModelDip",
-                "SlabModelStrike",
-                "SlabModelMaximumDepth",
-            ]
-        )
+        # Add in probability calculations for stable, active, volcanic, and
+        # subduction
+        # first, look for custom select.conf in data directory
+        default_conf = pathlib.Path(__file__).parent / "data" / "select.conf"
+        select_conf = pathlib.Path(config["DATA"]["folder"]) / "select.conf"
+        if not select_conf.exists():
+            select_conf = default_conf
+        select_config, result = get_select_config(select_conf)
+        probs = get_probs(magnitude, depth, results, select_config)
+
+        for key, prob_value in probs.items():
+            for shortkey, longkey in PROB_TRANSLATOR.items():
+                if key.startswith(shortkey):
+                    if "_" in key:
+                        remainder = key.replace(f"{shortkey}_", "")
+                        newkey = f"{longkey}{remainder.capitalize()}"
+                        results[newkey] = prob_value
+                    else:
+                        results[longkey] = prob_value
+                    break
+
+        # TODO: Some of the probability keys may not be predictable. shove them to the end?
+        predictable_index = [
+            "TectonicRegion",
+            "FocalMechanism",
+            "TensorType",
+            "TensorSource",
+            "KaganAngle",
+            "CompositeVariability",
+            "NComposite",
+            "DistanceToStable",
+            "DistanceToActive",
+            "DistanceToSubduction",
+            "DistanceToHotSpot",
+            "Oceanic",
+            "DistanceToOceanic",
+            "DistanceToContinental",
+            "SlabModelRegion",
+            "SlabModelDepth",
+            "SlabModelDepthUncertainty",
+            "SlabModelDip",
+            "SlabModelStrike",
+            "SlabModelMaximumDepth",
+            "ProbabilityActive",
+            "ProbabilityStable",
+            "ProbabilitySubduction",
+            "ProbabilityVolcanic",
+            "ProbabilitySubductionCrustal",
+            "ProbabilitySubductionInterface",
+            "ProbabilitySubductionIntraslab",
+        ]
+        remainder_index = set(results.index) - set(predictable_index)
+        index = predictable_index + list(remainder_index)
+        results = results.reindex(index=index)
 
         return results
 
 
 def get_focal_mechanism(tensor_params):
     """Return focal mechanism (strike-slip,normal, or reverse).
```

### Comparing `usgs-strec-2.2.5/src/strec/utils.py` & `usgs-strec-2.2.6/src/strec/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 def read_input_file(input_file, hypo_columns, id_column):
     """Read a CSV/Excel input file, return a DataFrame
 
     This function will deal with any moment tensor component columns it finds,
     (mrr,mtt,etc) and convert any that are integers into floats.
 
     Args:
-        input_file (str): Path to CSV/Excel file containing lat,lon,depth columns
+        input_file (str): Path to CSV/Excel file containing lat,lon,depth,mag columns
             and optionally moment tensor columns
             ('mrr','mtt','mpp','mrt','mrp','mtp').
     Returns:
         DataFrame: Pandas dataframe containing contents of input file.
     Raises:
         ValueError: When input file is neither a CSV nor an Excel file.
     """
@@ -144,18 +144,19 @@
         except Exception:
             raise ValueError("%s is neither a CSV nor Excel file." % input_file)
 
     idcol = None  # this is not required
     latcol = None
     loncol = None
     depcol = None
+    magcol = None
     if hypo_columns[0] is not None:
         if not set(hypo_columns).issubset(set(df.columns)):
             raise KeyError(f"Missing input hypo columns: {str(hypo_columns)}")
-        latcol, loncol, depcol = hypo_columns
+        latcol, loncol, depcol, magcol = hypo_columns
     if id_column is not None:
         if id_column not in df.columns:
             raise KeyError(f"Missing input comcat ID column: {id_column}")
         idcol = id_column
 
     # if the column names were not set by the user, try to find columns
     # that indicate comcatid, latitude, longitude and depth.
@@ -164,39 +165,42 @@
         latcol = df.columns[latidx].array[0]
     lonidx = df.columns.to_series().str.contains("^lon", case=False)
     if lonidx.any():
         loncol = df.columns[lonidx].array[0]
     depidx = df.columns.to_series().str.contains("^depth", case=False)
     if depidx.any():
         depcol = df.columns[depidx].array[0]
+    magidx = df.columns.to_series().str.contains("^mag", case=False)
+    if magidx.any():
+        magcol = df.columns[magidx].array[0]
 
     # the id column is not mandatory
     ididx = df.columns.to_series().str.contains("^eventid", case=False)
     if ididx.any():
         idcol = df.columns[ididx].array[0]
 
-    if latcol is None or loncol is None or depcol is None:
+    if latcol is None or loncol is None or depcol is None or magcol is None:
         raise KeyError(
             (
                 "Input table is missing identifiable columns for latitude, "
-                "longitude, and depth."
+                "longitude, depth, or magnitude."
             )
         )
 
     # convert any long integer moment component columns to floating point, because
     # otherwise pandas will complain later when re-writing row to a dataframe.  Doesn't
     # make sense, but seems necessary.
     for column in df:
         comps = ["mrr", "mtt", "mpp", "mrt", "mrp", "mtp"]
         for comp in comps:
             if column.lower().find(comp) > -1:
                 col = df[column].apply(lambda x: convert_float(x))
                 df[column] = col
 
-    return (df, idcol, latcol, loncol, depcol)
+    return (df, idcol, latcol, loncol, depcol, magcol)
 
 
 def convert_float(val):
     try:
         return float(val)
     except ValueError:
         return np.nan
```

### Comparing `usgs-strec-2.2.5/src/usgs_strec.egg-info/PKG-INFO` & `usgs-strec-2.2.6/src/usgs_strec.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.5
+Version: 2.2.6
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -29,14 +29,15 @@
 # Table of Contents
 - [Table of Contents](#table-of-contents)
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Upgrade](#upgrade)
 - [Configuration](#configuration)
 - [Usage](#usage)
+- [Probabilities] (#probabilities)
 - [Glossary](#glossary)
 
 # Introduction
 
 This library and set of tools was created to provide functionality to
 automatically determine the tectonic region of an earthquake
 (Subduction, Active, HotSpot, Stable), and the distance to the tectonic
@@ -170,14 +171,81 @@
 `regcalc -e -0.950 -21.725 10.0 -m 260 84 169 6.9`
 
 *Note: Users may notice that distances to tectonic regions the earthquake is NOT in may be unreasonably large values. The reason 
 for returning the distances to other regions is to help inform the user when the earthquake is close to another region.
 When STREC outputs these large numbers it indicates that the distance to that other region is not close enough to affect
 the properties of the earthquake.*
 
+# Probabilities
+
+STREC now calculates the probabilities of an earthquake being in any of the tectonic regions, and also in
+any of the various defined depth categories. For subduction regions these are hardcoded as 
+crustal, interface, and intraslab. For other regions, the *default* configuration includes the following:
+
+ - acr_shallow : active earthquakes occurring above 30 km
+ - acr_deep - active earthquakes occurring below 30 km
+ - scr_shallow - stable earthquakes at any depth
+ - volcanic_shallow - volcanic earthquakes at any depth
+
+## Probability configuration
+
+Users can configure the probability settings to include more finely grained depth zones for active, 
+stable, and volcanic regions. The default config file is located in the [repository] 
+(https://code.usgs.gov/ghsc/esi/strec/-/blob/main/src/strec/data/select.conf) and 
+installed with the software. To customize the probability depth zones, download a copy of the file from 
+the repository and save it in the [DATA]->folder in the config.ini file described above.
+
+```
+[DATA]
+folder = /data/strec
+```
+
+The relevant section of the select.conf file to modify looks like the following:
+
+```
+[tectonic_regions]
+    [[acr]]
+        horizontal_buffer = 100
+        vertical_buffer = 5
+        depth_labels = shallow, deep
+        min_depth = -Inf, 30
+        max_depth = 30, Inf
+    [[scr]]
+        horizontal_buffer = 100
+        vertical_buffer = 5
+        depth_labels = shallow
+        min_depth = -Inf
+        max_depth = Inf
+    [[subduction]]
+        horizontal_buffer = 100
+        vertical_buffer = 5
+        depth_labels = crustal, interface, intraslab
+        min_depth = -Inf, 15, 70
+        max_depth = 15, 70, Inf
+        use_slab = True
+    [[volcanic]]
+        horizontal_buffer = 10
+        vertical_buffer = 5
+        depth_labels = shallow
+        min_depth = -Inf
+        max_depth = Inf
+```
+
+To add a "deep" (10 km or deeper) category to the scr section, you would modify that 
+section to look like the following:
+
+```
+    [[scr]]
+        horizontal_buffer = 100
+        vertical_buffer = 5
+        depth_labels = shallow, deep
+        min_depth = -Inf, 10
+        max_depth = 10, Inf
+```
+
 
 # Glossary
 
 STREC defines a number of terms that may not be commonly
 understood, so they are explained here.  These terms may be different
 from the Garcia paper upon which this software is originally based.
```

### Comparing `usgs-strec-2.2.5/src/usgs_strec.egg-info/SOURCES.txt` & `usgs-strec-2.2.6/src/usgs_strec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 install.sh
 license.txt
 pyproject.toml
 select_regions.png
 src/strec/__init__.py
 src/strec/calc.py
 src/strec/cmt.py
+src/strec/config.py
 src/strec/database.py
 src/strec/distance.py
 src/strec/gcmt.py
 src/strec/gmreg.py
 src/strec/kagan.py
-src/strec/ngasub.py
 src/strec/slab.py
 src/strec/sm_probs.py
 src/strec/subduction.py
 src/strec/subtype.py
 src/strec/utils.py
 src/strec/bin/regcalc.py
 src/strec/bin/strec_cfg.py
 src/strec/data/REGION_GRIDS_README.txt
 src/strec/data/active.geojson
 src/strec/data/domains.xlsx
 src/strec/data/land.geojson
 src/strec/data/maximum_interface_depths.csv
 src/strec/data/moment_tensors.db
 src/strec/data/ocean.geojson
+src/strec/data/select.conf
+src/strec/data/selectspec.conf
 src/strec/data/stable.geojson
 src/strec/data/strec.ini
 src/strec/data/subduction.geojson
 src/strec/data/volcanic.geojson
 src/usgs_strec.egg-info/PKG-INFO
 src/usgs_strec.egg-info/SOURCES.txt
 src/usgs_strec.egg-info/dependency_links.txt
@@ -51,15 +53,14 @@
 test/src/strec/calc_test.py
 test/src/strec/cmt_test.py
 test/src/strec/database_test.py
 test/src/strec/distance_test.py
 test/src/strec/gcmt_test.py
 test/src/strec/gmreg_test.py
 test/src/strec/kagan_test.py
-test/src/strec/ngasub_test.py
 test/src/strec/probs_test.py
 test/src/strec/slab_test.py
 test/src/strec/subduction_test.py
 test/src/strec/subtype_test.py
 test/src/strec/utils_test.py
 test/src/strec/data/big_focals.xlsx
 test/src/strec/data/comcatid_catalog.xlsx
```

### Comparing `usgs-strec-2.2.5/test/src/data/AMlvPS_trench.json` & `usgs-strec-2.2.6/test/src/data/AMlvPS_trench.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/data/large_events.xlsx` & `usgs-strec-2.2.6/test/src/data/large_events.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/data/strec.db` & `usgs-strec-2.2.6/test/src/data/strec.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/data/test_regimes.xlsx` & `usgs-strec-2.2.6/test/src/data/test_regimes.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/calc_test.py` & `usgs-strec-2.2.6/test/src/strec/calc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,87 +158,88 @@
     assert not check_moment_row(row)
 
 
 def test_get_input_dataframe():
     simple_catalog_file = pathlib.Path(__file__).parent / "data" / "simple_catalog.xlsx"
     eqinfo = None
     event_id = None
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
-    simple_dataframe, _, _, _, _ = get_input_dataframe(
+    simple_dataframe, _, _, _, _, _ = get_input_dataframe(
         simple_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
     cmp_simple = pd.DataFrame(
         {
             "Latitude": [-5.074, -1.008],
             "Longitude": [103.083, 98.642],
             "Depth": [50.5, 17.6],
+            "Magnitude": [6.5, 6.5],
         }
     )
     assert simple_dataframe.equals(cmp_simple)
 
     comcat_catalog_file = (
         pathlib.Path(__file__).parent / "data" / "comcatid_catalog.xlsx"
     )
     eqinfo = None
     event_id = None
     hypo_columns = [None, None, None]
     id_column = None
-    comcat_dataframe, idcol, _, _, _ = get_input_dataframe(
+    comcat_dataframe, idcol, _, _, _, _ = get_input_dataframe(
         comcat_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
     assert idcol == "EventID"
 
     id_catalog_file = pathlib.Path(__file__).parent / "data" / "id_catalog.xlsx"
     eqinfo = None
     event_id = None
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = "id"
-    comcat_dataframe, idcol, _, _, _ = get_input_dataframe(
+    comcat_dataframe, idcol, _, _, _, _ = get_input_dataframe(
         id_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
     assert idcol == "id"
 
     hypo_catalog_file = pathlib.Path(__file__).parent / "data" / "hypocols_catalog.xlsx"
     eqinfo = None
     event_id = None
-    hypo_columns = ["EventLatitude", "EventLongitude", "EventDepth"]
+    hypo_columns = ["EventLatitude", "EventLongitude", "EventDepth", "magnitude"]
     id_column = None
-    hypo_dataframe, idcol, latcol, loncol, depcol = get_input_dataframe(
+    hypo_dataframe, idcol, latcol, loncol, depcol, magcol = get_input_dataframe(
         hypo_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
-    assert [latcol, loncol, depcol] == hypo_columns
+    assert [latcol, loncol, depcol, magcol] == hypo_columns
 
     moment_catalog_file = pathlib.Path(__file__).parent / "data" / "moment_catalog.xlsx"
     eqinfo = None
     event_id = None
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
-    moment_dataframe, _, _, _, _ = get_input_dataframe(
+    moment_dataframe, _, _, _, _, _ = get_input_dataframe(
         moment_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
     assert "mrt" in moment_dataframe.columns
 
     focal_catalog_file = pathlib.Path(__file__).parent / "data" / "focal_catalog.xlsx"
     eqinfo = None
     event_id = None
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
-    focal_dataframe, _, _, _, _ = get_input_dataframe(
+    focal_dataframe, _, _, _, _, _ = get_input_dataframe(
         focal_catalog_file, eqinfo, event_id, hypo_columns, id_column
     )
     assert "strike" in focal_dataframe.columns
 
 
 def test_select_regions():
     simple_catalog_file = pathlib.Path(__file__).parent / "data" / "simple_catalog.xlsx"
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
     simple_dataframe = select_regions(
         simple_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
@@ -250,15 +251,15 @@
 
     comcat_catalog_file = (
         pathlib.Path(__file__).parent / "data" / "comcatid_catalog.xlsx"
     )
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
     comcat_dataframe = select_regions(
         comcat_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
@@ -267,15 +268,15 @@
     )
     assert comcat_dataframe["FocalMechanism"].to_list() == ["RS", "SS"]
 
     id_catalog_file = pathlib.Path(__file__).parent / "data" / "id_catalog.xlsx"
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = "id"
     id_dataframe = select_regions(
         id_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
@@ -284,15 +285,15 @@
     )
     assert id_dataframe["FocalMechanism"].to_list() == ["RS", "SS"]
 
     hypo_catalog_file = pathlib.Path(__file__).parent / "data" / "hypocols_catalog.xlsx"
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = ["EventLatitude", "EventLongitude", "EventDepth"]
+    hypo_columns = ["EventLatitude", "EventLongitude", "EventDepth", "magnitude"]
     id_column = None
     hypo_dataframe = select_regions(
         hypo_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
@@ -301,15 +302,15 @@
     )
     assert hypo_dataframe["FocalMechanism"].to_list() == ["RS", "SS"]
 
     moment_catalog_file = pathlib.Path(__file__).parent / "data" / "moment_catalog.xlsx"
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
     moment_dataframe = select_regions(
         moment_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
@@ -318,31 +319,31 @@
     )
     assert moment_dataframe["FocalMechanism"].to_list() == ["RS", "SS"]
 
     focal_catalog_file = pathlib.Path(__file__).parent / "data" / "focal_catalog.xlsx"
     eqinfo = None
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
     focal_dataframe = select_regions(
         focal_catalog_file,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
         id_column,
         False,
     )
     assert focal_dataframe["FocalMechanism"].to_list() == ["RS", "SS"]
 
-    eqinfo = [37.7132, 141.5793, 41]
+    eqinfo = [37.7132, 141.5793, 41, 6.5]
     event_id = None
     moment_info = [None, None, None, None]
-    hypo_columns = [None, None, None]
+    hypo_columns = [None, None, None, None]
     id_column = None
     eq_dataframe = select_regions(
         None,
         eqinfo,
         moment_info,
         event_id,
         hypo_columns,
```

### Comparing `usgs-strec-2.2.5/test/src/strec/cmt_test.py` & `usgs-strec-2.2.6/test/src/strec/cmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/big_focals.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/big_focals.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/comcatid_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/comcatid_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/focal_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/focal_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/hypocols_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/hypocols_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/id_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/id_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/moment_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/moment_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/nga_matched.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/nga_matched.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/simple_catalog.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/simple_catalog.xlsx`

 * *Files 14% similar despite different names*

```diff
@@ -103,524 +103,533 @@
 00000660: d542 53ed ad86 b0b7 37a0 ea93 cf9b 7fd7  .BS.....7.......
 00000670: 96a6 e90d 3f88 394c ecd2 9915 c873 6267  ....?.9L.....sbg
 00000680: d9ae 7cc8 6c21 f5f9 1a55 5368 3969 b062  ..|.l!...USh9i.b
 00000690: 9e72 3a22 795f 646c c0f3 449b bf13 fd7c  .r:"y_dl..D....|
 000006a0: 2d4e 9cc8 5222 3412 f832 cf47 c725 a0f5  -N..R"4..2.G.%..
 000006b0: 7f5a b434 f1cb 9d79 c437 09c3 abc8 f0c9  .Z.4...y.7......
 000006c0: 828b 1fa8 de01 0000 ffff 0300 504b 0304  ............PK..
-000006d0: 1400 0600 0800 0000 2100 dd65 4702 6d03  ........!..eG.m.
-000006e0: 0000 6208 0000 0f00 0000 786c 2f77 6f72  ..b.......xl/wor
-000006f0: 6b62 6f6f 6b2e 786d 6cac 556d 6fa3 3810  kbook.xml.Umo.8.
-00000700: fe7e d2fd 0784 ee2b c526 bcab 7495 04d0  .~.....+.&..t...
-00000710: 556a 5755 9b6d bf44 5a39 608a 55c0 9c31  UjWU.m.DZ9`.U..1
-00000720: 4daa 6aff fb8d 21a4 6fa7 55b6 7b55 6a63  M.j...!.o.U.{Ujc
-00000730: 8f79 fccc cc33 c3e9 975d 5d69 8f54 748c  .y...3...]]i.Tt.
-00000740: 3791 8e4f 90ae d126 e339 6bee 23fd db2a  7..O...&.9k.#..*
-00000750: 357c 5deb 2469 7252 f186 46fa 13ed f42f  5|].$irR..F..../
-00000760: 677f fe71 bae5 e261 c3f9 8306 004d 17e9  g..q...a.....M..
-00000770: a594 6d68 9a5d 56d2 9a74 27bc a50d 580a  ..mh.]V..t'...X.
-00000780: 2e6a 2261 29ee cdae 1594 e45d 49a9 ac2b  .j"a)......]I..+
-00000790: d342 c835 6bc2 1a7d 4408 c531 18bc 2858  .B.5k..}D..1..(X
-000007a0: 4663 9ef5 356d e408 2268 4524 d0ef 4ad6  Fc..5m.."hE$..J.
-000007b0: 7613 5a9d 1d03 5713 f1d0 b746 c6eb 1620  v.Z...W....F... 
-000007c0: 36ac 62f2 6900 d5b5 3a0b cfef 1b2e c8a6  6.b.i...:.......
-000007d0: 02b7 77d8 d176 027e 2efc 6304 8335 dd04  ..w..v.~..c..5..
-000007e0: a60f 57d5 2c13 bce3 853c 0168 7324 fdc1  ..W.,....<.hs$..
-000007f0: 7f8c 4c8c df84 60f7 3106 c721 d9a6 a08f  ..L...`.1..!....
-00000800: 4ce5 f0c0 4ab8 9f64 e51e b0dc 1730 8c7e  L...J..d.....0.~
-00000810: 1b0d 83b4 06ad 8410 bc4f a239 076e 967e  .........O.9.n.~
-00000820: 765a b08a de8e d2d5 48db 7e25 b5ca 54a5  vZ......H.~%..T.
-00000830: 6b15 e964 9233 49f3 48f7 60c9 b7f4 cd86  k..d.3I.H.`.....
-00000840: e8db 45cf 2ab0 5a33 1f61 dd3c 3bc8 f94a  ..E.*.Z3.a.<;..J
-00000850: 6839 2d48 5fc9 1508 7982 87ca 70dd c072  h9-H_...y...p..r
-00000860: d449 10c6 bc92 5434 44d2 256f 24e8 70ef  .I....T4D.%o$.p.
-00000870: d7ef 6a6e c05e 961c 14ae 5dd3 7f7a 2628  ..jn.^....]..z&(
-00000880: 1416 e80b 7c85 9164 21d9 7457 4496 5a2f  ....|..d!.tWD.Z/
-00000890: aa48 5faf b75d f5d7 fadb a66f 64bf 2e79  .H_..].....od..y
-000008a0: 4dd7 7549 8968 e85a d6ed fa95 3ec9 c762  M.uI.h.Z....>..b
-000008b0: f805 8592 4cb9 6d82 df23 b7f1 f97d 0c80  ....L.m..#...}..
-000008c0: a208 2715 5e49 a1c1 f379 7c01 99b8 218f  ..'.^I...y|...!.
-000008d0: 9017 c87e be2f db73 08bc fffd d90d 528c  ...~./.s......R.
-000008e0: 96ae 6d78 73bc 34ec 24f6 8dc0 b36d 23c0  ..mxs.4.$....m#.
-000008f0: 6992 2eac 349e 63eb 0778 21dc 30e3 a497  i...4.c..x!.0...
-00000900: e53e d70a 33d2 6da5 cef7 a64b b29b 2c18  .>..3.m....K..,.
-00000910: 853d cb5f ee7f 46fb 3f43 cdef 86c9 f643  .=._..F.?C.....C
-00000920: 79aa bada 2da3 dbee 4515 6aa9 edee 5893  y...-...E.j...X.
-00000930: f36d a41b d8c3 9ea3 6b4f d306 c60e 2cb7  .m......kO....,.
-00000940: 83f9 8ee5 b204 bdd8 d805 97c7 bdbf 29bb  ..............).
-00000950: 2f81 33b6 7c5b 5581 b014 b748 7f9e c781  /.3.|[U....H....
-00000960: eff9 9e67 5833 1b42 60cf 7dc3 c7b6 6358  ...gX3.B`.}...cX
-00000970: 4b84 e265 e240 4c66 0327 f315 a9a1 8302  K..e.@Lf.'......
-00000980: b961 d69a 41f5 37aa ab62 68d5 6a56 f185  .a..A.7..bh.jV..
-00000990: 6711 aa3b c479 3e08 dc9c 5ecb 4895 81ca  g..;.y>...^.H...
-000009a0: d534 1c0c 30b2 02e5 37dd c98b 4e0e 3308  .4..0...7...N.3.
-000009b0: 8c01 3d6c a3b9 8702 db40 c9cc 316c 3fb0  ..=l.....@..1l?.
-000009c0: 0cdf 9e59 c6d2 8ead c4f1 9238 5938 2a43  ...Y.......8Y8*C
-000009d0: ea0b 10fe 1f7d 70d0 7938 7d5a 14cb 9208  .....}p.y8}Z....
-000009e0: b912 247b 800f d235 2d16 a403 2d8d 0e01  ..${...5-...-...
-000009f0: dfd7 6417 8ebf 4033 a068 a738 356c 1c20  ..d...@3.h.85l. 
-00000a00: 63b1 0075 3971 3a73 3cac c299 be90 55ee  c..u9q:s<.....U.
-00000a10: 179f ec42 be39 bc4d 89ec a142 5571 0eeb  ...B.9.M...BUq..
-00000a20: 508d e97e f7b0 598c 1bfb 3cbd 29bb f03a  P..~..Y...<.)..:
-00000a30: 5671 dfbf fdb3 8337 e07d 458f 3c9c de1e  Vq.....7.}E.<...
-00000a40: 7970 f9f5 7275 79e4 d98b 64f5 fd2e 1d1a  yp..ruy...d.....
-00000a50: c17f 7a6b 0ed9 50e3 a021 73ca e1d9 bf00  ..zk..P..!s.....
-00000a60: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00000a70: 0000 2100 813e 9497 f300 0000 ba02 0000  ..!..>..........
-00000a80: 1a00 0801 786c 2f5f 7265 6c73 2f77 6f72  ....xl/_rels/wor
-00000a90: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 20a2  kbook.xml.rels .
-00000aa0: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006d0: 1400 0600 0800 0000 2100 f4e4 7444 8903  ........!...tD..
+000006e0: 0000 9308 0000 0f00 0000 786c 2f77 6f72  ..........xl/wor
+000006f0: 6b62 6f6f 6b2e 786d 6cac 555d 6fa3 3814  kbook.xml.U]o.8.
+00000700: 7d5f 69fe 03e2 9d62 1320 809a 8e02 046d  }_i....b. .....m
+00000710: a576 54b5 99f6 05a9 72c0 29a8 8019 db34  .vT.....r.)....4
+00000720: a9aa f9ef 73ed 84b4 9dae 56d9 ce46 c4c6  ....s.....V..F..
+00000730: 1f1c ceb9 f75c 73fa 75db 36c6 13e5 a266  .....\s.u.6....f
+00000740: ddcc c427 c834 6857 b0b2 ee1e 66e6 f765  ...'.4hW....f..e
+00000750: 6605 a621 24e9 4ad2 b08e cecc 672a ccaf  f..!$.J.....g*..
+00000760: 675f fe3a dd30 feb8 62ec d100 804e cccc  g_.:.0..b....N..
+00000770: 4aca 3eb2 6d51 54b4 25e2 84f5 b483 9535  J.>.mQT.%......5
+00000780: e32d 9130 e40f b6e8 3925 a5a8 2895 6d63  .-.0....9%..(.mc
+00000790: 3b08 f976 4bea cedc 2144 fc18 0cb6 5ed7  ;..vK...!D....^.
+000007a0: 054d 5931 b4b4 933b 104e 1b22 81be a8ea  .MY1...;.N."....
+000007b0: 5e8c 686d 710c 5c4b f8e3 d05b 056b 7b80  ^.hmq.\K...[.k{.
+000007c0: 58d5 4d2d 9f35 a869 b445 74fe d031 4e56  X.M-.5.i.Et..1NV
+000007d0: 0dc8 de62 cfd8 72b8 7cf8 6304 8d33 be09  ...b..r.|.c..3..
+000007e0: 963e bcaa ad0b ce04 5bcb 1380 b677 a43f  .>......[....w.?
+000007f0: e8c7 c8c6 f85d 08b6 1f63 701c 926b 73fa  .....]...cp..ks.
+00000800: 54ab 1c1e 5871 ff93 acfc 0396 ff0a 86d1  T...Xq..........
+00000810: 1fa3 61b0 96f6 4a04 c1fb 249a 77e0 e698  ..a...J...$.w...
+00000820: 67a7 ebba a1b7 3beb 1aa4 efbf 9156 65aa  g.....;......Ve.
+00000830: 318d 8608 b928 6b49 cb99 3985 21db d077  1....(kI..9.!..w
+00000840: 137c e8e3 a16e 60d5 f17c 844d fbec 60e7  .|...n`..|.M..`.
+00000850: 2b6e 9474 4d86 462e c1c8 233c 5486 ef87  +n.tM.F...#<T...
+00000860: 8ea7 7682 31e6 8da4 bc23 9226 ac93 e0c3  ..v.1....#.&....
+00000870: bdae 3ff5 9cc6 4e2a 060e 37ae e98f a1e6  ..?...N*..7.....
+00000880: 140a 0bfc 055a a125 4544 56e2 8ac8 ca18  .....Z.%EDV.....
+00000890: 7833 33f3 7c23 9a93 8615 a4a9 9890 f9f7  x33.|#..........
+000008a0: d5d0 c921 af58 4bf3 b6a2 8477 3417 bcc8  ...!.XK....w4...
+000008b0: fb67 59b1 2e17 92d3 2297 1009 3dbb 1b96  .gY....."...=...
+000008c0: 4492 fc8d 93c9 c7b2 f90f 5e26 850a 900d  D.........^&....
+000008d0: 11da a9d8 ddff 1e2d 10c3 a3d1 af57 921b  .......-.....W..
+000008e0: 707f 9e5e 40ce 6ec8 1364 107c 52ee 0bfc  p..^@.n..d.|R...
+000008f0: 1c52 8427 f75d c123 7cff 924d ddc0 f713  .R.'.].#|..M....
+00000900: c78a 131c 582e 9e27 d61c bb8e 859d 050a  ....X..'........
+00000910: c238 4b27 71f8 13c4 703f 2a18 1964 b537  .8K'q...p?*..d.7
+00000920: 8782 9e99 2e38 e1c3 d225 d98e 2b18 4543  .....8...%..+.EC
+00000930: 5dbe d278 41fb 9fa5 fadf 9a71 eda7 12ac  ]..xA......q....
+00000940: 8ec1 db9a 6ec4 ab8d d4d0 d8de d55d c936  ....n........].6
+00000950: 33d3 727c 04e6 319e c709 0f87 a072 a397  3.r|..1......r..
+00000960: efea 5256 2073 8afd c3dc dfb4 7ea8 8033  ..RV s......~..3
+00000970: c648 970d 7714 b799 f932 4fc3 601a 4ca7  .H..w....2O.`.L.
+00000980: 9633 7113 cb75 e781 1560 d7b3 9c04 a134  .3q..u...`.....4
+00000990: 5978 8b34 9868 4ef6 1b52 fac8 0572 ba37  Yx.4.hN..R...r.7
+000009a0: 3a5d 2637 ea18 c670 b6ab 5e87 d934 78a4  :]&7...p..^..4x.
+000009b0: dec1 cf4b 5d11 f6f8 18f8 ab80 b250 9dde  ...K]........P..
+000009c0: 1862 e484 4a37 ddca 0b21 750f 8eac 811e  .b..J7...!u.....
+000009d0: 76d1 7c8a 42d7 428b 8967 b941 e858 813b  v.|.B.B..g.A.X.;
+000009e0: 71ac c44d 9d85 375d a48b d853 1952 9f8c  q..M..7]...S.R..
+000009f0: e8ff 3838 7561 44e3 b748 b1ac 0897 4b4e  ..88uaD..H....KN
+00000a00: 8a47 f882 5dd3 754c 0458 6a27 08f8 be25  .G..].uL.Xj'...%
+00000a10: 1b7b 418c 2640 d1cd 7006 760a 9115 c7be  .{A.&@..p.v.....
+00000a20: 6b79 6936 f1a6 5885 337b 25ab e4af 3f79  kyi6..X.3{%...?y
+00000a30: 6c05 b67e 9a12 3940 49ab 6ad6 e348 b5d9  l..~..9@I.j..H..
+00000a40: 7ef6 30b9 de4d ecf3 f4ae faa2 eb54 c57d  ~.0..M.......T.}
+00000a50: fff4 bf6d bc01 f50d 3d72 7376 7be4 c6e4  ...m....=rsv{...
+00000a60: dbe5 f2f2 c8bd 178b e5fd 5da6 cf83 7f54  ..........]....T
+00000a70: 6beb 6ca8 567b c81e 7378 f60b 0000 ffff  k.l.V{..sx......
+00000a80: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00000a90: 813e 9497 f300 0000 ba02 0000 1a00 0801  .>..............
+00000aa0: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
+00000ab0: 6b2e 786d 6c2e 7265 6c73 20a2 0401 28a0  k.xml.rels ...(.
+00000ac0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ba0: 0000 0000 0000 ac52 4d4b c430 10bd 0bfe  .......RMK.0....
-00000bb0: 8730 779b 7615 11d9 742f 22ec 55eb 0f08  .0w.v...t/".U...
-00000bc0: c9b4 29db 2621 337e f4df 1b2a ba5d 58d6  ..).&!3~...*.]X.
-00000bd0: 4b2f 036f 8679 efcd c776 f735 0ee2 0313  K/.o.y...v.5....
-00000be0: f5c1 2ba8 8a12 047a 136c ef3b 056f cdf3  ..+....z.l.;.o..
-00000bf0: cd03 0862 edad 1e82 4705 1312 ecea ebab  ...b....G.......
-00000c00: ed0b 0e9a 7313 b93e 92c8 2c9e 1438 e6f8  ....s..>..,..8..
-00000c10: 2825 1987 a3a6 2244 f4b9 d286 346a ce30  (%...."D....4j.0
-00000c20: 7532 6a73 d01d ca4d 59de cbb4 e480 fa84  u2js...MY.......
-00000c30: 53ec ad82 b4b7 b720 9a29 66e5 ffb9 43db  S...... .)f...C.
-00000c40: f606 9f82 791f d1f3 1909 493c 0d79 00d1  ....y.....I<.y..
-00000c50: e8d4 212b f8c1 45f6 08f2 bcfc 664d 79ce  ..!+..E.....fMy.
-00000c60: 6bc1 a3fa 0ce5 1cab 4b1e aa35 3d7c 8674  k.......K..5=|.t
-00000c70: 2087 c847 1f7f 2992 73e5 a299 bb55 efe1   ..G..).s....U..
-00000c80: 7442 fbca 29bf dbf2 2ccb f4ef 66e4 c9c7  tB..)...,...f...
-00000c90: d5df 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00000ca0: 0008 0000 0021 0093 eade ab7b 0200 00c7  .....!.....{....
-00000cb0: 0500 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
-00000cc0: 6565 7473 2f73 6865 6574 312e 786d 6c9c  eets/sheet1.xml.
-00000cd0: 544d 8f9b 3010 bd57 ea7f b07c 076c 2024  TM..0..W...|.l $
-00000ce0: 4140 954f 750f 95aa 6edb bb63 4c62 2d60  A@.Ou...n..cLb-`
-00000cf0: 6a3b c9ae aafe f70e d010 9add 43b4 0824  j;..........C..$
-00000d00: 9b19 de7b 33f3 70f2 e9b9 2ad1 4968 2355  ...{3.p...*.Ih#U
-00000d10: 9d62 ea12 8c44 cd55 2eeb 7d8a 7f7c df3a  .b...D.U..}..|.:
-00000d20: 338c 8c65 75ce 4a55 8b14 bf08 833f 651f  3..eu.JU.....?e.
-00000d30: 3f24 67a5 9fcc 4108 8b00 a136 293e 58db  ?$g...A....6)>X.
-00000d40: c49e 67f8 4154 ccb8 aa11 3544 0aa5 2b66  ..g.AT....5D..+f
-00000d50: 61ab f79e 69b4 6079 f751 557a 3e21 9157  a...i.`y.QUz>!.W
-00000d60: 3159 e31e 21d6 f760 a8a2 905c ac15 3f56  1Y..!..`...\..?V
-00000d70: a2b6 3d88 1625 b3a0 df1c 6463 2e68 15bf  ..=..%....dc.h..
-00000d80: 07ae 62fa e9d8 385c 550d 40ec 6429 ed4b  ..b...8\U.@.d).K
-00000d90: 078a 51c5 e387 7dad 34db 9550 f733 0d19  ..Q...}.4..P.3..
-00000da0: 47cf 1a6e 1f9e e042 d3bd 7fc5 5449 ae95  G..n...B....TI..
-00000db0: 5185 7501 d9eb 35bf 2e7f eecd 3dc6 07a4  Q.u...5.....=...
-00000dc0: d7f5 df05 4343 4f8b 936c 0778 85f2 df27  ....CCO..l.x...'
-00000dd0: 894e 062c ff0a 16bc 132c 1ac0 da76 e9f8  .N.,.....,...v..
-00000de0: 28f3 14ff 8e36 4bb2 5dcf 67ce 6a43 0227  (....6K.].g.jC.'
-00000df0: 5c6d a6ce 72b6 993b 34f4 b793 e562 1146  \m..r..;4....b.F
-00000e00: 01fd 83b3 2497 30e1 b62a a445 91e2 058d  ....$.0..*.E....
-00000e10: 5701 f6b2 a4f3 cf4f 29ce 66b4 4696 ed1e  W......O).f.F...
-00000e20: 4529 b815 c041 316a edb9 53ea a94d 7c80  E)...A1j..S..M|.
-00000e30: 5704 104d 97d0 2232 6ee5 49ac 4459 a678  W..M.."2n.I.DY.x
-00000e40: 1581 c37f 751c b004 026f 6018 af2f 6cdb  ....u....o`../l.
-00000e50: ced0 5f35 ca45 c18e a5fd a6ce 9f85 dc1f  .._5.E..........
-00000e60: 2cd0 866e 0885 b64e 89f3 97b5 301c 2c0a  ,..n...N....0.,.
-00000e70: d4ee 55f7 9a59 9625 5a9d 114c 1b64 9a86  ..U..Y.%Z..L.d..
-00000e80: b5ff 0e8d db0e bdf5 6196 f036 7501 b900  ........a..6u...
-00000e90: 65a0 8a53 4612 ef04 d2f8 bfd8 721c a3ff  e..SF.......r...
-00000ea0: c756 e398 3fc4 3c50 30c8 8049 df2d c3ef  .V..?.<P0..I.-..
-00000eb0: 0438 1397 4c83 f9e8 9add 48ea f328 095c  .8..L.....H..(.\
-00000ec0: 320b 6e24 f5b1 0971 276f eb81 56dc ad27  2.n$...q'o..V..'
-00000ed0: e8f5 c0b9 456e 25f4 a1f9 cc8d 423a 521a  ....En%.....B:R.
-00000ee0: dda8 e9d3 e8d4 8dc8 f8ba f6b1 ef55 6f8a  .............Uo.
-00000ef0: 7e7c 0ddb 8b2f 4cef 656d 5029 8a6e c453  ~|.../L.emP).n.S
-00000f00: 8c74 ef02 e2c2 daaa a61d fc74 82d1 4e59  .t.........t..NY
-00000f10: abaa cbee 0027 a080 81b6 a640 8552 f6b2  .....'.....@.R..
-00000f20: 01e3 b5b8 8fc2 1e1b a4b4 04eb 7487 5a8a  ............t.Z.
-00000f30: 1ba5 ad66 d202 43dc fe41 fa21 a79d 4f87  ...f..C..A.!..O.
-00000f40: 2338 fb0b 0000 ffff 0300 504b 0304 1400  #8........PK....
-00000f50: 0600 0800 0000 2100 c117 10be 4e07 0000  ......!.....N...
-00000f60: c620 0000 1300 0000 786c 2f74 6865 6d65  . ......xl/theme
-00000f70: 2f74 6865 6d65 312e 786d 6cec 59cd 8b1b  /theme1.xml.Y...
-00000f80: 3714 bf17 fa3f 0c73 77fc 35e3 8f25 dee0  7....?.sw.5..%..
-00000f90: cf6c 93dd 2464 9d94 1cb5 b6ec 5156 3332  .l..$d......QV32
-00000fa0: 92bc 1b13 0225 39f5 5228 a4a5 9742 6f3d  .....%9.R(...Bo=
-00000fb0: 94d2 4003 0dbd f48f 0924 b4e9 1fd1 27cd  ..@......$....'.
-00000fc0: d823 ade5 249b 6c4a 5a76 0d8b 47fe bda7  .#..$.lJZv..G...
-00000fd0: a7f7 9e7e 7af3 74f1 d2bd 987a 4798 0bc2  ...~z.t....zG...
-00000fe0: 9296 5fbe 50f2 3d9c 8cd8 9824 d396 7f6b  .._.P.=....$...k
-00000ff0: 3828 347c 4f48 948c 1165 096e f90b 2cfc  8(4|OH...e.n..,.
-00001000: 4bdb 9f7e 7211 6dc9 08c7 d803 f944 6ca1  K..~r.m......Dl.
-00001010: 961f 4939 db2a 16c5 0886 91b8 c066 3881  ..I9.*.......f8.
-00001020: df26 8cc7 48c2 239f 16c7 1c1d 83de 9816  .&..H.#.........
-00001030: 2ba5 52ad 1823 92f8 5e82 6250 7b7d 3221  +.R..#..^.bP{}2!
-00001040: 23ec 0d95 4a7f 7ba9 bc4f e131 9142 0d8c  #...J.{..O.1.B..
-00001050: 28df 57aa b125 a1b1 e3c3 b242 8885 e852  (.W..%.....B...R
-00001060: ee1d 21da f261 9e31 3b1e e27b d2f7 2812  ..!..a.1;..{..(.
-00001070: 127e 68f9 25fd e717 b72f 16d1 5626 44e5  .~h.%..../..V&D.
-00001080: 0659 436e a0ff 32b9 4c60 7c58 d173 f2e9  .YCn..2.L`|X.s..
-00001090: c16a d220 0883 5a7b a55f 03a8 5cc7 f5eb  .j. ..Z{._..\...
-000010a0: fd5a bfb6 d2a7 0168 3482 95a6 b6d8 3aeb  .Z.....h4.....:.
-000010b0: 956e 9061 0d50 fad5 a1bb 57ef 55cb 16de  .n.a.P....W.U...
-000010c0: d05f 5db3 b91d aa8f 85d7 a054 7fb0 861f  ._]........T....
-000010d0: 0cba e045 0baf 4129 3e5c c387 9d66 a767  ...E..A)>\...f.g
-000010e0: ebd7 a014 5f5b c3d7 4bed 5e50 b7f4 6b50  ...._[..K.^P..kP
-000010f0: 4449 72b8 862e 85b5 6a77 b9da 1564 c2e8  DIr.....jw...d..
-00001100: 8e13 de0c 8341 bd92 29cf 5190 0dab ec52  .....A..).Q....R
-00001110: 534c 5822 37e5 5a8c ee32 3e00 8002 5224  SLX"7.Z..2>...R$
-00001120: 49e2 c9c5 0c4f d008 b2b8 8b28 39e0 c4db  I....O.....(9...
-00001130: 25d3 0812 6f86 1226 60b8 5429 0d4a 55f8  %...o..&`.T).JU.
-00001140: af3e 81fe a623 8ab6 3032 a495 5d60 8958  .>...#..02..]`.X
-00001150: 1b52 f678 62c4 c94c b6fc 2ba0 d537 202f  .R.xb..L..+..7 /
-00001160: 9e3d 7bfe f0e9 f387 bf3d 7ff4 e8f9 c35f  .={......=....._
-00001170: b2b9 b52a 4b6e 0725 5353 eed5 8f5f fffd  ...*Kn.%SS..._..
-00001180: fd17 de5f bffe f0ea f137 e9d4 27f1 c2c4  ..._.....7..'...
-00001190: bffc f9cb 97bf fff1 3af5 b0e2 dc15 2fbe  ........:...../.
-000011a0: 7df2 f2e9 9317 df7d f5e7 4f8f 1dda db1c  }......}..O.....
-000011b0: 1d98 f021 89b1 f0ae e163 ef26 8b61 810e  ...!.....c.&.a..
-000011c0: fbf1 013f 9dc4 3042 c492 4011 e876 a8ee  ...?..0B..@..v..
-000011d0: cbc8 025e 5b20 eac2 75b0 edc2 db1c 58c6  ...^[ ..u.....X.
-000011e0: 05bc 3cbf 6bd9 ba1f f1b9 248e 99af 46b1  ..<.k.....$...F.
-000011f0: 05dc 638c 7618 773a e0aa 9acb f0f0 709e  ..c.v.w:......p.
-00001200: 4cdd 93f3 b989 bb89 d091 6bee 2e4a ac00  L.........k..J..
-00001210: f7e7 33a0 57e2 52d9 8db0 65e6 0d8a 1289  ..3.W.R...e.....
-00001220: a638 c1d2 53bf b143 8c1d abbb 4388 e5d7  .8..S..C....C...
-00001230: 3d32 e24c b089 f4ee 10af 8388 d325 4372  =2.L.........%Cr
-00001240: 6025 522e b443 6288 cbc2 6520 84da f2cd  `%R..Cb...e ....
-00001250: de6d afc3 a86b d53d 7c64 2361 5b20 ea30  .m...k.=|d#a[ .0
-00001260: 7e88 a9e5 c6cb 682e 51ec 5239 4431 351d  ~.....h.Q.R9D15.
-00001270: be8b 64e4 3272 7fc1 4726 ae2f 2444 7a8a  ..d.2r..G&./$Dz.
-00001280: 29f3 fa63 2c84 4be6 3a87 f51a 41bf 0a0c  )..c,.K.:...A...
-00001290: e30e fb1e 5dc4 3692 4b72 e8d2 b98b 1833  ....].6.Kr.....3
-000012a0: 913d 76d8 8d50 3c73 da4c 92c8 c47e 260e  .=v..P<s.L...~&.
-000012b0: 2145 9177 8349 177c 8fd9 3b44 3d43 1c50  !E.w.I.|..;D=C.P
-000012c0: b231 dcb7 09b6 c2fd 6622 b805 e46a 9a94  .1......f"...j..
-000012d0: 2788 fa65 ce1d b1bc 8c99 bd1f 1774 82b0  '..e.........t..
-000012e0: 8b65 da3c b6d8 b5cd 8933 3b3a f3a9 95da  .e.<.....3;:....
-000012f0: bb18 5374 8cc6 187b b73e 7358 d061 33cb  ..St...{.>sX.a3.
-00001300: e7b9 d157 2260 951d ec4a ac2b c8ce 55f5  ...W"`...J.+..U.
-00001310: 9c60 0165 92aa 6bd6 2972 9708 2b65 f7f1  .`.e..k.)r..+e..
-00001320: 946d b067 6f71 8278 1628 8911 dfa4 f91a  .m.goq.x.(......
-00001330: 44dd 4a5d 38e5 9c54 7a9d 8e0e 4de0 3502  D.J]8..Tz...M.5.
-00001340: e51f e48b d329 d705 e830 92bb bf49 eb8d  .....)...0...I..
-00001350: 0859 6797 7a16 ee7c 5d70 2b7e 6fb3 c760  .Yg.z..|]p+~o..`
-00001360: 5fde 3ded be04 197c 6a19 20f6 b7f6 cd10  _.=....|j. .....
-00001370: 516b 823c 6186 080a 0c17 dd82 8815 fe5c  Qk.<a..........\
-00001380: 449d ab5a 6cee 949b d89b 360f 0314 4656  D..Zl.....6...FV
-00001390: bd13 93e4 8dc5 cf89 b227 fc77 ca1e 7701  .........'.w..w.
-000013a0: 7306 058f 5bf1 fb94 3a9b 2865 e744 81b3  s...[...:.(e.D..
-000013b0: 09f7 1f2c 6b7a 689e dcc0 7092 ac73 d679  ...,kzh...p..s.y
-000013c0: 5573 5ed5 f8ff fbaa 66d3 5e3e af65 ce6b  Us^.....f.^>.e.k
-000013d0: 99f3 5ac6 f5f6 f541 6a99 bc7c 81ca 26ef  ..Z....Aj..|..&.
-000013e0: f2e8 9e4f bcb1 e533 2194 eecb 05c5 bb42  ...O...3!......B
-000013f0: 777d 04bc d18c 0730 a8db 51ba 27b9 6a01  w}.....0..Q.'.j.
-00001400: ce22 f89a 3598 2cdc 9423 2de3 7126 3f27  ."..5.,..#-.q&?'
-00001410: 32da 8fd0 0c5a 4365 ddc0 9c8a 4cf5 5478  2....ZCe....L.Tx
-00001420: 3326 a063 a487 752b 159f d0ad fb4e f378  3&.c..u+.....N.x
-00001430: 8f8d d34e 67b9 acba 9aa9 0b05 92f9 7829  ...Ng.........x)
-00001440: 5c8d 4397 4aa6 e85a 3def dead d4eb 7ee8  \.C.J..Z=.....~.
-00001450: 5477 5997 0628 d9d3 1861 4c66 1b51 7518  TwY..(...aLf.Qu.
-00001460: 515f 0e42 145e 6784 5ed9 9958 d174 58d1  Q_.B.^g.^..X.tX.
-00001470: 50ea 97a1 5a46 71e5 0a30 6d15 1578 e5f6  P...ZFq..0m..x..
-00001480: e045 bde5 8741 da41 8666 1c94 e763 15a7  .E...A.A.f...c..
-00001490: b499 bc8c ae0a ce99 467a 9333 a999 0150  ........Fz.3...P
-000014a0: 622f 3320 8f74 53d9 ba71 796a 7569 aabd  b/3 .tS..qyjui..
-000014b0: 45a4 2d23 8c74 b38d 30d2 3082 17e1 2c3b  E.-#.t..0.0...,;
-000014c0: cd96 fb59 c6ba 9987 d432 4fb9 62b9 1b72  ...Y.....2O.b..r
-000014d0: 33ea 8d0f 116b 4522 27b8 8126 2653 d0c4  3....kE"'..&&S..
-000014e0: 3b6e f9b5 6a08 b72a 2334 6bf9 13e8 18c3  ;n..j..*#4k.....
-000014f0: d778 06b9 23d4 5b17 a253 b876 1949 9e6e  .x..#.[..S.v.I.n
-00001500: f877 6196 1917 b287 4494 3a5c 934e ca06  .wa.....D.:\.N..
-00001510: 3191 987b 94c4 2d5f 2d7f 950d 34d1 1ca2  1..{..-_-...4...
-00001520: 6d2b 5780 103e 5ae3 9a40 2b1f 9b71 1074  m+W..>Z..@+..q.t
-00001530: 3bc8 7832 c123 6986 dd18 519e 4e1f 81e1  ;.x2.#i...Q.N...
-00001540: 53ae 70fe aac5 df1d ac24 d91c c2bd 1f8d  S.p......$......
-00001550: 8fbd 033a e737 11a4 5858 2f2b 078e 8980  ...:.7..XX/+....
-00001560: 8b83 72ea cd31 819b b015 91e5 f977 e260  ..r..1.......w.`
-00001570: ca68 d7bc 8ad2 3994 8e23 3a8b 5076 a298  .h....9..#:.Pv..
-00001580: 649e c235 89ae ccd1 4f2b 1f18 4fd9 9ac1  d..5....O+..O...
-00001590: a1eb 2e3c 98aa 03f6 bd4f dd37 1fd5 ca73  ...<.....O.7...s
-000015a0: 0669 e667 a6c5 2aea d474 93e9 873b e40d  .i.g..*..t...;..
-000015b0: abf2 43d4 b22a a56e fd4e 2d72 ae6b 2eb9  ..C..*.n.N-r.k..
-000015c0: 0e12 d579 4abc e1d4 7d8b 03c1 302d 9fcc  ...yJ...}...0-..
-000015d0: 324d 59bc 4ec3 8ab3 b351 dbb4 332c 080c  2MY.N....Q..3,..
-000015e0: 4fd4 36f8 6d75 4638 3df1 ae27 3fc8 9dcc  O.6.muF8=..'?...
-000015f0: 5a75 402c eb4a 9df8 faca dcbc d566 0777  Zu@,.J.......f.w
-00001600: 813c 7a70 7f38 a752 e850 426f 9723 28fa  .<zp.8.R.PBo.#(.
-00001610: d21b c894 3660 8bdc 9359 8d08 dfbc 3927  ....6`...Y....9'
-00001620: 2dff 7e29 6c07 dd4a d82d 941a 61bf 1054  -.~)l..J.-..a..T
-00001630: 8352 a111 b6ab 8576 1856 cbfd b05c ea75  .R.....v.V...\.u
-00001640: 2a0f e060 9151 5c0e d3eb fa01 5c61 d045  *..`.Q\.....\a.E
-00001650: 7669 afc7 d72e eee3 e52d cd85 118b 8b4c  vi.......-.....L
-00001660: 5fcc 17b5 e1fa e2be 5cd9 7c71 ef11 209d  _.......\.|q.. .
-00001670: fbb5 caa0 596d 766a 8566 b53d 2804 bd4e  ....Ymvj.f.=(..N
-00001680: a3d0 ecd6 3a85 5ead 5bef 0d7a ddb0 d11c  ....:.^.[..z....
-00001690: 3cf0 bd23 0d0e dad5 6e50 eb37 0ab5 72b7  <..#....nP.7..r.
-000016a0: 5b08 6a25 657e a359 a807 954a 3ba8 b71b  [.j%e~.Y...J;...
-000016b0: fda0 fd20 2b63 60e5 297d 64be 00f7 6abb  ... +c`.)}d...j.
-000016c0: b6ff 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
-000016d0: 0008 0000 0021 0079 a180 6ca4 0200 0052  .....!.y..l....R
-000016e0: 0600 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
-000016f0: 2e78 6d6c a455 6d6b db30 10fe 3ed8 7f10  .xml.Umk.0..>...
-00001700: faee ca76 e32c 09b6 cbd2 d450 e8c6 a01d  ...v.,.....P....
-00001710: ecab 62cb 89a8 5e8c 2467 cec6 fefb 4e76  ..b...^.$g....Nv
-00001720: 5e1c 3ab6 d17e 894e e7d3 73cf dd73 52d2  ^.:..~.N..s..sR.
-00001730: 9b4e 0ab4 63c6 72ad 321c 5d85 1831 55ea  .N..c.r.2.]..1U.
-00001740: 8aab 4d86 bf3e 15c1 0c23 eba8 aaa8 d08a  ..M..>...#......
-00001750: 6578 cf2c bec9 dfbf 4bad db0b f6b8 65cc  ex.,....K.....e.
-00001760: 2180 5036 c35b e79a 0521 b6dc 3249 ed95  !.P6.[...!..2I..
-00001770: 6e98 822f b536 923a d89a 0db1 8d61 b4b2  n../.6.:.....a..
-00001780: fe90 1424 0ec3 2991 942b 3c20 2c64 f93f  ...$..)..+< ,d.?
-00001790: 2092 9ae7 b609 4a2d 1bea f89a 0bee f63d   .....J-.......=
-000017a0: 1646 b25c dc6f 9436 742d 806a 174d 6889  .F.\.o.6t-.j.Mh.
-000017b0: ba68 6a62 d499 6392 defb 228f e4a5 d156  .hjb..c..."....V
-000017c0: d7ee 0a70 89ae 6b5e b297 74e7 644e 6879  ...p..k^..t.dNhy
-000017d0: 4602 e4d7 2145 0909 e38b da3b f34a a409  F...!E.....;.J..
-000017e0: 316c c7bd 7c38 4f6b ad9c 45a5 6e95 0331  1l..|8Ok..E.n..1
-000017f0: 81a8 6fc1 e259 e9ef aaf0 9fbc 7388 ca53  ..o..Y......s..S
-00001800: fb03 eda8 004f 8449 9e96 5a68 831c 4807  .....O.I..Zh..H.
-00001810: 9deb 3d8a 4a36 44dc 52c1 d786 fbb0 9a4a  ..=.J6D.R......J
-00001820: 2ef6 833b f68e 5eed 439c e4d0 7bef 249e  ...;..^.C...{.$.
-00001830: c761 b170 880b 7162 157b 02e0 c853 90cf  .a.p..qb.{...S..
-00001840: 31a3 0ad8 a083 fdb4 6f20 bd82 491b 60fa  1.......o ..I.`.
-00001850: b87f 446f 0cdd 4771 323a 40fa 8479 bad6  ..Do..Gq2:@..y..
-00001860: a682 c93e f7e3 e8ca 53c1 6a07 440d df6c  ...>....S.j.D..l
-00001870: fdea 7403 bf6b ed1c a89f a715 a71b ada8  ..t..k..........
-00001880: f0a5 0c20 2703 ca29 9910 8f7e fabf d517  ... '..)...~....
-00001890: d85d 8d54 2b0b e9ee ab0c c33d f24d 389a  .].T+......=.M8.
-000018a0: 50c8 c11c f086 8dc7 1fa3 0dd8 6f86 455d  P...........o.E]
-000018b0: 7d89 0f88 23da 17a4 4fe9 91d7 3bc3 9ffd  }...#...O...;...
-000018c0: 7515 3039 0708 b46e b970 5cfd 8130 6056  u.09...n.p\..0`V
-000018d0: ddb9 05a1 57c0 f9ab d737 e794 053a 51b1  ....W....7...:Q.
-000018e0: 9ab6 c23d 9d3e 66f8 6c7f 6215 6f65 7c8a  ...=.>f.l.b.oe|.
-000018f0: fac2 77da f510 193e db0f 5ea9 68ea 73b0  ..w....>..^.h.s.
-00001900: ce3d 5818 2f58 516b 7886 7fde 2d3f cc57  .=X./XQkx...-?.W
-00001910: 7745 1ccc c2e5 2c98 5cb3 2498 27cb 5590  wE....,.\.$.'.U.
-00001920: 4c6e 97ab 5531 0fe3 f0f6 d7e8 0178 c3f5  Ln..U1.......x..
-00001930: efdf ab3c 858b b5b0 021e 0973 28f6 50e2  ...<.......s(.P.
-00001940: e3d9 97e1 d166 a0df cf28 d01e 739f c7d3  .....f...(..s...
-00001950: f063 1285 4171 1d46 c164 4a67 c16c 7a9d  .c..Aq.F.dJg.lz.
-00001960: 0445 12c5 abe9 6479 9714 c988 7bf2 ca67  .E....dy....{..g
-00001970: 2224 5134 3c38 9e7c b270 5c32 c1d5 51ab  "$Q4<8.|.p\2..Q.
-00001980: a342 632f 8804 dbbf 1441 8e4a 90f3 9f41  .Bc/.....A.J...A
-00001990: fe1b 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-000019a0: 0800 0000 2100 7155 f0bf ac00 0000 e600  ....!.qU........
-000019b0: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-000019c0: 7472 696e 6773 2e78 6d6c 6c8e c10a c230  trings.xmll....0
-000019d0: 1044 ef82 ff10 f66e 5315 4424 490f 8a27  .D.....nS.D$I..'
-000019e0: 8ffa 01a1 5ddb 40b3 89dd ade8 df5b 41f1  ....].@......[A.
-000019f0: e271 de9b 8131 d523 f6ea 8e03 8744 1696  .q...1.#.....D..
-00001a00: 4509 0aa9 4e4d a0d6 c2e5 7c5c 6c41 b178  E...NM....|\lA.x
-00001a10: 6a7c 9f08 2d3c 91a1 72f3 9961 1635 6d89  j|..-<..r..a.5m.
-00001a20: 2d74 2279 a735 d71d 46cf 45ca 4893 b9a6  -t"y.5..F.E.H...
-00001a30: 217a 99e2 d06a ce03 fa86 3b44 89bd 5e95  !z...j....;D..^.
-00001a40: e546 471f 0854 9d46 120b 6b50 2385 db88  .FG..T.F..kP#...
-00001a50: fb6f 7686 8333 e24e 5e82 8c0d 1a2d cee8  .ov..3.N^....-..
-00001a60: 37fb f044 ed5f 71c0 2cdd afad a79f ee05  7..D._q.,.......
-00001a70: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001a80: 0000 2100 3b6d 324b c100 0000 4201 0000  ..!.;m2K....B...
-00001a90: 2300 0000 786c 2f77 6f72 6b73 6865 6574  #...xl/worksheet
-00001aa0: 732f 5f72 656c 732f 7368 6565 7431 2e78  s/_rels/sheet1.x
-00001ab0: 6d6c 2e72 656c 7384 8fc1 8ac2 3014 45f7  ml.rels.....0.E.
-00001ac0: 03fe 4378 7b93 d685 0c43 5337 22b8 55e7  ..Cx{....CS7".U.
-00001ad0: 0362 fada 06db 9790 f714 fd7b b31c 65c0  .b.........{..e.
-00001ae0: e5e5 70cf e536 9bfb 3ca9 1b66 0e91 2cd4  ..p..6..<..f..,.
-00001af0: ba02 85e4 6317 68b0 f07b da2d bf41 b138  ....c.h..{.-.A.8
-00001b00: eadc 1409 2d3c 9061 d32e be9a 034e 4e4a  ....-<.a.....NNJ
-00001b10: 89c7 9058 150b b185 5124 fd18 c37e c4d9  ...X....Q$...~..
-00001b20: b18e 09a9 903e e6d9 4989 7930 c9f9 8b1b  .....>..I.y0....
-00001b30: d0ac aa6a 6df2 5f07 b42f 4eb5 ef2c e47d  ...jm._../N..,.}
-00001b40: 5783 3a3d 5259 feec 8e7d 1f3c 6ea3 bfce  W.:=RY...}.<n...
-00001b50: 48f2 cf84 4939 9060 3ea2 4839 c845 edf2  H...I9.`>.H9.E..
-00001b60: 8062 41eb 77f6 9e6b 7d0e 04a6 6dcc cbf3  .bA.w..k}...m...
-00001b70: f609 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00001b80: 0800 0000 2100 5e39 c135 e802 0000 0021  ....!.^9.5.....!
-00001b90: 0000 2700 0000 786c 2f70 7269 6e74 6572  ..'...xl/printer
-00001ba0: 5365 7474 696e 6773 2f70 7269 6e74 6572  Settings/printer
-00001bb0: 5365 7474 696e 6773 312e 6269 6e0a 6008  Settings1.bin.`.
-00001bc0: 62f0 64f0 6308 6170 6670 6508 0642 0506  b.d.c.apfpe..B..
-00001bd0: 0d06 0f86 0020 edcc 90cf 9003 c445 40b6  ..... .......E@.
-00001be0: 0f43 2243 3143 2a90 ed05 244b 8022 be0c  .C"C1C*...$K."..
-00001bf0: 20c0 c8c2 cc76 8741 45c1 f97f 033b 2303   ....v.AE....;#.
-00001c00: 23c3 2bae 7c8e 1420 cdcf 10c1 c404 a423  #.+.|.. .......#
-00001c10: 9898 81a4 0f58 4f09 583f 581b 4504 2354  .....XO.X?X.E.#T
-00001c20: 3788 6602 626d 20e3 3f10 a01b eae2 e917  7.f.bm .?.......
-00001c30: aac4 f080 d386 e785 f0aa 97eb b7e1 b314  ................
-00001c40: e21b 6c2a 40b6 c06c 4495 6765 6066 6001  ..l*@..lD.ge`f`.
-00001c50: 6316 204d 1e00 8519 0252 1e36 a326 901f  c. M.....R.6.&..
-00001c60: 02d8 6319 bb79 0f38 1918 827d 43bc 40b2  ..c..y.8...}C.@.
-00001c70: 020c 1780 bc51 301a 02a3 2130 1a02 a321  .....Q0...!0...!
-00001c80: 301a 02a3 2130 1a02 a321 3094 43e0 8530  0...!0...!0.C..0
-00001c90: 0383 6768 8087 12b0 755e 31e7 edcd b35e  ..gh....u^1....^
-00001ca0: 4c81 126c 0fca 8d9c 6e89 6cc9 5176 cc6d  L..l....n.l.Qv.m
-00001cb0: 0a73 0e71 337c 39e5 d2fd 14c7 ee2c c5cc  .s.q3|9......,..
-00001cc0: 940c e1ac 979b c404 ef3a 4d0f 307f b889  .........:M.0...
-00001cd0: 3b43 3a77 b176 4668 6dba 4cf6 05b5 6897  ;C:w.vFhm.L...h.
-00001ce0: 45fb ce3f fc31 d7d2 f8b8 a484 4dbd 1d3f  E..?.1......M..?
-00001cf0: 63e0 e5ae 5e07 67df fe27 eb95 151e 6866  c...^.g..'....hf
-00001d00: 4f0a 3a97 fee0 b395 68f8 04b7 c020 a9ca  O.:.....h.... ..
-00001d10: 1f17 3f5c ca67 6f2c e7bf baef fcf6 a3ef  ..?\.go,........
-00001d20: 334b 2f9e 9f7d 27f8 a840 5901 4f74 9154  3K/..}'..@Y.Ot.T
-00001d30: 757d 417d 967e cd7f 97bb ded3 7376 3ebd  u}A}.~......sv>.
-00001d40: 3523 7065 88dd e3c0 051b 7b9f 3d0b 393c  5#pe......{.=.9<
-00001d50: f3f3 cfb4 ef9f a5a7 ff79 75f5 c68e 2e09  .........yu.....
-00001d60: 1f09 8f04 5fa5 d2f9 9195 bf97 1bad de34  ...._..........4
-00001d70: d139 2889 edf7 8cec afce 81ec 176a 4e7d  .9(..........jN}
-00001d80: 0db1 3751 28bc b3f7 4474 5df9 f34b f7aa  ..7Q(...Dt]..K..
-00001d90: de57 eadb 469c 7571 71b1 5fd9 ab6c 2973  .W..F.uqq._..l)s
-00001da0: 8acb b673 cfe6 2075 a545 6181 d5f2 5955  ...s.. u.Ea...YU
-00001db0: f99e fd73 26da edec 9870 65e5 a799 9bbf  ...s&....pe.....
-00001dc0: cb4f fa77 cbed e04a fb09 9356 793e 7209  .O.w...J...Vy>r.
-00001dd0: ba16 b937 2c7c a38b cb5b dfbf ef57 7e73  ...7,|...[...W~s
-00001de0: e052 bf39 2976 d615 f54b a9e9 5dab fe3a  .R.9)v...K..]..:
-00001df0: afbb 9f9f b9ed ffa7 af17 f6ae b04d 6631  .............Mf1
-00001e00: be71 d4ec 5184 b3c8 eba0 5b53 1e37 5d0e  .q..Q.....[S.7].
-00001e10: 9fbe e4bd 5ea2 9095 da92 78fd e277 772f  ....^.....x..ww/
-00001e20: ee38 f52a cffb d369 75a5 555d d16e 2ab3  .8.*...iu.U].n*.
-00001e30: 6ef4 e5e9 4946 0b1e eee2 6f7f 2fb6 fe4b  n...IF....o./..K
-00001e40: fae7 470f 33b3 3294 f7dc b9a0 50fc b9c2  ..G.3.2.....P...
-00001e50: f25b 565c ff3e 9ffb 7cd3 deeb 662b a6cd  .[V\.>..|...f+..
-00001e60: e07c 3d7b bd9a 1204 64bd 62fe f52f effb  .|={....d.b../..
-00001e70: 6866 1c0d 81d1 1018 0d81 d110 180d 81d1  hf..............
-00001e80: 1018 0d81 d110 180d 81d1 1018 0d81 d110  ................
-00001e90: 180d 81d1 1018 0d81 d110 18a1 2100 0000  ............!...
-00001ea0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001eb0: 0021 00d0 818c cd44 0100 0069 0200 0011  .!.....D...i....
-00001ec0: 0008 0164 6f63 5072 6f70 732f 636f 7265  ...docProps/core
-00001ed0: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
-00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000bc0: 0000 ac52 4d4b c430 10bd 0bfe 8730 779b  ...RMK.0.....0w.
+00000bd0: 7615 11d9 742f 22ec 55eb 0f08 c9b4 29db  v...t/".U.....).
+00000be0: 2621 337e f4df 1b2a ba5d 58d6 4b2f 036f  &!3~...*.]X.K/.o
+00000bf0: 8679 efcd c776 f735 0ee2 0313 f5c1 2ba8  .y...v.5......+.
+00000c00: 8a12 047a 136c ef3b 056f cdf3 cd03 0862  ...z.l.;.o.....b
+00000c10: edad 1e82 4705 1312 ecea ebab ed0b 0e9a  ....G...........
+00000c20: 7313 b93e 92c8 2c9e 1438 e6f8 2825 1987  s..>..,..8..(%..
+00000c30: a3a6 2244 f4b9 d286 346a ce30 7532 6a73  .."D....4j.0u2js
+00000c40: d01d ca4d 59de cbb4 e480 fa84 53ec ad82  ...MY.......S...
+00000c50: b4b7 b720 9a29 66e5 ffb9 43db f606 9f82  ... .)f...C.....
+00000c60: 791f d1f3 1909 493c 0d79 00d1 e8d4 212b  y.....I<.y....!+
+00000c70: f8c1 45f6 08f2 bcfc 664d 79ce 6bc1 a3fa  ..E.....fMy.k...
+00000c80: 0ce5 1cab 4b1e aa35 3d7c 8674 2087 c847  ....K..5=|.t ..G
+00000c90: 1f7f 2992 73e5 a299 bb55 efe1 7442 fbca  ..).s....U..tB..
+00000ca0: 29bf dbf2 2ccb f4ef 66e4 c9c7 d5df 0000  )...,...f.......
+00000cb0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00000cc0: 0021 00e2 1e79 58df 0200 0013 0600 0018  .!...yX.........
+00000cd0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00000ce0: 2f73 6865 6574 312e 786d 6c9c 925d 8fa2  /sheet1.xml..]..
+00000cf0: 3014 86ef 37d9 ffd0 f41e cad7 b84a c489  0...7........J..
+00000d00: 8a66 e66e b35f f7b5 1ca4 91b6 4c5b bfb2  .f.n._......L[..
+00000d10: d9ff be07 8cce 24de 9849 2039 94f2 3ce7  ......$..I 9..<.
+00000d20: d077 fa7c 522d 3980 75d2 e882 c661 4409  .w.|R-9.u....aD.
+00000d30: 6861 2aa9 b705 fdfd 6b1d 8c29 719e eb8a  ha*.....k..)q...
+00000d40: b746 4341 cfe0 e8f3 eceb 97e9 d1d8 9d6b  .FCA...........k
+00000d50: 003c 4182 7605 6dbc ef72 c69c 6840 7117  .<A.v.m..r..h@q.
+00000d60: 9a0e 34be a98d 55dc e3a3 dd32 d759 e0d5  ..4...U....2.Y..
+00000d70: f091 6a59 1245 23a6 b8d4 f442 c8ed 230c  ..jY.E#....B..#.
+00000d80: 53d7 5240 69c4 5e81 f617 8885 967b ecdf  S.R@i.^......{..
+00000d90: 35b2 7357 9a12 8fe0 14b7 bb7d 1708 a33a  5.sW.......}...:
+00000da0: 446c 642b fd79 8052 a244 feba d5c6 f24d  Dld+.y.R.D.....M
+00000db0: 8b73 9fe2 8c0b 72b2 7825 78a7 57cd b07e  .s....r.x%x.W..~
+00000dc0: 6752 5258 e34c ed43 24b3 4bcf f7e3 4fd8  gRRX.L.C$.K...O.
+00000dd0: 8471 7123 ddcf ff10 26ce 9885 83ec 0ff0  .qq#....&.......
+00000de0: 1d95 7cae a5f8 e9c6 4ade 61e9 2761 a31b  ..|.....J.a.'a..
+00000df0: acff 5d36 dfcb aaa0 7f47 ab45 b42e 27e3  ..]6.....G.E..'.
+00000e00: 60b9 8ad2 205b aebe 058b f16a 12c4 59b2  `... [.....j..Y.
+00000e10: 7e5a cce7 d928 8dff d1d9 b492 78c2 fd54  ~Z...(......x..T
+00000e20: c442 5dd0 799c 9729 65b3 e990 9f3f 128e  .B].y..)e....?..
+00000e30: ee43 4d3c dffc 8416 8407 74c4 94f4 f1dc  .CM<......t.....
+00000e40: 18b3 eb37 bee2 5284 4437 6ce8 895c 7879  ...7..R.D7l..\xy
+00000e50: 8025 b46d 41cb 0c13 fe36 38b0 4401 bb19  .%.mA....68.D...
+00000e60: 3ed6 57db 7a08 f477 4b2a a8f9 bef5 3fcc  >.W.z..wK*....?.
+00000e70: f105 e4b6 f1a8 cd42 640d 89c8 ab73 094e  .......Bd....s.N
+00000e80: 6044 511d f67d ff07 0000 ffff 0000 00ff  `DQ..}..........
+00000e90: ff94 924d 0e83 2010 46af 62d8 0b83 f81f  ...M.. .F.b.....
+00000ea0: 2469 e522 8492 7465 1b31 b6bd 7d51 1a45  $i."..te.1..}Q.E
+00000eb0: ba72 5630 ef4b 7833 81db bb31 9354 9312  .rV0.Kx3...1.T..
+00000ec0: 7c7c bc92 b143 1425 f6a9 06eb 4e6d 8e92  ||...C.%....Nm..
+00000ed0: 37cd 956e 6f1f 69ac 36c3 d421 c00c 09ae  7..no.i.6..!....
+00000ee0: 97e8 c565 5dc7 bafb 2c80 9359 70a2 7fec  ...e]...,..Yp...
+00000ef0: 1a32 7a64 7dc8 b223 9321 631b 23ce 6e53  .2zd}..#.!c.#.nS
+00000f00: cc4e 2866 ab5c 5a60 a858 1354 1de9 fa1c  .N(f.\Z`.X.T....
+00000f10: 0586 a1de 9f5d c7ec 3d2b 0017 91ab 0765  .....]..=+.....e
+00000f20: d03f 78b2 139e cb52 6791 520c 10ab 79d4  .?x....Rg.R...y.
+00000f30: d4b8 cc69 3041 192d d5c7 6885 4b08 2bda  ...i0A.-..h.K.+.
+00000f40: bdf4 b17f 67b2 7f85 2f00 0000 ffff 0000  ....g.../.......
+00000f50: 00ff ff34 8dc1 0ac2 3010 447f 25ec 0758  ...4....0.D.%..X
+00000f60: 4544 90a6 770f 9efc 8295 6c93 45cd 86ed  ED..w.....l.E...
+00000f70: 88bf 6f2b e436 6f78 cc8c 8db3 dcd8 b3d6  ..o+.6ox........
+00000f80: 25bc 6446 a4fd ee4c c135 979e 61ed df9e  %.dF...L.5..a...
+00000f90: 283c 0cb0 77a7 229c c437 3a52 98cd d061  (<..w."..7:R...a
+00000fa0: 98c6 6df7 2ef8 b460 ae52 c150 ab91 9a39  ..m....`.R.P...9
+00000fb0: 9c15 ebc3 4553 24bf a603 adfa f035 7f2e  ....ES$......5..
+00000fc0: 4504 d30f 0000 ffff 0300 504b 0304 1400  E.........PK....
+00000fd0: 0600 0800 0000 2100 c117 10be 4e07 0000  ......!.....N...
+00000fe0: c620 0000 1300 0000 786c 2f74 6865 6d65  . ......xl/theme
+00000ff0: 2f74 6865 6d65 312e 786d 6cec 59cd 8b1b  /theme1.xml.Y...
+00001000: 3714 bf17 fa3f 0c73 77fc 35e3 8f25 dee0  7....?.sw.5..%..
+00001010: cf6c 93dd 2464 9d94 1cb5 b6ec 5156 3332  .l..$d......QV32
+00001020: 92bc 1b13 0225 39f5 5228 a4a5 9742 6f3d  .....%9.R(...Bo=
+00001030: 94d2 4003 0dbd f48f 0924 b4e9 1fd1 27cd  ..@......$....'.
+00001040: d823 ade5 249b 6c4a 5a76 0d8b 47fe bda7  .#..$.lJZv..G...
+00001050: a7f7 9e7e 7af3 74f1 d2bd 987a 4798 0bc2  ...~z.t....zG...
+00001060: 9296 5fbe 50f2 3d9c 8cd8 9824 d396 7f6b  .._.P.=....$...k
+00001070: 3828 347c 4f48 948c 1165 096e f90b 2cfc  8(4|OH...e.n..,.
+00001080: 4bdb 9f7e 7211 6dc9 08c7 d803 f944 6ca1  K..~r.m......Dl.
+00001090: 961f 4939 db2a 16c5 0886 91b8 c066 3881  ..I9.*.......f8.
+000010a0: df26 8cc7 48c2 239f 16c7 1c1d 83de 9816  .&..H.#.........
+000010b0: 2ba5 52ad 1823 92f8 5e82 6250 7b7d 3221  +.R..#..^.bP{}2!
+000010c0: 23ec 0d95 4a7f 7ba9 bc4f e131 9142 0d8c  #...J.{..O.1.B..
+000010d0: 28df 57aa b125 a1b1 e3c3 b242 8885 e852  (.W..%.....B...R
+000010e0: ee1d 21da f261 9e31 3b1e e27b d2f7 2812  ..!..a.1;..{..(.
+000010f0: 127e 68f9 25fd e717 b72f 16d1 5626 44e5  .~h.%..../..V&D.
+00001100: 0659 436e a0ff 32b9 4c60 7c58 d173 f2e9  .YCn..2.L`|X.s..
+00001110: c16a d220 0883 5a7b a55f 03a8 5cc7 f5eb  .j. ..Z{._..\...
+00001120: fd5a bfb6 d2a7 0168 3482 95a6 b6d8 3aeb  .Z.....h4.....:.
+00001130: 956e 9061 0d50 fad5 a1bb 57ef 55cb 16de  .n.a.P....W.U...
+00001140: d05f 5db3 b91d aa8f 85d7 a054 7fb0 861f  ._]........T....
+00001150: 0cba e045 0baf 4129 3e5c c387 9d66 a767  ...E..A)>\...f.g
+00001160: ebd7 a014 5f5b c3d7 4bed 5e50 b7f4 6b50  ...._[..K.^P..kP
+00001170: 4449 72b8 862e 85b5 6a77 b9da 1564 c2e8  DIr.....jw...d..
+00001180: 8e13 de0c 8341 bd92 29cf 5190 0dab ec52  .....A..).Q....R
+00001190: 534c 5822 37e5 5a8c ee32 3e00 8002 5224  SLX"7.Z..2>...R$
+000011a0: 49e2 c9c5 0c4f d008 b2b8 8b28 39e0 c4db  I....O.....(9...
+000011b0: 25d3 0812 6f86 1226 60b8 5429 0d4a 55f8  %...o..&`.T).JU.
+000011c0: af3e 81fe a623 8ab6 3032 a495 5d60 8958  .>...#..02..]`.X
+000011d0: 1b52 f678 62c4 c94c b6fc 2ba0 d537 202f  .R.xb..L..+..7 /
+000011e0: 9e3d 7bfe f0e9 f387 bf3d 7ff4 e8f9 c35f  .={......=....._
+000011f0: b2b9 b52a 4b6e 0725 5353 eed5 8f5f fffd  ...*Kn.%SS..._..
+00001200: fd17 de5f bffe f0ea f137 e9d4 27f1 c2c4  ..._.....7..'...
+00001210: bffc f9cb 97bf fff1 3af5 b0e2 dc15 2fbe  ........:...../.
+00001220: 7df2 f2e9 9317 df7d f5e7 4f8f 1dda db1c  }......}..O.....
+00001230: 1d98 f021 89b1 f0ae e163 ef26 8b61 810e  ...!.....c.&.a..
+00001240: fbf1 013f 9dc4 3042 c492 4011 e876 a8ee  ...?..0B..@..v..
+00001250: cbc8 025e 5b20 eac2 75b0 edc2 db1c 58c6  ...^[ ..u.....X.
+00001260: 05bc 3cbf 6bd9 ba1f f1b9 248e 99af 46b1  ..<.k.....$...F.
+00001270: 05dc 638c 7618 773a e0aa 9acb f0f0 709e  ..c.v.w:......p.
+00001280: 4cdd 93f3 b989 bb89 d091 6bee 2e4a ac00  L.........k..J..
+00001290: f7e7 33a0 57e2 52d9 8db0 65e6 0d8a 1289  ..3.W.R...e.....
+000012a0: a638 c1d2 53bf b143 8c1d abbb 4388 e5d7  .8..S..C....C...
+000012b0: 3d32 e24c b089 f4ee 10af 8388 d325 4372  =2.L.........%Cr
+000012c0: 6025 522e b443 6288 cbc2 6520 84da f2cd  `%R..Cb...e ....
+000012d0: de6d afc3 a86b d53d 7c64 2361 5b20 ea30  .m...k.=|d#a[ .0
+000012e0: 7e88 a9e5 c6cb 682e 51ec 5239 4431 351d  ~.....h.Q.R9D15.
+000012f0: be8b 64e4 3272 7fc1 4726 ae2f 2444 7a8a  ..d.2r..G&./$Dz.
+00001300: 29f3 fa63 2c84 4be6 3a87 f51a 41bf 0a0c  )..c,.K.:...A...
+00001310: e30e fb1e 5dc4 3692 4b72 e8d2 b98b 1833  ....].6.Kr.....3
+00001320: 913d 76d8 8d50 3c73 da4c 92c8 c47e 260e  .=v..P<s.L...~&.
+00001330: 2145 9177 8349 177c 8fd9 3b44 3d43 1c50  !E.w.I.|..;D=C.P
+00001340: b231 dcb7 09b6 c2fd 6622 b805 e46a 9a94  .1......f"...j..
+00001350: 2788 fa65 ce1d b1bc 8c99 bd1f 1774 82b0  '..e.........t..
+00001360: 8b65 da3c b6d8 b5cd 8933 3b3a f3a9 95da  .e.<.....3;:....
+00001370: bb18 5374 8cc6 187b b73e 7358 d061 33cb  ..St...{.>sX.a3.
+00001380: e7b9 d157 2260 951d ec4a ac2b c8ce 55f5  ...W"`...J.+..U.
+00001390: 9c60 0165 92aa 6bd6 2972 9708 2b65 f7f1  .`.e..k.)r..+e..
+000013a0: 946d b067 6f71 8278 1628 8911 dfa4 f91a  .m.goq.x.(......
+000013b0: 44dd 4a5d 38e5 9c54 7a9d 8e0e 4de0 3502  D.J]8..Tz...M.5.
+000013c0: e51f e48b d329 d705 e830 92bb bf49 eb8d  .....)...0...I..
+000013d0: 0859 6797 7a16 ee7c 5d70 2b7e 6fb3 c760  .Yg.z..|]p+~o..`
+000013e0: 5fde 3ded be04 197c 6a19 20f6 b7f6 cd10  _.=....|j. .....
+000013f0: 516b 823c 6186 080a 0c17 dd82 8815 fe5c  Qk.<a..........\
+00001400: 449d ab5a 6cee 949b d89b 360f 0314 4656  D..Zl.....6...FV
+00001410: bd13 93e4 8dc5 cf89 b227 fc77 ca1e 7701  .........'.w..w.
+00001420: 7306 058f 5bf1 fb94 3a9b 2865 e744 81b3  s...[...:.(e.D..
+00001430: 09f7 1f2c 6b7a 689e dcc0 7092 ac73 d679  ...,kzh...p..s.y
+00001440: 5573 5ed5 f8ff fbaa 66d3 5e3e af65 ce6b  Us^.....f.^>.e.k
+00001450: 99f3 5ac6 f5f6 f541 6a99 bc7c 81ca 26ef  ..Z....Aj..|..&.
+00001460: f2e8 9e4f bcb1 e533 2194 eecb 05c5 bb42  ...O...3!......B
+00001470: 777d 04bc d18c 0730 a8db 51ba 27b9 6a01  w}.....0..Q.'.j.
+00001480: ce22 f89a 3598 2cdc 9423 2de3 7126 3f27  ."..5.,..#-.q&?'
+00001490: 32da 8fd0 0c5a 4365 ddc0 9c8a 4cf5 5478  2....ZCe....L.Tx
+000014a0: 3326 a063 a487 752b 159f d0ad fb4e f378  3&.c..u+.....N.x
+000014b0: 8f8d d34e 67b9 acba 9aa9 0b05 92f9 7829  ...Ng.........x)
+000014c0: 5c8d 4397 4aa6 e85a 3def dead d4eb 7ee8  \.C.J..Z=.....~.
+000014d0: 5477 5997 0628 d9d3 1861 4c66 1b51 7518  TwY..(...aLf.Qu.
+000014e0: 515f 0e42 145e 6784 5ed9 9958 d174 58d1  Q_.B.^g.^..X.tX.
+000014f0: 50ea 97a1 5a46 71e5 0a30 6d15 1578 e5f6  P...ZFq..0m..x..
+00001500: e045 bde5 8741 da41 8666 1c94 e763 15a7  .E...A.A.f...c..
+00001510: b499 bc8c ae0a ce99 467a 9333 a999 0150  ........Fz.3...P
+00001520: 622f 3320 8f74 53d9 ba71 796a 7569 aabd  b/3 .tS..qyjui..
+00001530: 45a4 2d23 8c74 b38d 30d2 3082 17e1 2c3b  E.-#.t..0.0...,;
+00001540: cd96 fb59 c6ba 9987 d432 4fb9 62b9 1b72  ...Y.....2O.b..r
+00001550: 33ea 8d0f 116b 4522 27b8 8126 2653 d0c4  3....kE"'..&&S..
+00001560: 3b6e f9b5 6a08 b72a 2334 6bf9 13e8 18c3  ;n..j..*#4k.....
+00001570: d778 06b9 23d4 5b17 a253 b876 1949 9e6e  .x..#.[..S.v.I.n
+00001580: f877 6196 1917 b287 4494 3a5c 934e ca06  .wa.....D.:\.N..
+00001590: 3191 987b 94c4 2d5f 2d7f 950d 34d1 1ca2  1..{..-_-...4...
+000015a0: 6d2b 5780 103e 5ae3 9a40 2b1f 9b71 1074  m+W..>Z..@+..q.t
+000015b0: 3bc8 7832 c123 6986 dd18 519e 4e1f 81e1  ;.x2.#i...Q.N...
+000015c0: 53ae 70fe aac5 df1d ac24 d91c c2bd 1f8d  S.p......$......
+000015d0: 8fbd 033a e737 11a4 5858 2f2b 078e 8980  ...:.7..XX/+....
+000015e0: 8b83 72ea cd31 819b b015 91e5 f977 e260  ..r..1.......w.`
+000015f0: ca68 d7bc 8ad2 3994 8e23 3a8b 5076 a298  .h....9..#:.Pv..
+00001600: 649e c235 89ae ccd1 4f2b 1f18 4fd9 9ac1  d..5....O+..O...
+00001610: a1eb 2e3c 98aa 03f6 bd4f dd37 1fd5 ca73  ...<.....O.7...s
+00001620: 0669 e667 a6c5 2aea d474 93e9 873b e40d  .i.g..*..t...;..
+00001630: abf2 43d4 b22a a56e fd4e 2d72 ae6b 2eb9  ..C..*.n.N-r.k..
+00001640: 0e12 d579 4abc e1d4 7d8b 03c1 302d 9fcc  ...yJ...}...0-..
+00001650: 324d 59bc 4ec3 8ab3 b351 dbb4 332c 080c  2MY.N....Q..3,..
+00001660: 4fd4 36f8 6d75 4638 3df1 ae27 3fc8 9dcc  O.6.muF8=..'?...
+00001670: 5a75 402c eb4a 9df8 faca dcbc d566 0777  Zu@,.J.......f.w
+00001680: 813c 7a70 7f38 a752 e850 426f 9723 28fa  .<zp.8.R.PBo.#(.
+00001690: d21b c894 3660 8bdc 9359 8d08 dfbc 3927  ....6`...Y....9'
+000016a0: 2dff 7e29 6c07 dd4a d82d 941a 61bf 1054  -.~)l..J.-..a..T
+000016b0: 8352 a111 b6ab 8576 1856 cbfd b05c ea75  .R.....v.V...\.u
+000016c0: 2a0f e060 9151 5c0e d3eb fa01 5c61 d045  *..`.Q\.....\a.E
+000016d0: 7669 afc7 d72e eee3 e52d cd85 118b 8b4c  vi.......-.....L
+000016e0: 5fcc 17b5 e1fa e2be 5cd9 7c71 ef11 209d  _.......\.|q.. .
+000016f0: fbb5 caa0 596d 766a 8566 b53d 2804 bd4e  ....Ymvj.f.=(..N
+00001700: a3d0 ecd6 3a85 5ead 5bef 0d7a ddb0 d11c  ....:.^.[..z....
+00001710: 3cf0 bd23 0d0e dad5 6e50 eb37 0ab5 72b7  <..#....nP.7..r.
+00001720: 5b08 6a25 657e a359 a807 954a 3ba8 b71b  [.j%e~.Y...J;...
+00001730: fda0 fd20 2b63 60e5 297d 64be 00f7 6abb  ... +c`.)}d...j.
+00001740: b6ff 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00001750: 0008 0000 0021 0079 a180 6ca4 0200 0052  .....!.y..l....R
+00001760: 0600 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+00001770: 2e78 6d6c a455 6d6b db30 10fe 3ed8 7f10  .xml.Umk.0..>...
+00001780: faee ca76 e32c 09b6 cbd2 d450 e8c6 a01d  ...v.,.....P....
+00001790: ecab 62cb 89a8 5e8c 2467 cec6 fefb 4e76  ..b...^.$g....Nv
+000017a0: 5e1c 3ab6 d17e 894e e7d3 73cf dd73 52d2  ^.:..~.N..s..sR.
+000017b0: 9b4e 0ab4 63c6 72ad 321c 5d85 1831 55ea  .N..c.r.2.]..1U.
+000017c0: 8aab 4d86 bf3e 15c1 0c23 eba8 aaa8 d08a  ..M..>...#......
+000017d0: 6578 cf2c bec9 dfbf 4bad db0b f6b8 65cc  ex.,....K.....e.
+000017e0: 2180 5036 c35b e79a 0521 b6dc 3249 ed95  !.P6.[...!..2I..
+000017f0: 6e98 822f b536 923a d89a 0db1 8d61 b4b2  n../.6.:.....a..
+00001800: fe90 1424 0ec3 2991 942b 3c20 2c64 f93f  ...$..)..+< ,d.?
+00001810: 2092 9ae7 b609 4a2d 1bea f89a 0bee f63d   .....J-.......=
+00001820: 1646 b25c dc6f 9436 742d 806a 174d 6889  .F.\.o.6t-.j.Mh.
+00001830: ba68 6a62 d499 6392 defb 228f e4a5 d156  .hjb..c..."....V
+00001840: d7ee 0a70 89ae 6b5e b297 74e7 644e 6879  ...p..k^..t.dNhy
+00001850: 4602 e4d7 2145 0909 e38b da3b f34a a409  F...!E.....;.J..
+00001860: 316c c7bd 7c38 4f6b ad9c 45a5 6e95 0331  1l..|8Ok..E.n..1
+00001870: 81a8 6fc1 e259 e9ef aaf0 9fbc 7388 ca53  ..o..Y......s..S
+00001880: fb03 eda8 004f 8449 9e96 5a68 831c 4807  .....O.I..Zh..H.
+00001890: 9deb 3d8a 4a36 44dc 52c1 d786 fbb0 9a4a  ..=.J6D.R......J
+000018a0: 2ef6 833b f68e 5eed 439c e4d0 7bef 249e  ...;..^.C...{.$.
+000018b0: c761 b170 880b 7162 157b 02e0 c853 90cf  .a.p..qb.{...S..
+000018c0: 31a3 0ad8 a083 fdb4 6f20 bd82 491b 60fa  1.......o ..I.`.
+000018d0: b87f 446f 0cdd 4771 323a 40fa 8479 bad6  ..Do..Gq2:@..y..
+000018e0: a682 c93e f7e3 e8ca 53c1 6a07 440d df6c  ...>....S.j.D..l
+000018f0: fdea 7403 bf6b ed1c a89f a715 a71b ada8  ..t..k..........
+00001900: f0a5 0c20 2703 ca29 9910 8f7e fabf d517  ... '..)...~....
+00001910: d85d 8d54 2b0b e9ee ab0c c33d f24d 389a  .].T+......=.M8.
+00001920: 50c8 c11c f086 8dc7 1fa3 0dd8 6f86 455d  P...........o.E]
+00001930: 7d89 0f88 23da 17a4 4fe9 91d7 3bc3 9ffd  }...#...O...;...
+00001940: 7515 3039 0708 b46e b970 5cfd 8130 6056  u.09...n.p\..0`V
+00001950: ddb9 05a1 57c0 f9ab d737 e794 053a 51b1  ....W....7...:Q.
+00001960: 9ab6 c23d 9d3e 66f8 6c7f 6215 6f65 7c8a  ...=.>f.l.b.oe|.
+00001970: fac2 77da f510 193e db0f 5ea9 68ea 73b0  ..w....>..^.h.s.
+00001980: ce3d 5818 2f58 516b 7886 7fde 2d3f cc57  .=X./XQkx...-?.W
+00001990: 7745 1ccc c2e5 2c98 5cb3 2498 27cb 5590  wE....,.\.$.'.U.
+000019a0: 4c6e 97ab 5531 0fe3 f0f6 d7e8 0178 c3f5  Ln..U1.......x..
+000019b0: efdf ab3c 858b b5b0 021e 0973 28f6 50e2  ...<.......s(.P.
+000019c0: e3d9 97e1 d166 a0df cf28 d01e 739f c7d3  .....f...(..s...
+000019d0: f063 1285 4171 1d46 c164 4a67 c16c 7a9d  .c..Aq.F.dJg.lz.
+000019e0: 0445 12c5 abe9 6479 9714 c988 7bf2 ca67  .E....dy....{..g
+000019f0: 2224 5134 3c38 9e7c b270 5c32 c1d5 51ab  "$Q4<8.|.p\2..Q.
+00001a00: a342 632f 8804 dbbf 1441 8e4a 90f3 9f41  .Bc/.....A.J...A
+00001a10: fe1b 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00001a20: 0800 0000 2100 567c f849 b200 0000 ff00  ....!.V|.I......
+00001a30: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
+00001a40: 7472 696e 6773 2e78 6d6c 6c8f c10a c230  trings.xmll....0
+00001a50: 1044 ef82 ff10 f66e 5345 4424 490f 8a27  .D.....nSED$I..'
+00001a60: bde9 0784 766d 03cd a676 b7a2 7f6f 05bd  ....vm...v...o..
+00001a70: 148f efcd cc61 4cf1 8cad 7a60 cf21 9185  .....aL...z`.!..
+00001a80: 6596 8342 2a53 15a8 b670 bd1c 175b 502c  e..B*S...p...[P,
+00001a90: 9e2a df26 420b 2f64 28dc 7c66 9845 8d5b  .*.&B./d(.|f.E.[
+00001aa0: 620b 8d48 b7d3 9acb 06a3 e72c 7548 6372  b..H.......,uHcr
+00001ab0: 4b7d f432 625f 6bee 7af4 1537 8812 5bbd  K}.2b_k.z..7..[.
+00001ac0: caf3 8d8e 3e10 a832 0d24 16d6 a006 0af7  ....>..2.$......
+00001ad0: 01f7 3f76 8683 33e2 4e5e 820c 151a 2dce  ..?v..3.N^....-.
+00001ae0: e88f fbfa 44f5 dfe0 809d 34d3 f6d9 d734  ....D.....4....4
+00001af0: 69eb f180 7b03 0000 ffff 0300 504b 0304  i...{.......PK..
+00001b00: 1400 0600 0800 0000 2100 3b6d 324b c100  ........!.;m2K..
+00001b10: 0000 4201 0000 2300 0000 786c 2f77 6f72  ..B...#...xl/wor
+00001b20: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
+00001b30: 6565 7431 2e78 6d6c 2e72 656c 7384 8fc1  eet1.xml.rels...
+00001b40: 8ac2 3014 45f7 03fe 4378 7b93 d685 0c43  ..0.E...Cx{....C
+00001b50: 5337 22b8 55e7 0362 fada 06db 9790 f714  S7".U..b........
+00001b60: fd7b b31c 65c0 e5e5 70cf e536 9bfb 3ca9  .{..e...p..6..<.
+00001b70: 1b66 0e91 2cd4 ba02 85e4 6317 68b0 f07b  .f..,.....c.h..{
+00001b80: da2d bf41 b138 eadc 1409 2d3c 9061 d32e  .-.A.8....-<.a..
+00001b90: be9a 034e 4e4a 89c7 9058 150b b185 5124  ...NNJ...X....Q$
+00001ba0: fd18 c37e c4d9 b18e 09a9 903e e6d9 4989  ...~.......>..I.
+00001bb0: 7930 c9f9 8b1b d0ac aa6a 6df2 5f07 b42f  y0.......jm._../
+00001bc0: 4eb5 ef2c e47d 5783 3a3d 5259 feec 8e7d  N..,.}W.:=RY...}
+00001bd0: 1f3c 6ea3 bfce 48f2 cf84 4939 9060 3ea2  .<n...H...I9.`>.
+00001be0: 4839 c845 edf2 8062 41eb 77f6 9e6b 7d0e  H9.E...bA.w..k}.
+00001bf0: 04a6 6dcc cbf3 f609 0000 ffff 0300 504b  ..m...........PK
+00001c00: 0304 1400 0600 0800 0000 2100 5e39 c135  ..........!.^9.5
+00001c10: e802 0000 0021 0000 2700 0000 786c 2f70  .....!..'...xl/p
+00001c20: 7269 6e74 6572 5365 7474 696e 6773 2f70  rinterSettings/p
+00001c30: 7269 6e74 6572 5365 7474 696e 6773 312e  rinterSettings1.
+00001c40: 6269 6e0a 6008 62f0 64f0 6308 6170 6670  bin.`.b.d.c.apfp
+00001c50: 6508 0642 0506 0d06 0f86 0020 edcc 90cf  e..B....... ....
+00001c60: 9003 c445 40b6 0f43 2243 3143 2a90 ed05  ...E@..C"C1C*...
+00001c70: 244b 8022 be0c 20c0 c8c2 cc76 8741 45c1  $K.".. ....v.AE.
+00001c80: f97f 033b 2303 23c3 2bae 7c8e 1420 cdcf  ...;#.#.+.|.. ..
+00001c90: 10c1 c404 a423 9898 81a4 0f58 4f09 583f  .....#.....XO.X?
+00001ca0: 581b 4504 2354 3788 6602 626d 20e3 3f10  X.E.#T7.f.bm .?.
+00001cb0: a01b eae2 e917 aac4 f080 d386 e785 f0aa  ................
+00001cc0: 97eb b7e1 b314 e21b 6c2a 40b6 c06c 4495  ........l*@..lD.
+00001cd0: 6765 6066 6001 6316 204d 1e00 8519 0252  ge`f`.c. M.....R
+00001ce0: 1e36 a326 901f 02d8 6319 bb79 0f38 1918  .6.&....c..y.8..
+00001cf0: 827d 43bc 40b2 020c 1780 bc51 301a 02a3  .}C.@......Q0...
+00001d00: 2130 1a02 a321 301a 02a3 2130 1a02 a321  !0...!0...!0...!
+00001d10: 3094 43e0 8530 0383 6768 8087 12b0 755e  0.C..0..gh....u^
+00001d20: 31e7 edcd b35e 4c81 126c 0fca 8d9c 6e89  1....^L..l....n.
+00001d30: 6cc9 5176 cc6d 0a73 0e71 337c 39e5 d2fd  l.Qv.m.s.q3|9...
+00001d40: 14c7 ee2c c5cc 940c e1ac 979b c404 ef3a  ...,...........:
+00001d50: 4d0f 307f b889 3b43 3a77 b176 4668 6dba  M.0...;C:w.vFhm.
+00001d60: 4cf6 05b5 6897 45fb ce3f fc31 d7d2 f8b8  L...h.E..?.1....
+00001d70: a484 4dbd 1d3f 63e0 e5ae 5e07 67df fe27  ..M..?c...^.g..'
+00001d80: eb95 151e 6866 4f0a 3a97 fee0 b395 68f8  ....hfO.:.....h.
+00001d90: 04b7 c020 a9ca 1f17 3f5c ca67 6f2c e7bf  ... ....?\.go,..
+00001da0: baef fcf6 a3ef 334b 2f9e 9f7d 27f8 a840  ......3K/..}'..@
+00001db0: 5901 4f74 9154 757d 417d 967e cd7f 97bb  Y.Ot.Tu}A}.~....
+00001dc0: ded3 7376 3ebd 3523 7065 88dd e3c0 051b  ..sv>.5#pe......
+00001dd0: 7b9f 3d0b 393c f3f3 cfb4 ef9f a5a7 ff79  {.=.9<.........y
+00001de0: 75f5 c68e 2e09 1f09 8f04 5fa5 d2f9 9195  u........._.....
+00001df0: bf97 1bad de34 d139 2889 edf7 8cec afce  .....4.9(.......
+00001e00: 81ec 176a 4e7d 0db1 3751 28bc b3f7 4474  ...jN}..7Q(...Dt
+00001e10: 5df9 f34b f7aa de57 eadb 469c 7571 71b1  ]..K...W..F.uqq.
+00001e20: 5fd9 ab6c 2973 8acb b673 cfe6 2075 a545  _..l)s...s.. u.E
+00001e30: 6181 d5f2 5955 f99e fd73 26da edec 9870  a...YU...s&....p
+00001e40: 65e5 a799 9bbf cb4f fa77 cbed e04a fb09  e......O.w...J..
+00001e50: 9356 793e 7209 ba16 b937 2c7c a38b cb5b  .Vy>r....7,|...[
+00001e60: dfbf ef57 7e73 e052 bf39 2976 d615 f54b  ...W~s.R.9)v...K
+00001e70: a9e9 5dab fe3a afbb 9f9f b9ed ffa7 af17  ..]..:..........
+00001e80: f6ae b04d 6631 be71 d4ec 5184 b3c8 eba0  ...Mf1.q..Q.....
+00001e90: 5b53 1e37 5d0e 9fbe e4bd 5ea2 9095 da92  [S.7].....^.....
+00001ea0: 78fd e277 772f ee38 f52a cffb d369 75a5  x..ww/.8.*...iu.
+00001eb0: 555d d16e 2ab3 6ef4 e5e9 4946 0b1e eee2  U].n*.n...IF....
+00001ec0: 6f7f 2fb6 fe4b fae7 470f 33b3 3294 f7dc  o./..K..G.3.2...
+00001ed0: b9a0 50fc b9c2 f25b 565c ff3e 9ffb 7cd3  ..P....[V\.>..|.
+00001ee0: deeb 662b a6cd e07c 3d7b bd9a 1204 64bd  ..f+...|={....d.
+00001ef0: 62fe f52f effb 6866 1c0d 81d1 1018 0d81  b../..hf........
+00001f00: d110 180d 81d1 1018 0d81 d110 180d 81d1  ................
+00001f10: 1018 0d81 d110 180d 81d1 1018 0d81 d110  ................
+00001f20: 18a1 2100 0000 00ff ff03 0050 4b03 0414  ..!........PK...
+00001f30: 0006 0008 0000 0021 00b1 7bf0 024d 0100  .......!..{..M..
+00001f40: 0069 0200 0011 0008 0164 6f63 5072 6f70  .i.......docProp
+00001f50: 732f 636f 7265 2e78 6d6c 20a2 0401 28a0  s/core.xml ...(.
+00001f60: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fd0: 0000 0000 0000 0000 0000 0000 8c92 514b  ..............QK
-00001fe0: c330 1485 df05 ff43 c9b3 5dda 14e6 0c6d  .0.....C..]....m
-00001ff0: 072a c307 0782 13c5 b790 dc6d 614d 1a92  .*.........maM..
-00002000: 68b7 7f6f da6e b53a 1f7c 4cce b95f ceb9  h..o.n.:.|L.._..
-00002010: 249f ef55 157d 8275 b2d6 054a 2709 8a40  $..U.}.u...J'..@
-00002020: f35a 48bd 29d0 cb6a 11cf 50e4 3cd3 8255  .ZH.)..j..P.<..U
-00002030: b586 021d c0a1 7979 7991 7343 796d e1c9  ......yyy.sCym..
-00002040: d606 ac97 e0a2 40d2 8e72 53a0 adf7 8662  ......@..rS....b
-00002050: ecf8 1614 7393 e0d0 415c d756 311f 8e76  ....s...A\.V1..v
-00002060: 830d e33b b601 4c92 648a 1578 2698 67b8  ...;..L.d..x&.g.
-00002070: 05c6 6620 a223 52f0 0169 3e6c d501 04c7  ..f .#R..i>l....
-00002080: 5081 02ed 1d4e 2729 fef6 7ab0 cafd 39d0  P....N')..z...9.
-00002090: 2923 a792 fe60 42a7 63dc 315b f05e 1cdc  )#...`B.c.1[.^..
-000020a0: 7b27 0763 d334 9326 eb62 84fc 297e 5b3e  {'.c.4.&.b..)~[>
-000020b0: 3e77 5563 a9db 5d71 4065 2e38 e516 98af  >wUc..]q@e.8....
-000020c0: 6df9 00cc 6ab8 8a96 7207 391e 09ed 122b  m...j...r.9....+
-000020d0: e6fc 32ec 7b2d 41dc 1e7e 79cf f5c0 ed6a  ..2.{-A..~y....j
-000020e0: f470 1051 0846 fb1a 27e5 35bb bb5f 2d50  .p.Q.F..'.5.._-P
-000020f0: 4912 42e2 e426 4ec8 8a10 9a5d 5392 bdb7  I.B..&N....]S...
-00002100: cfff 986f 83f6 17ea 18e2 ffc4 194d a623  ...o.........M.#
-00002110: e209 50e6 f8ec 7394 5f00 0000 ffff 0300  ..P...s._.......
-00002120: 504b 0304 1400 0600 0800 0000 2100 6149  PK..........!.aI
-00002130: 0910 8901 0000 1103 0000 1000 0801 646f  ..............do
-00002140: 6350 726f 7073 2f61 7070 2e78 6d6c 20a2  cProps/app.xml .
-00002150: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-00002160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002060: 0000 7c92 5f4b c330 14c5 df05 bf43 c9b3  ..|._K.0.....C..
+00002070: 5dd2 d43f 5b68 3b50 193e 3810 ac28 be85  ]..?[h;P.>8..(..
+00002080: e46e 2b6b d390 44bb 7d7b d376 abd5 898f  .n+k..D.}{.v....
+00002090: c939 f797 732e 49e6 bbaa 0c3e c1d8 a256  .9..s.I....>...V
+000020a0: 298a 2604 05a0 442d 0bb5 4ed1 4bbe 08a7  ).&...D-..N.K...
+000020b0: 28b0 8e2b c9cb 5a41 8af6 60d1 3c3b 3f4b  (..+..ZA..`.<;?K
+000020c0: 8466 a236 f064 6a0d c615 6003 4f52 9609  .f.6.dj...`.OR..
+000020d0: 9da2 8d73 9a61 6cc5 062a 6e27 dea1 bcb8  ...s.al..*n'....
+000020e0: aa4d c59d 3f9a 35d6 5c6c f91a 3025 e41a  .M..?.5.\l..0%..
+000020f0: 57e0 b8e4 8ee3 1618 ea81 880e 4829 06a4  W...........H)..
+00002100: fe30 6507 9002 4309 1528 6771 3489 f0b7  .0e...C..(gq4...
+00002110: d781 a9ec 9f03 9d32 7256 85db 6bdf e910  .......2rV..k...
+00002120: 77cc 96a2 1707 f7ce 1683 b169 9a49 1377  w..........i.I.w
+00002130: 317c fe08 bf2d 1f9f bbaa 61a1 da5d 0940  1|...-....a..].@
+00002140: 5922 0513 06b8 ab4d f600 dc28 b808 96c5  Y".....M...(....
+00002150: 1612 3c12 da25 96dc baa5 dff7 aa00 79bb  ..<..%........y.
+00002160: ffe5 3dd5 3db7 abd1 c341 063e 18eb 6b1c  ..=.=....A.>..k.
+00002170: 95d7 f8ee 3e5f a08c 124a 4332 0b09 cd29  ....>_...JC2...)
+00002180: 65f1 0da3 f17b fbfc 8ff9 3668 7f51 1d42  e....{....6h.Q.B
+00002190: fc4f 8c43 7219 9238 2794 d129 bb9a 8d88  .O.Cr..8'..)....
+000021a0: 4740 96e0 93cf 917d 0100 00ff ff03 0050  G@.....}.......P
+000021b0: 4b03 0414 0006 0008 0000 0021 0061 4909  K..........!.aI.
+000021c0: 1089 0100 0011 0300 0010 0008 0164 6f63  .............doc
+000021d0: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
+000021e0: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002250: 0000 0000 0000 9c92 416f db30 0c85 ef03  ........Ao.0....
-00002260: fa1f 0cdd 1b39 dd50 0c81 ac62 4857 f4b0  .....9.P...bHW..
-00002270: 6101 92b6 674d a663 a1b2 2488 ac91 ecd7  a...gM.c..$.....
-00002280: 8fb6 d1d4 d97a ea8d e47b 78fa 4449 dd1c  .....z...{x.DI..
-00002290: 3a5f f490 d1c5 5089 e5a2 1405 041b 6b17  :_....P.......k.
-000022a0: f695 78d8 dd5d 7e15 0592 09b5 f131 4025  ..x..]~......1@%
-000022b0: 8e80 e246 5f7c 529b 1c13 6472 8005 4704  ...F_|R...dr..G.
-000022c0: ac44 4b94 5652 a26d a133 b860 39b0 d2c4  .DK.VR.m.3.`9...
-000022d0: dc19 e236 ef65 6c1a 67e1 36da 970e 02c9  ...6.el.g.6.....
-000022e0: abb2 bc96 7020 0835 d497 e914 28a6 c455  ....p .5....(..U
-000022f0: 4f1f 0dad a31d f8f0 7177 4c0c acd5 b794  O.......qwL.....
-00002300: bcb3 86f8 96fa a7b3 3962 6ca8 f87e b0e0  ........9bl..~..
-00002310: 959c 8b8a e9b6 605f b2a3 a32e 959c b76a  ......`_.......j
-00002320: 6b8d 8735 07eb c678 0425 df06 ea1e ccb0  k..5...x.%......
-00002330: b48d 7119 b5ea 69d5 83a5 980b 747f 786d  ..q...i.....t.xm
-00002340: 57a2 f86d 1006 9c4a f426 3b13 88b1 06db  W..m...J.&;.....
-00002350: d48c b54f 4859 3fc5 fc8c 2d00 a192 6c98  ...OHY?...-...l.
-00002360: 8663 39f7 ce6b f745 2f47 0317 e7c6 2160  .c9..k.E/G....!`
-00002370: 0261 e11c 71e7 c803 fe6a 3626 d33b c4cb  .a..q....j6&.;..
-00002380: 39f1 c830 f14e 38db 816f 3a73 ce37 5e99  9..0.N8..o:s.7^.
-00002390: 4ffa 277b 1dbb 64c2 9185 53f5 c385 677c  O.'{..d...S...g|
-000023a0: 48bb 786b 085e d779 3e54 dbd6 64a8 f905  H.xk.^.y>T..d...
-000023b0: 4eeb 3e0d d43d 6f32 fb21 64dd 9ab0 87fa  N.>..=o2.!d.....
-000023c0: d5f3 bf30 3cfe e3f4 c3f5 f27a 517e 2ef9  ...0<......zQ~..
-000023d0: 5d67 3325 dffe b2fe 0b00 00ff ff03 0050  ]g3%...........P
-000023e0: 4b01 022d 0014 0006 0008 0000 0021 0041  K..-.........!.A
-000023f0: 3782 cf6e 0100 0004 0500 0013 0000 0000  7..n............
-00002400: 0000 0000 0000 0000 0000 0000 005b 436f  .............[Co
-00002410: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00002420: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00002430: b555 3023 f400 0000 4c02 0000 0b00 0000  .U0#....L.......
-00002440: 0000 0000 0000 0000 0000 a703 0000 5f72  .............._r
-00002450: 656c 732f 2e72 656c 7350 4b01 022d 0014  els/.relsPK..-..
-00002460: 0006 0008 0000 0021 00dd 6547 026d 0300  .......!..eG.m..
-00002470: 0062 0800 000f 0000 0000 0000 0000 0000  .b..............
-00002480: 0000 00cc 0600 0078 6c2f 776f 726b 626f  .......xl/workbo
-00002490: 6f6b 2e78 6d6c 504b 0102 2d00 1400 0600  ok.xmlPK..-.....
-000024a0: 0800 0000 2100 813e 9497 f300 0000 ba02  ....!..>........
-000024b0: 0000 1a00 0000 0000 0000 0000 0000 0000  ................
-000024c0: 660a 0000 786c 2f5f 7265 6c73 2f77 6f72  f...xl/_rels/wor
-000024d0: 6b62 6f6f 6b2e 786d 6c2e 7265 6c73 504b  kbook.xml.relsPK
-000024e0: 0102 2d00 1400 0600 0800 0000 2100 93ea  ..-.........!...
-000024f0: deab 7b02 0000 c705 0000 1800 0000 0000  ..{.............
-00002500: 0000 0000 0000 0000 990c 0000 786c 2f77  ............xl/w
-00002510: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002520: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00002530: 0000 2100 c117 10be 4e07 0000 c620 0000  ..!.....N.... ..
-00002540: 1300 0000 0000 0000 0000 0000 0000 4a0f  ..............J.
-00002550: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
-00002560: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
-00002570: 0000 0021 0079 a180 6ca4 0200 0052 0600  ...!.y..l....R..
-00002580: 000d 0000 0000 0000 0000 0000 0000 00c9  ................
-00002590: 1600 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
-000025a0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000025b0: 7155 f0bf ac00 0000 e600 0000 1400 0000  qU..............
-000025c0: 0000 0000 0000 0000 0000 9819 0000 786c  ..............xl
-000025d0: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-000025e0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000025f0: 2100 3b6d 324b c100 0000 4201 0000 2300  !.;m2K....B...#.
-00002600: 0000 0000 0000 0000 0000 0000 761a 0000  ............v...
-00002610: 786c 2f77 6f72 6b73 6865 6574 732f 5f72  xl/worksheets/_r
-00002620: 656c 732f 7368 6565 7431 2e78 6d6c 2e72  els/sheet1.xml.r
-00002630: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00002640: 0021 005e 39c1 35e8 0200 0000 2100 0027  .!.^9.5.....!..'
-00002650: 0000 0000 0000 0000 0000 0000 0078 1b00  .............x..
-00002660: 0078 6c2f 7072 696e 7465 7253 6574 7469  .xl/printerSetti
-00002670: 6e67 732f 7072 696e 7465 7253 6574 7469  ngs/printerSetti
-00002680: 6e67 7331 2e62 696e 504b 0102 2d00 1400  ngs1.binPK..-...
-00002690: 0600 0800 0000 2100 d081 8ccd 4401 0000  ......!.....D...
-000026a0: 6902 0000 1100 0000 0000 0000 0000 0000  i...............
-000026b0: 0000 a51e 0000 646f 6350 726f 7073 2f63  ......docProps/c
-000026c0: 6f72 652e 786d 6c50 4b01 022d 0014 0006  ore.xmlPK..-....
-000026d0: 0008 0000 0021 0061 4909 1089 0100 0011  .....!.aI.......
-000026e0: 0300 0010 0000 0000 0000 0000 0000 0000  ................
-000026f0: 0020 2100 0064 6f63 5072 6f70 732f 6170  . !..docProps/ap
-00002700: 702e 786d 6c50 4b05 0600 0000 000c 000c  p.xmlPK.........
-00002710: 0026 0300 00df 2300 0000 00              .&....#....
+00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022e0: 0000 0000 009c 9241 6fdb 300c 85ef 03fa  .......Ao.0.....
+000022f0: 1f0c dd1b 39dd 500c 81ac 6248 57f4 b061  ....9.P...bHW..a
+00002300: 0192 b667 4da6 63a1 b224 88ac 91ec d78f  ...gM.c..$......
+00002310: b6d1 d4d9 7aea 8de4 7b78 fa44 49dd 1c3a  ....z...{x.DI..:
+00002320: 5ff4 90d1 c550 89e5 a214 0504 1b6b 17f6  _....P.......k..
+00002330: 9578 d8dd 5d7e 1505 9209 b5f1 3140 258e  .x..]~......1@%.
+00002340: 80e2 465f 7c52 9b1c 1364 7280 0547 04ac  ..F_|R...dr..G..
+00002350: 444b 9456 52a2 6da1 33b8 6039 b0d2 c4dc  DK.VR.m.3.`9....
+00002360: 19e2 36ef 656c 1a67 e136 da97 0e02 c9ab  ..6.el.g.6......
+00002370: b2bc 9670 2008 35d4 97e9 1428 a6c4 554f  ...p .5....(..UO
+00002380: 1f0d ada3 1df8 f071 774c 0cac d5b7 94bc  .......qwL......
+00002390: b386 f896 faa7 b339 626c a8f8 7eb0 e095  .......9bl..~...
+000023a0: 9c8b 8ae9 b660 5fb2 a3a3 2e95 9cb7 6a6b  .....`_.......jk
+000023b0: 8d87 3507 ebc6 7804 25df 06ea 1ecc b0b4  ..5...x.%.......
+000023c0: 8d71 19b5 ea69 d583 a598 0b74 7f78 6d57  .q...i.....t.xmW
+000023d0: a2f8 6d10 069c 4af4 263b 1388 b106 dbd4  ..m...J.&;......
+000023e0: 8cb5 4f48 593f c5fc 8c2d 00a1 926c 9886  ..OHY?...-...l..
+000023f0: 6339 f7ce 6bf7 452f 4703 17e7 c621 6002  c9..k.E/G....!`.
+00002400: 61e1 1c71 e7c8 03fe 6a36 26d3 3bc4 cb39  a..q....j6&.;..9
+00002410: f1c8 30f1 4e38 db81 6f3a 73ce 375e 994f  ..0.N8..o:s.7^.O
+00002420: fa27 7b1d bb64 c291 8553 f5c3 8567 7c48  .'{..d...S...g|H
+00002430: bb78 6b08 5ed7 793e 54db d664 a8f9 054e  .xk.^.y>T..d...N
+00002440: eb3e 0dd4 3d6f 32fb 2164 dd9a b087 fad5  .>..=o2.!d......
+00002450: f3bf 303c fee3 f4c3 f5f2 7a51 7e2e f95d  ..0<......zQ~..]
+00002460: 6733 25df feb2 fe0b 0000 ffff 0300 504b  g3%...........PK
+00002470: 0102 2d00 1400 0600 0800 0000 2100 4137  ..-.........!.A7
+00002480: 82cf 6e01 0000 0405 0000 1300 0000 0000  ..n.............
+00002490: 0000 0000 0000 0000 0000 0000 5b43 6f6e  ............[Con
+000024a0: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
+000024b0: 4b01 022d 0014 0006 0008 0000 0021 00b5  K..-.........!..
+000024c0: 5530 23f4 0000 004c 0200 000b 0000 0000  U0#....L........
+000024d0: 0000 0000 0000 0000 00a7 0300 005f 7265  ............._re
+000024e0: 6c73 2f2e 7265 6c73 504b 0102 2d00 1400  ls/.relsPK..-...
+000024f0: 0600 0800 0000 2100 f4e4 7444 8903 0000  ......!...tD....
+00002500: 9308 0000 0f00 0000 0000 0000 0000 0000  ................
+00002510: 0000 cc06 0000 786c 2f77 6f72 6b62 6f6f  ......xl/workboo
+00002520: 6b2e 786d 6c50 4b01 022d 0014 0006 0008  k.xmlPK..-......
+00002530: 0000 0021 0081 3e94 97f3 0000 00ba 0200  ...!..>.........
+00002540: 001a 0000 0000 0000 0000 0000 0000 0082  ................
+00002550: 0a00 0078 6c2f 5f72 656c 732f 776f 726b  ...xl/_rels/work
+00002560: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
+00002570: 022d 0014 0006 0008 0000 0021 00e2 1e79  .-.........!...y
+00002580: 58df 0200 0013 0600 0018 0000 0000 0000  X...............
+00002590: 0000 0000 0000 00b5 0c00 0078 6c2f 776f  ...........xl/wo
+000025a0: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+000025b0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000025c0: 0021 00c1 1710 be4e 0700 00c6 2000 0013  .!.....N.... ...
+000025d0: 0000 0000 0000 0000 0000 0000 00ca 0f00  ................
+000025e0: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
+000025f0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00002600: 0000 2100 79a1 806c a402 0000 5206 0000  ..!.y..l....R...
+00002610: 0d00 0000 0000 0000 0000 0000 0000 4917  ..............I.
+00002620: 0000 786c 2f73 7479 6c65 732e 786d 6c50  ..xl/styles.xmlP
+00002630: 4b01 022d 0014 0006 0008 0000 0021 0056  K..-.........!.V
+00002640: 7cf8 49b2 0000 00ff 0000 0014 0000 0000  |.I.............
+00002650: 0000 0000 0000 0000 0018 1a00 0078 6c2f  .............xl/
+00002660: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
+00002670: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00002680: 003b 6d32 4bc1 0000 0042 0100 0023 0000  .;m2K....B...#..
+00002690: 0000 0000 0000 0000 0000 00fc 1a00 0078  ...............x
+000026a0: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
+000026b0: 6c73 2f73 6865 6574 312e 786d 6c2e 7265  ls/sheet1.xml.re
+000026c0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+000026d0: 2100 5e39 c135 e802 0000 0021 0000 2700  !.^9.5.....!..'.
+000026e0: 0000 0000 0000 0000 0000 0000 fe1b 0000  ................
+000026f0: 786c 2f70 7269 6e74 6572 5365 7474 696e  xl/printerSettin
+00002700: 6773 2f70 7269 6e74 6572 5365 7474 696e  gs/printerSettin
+00002710: 6773 312e 6269 6e50 4b01 022d 0014 0006  gs1.binPK..-....
+00002720: 0008 0000 0021 00b1 7bf0 024d 0100 0069  .....!..{..M...i
+00002730: 0200 0011 0000 0000 0000 0000 0000 0000  ................
+00002740: 002b 1f00 0064 6f63 5072 6f70 732f 636f  .+...docProps/co
+00002750: 7265 2e78 6d6c 504b 0102 2d00 1400 0600  re.xmlPK..-.....
+00002760: 0800 0000 2100 6149 0910 8901 0000 1103  ....!.aI........
+00002770: 0000 1000 0000 0000 0000 0000 0000 0000  ................
+00002780: af21 0000 646f 6350 726f 7073 2f61 7070  .!..docProps/app
+00002790: 2e78 6d6c 504b 0506 0000 0000 0c00 0c00  .xmlPK..........
+000027a0: 2603 0000 6e24 0000 0000                 &...n$....
```

### Comparing `usgs-strec-2.2.5/test/src/strec/data/subsampled_nga_results.xlsx` & `usgs-strec-2.2.6/test/src/strec/data/subsampled_nga_results.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/van_slab2_dep_02.23.18.grd` & `usgs-strec-2.2.6/test/src/strec/data/van_slab2_dep_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/van_slab2_dip_02.23.18.grd` & `usgs-strec-2.2.6/test/src/strec/data/van_slab2_dip_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/van_slab2_str_02.23.18.grd` & `usgs-strec-2.2.6/test/src/strec/data/van_slab2_str_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/van_slab2_thk_02.23.18.grd` & `usgs-strec-2.2.6/test/src/strec/data/van_slab2_thk_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/data/van_slab2_unc_02.23.18.grd` & `usgs-strec-2.2.6/test/src/strec/data/van_slab2_unc_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/database_test.py` & `usgs-strec-2.2.6/test/src/strec/database_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/distance_test.py` & `usgs-strec-2.2.6/test/src/strec/distance_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/gcmt_test.py` & `usgs-strec-2.2.6/test/src/strec/gcmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/gmreg_test.py` & `usgs-strec-2.2.6/test/src/strec/gmreg_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/kagan_test.py` & `usgs-strec-2.2.6/test/src/strec/kagan_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/slab_test.py` & `usgs-strec-2.2.6/test/src/strec/slab_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/subduction_test.py` & `usgs-strec-2.2.6/test/src/strec/subduction_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.5/test/src/strec/subtype_test.py` & `usgs-strec-2.2.6/test/src/strec/subtype_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,17 +95,23 @@
 
 
 def test_get_online_tensor():
     eventid_with_tensor = "official20110311054624120_30"
     eventid_without_tensor = "us2000ati0"
     eventid_with_local_tensor = "nc72852946"
     selector = SubductionSelector()
-    lat1, lon1, depth1, tensor1 = selector.getOnlineTensor(eventid_with_tensor)
-    lat2, lon2, depth2, tensor2 = selector.getOnlineTensor(eventid_without_tensor)
-    lat3, lon3, depth3, tensor3 = selector.getOnlineTensor(eventid_with_local_tensor)
+    lat1, lon1, depth1, magnitude, tensor1 = selector.getOnlineTensor(
+        eventid_with_tensor
+    )
+    lat2, lon2, depth2, magnitude, tensor2 = selector.getOnlineTensor(
+        eventid_without_tensor
+    )
+    lat3, lon3, depth3, magnitude, tensor3 = selector.getOnlineTensor(
+        eventid_with_local_tensor
+    )
     tensor1_cmp = {
         "T": {"value": 5.6e22, "plunge": 53.0, "azimuth": 296.0},
         "mtt": -1.509e21,
         "mpp": -1.523e22,
         "mrp": 4.837e22,
         "N": {"value": 1.2e20, "plunge": 1.0, "azimuth": 204.0},
         "mrr": 1.674e22,
@@ -173,56 +179,61 @@
     results1 = selector.getSubductionType(lat, lon, depth, eventid)
     assert results1["FocalMechanism"] == "SS"
 
     # Made up event that should  have a composite moment tensor
     lat = 2.321
     lon = 128.132
     depth = 21.7
-    results1 = selector.getSubductionType(lat, lon, depth)
+    magnitude = 6.5
+    results1 = selector.getSubductionType(lat, lon, depth, magnitude)
     assert results1["TensorType"] == "composite"
     assert results1["FocalMechanism"] == "RS"
 
     # Made up event that should not have a composite moment tensor
     lat = -27.725
     lon = -147.832
     depth = 25
-    results1 = selector.getSubductionType(lat, lon, depth)
+    magnitude = 6.5
+    results1 = selector.getSubductionType(lat, lon, depth, magnitude)
     assert results1["FocalMechanism"] == "ALL"
 
     # Pass in an event with tensor parameters
     # chile 2010
     lat = -36.122
     lon = -72.898
     depth = 22.9
+    magnitude = 9.0
     tensor_params = {
         "source": "duputel",
         "type": "Mww",
         "NP1": {"strike": 178, "dip": 77, "rake": 86},
         "NP2": {"strike": 17, "dip": 14, "rake": 108},
         "T": {"value": 2.236e22, "plunge": 58, "azimuth": 82},
         "N": {"value": 0.040e22, "plunge": 4, "azimuth": 179},
         "P": {"value": -2.276e22, "plunge": 32, "azimuth": 272},
     }
     results1 = selector.getSubductionType(
-        lat, lon, depth, eventid=None, tensor_params=tensor_params
+        lat, lon, depth, magnitude, eventid=None, tensor_params=tensor_params
     )
     assert results1["FocalMechanism"] == "RS"
 
     # event location inside grid but not horizontally on subducting slab
     lat = 13.58
     lon = -92.92
     depth = 20.0
-    results1 = selector.getSubductionType(lat, lon, depth)
+    magnitude = 6.5
+    results1 = selector.getSubductionType(lat, lon, depth, magnitude)
     assert results1["SlabModelRegion"] == "Central America"
 
     # event at a VERY high latitude to see if grid stuff blows up
     lat = 89.1
     lon = 49.1
     depth = 20.0
-    results1 = selector.getSubductionType(lat, lon, depth)
+    magnitude = 6.5
+    results1 = selector.getSubductionType(lat, lon, depth, magnitude)
     assert results1["TectonicRegion"] == "Stable"
     assert results1["FocalMechanism"] == "ALL"
 
 
 def test_get_subduction_by_id():
     selector = SubductionSelector()
     # Tohoku, should have an online moment tensor
```

### Comparing `usgs-strec-2.2.5/test/src/strec/utils_test.py` & `usgs-strec-2.2.6/test/src/strec/utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         raise (e)
     finally:
         if pathlib.Path(tempfile).is_file():
             os.remove(tempfile)
 
 
 def test_read_input_file():
-    df = pd.DataFrame({"lat": [1, 2, 3], "lon": [1, 2, 3], "depth": [1, 2, 3]})
+    df = pd.DataFrame(
+        {"lat": [1, 2, 3], "lon": [1, 2, 3], "depth": [1, 2, 3], "mag": [1, 2, 3]}
+    )
     tmpfile = None
     try:
         h, tmpfile = mkstemp(suffix=".xlsx")
         os.close(h)
         df.to_excel(tmpfile)
         read_input_file(tmpfile, [None], None)
         df.to_csv(tmpfile)
```

