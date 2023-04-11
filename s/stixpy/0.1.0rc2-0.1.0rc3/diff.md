# Comparing `tmp/stixpy-0.1.0rc2.tar.gz` & `tmp/stixpy-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shane/Projects/stixpy/dist/.tmp-ox1ncvyp/stixpy-0.1.0rc2.tar", last modified: Thu Jan 26 11:19:43 2023, max compression
+gzip compressed data, was "/Users/shane/Projects/stixpy/dist/.tmp-a41_eeuk/stixpy-0.1.0rc3.tar", last modified: Tue Apr 11 09:47:14 2023, max compression
```

## Comparing `stixpy-0.1.0rc2.tar` & `stixpy-0.1.0rc3.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/.circleci/
--rw-r--r--   0 shane      (501) staff       (20)     1991 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/.circleci/config.yml
--rw-r--r--   0 shane      (501) staff       (20)      235 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/.circleci/early_exit.sh
--rw-r--r--   0 shane      (501) staff       (20)     2298 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/.gitignore
--rw-r--r--   0 shane      (501) staff       (20)     1553 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 shane      (501) staff       (20)      544 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/.readthedocs.yml
--rw-r--r--   0 shane      (501) staff       (20)        0 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/CHANGELOG.rst
--rw-r--r--   0 shane      (501) staff       (20)     1481 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/LICENSE.rst
--rw-r--r--   0 shane      (501) staff       (20)      361 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/MANIFEST.in
--rw-r--r--   0 shane      (501) staff       (20)     3261 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)     2902 2023-01-26 11:16:48.000000 stixpy-0.1.0rc2/README.rst
--rw-r--r--   0 shane      (501) staff       (20)     1703 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/azure-pipelines.yml
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/calibration/
--rw-r--r--   0 shane      (501) staff       (20)        0 2021-01-12 17:09:31.000000 stixpy-0.1.0rc2/calibration/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     5894 2021-01-13 09:38:52.000000 stixpy-0.1.0rc2/calibration/compression.py
--rw-r--r--   0 shane      (501) staff       (20)     1489 2022-07-13 13:02:40.000000 stixpy-0.1.0rc2/calibration/detector.py
--rw-r--r--   0 shane      (501) staff       (20)     2684 2022-08-30 08:34:33.000000 stixpy-0.1.0rc2/calibration/energy.py
--rw-r--r--   0 shane      (501) staff       (20)     6508 2022-08-30 08:34:34.000000 stixpy-0.1.0rc2/calibration/grid.py
--rw-r--r--   0 shane      (501) staff       (20)     3149 2022-08-30 08:34:33.000000 stixpy-0.1.0rc2/calibration/livetime.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/calibration/tests/
--rw-r--r--   0 shane      (501) staff       (20)        0 2021-01-12 17:09:31.000000 stixpy-0.1.0rc2/calibration/tests/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)    37006 2021-01-13 09:38:52.000000 stixpy-0.1.0rc2/calibration/tests/test_compression.py
--rw-r--r--   0 shane      (501) staff       (20)       91 2022-07-11 09:17:50.000000 stixpy-0.1.0rc2/calibration/tests/test_detector.py
--rw-r--r--   0 shane      (501) staff       (20)      814 2022-08-30 08:34:34.000000 stixpy-0.1.0rc2/calibration/tests/test_energy.py
--rw-r--r--   0 shane      (501) staff       (20)     1448 2022-08-30 08:34:34.000000 stixpy-0.1.0rc2/calibration/tests/test_grid.py
--rw-r--r--   0 shane      (501) staff       (20)      592 2021-01-12 17:09:31.000000 stixpy-0.1.0rc2/calibration/tests/test_livetime.py
--rw-r--r--   0 shane      (501) staff       (20)     1823 2022-08-16 15:03:56.000000 stixpy-0.1.0rc2/calibration/tests/test_transmission.py
--rw-r--r--   0 shane      (501) staff       (20)     9518 2022-08-16 15:03:56.000000 stixpy-0.1.0rc2/calibration/transmission.py
--rw-r--r--   0 shane      (501) staff       (20)    13598 2022-08-30 09:43:50.000000 stixpy-0.1.0rc2/calibration/visibility.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/changelog/
--rw-r--r--   0 shane      (501) staff       (20)     1886 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/changelog/README.rst
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/docs/
--rw-r--r--   0 shane      (501) staff       (20)     6148 2020-11-24 22:37:15.000000 stixpy-0.1.0rc2/docs/.DS_Store
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/docs/.idea/
--rw-r--r--   0 shane      (501) staff       (20)      176 2021-05-28 08:58:13.000000 stixpy-0.1.0rc2/docs/.idea/.gitignore
--rw-r--r--   0 shane      (501) staff       (20)      284 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/docs.iml
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/docs/.idea/inspectionProfiles/
--rw-r--r--   0 shane      (501) staff       (20)    11220 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 shane      (501) staff       (20)      174 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 shane      (501) staff       (20)      206 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/misc.xml
--rw-r--r--   0 shane      (501) staff       (20)      260 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/modules.xml
--rw-r--r--   0 shane      (501) staff       (20)      183 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/vcs.xml
--rw-r--r--   0 shane      (501) staff       (20)     2103 2021-05-28 08:58:26.000000 stixpy-0.1.0rc2/docs/.idea/workspace.xml
--rw-r--r--   0 shane      (501) staff       (20)      634 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/docs/Makefile
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/docs/code_ref/
--rw-r--r--   0 shane      (501) staff       (20)      167 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/docs/code_ref/data.rst
--rw-r--r--   0 shane      (501) staff       (20)      143 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/docs/code_ref/frames.rst
--rw-r--r--   0 shane      (501) staff       (20)      142 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/docs/code_ref/index.rst
--rw-r--r--   0 shane      (501) staff       (20)      119 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/docs/code_ref/science.rst
--rw-r--r--   0 shane      (501) staff       (20)      146 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/docs/code_ref/timeseries.rst
--rw-r--r--   0 shane      (501) staff       (20)      122 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/docs/code_ref/vis.rst
--rw-r--r--   0 shane      (501) staff       (20)     4179 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/docs/conf.py
--rw-r--r--   0 shane      (501) staff       (20)     4897 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/docs/dev_guide.rst
--rw-r--r--   0 shane      (501) staff       (20)      204 2021-02-02 22:03:20.000000 stixpy-0.1.0rc2/docs/index.rst
--rw-r--r--   0 shane      (501) staff       (20)      760 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/docs/make.bat
--rw-r--r--   0 shane      (501) staff       (20)     2366 2023-01-19 14:11:23.000000 stixpy-0.1.0rc2/docs/quickstart.rst
--rw-r--r--   0 shane      (501) staff       (20)     3553 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/docs/stix.rst
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/docs/whatsnew/
--rw-r--r--   0 shane      (501) staff       (20)      129 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/docs/whatsnew/changelog.rst
--rw-r--r--   0 shane      (501) staff       (20)       92 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/docs/whatsnew/index.rst
--rw-r--r--   0 shane      (501) staff       (20)     7576 2021-05-06 10:33:25.000000 stixpy-0.1.0rc2/docs/whatsnew/latest_changelog.txt
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/examples/
--rw-r--r--   0 shane      (501) staff       (20)     2490 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/examples/imaging_demo.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/licenses/
--rw-r--r--   0 shane      (501) staff       (20)      372 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/licenses/README.rst
--rw-r--r--   0 shane      (501) staff       (20)     1659 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/licenses/TEMPLATE_LICENSE.rst
--rw-r--r--   0 shane      (501) staff       (20)     1139 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/pyproject.toml
--rw-r--r--   0 shane      (501) staff       (20)        1 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/requirements.txt
--rw-r--r--   0 shane      (501) staff       (20)     1434 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/setup.cfg
--rwxr-xr-x   0 shane      (501) staff       (20)     1577 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/setup.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy/
--rw-r--r--   0 shane      (501) staff       (20)      155 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)      137 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/stixpy/conftest.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/data/
--rw-r--r--   0 shane      (501) staff       (20)      245 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/stixpy/data/README.rst
--rw-r--r--   0 shane      (501) staff       (20)       61 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/data/__init__.py
--rw-rw-r--   0 shane      (501) staff       (20)  4769280 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-cal-energy_20200506_V01.fits
--rw-r--r--   0 shane      (501) staff       (20)  1022400 2022-09-11 20:39:46.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-hk-maxi_20200501_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)   878400 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-background_20200506_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)    46080 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-flareflag_20200506_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)  1693440 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-lightcurve_20200506_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)    40320 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-ql-tmstatusflarelist_20200506_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)   195840 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-spectra_20200506_V01.fits
--rw-rw-r--   0 shane      (501) staff       (20)   368640 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-variance_20200506_V01.fits
--rw-r--r--   0 shane      (501) staff       (20)   420480 2022-09-11 15:04:14.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-cpd_20200505T235959-20200506T000019_V01_0087031809-50883.fits
--rw-r--r--   0 shane      (501) staff       (20)   169920 2022-09-11 15:04:06.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-rpd_20200505T235959-20200506T000019_V01_0087031808-50882.fits
--rw-rw-r--   0 shane      (501) staff       (20)   420480 2022-03-22 11:45:39.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-scpd_20200505T235959-20200506T000019_V01_0087031810-50884.fits
--rw-r--r--   0 shane      (501) staff       (20)    51840 2022-09-11 15:04:41.000000 stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-spec_20200505T235959-20200506T000019_V01_0087031812-50886.fits
--rw-r--r--   0 shane      (501) staff       (20)     2525 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/data/test.py
--rw-r--r--   0 shane      (501) staff       (20)   629729 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/data/test_data.tar.gz
--rw-r--r--   0 shane      (501) staff       (20)    10456 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/frames.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/net/
--rw-r--r--   0 shane      (501) staff       (20)       29 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/net/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     1010 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/net/attrs.py
--rw-r--r--   0 shane      (501) staff       (20)     8401 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/net/client.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/net/tests/
--rw-r--r--   0 shane      (501) staff       (20)        0 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/net/tests/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     1913 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/net/tests/test_client.py
--rw-r--r--   0 shane      (501) staff       (20)    40362 2023-01-26 10:59:49.000000 stixpy-0.1.0rc2/stixpy/science.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/tests/
--rw-r--r--   0 shane      (501) staff       (20)      108 2020-07-15 13:40:37.000000 stixpy-0.1.0rc2/stixpy/tests/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     2684 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/tests/test_frames.py
--rw-r--r--   0 shane      (501) staff       (20)     6505 2023-01-26 10:59:49.000000 stixpy-0.1.0rc2/stixpy/tests/test_science.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/timeseries/
--rw-r--r--   0 shane      (501) staff       (20)       42 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/timeseries/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)    19911 2023-01-23 23:02:58.000000 stixpy-0.1.0rc2/stixpy/timeseries/quicklook.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/timeseries/tests/
--rw-r--r--   0 shane      (501) staff       (20)        0 2020-11-24 22:39:04.000000 stixpy-0.1.0rc2/stixpy/timeseries/tests/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)      650 2023-01-19 14:20:38.000000 stixpy-0.1.0rc2/stixpy/timeseries/tests/test_quicklook.py
--rw-r--r--   0 shane      (501) staff       (20)      348 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy/version.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/vis/
--rw-r--r--   0 shane      (501) staff       (20)        0 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/stixpy/vis/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     7784 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/stixpy/vis/map_reprojection.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy/vis/tests/
--rw-r--r--   0 shane      (501) staff       (20)        0 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/stixpy/vis/tests/__init__.py
--rw-r--r--   0 shane      (501) staff       (20)     1248 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/stixpy/vis/tests/test_map_reprojection.py
-drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-01-26 11:19:43.000000 stixpy-0.1.0rc2/stixpy.egg-info/
--rw-r--r--   0 shane      (501) staff       (20)     3261 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy.egg-info/PKG-INFO
--rw-r--r--   0 shane      (501) staff       (20)     3020 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy.egg-info/SOURCES.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy.egg-info/dependency_links.txt
--rw-r--r--   0 shane      (501) staff       (20)        1 2020-07-29 17:38:09.000000 stixpy-0.1.0rc2/stixpy.egg-info/not-zip-safe
--rw-r--r--   0 shane      (501) staff       (20)      295 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy.egg-info/requires.txt
--rw-r--r--   0 shane      (501) staff       (20)       19 2023-01-26 11:19:42.000000 stixpy-0.1.0rc2/stixpy.egg-info/top_level.txt
--rw-r--r--   0 shane      (501) staff       (20)     1904 2023-01-19 14:17:40.000000 stixpy-0.1.0rc2/tox.ini
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.594498 stixpy-0.1.0rc3/
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.481400 stixpy-0.1.0rc3/.circleci/
+-rw-r--r--   0 shane      (501) staff       (20)     1991 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/.circleci/config.yml
+-rw-r--r--   0 shane      (501) staff       (20)      235 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/.circleci/early_exit.sh
+-rw-r--r--   0 shane      (501) staff       (20)     2298 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/.gitignore
+-rw-r--r--   0 shane      (501) staff       (20)     1553 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 shane      (501) staff       (20)      544 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/.readthedocs.yml
+-rw-r--r--   0 shane      (501) staff       (20)        0 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/CHANGELOG.rst
+-rw-r--r--   0 shane      (501) staff       (20)     1481 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/LICENSE.rst
+-rw-r--r--   0 shane      (501) staff       (20)      361 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/MANIFEST.in
+-rw-r--r--   0 shane      (501) staff       (20)     3260 2023-04-11 09:47:14.594783 stixpy-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)     2901 2023-04-11 09:25:39.000000 stixpy-0.1.0rc3/README.rst
+-rw-r--r--   0 shane      (501) staff       (20)     1704 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/azure-pipelines.yml
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.482172 stixpy-0.1.0rc3/changelog/
+-rw-r--r--   0 shane      (501) staff       (20)     1886 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/changelog/README.rst
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.487506 stixpy-0.1.0rc3/docs/
+-rw-r--r--   0 shane      (501) staff       (20)     8196 2023-02-01 09:51:43.000000 stixpy-0.1.0rc3/docs/.DS_Store
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.494014 stixpy-0.1.0rc3/docs/.idea/
+-rw-r--r--   0 shane      (501) staff       (20)      176 2021-05-28 08:58:13.000000 stixpy-0.1.0rc3/docs/.idea/.gitignore
+-rw-r--r--   0 shane      (501) staff       (20)      284 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/docs.iml
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.496133 stixpy-0.1.0rc3/docs/.idea/inspectionProfiles/
+-rw-r--r--   0 shane      (501) staff       (20)    11220 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 shane      (501) staff       (20)      174 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 shane      (501) staff       (20)      206 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/misc.xml
+-rw-r--r--   0 shane      (501) staff       (20)      260 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/modules.xml
+-rw-r--r--   0 shane      (501) staff       (20)      183 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/vcs.xml
+-rw-r--r--   0 shane      (501) staff       (20)     2103 2021-05-28 08:58:26.000000 stixpy-0.1.0rc3/docs/.idea/workspace.xml
+-rw-r--r--   0 shane      (501) staff       (20)      634 2023-01-30 14:32:10.000000 stixpy-0.1.0rc3/docs/Makefile
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.501550 stixpy-0.1.0rc3/docs/code_ref/
+-rw-r--r--   0 shane      (501) staff       (20)      196 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/data.rst
+-rw-r--r--   0 shane      (501) staff       (20)      177 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/frames.rst
+-rw-r--r--   0 shane      (501) staff       (20)      175 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/index.rst
+-rw-r--r--   0 shane      (501) staff       (20)     2092 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/product.rst
+-rw-r--r--   0 shane      (501) staff       (20)      314 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/science.rst
+-rw-r--r--   0 shane      (501) staff       (20)      294 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/timeseries.rst
+-rw-r--r--   0 shane      (501) staff       (20)      280 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/code_ref/visualisation.rst
+-rw-r--r--   0 shane      (501) staff       (20)     3775 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/conf.py
+-rw-r--r--   0 shane      (501) staff       (20)     4897 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/dev_guide.rst
+-rw-r--r--   0 shane      (501) staff       (20)     1384 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/index.rst
+-rw-r--r--   0 shane      (501) staff       (20)      760 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/docs/make.bat
+-rw-r--r--   0 shane      (501) staff       (20)     7905 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/quickstart.rst
+-rw-r--r--   0 shane      (501) staff       (20)     3553 2023-01-19 14:17:40.000000 stixpy-0.1.0rc3/docs/stix.rst
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.503561 stixpy-0.1.0rc3/docs/whatsnew/
+-rw-r--r--   0 shane      (501) staff       (20)      237 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/docs/whatsnew/changelog.rst
+-rw-r--r--   0 shane      (501) staff       (20)       92 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/docs/whatsnew/index.rst
+-rw-r--r--   0 shane      (501) staff       (20)     7576 2021-05-06 10:33:25.000000 stixpy-0.1.0rc3/docs/whatsnew/latest_changelog.txt
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.504792 stixpy-0.1.0rc3/examples/
+-rw-r--r--   0 shane      (501) staff       (20)     2490 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/examples/imaging_demo.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.506470 stixpy-0.1.0rc3/licenses/
+-rw-r--r--   0 shane      (501) staff       (20)      372 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/licenses/README.rst
+-rw-r--r--   0 shane      (501) staff       (20)     1659 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/licenses/TEMPLATE_LICENSE.rst
+-rw-r--r--   0 shane      (501) staff       (20)     1139 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/pyproject.toml
+-rw-r--r--   0 shane      (501) staff       (20)        1 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/requirements.txt
+-rw-r--r--   0 shane      (501) staff       (20)     1502 2023-04-11 09:47:14.596307 stixpy-0.1.0rc3/setup.cfg
+-rwxr-xr-x   0 shane      (501) staff       (20)     1577 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/setup.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.512397 stixpy-0.1.0rc3/stixpy/
+-rw-r--r--   0 shane      (501) staff       (20)      155 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)      137 2023-01-19 14:17:40.000000 stixpy-0.1.0rc3/stixpy/conftest.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.567684 stixpy-0.1.0rc3/stixpy/data/
+-rw-r--r--   0 shane      (501) staff       (20)      245 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/stixpy/data/README.rst
+-rw-r--r--   0 shane      (501) staff       (20)       61 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/data/__init__.py
+-rw-rw-r--   0 shane      (501) staff       (20)  4769280 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-cal-energy_20200506_V01.fits
+-rw-r--r--   0 shane      (501) staff       (20)  1022400 2022-09-11 20:39:46.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-hk-maxi_20200501_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)   878400 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-background_20200506_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)    46080 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-flareflag_20200506_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)  1693440 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-lightcurve_20200506_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)    40320 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-ql-tmstatusflarelist_20200506_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)   195840 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-spectra_20200506_V01.fits
+-rw-rw-r--   0 shane      (501) staff       (20)   368640 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-variance_20200506_V01.fits
+-rw-r--r--   0 shane      (501) staff       (20)   420480 2022-09-11 15:04:14.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-cpd_20200505T235959-20200506T000019_V01_0087031809-50883.fits
+-rw-r--r--   0 shane      (501) staff       (20)   169920 2022-09-11 15:04:06.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-rpd_20200505T235959-20200506T000019_V01_0087031808-50882.fits
+-rw-rw-r--   0 shane      (501) staff       (20)   420480 2022-03-22 11:45:39.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-scpd_20200505T235959-20200506T000019_V01_0087031810-50884.fits
+-rw-r--r--   0 shane      (501) staff       (20)    51840 2022-09-11 15:04:41.000000 stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-spec_20200505T235959-20200506T000019_V01_0087031812-50886.fits
+-rw-r--r--   0 shane      (501) staff       (20)     2525 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/data/test.py
+-rw-r--r--   0 shane      (501) staff       (20)   629729 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/data/test_data.tar.gz
+-rw-r--r--   0 shane      (501) staff       (20)    10455 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/frames.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.573503 stixpy-0.1.0rc3/stixpy/net/
+-rw-r--r--   0 shane      (501) staff       (20)       29 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/net/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     1010 2023-03-08 15:30:46.000000 stixpy-0.1.0rc3/stixpy/net/attrs.py
+-rw-r--r--   0 shane      (501) staff       (20)     8401 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/net/client.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.574770 stixpy-0.1.0rc3/stixpy/net/tests/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/net/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     1913 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/net/tests/test_client.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.577113 stixpy-0.1.0rc3/stixpy/product/
+-rw-r--r--   0 shane      (501) staff       (20)       88 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     2862 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/product.py
+-rw-r--r--   0 shane      (501) staff       (20)    11200 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/product_factory.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.580206 stixpy-0.1.0rc3/stixpy/product/sources/
+-rw-r--r--   0 shane      (501) staff       (20)      142 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/sources/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     1441 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/sources/housekeeping.py
+-rw-r--r--   0 shane      (501) staff       (20)     1565 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/sources/quicklook.py
+-rw-r--r--   0 shane      (501) staff       (20)    40845 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/sources/science.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.582698 stixpy-0.1.0rc3/stixpy/product/tests/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)      852 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/product/tests/test_product_factory.py
+-rw-r--r--   0 shane      (501) staff       (20)      526 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/science.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.585790 stixpy-0.1.0rc3/stixpy/tests/
+-rw-r--r--   0 shane      (501) staff       (20)      108 2020-07-15 13:40:37.000000 stixpy-0.1.0rc3/stixpy/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     2684 2023-03-08 15:30:46.000000 stixpy-0.1.0rc3/stixpy/tests/test_frames.py
+-rw-r--r--   0 shane      (501) staff       (20)     6787 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/tests/test_science.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.587911 stixpy-0.1.0rc3/stixpy/timeseries/
+-rw-r--r--   0 shane      (501) staff       (20)       42 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/timeseries/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)    24201 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/timeseries/quicklook.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.589203 stixpy-0.1.0rc3/stixpy/timeseries/tests/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2020-11-24 22:39:04.000000 stixpy-0.1.0rc3/stixpy/timeseries/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)      650 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/timeseries/tests/test_quicklook.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.590971 stixpy-0.1.0rc3/stixpy/utils/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/utils/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     1379 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/utils/logging.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.591973 stixpy-0.1.0rc3/stixpy/utils/tests/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/utils/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     2454 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/utils/tests/test_time.py
+-rw-r--r--   0 shane      (501) staff       (20)     2794 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/utils/time.py
+-rw-r--r--   0 shane      (501) staff       (20)      348 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy/version.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.593009 stixpy-0.1.0rc3/stixpy/visualisation/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/visualisation/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     8057 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/visualisation/map_reprojection.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.594036 stixpy-0.1.0rc3/stixpy/visualisation/tests/
+-rw-r--r--   0 shane      (501) staff       (20)        0 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/visualisation/tests/__init__.py
+-rw-r--r--   0 shane      (501) staff       (20)     1289 2023-04-11 09:24:23.000000 stixpy-0.1.0rc3/stixpy/visualisation/tests/test_map_reprojection.py
+drwxr-xr-x   0 shane      (501) staff       (20)        0 2023-04-11 09:47:14.515815 stixpy-0.1.0rc3/stixpy.egg-info/
+-rw-r--r--   0 shane      (501) staff       (20)     3260 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy.egg-info/PKG-INFO
+-rw-r--r--   0 shane      (501) staff       (20)     3102 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy.egg-info/SOURCES.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy.egg-info/dependency_links.txt
+-rw-r--r--   0 shane      (501) staff       (20)        1 2020-07-29 17:38:09.000000 stixpy-0.1.0rc3/stixpy.egg-info/not-zip-safe
+-rw-r--r--   0 shane      (501) staff       (20)      368 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy.egg-info/requires.txt
+-rw-r--r--   0 shane      (501) staff       (20)        7 2023-04-11 09:47:14.000000 stixpy-0.1.0rc3/stixpy.egg-info/top_level.txt
+-rw-r--r--   0 shane      (501) staff       (20)     1904 2023-01-19 14:17:40.000000 stixpy-0.1.0rc3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stixpy-0.1.0rc2/.circleci/config.yml` & `stixpy-0.1.0rc3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/.gitignore` & `stixpy-0.1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/.pre-commit-config.yaml` & `stixpy-0.1.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/.readthedocs.yml` & `stixpy-0.1.0rc3/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
   configuration: docs/conftest.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 formats: []
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.7
+  version: 3.8
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
         - all
