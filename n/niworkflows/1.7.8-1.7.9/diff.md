# Comparing `tmp/niworkflows-1.7.8.tar.gz` & `tmp/niworkflows-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niworkflows-1.7.8.tar", last modified: Fri Mar 24 19:09:12 2023, max compression
+gzip compressed data, was "niworkflows-1.7.9.tar", last modified: Tue Apr 11 15:49:45 2023, max compression
```

## Comparing `niworkflows-1.7.8.tar` & `niworkflows-1.7.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-03-24 19:09:06.000000 niworkflows-1.7.8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-03-24 19:09:06.000000 niworkflows-1.7.8/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-03-24 19:09:12.584775 niworkflows-1.7.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-03-24 19:09:06.000000 niworkflows-1.7.8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1528 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/__about__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.572775 niworkflows-1.7.8/niworkflows/anat/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/anat/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42038 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/anat/ants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12558 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/anat/coregistration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5595 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/anat/freesurfer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/anat/skullstrip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.572775 niworkflows-1.7.8/niworkflows/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2948 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/cli/boldref.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.576775 niworkflows-1.7.8/niworkflows/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/antsBrainExtractionNoLaplacian_precise.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/antsBrainExtractionNoLaplacian_testing.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/antsBrainExtraction_precise.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/antsBrainExtraction_testing.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_000.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_001.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_002.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_000.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_001.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_002.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/epi_atlasbased_brainmask.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      149 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/itkIdentityTransform.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10671 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/nipreps.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/sentinel.nii.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)      968 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_fast_000.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_000.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_001.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_002.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      860 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_000.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      822 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_001.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      822 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_002.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.576775 niworkflows-1.7.8/niworkflows/dwi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/dwi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.576775 niworkflows-1.7.8/niworkflows/engine/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/engine/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/engine/workflows.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.576775 niworkflows-1.7.8/niworkflows/func/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/func/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22144 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/func/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.580775 niworkflows-1.7.8/niworkflows/interfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38823 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/bids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3411 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/bold.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13457 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/cifti.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24651 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/confounds.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6377 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/fixes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19002 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/freesurfer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18710 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/header.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26354 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/images.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11492 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/itk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3746 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/morphology.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27161 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/nibabel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9577 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/nilearn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3621 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/nitransforms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23903 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/norm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2259 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/patches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8347 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/plotting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7418 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/probmaps.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.580775 niworkflows-1.7.8/niworkflows/interfaces/reportlets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/reportlets/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6601 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/reportlets/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9581 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/reportlets/masks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13837 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/reportlets/registration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7910 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/reportlets/segmentation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2645 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/space.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23640 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/surf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17899 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/interfaces/utility.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.580775 niworkflows-1.7.8/niworkflows/reports/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/reports/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/reports/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10783 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/reports/default.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5875 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/reports/report.tpl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2023-03-24 19:09:06.000000 niworkflows-1.7.8/niworkflows/testing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16857 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/bids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2136 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/connections.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/images.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10496 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/misc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25729 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/spaces.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3372 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/testing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3232 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/utils/timeseries.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/viz/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/viz/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/viz/notebook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36068 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/viz/plots.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24798 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/viz/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/workflows/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/workflows/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.584775 niworkflows-1.7.8/niworkflows/workflows/epi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/workflows/epi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9704 2023-03-24 19:09:07.000000 niworkflows-1.7.8/niworkflows/workflows/epi/refmap.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-24 19:09:12.572775 niworkflows-1.7.8/niworkflows.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3412 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-24 19:09:12.000000 niworkflows-1.7.8/niworkflows.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-03-24 19:09:07.000000 niworkflows-1.7.8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2884 2023-03-24 19:09:12.584775 niworkflows-1.7.8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1164 2023-03-24 19:09:07.000000 niworkflows-1.7.8/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    81674 2023-03-24 19:09:07.000000 niworkflows-1.7.8/versioneer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2023-04-11 15:49:39.000000 niworkflows-1.7.9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-04-11 15:49:39.000000 niworkflows-1.7.9/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-04-11 15:49:45.387407 niworkflows-1.7.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-04-11 15:49:39.000000 niworkflows-1.7.9/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.391407 niworkflows-1.7.9/niworkflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1528 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/__about__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2023-04-11 15:49:45.391407 niworkflows-1.7.9/niworkflows/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.379407 niworkflows-1.7.9/niworkflows/anat/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/anat/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42038 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/anat/ants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12558 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/anat/coregistration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5595 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/anat/freesurfer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4889 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/anat/skullstrip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.379407 niworkflows-1.7.9/niworkflows/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2948 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/cli/boldref.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.383407 niworkflows-1.7.9/niworkflows/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/antsBrainExtractionNoLaplacian_precise.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/antsBrainExtractionNoLaplacian_testing.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/antsBrainExtraction_precise.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/antsBrainExtraction_testing.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_000.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_001.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_002.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_000.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_001.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_002.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      566 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/epi_atlasbased_brainmask.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      149 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/itkIdentityTransform.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10671 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/nipreps.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/sentinel.nii.gz
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      968 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_fast_000.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_000.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_001.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_002.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      860 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_000.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      822 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_001.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      822 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_002.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.383407 niworkflows-1.7.9/niworkflows/dwi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/dwi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.383407 niworkflows-1.7.9/niworkflows/engine/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/engine/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/engine/workflows.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.383407 niworkflows-1.7.9/niworkflows/func/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/func/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22144 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/func/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.383407 niworkflows-1.7.9/niworkflows/interfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38823 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/bids.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3411 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/bold.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13457 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/cifti.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24651 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/confounds.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6377 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/fixes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19002 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/freesurfer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18710 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/header.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26354 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/images.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11492 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/itk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3746 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/morphology.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27161 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/nibabel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9577 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/nilearn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3621 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/nitransforms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23903 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/norm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2259 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/patches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8347 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/plotting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7418 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/probmaps.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/interfaces/reportlets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/reportlets/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6601 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/reportlets/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9581 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/reportlets/masks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13837 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/reportlets/registration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7910 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/reportlets/segmentation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2645 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/space.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23640 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/surf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17899 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/interfaces/utility.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/reports/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/reports/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/reports/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10783 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/reports/default.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5875 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/reports/report.tpl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/testing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16857 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/bids.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2136 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/connections.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11316 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/images.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10496 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25729 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/spaces.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3372 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3232 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/utils/timeseries.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/viz/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/viz/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/viz/notebook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36054 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/viz/plots.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24798 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/viz/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/workflows/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/workflows/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.387407 niworkflows-1.7.9/niworkflows/workflows/epi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/workflows/epi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9704 2023-04-11 15:49:39.000000 niworkflows-1.7.9/niworkflows/workflows/epi/refmap.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-11 15:49:45.379407 niworkflows-1.7.9/niworkflows.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3412 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-11 15:49:45.000000 niworkflows-1.7.9/niworkflows.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2023-04-11 15:49:39.000000 niworkflows-1.7.9/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2884 2023-04-11 15:49:45.387407 niworkflows-1.7.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1164 2023-04-11 15:49:39.000000 niworkflows-1.7.9/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    81674 2023-04-11 15:49:39.000000 niworkflows-1.7.9/versioneer.py
```

### Comparing `niworkflows-1.7.8/LICENSE` & `niworkflows-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/PKG-INFO` & `niworkflows-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niworkflows
-Version: 1.7.8
+Version: 1.7.9
 Summary: NeuroImaging Workflows provides processing tools for magnetic resonance images of the brain.
 Home-page: https://www.nipreps.org
 Author: The NiPreps Developers
 Author-email: nipreps@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://www.nipreps.org/niworkflows
 Project-URL: GitHub, https://github.com/nipreps/niworkflows
