# Comparing `tmp/dtiplayground-0.5.7b8.tar.gz` & `tmp/dtiplayground-0.5.7b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtiplayground-0.5.7b8.tar", last modified: Thu Mar 16 21:43:55 2023, max compression
+gzip compressed data, was "dtiplayground-0.5.7b9.tar", last modified: Fri Mar 17 14:57:29 2023, max compression
```

## Comparing `dtiplayground-0.5.7b8.tar` & `dtiplayground-0.5.7b9.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.373942 dtiplayground-0.5.7b8/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1132 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/LICENSE
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      386 2023-03-16 21:43:55.374942 dtiplayground-0.5.7b8/PKG-INFO
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      326 2023-02-23 20:44:53.000000 dtiplayground-0.5.7b8/README.rst
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.323942 dtiplayground-0.5.7b8/bin/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      126 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriatlas
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6914 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriatlas.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      130 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriautotract
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    38839 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriautotract.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      133 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmrifiberprofile
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    38801 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmrifiberprofile.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      132 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriplayground
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6543 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriplayground.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      147 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriplaygroundlab
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      125 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b8/bin/dmriprep
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    11984 2023-02-20 16:41:31.000000 dtiplayground-0.5.7b8/bin/dmriprep.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.761942 dtiplayground-0.5.7b8/dtiplayground/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.809942 dtiplayground-0.5.7b8/dtiplayground/api/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    13478 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/application.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     6162 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/dmriatlasbuilder.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    15374 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/dmriprep.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2396 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/server.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.818942 dtiplayground-0.5.7b8/dtiplayground/api/static/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/static/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.839942 dtiplayground-0.5.7b8/dtiplayground/api/static/spa/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/static/spa/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)  7196793 2023-02-20 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/api/static/spa/spa.zip
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     4904 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/api/utils.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      321 2023-03-16 21:43:35.000000 dtiplayground-0.5.7b8/dtiplayground/config.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.924942 dtiplayground-0.5.7b8/dtiplayground/dmri/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      314 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:53.970942 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      249 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2065 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/app.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    71084 2023-03-01 23:23:58.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/atlasbuilder.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.002942 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1843 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    29281 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/template.json
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    24909 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/utils.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.052942 dtiplayground-0.5.7b8/dtiplayground/dmri/common/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     5542 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    24510 2023-03-07 16:56:56.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/appbase.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.094942 dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    77533 2023-02-28 22:49:17.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/fslinstaller.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    97554 2023-02-24 13:59:31.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/fslinstaller_py2.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1966 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/software_paths.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    29243 2023-03-16 19:58:11.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/dwi.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    20966 2023-03-16 21:35:34.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/module.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    23399 2023-03-16 21:41:10.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/pipeline.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.113942 dtiplayground-0.5.7b8/dtiplayground/dmri/common/study/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1444 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/study/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2018 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/study/loaders.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.278942 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      511 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2897 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/base.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1090 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/brainsfit.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      394 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/crop_dti.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     4132 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dti_reg.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      748 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dtiaverage.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      493 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dtiestim.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      793 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dtiprocess.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      428 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/fiberprocess.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     8801 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/fsl.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      435 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/greedy_atlas.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1141 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/image_math.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      221 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/itk_transform_tools.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2140 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/niral_utilities.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     3174 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      663 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/unu.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.293942 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.301942 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.330942 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      796 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      346 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      102 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/protocols.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.368942 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      792 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/module_template.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      338 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/module_template.yml
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2363 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.384942 dtiplayground-0.5.7b8/dtiplayground/dmri/playground/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/playground/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     3004 2023-02-28 23:00:41.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/playground/app.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.422942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2574 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      341 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    19294 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/app.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.439942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/data/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/data/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1966 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/data/software_paths.yml
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.454942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.492942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    12259 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2505 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1273 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.542942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6566 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1508 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      673 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.592942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    15310 2023-03-16 20:17:34.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     4381 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2491 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.625942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     7795 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2062 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1073 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.660942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     5846 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2343 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1248 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.690942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    12921 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1230 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      675 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.730942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1199 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      552 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      226 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.785942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     7854 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1778 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      929 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.868942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    15789 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1637 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      954 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.919942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1939 2023-02-20 16:02:35.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      417 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      349 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:54.968942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    17149 2023-02-24 14:58:17.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      481 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      343 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.016942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1227 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     9061 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1943 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.063942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      618 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    20321 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      955 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.093942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      997 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.136942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      235 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/README.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1745 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      356 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.yml
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)       88 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/__init__.py
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/protocols.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.180942 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      101 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/module_template.md
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      818 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/module_template.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      330 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/module_template.yml
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     5435 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/protocol_template.yml
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.200942 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/__init__.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.212942 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/modules/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      102 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/modules/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/protocols.py
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.254942 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/__init__.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      792 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/module_template.py
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      338 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/module_template.yml
--rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2666 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/protocol_template.yml
-drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-16 21:43:55.369942 dtiplayground-0.5.7b8/dtiplayground.egg-info/
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      386 2023-03-16 21:43:51.000000 dtiplayground-0.5.7b8/dtiplayground.egg-info/PKG-INFO
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     8462 2023-03-16 21:43:53.000000 dtiplayground-0.5.7b8/dtiplayground.egg-info/SOURCES.txt
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        1 2023-03-16 21:43:51.000000 dtiplayground-0.5.7b8/dtiplayground.egg-info/dependency_links.txt
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      205 2023-03-16 21:43:51.000000 dtiplayground-0.5.7b8/dtiplayground.egg-info/requires.txt
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)       14 2023-03-16 21:43:51.000000 dtiplayground-0.5.7b8/dtiplayground.egg-info/top_level.txt
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      103 2023-03-16 21:43:55.377942 dtiplayground-0.5.7b8/setup.cfg
--rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1525 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b8/setup.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:30.041388 dtiplayground-0.5.7b9/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1132 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/LICENSE
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      386 2023-03-17 14:57:30.042388 dtiplayground-0.5.7b9/PKG-INFO
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      326 2023-02-23 20:44:53.000000 dtiplayground-0.5.7b9/README.rst
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:30.015388 dtiplayground-0.5.7b9/bin/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      126 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriatlas
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6914 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriatlas.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      130 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriautotract
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    38839 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriautotract.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      133 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmrifiberprofile
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    38801 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmrifiberprofile.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      132 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriplayground
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6543 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriplayground.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      147 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriplaygroundlab
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      125 2023-02-15 16:59:26.000000 dtiplayground-0.5.7b9/bin/dmriprep
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    11984 2023-02-20 16:41:31.000000 dtiplayground-0.5.7b9/bin/dmriprep.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.695388 dtiplayground-0.5.7b9/dtiplayground/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.728388 dtiplayground-0.5.7b9/dtiplayground/api/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    13478 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/application.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     6162 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/dmriatlasbuilder.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    15374 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/dmriprep.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2396 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/server.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.736388 dtiplayground-0.5.7b9/dtiplayground/api/static/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/static/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.753388 dtiplayground-0.5.7b9/dtiplayground/api/static/spa/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/static/spa/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)  7196793 2023-02-20 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/api/static/spa/spa.zip
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     4904 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/api/utils.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      321 2023-03-17 14:57:21.000000 dtiplayground-0.5.7b9/dtiplayground/config.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.841388 dtiplayground-0.5.7b9/dtiplayground/dmri/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      314 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.878388 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      249 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2065 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/app.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    71084 2023-03-01 23:23:58.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/atlasbuilder.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.906388 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1843 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    29281 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/template.json
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    24909 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/utils.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.952388 dtiplayground-0.5.7b9/dtiplayground/dmri/common/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     5542 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    24510 2023-03-07 16:56:56.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/appbase.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:28.992388 dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    77533 2023-02-28 22:49:17.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/fslinstaller.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    97554 2023-02-24 13:59:31.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/fslinstaller_py2.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1966 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/software_paths.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    29243 2023-03-16 19:58:11.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/dwi.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    20966 2023-03-16 21:35:34.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/module.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    23399 2023-03-16 21:41:10.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/pipeline.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.009388 dtiplayground-0.5.7b9/dtiplayground/dmri/common/study/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1444 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/study/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2018 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/study/loaders.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.153388 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      511 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2897 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/base.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1090 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/brainsfit.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      394 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/crop_dti.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     4132 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dti_reg.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      748 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dtiaverage.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      493 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dtiestim.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      793 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dtiprocess.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      428 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/fiberprocess.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     8801 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/fsl.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      435 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/greedy_atlas.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1141 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/image_math.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      221 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/itk_transform_tools.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2140 2023-02-15 16:59:27.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/niral_utilities.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     3174 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      663 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/unu.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.169388 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.178388 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.209388 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      796 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      346 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      102 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/protocols.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.245388 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      792 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/module_template.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      338 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/module_template.yml
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2363 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.261388 dtiplayground-0.5.7b9/dtiplayground/dmri/playground/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/playground/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     3004 2023-02-28 23:00:41.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/playground/app.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.296388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2574 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      341 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    19294 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/app.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.313388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/data/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/data/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1966 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/data/software_paths.yml
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.322388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.362388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    12259 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2505 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1273 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.400388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     6566 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1508 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      673 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.437388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    15310 2023-03-16 20:17:34.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     4381 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2491 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.464388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     7795 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2062 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1073 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.491388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     5846 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     2343 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1248 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.524388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    12921 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1230 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      675 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:28.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.556388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1199 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      552 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      226 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.596388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     7854 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1778 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      929 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.635388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    15789 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1637 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      954 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.673388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1939 2023-02-20 16:02:35.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      417 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      349 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.712388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)    17149 2023-02-24 14:58:17.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      481 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      343 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.752388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1227 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     9061 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     1943 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.792388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      618 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)    20321 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      955 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.812388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      997 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.851388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      235 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/README.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1745 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      356 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.yml
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)       88 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/__init__.py
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/protocols.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.893388 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      101 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/module_template.md
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      818 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/module_template.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      330 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/module_template.yml
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     5435 2023-02-15 16:59:29.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/protocol_template.yml
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.911388 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/__init__.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.920388 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/modules/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      102 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/modules/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      655 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/protocols.py
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:29.955388 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        0 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/__init__.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      792 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/module_template.py
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      338 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/module_template.yml
+-rwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)     2666 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/protocol_template.yml
+drwxrwxr-x   0 scalphunter  (1000) scalphunter  (1000)        0 2023-03-17 14:57:30.038388 dtiplayground-0.5.7b9/dtiplayground.egg-info/
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      386 2023-03-17 14:57:27.000000 dtiplayground-0.5.7b9/dtiplayground.egg-info/PKG-INFO
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     8462 2023-03-17 14:57:28.000000 dtiplayground-0.5.7b9/dtiplayground.egg-info/SOURCES.txt
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)        1 2023-03-17 14:57:27.000000 dtiplayground-0.5.7b9/dtiplayground.egg-info/dependency_links.txt
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      205 2023-03-17 14:57:27.000000 dtiplayground-0.5.7b9/dtiplayground.egg-info/requires.txt
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)       14 2023-03-17 14:57:27.000000 dtiplayground-0.5.7b9/dtiplayground.egg-info/top_level.txt
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)      103 2023-03-17 14:57:30.044388 dtiplayground-0.5.7b9/setup.cfg
+-rw-rw-r--   0 scalphunter  (1000) scalphunter  (1000)     1525 2023-02-15 16:59:30.000000 dtiplayground-0.5.7b9/setup.py
```

### Comparing `dtiplayground-0.5.7b8/LICENSE` & `dtiplayground-0.5.7b9/LICENSE`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/bin/dmriatlas.py` & `dtiplayground-0.5.7b9/bin/dmriatlas.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/bin/dmriautotract.py` & `dtiplayground-0.5.7b9/bin/dmriautotract.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/bin/dmrifiberprofile.py` & `dtiplayground-0.5.7b9/bin/dmrifiberprofile.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/bin/dmriplayground.py` & `dtiplayground-0.5.7b9/bin/dmriplayground.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/bin/dmriprep.py` & `dtiplayground-0.5.7b9/bin/dmriprep.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/application.py` & `dtiplayground-0.5.7b9/dtiplayground/api/application.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/dmriatlasbuilder.py` & `dtiplayground-0.5.7b9/dtiplayground/api/dmriatlasbuilder.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/dmriprep.py` & `dtiplayground-0.5.7b9/dtiplayground/api/dmriprep.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/server.py` & `dtiplayground-0.5.7b9/dtiplayground/api/server.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/static/spa/spa.zip` & `dtiplayground-0.5.7b9/dtiplayground/api/static/spa/spa.zip`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/api/utils.py` & `dtiplayground-0.5.7b9/dtiplayground/api/utils.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/app.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/atlasbuilder.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/atlasbuilder.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/data/template.json` & `dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/data/template.json`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/atlasbuilder/utils.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/atlasbuilder/utils.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/__init__.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/appbase.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/appbase.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/fslinstaller.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/fslinstaller.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/fslinstaller_py2.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/fslinstaller_py2.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/data/software_paths.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/data/software_paths.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/dwi.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/dwi.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/module.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/module.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/pipeline.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/study/__init__.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/study/__init__.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/study/loaders.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/study/loaders.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/base.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/base.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/brainsfit.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/brainsfit.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dti_reg.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dti_reg.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dtiaverage.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dtiaverage.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/dtiprocess.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/dtiprocess.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/fsl.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/fsl.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/image_math.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/image_math.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/niral_utilities.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/niral_utilities.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/common/tools/unu.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/common/tools/unu.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/protocols.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/protocols.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/module_template.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/playground/app.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/playground/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/app.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/data/software_paths.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/data/software_paths.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/protocols.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/module_template.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/preprocessing/templates/protocol_template.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/preprocessing/templates/protocol_template.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/protocols.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/protocols.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/module_template.py` & `dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground/dmri/tractography/templates/protocol_template.yml` & `dtiplayground-0.5.7b9/dtiplayground/dmri/tractography/templates/protocol_template.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/dtiplayground.egg-info/SOURCES.txt` & `dtiplayground-0.5.7b9/dtiplayground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.7b8/setup.py` & `dtiplayground-0.5.7b9/setup.py`

 * *Files identical despite different names*