```

### Comparing `stixpy-0.1.0rc2/LICENSE.rst` & `stixpy-0.1.0rc3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/PKG-INFO` & `stixpy-0.1.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: stixpy
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Analysis software for Solar Orbiter Spectromter Telescope for Imaging X-rays
 Home-page: 
 Author: STIX Team
 Author-email: shane.maloney@dias.ie
 License: BSD 3-Clause
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.rst
 
 Analysis software for Solar Orbiter Spectrometer Telescope for Imaging X-rays
@@ -31,15 +31,15 @@
 Installation
 ------------
 
 It is strongly advised that you use and isolated environment through python's venv, virturalenv, anaconda or similar.
 
 .. code-block::
 
-    pip install git+https://github.com/samaloney/stixpy
+   pip install git+https://github.com/samaloney/stixpy
 
 
 License
 -------
 
 This project is Copyright (c) STIX Team and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
```

### Comparing `stixpy-0.1.0rc2/README.rst` & `stixpy-0.1.0rc3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Installation
 ------------
 
 It is strongly advised that you use and isolated environment through python's venv, virturalenv, anaconda or similar.
 
 .. code-block::
 
-    pip install git+https://github.com/samaloney/stixpy
+   pip install git+https://github.com/samaloney/stixpy
 
 
 License
 -------
 
 This project is Copyright (c) STIX Team and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