```

### Comparing `niworkflows-1.7.8/README.rst` & `niworkflows-1.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/__about__.py` & `niworkflows-1.7.9/niworkflows/__about__.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/__init__.py` & `niworkflows-1.7.9/niworkflows/__init__.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/anat/ants.py` & `niworkflows-1.7.9/niworkflows/anat/ants.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/anat/coregistration.py` & `niworkflows-1.7.9/niworkflows/anat/coregistration.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/anat/freesurfer.py` & `niworkflows-1.7.9/niworkflows/anat/freesurfer.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/anat/skullstrip.py` & `niworkflows-1.7.9/niworkflows/anat/skullstrip.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/cli/boldref.py` & `niworkflows-1.7.9/niworkflows/cli/boldref.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/antsBrainExtractionNoLaplacian_precise.json` & `niworkflows-1.7.9/niworkflows/data/antsBrainExtractionNoLaplacian_precise.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/antsBrainExtractionNoLaplacian_testing.json` & `niworkflows-1.7.9/niworkflows/data/antsBrainExtractionNoLaplacian_testing.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/antsBrainExtraction_precise.json` & `niworkflows-1.7.9/niworkflows/data/antsBrainExtraction_precise.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/antsBrainExtraction_testing.json` & `niworkflows-1.7.9/niworkflows/data/antsBrainExtraction_testing.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_000.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_000.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_001.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_001.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_precise_002.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_precise_002.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_000.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_000.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_001.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_001.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/boldref-mni_registration_testing_002.json` & `niworkflows-1.7.9/niworkflows/data/boldref-mni_registration_testing_002.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/epi_atlasbased_brainmask.json` & `niworkflows-1.7.9/niworkflows/data/epi_atlasbased_brainmask.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/nipreps.json` & `niworkflows-1.7.9/niworkflows/data/nipreps.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_fast_000.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_fast_000.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_000.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_000.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_001.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_001.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_precise_002.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_precise_002.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_000.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_000.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_001.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_001.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/data/t1w-mni_registration_testing_002.json` & `niworkflows-1.7.9/niworkflows/data/t1w-mni_registration_testing_002.json`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/engine/workflows.py` & `niworkflows-1.7.9/niworkflows/engine/workflows.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/func/util.py` & `niworkflows-1.7.9/niworkflows/func/util.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/bids.py` & `niworkflows-1.7.9/niworkflows/interfaces/bids.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/bold.py` & `niworkflows-1.7.9/niworkflows/interfaces/bold.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/cifti.py` & `niworkflows-1.7.9/niworkflows/interfaces/cifti.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/confounds.py` & `niworkflows-1.7.9/niworkflows/interfaces/confounds.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/fixes.py` & `niworkflows-1.7.9/niworkflows/interfaces/fixes.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/freesurfer.py` & `niworkflows-1.7.9/niworkflows/interfaces/freesurfer.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/header.py` & `niworkflows-1.7.9/niworkflows/interfaces/header.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/images.py` & `niworkflows-1.7.9/niworkflows/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/itk.py` & `niworkflows-1.7.9/niworkflows/interfaces/itk.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/morphology.py` & `niworkflows-1.7.9/niworkflows/interfaces/morphology.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/nibabel.py` & `niworkflows-1.7.9/niworkflows/interfaces/nibabel.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/nilearn.py` & `niworkflows-1.7.9/niworkflows/interfaces/nilearn.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/nitransforms.py` & `niworkflows-1.7.9/niworkflows/interfaces/nitransforms.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/norm.py` & `niworkflows-1.7.9/niworkflows/interfaces/norm.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/patches.py` & `niworkflows-1.7.9/niworkflows/interfaces/patches.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/plotting.py` & `niworkflows-1.7.9/niworkflows/interfaces/plotting.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/probmaps.py` & `niworkflows-1.7.9/niworkflows/interfaces/probmaps.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/reportlets/base.py` & `niworkflows-1.7.9/niworkflows/interfaces/reportlets/base.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/reportlets/masks.py` & `niworkflows-1.7.9/niworkflows/interfaces/reportlets/masks.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/reportlets/registration.py` & `niworkflows-1.7.9/niworkflows/interfaces/reportlets/registration.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/reportlets/segmentation.py` & `niworkflows-1.7.9/niworkflows/interfaces/reportlets/segmentation.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/space.py` & `niworkflows-1.7.9/niworkflows/interfaces/space.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/surf.py` & `niworkflows-1.7.9/niworkflows/interfaces/surf.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/interfaces/utility.py` & `niworkflows-1.7.9/niworkflows/interfaces/utility.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/reports/core.py` & `niworkflows-1.7.9/niworkflows/reports/core.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/reports/default.yml` & `niworkflows-1.7.9/niworkflows/reports/default.yml`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/reports/report.tpl` & `niworkflows-1.7.9/niworkflows/reports/report.tpl`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/testing.py` & `niworkflows-1.7.9/niworkflows/testing.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/bids.py` & `niworkflows-1.7.9/niworkflows/utils/bids.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/connections.py` & `niworkflows-1.7.9/niworkflows/utils/connections.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/images.py` & `niworkflows-1.7.9/niworkflows/utils/images.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/misc.py` & `niworkflows-1.7.9/niworkflows/utils/misc.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/spaces.py` & `niworkflows-1.7.9/niworkflows/utils/spaces.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/testing.py` & `niworkflows-1.7.9/niworkflows/utils/testing.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/utils/timeseries.py` & `niworkflows-1.7.9/niworkflows/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/viz/notebook.py` & `niworkflows-1.7.9/niworkflows/viz/notebook.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/viz/plots.py` & `niworkflows-1.7.9/niworkflows/viz/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,16 +192,15 @@
 
     """
     if segments is None:
         segments = {
             "whole brain (voxels)": list(range(data.shape[0]))
         }
 
-    nsegments = len(segments)
-    if nsegments == 1:
+    if len(segments) == 1:
         legend = False
 
     if cmap is None:
         colors = cm.get_cmap("tab10").colors
     elif cmap == "paired":
         colors = list(cm.get_cmap("Paired").colors)
         colors[0], colors[1] = colors[1], colors[0]
@@ -252,15 +251,15 @@
 
     # Calculate time decimation factor
     t_dec = max(int((1.8 * n_trs) // size[1]), 1)
     data = data[:, drop_trs::t_dec]
 
     # Define nested GridSpec
     gs = mgs.GridSpecFromSubplotSpec(
-        nsegments,
+        len(segments),
         1,
         subplot_spec=subplot,
         hspace=0.05,
         height_ratios=[len(v) for v in segments.values()]
     )
 
     for i, (label, indices) in enumerate(segments.items()):
@@ -290,15 +289,15 @@
 
         # Make all subplots have same xticks
         xticks = np.linspace(0, data.shape[-1], endpoint=True, num=7)
         ax.set_xticks(xticks)
         ax.set_yticks([])
         ax.grid(False)
 
-        if i == (nsegments - 1):
+        if i == (len(segments) - 1):
             xlabel = "time-points (index)"
             xticklabels = (xticks * n_trs / data.shape[-1]).astype("uint32") + drop_trs
             if tr is not None:
                 xlabel = "time (mm:ss)"
                 xticklabels = [
                     f"{int(t // 60):02d}:{(t % 60).round(0).astype(int):02d}"
                     for t in (tr * xticklabels)
@@ -314,15 +313,15 @@
             ax.set_xticks([])
             ax.spines["bottom"].set_color("none")
             ax.spines["bottom"].set_visible(False)
 
         if title and i == 0:
             ax.set_title(title)
 
-    if nsegments == 1:
+    if len(segments) == 1:
         ax.set_ylabel(label)
 
     if legend:
         from matplotlib.patches import Patch
         from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 
         axlegend = inset_axes(
```

### Comparing `niworkflows-1.7.8/niworkflows/viz/utils.py` & `niworkflows-1.7.9/niworkflows/viz/utils.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows/workflows/epi/refmap.py` & `niworkflows-1.7.9/niworkflows/workflows/epi/refmap.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows.egg-info/PKG-INFO` & `niworkflows-1.7.9/niworkflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niworkflows
-Version: 1.7.8
+Version: 1.7.9
 Summary: NeuroImaging Workflows provides processing tools for magnetic resonance images of the brain.
 Home-page: https://www.nipreps.org
 Author: The NiPreps Developers
 Author-email: nipreps@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://www.nipreps.org/niworkflows
 Project-URL: GitHub, https://github.com/nipreps/niworkflows
```

### Comparing `niworkflows-1.7.8/niworkflows.egg-info/SOURCES.txt` & `niworkflows-1.7.9/niworkflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/niworkflows.egg-info/requires.txt` & `niworkflows-1.7.9/niworkflows.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/setup.cfg` & `niworkflows-1.7.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/setup.py` & `niworkflows-1.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `niworkflows-1.7.8/versioneer.py` & `niworkflows-1.7.9/versioneer.py`

 * *Files identical despite different names*