```

### Comparing `stixpy-0.1.0rc2/azure-pipelines.yml` & `stixpy-0.1.0rc3/azure-pipelines.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: $(BuildDefinitionName)_$(Date:yyyyMMdd)$(Rev:.rr)
 variables:
   CI_NAME: Azure Pipelines
   CI_BUILD_ID: $(Build.BuildId)
   CI_BUILD_URL: "https://dev.azure.com/samaloney/STIXpy/_build/results?buildId=$(Build.BuildId)"
-  CIBW_BUILD: cp36-* cp37-* cp38-*
+  CIBW_BUILD: cp38-* cp39-* cp310-*
   CIBW_SKIP: "*-win32 *-manylinux1_i686"
 
 resources:
   repositories:
   - repository: OpenAstronomy
     type: github
     endpoint: samaloney
@@ -32,22 +32,22 @@
 - template: run-tox-env.yml@OpenAstronomy
   parameters:
     toxverspec: <4
     toxdeps: tox-pypi-filter
     submodules: false
     coverage: codecov
     envs:
-      - macos: py37
-        name: py37_mac
+      - macos: py38
+        name: py38_mac
 
-      - windows: py37
-        name: py37_win
+      - windows: py38
+        name: py38_win
 
-      - linux: py37
-        name: py37_lin
+      - linux: py38
+        name: py38_lin
 
       - linux: codestyle
         name: codestyle
 
 
 # On branches which aren't master, and not Pull Requests, build the wheels but only upload them on tags
 - ${{ if and(ne(variables['Build.Reason'], 'PullRequest'), not(contains(variables['Build.SourceBranch'], 'master'))) }}:
@@ -61,10 +61,10 @@
       test_command: 'pytest -p no:warnings --doctest-rst -m "not figure" --pyargs stixpy'
       submodules: false
       targets:
 #        - wheels_linux
 #        - wheels_macos
         - sdist
       dependsOn:
-        - py37_mac
-        - py37_win
-        - py37_lin
+        - py38_mac
+        - py38_win
+        - py38_lin
```

### Comparing `stixpy-0.1.0rc2/changelog/README.rst` & `stixpy-0.1.0rc3/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/.idea/inspectionProfiles/Project_Default.xml` & `stixpy-0.1.0rc3/docs/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/.idea/workspace.xml` & `stixpy-0.1.0rc3/docs/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/Makefile` & `stixpy-0.1.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/conf.py` & `stixpy-0.1.0rc3/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     'sphinx.ext.inheritance_diagram',
     'sphinx.ext.viewcode',
     'sphinx.ext.napoleon',
     'sphinx.ext.doctest',
     'sphinx.ext.mathjax',
     'sphinx_automodapi.automodapi',
     'sphinx_automodapi.smart_resolver',
+    'sphinx_design',
+    'sphinx_changelog',
     'matplotlib.sphinxext.plot_directive'
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
@@ -107,21 +109,7 @@
     '-Nfontsize=10',
     '-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif',
     '-Efontsize=10',
     '-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif',
     '-Gfontsize=10',
     '-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif'
 ]
-
-
-"""
-Write the latest changelog into the documentation.
-"""
-target_file = os.path.abspath("./whatsnew/latest_changelog.txt")
-try:
-    from sunpy.util.towncrier import generate_changelog_for_docs
-    if is_development:
-        generate_changelog_for_docs("../", target_file)
-except Exception as e:
-    print(f"Failed to add changelog to docs with error {e}.")
-# Make sure the file exists or else sphinx will complain.
-open(target_file, 'a').close()
```

### Comparing `stixpy-0.1.0rc2/docs/dev_guide.rst` & `stixpy-0.1.0rc3/docs/dev_guide.rst`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/make.bat` & `stixpy-0.1.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/stix.rst` & `stixpy-0.1.0rc3/docs/stix.rst`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/docs/whatsnew/latest_changelog.txt` & `stixpy-0.1.0rc3/docs/whatsnew/latest_changelog.txt`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/examples/imaging_demo.py` & `stixpy-0.1.0rc3/examples/imaging_demo.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/licenses/TEMPLATE_LICENSE.rst` & `stixpy-0.1.0rc3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/pyproject.toml` & `stixpy-0.1.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/setup.cfg` & `stixpy-0.1.0rc3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,36 +7,40 @@
 url = 
 description = Analysis software for Solar Orbiter Spectromter Telescope for Imaging X-rays
 long_description = file: README.rst
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
 	sunpy[net,timeseries]>=3.1
 	reproject
+	astroquery
 
 [options.extras_require]
 test = 
 	pytest<=6.0.0
 	pytest-astropy
 	pytest-cov
 docs = 
 	sphinx
 	sphinx-automodapi
 	towncrier
 	sunpy-sphinx-theme
+	sphinx-design
+	sphinx_changelog
 
 [options.package_data]
 stixpy = data/*
 
 [tool:pytest]
 testpaths = "stixpy" "docs"
+norecursedirs = _build
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
 remote_data_strict = True
 filterwarnings = 
 	ignore:defusedxml.lxml is no longer supported:DeprecationWarning
 	ignore:Matplotlib is currently using agg:UserWarning
```

### Comparing `stixpy-0.1.0rc2/setup.py` & `stixpy-0.1.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-cal-energy_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-cal-energy_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-hk-maxi_20200501_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-hk-maxi_20200501_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-background_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-background_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-flareflag_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-flareflag_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-lightcurve_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-lightcurve_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-ql-tmstatusflarelist_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-ql-tmstatusflarelist_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-spectra_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-spectra_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-ql-variance_20200506_V01.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-ql-variance_20200506_V01.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-cpd_20200505T235959-20200506T000019_V01_0087031809-50883.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-cpd_20200505T235959-20200506T000019_V01_0087031809-50883.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-rpd_20200505T235959-20200506T000019_V01_0087031808-50882.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-rpd_20200505T235959-20200506T000019_V01_0087031808-50882.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-scpd_20200505T235959-20200506T000019_V01_0087031810-50884.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-scpd_20200505T235959-20200506T000019_V01_0087031810-50884.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/solo_L1_stix-sci-xray-spec_20200505T235959-20200506T000019_V01_0087031812-50886.fits` & `stixpy-0.1.0rc3/stixpy/data/solo_L1_stix-sci-xray-spec_20200505T235959-20200506T000019_V01_0087031812-50886.fits`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/test.py` & `stixpy-0.1.0rc3/stixpy/data/test.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/data/test_data.tar.gz` & `stixpy-0.1.0rc3/stixpy/data/test_data.tar.gz`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/frames.py` & `stixpy-0.1.0rc3/stixpy/frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from astropy.time import Time
 from sunpy.coordinates.frames import HeliographicStonyhurst, Helioprojective, \
     SunPyBaseCoordinateFrame
 from sunpy.coordinates.transformations import _check_observer_defined
 from sunpy.net import Fido, attrs as a
 from sunpy.util.exceptions import warn_user
 
-from stixcore.util.logging import get_logger
+from stixpy.utils.logging import get_logger
 from stixpy.net.client import STIXClient  # noqa
 
 logger = get_logger(__name__, 'DEBUG')
 
 __all__ = ['STIXImagingFrame', '_get_rotation_matrix_and_position', 'hpc_to_stixim', 'stixim_to_hpc']
 
 STIX_X_SHIFT = 26.1 * u.arcsec  # fall back to this when non sas solution available
```

### Comparing `stixpy-0.1.0rc2/stixpy/net/attrs.py` & `stixpy-0.1.0rc3/stixpy/net/attrs.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/net/client.py` & `stixpy-0.1.0rc3/stixpy/net/client.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/net/tests/test_client.py` & `stixpy-0.1.0rc3/stixpy/net/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/science.py` & `stixpy-0.1.0rc3/stixpy/product/sources/science.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from sunpy.time.timerange import TimeRange
 
 __all__ = ['ScienceData', 'RawPixelData', 'CompressedPixelData', 'SummedCompressedPixelData',
            'Visibility', 'Spectrogram', 'TimesSeriesPlotMixin', 'SpectrogramPlotMixin',
            'PixelPlotMixin', 'PPrintMixin', 'IndexMasks', 'DetectorMasks', 'PixelMasks',
            'EnergyMasks']
 
+from stixpy.product.product import L1Product
+
 quantity_support()
 
 
 class PPrintMixin:
     """
     Provides pretty printing for index masks.
     """
@@ -381,45 +383,43 @@
                         + count_err[time_index, did, pid, energy_index]
                     bars[1].set_segments(segs)
 
         senergy.on_changed(update)
         stime.on_changed(update)
 
 
-class ScienceData:
+class ScienceData(L1Product):
     """
     Basic science data class
     """
-    def __init__(self, *, header, control, data, energies):
+    def __init__(self, *, meta, control, data, energies, idb_versions=None):
         """
 
         Parameters
         ----------
         header : `astropy.fits.Header`
             Fits header
         control : `astropy.table.QTable`
             Fits file control extension
         data :` astropy.table.QTable`
             Fits file data extension
         energies : `astropy.table.QTable`
             Fits file energy extension
         """
+        super().__init__(meta=meta, control=control, data=data,
+                         energies=energies, idb_versions=idb_versions)
+
         self.count_type = 'rate'
-        self.header = header
-        self.control = control
-        self.data = data
-        self.energies_ = energies
         if 'detector_masks' in self.data.colnames:
             self.detector_masks = DetectorMasks(self.data['detector_masks'])
         if 'pixel_masks' in self.data.colnames:
             self.pixel_masks = PixelMasks(self.data['pixel_masks'])
-        if 'energy_bin_mask' in self.control.colnames:
-            self.energy_masks = EnergyMasks(self.control['energy_bin_mask'])
-            self.dE = (energies['e_high'] - energies['e_low'])[self.energy_masks.masks[0] == 1]
-            #
+        if 'energy_bin_edge_mask' in self.control.colnames:
+            self.energy_masks = EnergyMasks(self.control['energy_bin_edge_mask'])
+            self.dE = energies['e_high'] - energies['e_low']
 
     @property
     def time_range(self):
         """
         A `sunpy.time.TimeRange` for the data.
         """
         return TimeRange(self.data['time'][0] - self.data['timedel'][0]/2,
@@ -440,23 +440,30 @@
         return self.detector_masks
 
     @property
     def energies(self):
         """
         A `astropy.table.Table` object representing the energies contained in the data.
         """
-        return self.energies_[self.energy_masks.masks[0] == 1]
+        return self._energies
 
     @property
     def times(self):
         """
         An `astropy.time.Time` array representing the center of the observed time bins.
         """
         return self.data['time']
 
+    @property
+    def durtaion(self):
+        """
+        An `astropy.units.Quantiy` array giving the duration or integration time
+        """
+        return self.data['timedel']
+
     def get_data(self, time_indices=None, energy_indices=None, detector_indices=None,
                  pixel_indices=None, sum_all_times=False):
         """
         Return the counts, errors, times, durations and energies for selected data.
 
         Optionally summing in time and or energy.
 
@@ -484,15 +491,18 @@
         Returns
         -------
         `tuple`
             Counts, errors, times, deltatimes,  energies
 
         """
         counts = self.data['counts']
-        counts_var = self.data['counts_err']**2
+        try:
+            counts_var = self.data['counts_comp_err']**2
+        except KeyError:
+            counts_var = self.data['counts_comp_comp_err'] ** 2
         shape = counts.shape
         if len(shape) < 4:
             counts = counts.reshape(shape[0], 1, 1, shape[-1])
             counts_var = counts_var.reshape(shape[0], 1, 1, shape[-1])
 
         energies = self.energies[:]
         times = self.times
@@ -545,15 +555,15 @@
                     [np.sum(counts_var[..., el:eh+1], axis=-1, keepdims=True)
                      for el, eh in energy_indices], axis=-1)
 
                 e_norm = np.hstack([(energies['e_high'][eh] - energies['e_low'][el])
                                     for el, eh in energy_indices])
 
                 energies = np.atleast_2d(
-                    [(self.energies_['e_low'][el].value, self.energies_['e_high'][eh].value)
+                    [(self._energies['e_low'][el].value, self._energies['e_high'][eh].value)
                      for el, eh in energy_indices])
                 energies = QTable(energies*u.keV, names=['e_low', 'e_high'])
 
         t_norm = self.data['timedel']
         if time_indices is not None:
             time_indices = np.asarray(time_indices)
             if time_indices.ndim == 1:
@@ -627,61 +637,24 @@
                      for table in [control, other.control, data, other.data]]
                 except KeyError:
                     pass
 
                 control = vstack([control, other.control])
                 data = vstack([data, other.data])
 
-            return type(self)(header=self.header, control=control, data=data,
-                              energies=self.energies)
+            return type(self)(meta=self.meta, control=control, data=data,
+                              energies=self.energies, idb_version=self.idb_versions)
 
     def __repr__(self):
         return f'{self.__class__.__name__}' \
                f'{self.time_range}' \
                f'    {self.detector_masks}\n' \
                f'    {self.pixel_masks}\n' \
                f'    {self.energy_masks}'
 
-    @classmethod
-    def from_fits(cls, file):
-        """
-        Parses STIX FITS data files to create science products.
-        Should only be applied to L1 fits files (not L1A)
-
-        Parameters
-        ----------
-        file : `str` or `pathlib.Path`
-            The path to the file to open read.
-        """
-
-        file = Path(file)
-        header = fits.getheader(file)
-        control = QTable.read(file, hdu=1)
-        data = QTable.read(file, hdu=2)
-        data['time'] = Time(header['date-obs']) + TimeDelta(data['time'])
-        energies = QTable.read(file, hdu=4)
-
-        #TODO Fix time before FSW update
-
-        filename = file.name
-        if 'xray-rpd' in filename:
-            return RawPixelData(header=header, control=control, data=data, energies=energies)
-        elif 'xray-cpd' in filename:
-            return CompressedPixelData(header=header, control=control,
-                                       data=data, energies=energies)
-        elif 'xray-scpd' in filename:
-            return SummedCompressedPixelData(header=header, control=control,
-                                             data=data, energies=energies)
-        elif 'xray-vis' in filename:
-            return Visibility(header=header, control=control, data=data, energies=energies)
-        elif 'xray-spec' in filename:
-            return Spectrogram(header=header, control=control, data=data, energies=energies)
-        else:
-            raise TypeError(f'File {file} does not contain pixel data')
-
 
 class RawPixelData(ScienceData, PixelPlotMixin, TimesSeriesPlotMixin, SpectrogramPlotMixin):
     """
     Uncompressed or raw count data from selected pixels, detectors and energies.
 
     Examples
     --------
@@ -705,14 +678,22 @@
     <BLANKLINE>
         EnergyMasks
         [0]: [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]
     <BLANKLINE>
     """
     pass
 
+    @classmethod
+    def is_datasource_for(cls, *, meta, **kwargs):
+        """Determines if meta data meach Raw Pixel Data"""
+        service_subservice_ssid = tuple(meta[name] for name in ['STYPE', 'SSTYPE', 'SSID'])
+        level = meta['level']
+        if service_subservice_ssid == (21, 6, 20) and level == 'L1':
+            return True
+
 
 class CompressedPixelData(ScienceData, PixelPlotMixin, TimesSeriesPlotMixin, SpectrogramPlotMixin):
     """
     Compressed count data from selected pixels, detectors and energies.
 
     Examples
     --------
@@ -733,15 +714,22 @@
     <BLANKLINE>
         PixelMasks
         [0...4]: [['1' '1' '1' '1' '1' '1' '1' '1' '1' '1' '1' '1']]
     <BLANKLINE>
         EnergyMasks
         [0]: [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]
     """
-    pass
+
+    @classmethod
+    def is_datasource_for(cls, *, meta, **kwargs):
+        """Determines if meta data meach Raw Pixel Data"""
+        service_subservice_ssid = tuple(meta[name] for name in ['STYPE', 'SSTYPE', 'SSID'])
+        level = meta['level']
+        if service_subservice_ssid == (21, 6, 21) and level == 'L1':
+            return True
 
 
 class SummedCompressedPixelData(ScienceData, PixelPlotMixin, TimesSeriesPlotMixin,
                                 SpectrogramPlotMixin):
     """
     Compressed and Summed count data from selected pixels, detectors and energies.
 
@@ -769,14 +757,22 @@
      ['1' '0' '0' '0' '1' '0' '0' '0' '1' '0' '0' '0']]]
     <BLANKLINE>
         EnergyMasks
         [0]: [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]
     """
     pass
 
+    @classmethod
+    def is_datasource_for(cls, *, meta, **kwargs):
+        """Determines if meta data meach Raw Pixel Data"""
+        service_subservice_ssid = tuple(meta[name] for name in ['STYPE', 'SSTYPE', 'SSID'])
+        level = meta['level']
+        if service_subservice_ssid == (21, 6, 22) and level == 'L1':
+            return True
+
 
 class Visibility(ScienceData):
     """
     Compressed visibilities from selected pixels, detectors and energies.
 
     Examples
     --------
@@ -858,21 +854,29 @@
     #  ['0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '0.0' '1.0']]]
     # <BLANKLINE>
     #     EnergyMasks
     #     [0]: [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]
     # <BLANKLINE>
     """
     def __init__(self, *, header, control, data, energies):
-        super().__init__(header=header, control=control, data=data, energies=energies)
+        super().__init__(meta=header, control=control, data=data, energies=energies)
         self.pixel_masks = PixelMasks(self.pixels)
 
     @property
     def pixels(self):
         return np.vstack([self.data[f'pixel_mask{i}'][0] for i in range(1, 6)])
 
+    @classmethod
+    def is_datasource_for(cls, *, meta, **kwargs):
+        """Determines if meta data meach Raw Pixel Data"""
+        service_subservice_ssid = tuple(meta[name] for name in ['STYPE', 'SSTYPE', 'SSID'])
+        level = meta['level']
+        if service_subservice_ssid == (21, 6, 23) and level == 'L1':
+            return True
+
 
 class Spectrogram(ScienceData, TimesSeriesPlotMixin, SpectrogramPlotMixin):
     """
     Spectrogram from selected pixels, detectors and energies.
 
     Parameters
     ----------
@@ -901,36 +905,41 @@
         PixelMasks
         [0...4]: [['0' '0' '0' '0' '0' '0' '0' '0' '0' '0' '0' '0']]
     <BLANKLINE>
         EnergyMasks
         [0]: [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31]
     <BLANKLINE>
     """
-    def __init__(self, *, header, control, data, energies):
+    def __init__(self, *, meta, control, data, energies, idb_versions):
         """
 
         Parameters
         ----------
         header : astropy.fits.Header
         control : astropy.table.QTable
         data : astropy.table.QTable
         energies : astropy.table.QTable
         """
-        super().__init__(header=header, control=control, data=data, energies=energies)
+        super().__init__(meta=meta, control=control, data=data,
+                         energies=energies, idb_versions=idb_versions)
         self.count_type = 'rate'
-        self.header = header
-        self.control = control
-        self.data = data
-        self.energies_ = energies
         self.detector_masks = DetectorMasks(self.control['detector_masks'])
         self.pixel_masks = PixelMasks(self.data['pixel_masks'])
         self.energy_masks = EnergyMasks(self.control['energy_bin_mask'])
         self.dE = (energies['e_high'] - energies['e_low'])[self.energy_masks.masks[0] == 1]
         # self.dE = np.hstack([[1], np.diff(energies['e_low'][1:]).value, [1]]) * u.keV
 
+    @classmethod
+    def is_datasource_for(cls, *, meta, **kwargs):
+        """Determines if meta data meach Raw Pixel Data"""
+        service_subservice_ssid = tuple(meta[name] for name in ['STYPE', 'SSTYPE', 'SSID'])
+        level = meta['level']
+        if service_subservice_ssid == (21, 6, 24) and level == 'L1':
+            return True
+
 
 class SliderCustomValue(Slider):
     """
     A slider with a customisable formatter
     """
     def __init__(self, *args, format_func=None, **kwargs):
         if format_func is not None:
```

### Comparing `stixpy-0.1.0rc2/stixpy/tests/test_frames.py` & `stixpy-0.1.0rc3/stixpy/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/tests/test_science.py` & `stixpy-0.1.0rc3/stixpy/tests/test_science.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 import astropy.units as u
 import numpy as np
 
 from stixpy.data import test
-from stixpy.science import *
+from stixpy.product.sources import CompressedPixelData, SummedCompressedPixelData, Spectrogram, RawPixelData
+from stixpy.science import ScienceData
 
 
 def test_sciencedata_get_data():
     l1 = ScienceData.from_fits(test.STIX_SCI_XRAY_CPD)
     tot = l1.data['counts']
     norm = (l1.data['timedel'].reshape(5, 1, 1, 1) * l1.dE)
     rate = tot / norm
-    error = np.sqrt(tot*u.ct+l1.data['counts_err']**2) / norm
+    error = np.sqrt(tot*u.ct+l1.data['counts_comp_err']**2) / norm
     r, re, t, dt, e = l1.get_data()
     assert np.allclose(rate, r)
     assert np.allclose(error, re)
 
     # Detector sum
     tot = l1.data['counts'][:, 0:32, ...].sum(axis=1, keepdims=True)
     norm = (l1.data['timedel'].reshape(5, 1, 1, 1) * l1.dE)
     rate = tot / norm
-    error = np.sqrt(tot*u.ct+l1.data['counts_err'][:, 0:32, ...].sum(axis=1, keepdims=True)**2)/norm
+    error = np.sqrt(tot*u.ct+l1.data['counts_comp_err'][:, 0:32, ...].sum(axis=1, keepdims=True)**2)/norm
     r, re, t, dt, e = l1.get_data(detector_indices=[[0, 31]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re, atol=1e-3)
 
     # Pixel sum
     tot = l1.data['counts'][..., 0:12, :].sum(axis=2, keepdims=True)
     norm = (l1.data['timedel'].reshape(5, 1, 1, 1) * l1.dE)
     rate = tot / norm
     error = np.sqrt(tot * u.ct
-                    + l1.data['counts_err'][..., 0:12, :].sum(axis=2, keepdims=True)**2) / norm
+                    + l1.data['counts_comp_err'][..., 0:12, :].sum(axis=2, keepdims=True)**2) / norm
     r, re, t, dt, e = l1.get_data(pixel_indices=[[0, 11]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re)
 
     # Detector and Pixel sum
     tot = l1.data['counts'][:, 0:32, 0:12, :].sum(axis=(1, 2), keepdims=True)
     norm = (l1.data['timedel'].reshape(5, 1, 1, 1) * l1.dE)
     rate = tot / norm
-    error = np.sqrt(tot*u.ct + l1.data['counts_err'][:, 0:32, 0:12, :].sum(axis=(1, 2),
+    error = np.sqrt(tot*u.ct + l1.data['counts_comp_err'][:, 0:32, 0:12, :].sum(axis=(1, 2),
                                                                            keepdims=True)**2) / norm
     r, re, t, dt, e = l1.get_data(pixel_indices=[[0, 11]], detector_indices=[[0, 31]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re, atol=1e-3)
 
     # Energy sum
     tot = l1.data['counts'][..., 1:31].sum(axis=3, keepdims=True)
     norm = (l1.data['timedel'].reshape(5, 1, 1, 1)
             * (l1.energies[30]['e_high']-l1.energies[1]['e_low']))
     rate = tot / norm
-    error = np.sqrt(tot*u.ct + l1.data['counts_err'][..., 1:31].sum(axis=3, keepdims=True)**2)/norm
+    error = np.sqrt(tot*u.ct + l1.data['counts_comp_err'][..., 1:31].sum(axis=3, keepdims=True)**2)/norm
     r, re, t, dt, e = l1.get_data(energy_indices=[[1, 30]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re, atol=1e-3)
 
     # Time sum
     tot = l1.data['counts'][:, ...].sum(axis=0, keepdims=True)
     norm = (l1.data['timedel'].sum() * l1.dE)
     rate = tot / norm
-    error = np.sqrt(tot * u.ct + l1.data['counts_err'][:, ...].sum(axis=0, keepdims=True) ** 2)/norm
+    error = np.sqrt(tot * u.ct + l1.data['counts_comp_err'][:, ...].sum(axis=0, keepdims=True) ** 2)/norm
     r, re, t, dt, e = l1.get_data(time_indices=[[0, 4]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re)
 
     # Sum everything down to one number
     tot = l1.data['counts'][..., 1:31].sum(keepdims=True)
     norm = (l1.data['timedel'].sum() * (l1.energies[30]['e_high'] - l1.energies[1]['e_low']))
     rate = tot/norm
-    error = np.sqrt(tot * u.ct + l1.data['counts_err'][..., 1:31].sum(keepdims=True) ** 2) / norm
+    error = np.sqrt(tot * u.ct + l1.data['counts_comp_err'][..., 1:31].sum(keepdims=True) ** 2) / norm
     r, re, t, dt, e = l1.get_data(time_indices=[[0, 4]], energy_indices=[[1, 30]],
                                   pixel_indices=[[0, 11]], detector_indices=[[0, 31]])
     assert np.allclose(rate, r)
     assert np.allclose(error, re, atol=1e-3)
 
     # Overwrite data with known values
     # 5 seconds, with dE 1/30keV across 30 channels
-    l1.data['counts'] = 146/(5*30) * u.ct
-    l1.data.remove_column('counts_err')
-    l1.data['counts_err'] = np.full_like(l1.data['counts'], np.sqrt(146*145/(5*30))*u.ct)
+    l1.data.remove_column('counts') # need to remove and add to avoid error regarding casting
+    l1.data['counts'] = np.full((5, 32, 12, 32), 146/(5*30))*u.ct
+    l1.data.remove_column('counts_comp_err')
+    l1.data['counts_comp_err'] = np.full_like(l1.data['counts'], np.sqrt(146*145/(5*30))*u.ct)
     l1.data['timedel'] = 1/5*u.s
     l1.dE[:] = ((1/30)*u.keV).astype(np.float32)
     l1.energies['e_high'][1:-1] = ((np.arange(31) / 30)[1:] * u.keV).astype(np.float32)
     l1.energies['e_low'][1:-1] = ((np.arange(31) / 30)[:-1] * u.keV).astype(np.float32)
     l1.data['time'] = l1.time_range.start + np.arange(5)/5*u.s
     count, count_err, times, timedel, energies = l1.get_data(time_indices=[[0, 4]],
                                                              energy_indices=[[1, 30]])
```

### Comparing `stixpy-0.1.0rc2/stixpy/timeseries/quicklook.py` & `stixpy-0.1.0rc3/stixpy/timeseries/quicklook.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     Nominally in 5 energy bands from 4 - 150 kev
 
     Examples
     --------
     >>> from stixpy.data import test
     >>> from sunpy.timeseries import TimeSeries
     >>> from stixpy.timeseries.quicklook import QLLightCurve
-    >>> lc = TimeSeries(test.STIX_QL_LIGHTCURVE_TIMESERIES)
-    >>> lc
+    >>> ql_lc = TimeSeries(test.STIX_QL_LIGHTCURVE_TIMESERIES)
+    >>> ql_lc # doctest: +SKIP
     QLLightCurve
            <sunpy.time.timerange.TimeRange object at ...>
         Start: 2020-05-06 00:00:01
         End:   2020-05-06 23:59:57
         Center:2020-05-06 11:59:59
         Duration:0.9999538194444444 days or
                23.998891666666665 hours or
@@ -155,28 +155,32 @@
 
         data['counts'] = data['counts'] / (live_time.reshape(-1, 1) * energy_delta)
 
         names = ['{:d}-{:d} keV'.format(energies["e_low"][i].astype(int),energies["e_high"][i].astype(int)) for i in range(5)]
 
         [data.add_column(data['counts'][:, i], name=names[i]) for i in range(5)]
         data.remove_column('counts')
-        [data.add_column(data['counts_err'][:, i], name=f'{names[i]}_err') for i in range(5)]
-        data.remove_column('counts_err')
-        data['time'] = Time(header['date-obs']) + data['time'] * u.cs
+        [data.add_column(data['counts_comp_err'][:, i], name=f'{names[i]}_comp_err') for i in range(5)]
+        data.remove_column('counts_comp_err')
+
+        try:
+            data['time'] = Time(header['date_obs']) + data['time'] * u.cs
+        except KeyError:
+            data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.cs)
 
         units = OrderedDict([('control_index', None),
                              ('timedel', u.s),
                              ('triggers', None),
-                             ('triggers_err', None),
+                             ('triggers_comp_err', None),
                              ('rcr', None)])
         units.update([(name, u.ct) for name in names])
-        units.update([(f'{name}_err', u.ct) for name in names])
+        units.update([(f'{name}_comp_err', u.ct) for name in names])
 
         data['triggers'] = data['triggers'].reshape(-1)
-        data['triggers_err'] = data['triggers_err'].reshape(-1)
+        data['triggers_comp_err'] = data['triggers_comp_err'].reshape(-1)
 
         data_df = data.to_pandas()
         data_df.index = data_df['time']
         data_df.drop(columns='time', inplace=True)
 
         return data_df, header, units
 
@@ -205,17 +209,45 @@
     Quicklook X-ray background detector time series.
 
     Examples
     --------
     >>> from stixpy.data import test
     >>> from sunpy.timeseries import TimeSeries
     >>> from stixpy.timeseries.quicklook import QLLightCurve
-    >>> bg = TimeSeries(test.STIX_QL_BACKGROUND_TIMESERIES)
-    >>> bg
-    <stixpy.timeseries.quicklook.QLBackground object at ...>
+    >>> ql_bg = TimeSeries(test.STIX_QL_BACKGROUND_TIMESERIES)
+    >>> ql_bg # doctest: +SKIP
+    <stixpy.timeseries.quicklook.QLBackground object at ...
+    SunPy TimeSeries
+    ----------------
+     Observatory:		 SOLO/STIX
+     Instrument:		 STIX
+     Channel(s):		 control_index<br>timedel<br>triggers<br>triggers_err<br>4.0-10.0<br>10.0-15.0<br>15.0-25.0<br>25.0-50.0<br>50.0-150.0<br>4.0-10.0_err<br>10.0-15.0_err<br>15.0-25.0_err<br>25.0-50.0_err<br>50.0-150.0_err
+     Start Date:		 2020-05-06 00:00:04
+     End Date:		 2020-05-06 23:59:56
+     Center Date:		 2020-05-06 11:59:59
+     Resolution:		 8.03 s
+     Samples per Channel:		 10758
+     Data Range(s):		 control_index    1.60E+01<br>timedel          0.00E+00<br>triggers         1.10E+03<br>triggers_err     3.23E+01<br>4.0-10.0         7.72E+01<br>10.0-15.0        1.34E+02<br>15.0-25.0        6.07E+01<br>25.0-50.0        2.17E+01<br>50.0-150.0       4.95E+00<br>4.0-10.0_err     9.25E+00<br>10.0-15.0_err    1.85E+01<br>15.0-25.0_err    1.85E+01<br>25.0-50.0_err    1.85E+01<br>50.0-150.0_err   9.25E+00
+     Units:		 None<br>ct<br>s
+                              control_index  timedel  ...  25.0-50.0_err  50.0-150.0_err
+     time                                             ...
+     2020-05-06 00:00:03.531              3      800  ...       2.345208        0.707107
+     2020-05-06 00:00:11.531              3      800  ...       2.345208        0.707107
+     2020-05-06 00:00:19.531              3      800  ...       2.345208        0.000000
+     2020-05-06 00:00:27.531              3      800  ...       2.345208        0.000000
+     2020-05-06 00:00:35.531              3      800  ...       2.345208        0.000000
+     ...                                ...      ...  ...            ...             ...
+     2020-05-06 23:59:23.531              2      800  ...       0.707107        1.224745
+     2020-05-06 23:59:31.531              2      800  ...       0.000000        2.345208
+     2020-05-06 23:59:39.531              2      800  ...       0.000000        4.636809
+     2020-05-06 23:59:47.531              2      800  ...       0.000000        1.224745
+     2020-05-06 23:59:55.531              2      800  ...       0.707107        2.345208
+     <BLANKLINE>
+     [10758 rows x 14 columns]
+
     """
     @peek_show
     def peek(self, **kwargs):
         """
         Displays a graphical overview of the data in this object for user evaluation.
         For the creation of plots, users should instead use the
         `.plot` method and Matplotlib's pyplot framework.
@@ -319,31 +351,34 @@
         data['counts'] = data['counts'] / (live_time.reshape(-1, 1) * energy_delta)
 
         names = [f'{energies["e_low"][i]}-{energies["e_high"][i]}' for i in range(5)]
 
         [data.add_column(data['counts'][:, i], name=names[i]) for i in range(5)]
         data.remove_column('counts')
 
-        [data.add_column(data['counts_err'][:, i], name=f'{names[i]}_err') for i in range(5)]
-        data.remove_column('counts_err')
+        [data.add_column(data['counts_comp_err'][:, i], name=f'{names[i]}_comp_err') for i in range(5)]
+        data.remove_column('counts_comp_err')
 
-        data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.cs)
+        try:
+            data['time'] = Time(header['date_obs']) + TimeDelta(data['time'] * u.s)
+        except KeyError:
+            data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.s)
 
         # [f'{energies[i]["e_low"]} - {energies[i]["e_high"]} keV' for i in range(5)]
 
         units = OrderedDict([('control_index', None),
                              ('timedel', u.s),
                              ('triggers', None),
-                             ('triggers_err', None),
+                             ('triggers_comp_err', None),
                              ('rcr', None)])
         units.update([(name, u.ct) for name in names])
-        units.update([(f'{name}_err', u.ct) for name in names])
+        units.update([(f'{name}_comp_err', u.ct) for name in names])
 
         data['triggers'] = data['triggers'].reshape(-1)
-        data['triggers_err'] = data['triggers_err'].reshape(-1)
+        data['triggers_comp_err'] = data['triggers_comp_err'].reshape(-1)
 
         data_df = data.to_pandas()
         data_df.index = data_df['time']
         data_df.drop(columns='time', inplace=True)
 
         return data_df, header, units
 
@@ -368,17 +403,44 @@
     Quicklook X-ray background detector time series.
 
     Examples
     --------
     >>> from stixpy.data import test
     >>> from sunpy.timeseries import TimeSeries
     >>> from stixpy.timeseries.quicklook import QLLightCurve
-    >>> bg = TimeSeries(test.STIX_QL_VARIANCE_TIMESERIES)
-    >>> bg
+    >>> ql_var = TimeSeries(test.STIX_QL_VARIANCE_TIMESERIES)
+    >>> ql_var # doctest: +SKIP
     <stixpy.timeseries.quicklook.QLVariance object at ...>
+    SunPy TimeSeries
+    ----------------
+    Observatory:		 SOLO/STIX
+    Instrument:		     STIX
+    Channel(s):		     timedel<br>control_index<br>4.0-20.0<br>4.0-20.0_err
+    Start Date:		     2020-05-06 00:00:02
+    End Date:		  2020-05-06 23:59:58
+    Center Date:		 2020-05-06 11:59:59
+    Resolution:		 4.015 s
+    Samples per Channel:		 21516
+    Data Range(s):		 timedel         0.00E+00<br>control_index   6.00E+00<br>4.0-20.0        4.93E+00<br>4.0-20.0_err    5.87E+02
+    Units:		 ct<br>s<br>None
+                             timedel  control_index  4.0-20.0  4.0-20.0_err
+    time
+    2020-05-06 00:00:01.531      400              2  0.419844     73.901962
+    2020-05-06 00:00:05.531      400              2  0.169844     36.952671
+    2020-05-06 00:00:09.531      400              2  0.154844     18.479719
+    2020-05-06 00:00:13.531      400              2  1.359844    295.603607
+    2020-05-06 00:00:17.531      400              2  0.114844     18.479719
+    ...                          ...            ...       ...           ...
+    2020-05-06 23:59:41.531      400              1  0.919844    147.802231
+    2020-05-06 23:59:45.531      400              1  0.919844    147.802231
+    2020-05-06 23:59:49.531      400              1  2.159844    295.603607
+    2020-05-06 23:59:53.531      400              1  0.094844     18.479719
+    2020-05-06 23:59:57.531      400              1  0.154844     18.479719
+    <BLANKLINE>
+    [21516 rows x 4 columns]
     """
     def plot(self, axes=None, **plot_args):
         """
         Show a plot of the data.
 
         Parameters
         ----------
@@ -456,30 +518,34 @@
         header['control'] = control
         data = Table(hdulist[2].data)
         energies = Table(hdulist[4].data)
         dE = energies[control['energy_bin_mask'][0]]['e_high'][-1] \
              - energies[control['energy_bin_mask'][0]]['e_low'][0] << u.keV
         name = f'{energies[control["energy_bin_mask"][0]]["e_low"][0]}' \
                f'-{energies[control["energy_bin_mask"][0]]["e_high"][-1]}'
-        data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.cs)
+
+        try:
+            data['time'] = Time(header['date_obs']) + TimeDelta(data['time'] * u.s)
+        except KeyError:
+            data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.s)
 
         data['variance'] = data['variance'].reshape(-1)/(dE * data['timedel'])
 
         data.add_column(data['variance'], name=name)
         data.remove_column('variance')
-        data.add_column(data['variance_err'], name=f'{name}_err')
-        data.remove_column('variance_err')
+        data.add_column(data['variance_comp_err'], name=f'{name}_comp_err')
+        data.remove_column('variance_comp_err')
 
         units = OrderedDict([('control_index', None),
                              ('timedel', u.s),
                              (name, u.count),
-                             (f'{name}_err', u.count)])
+                             (f'{name}_comp_err', u.count)])
 
         data[name] = data[name].reshape(-1)
-        data[f'{name}_err'] = data[f'{name}_err'].reshape(-1)
+        data[f'{name}_comp_err'] = data[f'{name}_comp_err'].reshape(-1)
 
         data_df = data.to_pandas()
         data_df.index = data_df['time']
         data_df.drop(columns='time', inplace=True)
 
         return data_df, header, units
 
@@ -497,23 +563,23 @@
         if 'meta' in kwargs.keys():
             return (kwargs['meta'].get('telescop', '') == 'SOLO/STIX'
                     and 'ql-variance' in kwargs['meta']['filename'])
 
 
 class HKMaxi(GenericTimeSeries):
     """
-    House Keeping Maxi Report.
+    Housekeeping Maxi Report.
 
     Examples
     --------
     >>> from stixpy.data import test
     >>> from sunpy.timeseries import TimeSeries
     >>> from stixpy.timeseries.quicklook import HKMaxi
     >>> hk = TimeSeries(test.STIX_HK_MAXI_TIMESERIES)
-    >>> hk
+    >>> hk  # doctest: +SKIP
     <stixpy.timeseries.quicklook.HKMaxi ...>
     """
     # def plot(self, axes=None, **plot_args):
     #     """
     #     Show a plot of the data.
     #
     #     Parameters
@@ -588,15 +654,18 @@
             The path to the file you want to parse.
         """
         header = hdulist[0].header
         control = Table(hdulist[1].data)
         header['control'] = control
         data = Table(hdulist[2].data)
 
-        data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.cs)
+        try:
+            data['time'] = Time(header['date_obs']) + TimeDelta(data['time'] * u.s)
+        except KeyError:
+            data['time'] = Time(header['date-obs']) + TimeDelta(data['time'] * u.s)
 
         data_df = data.to_pandas()
         data_df.index = data_df['time']
         data_df.drop(columns='time', inplace=True)
 
         return data_df, header, None
```

### Comparing `stixpy-0.1.0rc2/stixpy/timeseries/tests/test_quicklook.py` & `stixpy-0.1.0rc3/stixpy/timeseries/tests/test_quicklook.py`

 * *Files identical despite different names*

### Comparing `stixpy-0.1.0rc2/stixpy/vis/map_reprojection.py` & `stixpy-0.1.0rc3/stixpy/visualisation/map_reprojection.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
    :include-source: true
 
    import astropy.units as u
    from astropy.coordinates import SkyCoord
    from sunpy.net import Fido, attrs as a
    from sunpy.map import Map
    from sunpy.coordinates.frames import HeliographicStonyhurst
-   from stixpy.vis.map_reprojection import reproject_map, plot_map_reproj, get_solo_position
+   from stixpy.visualisation.map_reprojection import reproject_map, plot_map_reproj, get_solo_position
 
    # Search and download map using FIDO
    aia = (a.Instrument.aia &
        a.Sample(24 * u.hour) &
        a.Time('2021-04-17', '2021-04-18'))
    wave = a.Wavelength(19.3 * u.nm, 19.3 * u.nm)
    query = Fido.search(wave, aia)
@@ -44,15 +44,15 @@
    :include-source: true
 
    import astropy.units as u
    from astropy.coordinates import SkyCoord
    from sunpy.net import Fido, attrs as a
    from sunpy.map import Map
    from sunpy.coordinates.frames import HeliographicStonyhurst
-   from stixpy.vis.map_reprojection import reproject_map, plot_map_reproj, get_solo_position
+   from stixpy.visualisation.map_reprojection import reproject_map, plot_map_reproj, get_solo_position
 
    # Search and download map using FIDO
    query = Fido.search(a.Time('2020/06/12 13:20:00', '2020/06/12 13:40:00'),
                        a.Instrument.hmi, a.Physobs.los_magnetic_field)
    result = Fido.fetch(query[0][0])
 
    # Create map and resample to speed up calculations
@@ -69,29 +69,32 @@
 
    # Run plotting function
    plot_map_reproj(map, reprojected_map)
 
 
 """
 
-
-from pathlib import Path
-
 import astropy.units as u
 import matplotlib.pyplot as plt
-import stixcore.data.test
+
 import sunpy
 from astropy.coordinates import SkyCoord
 from astropy.wcs import WCS
 from reproject import reproject_interp
-from stixcore.ephemeris.manager import Spice
-from stixcore.data.test import test_data
+try:
+    from stixcore.ephemeris.manager import Spice
+except (ImportError, ModuleNotFoundError):
+    Spice = None
 from sunpy.coordinates import frames
 from sunpy.coordinates import get_body_heliographic_stonyhurst
 
+from stixpy.utils.logging import get_logger
+
+logger = get_logger(__name__)
+
 __all__ = ['get_solo_position', 'reproject_map', 'create_headers', 'plot_map_reproj']
 
 
 def get_solo_position(map):
     """
     Return the position of SOLO at the time the map was observed
 
@@ -101,21 +104,25 @@
         Map to reproject to be as seen from SOLO
 
     Returns
     -------
     solo_hgs : `astropy.coordinates.SkyCoord`
         The position of SOLO in HeliographicStonyhurst frame
     """
-    p = Spice.instance.get_position(date=map.date.datetime, frame='SOLO_HEE')
-    solo_hee = SkyCoord(*p, frame=frames.HeliocentricEarthEcliptic, representation_type='cartesian',
-                        obstime=map.date.datetime)
-    # Converting HeliocentricEarthEcliptic coords of SOLAR ORBITER position to
-    # HeliographicStonyhurst frame
-    solo_hgs = solo_hee.transform_to(frames.HeliographicStonyhurst)
-    return solo_hgs
+    if Spice is not None:
+        logger.info('Using Spice')
+        p = Spice.instance.get_position(date=map.date.datetime, frame='SOLO_HEE')
+        solo_hee = SkyCoord(*p, frame=frames.HeliocentricEarthEcliptic, representation_type='cartesian',
+                            obstime=map.date.datetime)
+        # Converting HeliocentricEarthEcliptic coords of SOLAR ORBITER position to
+        # HeliographicStonyhurst frame
+        solo_hgs = solo_hee.transform_to(frames.HeliographicStonyhurst)
+    else:
+        logger.info('Spice not configured falling back to JPL ')
+        solo_hgs = get_horizons_coord('solo', time=map.date)
 
 
 def create_headers(obs_ref_coord, map, out_shape=None, out_scale=None):
     """
     Generates MetaDict and WCS headers for reprojected map
 
     Parameters
```

### Comparing `stixpy-0.1.0rc2/stixpy/vis/tests/test_map_reprojection.py` & `stixpy-0.1.0rc3/stixpy/visualisation/tests/test_map_reprojection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import pytest
 from unittest.mock import patch
 
 import astropy.units as u
 import numpy as np
 from astropy.time.core import Time
 from sunpy.data import sample
 from sunpy.map import Map
 
-from stixpy.vis.map_reprojection import get_solo_position, reproject_map
-
+from stixpy.visualisation.map_reprojection import get_solo_position, reproject_map
 
+@pytest.mark.skip
 @patch('sunpy.map.GenericMap')
 def test_get_solo_position(mock_map):
     mock_map.date = Time('2021-04-17T00:00')
     solo_pos = get_solo_position(mock_map)
 
     # equivalent to to meter i.e. a lenght and finite
     assert solo_pos.data.xyz.unit.is_equivalent('m')
```

### Comparing `stixpy-0.1.0rc2/stixpy.egg-info/PKG-INFO` & `stixpy-0.1.0rc3/stixpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: stixpy
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Analysis software for Solar Orbiter Spectromter Telescope for Imaging X-rays
 Home-page: 
 Author: STIX Team
 Author-email: shane.maloney@dias.ie
 License: BSD 3-Clause
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE.rst
 
 Analysis software for Solar Orbiter Spectrometer Telescope for Imaging X-rays
@@ -31,15 +31,15 @@
 Installation
 ------------
 
 It is strongly advised that you use and isolated environment through python's venv, virturalenv, anaconda or similar.
 
 .. code-block::
 
-    pip install git+https://github.com/samaloney/stixpy
+   pip install git+https://github.com/samaloney/stixpy
 
 
 License
 -------
 
 This project is Copyright (c) STIX Team and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
```

### Comparing `stixpy-0.1.0rc2/stixpy.egg-info/SOURCES.txt` & `stixpy-0.1.0rc3/stixpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,29 +9,14 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .circleci/config.yml
 .circleci/early_exit.sh
-calibration/__init__.py
-calibration/compression.py
-calibration/detector.py
-calibration/energy.py
-calibration/grid.py
-calibration/livetime.py
-calibration/transmission.py
-calibration/visibility.py
-calibration/tests/__init__.py
-calibration/tests/test_compression.py
-calibration/tests/test_detector.py
-calibration/tests/test_energy.py
-calibration/tests/test_grid.py
-calibration/tests/test_livetime.py
-calibration/tests/test_transmission.py
 changelog/README.rst
 docs/.DS_Store
 docs/Makefile
 docs/conf.py
 docs/dev_guide.rst
 docs/index.rst
 docs/make.bat
@@ -44,17 +29,18 @@
 docs/.idea/vcs.xml
 docs/.idea/workspace.xml
 docs/.idea/inspectionProfiles/Project_Default.xml
 docs/.idea/inspectionProfiles/profiles_settings.xml
 docs/code_ref/data.rst
 docs/code_ref/frames.rst
 docs/code_ref/index.rst
+docs/code_ref/product.rst
 docs/code_ref/science.rst
 docs/code_ref/timeseries.rst
-docs/code_ref/vis.rst
+docs/code_ref/visualisation.rst
 docs/whatsnew/changelog.rst
 docs/whatsnew/index.rst
 docs/whatsnew/latest_changelog.txt
 examples/imaging_demo.py
 licenses/README.rst
 licenses/TEMPLATE_LICENSE.rst
 stixpy/__init__.py
@@ -85,18 +71,32 @@
 stixpy/data/test.py
 stixpy/data/test_data.tar.gz
 stixpy/net/__init__.py
 stixpy/net/attrs.py
 stixpy/net/client.py
 stixpy/net/tests/__init__.py
 stixpy/net/tests/test_client.py
+stixpy/product/__init__.py
+stixpy/product/product.py
+stixpy/product/product_factory.py
+stixpy/product/sources/__init__.py
+stixpy/product/sources/housekeeping.py
+stixpy/product/sources/quicklook.py
+stixpy/product/sources/science.py
+stixpy/product/tests/__init__.py
+stixpy/product/tests/test_product_factory.py
 stixpy/tests/__init__.py
 stixpy/tests/test_frames.py
 stixpy/tests/test_science.py
 stixpy/timeseries/__init__.py
 stixpy/timeseries/quicklook.py
 stixpy/timeseries/tests/__init__.py
 stixpy/timeseries/tests/test_quicklook.py
-stixpy/vis/__init__.py
-stixpy/vis/map_reprojection.py
-stixpy/vis/tests/__init__.py
-stixpy/vis/tests/test_map_reprojection.py
+stixpy/utils/__init__.py
+stixpy/utils/logging.py
+stixpy/utils/time.py
+stixpy/utils/tests/__init__.py
+stixpy/utils/tests/test_time.py
+stixpy/visualisation/__init__.py
+stixpy/visualisation/map_reprojection.py
+stixpy/visualisation/tests/__init__.py
+stixpy/visualisation/tests/test_map_reprojection.py
```

### Comparing `stixpy-0.1.0rc2/tox.ini` & `stixpy-0.1.0rc3/tox.ini`

 * *Files identical despite different names*

