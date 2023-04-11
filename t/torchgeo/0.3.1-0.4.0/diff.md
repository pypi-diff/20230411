# Comparing `tmp/torchgeo-0.3.1.tar.gz` & `tmp/torchgeo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgeo-0.3.1.tar", last modified: Thu Sep  8 21:32:55 2022, max compression
+gzip compressed data, was "torchgeo-0.4.0.tar", last modified: Tue Jan 24 23:51:50 2023, max compression
```

## Comparing `torchgeo-0.3.1.tar` & `torchgeo-0.4.0.tar`

### file list

```diff
@@ -1,124 +1,131 @@
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.912037 torchgeo-0.3.1/
--rw-r-----   0 ajstewart   (501) staff       (20)     1141 2022-05-18 20:55:50.000000 torchgeo-0.3.1/LICENSE
--rw-r-----   0 ajstewart   (501) staff       (20)    12490 2022-09-08 21:32:55.912413 torchgeo-0.3.1/PKG-INFO
--rw-r-----   0 ajstewart   (501) staff       (20)    11384 2022-09-06 02:56:56.000000 torchgeo-0.3.1/README.md
--rw-r-----   0 ajstewart   (501) staff       (20)     4687 2022-09-08 04:29:39.000000 torchgeo-0.3.1/pyproject.toml
--rw-r-----   0 ajstewart   (501) staff       (20)     2338 2022-09-08 21:32:55.915476 torchgeo-0.3.1/setup.cfg
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.581886 torchgeo-0.3.1/torchgeo/
--rw-r-----   0 ajstewart   (501) staff       (20)      501 2022-09-08 17:42:10.000000 torchgeo-0.3.1/torchgeo/__init__.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.671484 torchgeo-0.3.1/torchgeo/datamodules/
--rw-r-----   0 ajstewart   (501) staff       (20)     1867 2022-08-02 21:23:52.000000 torchgeo-0.3.1/torchgeo/datamodules/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5673 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/bigearthnet.py
--rw-r-----   0 ajstewart   (501) staff       (20)    11843 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/chesapeake.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4241 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/cowc.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5625 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/cyclone.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3636 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/deepglobelandcover.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4582 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/etci2021.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4288 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/eurosat.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3953 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/fair1m.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8814 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/inria.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5343 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/landcoverai.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3739 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/loveda.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5774 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/naip.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4209 2022-09-06 20:37:59.000000 torchgeo-0.3.1/torchgeo/datamodules/nasa_marine_debris.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7038 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/oscd.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3511 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/potsdam.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5132 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/resisc45.py
--rw-r-----   0 ajstewart   (501) staff       (20)     6573 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/sen12ms.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5873 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/so2sat.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3797 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/ucmerced.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3164 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/usavars.py
--rw-r-----   0 ajstewart   (501) staff       (20)     1344 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/utils.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3525 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/vaihingen.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3493 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datamodules/xview.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.839037 torchgeo-0.3.1/torchgeo/datasets/
--rw-r-----   0 ajstewart   (501) staff       (20)     4784 2022-09-08 17:42:10.000000 torchgeo-0.3.1/torchgeo/datasets/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8102 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/advance.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5350 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/agb_live_woody_density.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4282 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/astergdem.py
--rw-r-----   0 ajstewart   (501) staff       (20)    15179 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/benin_cashews.py
--rw-r-----   0 ajstewart   (501) staff       (20)    18765 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/bigearthnet.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5769 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cbf.py
--rw-r-----   0 ajstewart   (501) staff       (20)    14954 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cdl.py
--rw-r-----   0 ajstewart   (501) staff       (20)    25136 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/chesapeake.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8457 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cms_mangrove_canopy.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9469 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cowc.py
--rw-r-----   0 ajstewart   (501) staff       (20)    15047 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cv4a_kenya_crop_type.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8533 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/cyclone.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8411 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/deepglobelandcover.py
--rw-r-----   0 ajstewart   (501) staff       (20)    11679 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/dfc2022.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3738 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/eddmaps.py
--rw-r-----   0 ajstewart   (501) staff       (20)    17649 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/enviroatlas.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5877 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/esri2020.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10567 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/etci2021.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7233 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/eudem.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9713 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/eurosat.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10709 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/fair1m.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10182 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/forestdamage.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4583 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/gbif.py
--rw-r-----   0 ajstewart   (501) staff       (20)    33446 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datasets/geo.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8398 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/gid15.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10942 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/globbiomass.py
--rw-r-----   0 ajstewart   (501) staff       (20)    20609 2022-09-08 03:53:15.000000 torchgeo-0.3.1/torchgeo/datasets/idtrees.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3862 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/inaturalist.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7363 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/inria.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8671 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/landcoverai.py
--rw-r-----   0 ajstewart   (501) staff       (20)     6336 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/landsat.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7906 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/levircd.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9071 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/loveda.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10422 2022-07-10 02:06:20.000000 torchgeo-0.3.1/torchgeo/datasets/millionaid.py
--rw-r-----   0 ajstewart   (501) staff       (20)     2751 2022-07-10 17:36:27.000000 torchgeo-0.3.1/torchgeo/datasets/naip.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8373 2022-09-06 20:37:59.000000 torchgeo-0.3.1/torchgeo/datasets/nasa_marine_debris.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7901 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/nwpu.py
--rw-r-----   0 ajstewart   (501) staff       (20)    20480 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datasets/openbuildings.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10309 2022-08-19 00:44:11.000000 torchgeo-0.3.1/torchgeo/datasets/oscd.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5454 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/patternnet.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8761 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/potsdam.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8734 2022-07-10 02:06:20.000000 torchgeo-0.3.1/torchgeo/datasets/reforestree.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8239 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/resisc45.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9676 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/seco.py
--rw-r-----   0 ajstewart   (501) staff       (20)    11506 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/sen12ms.py
--rw-r-----   0 ajstewart   (501) staff       (20)     4912 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datasets/sentinel.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10141 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datasets/so2sat.py
--rw-r-----   0 ajstewart   (501) staff       (20)    42088 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/datasets/spacenet.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7663 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/ucmerced.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9385 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/usavars.py
--rw-r-----   0 ajstewart   (501) staff       (20)    21269 2022-07-10 02:06:20.000000 torchgeo-0.3.1/torchgeo/datasets/utils.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9190 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/vaihingen.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9152 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/xview.py
--rw-r-----   0 ajstewart   (501) staff       (20)    10230 2022-07-11 05:35:04.000000 torchgeo-0.3.1/torchgeo/datasets/zuericrop.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.844738 torchgeo-0.3.1/torchgeo/losses/
--rw-r-----   0 ajstewart   (501) staff       (20)      306 2022-06-29 19:23:59.000000 torchgeo-0.3.1/torchgeo/losses/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)     2164 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/losses/qr.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.863764 torchgeo-0.3.1/torchgeo/models/
--rw-r-----   0 ajstewart   (501) staff       (20)      614 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/models/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)     7876 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/models/changestar.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8680 2022-09-06 16:29:09.000000 torchgeo-0.3.1/torchgeo/models/farseg.py
--rw-r-----   0 ajstewart   (501) staff       (20)     2123 2022-06-29 19:23:59.000000 torchgeo-0.3.1/torchgeo/models/fcn.py
--rw-r-----   0 ajstewart   (501) staff       (20)     8295 2022-09-03 19:25:08.000000 torchgeo-0.3.1/torchgeo/models/fcsiam.py
--rw-r-----   0 ajstewart   (501) staff       (20)     3410 2022-08-22 06:00:06.000000 torchgeo-0.3.1/torchgeo/models/rcf.py
--rw-r-----   0 ajstewart   (501) staff       (20)     2776 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/models/resnet.py
--rw-r-----   0 ajstewart   (501) staff       (20)        0 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/py.typed
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.879082 torchgeo-0.3.1/torchgeo/samplers/
--rw-r-----   0 ajstewart   (501) staff       (20)      664 2022-09-03 18:18:11.000000 torchgeo-0.3.1/torchgeo/samplers/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5311 2022-09-03 18:18:11.000000 torchgeo-0.3.1/torchgeo/samplers/batch.py
--rw-r-----   0 ajstewart   (501) staff       (20)      477 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/samplers/constants.py
--rw-r-----   0 ajstewart   (501) staff       (20)    12397 2022-09-06 02:56:56.000000 torchgeo-0.3.1/torchgeo/samplers/single.py
--rw-r-----   0 ajstewart   (501) staff       (20)     1854 2022-09-03 18:18:11.000000 torchgeo-0.3.1/torchgeo/samplers/utils.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.895747 torchgeo-0.3.1/torchgeo/trainers/
--rw-r-----   0 ajstewart   (501) staff       (20)      588 2022-09-06 20:37:59.000000 torchgeo-0.3.1/torchgeo/trainers/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)    15522 2022-09-06 16:29:09.000000 torchgeo-0.3.1/torchgeo/trainers/byol.py
--rw-r-----   0 ajstewart   (501) staff       (20)    13542 2022-09-03 19:29:12.000000 torchgeo-0.3.1/torchgeo/trainers/classification.py
--rw-r-----   0 ajstewart   (501) staff       (20)     6515 2022-09-08 17:42:10.000000 torchgeo-0.3.1/torchgeo/trainers/regression.py
--rw-r-----   0 ajstewart   (501) staff       (20)     9254 2022-09-03 19:29:12.000000 torchgeo-0.3.1/torchgeo/trainers/segmentation.py
--rw-r-----   0 ajstewart   (501) staff       (20)     5470 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/trainers/utils.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.911015 torchgeo-0.3.1/torchgeo/transforms/
--rw-r-----   0 ajstewart   (501) staff       (20)      954 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/transforms/__init__.py
--rw-r-----   0 ajstewart   (501) staff       (20)    13479 2022-09-08 17:42:10.000000 torchgeo-0.3.1/torchgeo/transforms/indices.py
--rw-r-----   0 ajstewart   (501) staff       (20)     2419 2022-07-09 23:31:15.000000 torchgeo-0.3.1/torchgeo/transforms/transforms.py
-drwxr-x---   0 ajstewart   (501) staff       (20)        0 2022-09-08 21:32:55.584364 torchgeo-0.3.1/torchgeo.egg-info/
--rw-r-----   0 ajstewart   (501) staff       (20)    12490 2022-09-08 21:32:55.000000 torchgeo-0.3.1/torchgeo.egg-info/PKG-INFO
--rw-r-----   0 ajstewart   (501) staff       (20)     3363 2022-09-08 21:32:55.000000 torchgeo-0.3.1/torchgeo.egg-info/SOURCES.txt
--rw-r-----   0 ajstewart   (501) staff       (20)        1 2022-09-08 21:32:55.000000 torchgeo-0.3.1/torchgeo.egg-info/dependency_links.txt
--rw-r-----   0 ajstewart   (501) staff       (20)      882 2022-09-08 21:32:55.000000 torchgeo-0.3.1/torchgeo.egg-info/requires.txt
--rw-r-----   0 ajstewart   (501) staff       (20)        9 2022-09-08 21:32:55.000000 torchgeo-0.3.1/torchgeo.egg-info/top_level.txt
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.179207 torchgeo-0.4.0/
+-rw-r-----   0 Adam       (501) staff       (20)     1141 2022-03-19 20:19:53.000000 torchgeo-0.4.0/LICENSE
+-rw-r-----   0 Adam       (501) staff       (20)    12770 2023-01-24 23:51:50.179475 torchgeo-0.4.0/PKG-INFO
+-rw-r-----   0 Adam       (501) staff       (20)    11664 2023-01-23 23:20:43.000000 torchgeo-0.4.0/README.md
+-rw-r-----   0 Adam       (501) staff       (20)     5454 2023-01-24 23:29:57.000000 torchgeo-0.4.0/pyproject.toml
+-rw-r-----   0 Adam       (501) staff       (20)     2333 2023-01-24 23:51:50.181335 torchgeo-0.4.0/setup.cfg
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.037776 torchgeo-0.4.0/torchgeo/
+-rw-r-----   0 Adam       (501) staff       (20)      501 2023-01-24 23:51:15.000000 torchgeo-0.4.0/torchgeo/__init__.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.073740 torchgeo-0.4.0/torchgeo/datamodules/
+-rw-r-----   0 Adam       (501) staff       (20)     2088 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)     2425 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/bigearthnet.py
+-rw-r-----   0 Adam       (501) staff       (20)     6684 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/chesapeake.py
+-rw-r-----   0 Adam       (501) staff       (20)     1445 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/cowc.py
+-rw-r-----   0 Adam       (501) staff       (20)     2188 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/cyclone.py
+-rw-r-----   0 Adam       (501) staff       (20)     2362 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/deepglobelandcover.py
+-rw-r-----   0 Adam       (501) staff       (20)     2633 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/etci2021.py
+-rw-r-----   0 Adam       (501) staff       (20)     1706 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/eurosat.py
+-rw-r-----   0 Adam       (501) staff       (20)     1602 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/fair1m.py
+-rw-r-----   0 Adam       (501) staff       (20)    20926 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/geo.py
+-rw-r-----   0 Adam       (501) staff       (20)     2544 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/gid15.py
+-rw-r-----   0 Adam       (501) staff       (20)     3257 2023-01-24 23:29:57.000000 torchgeo-0.4.0/torchgeo/datamodules/inria.py
+-rw-r-----   0 Adam       (501) staff       (20)     1686 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/landcoverai.py
+-rw-r-----   0 Adam       (501) staff       (20)     1442 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/loveda.py
+-rw-r-----   0 Adam       (501) staff       (20)     3835 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/naip.py
+-rw-r-----   0 Adam       (501) staff       (20)     2293 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/nasa_marine_debris.py
+-rw-r-----   0 Adam       (501) staff       (20)     3362 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/oscd.py
+-rw-r-----   0 Adam       (501) staff       (20)     2277 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/potsdam.py
+-rw-r-----   0 Adam       (501) staff       (20)     1698 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/resisc45.py
+-rw-r-----   0 Adam       (501) staff       (20)     4202 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/sen12ms.py
+-rw-r-----   0 Adam       (501) staff       (20)     3017 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/so2sat.py
+-rw-r-----   0 Adam       (501) staff       (20)     3304 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/spacenet.py
+-rw-r-----   0 Adam       (501) staff       (20)     1126 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/ucmerced.py
+-rw-r-----   0 Adam       (501) staff       (20)      889 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/usavars.py
+-rw-r-----   0 Adam       (501) staff       (20)     1829 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/utils.py
+-rw-r-----   0 Adam       (501) staff       (20)     2295 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/vaihingen.py
+-rw-r-----   0 Adam       (501) staff       (20)     1623 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datamodules/xview.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.148336 torchgeo-0.4.0/torchgeo/datasets/
+-rw-r-----   0 Adam       (501) staff       (20)     4655 2023-01-24 23:29:57.000000 torchgeo-0.4.0/torchgeo/datasets/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)     8102 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/advance.py
+-rw-r-----   0 Adam       (501) staff       (20)     5367 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/agb_live_woody_density.py
+-rw-r-----   0 Adam       (501) staff       (20)     4296 2022-12-30 16:35:09.000000 torchgeo-0.4.0/torchgeo/datasets/astergdem.py
+-rw-r-----   0 Adam       (501) staff       (20)    15179 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/benin_cashews.py
+-rw-r-----   0 Adam       (501) staff       (20)    18706 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/bigearthnet.py
+-rw-r-----   0 Adam       (501) staff       (20)     5769 2022-06-27 00:21:59.000000 torchgeo-0.4.0/torchgeo/datasets/cbf.py
+-rw-r-----   0 Adam       (501) staff       (20)    14971 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/cdl.py
+-rw-r-----   0 Adam       (501) staff       (20)    29996 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/chesapeake.py
+-rw-r-----   0 Adam       (501) staff       (20)    13470 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/cloud_cover.py
+-rw-r-----   0 Adam       (501) staff       (20)     8474 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/cms_mangrove_canopy.py
+-rw-r-----   0 Adam       (501) staff       (20)     9485 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/cowc.py
+-rw-r-----   0 Adam       (501) staff       (20)    15047 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/cv4a_kenya_crop_type.py
+-rw-r-----   0 Adam       (501) staff       (20)     8658 2023-01-24 23:29:57.000000 torchgeo-0.4.0/torchgeo/datasets/cyclone.py
+-rw-r-----   0 Adam       (501) staff       (20)     8429 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/deepglobelandcover.py
+-rw-r-----   0 Adam       (501) staff       (20)    11679 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/dfc2022.py
+-rw-r-----   0 Adam       (501) staff       (20)     3738 2022-06-27 00:21:59.000000 torchgeo-0.4.0/torchgeo/datasets/eddmaps.py
+-rw-r-----   0 Adam       (501) staff       (20)    17689 2022-12-19 19:05:17.000000 torchgeo-0.4.0/torchgeo/datasets/enviroatlas.py
+-rw-r-----   0 Adam       (501) staff       (20)     5894 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/esri2020.py
+-rw-r-----   0 Adam       (501) staff       (20)    10617 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/etci2021.py
+-rw-r-----   0 Adam       (501) staff       (20)     7250 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/eudem.py
+-rw-r-----   0 Adam       (501) staff       (20)     9721 2023-01-23 05:39:08.000000 torchgeo-0.4.0/torchgeo/datasets/eurosat.py
+-rw-r-----   0 Adam       (501) staff       (20)    10709 2023-01-12 18:45:34.000000 torchgeo-0.4.0/torchgeo/datasets/fair1m.py
+-rw-r-----   0 Adam       (501) staff       (20)    10182 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/forestdamage.py
+-rw-r-----   0 Adam       (501) staff       (20)     4586 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/gbif.py
+-rw-r-----   0 Adam       (501) staff       (20)    34378 2023-01-24 23:29:57.000000 torchgeo-0.4.0/torchgeo/datasets/geo.py
+-rw-r-----   0 Adam       (501) staff       (20)     8406 2023-01-23 04:47:21.000000 torchgeo-0.4.0/torchgeo/datasets/gid15.py
+-rw-r-----   0 Adam       (501) staff       (20)    10988 2022-12-19 19:05:17.000000 torchgeo-0.4.0/torchgeo/datasets/globbiomass.py
+-rw-r-----   0 Adam       (501) staff       (20)    20256 2023-01-23 23:17:09.000000 torchgeo-0.4.0/torchgeo/datasets/idtrees.py
+-rw-r-----   0 Adam       (501) staff       (20)     3863 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/inaturalist.py
+-rw-r-----   0 Adam       (501) staff       (20)     7387 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/inria.py
+-rw-r-----   0 Adam       (501) staff       (20)     8686 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/landcoverai.py
+-rw-r-----   0 Adam       (501) staff       (20)     6334 2022-09-21 14:05:11.000000 torchgeo-0.4.0/torchgeo/datasets/landsat.py
+-rw-r-----   0 Adam       (501) staff       (20)     7906 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/levircd.py
+-rw-r-----   0 Adam       (501) staff       (20)     9056 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/loveda.py
+-rw-r-----   0 Adam       (501) staff       (20)    10422 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/millionaid.py
+-rw-r-----   0 Adam       (501) staff       (20)     2751 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/naip.py
+-rw-r-----   0 Adam       (501) staff       (20)     8816 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/nasa_marine_debris.py
+-rw-r-----   0 Adam       (501) staff       (20)    20448 2023-01-23 19:04:19.000000 torchgeo-0.4.0/torchgeo/datasets/openbuildings.py
+-rw-r-----   0 Adam       (501) staff       (20)    10350 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/oscd.py
+-rw-r-----   0 Adam       (501) staff       (20)     5454 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/patternnet.py
+-rw-r-----   0 Adam       (501) staff       (20)     8769 2023-01-16 22:12:00.000000 torchgeo-0.4.0/torchgeo/datasets/potsdam.py
+-rw-r-----   0 Adam       (501) staff       (20)     8734 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/reforestree.py
+-rw-r-----   0 Adam       (501) staff       (20)     8244 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/resisc45.py
+-rw-r-----   0 Adam       (501) staff       (20)     9676 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/seco.py
+-rw-r-----   0 Adam       (501) staff       (20)    11510 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/sen12ms.py
+-rw-r-----   0 Adam       (501) staff       (20)    13478 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/sentinel.py
+-rw-r-----   0 Adam       (501) staff       (20)    10256 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/so2sat.py
+-rw-r-----   0 Adam       (501) staff       (20)    45386 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/spacenet.py
+-rw-r-----   0 Adam       (501) staff       (20)     7663 2022-07-13 15:53:56.000000 torchgeo-0.4.0/torchgeo/datasets/ucmerced.py
+-rw-r-----   0 Adam       (501) staff       (20)     9386 2023-01-24 23:21:50.000000 torchgeo-0.4.0/torchgeo/datasets/usavars.py
+-rw-r-----   0 Adam       (501) staff       (20)    21283 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/utils.py
+-rw-r-----   0 Adam       (501) staff       (20)     9260 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/vaihingen.py
+-rw-r-----   0 Adam       (501) staff       (20)    17851 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/datasets/vhr10.py
+-rw-r-----   0 Adam       (501) staff       (20)     9142 2022-12-19 19:05:17.000000 torchgeo-0.4.0/torchgeo/datasets/xview.py
+-rw-r-----   0 Adam       (501) staff       (20)    10230 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/datasets/zuericrop.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.151969 torchgeo-0.4.0/torchgeo/losses/
+-rw-r-----   0 Adam       (501) staff       (20)      182 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/losses/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)     2034 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/losses/qr.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.163692 torchgeo-0.4.0/torchgeo/models/
+-rw-r-----   0 Adam       (501) staff       (20)      907 2023-01-23 05:39:05.000000 torchgeo-0.4.0/torchgeo/models/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)     2344 2023-01-23 05:39:05.000000 torchgeo-0.4.0/torchgeo/models/api.py
+-rw-r-----   0 Adam       (501) staff       (20)     7746 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/models/changestar.py
+-rw-r-----   0 Adam       (501) staff       (20)     8039 2023-01-23 05:39:05.000000 torchgeo-0.4.0/torchgeo/models/farseg.py
+-rw-r-----   0 Adam       (501) staff       (20)     1993 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/models/fcn.py
+-rw-r-----   0 Adam       (501) staff       (20)     8246 2023-01-16 19:59:45.000000 torchgeo-0.4.0/torchgeo/models/fcsiam.py
+-rw-r-----   0 Adam       (501) staff       (20)     3339 2023-01-23 04:47:21.000000 torchgeo-0.4.0/torchgeo/models/rcf.py
+-rw-r-----   0 Adam       (501) staff       (20)     7014 2023-01-23 05:39:05.000000 torchgeo-0.4.0/torchgeo/models/resnet.py
+-rw-r-----   0 Adam       (501) staff       (20)     3018 2023-01-23 05:39:05.000000 torchgeo-0.4.0/torchgeo/models/vit.py
+-rw-r-----   0 Adam       (501) staff       (20)        0 2022-06-27 00:21:59.000000 torchgeo-0.4.0/torchgeo/py.typed
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.168468 torchgeo-0.4.0/torchgeo/samplers/
+-rw-r-----   0 Adam       (501) staff       (20)      664 2023-01-16 19:59:46.000000 torchgeo-0.4.0/torchgeo/samplers/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)     5828 2023-01-23 04:47:21.000000 torchgeo-0.4.0/torchgeo/samplers/batch.py
+-rw-r-----   0 Adam       (501) staff       (20)      477 2022-03-20 16:49:39.000000 torchgeo-0.4.0/torchgeo/samplers/constants.py
+-rw-r-----   0 Adam       (501) staff       (20)    11933 2023-01-23 04:47:21.000000 torchgeo-0.4.0/torchgeo/samplers/single.py
+-rw-r-----   0 Adam       (501) staff       (20)     3436 2023-01-16 19:59:46.000000 torchgeo-0.4.0/torchgeo/samplers/utils.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.175835 torchgeo-0.4.0/torchgeo/trainers/
+-rw-r-----   0 Adam       (501) staff       (20)      532 2023-01-16 19:59:46.000000 torchgeo-0.4.0/torchgeo/trainers/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)    14681 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/trainers/byol.py
+-rw-r-----   0 Adam       (501) staff       (20)    14348 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/trainers/classification.py
+-rw-r-----   0 Adam       (501) staff       (20)    11448 2023-01-23 23:44:23.000000 torchgeo-0.4.0/torchgeo/trainers/detection.py
+-rw-r-----   0 Adam       (501) staff       (20)     7558 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/trainers/regression.py
+-rw-r-----   0 Adam       (501) staff       (20)    10681 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/trainers/segmentation.py
+-rw-r-----   0 Adam       (501) staff       (20)     5366 2023-01-23 19:04:19.000000 torchgeo-0.4.0/torchgeo/trainers/utils.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.178422 torchgeo-0.4.0/torchgeo/transforms/
+-rw-r-----   0 Adam       (501) staff       (20)      826 2023-01-16 19:59:46.000000 torchgeo-0.4.0/torchgeo/transforms/__init__.py
+-rw-r-----   0 Adam       (501) staff       (20)    12842 2023-01-23 19:04:19.000000 torchgeo-0.4.0/torchgeo/transforms/indices.py
+-rw-r-----   0 Adam       (501) staff       (20)     5502 2023-01-23 23:20:43.000000 torchgeo-0.4.0/torchgeo/transforms/transforms.py
+drwxr-x---   0 Adam       (501) staff       (20)        0 2023-01-24 23:51:50.041494 torchgeo-0.4.0/torchgeo.egg-info/
+-rw-r-----   0 Adam       (501) staff       (20)    12770 2023-01-24 23:51:50.000000 torchgeo-0.4.0/torchgeo.egg-info/PKG-INFO
+-rw-r-----   0 Adam       (501) staff       (20)     3565 2023-01-24 23:51:50.000000 torchgeo-0.4.0/torchgeo.egg-info/SOURCES.txt
+-rw-r-----   0 Adam       (501) staff       (20)        1 2023-01-24 23:51:50.000000 torchgeo-0.4.0/torchgeo.egg-info/dependency_links.txt
+-rw-r-----   0 Adam       (501) staff       (20)      863 2023-01-24 23:51:50.000000 torchgeo-0.4.0/torchgeo.egg-info/requires.txt
+-rw-r-----   0 Adam       (501) staff       (20)        9 2023-01-24 23:51:50.000000 torchgeo-0.4.0/torchgeo.egg-info/top_level.txt
```

### Comparing `torchgeo-0.3.1/LICENSE` & `torchgeo-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/PKG-INFO` & `torchgeo-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgeo
-Version: 0.3.1
+Version: 0.4.0
 Summary: TorchGeo: datasets, samplers, transforms, and pre-trained models for geospatial data
 Home-page: https://github.com/microsoft/torchgeo
 Author: Adam J. Stewart
 Author-email: ajstewart426@gmail.com
 Keywords: pytorch,deep learning,machine learning,remote sensing,satellite imagery,earth observation,geospatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -53,15 +53,15 @@
 $ pip install torchgeo
 ```
 
 For [conda](https://docs.conda.io/) and [spack](https://spack.io/) installation instructions, see the [documentation](https://torchgeo.readthedocs.io/en/stable/user/installation.html).
 
 ## Documentation
 
-You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://arxiv.org/abs/2111.08872) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
+You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
 
 ## Example Usage
 
 The following sections give basic examples of what you can do with TorchGeo.
 
 First we'll import various classes and functions used in the following sections:
 
@@ -137,24 +137,24 @@
 for batch in dataloader:
     image = batch["image"]
     label = batch["label"]
 
     # train a model, or make predictions using a pre-trained model
 ```
 
-<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the NWPU VHR-10 dataset"/>
+<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the VHR-10 dataset"/>
 
 All TorchGeo datasets are compatible with PyTorch data loaders, making them easy to integrate into existing training workflows. The only difference between a benchmark dataset in TorchGeo and a similar dataset in torchvision is that each dataset returns a dictionary with keys for each PyTorch `Tensor`.
 
 ### Reproducibility with PyTorch Lightning
 
 In order to facilitate direct comparisons between results published in the literature and further reduce the boilerplate code needed to run experiments with datasets in TorchGeo, we have created PyTorch Lightning [*datamodules*](https://torchgeo.readthedocs.io/en/stable/api/datamodules.html) with well-defined train-val-test splits and [*trainers*](https://torchgeo.readthedocs.io/en/stable/api/trainers.html) for various tasks like classification, regression, and semantic segmentation. These datamodules show how to incorporate augmentations from the kornia library, include preprocessing transforms (with pre-calculated channel statistics), and let users easily experiment with hyperparameters related to the data itself (as opposed to the modeling process). Training a semantic segmentation model on the [Inria Aerial Image Labeling](https://project.inria.fr/aerialimagelabeling/) dataset is as easy as a few imports and four lines of code.
 
 ```python
-datamodule = InriaAerialImageLabelingDataModule(root_dir="...", batch_size=64, num_workers=6)
+datamodule = InriaAerialImageLabelingDataModule(root="...", batch_size=64, num_workers=6)
 task = SemanticSegmentationTask(segmentation_model="unet", encoder_weights="imagenet", learning_rate=0.1)
 trainer = Trainer(gpus=1, default_root_dir="...")
 
 trainer.fit(model=task, datamodule=datamodule)
 ```
 
 <img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/inria.png" alt="Building segmentations produced by a U-Net model trained on the Inria Aerial Image Labeling dataset"/>
@@ -163,23 +163,28 @@
 
 ```console
 $ python train.py config_file=conf/landcoverai.yaml
 ```
 
 ## Citation
 
-If you use this software in your work, please cite our [paper](https://arxiv.org/abs/2111.08872):
+If you use this software in your work, please cite our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953):
 ```
-@article{Stewart_TorchGeo_deep_learning_2021,
+@inproceedings{Stewart_TorchGeo_Deep_Learning_2022,
+    address = {Seattle, Washington},
     author = {Stewart, Adam J. and Robinson, Caleb and Corley, Isaac A. and Ortiz, Anthony and Lavista Ferres, Juan M. and Banerjee, Arindam},
-    journal = {arXiv preprint arXiv:2111.08872},
+    booktitle = {Proceedings of the 30th International Conference on Advances in Geographic Information Systems},
+    doi = {10.1145/3557915.3560953},
     month = {11},
+    pages = {1--12},
+    publisher = {Association for Computing Machinery},
+    series = {SIGSPATIAL '22},
     title = {{TorchGeo}: Deep Learning With Geospatial Data},
-    url = {https://github.com/microsoft/torchgeo},
-    year = {2021}
+    url = {https://dl.acm.org/doi/10.1145/3557915.3560953},
+    year = {2022}
 }
 ```
 
 ## Contributing
 
 This project welcomes contributions and suggestions. If you would like to submit a pull request, see our [Contribution Guide](https://torchgeo.readthedocs.io/en/stable/user/contributing.html) for more information.
```

### Comparing `torchgeo-0.3.1/README.md` & `torchgeo-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 $ pip install torchgeo
 ```
 
 For [conda](https://docs.conda.io/) and [spack](https://spack.io/) installation instructions, see the [documentation](https://torchgeo.readthedocs.io/en/stable/user/installation.html).
 
 ## Documentation
 
-You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://arxiv.org/abs/2111.08872) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
+You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
 
 ## Example Usage
 
 The following sections give basic examples of what you can do with TorchGeo.
 
 First we'll import various classes and functions used in the following sections:
 
@@ -110,24 +110,24 @@
 for batch in dataloader:
     image = batch["image"]
     label = batch["label"]
 
     # train a model, or make predictions using a pre-trained model
 ```
 
-<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the NWPU VHR-10 dataset"/>
+<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the VHR-10 dataset"/>
 
 All TorchGeo datasets are compatible with PyTorch data loaders, making them easy to integrate into existing training workflows. The only difference between a benchmark dataset in TorchGeo and a similar dataset in torchvision is that each dataset returns a dictionary with keys for each PyTorch `Tensor`.
 
 ### Reproducibility with PyTorch Lightning
 
 In order to facilitate direct comparisons between results published in the literature and further reduce the boilerplate code needed to run experiments with datasets in TorchGeo, we have created PyTorch Lightning [*datamodules*](https://torchgeo.readthedocs.io/en/stable/api/datamodules.html) with well-defined train-val-test splits and [*trainers*](https://torchgeo.readthedocs.io/en/stable/api/trainers.html) for various tasks like classification, regression, and semantic segmentation. These datamodules show how to incorporate augmentations from the kornia library, include preprocessing transforms (with pre-calculated channel statistics), and let users easily experiment with hyperparameters related to the data itself (as opposed to the modeling process). Training a semantic segmentation model on the [Inria Aerial Image Labeling](https://project.inria.fr/aerialimagelabeling/) dataset is as easy as a few imports and four lines of code.
 
 ```python
-datamodule = InriaAerialImageLabelingDataModule(root_dir="...", batch_size=64, num_workers=6)
+datamodule = InriaAerialImageLabelingDataModule(root="...", batch_size=64, num_workers=6)
 task = SemanticSegmentationTask(segmentation_model="unet", encoder_weights="imagenet", learning_rate=0.1)
 trainer = Trainer(gpus=1, default_root_dir="...")
 
 trainer.fit(model=task, datamodule=datamodule)
 ```
 
 <img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/inria.png" alt="Building segmentations produced by a U-Net model trained on the Inria Aerial Image Labeling dataset"/>
@@ -136,23 +136,28 @@
 
 ```console
 $ python train.py config_file=conf/landcoverai.yaml
 ```
 
 ## Citation
 
-If you use this software in your work, please cite our [paper](https://arxiv.org/abs/2111.08872):
+If you use this software in your work, please cite our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953):
 ```
-@article{Stewart_TorchGeo_deep_learning_2021,
+@inproceedings{Stewart_TorchGeo_Deep_Learning_2022,
+    address = {Seattle, Washington},
     author = {Stewart, Adam J. and Robinson, Caleb and Corley, Isaac A. and Ortiz, Anthony and Lavista Ferres, Juan M. and Banerjee, Arindam},
-    journal = {arXiv preprint arXiv:2111.08872},
+    booktitle = {Proceedings of the 30th International Conference on Advances in Geographic Information Systems},
+    doi = {10.1145/3557915.3560953},
     month = {11},
+    pages = {1--12},
+    publisher = {Association for Computing Machinery},
+    series = {SIGSPATIAL '22},
     title = {{TorchGeo}: Deep Learning With Geospatial Data},
-    url = {https://github.com/microsoft/torchgeo},
-    year = {2021}
+    url = {https://dl.acm.org/doi/10.1145/3557915.3560953},
+    year = {2022}
 }
 ```
 
 ## Contributing
 
 This project welcomes contributions and suggestions. If you would like to submit a pull request, see our [Contribution Guide](https://torchgeo.readthedocs.io/en/stable/user/contributing.html) for more information.
```

### Comparing `torchgeo-0.3.1/pyproject.toml` & `torchgeo-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
     # setuptools 42+ required for metadata.license_files support in setup.cfg
-    "setuptools>=42,<66",
+    "setuptools>=42,<67",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 target-version = ["py37", "py38", "py39"]
 color = true
 skip_magic_trailing_comma = true
@@ -81,14 +81,24 @@
     # https://github.com/pytorch/pytorch/issues/60053
     # https://github.com/pytorch/pytorch/pull/60059
     "ignore:Named tensors and all their associated APIs are an experimental feature and subject to change:UserWarning:torch.nn.functional",
     # https://github.com/tensorflow/tensorboard/issues/5798
     "ignore:Call to deprecated create function:DeprecationWarning:tensorboard.compat.proto",
     # https://github.com/treebeardtech/nbmake/issues/68
     'ignore:The \(fspath. py.path.local\) argument to NotebookFile is deprecated:pytest.PytestDeprecationWarning:nbmake.pytest_plugin',
+    # https://github.com/lanpa/tensorboardX/issues/653
+    # https://github.com/lanpa/tensorboardX/pull/654
+    "ignore:Call to deprecated create function:DeprecationWarning:tensorboardX",
+    # https://github.com/kornia/kornia/issues/777
+    "ignore:Default upsampling behavior when mode=bilinear is changed to align_corners=False since 0.4.0:UserWarning:torch.nn.functional",
+    # https://github.com/scikit-image/scikit-image/issues/6663
+    # https://github.com/scikit-image/scikit-image/pull/6637
+    "ignore:`np.bool8` is a deprecated alias for `np.bool_`.:DeprecationWarning:skimage.util.dtype",
+    # https://github.com/lanpa/tensorboardX/pull/677
+    "ignore:ANTIALIAS is deprecated and will be removed in Pillow 10:DeprecationWarning:tensorboardX.summary",
 
     # Expected warnings
     # pytorch-lightning warns us about using num_workers=0, but it's faster on macOS
     "ignore:The dataloader, .*, does not have many workers which may be a bottleneck:UserWarning",
     # pytorch-lightning warns us about using the CPU when a GPU is available
     "ignore:GPU available but not used.:UserWarning",
```

### Comparing `torchgeo-0.3.1/setup.cfg` & `torchgeo-0.4.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -20,70 +20,70 @@
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Scientific/Engineering :: GIS
 keywords = pytorch, deep learning, machine learning, remote sensing, satellite imagery, earth observation, geospatial
 
 [options]
 install_requires = 
-	einops>=0.3,<0.5
+	einops>=0.3,<0.7
 	fiona>=1.8,<2
-	kornia>=0.6.4,<0.7
+	kornia>=0.6.5,<0.7
 	matplotlib>=3.3,<4
 	numpy>=1.17.2,<2
 	omegaconf>=2.1,<3
-	packaging>=17,<22
 	pillow>=6.2,<10
 	pyproj>=2.2,<4
-	pytorch-lightning>=1.5.1,<2
+	pytorch-lightning[extra]>=1.5.1,<2
 	rasterio>=1.0.20,<2
 	rtree>=1,<2
 	scikit-learn>=0.21,<2
 	segmentation-models-pytorch>=0.2,<0.4
-	shapely>=1.3,<2
-	timm>=0.4.12,<0.5
-	torch>=1.9,<2
-	torchmetrics>=0.7,<0.10
-	torchvision>=0.10,<0.14
+	shapely>=1.3,<3
+	timm>=0.4.12,<0.7
+	torch>=1.12,<2
+	torchmetrics>=0.10,<0.12
+	torchvision>=0.13,<0.15
 python_requires = ~= 3.7
 packages = find:
 
 [options.package_data]
 torchgeo = py.typed
 
 [options.packages.find]
 include = torchgeo*
 
 [options.extras_require]
 datasets = 
 	h5py>=2.6,<4
 	laspy>=2,<3
-	open3d>=0.11.2,<0.15;python_version<'3.10'
 	opencv-python>=3.4.2.17,<5
 	pandas>=0.23.2,<2
 	pycocotools>=2,<3
+	pyvista>=0.20,<0.38
 	radiant-mlhub>=0.2.1,<0.5
 	rarfile>=3,<5
-	scipy>=1.2,<2
+	scikit-image>=0.18,<0.20
+	scipy>=1.6.2,<2
 	zipfile-deflate64>=0.2,<0.3
 docs = 
 	ipywidgets>=7,<9
 	nbsphinx>=0.8.5,<0.9
 	pytorch-sphinx-theme
-	sphinx>=4,<6
+	sphinx>=4,<7
 style = 
 	black[jupyter]>=21.8,<23
-	flake8>=3.8,<6
+	flake8>=3.8,<7
 	isort[colors]>=5.8,<6
 	pydocstyle[toml]>=6.1,<7
-	pyupgrade>=1.24,<3
+	pyupgrade>=1.24,<4
 tests = 
-	mypy>=0.900,<0.972
+	mypy>=0.900,<0.992
 	nbmake>=0.1,<2
 	pytest>=6.1.2,<8
-	pytest-cov>=2.4,<4
+	pytest-cov>=2.4,<5
 
 [flake8]
 max-line-length = 88
 extend-ignore = 
 	E203,
 exclude = 
 	data/,
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/__init__.py` & `torchgeo-0.4.0/torchgeo/datamodules/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,57 +2,64 @@
 # Licensed under the MIT License.
 
 """TorchGeo datamodules."""
 
 from .bigearthnet import BigEarthNetDataModule
 from .chesapeake import ChesapeakeCVPRDataModule
 from .cowc import COWCCountingDataModule
-from .cyclone import CycloneDataModule
+from .cyclone import TropicalCycloneDataModule
 from .deepglobelandcover import DeepGlobeLandCoverDataModule
 from .etci2021 import ETCI2021DataModule
 from .eurosat import EuroSATDataModule
 from .fair1m import FAIR1MDataModule
+from .geo import GeoDataModule, NonGeoDataModule
+from .gid15 import GID15DataModule
 from .inria import InriaAerialImageLabelingDataModule
 from .landcoverai import LandCoverAIDataModule
 from .loveda import LoveDADataModule
 from .naip import NAIPChesapeakeDataModule
 from .nasa_marine_debris import NASAMarineDebrisDataModule
 from .oscd import OSCDDataModule
 from .potsdam import Potsdam2DDataModule
 from .resisc45 import RESISC45DataModule
 from .sen12ms import SEN12MSDataModule
 from .so2sat import So2SatDataModule
+from .spacenet import SpaceNet1DataModule
 from .ucmerced import UCMercedDataModule
 from .usavars import USAVarsDataModule
+from .utils import MisconfigurationException
 from .vaihingen import Vaihingen2DDataModule
 from .xview import XView2DataModule
 
 __all__ = (
     # GeoDataset
     "ChesapeakeCVPRDataModule",
     "NAIPChesapeakeDataModule",
     # NonGeoDataset
     "BigEarthNetDataModule",
     "COWCCountingDataModule",
     "DeepGlobeLandCoverDataModule",
     "ETCI2021DataModule",
     "EuroSATDataModule",
     "FAIR1MDataModule",
+    "GID15DataModule",
     "InriaAerialImageLabelingDataModule",
     "LandCoverAIDataModule",
     "LoveDADataModule",
     "NASAMarineDebrisDataModule",
     "OSCDDataModule",
     "Potsdam2DDataModule",
     "RESISC45DataModule",
     "SEN12MSDataModule",
     "So2SatDataModule",
-    "CycloneDataModule",
+    "SpaceNet1DataModule",
+    "TropicalCycloneDataModule",
     "UCMercedDataModule",
     "USAVarsDataModule",
     "Vaihingen2DDataModule",
     "XView2DataModule",
+    # Base classes
+    "GeoDataModule",
+    "NonGeoDataModule",
+    # Utilities
+    "MisconfigurationException",
 )
-
-# https://stackoverflow.com/questions/40018681
-for module in __all__:
-    globals()[module].__module__ = "torchgeo.datamodules"
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/chesapeake.py` & `torchgeo-0.4.0/torchgeo/datasets/forestdamage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,352 +1,332 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""Chesapeake Bay High-Resolution Land Cover Project datamodule."""
-
-from typing import Any, Callable, Dict, List, Optional
+"""Forest Damage dataset."""
 
+import glob
+import os
+from typing import Any, Callable, Dict, List, Optional, Tuple
+from xml.etree import ElementTree
+
+import matplotlib.patches as patches
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
-import torch.nn.functional as F
-from pytorch_lightning.core.datamodule import LightningDataModule
+from PIL import Image
 from torch import Tensor
-from torch.utils.data import DataLoader
-from torchvision.transforms import Compose
 
-from ..datasets import ChesapeakeCVPR, stack_samples
-from ..samplers.batch import RandomBatchGeoSampler
-from ..samplers.single import GridGeoSampler
+from .geo import NonGeoDataset
+from .utils import check_integrity, download_and_extract_archive, extract_archive
+
+
+def parse_pascal_voc(path: str) -> Dict[str, Any]:
+    """Read a PASCAL VOC annotation file.
+
+    Args:
+        path: path to xml file
+
+    Returns:
+        dict of image filename, points, and class labels
+    """
+    et = ElementTree.parse(path)
+    element = et.getroot()
+    filename = element.find("filename").text  # type: ignore[union-attr]
+    labels, bboxes = [], []
+    for obj in element.findall("object"):
+        bndbox = obj.find("bndbox")
+        bbox = [
+            int(bndbox.find("xmin").text),  # type: ignore[union-attr, arg-type]
+            int(bndbox.find("ymin").text),  # type: ignore[union-attr, arg-type]
+            int(bndbox.find("xmax").text),  # type: ignore[union-attr, arg-type]
+            int(bndbox.find("ymax").text),  # type: ignore[union-attr, arg-type]
+        ]
+
+        label_var = obj.find("damage")
+        if label_var is not None:
+            label = label_var.text
+        else:
+            label = "other"
+        bboxes.append(bbox)
+        labels.append(label)
+    return dict(filename=filename, bboxes=bboxes, labels=labels)
+
+
+class ForestDamage(NonGeoDataset):
+    """Forest Damage dataset.
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
+    The `ForestDamage
+    <https://lila.science/datasets/forest-damages-larch-casebearer/>`_
+    dataset contains drone imagery that can be used for tree identification,
+    as well as tree damage classification for larch trees.
 
+    Dataset features:
 
-class ChesapeakeCVPRDataModule(LightningDataModule):
-    """LightningDataModule implementation for the Chesapeake CVPR Land Cover dataset.
+    * 1543 images
+    * 101,878 tree annotations
+    * subset of 840 images contain 44,522 annotations about tree health
+      (Healthy (H), Light Damage (LD), High Damage (HD)), all other
+      images have "other" as damage level
 
-    Uses the random splits defined per state to partition tiles into train, val,
-    and test sets.
+    Dataset format:
+
+    * images are three-channel jpgs
+    * annotations are in `Pascal VOC XML format
+      <https://roboflow.com/formats/pascal-voc-xml#w-tabs-0-data-w-pane-3>`_
+
+    Dataset Classes:
+
+    0. other
+    1. healthy
+    2. light damage
+    3. high damage
+
+    If the download fails or stalls, it is recommended to try azcopy
+    as suggested `here <https://lila.science/faq>`__. It is expected that the
+    downloaded data file with name ``Data_Set_Larch_Casebearer``
+    can be found in ``root``.
+
+    If you use this dataset in your research, please use the following citation:
+
+    * Swedish Forest Agency (2021): Forest Damages - Larch Casebearer 1.0.
+      National Forest Data Lab. Dataset.
+
+    .. versionadded:: 0.3
     """
 
+    classes = ["other", "H", "LD", "HD"]
+    url = (
+        "https://lilablobssc.blob.core.windows.net/larch-casebearer/"
+        "Data_Set_Larch_Casebearer.zip"
+    )
+    data_dir = "Data_Set_Larch_Casebearer"
+    md5 = "907815bcc739bff89496fac8f8ce63d7"
+
     def __init__(
         self,
-        root_dir: str,
-        train_splits: List[str],
-        val_splits: List[str],
-        test_splits: List[str],
-        patches_per_tile: int = 200,
-        patch_size: int = 256,
-        batch_size: int = 64,
-        num_workers: int = 0,
-        class_set: int = 7,
-        use_prior_labels: bool = False,
-        prior_smoothing_constant: float = 1e-4,
-        **kwargs: Any,
+        root: str = "data",
+        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
+        download: bool = False,
+        checksum: bool = False,
     ) -> None:
-        """Initialize a LightningDataModule for Chesapeake CVPR based DataLoaders.
+        """Initialize a new ForestDamage dataset instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the ChesapeakeCVPR Dataset
-                classes
-            train_splits: The splits used to train the model, e.g. ["ny-train"]
-            val_splits: The splits used to validate the model, e.g. ["ny-val"]
-            test_splits: The splits used to test the model, e.g. ["ny-test"]
-            patches_per_tile: The number of patches per tile to sample
-            patch_size: The size of each patch in pixels (test patches will be 1.5 times
-                this size)
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
-            class_set: The high-resolution land cover class set to use - 5 or 7
-            use_prior_labels: Flag for using a prior over high-resolution classes
-                instead of the high-resolution labels themselves
-            prior_smoothing_constant: additive smoothing to add when using prior labels
+            root: root directory where dataset can be found
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
+            download: if True, download dataset and store it in the root directory
+            checksum: if True, check the MD5 of the downloaded files (may be slow)
 
         Raises:
-            ValueError: if ``use_prior_labels`` is used with ``class_set==7``
+            RuntimeError: if ``download=False`` and data is not found, or checksums
+                don't match
         """
-        super().__init__()
-        for state in train_splits + val_splits + test_splits:
-            assert state in ChesapeakeCVPR.splits
-        assert class_set in [5, 7]
-        if use_prior_labels and class_set != 5:
-            raise ValueError(
-                "The pre-generated prior labels are only valid for the 5"
-                + " class set of labels"
-            )
+        self.root = root
+        self.transforms = transforms
+        self.checksum = checksum
+        self.download = download
 
-        self.root_dir = root_dir
-        self.train_splits = train_splits
-        self.val_splits = val_splits
-        self.test_splits = test_splits
-        self.patches_per_tile = patches_per_tile
-        self.patch_size = patch_size
-        # This is a rough estimate of how large of a patch we will need to sample in
-        # EPSG:3857 in order to guarantee a large enough patch in the local CRS.
-        self.original_patch_size = patch_size * 2
-        self.batch_size = batch_size
-        self.num_workers = num_workers
-        self.class_set = class_set
-        self.use_prior_labels = use_prior_labels
-        self.prior_smoothing_constant = prior_smoothing_constant
-
-        if self.use_prior_labels:
-            self.layers = [
-                "naip-new",
-                "prior_from_cooccurrences_101_31_no_osm_no_buildings",
-            ]
-        else:
-            self.layers = ["naip-new", "lc"]
+        self._verify()
+
+        self.files = self._load_files(self.root)
 
-    def pad_to(
-        self, size: int = 512, image_value: int = 0, mask_value: int = 0
-    ) -> Callable[[Dict[str, Tensor]], Dict[str, Tensor]]:
-        """Returns a function to perform a padding transform on a single sample.
+        self.class_to_idx: Dict[str, int] = {c: i for i, c in enumerate(self.classes)}
+
+    def __getitem__(self, index: int) -> Dict[str, Tensor]:
+        """Return an index within the dataset.
 
         Args:
-            size: output image size
-            image_value: value to pad image with
-            mask_value: value to pad mask with
+            index: index to return
 
         Returns:
-            function to perform padding
+            data and label at that index
         """
+        files = self.files[index]
+        parsed = parse_pascal_voc(files["annotation"])
+        image = self._load_image(files["image"])
 
-        def pad_inner(sample: Dict[str, Tensor]) -> Dict[str, Tensor]:
-            _, height, width = sample["image"].shape
-            assert height <= size and width <= size
-
-            height_pad = size - height
-            width_pad = size - width
-
-            # See https://pytorch.org/docs/stable/generated/torch.nn.functional.pad.html
-            # for a description of the format of the padding tuple
-            sample["image"] = F.pad(
-                sample["image"],
-                (0, width_pad, 0, height_pad),
-                mode="constant",
-                value=image_value,
-            )
-            sample["mask"] = F.pad(
-                sample["mask"],
-                (0, width_pad, 0, height_pad),
-                mode="constant",
-                value=mask_value,
-            )
-            return sample
+        boxes, labels = self._load_target(parsed["bboxes"], parsed["labels"])
 
-        return pad_inner
+        sample = {"image": image, "boxes": boxes, "label": labels}
 
-    def center_crop(
-        self, size: int = 512
-    ) -> Callable[[Dict[str, Tensor]], Dict[str, Tensor]]:
-        """Returns a function to perform a center crop transform on a single sample.
+        if self.transforms is not None:
+            sample = self.transforms(sample)
 
-        Args:
-            size: output image size
+        return sample
+
+    def __len__(self) -> int:
+        """Return the number of data points in the dataset.
 
         Returns:
-            function to perform center crop
+            length of the dataset
         """
+        return len(self.files)
 
-        def center_crop_inner(sample: Dict[str, Tensor]) -> Dict[str, Tensor]:
-            _, height, width = sample["image"].shape
-
-            y1 = round((height - size) / 2)
-            x1 = round((width - size) / 2)
-            sample["image"] = sample["image"][:, y1 : y1 + size, x1 : x1 + size]
-            sample["mask"] = sample["mask"][:, y1 : y1 + size, x1 : x1 + size]
-
-            return sample
-
-        return center_crop_inner
-
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Preprocesses a single sample.
+    def _load_files(self, root: str) -> List[Dict[str, str]]:
+        """Return the paths of the files in the dataset.
 
         Args:
-            sample: sample dictionary containing image and mask
+            root: root dir of dataset
 
         Returns:
-            preprocessed sample
+            list of dicts containing paths for each pair of image, annotation
         """
-        sample["image"] = sample["image"].float()
-        sample["image"] /= 255.0
+        images = sorted(
+            glob.glob(os.path.join(root, self.data_dir, "**", "Images", "*.JPG"))
+        )
+        annotations = sorted(
+            glob.glob(os.path.join(root, self.data_dir, "**", "Annotations", "*.xml"))
+        )
 
-        if "mask" in sample:
-            sample["mask"] = sample["mask"].squeeze()
-            if self.use_prior_labels:
-                sample["mask"] = F.normalize(sample["mask"].float(), p=1, dim=0)
-                sample["mask"] = F.normalize(
-                    sample["mask"] + self.prior_smoothing_constant, p=1, dim=0
-                )
-            else:
-                if self.class_set == 5:
-                    sample["mask"][sample["mask"] == 5] = 4
-                    sample["mask"][sample["mask"] == 6] = 4
-                sample["mask"] = sample["mask"].long()
+        files = [
+            dict(image=image, annotation=annotation)
+            for image, annotation in zip(images, annotations)
+        ]
 
-        return sample
+        return files
 
-    def remove_bbox(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Removes the bounding box property from a sample.
+    def _load_image(self, path: str) -> Tensor:
+        """Load a single image.
 
         Args:
-            sample: dictionary with geographic metadata
+            path: path to the image
 
-        Returns
-            sample without the bbox property
+        Returns:
+            the image
         """
-        del sample["bbox"]
-        return sample
-
-    def nodata_check(
-        self, size: int = 512
-    ) -> Callable[[Dict[str, Tensor]], Dict[str, Tensor]]:
-        """Returns a function to check for nodata or mis-sized input.
+        with Image.open(path) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
+            tensor: Tensor = torch.from_numpy(array)
+            # Convert from HxWxC to CxHxW
+            tensor = tensor.permute((2, 0, 1))
+            return tensor
+
+    def _load_target(
+        self, bboxes: List[List[int]], labels_list: List[str]
+    ) -> Tuple[Tensor, Tensor]:
+        """Load the target mask for a single image.
 
         Args:
-            size: output image size
+            bboxes: list of bbox coordinats [xmin, ymin, xmax, ymax]
+            labels_list: list of class labels
 
         Returns:
-            function to check for nodata values
+            the target bounding boxes and labels
         """
+        labels = torch.tensor([self.class_to_idx[label] for label in labels_list])
+        boxes = torch.tensor(bboxes).to(torch.float)
+        return boxes, labels
 
-        def nodata_check_inner(sample: Dict[str, Tensor]) -> Dict[str, Tensor]:
-            num_channels, height, width = sample["image"].shape
-
-            if height < size or width < size:
-                sample["image"] = torch.zeros((num_channels, size, size))
-                sample["mask"] = torch.zeros((size, size))
-
-            return sample
+    def _verify(self) -> None:
+        """Checks the integrity of the dataset structure.
 
-        return nodata_check_inner
-
-    def prepare_data(self) -> None:
-        """Confirms that the dataset is downloaded on the local node.
-
-        This method is called once per node, while :func:`setup` is called once per GPU.
+        Returns:
+            True if the dataset directories are found, else False
         """
-        ChesapeakeCVPR(
-            self.root_dir,
-            splits=self.train_splits,
-            layers=self.layers,
-            transforms=None,
-            download=False,
-            checksum=False,
-        )
+        filepath = os.path.join(self.root, self.data_dir)
+        if os.path.isdir(filepath):
+            return
+
+        filepath = os.path.join(self.root, self.data_dir + ".zip")
+        if os.path.isfile(filepath):
+            if self.checksum and not check_integrity(filepath, self.md5):
+                raise RuntimeError("Dataset found, but corrupted.")
+            extract_archive(filepath)
+            return
+
+        # Check if the user requested to download the dataset
+        if not self.download:
+            raise RuntimeError(
+                "Dataset not found in `root` directory, either specify a different"
+                + " `root` directory or manually download "
+                + "the dataset to this directory."
+            )
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Create the train/val/test splits based on the original Dataset objects.
+        # else download the dataset
+        self._download()
 
-        The splits should be done here vs. in :func:`__init__` per the docs:
-        https://pytorch-lightning.readthedocs.io/en/latest/extensions/datamodules.html#setup.
+    def _download(self) -> None:
+        """Download the dataset and extract it.
 
-        Args:
-            stage: stage to set up
+        Raises:
+            AssertionError: if the checksum does not match
         """
-        train_transforms = Compose(
-            [
-                self.center_crop(self.patch_size),
-                self.nodata_check(self.patch_size),
-                self.preprocess,
-                self.remove_bbox,
-            ]
-        )
-        val_transforms = Compose(
-            [
-                self.center_crop(self.patch_size),
-                self.nodata_check(self.patch_size),
-                self.preprocess,
-                self.remove_bbox,
-            ]
-        )
-        test_transforms = Compose(
-            [
-                self.pad_to(self.original_patch_size, image_value=0, mask_value=0),
-                self.preprocess,
-                self.remove_bbox,
-            ]
+        download_and_extract_archive(
+            self.url,
+            self.root,
+            filename=self.data_dir + ".zip",
+            md5=self.md5 if self.checksum else None,
         )
 
-        self.train_dataset = ChesapeakeCVPR(
-            self.root_dir,
-            splits=self.train_splits,
-            layers=self.layers,
-            transforms=train_transforms,
-            download=False,
-            checksum=False,
-        )
-        self.val_dataset = ChesapeakeCVPR(
-            self.root_dir,
-            splits=self.val_splits,
-            layers=self.layers,
-            transforms=val_transforms,
-            download=False,
-            checksum=False,
-        )
-        self.test_dataset = ChesapeakeCVPR(
-            self.root_dir,
-            splits=self.test_splits,
-            layers=self.layers,
-            transforms=test_transforms,
-            download=False,
-            checksum=False,
-        )
+    def plot(
+        self,
+        sample: Dict[str, Tensor],
+        show_titles: bool = True,
+        suptitle: Optional[str] = None,
+    ) -> plt.Figure:
+        """Plot a sample from the dataset.
 
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
+        Args:
+            sample: a sample returned by :meth:`__getitem__`
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional string to use as a suptitle
 
         Returns:
-            training data loader
+            a matplotlib Figure with the rendered sample
         """
-        sampler = RandomBatchGeoSampler(
-            self.train_dataset,
-            size=self.original_patch_size,
-            batch_size=self.batch_size,
-            length=self.patches_per_tile * len(self.train_dataset),
-        )
-        return DataLoader(
-            self.train_dataset,
-            batch_sampler=sampler,
-            num_workers=self.num_workers,
-            collate_fn=stack_samples,
-        )
+        image = sample["image"].permute((1, 2, 0)).numpy()
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+        ncols = 1
+        showing_predictions = "prediction_boxes" in sample
+        if showing_predictions:
+            ncols += 1
+
+        fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
+        if not showing_predictions:
+            axs = [axs]
+
+        axs[0].imshow(image)
+        axs[0].axis("off")
+
+        bboxes = [
+            patches.Rectangle(
+                (bbox[0], bbox[1]),
+                bbox[2] - bbox[0],
+                bbox[3] - bbox[1],
+                linewidth=1,
+                edgecolor="r",
+                facecolor="none",
+            )
+            for bbox in sample["boxes"].numpy()
+        ]
+        for bbox in bboxes:
+            axs[0].add_patch(bbox)
+
+        if show_titles:
+            axs[0].set_title("Ground Truth")
+
+        if showing_predictions:
+            axs[1].imshow(image)
+            axs[1].axis("off")
+
+            pred_bboxes = [
+                patches.Rectangle(
+                    (bbox[0], bbox[1]),
+                    bbox[2] - bbox[0],
+                    bbox[3] - bbox[1],
+                    linewidth=1,
+                    edgecolor="r",
+                    facecolor="none",
+                )
+                for bbox in sample["prediction_boxes"].numpy()
+            ]
+            for bbox in pred_bboxes:
+                axs[1].add_patch(bbox)
 
-        Returns:
-            validation data loader
-        """
-        sampler = GridGeoSampler(
-            self.val_dataset,
-            size=self.original_patch_size,
-            stride=self.original_patch_size,
-        )
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            sampler=sampler,
-            num_workers=self.num_workers,
-            collate_fn=stack_samples,
-        )
+            if show_titles:
+                axs[1].set_title("Predictions")
 
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
+        if suptitle is not None:
+            plt.suptitle(suptitle)
 
-        Returns:
-            testing data loader
-        """
-        sampler = GridGeoSampler(
-            self.test_dataset,
-            size=self.original_patch_size,
-            stride=self.original_patch_size,
-        )
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            sampler=sampler,
-            num_workers=self.num_workers,
-            collate_fn=stack_samples,
-        )
+        return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/cowc.py` & `torchgeo-0.4.0/torchgeo/datamodules/naip.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,110 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""COWC datamodule."""
+"""National Agriculture Imagery Program (NAIP) datamodule."""
 
-from typing import Any, Dict, Optional
+from typing import Any, Tuple, Union
 
+import kornia.augmentation as K
 import matplotlib.pyplot as plt
-import pytorch_lightning as pl
-from torch import Generator
-from torch.utils.data import DataLoader, random_split
 
-from ..datasets import COWCCounting
+from ..datasets import NAIP, BoundingBox, Chesapeake13
+from ..samplers import GridGeoSampler, RandomBatchGeoSampler
+from ..transforms import AugmentationSequential
+from .geo import GeoDataModule
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
 
+class NAIPChesapeakeDataModule(GeoDataModule):
+    """LightningDataModule implementation for the NAIP and Chesapeake datasets.
 
-class COWCCountingDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the COWC Counting dataset."""
+    Uses the train/val/test splits from the dataset.
+    """
 
     def __init__(
         self,
-        root_dir: str,
-        seed: int,
         batch_size: int = 64,
+        patch_size: Union[int, Tuple[int, int]] = 256,
+        length: int = 1000,
         num_workers: int = 0,
         **kwargs: Any,
     ) -> None:
-        """Initialize a LightningDataModule for COWC Counting based DataLoaders.
+        """Initialize a new NAIPChesapeakeDataModule instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the COWCCounting Dataset class
-            seed: The seed value to use when doing the dataset random_split
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
-        """
-        super().__init__()
-        self.root_dir = root_dir
-        self.seed = seed
-        self.batch_size = batch_size
-        self.num_workers = num_workers
-
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
-
-        Args:
-            sample: dictionary containing image and target
-
-        Returns:
-            preprocessed sample
-        """
-        sample["image"] = sample["image"].float()
-        sample["image"] /= 255.0  # scale to [0, 1]
-        if "label" in sample:
-            sample["label"] = sample["label"].float()
-        return sample
-
-    def prepare_data(self) -> None:
-        """Initialize the main ``Dataset`` objects for use in :func:`setup`.
-
-        This includes optionally downloading the dataset. This is done once per node,
-        while :func:`setup` is done once per GPU.
-        """
-        COWCCounting(self.root_dir, download=False)
-
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Create the train/val/test splits based on the original Dataset objects.
-
-        The splits should be done here vs. in :func:`__init__` per the docs:
-        https://pytorch-lightning.readthedocs.io/en/latest/extensions/datamodules.html#setup.
-
-        Args:
-            stage: stage to set up
-        """
-        train_val_dataset = COWCCounting(
-            self.root_dir, split="train", transforms=self.preprocess
-        )
-        self.test_dataset = COWCCounting(
-            self.root_dir, split="test", transforms=self.preprocess
-        )
-        self.train_dataset, self.val_dataset = random_split(
-            train_val_dataset,
-            [len(train_val_dataset) - len(self.test_dataset), len(self.test_dataset)],
-            generator=Generator().manual_seed(self.seed),
+            batch_size: Size of each mini-batch.
+            patch_size: Size of each patch, either ``size`` or ``(height, width)``.
+            length: Length of each training epoch.
+            num_workers: Number of workers for parallel data loading.
+            **kwargs: Additional keyword arguments passed to
+                :class:`~torchgeo.datasets.NAIP` (prefix keys with ``naip_``) and
+                :class:`~torchgeo.datasets.Chesapeake13`
+                (prefix keys with ``chesapeake_``).
+        """
+        self.naip_kwargs = {}
+        self.chesapeake_kwargs = {}
+        for key, val in kwargs.items():
+            if key.startswith("naip_"):
+                self.naip_kwargs[key[5:]] = val
+            elif key.startswith("chesapeake_"):
+                self.chesapeake_kwargs[key[11:]] = val
+
+        super().__init__(
+            Chesapeake13,
+            batch_size,
+            patch_size,
+            length,
+            num_workers,
+            **self.chesapeake_kwargs,
         )
 
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
-
-        Returns:
-            training data loader
-        """
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=True,
+        self.aug = AugmentationSequential(
+            K.Normalize(mean=self.mean, std=self.std), data_keys=["image", "mask"]
         )
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+    def setup(self, stage: str) -> None:
+        """Set up datasets and samplers.
 
-        Returns:
-            validation data loader
+        Args:
+            stage: Either 'fit', 'validate', 'test', or 'predict'.
         """
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+        self.chesapeake = Chesapeake13(**self.chesapeake_kwargs)
+        self.naip = NAIP(**self.naip_kwargs)
+        self.dataset = self.chesapeake & self.naip
+
+        roi = self.dataset.bounds
+        midx = roi.minx + (roi.maxx - roi.minx) / 2
+        midy = roi.miny + (roi.maxy - roi.miny) / 2
+
+        if stage in ["fit"]:
+            train_roi = BoundingBox(
+                roi.minx, midx, roi.miny, roi.maxy, roi.mint, roi.maxt
+            )
+            self.train_batch_sampler = RandomBatchGeoSampler(
+                self.dataset, self.patch_size, self.batch_size, self.length, train_roi
+            )
+        if stage in ["fit", "validate"]:
+            val_roi = BoundingBox(midx, roi.maxx, roi.miny, midy, roi.mint, roi.maxt)
+            self.val_sampler = GridGeoSampler(
+                self.dataset, self.patch_size, self.patch_size, val_roi
+            )
+        if stage in ["test"]:
+            test_roi = BoundingBox(
+                roi.minx, roi.maxx, midy, roi.maxy, roi.mint, roi.maxt
+            )
+            self.test_sampler = GridGeoSampler(
+                self.dataset, self.patch_size, self.patch_size, test_roi
+            )
 
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
+    def plot(self, *args: Any, **kwargs: Any) -> plt.Figure:
+        """Run NAIP plot method.
 
-        Returns:
-            testing data loader
-        """
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+        Args:
+            *args: Arguments passed to plot method.
+            **kwargs: Keyword arguments passed to plot method.
 
-    def plot(self, *args: Any, **kwargs: Any) -> plt.Figure:
-        """Run :meth:`torchgeo.datasets.COWC.plot`.
+        Returns:
+            A matplotlib Figure with the image, ground truth, and predictions.
 
-        .. versionadded:: 0.2
+        .. versionadded:: 0.4
         """
-        return self.test_dataset.plot(*args, **kwargs)
+        return self.naip.plot(*args, **kwargs)
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/etci2021.py` & `torchgeo-0.4.0/torchgeo/datamodules/sen12ms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,115 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""ETCI 2021 datamodule."""
+"""SEN12MS datamodule."""
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 
-import matplotlib.pyplot as plt
-import pytorch_lightning as pl
 import torch
-from torch import Generator
-from torch.utils.data import DataLoader, random_split
-from torchvision.transforms import Normalize
+from sklearn.model_selection import GroupShuffleSplit
+from torch import Tensor
+from torch.utils.data import Subset
 
-from ..datasets import ETCI2021
+from ..datasets import SEN12MS
+from .geo import NonGeoDataModule
 
 
-class ETCI2021DataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the ETCI2021 dataset.
+class SEN12MSDataModule(NonGeoDataModule):
+    """LightningDataModule implementation for the SEN12MS dataset.
 
-    Splits the existing train split from the dataset into train/val with 80/20
-    proportions, then uses the existing val dataset as the test data.
+    Implements 80/20 geographic train/val splits and uses the test split from the
+    classification dataset definitions.
 
-    .. versionadded:: 0.2
+    Uses the Simplified IGBP scheme defined in the 2020 Data Fusion Competition. See
+    https://arxiv.org/abs/2002.08254.
     """
 
-    band_means = torch.tensor(
-        [0.52253931, 0.52253931, 0.52253931, 0.61221701, 0.61221701, 0.61221701]
+    #: Mapping from the IGBP class definitions to the DFC2020, taken from the dataloader
+    #: here: https://github.com/lukasliebel/dfc2020_baseline.
+    DFC2020_CLASS_MAPPING = torch.tensor(
+        [0, 1, 1, 1, 1, 1, 2, 2, 3, 3, 4, 5, 6, 7, 6, 8, 9, 10]
     )
 
-    band_stds = torch.tensor(
-        [0.35221376, 0.35221376, 0.35221376, 0.37364622, 0.37364622, 0.37364622]
+    std = torch.tensor(
+        [-25, -25, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4, 1e4]
     )
 
     def __init__(
         self,
-        root_dir: str,
-        seed: int = 0,
         batch_size: int = 64,
         num_workers: int = 0,
+        band_set: str = "all",
         **kwargs: Any,
     ) -> None:
-        """Initialize a LightningDataModule for ETCI2021 based DataLoaders.
+        """Initialize a new SEN12MSDataModule instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the ETCI2021 Dataset classes
-            seed: The seed value to use when doing the dataset random_split
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
-        """
-        super().__init__()
-        self.root_dir = root_dir
-        self.seed = seed
-        self.batch_size = batch_size
-        self.num_workers = num_workers
-
-        self.norm = Normalize(self.band_means, self.band_stds)
+            batch_size: Size of each mini-batch.
+            num_workers: Number of workers for parallel data loading.
+            band_set: Subset of S1/S2 bands to use. Options are: "all",
+                "s1", "s2-all", and "s2-reduced" where the "s2-reduced" set includes:
+                B2, B3, B4, B8, B11, and B12.
+            **kwargs: Additional keyword arguments passed to
+                :class:`~torchgeo.datasets.SEN12MS`.
+        """
+        kwargs["bands"] = SEN12MS.BAND_SETS[band_set]
+
+        if band_set == "s1":
+            self.std = self.std[:2]
+        elif band_set == "s2-all":
+            self.std = self.std[2:]
+        elif band_set == "s2-reduced":
+            self.std = self.std[torch.tensor([3, 4, 5, 9, 12, 13])]
 
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
+        super().__init__(SEN12MS, batch_size, num_workers, **kwargs)
 
-        Notably, moves the given water mask to act as an input layer.
+    def setup(self, stage: str) -> None:
+        """Set up datasets.
 
         Args:
-            sample: input image dictionary
-
-        Returns:
-            preprocessed sample
-        """
-        sample["image"] = sample["image"].float()
-        sample["image"] /= 255.0
-        sample["image"] = self.norm(sample["image"])
-
-        if "mask" in sample:
-            flood_mask = sample["mask"][1]
-            flood_mask = (flood_mask > 0).long()
-            sample["mask"] = flood_mask
-
-        return sample
-
-    def prepare_data(self) -> None:
-        """Make sure that the dataset is downloaded.
-
-        This method is only called once per run.
+            stage: Either 'fit', 'validate', 'test', or 'predict'.
         """
-        ETCI2021(self.root_dir, checksum=False)
+        if stage in ["fit", "validate"]:
+            season_to_int = {"winter": 0, "spring": 1000, "summer": 2000, "fall": 3000}
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Initialize the main ``Dataset`` objects.
+            self.dataset = SEN12MS(split="train", **self.kwargs)
 
-        This method is called once per GPU per run.
+            # A patch is a filename like:
+            #     "ROIs{num}_{season}_s2_{scene_id}_p{patch_id}.tif"
+            # This patch will belong to the scene that is uniquely identified by its
+            # (season, scene_id) tuple. Because the largest scene_id is 149, we can
+            # simply give each season a large number and representing a unique_scene_id
+            # as (season_id + scene_id).
+            scenes = []
+            for scene_fn in self.dataset.ids:
+                parts = scene_fn.split("_")
+                season_id = season_to_int[parts[1]]
+                scene_id = int(parts[3])
+                scenes.append(season_id + scene_id)
+
+            train_indices, val_indices = next(
+                GroupShuffleSplit(test_size=0.2, n_splits=2, random_state=0).split(
+                    scenes, groups=scenes
+                )
+            )
+
+            self.train_dataset = Subset(self.dataset, train_indices)
+            self.val_dataset = Subset(self.dataset, val_indices)
+        if stage in ["test"]:
+            self.test_dataset = SEN12MS(split="test", **self.kwargs)
+
+    def on_after_batch_transfer(
+        self, batch: Dict[str, Tensor], dataloader_idx: int
+    ) -> Dict[str, Tensor]:
+        """Apply batch augmentations to the batch after it is transferred to the device.
 
         Args:
-            stage: stage to set up
-        """
-        train_val_dataset = ETCI2021(
-            self.root_dir, split="train", transforms=self.preprocess
-        )
-        self.test_dataset = ETCI2021(
-            self.root_dir, split="val", transforms=self.preprocess
-        )
-
-        size_train_val = len(train_val_dataset)
-        size_train = round(0.8 * size_train_val)
-        size_val = size_train_val - size_train
-
-        self.train_dataset, self.val_dataset = random_split(
-            train_val_dataset,
-            [size_train, size_val],
-            generator=Generator().manual_seed(self.seed),
-        )
-
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
+            batch: A batch of data that needs to be altered or augmented.
+            dataloader_idx: The index of the dataloader to which the batch belongs.
 
         Returns:
-            training data loader
+            A batch of data.
         """
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=True,
-        )
-
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+        batch["mask"] = torch.take(self.DFC2020_CLASS_MAPPING, batch["mask"])
 
-        Returns:
-            validation data loader
-        """
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
-
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
-
-        Returns:
-            testing data loader
-        """
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
-
-    def plot(self, *args: Any, **kwargs: Any) -> plt.Figure:
-        """Run :meth:`torchgeo.datasets.ETCI2021.plot`."""
-        return self.test_dataset.plot(*args, **kwargs)
+        return super().on_after_batch_transfer(batch, dataloader_idx)
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/fair1m.py` & `torchgeo-0.4.0/torchgeo/datamodules/spacenet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,99 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""FAIR1M datamodule."""
+"""SpaceNet datamodules."""
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict
 
-import pytorch_lightning as pl
-import torch
+import kornia.augmentation as K
 from torch import Tensor
-from torch.utils.data import DataLoader
 
-from ..datasets import FAIR1M
+from ..datasets import SpaceNet1
+from ..transforms import AugmentationSequential
+from .geo import NonGeoDataModule
 from .utils import dataset_split
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
 
+class SpaceNet1DataModule(NonGeoDataModule):
+    """LightningDataModule implementation for the SpaceNet1 dataset.
 
-def collate_fn(batch: List[Dict[str, Tensor]]) -> Dict[str, Any]:
-    """Custom object detection collate fn to handle variable number of boxes.
-
-    Args:
-        batch: list of sample dicts return by dataset
-    Returns:
-        batch dict output
-    """
-    output: Dict[str, Any] = {}
-    output["image"] = torch.stack([sample["image"] for sample in batch])
-    output["boxes"] = [sample["boxes"] for sample in batch]
-    return output
-
-
-class FAIR1MDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the FAIR1M dataset.
+    Randomly splits into train/val/test.
 
-    .. versionadded:: 0.2
+    .. versionadded:: 0.4
     """
 
     def __init__(
         self,
-        root_dir: str,
         batch_size: int = 64,
         num_workers: int = 0,
-        val_split_pct: float = 0.2,
+        val_split_pct: float = 0.1,
         test_split_pct: float = 0.2,
         **kwargs: Any,
     ) -> None:
-        """Initialize a LightningDataModule for FAIR1M based DataLoaders.
+        """Initialize a new SpaceNet1DataModule instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the FAIR1M Dataset classes
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
-            val_split_pct: What percentage of the dataset to use as a validation set
-            test_split_pct: What percentage of the dataset to use as a test set
+            batch_size: Size of each mini-batch.
+            num_workers: Number of workers for parallel data loading.
+            val_split_pct: Percentage of the dataset to use as a validation set.
+            test_split_pct: Percentage of the dataset to use as a test set.
+            **kwargs: Additional keyword arguments passed to
+                :class:`~torchgeo.datasets.SpaceNet1`.
         """
-        super().__init__()
-        self.root_dir = root_dir
-        self.batch_size = batch_size
-        self.num_workers = num_workers
+        super().__init__(SpaceNet1, batch_size, num_workers, **kwargs)
+
         self.val_split_pct = val_split_pct
         self.test_split_pct = test_split_pct
 
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
-
-        Args:
-            sample: input image dictionary
-
-        Returns:
-            preprocessed sample
-        """
-        sample["image"] = sample["image"].float()
-        sample["image"] /= 255.0
-        return sample
-
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Initialize the main ``Dataset`` objects.
+        self.train_aug = AugmentationSequential(
+            K.Normalize(mean=self.mean, std=self.std),
+            K.PadTo((448, 448)),
+            K.RandomRotation(p=0.5, degrees=90),
+            K.RandomHorizontalFlip(p=0.5),
+            K.RandomVerticalFlip(p=0.5),
+            K.RandomSharpness(p=0.5),
+            K.ColorJitter(
+                p=0.5,
+                brightness=0.1,
+                contrast=0.1,
+                saturation=0.1,
+                hue=0.1,
+                silence_instantiation_warning=True,
+            ),
+            data_keys=["image", "mask"],
+        )
+        self.aug = AugmentationSequential(
+            K.Normalize(mean=self.mean, std=self.std),
+            K.PadTo((448, 448)),
+            data_keys=["image", "mask"],
+        )
 
-        This method is called once per GPU per run.
+    def setup(self, stage: str) -> None:
+        """Set up datasets.
 
         Args:
-            stage: stage to set up
+            stage: Either 'fit', 'validate', 'test', or 'predict'.
         """
-        dataset = FAIR1M(self.root_dir, transforms=self.preprocess)
+        self.dataset = SpaceNet1(**self.kwargs)
         self.train_dataset, self.val_dataset, self.test_dataset = dataset_split(
-            dataset, val_pct=self.val_split_pct, test_pct=self.test_split_pct
+            self.dataset, self.val_split_pct, self.test_split_pct
         )
 
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
-
-        Returns:
-            training data loader
-        """
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=True,
-            collate_fn=collate_fn,
-        )
+    def on_after_batch_transfer(
+        self, batch: Dict[str, Tensor], dataloader_idx: int
+    ) -> Dict[str, Tensor]:
+        """Apply batch augmentations to the batch after it is transferred to the device.
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+        Args:
+            batch: A batch of data that needs to be altered or augmented.
+            dataloader_idx: The index of the dataloader to which the batch belongs.
 
         Returns:
-            validation data loader
+            A batch of data.
         """
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-            collate_fn=collate_fn,
-        )
-
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
+        # We add 1 to the mask to map the current {background, building} labels to
+        # the values {1, 2}. This is necessary because we add 0 padding to the
+        # mask that we want to ignore in the loss function.
+        batch["mask"] += 1
 
-        Returns:
-            testing data loader
-        """
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-            collate_fn=collate_fn,
-        )
+        return super().on_after_batch_transfer(batch, dataloader_idx)
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/inria.py` & `torchgeo-0.4.0/torchgeo/datasets/loveda.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,300 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""InriaAerialImageLabeling datamodule."""
+"""LoveDA dataset."""
 
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+import glob
+import os
+from typing import Callable, Dict, List, Optional
 
-import kornia.augmentation as K
-import pytorch_lightning as pl
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
-import torchvision.transforms as T
-from einops import rearrange
-from kornia.contrib import compute_padding, extract_tensor_patches
-from torch.utils.data import DataLoader, Dataset
-from torch.utils.data._utils.collate import default_collate
+from PIL import Image
+from torch import Tensor
 
-from ..datasets import InriaAerialImageLabeling
-from ..samplers.utils import _to_tuple
-from .utils import dataset_split
+from .geo import NonGeoDataset
+from .utils import download_and_extract_archive
 
 
-def collate_wrapper(batch: List[Dict[str, Any]]) -> Dict[str, Any]:
-    """Flatten wrapper."""
-    r_batch: Dict[str, Any] = default_collate(batch)  # type: ignore[no-untyped-call]
-    r_batch["image"] = torch.flatten(r_batch["image"], 0, 1)
-    if "mask" in r_batch:
-        r_batch["mask"] = torch.flatten(r_batch["mask"], 0, 1)
+class LoveDA(NonGeoDataset):
+    """LoveDA dataset.
 
-    return r_batch
+    The `LoveDA <https://github.com/Junjue-Wang/LoveDA>`__ datataset is a
+    semantic segmentation dataset.
 
+    Dataset features:
 
-class InriaAerialImageLabelingDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the InriaAerialImageLabeling dataset.
+    * 2713 urban scene and 3274 rural scene HSR images, spatial resolution of 0.3m
+    * image source is Google Earth platform
+    * total of 166768 annotated objects from Nanjing, Changzhou and Wuhan cities
+    * dataset comes with predefined train, validation, and test set
+    * dataset differentiates between 'rural' and 'urban' images
 
-    Uses the train/test splits from the dataset and further splits
-    the train split into train/val splits.
+    Dataset format:
 
-    .. versionadded:: 0.3
+    * images are three-channel pngs with dimension 1024x1024
+    * segmentation masks are single-channel pngs
+
+    Dataset classes:
+
+    1. background
+    2. building
+    3. road
+    4. water
+    5. barren
+    6. forest
+    7. agriculture
+
+    No-data regions assigned with 0 and should be ignored.
+
+    If you use this dataset in your research, please cite the following paper:
+
+    * https://arxiv.org/abs/2110.08733
+
+    .. versionadded:: 0.2
     """
 
-    h, w = 5000, 5000
+    scenes = ["urban", "rural"]
+    splits = ["train", "val", "test"]
+
+    info_dict = {
+        "train": {
+            "url": "https://zenodo.org/record/5706578/files/Train.zip?download=1",
+            "filename": "Train.zip",
+            "md5": "de2b196043ed9b4af1690b3f9a7d558f",
+        },
+        "val": {
+            "url": "https://zenodo.org/record/5706578/files/Val.zip?download=1",
+            "filename": "Val.zip",
+            "md5": "84cae2577468ff0b5386758bb386d31d",
+        },
+        "test": {
+            "url": "https://zenodo.org/record/5706578/files/Test.zip?download=1",
+            "filename": "Test.zip",
+            "md5": "a489be0090465e01fb067795d24e6b47",
+        },
+    }
+
+    classes = [
+        "background",
+        "building",
+        "road",
+        "water",
+        "barren",
+        "forest",
+        "agriculture",
+        "no-data",
+    ]
 
     def __init__(
         self,
-        root_dir: str,
-        batch_size: int = 32,
-        num_workers: int = 0,
-        val_split_pct: float = 0.1,
-        test_split_pct: float = 0.1,
-        patch_size: Union[int, Tuple[int, int]] = 512,
-        num_patches_per_tile: int = 32,
-        predict_on: str = "test",
+        root: str = "data",
+        split: str = "train",
+        scene: List[str] = ["urban", "rural"],
+        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
+        download: bool = False,
+        checksum: bool = False,
     ) -> None:
-        """Initialize a LightningDataModule for InriaAerialImageLabeling.
+        """Initialize a new LoveDA dataset instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the InriaAerialImageLabeling
-                Dataset classes
-            batch_size: The batch size used in the train DataLoader
-                (val_batch_size == test_batch_size == 1)
-            num_workers: The number of workers to use in all created DataLoaders
-            val_split_pct: What percentage of the dataset to use as a validation set
-            test_split_pct: What percentage of the dataset to use as a test set
-            patch_size: Size of random patch from image and mask (height, width)
-            num_patches_per_tile: Number of random patches per sample
-            predict_on: Directory/Dataset of images to run inference on
-        """
-        super().__init__()
-        self.root_dir = root_dir
-        self.batch_size = batch_size
-        self.num_workers = num_workers
-        self.val_split_pct = val_split_pct
-        self.test_split_pct = test_split_pct
-        self.patch_size = cast(Tuple[int, int], _to_tuple(patch_size))
-        self.num_patches_per_tile = num_patches_per_tile
-        self.augmentations = K.AugmentationSequential(
-            K.RandomHorizontalFlip(p=0.5),
-            K.RandomVerticalFlip(p=0.5),
-            data_keys=["input", "mask"],
-        )
-        self.predict_on = predict_on
-        self.random_crop = K.AugmentationSequential(
-            K.RandomCrop(self.patch_size, p=1.0, keepdim=False),
-            data_keys=["input", "mask"],
-        )
+            root: root directory where dataset can be found
+            split: one of "train", "val", or "test"
+            scene: specify whether to load only 'urban', only 'rural' or both
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
+            download: if True, download dataset and store it in the root directory
+            checksum: if True, check the MD5 of the downloaded files (may be slow)
+
+        Raises:
+            AssertionError: if ``split`` argument is invalid
+            AssertionError: if ``scene`` argument is invalid
+            RuntimeError: if ``download=False`` and data is not found, or checksums
+                don't match
+        """
+        assert split in self.splits
+        assert set(scene).intersection(
+            set(self.scenes)
+        ), "The possible scenes are 'rural' and/or 'urban'"
+        assert len(scene) <= 2, "There are no other scenes than 'rural' or 'urban'"
+
+        self.root = root
+        self.split = split
+        self.scene = scene
+        self.transforms = transforms
+        self.checksum = checksum
+
+        self.url = self.info_dict[self.split]["url"]
+        self.filename = self.info_dict[self.split]["filename"]
+        self.md5 = self.info_dict[self.split]["md5"]
+
+        self.directory = os.path.join(self.root, split.capitalize())
+        self.scene_paths = [
+            os.path.join(self.directory, s.capitalize()) for s in self.scene
+        ]
+
+        if download:
+            self._download()
+
+        if not self._check_integrity():
+            raise RuntimeError(
+                "Dataset not found at root directory or corrupted. "
+                + "You can use download=True to download it"
+            )
 
-    def patch_sample(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Extract patches from single sample."""
-        assert sample["image"].ndim == 3
-        _, h, w = sample["image"].shape
-
-        padding = compute_padding((h, w), self.patch_size)
-        sample["original_shape"] = (h, w)
-        sample["patch_shape"] = self.patch_size
-        sample["padding"] = padding
-        sample["image"] = extract_tensor_patches(
-            sample["image"].unsqueeze(0),
-            self.patch_size,
-            self.patch_size,
-            padding=padding,
-        )
-        sample["image"] = rearrange(sample["image"], "() t c h w -> t () c h w")
-        return sample
+        self.files = self._load_files(self.scene_paths, self.split)
 
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
+    def __getitem__(self, index: int) -> Dict[str, Tensor]:
+        """Return an index within the dataset.
 
         Args:
-            sample: input image dictionary
+            index: index to return
 
         Returns:
-            preprocessed sample
+            image and mask at that index with image of dimension 3x1024x1024
+            and mask of dimension 1024x1024
         """
-        sample["image"] = sample["image"].float()
-        sample["image"] /= 255.0
-        sample["image"] = torch.clip(sample["image"], min=0.0, max=1.0)
+        files = self.files[index]
+        image = self._load_image(files["image"])
+
+        if self.split != "test":
+            mask = self._load_target(files["mask"])
+            sample = {"image": image, "mask": mask}
+        else:
+            sample = {"image": image}
 
-        if "mask" in sample:
-            sample["mask"] = rearrange(sample["mask"], "h w -> () h w")
+        if self.transforms is not None:
+            sample = self.transforms(sample)
 
         return sample
 
-    def n_random_crop(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Get n random crops."""
-        images, masks = [], []
-        for _ in range(self.num_patches_per_tile):
-            image, mask = sample["image"], sample["mask"]
-            # RandomCrop needs image and mask to be in float
-            mask = mask.to(torch.float)
-            image, mask = self.random_crop(image, mask)
-            images.append(image.squeeze())
-            masks.append(mask.squeeze(0).long())
-        sample["image"] = torch.stack(images)  # (t,c,h,w)
-        sample["mask"] = torch.stack(masks)  # (t, 1, h, w)
-        return sample
+    def __len__(self) -> int:
+        """Return the number of datapoints in the dataset.
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Initialize the main ``Dataset`` objects.
+        Returns:
+            length of dataset
+        """
+        return len(self.files)
+
+    def _load_files(self, scene_paths: List[str], split: str) -> List[Dict[str, str]]:
+        """Return the paths of the files in the dataset.
 
-        This method is called once per GPU per run.
+        Args:
+            scene_paths: contains one or two paths, depending on whether user has
+                         specified only 'rural', 'only 'urban' or both
+            split: subset of dataset, one of [train, val, test]
         """
-        train_transforms = T.Compose([self.preprocess, self.n_random_crop])
-        test_transforms = T.Compose([self.preprocess, self.patch_sample])
+        images = []
 
-        train_dataset = InriaAerialImageLabeling(
-            self.root_dir, split="train", transforms=train_transforms
-        )
+        for s in scene_paths:
+            images.extend(glob.glob(os.path.join(s, "images_png", "*.png")))
+
+        images = sorted(images)
 
-        self.train_dataset: Dataset[Any]
-        self.val_dataset: Dataset[Any]
-        self.test_dataset: Dataset[Any]
-
-        if self.val_split_pct > 0.0:
-            if self.test_split_pct > 0.0:
-                self.train_dataset, self.val_dataset, self.test_dataset = dataset_split(
-                    train_dataset,
-                    val_pct=self.val_split_pct,
-                    test_pct=self.test_split_pct,
-                )
-            else:
-                self.train_dataset, self.val_dataset = dataset_split(
-                    train_dataset, val_pct=self.val_split_pct
-                )
-                self.test_dataset = self.val_dataset
+        if self.split != "test":
+            masks = [image.replace("images_png", "masks_png") for image in images]
+            files = [
+                dict(image=image, mask=mask) for image, mask, in zip(images, masks)
+            ]
         else:
-            self.train_dataset = train_dataset
-            self.val_dataset = train_dataset
-            self.test_dataset = train_dataset
-
-        assert self.predict_on == "test"
-        self.predict_dataset = InriaAerialImageLabeling(
-            self.root_dir, self.predict_on, transforms=test_transforms
-        )
+            files = [dict(image=image) for image in images]
 
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training."""
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            collate_fn=collate_wrapper,
-            shuffle=True,
-        )
+        return files
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation."""
-        return DataLoader(
-            self.val_dataset,
-            batch_size=1,
-            num_workers=self.num_workers,
-            collate_fn=collate_wrapper,
-            shuffle=False,
-        )
+    def _load_image(self, path: str) -> Tensor:
+        """Load a single image.
 
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing."""
-        return DataLoader(
-            self.test_dataset,
-            batch_size=1,
-            num_workers=self.num_workers,
-            collate_fn=collate_wrapper,
-            shuffle=False,
-        )
+        Args:
+            path: path to the image
 
-    def predict_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for prediction."""
-        return DataLoader(
-            self.predict_dataset,
-            batch_size=1,
-            num_workers=self.num_workers,
-            collate_fn=collate_wrapper,
-            shuffle=False,
+        Returns:
+            the loaded image
+        """
+        filename = os.path.join(path)
+        with Image.open(filename) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
+            tensor = torch.from_numpy(array).float()
+            # Convert from HxWxC to CxHxW
+            tensor = tensor.permute((2, 0, 1))
+            return tensor
+
+    def _load_target(self, path: str) -> Tensor:
+        """Load a single mask corresponding to image.
+
+        Args:
+            path: path to the mask
+
+        Returns:
+            the mask of the image
+        """
+        filename = os.path.join(path)
+        with Image.open(filename) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("L"))
+            tensor = torch.from_numpy(array)
+            tensor = tensor.to(torch.long)
+            return tensor
+
+    def _check_integrity(self) -> bool:
+        """Check the integrity of the dataset structure.
+
+        Returns:
+            True if the dataset directories and split files are found, else False
+        """
+        for s in self.scene_paths:
+            if not os.path.exists(s):
+                return False
+
+        return True
+
+    def _download(self) -> None:
+        """Download the dataset and extract it.
+
+        Raises:
+            AssertionError: if the checksum of split.py does not match
+        """
+        if self._check_integrity():
+            print("Files already downloaded and verified")
+            return
+
+        download_and_extract_archive(
+            self.url,
+            self.root,
+            filename=self.filename,
+            md5=self.md5 if self.checksum else None,
         )
 
-    def on_after_batch_transfer(
-        self, batch: Dict[str, Any], dataloader_idx: int
-    ) -> Dict[str, Any]:
-        """Apply augmentations to batch after transferring to GPU.
-
-        Args:
-            batch (dict): A batch of data that needs to be altered or augmented.
-            dataloader_idx (int): The index of the dataloader to which the batch
-            belongs.
-
-        Returns:
-            dict: A batch of data
-        """
-        # Training
-        if (
-            hasattr(self, "trainer")
-            and self.trainer is not None
-            and hasattr(self.trainer, "training")
-            and self.trainer.training
-            and self.augmentations is not None
-        ):
-            batch["mask"] = batch["mask"].to(torch.float)
-            batch["image"], batch["mask"] = self.augmentations(
-                batch["image"], batch["mask"]
-            )
-            batch["mask"] = batch["mask"].to(torch.long)
+    def plot(
+        self, sample: Dict[str, Tensor], suptitle: Optional[str] = None
+    ) -> plt.Figure:
+        """Plot a sample from the dataset.
+
+        Args:
+            sample: a sample return by :meth:`__getitem__`
+            suptitle: optional suptitle to use for figure
+
+        Returns:
+            a matplotlib Figure with the rendered sample
+        """
+        if self.split != "test":
+            image, mask = sample["image"], sample["mask"]
+            ncols = 2
+        else:
+            image = sample["image"]
+            ncols = 1
+
+        fig, axs = plt.subplots(nrows=1, ncols=ncols, figsize=(10, ncols * 10))
+
+        if self.split != "test":
+            axs[0].imshow(image.permute(1, 2, 0))
+            axs[0].axis("off")
+            axs[1].imshow(mask)
+            axs[1].axis("off")
+        else:
+            axs.imshow(image.permute(1, 2, 0))
+            axs.axis("off")
+
+        if suptitle is not None:
+            plt.suptitle(suptitle)
 
-        # Validation
-        if "mask" in batch:
-            batch["mask"] = rearrange(batch["mask"], "b () h w -> b h w")
-        return batch
+        return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/oscd.py` & `torchgeo-0.4.0/torchgeo/datasets/landcoverai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,270 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""OSCD datamodule."""
+"""LandCover.ai dataset."""
 
-from typing import Any, Dict, List, Optional, Tuple
+import glob
+import hashlib
+import os
+from functools import lru_cache
+from typing import Callable, Dict, Optional
 
-import kornia.augmentation as K
-import pytorch_lightning as pl
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
-from einops import repeat
-from torch.utils.data import DataLoader, Dataset
-from torch.utils.data._utils.collate import default_collate
-from torchvision.transforms import Compose, Normalize
+from matplotlib.colors import ListedColormap
+from PIL import Image
+from torch import Tensor
 
-from ..datasets import OSCD
-from .utils import dataset_split
+from .geo import NonGeoDataset
+from .utils import download_url, extract_archive, working_dir
 
 
-class OSCDDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the OSCD dataset.
+class LandCoverAI(NonGeoDataset):
+    r"""LandCover.ai dataset.
 
-    Uses the train/test splits from the dataset and further splits
-    the train split into train/val splits.
+    The `LandCover.ai <https://landcover.ai/>`__ (Land Cover from Aerial Imagery)
+    dataset is a dataset for automatic mapping of buildings, woodlands, water and
+    roads from aerial images. This implementation is specifically for Version 1 of
+    Landcover.ai.
 
-    .. versionadded:: 0.2
-    """
+    Dataset features:
 
-    band_means = torch.tensor(
-        [
-            1583.0741,
-            1374.3202,
-            1294.1616,
-            1325.6158,
-            1478.7408,
-            1933.0822,
-            2166.0608,
-            2076.4868,
-            2306.0652,
-            690.9814,
-            16.2360,
-            2080.3347,
-            1524.6930,
-        ]
-    )
+    * land cover from Poland, Central Europe
+    * three spectral bands - RGB
+    * 33 orthophotos with 25 cm per pixel resolution (~9000x9500 px)
+    * 8 orthophotos with 50 cm per pixel resolution (~4200x4700 px)
+    * total area of 216.27 km\ :sup:`2`
+
+    Dataset format:
+
+    * rasters are three-channel GeoTiffs with EPSG:2180 spatial reference system
+    * masks are single-channel GeoTiffs with EPSG:2180 spatial reference system
+
+    Dataset classes:
 
-    band_stds = torch.tensor(
+    1. building (1.85 km\ :sup:`2`\ )
+    2. woodland (72.02 km\ :sup:`2`\ )
+    3. water (13.15 km\ :sup:`2`\ )
+    4. road (3.5 km\ :sup:`2`\ )
+
+    If you use this dataset in your research, please cite the following paper:
+
+    * https://arxiv.org/abs/2005.02264v3
+
+    .. note::
+
+       This dataset requires the following additional library to be installed:
+
+       * `opencv-python <https://pypi.org/project/opencv-python/>`_ to generate
+         the train/val/test split
+    """
+
+    url = "https://landcover.ai.linuxpolska.com/download/landcover.ai.v1.zip"
+    filename = "landcover.ai.v1.zip"
+    md5 = "3268c89070e8734b4e91d531c0617e03"
+    sha256 = "15ee4ca9e3fd187957addfa8f0d74ac31bc928a966f76926e11b3c33ea76daa1"
+    classes = ["Background", "Building", "Woodland", "Water", "Road"]
+    cmap = ListedColormap(
         [
-            52.1937,
-            83.4168,
-            105.6966,
-            151.1401,
-            147.4615,
-            115.9289,
-            123.1974,
-            114.6483,
-            141.4530,
-            73.2758,
-            4.8368,
-            213.4821,
-            179.4793,
+            [0.63921569, 1.0, 0.45098039],
+            [0.61176471, 0.61176471, 0.61176471],
+            [0.14901961, 0.45098039, 0.0],
+            [0.0, 0.77254902, 1.0],
+            [0.0, 0.0, 0.0],
         ]
     )
 
     def __init__(
         self,
-        root_dir: str,
-        bands: str = "all",
-        train_batch_size: int = 32,
-        num_workers: int = 0,
-        val_split_pct: float = 0.2,
-        patch_size: Tuple[int, int] = (64, 64),
-        num_patches_per_tile: int = 32,
-        pad_size: Tuple[int, int] = (1280, 1280),
-        **kwargs: Any,
+        root: str = "data",
+        split: str = "train",
+        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
+        download: bool = False,
+        checksum: bool = False,
     ) -> None:
-        """Initialize a LightningDataModule for OSCD based DataLoaders.
+        """Initialize a new LandCover.ai dataset instance.
+
+        Args:
+            root: root directory where dataset can be found
+            split: one of "train", "val", or "test"
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
+            download: if True, download dataset and store it in the root directory
+            checksum: if True, check the MD5 of the downloaded files (may be slow)
+
+        Raises:
+            AssertionError: if ``split`` argument is invalid
+            RuntimeError: if ``download=False`` and data is not found, or checksums
+                don't match
+        """
+        assert split in ["train", "val", "test"]
+
+        self.root = root
+        self.split = split
+        self.transforms = transforms
+        self.download = download
+        self.checksum = checksum
+
+        self._verify()
+
+        with open(os.path.join(self.root, split + ".txt")) as f:
+            self.ids = f.readlines()
+
+    def __getitem__(self, index: int) -> Dict[str, Tensor]:
+        """Return an index within the dataset.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the OSCD Dataset classes
-            bands: "rgb" or "all"
-            train_batch_size: The batch size used in the train DataLoader
-                (val_batch_size == test_batch_size == 1)
-            num_workers: The number of workers to use in all created DataLoaders
-            val_split_pct: What percentage of the dataset to use as a validation set
-            patch_size: Size of random patch from image and mask (height, width)
-            num_patches_per_tile: number of random patches per sample
-            pad_size: size to pad images to during val/test steps
-        """
-        super().__init__()
-        self.root_dir = root_dir
-        self.bands = bands
-        self.train_batch_size = train_batch_size
-        self.num_workers = num_workers
-        self.val_split_pct = val_split_pct
-        self.patch_size = patch_size
-        self.num_patches_per_tile = num_patches_per_tile
-
-        if bands == "rgb":
-            self.band_means = self.band_means[[3, 2, 1]]
-            self.band_stds = self.band_stds[[3, 2, 1]]
-
-        self.rcrop = K.AugmentationSequential(
-            K.RandomCrop(patch_size), data_keys=["input", "mask"], same_on_batch=True
-        )
-        self.padto = K.PadTo(pad_size)
-
-        self.norm = Normalize(self.band_means, self.band_stds)
-
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset."""
-        sample["image"] = sample["image"].float()
-        sample["image"] = self.norm(sample["image"])
-        sample["image"] = torch.flatten(sample["image"], 0, 1)
+            index: index to return
+
+        Returns:
+            data and label at that index
+        """
+        id_ = self.ids[index].rstrip()
+        sample = {"image": self._load_image(id_), "mask": self._load_target(id_)}
+
+        if self.transforms is not None:
+            sample = self.transforms(sample)
+
         return sample
 
-    def prepare_data(self) -> None:
-        """Make sure that the dataset is downloaded.
+    def __len__(self) -> int:
+        """Return the number of data points in the dataset.
 
-        This method is only called once per run.
+        Returns:
+            length of the dataset
         """
-        OSCD(self.root_dir, split="train", bands=self.bands, checksum=False)
+        return len(self.ids)
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Initialize the main ``Dataset`` objects.
-
-        This method is called once per GPU per run.
-        """
-
-        def n_random_crop(sample: Dict[str, Any]) -> Dict[str, Any]:
-            images, masks = [], []
-            for i in range(self.num_patches_per_tile):
-                mask = repeat(sample["mask"], "h w -> t h w", t=2).float()
-                image, mask = self.rcrop(sample["image"], mask)
-                mask = mask.squeeze()[0]
-                images.append(image.squeeze())
-                masks.append(mask.long())
-            sample["image"] = torch.stack(images)
-            sample["mask"] = torch.stack(masks)
-            return sample
-
-        def pad_to(sample: Dict[str, Any]) -> Dict[str, Any]:
-            sample["image"] = self.padto(sample["image"])[0]
-            sample["mask"] = self.padto(sample["mask"].float()).long()[0, 0]
-            return sample
-
-        train_transforms = Compose([self.preprocess, n_random_crop])
-        # for testing and validation we pad all inputs to a fixed size to avoid issues
-        # with the upsampling paths in encoder-decoder architectures
-        test_transforms = Compose([self.preprocess, pad_to])
-
-        train_dataset = OSCD(
-            self.root_dir, split="train", bands=self.bands, transforms=train_transforms
-        )
-
-        self.train_dataset: Dataset[Any]
-        self.val_dataset: Dataset[Any]
-
-        if self.val_split_pct > 0.0:
-            val_dataset = OSCD(
-                self.root_dir,
-                split="train",
-                bands=self.bands,
-                transforms=test_transforms,
-            )
-            self.train_dataset, self.val_dataset, _ = dataset_split(
-                train_dataset, val_pct=self.val_split_pct, test_pct=0.0
+    @lru_cache()
+    def _load_image(self, id_: str) -> Tensor:
+        """Load a single image.
+
+        Args:
+            id_: unique ID of the image
+
+        Returns:
+            the image
+        """
+        filename = os.path.join(self.root, "output", id_ + ".jpg")
+        with Image.open(filename) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img)
+            tensor = torch.from_numpy(array).float()
+            # Convert from HxWxC to CxHxW
+            tensor = tensor.permute((2, 0, 1))
+            return tensor
+
+    @lru_cache()
+    def _load_target(self, id_: str) -> Tensor:
+        """Load the target mask for a single image.
+
+        Args:
+            id_: unique ID of the image
+
+        Returns:
+            the target mask
+        """
+        filename = os.path.join(self.root, "output", id_ + "_m.png")
+        with Image.open(filename) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("L"))
+            tensor = torch.from_numpy(array).long()
+            return tensor
+
+    def _verify(self) -> None:
+        """Verify the integrity of the dataset.
+
+        Raises:
+            RuntimeError: if ``download=False`` but dataset is missing or checksum fails
+        """
+        # Check if the extracted files already exist
+        jpg = os.path.join(self.root, "output", "*_*.jpg")
+        png = os.path.join(self.root, "output", "*_*_m.png")
+        if glob.glob(jpg) and glob.glob(png):
+            return
+
+        # Check if the zip file has already been downloaded
+        pathname = os.path.join(self.root, self.filename)
+        if os.path.exists(pathname):
+            self._extract()
+            return
+
+        # Check if the user requested to download the dataset
+        if not self.download:
+            raise RuntimeError(
+                f"Dataset not found in `root={self.root}` and `download=False`, "
+                "either specify a different `root` directory or use `download=True` "
+                "to automatically download the dataset."
             )
-            self.val_dataset.dataset = val_dataset
-        else:
-            self.train_dataset = train_dataset
-            self.val_dataset = train_dataset
-
-        self.test_dataset = OSCD(
-            self.root_dir, split="test", bands=self.bands, transforms=test_transforms
-        )
-
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training."""
-
-        def collate_wrapper(batch: List[Dict[str, Any]]) -> Dict[str, Any]:
-            r_batch: Dict[str, Any] = default_collate(  # type: ignore[no-untyped-call]
-                batch
+
+        # Download the dataset
+        self._download()
+        self._extract()
+
+    def _download(self) -> None:
+        """Download the dataset."""
+        download_url(self.url, self.root, md5=self.md5 if self.checksum else None)
+
+    def _extract(self) -> None:
+        """Extract the dataset.
+
+        Raises:
+            AssertionError: if the checksum of split.py does not match
+        """
+        extract_archive(os.path.join(self.root, self.filename))
+
+        # Generate train/val/test splits
+        # Always check the sha256 of this file before executing
+        # to avoid malicious code injection
+        with working_dir(self.root):
+            with open("split.py") as f:
+                split = f.read().encode("utf-8")
+                assert hashlib.sha256(split).hexdigest() == self.sha256
+                exec(split)
+
+    def plot(
+        self,
+        sample: Dict[str, Tensor],
+        show_titles: bool = True,
+        suptitle: Optional[str] = None,
+    ) -> plt.Figure:
+        """Plot a sample from the dataset.
+
+        Args:
+            sample: a sample returned by :meth:`__getitem__`
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional string to use as a suptitle
+
+        Returns:
+            a matplotlib Figure with the rendered sample
+
+        .. versionadded:: 0.2
+        """
+        image = np.rollaxis(sample["image"].numpy(), 0, 3)
+        mask = sample["mask"].numpy()
+
+        num_panels = 2
+        showing_predictions = "prediction" in sample
+        if showing_predictions:
+            predictions = sample["prediction"].numpy()
+            num_panels += 1
+
+        fig, axs = plt.subplots(1, num_panels, figsize=(num_panels * 4, 5))
+        axs[0].imshow(image)
+        axs[0].axis("off")
+        axs[1].imshow(mask, vmin=0, vmax=4, cmap=self.cmap, interpolation="none")
+        axs[1].axis("off")
+        if show_titles:
+            axs[0].set_title("Image")
+            axs[1].set_title("Mask")
+
+        if showing_predictions:
+            axs[2].imshow(
+                predictions, vmin=0, vmax=4, cmap=self.cmap, interpolation="none"
             )
-            r_batch["image"] = torch.flatten(r_batch["image"], 0, 1)
-            r_batch["mask"] = torch.flatten(r_batch["mask"], 0, 1)
-            return r_batch
-
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.train_batch_size,
-            num_workers=self.num_workers,
-            collate_fn=collate_wrapper,
-            shuffle=True,
-        )
-
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation."""
-        return DataLoader(
-            self.val_dataset, batch_size=1, num_workers=self.num_workers, shuffle=False
-        )
-
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing."""
-        return DataLoader(
-            self.test_dataset, batch_size=1, num_workers=self.num_workers, shuffle=False
-        )
+            axs[2].axis("off")
+            if show_titles:
+                axs[2].set_title("Predictions")
+
+        if suptitle is not None:
+            plt.suptitle(suptitle)
+        return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/sen12ms.py` & `torchgeo-0.4.0/torchgeo/datamodules/chesapeake.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,182 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""SEN12MS datamodule."""
+"""Chesapeake Bay High-Resolution Land Cover Project datamodule."""
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List
 
-import pytorch_lightning as pl
-import torch
-from sklearn.model_selection import GroupShuffleSplit
-from torch.utils.data import DataLoader, Subset
+import kornia.augmentation as K
+import torch.nn as nn
+import torch.nn.functional as F
+from einops import rearrange
+from torch import Tensor
 
-from ..datasets import SEN12MS
+from ..datasets import ChesapeakeCVPR
+from ..samplers import GridGeoSampler, RandomBatchGeoSampler
+from ..transforms import AugmentationSequential
+from .geo import GeoDataModule
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
 
+class _Transform(nn.Module):
+    """Version of AugmentationSequential designed for samples, not batches."""
 
-class SEN12MSDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the SEN12MS dataset.
-
-    Implements 80/20 geographic train/val splits and uses the test split from the
-    classification dataset definitions. See :func:`setup` for more details.
-
-    Uses the Simplified IGBP scheme defined in the 2020 Data Fusion Competition. See
-    https://arxiv.org/abs/2002.08254.
-    """
-
-    #: Mapping from the IGBP class definitions to the DFC2020, taken from the dataloader
-    #: here https://github.com/lukasliebel/dfc2020_baseline.
-    DFC2020_CLASS_MAPPING = torch.tensor(
-        [
-            0,  # maps 0s to 0
-            1,  # maps 1s to 1
-            1,  # maps 2s to 1
-            1,  # ...
-            1,
-            1,
-            2,
-            2,
-            3,
-            3,
-            4,
-            5,
-            6,
-            7,
-            6,
-            8,
-            9,
-            10,
-        ]
-    )
-
-    def __init__(
-        self,
-        root_dir: str,
-        seed: int,
-        band_set: str = "all",
-        batch_size: int = 64,
-        num_workers: int = 0,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize a LightningDataModule for SEN12MS based DataLoaders.
+    def __init__(self, aug: nn.Module) -> None:
+        """Initialize a new _Transform instance.
 
         Args:
-            root_dir: The ``root`` arugment to pass to the SEN12MS Dataset classes
-            seed: The seed value to use when doing the sklearn based ShuffleSplit
-            band_set: The subset of S1/S2 bands to use. Options are: "all",
-                "s1", "s2-all", and "s2-reduced" where the "s2-reduced" set includes:
-                B2, B3, B4, B8, B11, and B12.
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
+            aug: Augmentation to apply.
         """
         super().__init__()
-        assert band_set in SEN12MS.BAND_SETS.keys()
-
-        self.root_dir = root_dir
-        self.seed = seed
-        self.band_set = band_set
-        self.band_indices = SEN12MS.BAND_SETS[band_set]
-        self.batch_size = batch_size
-        self.num_workers = num_workers
+        self.aug = aug
 
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
+    def forward(self, sample: Dict[str, Any]) -> Dict[str, Any]:
+        """Apply the augmentation.
 
         Args:
-            sample: dictionary containing image and mask
+            sample: Input sample.
 
         Returns:
-            preprocessed sample
+            Augmented sample.
         """
-        sample["image"] = sample["image"].float()
-
-        if self.band_set == "all":
-            sample["image"][:2] = sample["image"][:2].clamp(-25, 0) / -25
-            sample["image"][2:] = sample["image"][2:].clamp(0, 10000) / 10000
-        elif self.band_set == "s1":
-            sample["image"][:2] = sample["image"][:2].clamp(-25, 0) / -25
-        else:
-            sample["image"][:] = sample["image"][:].clamp(0, 10000) / 10000
-
-        if "mask" in sample:
-            sample["mask"] = sample["mask"][0, :, :].long()
-            sample["mask"] = torch.take(self.DFC2020_CLASS_MAPPING, sample["mask"])
-
+        for key in ["image", "mask"]:
+            dtype = sample[key].dtype
+            # All inputs must be float
+            sample[key] = sample[key].float()
+            sample[key] = self.aug(sample[key])
+            sample[key] = sample[key].to(dtype)
+            # Kornia adds batch dimension
+            sample[key] = rearrange(sample[key], "() c h w -> c h w")
         return sample
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Create the train/val/test splits based on the original Dataset objects.
 
-        The splits should be done here vs. in :func:`__init__` per the docs:
-        https://pytorch-lightning.readthedocs.io/en/latest/extensions/datamodules.html#setup.
-
-        We split samples between train and val geographically with proportions of 80/20.
-        This mimics the geographic test set split.
-
-        Args:
-            stage: stage to set up
-        """
-        season_to_int = {"winter": 0, "spring": 1000, "summer": 2000, "fall": 3000}
+class ChesapeakeCVPRDataModule(GeoDataModule):
+    """LightningDataModule implementation for the Chesapeake CVPR Land Cover dataset.
 
-        self.all_train_dataset = SEN12MS(
-            self.root_dir,
-            split="train",
-            bands=self.band_indices,
-            transforms=self.preprocess,
-            checksum=False,
-        )
+    Uses the random splits defined per state to partition tiles into train, val,
+    and test sets.
+    """
 
-        self.all_test_dataset = SEN12MS(
-            self.root_dir,
-            split="test",
-            bands=self.band_indices,
-            transforms=self.preprocess,
-            checksum=False,
-        )
+    def __init__(
+        self,
+        train_splits: List[str],
+        val_splits: List[str],
+        test_splits: List[str],
+        batch_size: int = 64,
+        patch_size: int = 256,
+        length: int = 1000,
+        num_workers: int = 0,
+        class_set: int = 7,
+        use_prior_labels: bool = False,
+        prior_smoothing_constant: float = 1e-4,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize a new ChesapeakeCVPRDataModule instance.
 
-        # A patch is a filename like: "ROIs{num}_{season}_s2_{scene_id}_p{patch_id}.tif"
-        # This patch will belong to the scene that is uniquelly identified by its
-        # (season, scene_id) tuple. Because the largest scene_id is 149, we can simply
-        # give each season a large number and representing a `unique_scene_id` as
-        # `season_id + scene_id`.
-        scenes = []
-        for scene_fn in self.all_train_dataset.ids:
-            parts = scene_fn.split("_")
-            season_id = season_to_int[parts[1]]
-            scene_id = int(parts[3])
-            scenes.append(season_id + scene_id)
-
-        train_indices, val_indices = next(
-            GroupShuffleSplit(test_size=0.2, n_splits=2, random_state=self.seed).split(
-                scenes, groups=scenes
+        Args:
+            train_splits: Splits used to train the model, e.g., ["ny-train"].
+            val_splits: Splits used to validate the model, e.g., ["ny-val"].
+            test_splits: Splits used to test the model, e.g., ["ny-test"].
+            batch_size: Size of each mini-batch.
+            patch_size: Size of each patch, either ``size`` or ``(height, width)``.
+                Should be a multiple of 32 for most segmentation architectures.
+            length: Length of each training epoch.
+            num_workers: Number of workers for parallel data loading.
+            class_set: The high-resolution land cover class set to use (5 or 7).
+            use_prior_labels: Flag for using a prior over high-resolution classes
+                instead of the high-resolution labels themselves.
+            prior_smoothing_constant: Additive smoothing to add when using prior labels.
+            **kwargs: Additional keyword arguments passed to
+                :class:`~torchgeo.datasets.ChesapeakeCVPR`.
+
+        Raises:
+            ValueError: If ``use_prior_labels=True`` is used with ``class_set=7``.
+        """
+        # This is a rough estimate of how large of a patch we will need to sample in
+        # EPSG:3857 in order to guarantee a large enough patch in the local CRS.
+        self.original_patch_size = patch_size * 2
+        kwargs["transforms"] = _Transform(K.CenterCrop(patch_size))
+
+        super().__init__(
+            ChesapeakeCVPR, batch_size, patch_size, length, num_workers, **kwargs
+        )
+
+        assert class_set in [5, 7]
+        if use_prior_labels and class_set == 7:
+            raise ValueError(
+                "The pre-generated prior labels are only valid for the 5"
+                + " class set of labels"
             )
-        )
 
-        self.train_dataset = Subset(self.all_train_dataset, train_indices)
-        self.val_dataset = Subset(self.all_train_dataset, val_indices)
-        self.test_dataset = Subset(
-            self.all_test_dataset, range(len(self.all_test_dataset))
-        )
-
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
+        self.train_splits = train_splits
+        self.val_splits = val_splits
+        self.test_splits = test_splits
+        self.class_set = class_set
+        self.use_prior_labels = use_prior_labels
+        self.prior_smoothing_constant = prior_smoothing_constant
+
+        if self.use_prior_labels:
+            self.layers = [
+                "naip-new",
+                "prior_from_cooccurrences_101_31_no_osm_no_buildings",
+            ]
+        else:
+            self.layers = ["naip-new", "lc"]
 
-        Returns:
-            training data loader
-        """
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=True,
+        self.aug = AugmentationSequential(
+            K.Normalize(mean=self.mean, std=self.std), data_keys=["image", "mask"]
         )
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+    def setup(self, stage: str) -> None:
+        """Set up datasets and samplers.
 
-        Returns:
-            validation data loader
+        Args:
+            stage: Either 'fit', 'validate', 'test', or 'predict'.
         """
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+        if stage in ["fit"]:
+            self.train_dataset = ChesapeakeCVPR(
+                splits=self.train_splits, layers=self.layers, **self.kwargs
+            )
+            self.train_batch_sampler = RandomBatchGeoSampler(
+                self.train_dataset,
+                self.original_patch_size,
+                self.batch_size,
+                self.length,
+            )
+        if stage in ["fit", "validate"]:
+            self.val_dataset = ChesapeakeCVPR(
+                splits=self.val_splits, layers=self.layers, **self.kwargs
+            )
+            self.val_sampler = GridGeoSampler(
+                self.val_dataset, self.original_patch_size, self.original_patch_size
+            )
+        if stage in ["test"]:
+            self.test_dataset = ChesapeakeCVPR(
+                splits=self.test_splits, layers=self.layers, **self.kwargs
+            )
+            self.test_sampler = GridGeoSampler(
+                self.test_dataset, self.original_patch_size, self.original_patch_size
+            )
+
+    def on_after_batch_transfer(
+        self, batch: Dict[str, Tensor], dataloader_idx: int
+    ) -> Dict[str, Tensor]:
+        """Apply batch augmentations to the batch after it is transferred to the device.
 
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
+        Args:
+            batch: A batch of data that needs to be altered or augmented.
+            dataloader_idx: The index of the dataloader to which the batch belongs.
 
         Returns:
-            testing data loader
+            A batch of data.
         """
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+        if self.use_prior_labels:
+            batch["mask"] = F.normalize(batch["mask"].float(), p=1, dim=1)
+            batch["mask"] = F.normalize(
+                batch["mask"] + self.prior_smoothing_constant, p=1, dim=1
+            ).long()
+        else:
+            if self.class_set == 5:
+                batch["mask"][batch["mask"] == 5] = 4
+                batch["mask"][batch["mask"] == 6] = 4
+
+        return super().on_after_batch_transfer(batch, dataloader_idx)
```

### Comparing `torchgeo-0.3.1/torchgeo/datamodules/so2sat.py` & `torchgeo-0.4.0/torchgeo/samplers/batch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,202 +1,159 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""So2Sat datamodule."""
+"""TorchGeo batch samplers."""
 
-from typing import Any, Dict, Optional, cast
+import abc
+from typing import Iterator, List, Optional, Tuple, Union
 
-import pytorch_lightning as pl
 import torch
-from torch.utils.data import DataLoader
-from torchvision.transforms import Compose, Normalize
+from rtree.index import Index, Property
+from torch.utils.data import Sampler
 
-from ..datasets import So2Sat
+from ..datasets import BoundingBox, GeoDataset
+from .constants import Units
+from .utils import _to_tuple, get_random_bounding_box, tile_to_chips
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
 
+class BatchGeoSampler(Sampler[List[BoundingBox]], abc.ABC):
+    """Abstract base class for sampling from :class:`~torchgeo.datasets.GeoDataset`.
 
-class So2SatDataModule(pl.LightningDataModule):
-    """LightningDataModule implementation for the So2Sat dataset.
-
-    Uses the train/val/test splits from the dataset.
+    Unlike PyTorch's :class:`~torch.utils.data.BatchSampler`, :class:`BatchGeoSampler`
+    returns enough geospatial information to uniquely index any
+    :class:`~torchgeo.datasets.GeoDataset`. This includes things like latitude,
+    longitude, height, width, projection, coordinate system, and time.
     """
 
-    band_means = torch.tensor(
-        [
-            0.12375696117681859,
-            0.1092774636368323,
-            0.1010855203267882,
-            0.1142398616114001,
-            0.1592656692023089,
-            0.18147236008771792,
-            0.1745740312291377,
-            0.19501607349635292,
-            0.15428468872076637,
-            0.10905050699570007,
-        ]
-    )
-
-    band_stds = torch.tensor(
-        [
-            0.03958795985905458,
-            0.047778262752410296,
-            0.06636616706371974,
-            0.06358874912497474,
-            0.07744387147984592,
-            0.09101635085921553,
-            0.09218466562387101,
-            0.10164581233948201,
-            0.09991773043519253,
-            0.08780632509122865,
-        ]
-    )
-
-    # this reorders the bands to put S2 RGB first, then remainder of S2
-    reindex_to_rgb_first = [2, 1, 0, 3, 4, 5, 6, 7, 8, 9]
-
-    def __init__(
-        self,
-        root_dir: str,
-        batch_size: int = 64,
-        num_workers: int = 0,
-        bands: str = "rgb",
-        unsupervised_mode: bool = False,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize a LightningDataModule for So2Sat based DataLoaders.
-
-        Args:
-            root_dir: The ``root`` arugment to pass to the So2Sat Dataset classes
-            batch_size: The batch size to use in all created DataLoaders
-            num_workers: The number of workers to use in all created DataLoaders
-            bands: Either "rgb" or "s2"
-            unsupervised_mode: Makes the train dataloader return imagery from the train,
-                val, and test sets
-        """
-        super().__init__()
-        self.root_dir = root_dir
-        self.batch_size = batch_size
-        self.num_workers = num_workers
-        self.bands = bands
-        self.unsupervised_mode = unsupervised_mode
-
-        self.norm = Normalize(self.band_means, self.band_stds)
-
-    def preprocess(self, sample: Dict[str, Any]) -> Dict[str, Any]:
-        """Transform a single sample from the Dataset.
+    def __init__(self, dataset: GeoDataset, roi: Optional[BoundingBox] = None) -> None:
+        """Initialize a new Sampler instance.
 
         Args:
-            sample: dictionary containing image
+            dataset: dataset to index from
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+        """
+        if roi is None:
+            self.index = dataset.index
+            roi = BoundingBox(*self.index.bounds)
+        else:
+            self.index = Index(interleaved=False, properties=Property(dimension=3))
+            hits = dataset.index.intersection(tuple(roi), objects=True)
+            for hit in hits:
+                bbox = BoundingBox(*hit.bounds) & roi
+                self.index.insert(hit.id, tuple(bbox), hit.object)
+
+        self.res = dataset.res
+        self.roi = roi
+
+    @abc.abstractmethod
+    def __iter__(self) -> Iterator[List[BoundingBox]]:
+        """Return a batch of indices of a dataset.
 
         Returns:
-            preprocessed sample
+            batch of (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
         """
-        sample["image"] = sample["image"].float()
-        sample["image"] = self.norm(sample["image"])
-        sample["image"] = sample["image"][self.reindex_to_rgb_first, :, :]
 
-        if self.bands == "rgb":
-            sample["image"] = sample["image"][:3, :, :]
 
-        return sample
+class RandomBatchGeoSampler(BatchGeoSampler):
+    """Samples batches of elements from a region of interest randomly.
 
-    def prepare_data(self) -> None:
-        """Make sure that the dataset is downloaded.
+    This is particularly useful during training when you want to maximize the size of
+    the dataset and return as many random :term:`chips <chip>` as possible. Note that
+    randomly sampled chips may overlap.
+    """
 
-        This method is only called once per run.
-        """
-        So2Sat(self.root_dir, checksum=False)
+    def __init__(
+        self,
+        dataset: GeoDataset,
+        size: Union[Tuple[float, float], float],
+        batch_size: int,
+        length: Optional[int] = None,
+        roi: Optional[BoundingBox] = None,
+        units: Units = Units.PIXELS,
+    ) -> None:
+        """Initialize a new Sampler instance.
 
-    def setup(self, stage: Optional[str] = None) -> None:
-        """Initialize the main ``Dataset`` objects.
+        The ``size`` argument can either be:
 
-        This method is called once per GPU per run.
+        * a single ``float`` - in which case the same value is used for the height and
+          width dimension
+        * a ``tuple`` of two floats - in which case, the first *float* is used for the
+          height dimension, and the second *float* for the width dimension
 
-        Args:
-            stage: stage to set up
-        """
-        train_transforms = Compose([self.preprocess])
-        val_test_transforms = self.preprocess
+        .. versionchanged:: 0.3
+           Added ``units`` parameter, changed default to pixel units
 
-        s2bands = So2Sat.BAND_SETS["s2"]
-        if not self.unsupervised_mode:
+        .. versionchanged:: 0.4
+           ``length`` parameter is now optional, a reasonable default will be used
 
-            self.train_dataset = So2Sat(
-                self.root_dir, split="train", bands=s2bands, transforms=train_transforms
-            )
-
-            self.val_dataset = So2Sat(
-                self.root_dir,
-                split="validation",
-                bands=s2bands,
-                transforms=val_test_transforms,
-            )
-
-            self.test_dataset = So2Sat(
-                self.root_dir,
-                split="test",
-                bands=s2bands,
-                transforms=val_test_transforms,
-            )
+        Args:
+            dataset: dataset to index from
+            size: dimensions of each :term:`patch`
+            batch_size: number of samples per batch
+            length: number of samples per epoch
+                (defaults to approximately the maximal number of non-overlapping
+                :term:`chips <chip>` of size ``size`` that could be sampled from
+                the dataset)
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+            units: defines if ``size`` is in pixel or CRS units
+        """
+        super().__init__(dataset, roi)
+        self.size = _to_tuple(size)
 
-        else:
+        if units == Units.PIXELS:
+            self.size = (self.size[0] * self.res, self.size[1] * self.res)
 
-            temp_train = So2Sat(
-                self.root_dir, split="train", bands=s2bands, transforms=train_transforms
-            )
-
-            self.val_dataset = So2Sat(
-                self.root_dir,
-                split="validation",
-                bands=s2bands,
-                transforms=train_transforms,
-            )
-
-            self.test_dataset = So2Sat(
-                self.root_dir, split="test", bands=s2bands, transforms=train_transforms
-            )
-
-            self.train_dataset = cast(
-                So2Sat, temp_train + self.val_dataset + self.test_dataset
-            )
+        self.batch_size = batch_size
+        self.length = 0
+        self.hits = []
+        areas = []
+        for hit in self.index.intersection(tuple(self.roi), objects=True):
+            bounds = BoundingBox(*hit.bounds)
+            if (
+                bounds.maxx - bounds.minx >= self.size[1]
+                and bounds.maxy - bounds.miny >= self.size[0]
+            ):
+                if bounds.area > 0:
+                    rows, cols = tile_to_chips(bounds, self.size)
+                    self.length += rows * cols
+                else:
+                    self.length += 1
+                self.hits.append(hit)
+                areas.append(bounds.area)
+        if length is not None:
+            self.length = length
+
+        # torch.multinomial requires float probabilities > 0
+        self.areas = torch.tensor(areas, dtype=torch.float)
+        if torch.sum(self.areas) == 0:
+            self.areas += 1
 
-    def train_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for training.
+    def __iter__(self) -> Iterator[List[BoundingBox]]:
+        """Return the indices of a dataset.
 
         Returns:
-            training data loader
+            batch of (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
         """
-        return DataLoader(
-            self.train_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=True,
-        )
+        for _ in range(len(self)):
+            # Choose a random tile, weighted by area
+            idx = torch.multinomial(self.areas, 1)
+            hit = self.hits[idx]
+            bounds = BoundingBox(*hit.bounds)
 
-    def val_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for validation.
+            # Choose random indices within that tile
+            batch = []
+            for _ in range(self.batch_size):
 
-        Returns:
-            validation data loader
-        """
-        return DataLoader(
-            self.val_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+                bounding_box = get_random_bounding_box(bounds, self.size, self.res)
+                batch.append(bounding_box)
+
+            yield batch
 
-    def test_dataloader(self) -> DataLoader[Any]:
-        """Return a DataLoader for testing.
+    def __len__(self) -> int:
+        """Return the number of batches in a single epoch.
 
         Returns:
-            testing data loader
+            number of batches in an epoch
         """
-        return DataLoader(
-            self.test_dataset,
-            batch_size=self.batch_size,
-            num_workers=self.num_workers,
-            shuffle=False,
-        )
+        return self.length // self.batch_size
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/__init__.py` & `torchgeo-0.4.0/torchgeo/datasets/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,19 @@
     ChesapeakeDE,
     ChesapeakeMD,
     ChesapeakeNY,
     ChesapeakePA,
     ChesapeakeVA,
     ChesapeakeWV,
 )
+from .cloud_cover import CloudCoverDetection
 from .cms_mangrove_canopy import CMSGlobalMangroveCanopy
 from .cowc import COWC, COWCCounting, COWCDetection
 from .cv4a_kenya_crop_type import CV4AKenyaCropType
-from .cyclone import TropicalCycloneWindEstimation
+from .cyclone import TropicalCyclone
 from .deepglobelandcover import DeepGlobeLandCover
 from .dfc2022 import DFC2022
 from .eddmaps import EDDMapS
 from .enviroatlas import EnviroAtlas
 from .esri2020 import Esri2020
 from .etci2021 import ETCI2021
 from .eudem import EUDEM
@@ -42,16 +43,14 @@
     GeoDataset,
     IntersectionDataset,
     NonGeoClassificationDataset,
     NonGeoDataset,
     RasterDataset,
     UnionDataset,
     VectorDataset,
-    VisionClassificationDataset,
-    VisionDataset,
 )
 from .gid15 import GID15
 from .globbiomass import GlobBiomass
 from .idtrees import IDTReeS
 from .inaturalist import INaturalist
 from .inria import InriaAerialImageLabeling
 from .landcoverai import LandCoverAI
@@ -69,44 +68,45 @@
     Landsat9,
 )
 from .levircd import LEVIRCDPlus
 from .loveda import LoveDA
 from .millionaid import MillionAID
 from .naip import NAIP
 from .nasa_marine_debris import NASAMarineDebris
-from .nwpu import VHR10
 from .openbuildings import OpenBuildings
 from .oscd import OSCD
 from .patternnet import PatternNet
 from .potsdam import Potsdam2D
 from .reforestree import ReforesTree
 from .resisc45 import RESISC45
 from .seco import SeasonalContrastS2
 from .sen12ms import SEN12MS
-from .sentinel import Sentinel, Sentinel2
+from .sentinel import Sentinel, Sentinel1, Sentinel2
 from .so2sat import So2Sat
 from .spacenet import (
     SpaceNet,
     SpaceNet1,
     SpaceNet2,
     SpaceNet3,
     SpaceNet4,
     SpaceNet5,
+    SpaceNet6,
     SpaceNet7,
 )
 from .ucmerced import UCMerced
 from .usavars import USAVars
 from .utils import (
     BoundingBox,
     concat_samples,
     merge_samples,
     stack_samples,
     unbind_samples,
 )
 from .vaihingen import Vaihingen2D
+from .vhr10 import VHR10
 from .xview import XView2
 from .zuericrop import ZueriCrop
 
 __all__ = (
     # GeoDataset
     "AbovegroundLiveWoodyBiomassDensity",
     "AsterGDEM",
@@ -140,19 +140,21 @@
     "Landsat5TM",
     "Landsat7",
     "Landsat8",
     "Landsat9",
     "NAIP",
     "OpenBuildings",
     "Sentinel",
+    "Sentinel1",
     "Sentinel2",
     # NonGeoDataset
     "ADVANCE",
     "BeninSmallHolderCashews",
     "BigEarthNet",
+    "CloudCoverDetection",
     "COWC",
     "COWCCounting",
     "COWCDetection",
     "CV4AKenyaCropType",
     "DeepGlobeLandCover",
     "DFC2022",
     "EnviroAtlas",
@@ -178,36 +180,31 @@
     "So2Sat",
     "SpaceNet",
     "SpaceNet1",
     "SpaceNet2",
     "SpaceNet3",
     "SpaceNet4",
     "SpaceNet5",
+    "SpaceNet6",
     "SpaceNet7",
-    "TropicalCycloneWindEstimation",
+    "TropicalCyclone",
     "UCMerced",
     "USAVars",
     "Vaihingen2D",
     "VHR10",
     "XView2",
     "ZueriCrop",
     # Base classes
     "GeoDataset",
     "IntersectionDataset",
     "NonGeoClassificationDataset",
     "NonGeoDataset",
     "RasterDataset",
     "UnionDataset",
     "VectorDataset",
-    "VisionClassificationDataset",
-    "VisionDataset",
     # Utilities
     "BoundingBox",
     "concat_samples",
     "merge_samples",
     "stack_samples",
     "unbind_samples",
 )
-
-# https://stackoverflow.com/questions/40018681
-for module in __all__:
-    globals()[module].__module__ = "torchgeo.datasets"
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/advance.py` & `torchgeo-0.4.0/torchgeo/datasets/advance.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/agb_live_woody_density.py` & `torchgeo-0.4.0/torchgeo/datasets/agb_live_woody_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             FileNotFoundError: if no files are found in ``root``
         """
         self.root = root
         self.download = download
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if dataset is missing
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/astergdem.py` & `torchgeo-0.4.0/torchgeo/datasets/astergdem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""Aster Global Digital Evaluation Model dataset."""
+"""Aster Global Digital Elevation Model dataset."""
 
 import glob
 import os
 from typing import Any, Callable, Dict, Optional
 
 import matplotlib.pyplot as plt
 from rasterio.crs import CRS
 
 from .geo import RasterDataset
 
 
 class AsterGDEM(RasterDataset):
-    """Aster Global Digital Evaluation Model Dataset.
+    """Aster Global Digital Elevation Model Dataset.
 
-    The `Aster Global Digital Evaluation Model
+    The `Aster Global Digital Elevation Model
     <https://lpdaac.usgs.gov/products/astgtmv003/>`_
     dataset is a Digital Elevation Model (DEM) on a global scale.
     The dataset can be downloaded from the
     `Earth Data website <https://search.earthdata.nasa.gov/search/>`_
     after making an account.
 
     Dataset features:
@@ -69,15 +69,15 @@
             FileNotFoundError: if no files are found in ``root``
             RuntimeError: if dataset is missing
         """
         self.root = root
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if dataset is missing
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/benin_cashews.py` & `torchgeo-0.4.0/torchgeo/datasets/benin_cashews.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,30 +133,30 @@
         "2020_10_10",
         "2020_10_15",
         "2020_10_20",
         "2020_10_25",
         "2020_10_30",
     )
 
-    ALL_BANDS = (
+    all_bands = (
         "B01",
         "B02",
         "B03",
         "B04",
         "B05",
         "B06",
         "B07",
         "B08",
         "B8A",
         "B09",
         "B11",
         "B12",
         "CLD",
     )
-    RGB_BANDS = ("B04", "B03", "B02")
+    rgb_bands = ("B04", "B03", "B02")
 
     classes = [
         "No data",
         "Well-managed planatation",
         "Poorly-managed planatation",
         "Non-planatation",
         "Residential",
@@ -169,15 +169,15 @@
     tile_width = 1122
 
     def __init__(
         self,
         root: str = "data",
         chip_size: int = 256,
         stride: int = 128,
-        bands: Tuple[str, ...] = ALL_BANDS,
+        bands: Tuple[str, ...] = all_bands,
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
         verbose: bool = False,
     ) -> None:
         """Initialize a new Benin Smallholder Cashew Plantations Dataset instance.
@@ -274,20 +274,20 @@
 
         Raises:
             AssertionError: if ``bands`` is not a tuple
             ValueError: if an invalid band name is provided
         """
         assert isinstance(bands, tuple), "The list of bands must be a tuple"
         for band in bands:
-            if band not in self.ALL_BANDS:
+            if band not in self.all_bands:
                 raise ValueError(f"'{band}' is an invalid band name.")
 
     @lru_cache(maxsize=128)
     def _load_all_imagery(
-        self, bands: Tuple[str, ...] = ALL_BANDS
+        self, bands: Tuple[str, ...] = all_bands
     ) -> Tuple[Tensor, rasterio.Affine, CRS]:
         """Load all the imagery (across time) for the dataset.
 
         Optionally allows for subsetting of the bands that are loaded.
 
         Args:
             bands: tuple of bands to load
@@ -443,15 +443,15 @@
 
         Raises:
             ValueError: if the RGB bands are not included in ``self.bands``
 
         .. versionadded:: 0.2
         """
         rgb_indices = []
-        for band in self.RGB_BANDS:
+        for band in self.rgb_bands:
             if band in self.bands:
                 rgb_indices.append(self.bands.index(band))
             else:
                 raise ValueError("Dataset doesn't contain some of the RGB bands")
 
         num_time_points = sample["image"].shape[0]
         assert time_step < num_time_points
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/bigearthnet.py` & `torchgeo-0.4.0/torchgeo/datasets/bigearthnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
                     indexes=1,
                     out_shape=self.image_size,
                     out_dtype="int32",
                     resampling=Resampling.bilinear,
                 )
                 images.append(array)
         arrays: "np.typing.NDArray[np.int_]" = np.stack(images, axis=0)
-        tensor = torch.from_numpy(arrays)
+        tensor = torch.from_numpy(arrays).float()
         return tensor
 
     def _load_target(self, index: int) -> Tensor:
         """Load the target mask for a single image.
 
         Args:
             index: index to return
@@ -535,17 +535,14 @@
             sample: a sample returned by :meth:`__getitem__`
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
 
-        Raises:
-            ValueError: if ``self.bands`` is "s1"
-
         .. versionadded:: 0.2
         """
         if self.bands == "s2":
             image = np.rollaxis(sample["image"][[3, 2, 1]].numpy(), 0, 3)
             image = np.clip(image / 2000, 0, 1)
         elif self.bands == "all":
             image = np.rollaxis(sample["image"][[5, 4, 3]].numpy(), 0, 3)
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cbf.py` & `torchgeo-0.4.0/torchgeo/datasets/cbf.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cdl.py` & `torchgeo-0.4.0/torchgeo/datasets/cdl.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         """
         self.root = root
         self.download = download
         self.checksum = checksum
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/chesapeake.py` & `torchgeo-0.4.0/torchgeo/datasets/chesapeake.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # Licensed under the MIT License.
 
 """Chesapeake Bay High-Resolution Land Cover Project datasets."""
 
 import abc
 import os
 import sys
-from typing import Any, Callable, Dict, Optional, Sequence
+from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
 import fiona
 import matplotlib.pyplot as plt
 import numpy as np
 import pyproj
 import rasterio
 import rasterio.mask
 import shapely.geometry
 import shapely.ops
 import torch
 from matplotlib.colors import ListedColormap
 from rasterio.crs import CRS
+from torch import Tensor
 
 from .geo import GeoDataset, RasterDataset
 from .utils import BoundingBox, download_url, extract_archive
 
 
 class Chesapeake(RasterDataset, abc.ABC):
     """Abstract base class for all Chesapeake datasets.
@@ -134,15 +135,15 @@
                     self.cmap[i][0] / 255.0,
                     self.cmap[i][1] / 255.0,
                     self.cmap[i][2] / 255.0,
                 )
             )
         self._cmap = ListedColormap(colors)
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
@@ -434,14 +435,54 @@
         "base": "1225ccbb9590e9396875f221e5031514",
         "prior_extension": "402f41d07823c8faf7ea6960d7c4e17a",
     }
 
     crs = CRS.from_epsg(3857)
     res = 1
 
+    lc_cmap = {
+        0: (0, 0, 0, 0),
+        1: (0, 197, 255, 255),
+        2: (38, 115, 0, 255),
+        3: (163, 255, 115, 255),
+        4: (255, 170, 0, 255),
+        5: (156, 156, 156, 255),
+        6: (0, 0, 0, 255),
+        15: (0, 0, 0, 0),
+    }
+
+    nlcd_cmap = {
+        0: (0, 0, 0, 0),
+        11: (70, 107, 159, 255),
+        12: (209, 222, 248, 255),
+        21: (222, 197, 197, 255),
+        22: (217, 146, 130, 255),
+        23: (235, 0, 0, 255),
+        24: (171, 0, 0, 255),
+        31: (179, 172, 159, 255),
+        41: (104, 171, 95, 255),
+        42: (28, 95, 44, 255),
+        43: (181, 197, 143, 255),
+        52: (204, 184, 121, 255),
+        71: (223, 223, 194, 255),
+        81: (220, 217, 57, 255),
+        82: (171, 108, 40, 255),
+        90: (184, 217, 235, 255),
+        95: (108, 159, 184, 255),
+    }
+
+    prior_color_matrix = np.array(
+        [
+            [0.0, 0.77254902, 1.0, 1.0],
+            [0.14901961, 0.45098039, 0.0, 1.0],
+            [0.63921569, 1.0, 0.45098039, 1.0],
+            [0.61176471, 0.61176471, 0.61176471, 1.0],
+        ]
+    )
+
     valid_layers = [
         "naip-new",
         "naip-old",
         "landsat-leaf-on",
         "landsat-leaf-off",
         "nlcd",
         "lc",
@@ -536,14 +577,24 @@
         self.download = download
         self.checksum = checksum
 
         self._verify()
 
         super().__init__(transforms)
 
+        lc_colors = np.zeros((max(self.lc_cmap.keys()) + 1, 4))
+        lc_colors[list(self.lc_cmap.keys())] = list(self.lc_cmap.values())
+        lc_colors = lc_colors[:, :3] / 255
+        self._lc_cmap = ListedColormap(lc_colors)
+
+        nlcd_colors = np.zeros((max(self.nlcd_cmap.keys()) + 1, 4))
+        nlcd_colors[list(self.nlcd_cmap.keys())] = list(self.nlcd_cmap.values())
+        nlcd_colors = nlcd_colors[:, :3] / 255
+        self._nlcd_cmap = ListedColormap(nlcd_colors)
+
         # Add all tiles into the index in epsg:3857 based on the included geojson
         mint: float = 0
         maxt: float = sys.maxsize
         with fiona.open(os.path.join(root, "spatial_index.geojson"), "r") as f:
             for i, row in enumerate(f):
                 if row["properties"]["split"] in splits:
                     box = shapely.geometry.shape(row["geometry"])
@@ -579,15 +630,15 @@
         Returns:
             sample of image/mask and metadata at that index
 
         Raises:
             IndexError: if query is not found in the index
         """
         hits = self.index.intersection(tuple(query), objects=True)
-        filepaths = [hit.object for hit in hits]
+        filepaths = cast(List[Dict[str, str]], [hit.object for hit in hits])
 
         sample = {"image": [], "mask": [], "crs": self.crs, "bbox": query}
 
         if len(filepaths) == 0:
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
@@ -633,16 +684,16 @@
                     sample["mask"].append(data)
         else:
             raise IndexError(f"query: {query} spans multiple tiles which is not valid")
 
         sample["image"] = np.concatenate(sample["image"], axis=0)
         sample["mask"] = np.concatenate(sample["mask"], axis=0)
 
-        sample["image"] = torch.from_numpy(sample["image"])
-        sample["mask"] = torch.from_numpy(sample["mask"])
+        sample["image"] = torch.from_numpy(sample["image"]).float()
+        sample["mask"] = torch.from_numpy(sample["mask"]).long()
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def _verify(self) -> None:
@@ -690,7 +741,96 @@
                 md5=self.md5s[subdataset],
             )
 
     def _extract(self) -> None:
         """Extract the dataset."""
         for subdataset in self.subdatasets:
             extract_archive(os.path.join(self.root, self.filenames[subdataset]))
+
+    def plot(
+        self,
+        sample: Dict[str, Tensor],
+        show_titles: bool = True,
+        suptitle: Optional[str] = None,
+    ) -> plt.Figure:
+        """Plot a sample from the dataset.
+
+        Args:
+            sample: a sample returned by :meth:`__getitem__`
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional string to use as a suptitle
+
+        Returns:
+            a matplotlib Figure with the rendered sample
+
+        .. versionadded:: 0.4
+        """
+        image = np.rollaxis(sample["image"].numpy(), 0, 3)
+        mask = sample["mask"].numpy()
+        if mask.ndim == 3:
+            mask = np.rollaxis(mask, 0, 3)
+        else:
+            mask = np.expand_dims(mask, 2)
+
+        num_panels = len(self.layers)
+        showing_predictions = "prediction" in sample
+        if showing_predictions:
+            predictions = sample["prediction"].numpy()
+            num_panels += 1
+
+        fig, axs = plt.subplots(1, num_panels, figsize=(num_panels * 4, 5))
+
+        i = 0
+        for layer in self.layers:
+            if layer == "naip-new" or layer == "naip-old":
+                img = image[:, :, :3] / 255
+                image = image[:, :, 4:]
+                axs[i].axis("off")
+                axs[i].imshow(img)
+            elif layer == "landsat-leaf-on" or layer == "landsat-leaf-off":
+                img = image[:, :, [3, 2, 1]] / 3000
+                image = image[:, :, 9:]
+                axs[i].axis("off")
+                axs[i].imshow(img)
+            elif layer == "nlcd":
+                img = mask[:, :, 0]
+                mask = mask[:, :, 1:]
+                axs[i].imshow(
+                    img, vmin=0, vmax=95, cmap=self._nlcd_cmap, interpolation="none"
+                )
+                axs[i].axis("off")
+            elif layer == "lc":
+                img = mask[:, :, 0]
+                mask = mask[:, :, 1:]
+                axs[i].imshow(
+                    img, vmin=0, vmax=15, cmap=self._lc_cmap, interpolation="none"
+                )
+                axs[i].axis("off")
+            elif layer == "buildings":
+                img = mask[:, :, 0]
+                mask = mask[:, :, 1:]
+                axs[i].imshow(img, vmin=0, vmax=1, cmap="gray", interpolation="none")
+                axs[i].axis("off")
+            elif layer == "prior_from_cooccurrences_101_31_no_osm_no_buildings":
+                img = (mask[:, :, :4] @ self.prior_color_matrix) / 255
+                mask = mask[:, :, 4:]
+                axs[i].imshow(img)
+                axs[i].axis("off")
+
+            if show_titles:
+                if layer == "prior_from_cooccurrences_101_31_no_osm_no_buildings":
+                    axs[i].set_title("prior")
+                else:
+                    axs[i].set_title(layer)
+            i += 1
+
+        if showing_predictions:
+            axs[i].imshow(
+                predictions, vmin=0, vmax=15, cmap=self._lc_cmap, interpolation="none"
+            )
+            axs[i].axis("off")
+            if show_titles:
+                axs[i].set_title("Predictions")
+
+        if suptitle is not None:
+            plt.suptitle(suptitle)
+        return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cms_mangrove_canopy.py` & `torchgeo-0.4.0/torchgeo/datasets/cms_mangrove_canopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         )
         self.measurement = measurement
 
         self.filename_glob = f"**/Mangrove_{self.measurement}_{self.country}*"
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if dataset is missing or checksum fails
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cowc.py` & `torchgeo-0.4.0/torchgeo/datasets/cowc.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,30 +143,30 @@
 
         Returns:
             the image
         """
         filename = os.path.join(self.root, self.images[index])
         with Image.open(filename) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img)
-            tensor = torch.from_numpy(array)
+            tensor = torch.from_numpy(array).float()
             # Convert from HxWxC to CxHxW
             tensor = tensor.permute((2, 0, 1))
             return tensor
 
     def _load_target(self, index: int) -> Tensor:
         """Load a single target.
 
         Args:
             index: index to return
 
         Returns:
             the target
         """
         target = int(self.targets[index])
-        tensor = torch.tensor(target)
+        tensor = torch.tensor(target).float()
         return tensor
 
     def _check_integrity(self) -> bool:
         """Check integrity of dataset.
 
         Returns:
             True if dataset files are found and/or MD5s match, else False
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cv4a_kenya_crop_type.py` & `torchgeo-0.4.0/torchgeo/datasets/cv4a_kenya_crop_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         "B8A",
         "B09",
         "B11",
         "B12",
         "CLD",
     )
 
-    RGB_BANDS = ["B04", "B03", "B02"]
+    rgb_bands = ["B04", "B03", "B02"]
 
     # Same for all tiles
     tile_height = 3035
     tile_width = 2016
 
     def __init__(
         self,
@@ -418,15 +418,15 @@
 
         Returns:
             a matplotlib Figure with the rendered sample
 
         .. versionadded:: 0.2
         """
         rgb_indices = []
-        for band in self.RGB_BANDS:
+        for band in self.rgb_bands:
             if band in self.bands:
                 rgb_indices.append(self.bands.index(band))
             else:
                 raise ValueError("Dataset doesn't contain some of the RGB bands")
 
         if "prediction" in sample:
             prediction = sample["prediction"]
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/cyclone.py` & `torchgeo-0.4.0/torchgeo/datasets/cyclone.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 # Licensed under the MIT License.
 
 """Tropical Cyclone Wind Estimation Competition dataset."""
 
 import json
 import os
 from functools import lru_cache
-from typing import Any, Callable, Dict, Optional, cast
+from typing import Any, Callable, Dict, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 from torch import Tensor
 
 from .geo import NonGeoDataset
 from .utils import check_integrity, download_radiant_mlhub_dataset, extract_archive
 
 
-class TropicalCycloneWindEstimation(NonGeoDataset):
+class TropicalCyclone(NonGeoDataset):
     """Tropical Cyclone Wind Estimation Competition dataset.
 
     A collection of tropical storms in the Atlantic and East Pacific Oceans from 2000 to
     2019 with corresponding maximum sustained surface wind speed. This dataset is split
     into training and test categories for the purpose of a competition.
 
     See https://www.drivendata.org/competitions/72/predict-wind-speeds/ for more
@@ -34,14 +34,18 @@
 
     .. note::
 
        This dataset requires the following additional library to be installed:
 
        * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
          imagery and labels from the Radiant Earth MLHub
+
+    .. versionchanged:: 0.4
+       Class name changed from TropicalCycloneWindEstimation to TropicalCyclone
+       to be consistent with TropicalCycloneDataModule.
     """
 
     collection_id = "nasa_tropical_storm_competition"
     md5s = {
         "train": {
             "source": "97e913667a398704ea8d28196d91dad6",
             "labels": "97d02608b74c82ffe7496a9404a30413",
@@ -145,18 +149,16 @@
             if img.height != self.size or img.width != self.size:
                 # Moved in PIL 9.1.0
                 try:
                     resample = Image.Resampling.BILINEAR
                 except AttributeError:
                     resample = Image.BILINEAR
                 img = img.resize(size=(self.size, self.size), resample=resample)
-            array: "np.typing.NDArray[np.int_]" = np.array(img)
-            if len(array.shape) == 3:
-                array = array[:, :, 0]
-            tensor = torch.from_numpy(array)
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
+            tensor = torch.from_numpy(array).permute((2, 0, 1)).float()
             return tensor
 
     def _load_features(self, directory: str) -> Dict[str, Any]:
         """Load features for a single image.
 
         Args:
             directory: directory containing image
@@ -170,15 +172,15 @@
 
         filename = os.path.join(directory.format("labels"), "labels.json")
         with open(filename) as f:
             features.update(json.load(f))
 
         features["relative_time"] = int(features["relative_time"])
         features["ocean"] = int(features["ocean"])
-        features["label"] = int(features["wind_speed"])
+        features["label"] = torch.tensor(int(features["wind_speed"])).float()
 
         return features
 
     def _check_integrity(self) -> bool:
         """Check integrity of dataset.
 
         Returns:
@@ -222,33 +224,33 @@
         """Plot a sample from the dataset.
 
         Args:
             sample: a sample return by :meth:`__getitem__`
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional suptitle to use for figure
 
-        Returns;
+        Returns:
             a matplotlib Figure with the rendered sample
 
         .. versionadded:: 0.2
         """
         image, label = sample["image"], sample["label"]
 
         showing_predictions = "prediction" in sample
         if showing_predictions:
             prediction = sample["prediction"].item()
 
         fig, ax = plt.subplots(1, 1, figsize=(10, 10))
 
-        ax.imshow(image, cmap="gray")
+        ax.imshow(image.permute(1, 2, 0))
         ax.axis("off")
 
         if show_titles:
             title = f"Label: {label}"
             if showing_predictions:
-                title += f"\nPrediction: {cast(str, prediction)}"
+                title += f"\nPrediction: {prediction}"
             ax.set_title(title)
 
         if suptitle is not None:
             plt.suptitle(suptitle)
 
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/deepglobelandcover.py` & `torchgeo-0.4.0/torchgeo/datasets/deepglobelandcover.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         """
         path = self.image_fns[index]
 
         with Image.open(path) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img)
             tensor = torch.from_numpy(array)
             # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
+            tensor = tensor.permute((2, 0, 1)).to(torch.float32)
             return tensor
 
     def _load_target(self, index: int) -> Tensor:
         """Load the target mask for a single image.
 
         Args:
             index: index to return
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/dfc2022.py` & `torchgeo-0.4.0/torchgeo/datasets/dfc2022.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/eddmaps.py` & `torchgeo-0.4.0/torchgeo/datasets/eddmaps.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/enviroatlas.py` & `torchgeo-0.4.0/torchgeo/datasets/enviroatlas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 """EnviroAtlas High-Resolution Land Cover datasets."""
 
 import os
 import sys
-from typing import Any, Callable, Dict, Optional, Sequence
+from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
 import fiona
 import matplotlib.pyplot as plt
 import numpy as np
 import pyproj
 import rasterio
 import rasterio.mask
@@ -339,15 +339,15 @@
         Returns:
             sample of image/mask and metadata at that index
 
         Raises:
             IndexError: if query is not found in the index
         """
         hits = self.index.intersection(tuple(query), objects=True)
-        filepaths = [hit.object for hit in hits]
+        filepaths = cast(List[Dict[str, str]], [hit.object for hit in hits])
 
         sample = {"image": [], "mask": [], "crs": self.crs, "bbox": query}
 
         if len(filepaths) == 0:
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/esri2020.py` & `torchgeo-0.4.0/torchgeo/datasets/esri2020.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         """
         self.root = root
         self.download = download
         self.checksum = checksum
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/etci2021.py` & `torchgeo-0.4.0/torchgeo/datasets/etci2021.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,23 +167,25 @@
         """
         files = []
         directory = self.metadata[split]["directory"]
         folders = sorted(glob.glob(os.path.join(root, directory, "*")))
         folders = [os.path.join(folder, "tiles") for folder in folders]
         for folder in folders:
             vvs = sorted(glob.glob(os.path.join(folder, "vv", "*.png")))
-            vhs = sorted(glob.glob(os.path.join(folder, "vh", "*.png")))
-            water_masks = sorted(
-                glob.glob(os.path.join(folder, "water_body_label", "*.png"))
-            )
+            vhs = [vv.replace("vv", "vh") for vv in vvs]
+            water_masks = [
+                vv.replace("_vv.png", ".png").replace("vv", "water_body_label")
+                for vv in vvs
+            ]
 
             if split != "test":
-                flood_masks = sorted(
-                    glob.glob(os.path.join(folder, "flood_label", "*.png"))
-                )
+                flood_masks = [
+                    vv.replace("_vv.png", ".png").replace("vv", "flood_label")
+                    for vv in vvs
+                ]
 
                 for vv, vh, flood_mask, water_mask in zip(
                     vvs, vhs, flood_masks, water_masks
                 ):
                     files.append(
                         dict(vv=vv, vh=vh, flood_mask=flood_mask, water_mask=water_mask)
                     )
@@ -201,15 +203,15 @@
 
         Returns:
             the image
         """
         filename = os.path.join(path)
         with Image.open(filename) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
-            tensor = torch.from_numpy(array)
+            tensor = torch.from_numpy(array).float()
             # Convert from HxWxC to CxHxW
             tensor = tensor.permute((2, 0, 1))
             return tensor
 
     def _load_target(self, path: str) -> Tensor:
         """Load the target mask for a single image.
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/eudem.py` & `torchgeo-0.4.0/torchgeo/datasets/eudem.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             FileNotFoundError: if no files are found in ``root``
         """
         self.root = root
         self.checksum = checksum
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if dataset is missing or checksum fails
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/eurosat.py` & `torchgeo-0.4.0/torchgeo/datasets/eurosat.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,17 @@
         "B08A",
         "B09",
         "B10",
         "B11",
         "B12",
     )
 
-    RGB_BANDS = ("B04", "B03", "B02")
+    rgb_bands = ("B04", "B03", "B02")
 
-    BAND_SETS = {"all": all_band_names, "rgb": RGB_BANDS}
+    BAND_SETS = {"all": all_band_names, "rgb": rgb_bands}
 
     def __init__(
         self,
         root: str = "data",
         split: str = "train",
         bands: Sequence[str] = BAND_SETS["all"],
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
@@ -166,15 +166,15 @@
         Args:
             index: index to return
         Returns:
             data and label at that index
         """
         image, label = self._load_image(index)
 
-        image = torch.index_select(image, dim=0, index=self.band_indices)
+        image = torch.index_select(image, dim=0, index=self.band_indices).float()
         sample = {"image": image, "label": label}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
@@ -273,15 +273,15 @@
 
         Raises:
             ValueError: if RGB bands are not found in dataset
 
         .. versionadded:: 0.2
         """
         rgb_indices = []
-        for band in self.RGB_BANDS:
+        for band in self.rgb_bands:
             if band in self.bands:
                 rgb_indices.append(self.bands.index(band))
             else:
                 raise ValueError("Dataset doesn't contain some of the RGB bands")
 
         image = np.take(sample["image"].numpy(), indices=rgb_indices, axis=0)
         image = np.rollaxis(image, 0, 3)
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/fair1m.py` & `torchgeo-0.4.0/torchgeo/datasets/fair1m.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/forestdamage.py` & `torchgeo-0.4.0/torchgeo/datasets/xview.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,332 +1,274 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""Forest Damage dataset."""
+"""xView2 dataset."""
 
 import glob
 import os
-from typing import Any, Callable, Dict, List, Optional, Tuple
-from xml.etree import ElementTree
+from typing import Callable, Dict, List, Optional
 
-import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 from torch import Tensor
 
 from .geo import NonGeoDataset
-from .utils import check_integrity, download_and_extract_archive, extract_archive
+from .utils import check_integrity, draw_semantic_segmentation_masks, extract_archive
 
 
-def parse_pascal_voc(path: str) -> Dict[str, Any]:
-    """Read a PASCAL VOC annotation file.
+class XView2(NonGeoDataset):
+    """xView2 dataset.
 
-    Args:
-        path: path to xml file
-
-    Returns:
-        dict of image filename, points, and class labels
-    """
-    et = ElementTree.parse(path)
-    element = et.getroot()
-    filename = element.find("filename").text  # type: ignore[union-attr]
-    labels, bboxes = [], []
-    for obj in element.findall("object"):
-        bndbox = obj.find("bndbox")
-        bbox = [
-            int(bndbox.find("xmin").text),  # type: ignore[union-attr, arg-type]
-            int(bndbox.find("ymin").text),  # type: ignore[union-attr, arg-type]
-            int(bndbox.find("xmax").text),  # type: ignore[union-attr, arg-type]
-            int(bndbox.find("ymax").text),  # type: ignore[union-attr, arg-type]
-        ]
-
-        label_var = obj.find("damage")
-        if label_var is not None:
-            label = label_var.text
-        else:
-            label = "other"
-        bboxes.append(bbox)
-        labels.append(label)
-    return dict(filename=filename, bboxes=bboxes, labels=labels)
-
-
-class ForestDamage(NonGeoDataset):
-    """Forest Damage dataset.
-
-    The `ForestDamage
-    <https://lila.science/datasets/forest-damages-larch-casebearer/>`_
-    dataset contains drone imagery that can be used for tree identification,
-    as well as tree damage classification for larch trees.
-
-    Dataset features:
-
-    * 1543 images
-    * 101,878 tree annotations
-    * subset of 840 images contain 44,522 annotations about tree health
-      (Healthy (H), Light Damage (LD), High Damage (HD)), all other
-      images have "other" as damage level
+    The `xView2 <https://xview2.org/>`__
+    dataset is a dataset for building disaster change detection. This dataset object
+    uses the "Challenge training set (~7.8 GB)" and "Challenge test set (~2.6 GB)" data
+    from the xView2 website as the train and test splits. Note, the xView2 website
+    contains other data under the xView2 umbrella that are _not_ included here. E.g.
+    the "Tier3 training data", the "Challenge holdout set", and the "full data".
 
     Dataset format:
 
-    * images are three-channel jpgs
-    * annotations are in `Pascal VOC XML format
-      <https://roboflow.com/formats/pascal-voc-xml#w-tabs-0-data-w-pane-3>`_
-
-    Dataset Classes:
+    * images are three-channel pngs
+    * masks are single-channel pngs where the pixel values represent the class
 
-    0. other
-    1. healthy
-    2. light damage
-    3. high damage
+    Dataset classes:
 
-    If the download fails or stalls, it is recommended to try azcopy
-    as suggested `here <https://lila.science/faq>`__. It is expected that the
-    downloaded data file with name ``Data_Set_Larch_Casebearer``
-    can be found in ``root``.
+    0. background
+    1. no damage
+    2. minor damage
+    3. major damage
+    4. destroyed
 
-    If you use this dataset in your research, please use the following citation:
+    If you use this dataset in your research, please cite the following paper:
 
-    * Swedish Forest Agency (2021): Forest Damages - Larch Casebearer 1.0.
-      National Forest Data Lab. Dataset.
+    * https://arxiv.org/abs/1911.09296
 
-    .. versionadded:: 0.3
+    .. versionadded:: 0.2
     """
 
-    classes = ["other", "H", "LD", "HD"]
-    url = (
-        "https://lilablobssc.blob.core.windows.net/larch-casebearer/"
-        "Data_Set_Larch_Casebearer.zip"
-    )
-    data_dir = "Data_Set_Larch_Casebearer"
-    md5 = "907815bcc739bff89496fac8f8ce63d7"
+    metadata = {
+        "train": {
+            "filename": "train_images_labels_targets.tar.gz",
+            "md5": "a20ebbfb7eb3452785b63ad02ffd1e16",
+            "directory": "train",
+        },
+        "test": {
+            "filename": "test_images_labels_targets.tar.gz",
+            "md5": "1b39c47e05d1319c17cc8763cee6fe0c",
+            "directory": "test",
+        },
+    }
+    classes = ["background", "no-damage", "minor-damage", "major-damage", "destroyed"]
+    colormap = ["green", "blue", "orange", "red"]
 
     def __init__(
         self,
         root: str = "data",
+        split: str = "train",
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
-        download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new ForestDamage dataset instance.
+        """Initialize a new xView2 dataset instance.
 
         Args:
             root: root directory where dataset can be found
+            split: one of "train" or "test"
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
-            download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
-
-        Raises:
-            RuntimeError: if ``download=False`` and data is not found, or checksums
-                don't match
         """
+        assert split in self.metadata
         self.root = root
+        self.split = split
         self.transforms = transforms
         self.checksum = checksum
-        self.download = download
 
         self._verify()
 
-        self.files = self._load_files(self.root)
-
-        self.class_to_idx: Dict[str, int] = {c: i for i, c in enumerate(self.classes)}
+        self.class2idx = {c: i for i, c in enumerate(self.classes)}
+        self.files = self._load_files(root, split)
 
     def __getitem__(self, index: int) -> Dict[str, Tensor]:
         """Return an index within the dataset.
 
         Args:
             index: index to return
 
         Returns:
             data and label at that index
         """
         files = self.files[index]
-        parsed = parse_pascal_voc(files["annotation"])
-        image = self._load_image(files["image"])
-
-        boxes, labels = self._load_target(parsed["bboxes"], parsed["labels"])
-
-        sample = {"image": image, "boxes": boxes, "label": labels}
+        image1 = self._load_image(files["image1"])
+        image2 = self._load_image(files["image2"])
+        mask1 = self._load_target(files["mask1"])
+        mask2 = self._load_target(files["mask2"])
+
+        image = torch.stack(tensors=[image1, image2], dim=0)
+        mask = torch.stack(tensors=[mask1, mask2], dim=0)
+        sample = {"image": image, "mask": mask}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
 
         Returns:
             length of the dataset
         """
         return len(self.files)
 
-    def _load_files(self, root: str) -> List[Dict[str, str]]:
+    def _load_files(self, root: str, split: str) -> List[Dict[str, str]]:
         """Return the paths of the files in the dataset.
 
         Args:
             root: root dir of dataset
+            split: subset of dataset, one of [train, test]
 
         Returns:
-            list of dicts containing paths for each pair of image, annotation
+            list of dicts containing paths for each pair of images and masks
         """
-        images = sorted(
-            glob.glob(os.path.join(root, self.data_dir, "**", "Images", "*.JPG"))
-        )
-        annotations = sorted(
-            glob.glob(os.path.join(root, self.data_dir, "**", "Annotations", "*.xml"))
-        )
-
-        files = [
-            dict(image=image, annotation=annotation)
-            for image, annotation in zip(images, annotations)
-        ]
-
+        files = []
+        directory = self.metadata[split]["directory"]
+        image_root = os.path.join(root, directory, "images")
+        mask_root = os.path.join(root, directory, "targets")
+        images = glob.glob(os.path.join(image_root, "*.png"))
+        basenames = [os.path.basename(f) for f in images]
+        basenames = ["_".join(f.split("_")[:-2]) for f in basenames]
+        for name in set(basenames):
+            image1 = os.path.join(image_root, f"{name}_pre_disaster.png")
+            image2 = os.path.join(image_root, f"{name}_post_disaster.png")
+            mask1 = os.path.join(mask_root, f"{name}_pre_disaster_target.png")
+            mask2 = os.path.join(mask_root, f"{name}_post_disaster_target.png")
+            files.append(dict(image1=image1, image2=image2, mask1=mask1, mask2=mask2))
         return files
 
     def _load_image(self, path: str) -> Tensor:
         """Load a single image.
 
         Args:
             path: path to the image
 
         Returns:
             the image
         """
-        with Image.open(path) as img:
+        filename = os.path.join(path)
+        with Image.open(filename) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
-            tensor: Tensor = torch.from_numpy(array)
+            tensor = torch.from_numpy(array)
             # Convert from HxWxC to CxHxW
             tensor = tensor.permute((2, 0, 1))
             return tensor
 
-    def _load_target(
-        self, bboxes: List[List[int]], labels_list: List[str]
-    ) -> Tuple[Tensor, Tensor]:
+    def _load_target(self, path: str) -> Tensor:
         """Load the target mask for a single image.
 
         Args:
-            bboxes: list of bbox coordinats [xmin, ymin, xmax, ymax]
-            labels_list: list of class labels
+            path: path to the image
 
         Returns:
-            the target bounding boxes and labels
+            the target mask
         """
-        labels = torch.tensor([self.class_to_idx[label] for label in labels_list])
-        boxes = torch.tensor(bboxes).to(torch.float)
-        return boxes, labels
+        filename = os.path.join(path)
+        with Image.open(filename) as img:
+            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("L"))
+            tensor = torch.from_numpy(array)
+            tensor = tensor.to(torch.long)
+            return tensor
 
     def _verify(self) -> None:
-        """Checks the integrity of the dataset structure.
+        """Verify the integrity of the dataset.
 
-        Returns:
-            True if the dataset directories are found, else False
+        Raises:
+            RuntimeError: if checksum fails or the dataset is not downloaded
         """
-        filepath = os.path.join(self.root, self.data_dir)
-        if os.path.isdir(filepath):
-            return
+        # Check if the files already exist
+        exists = []
+        for split_info in self.metadata.values():
+            for directory in ["images", "targets"]:
+                exists.append(
+                    os.path.exists(
+                        os.path.join(self.root, split_info["directory"], directory)
+                    )
+                )
 
-        filepath = os.path.join(self.root, self.data_dir + ".zip")
-        if os.path.isfile(filepath):
-            if self.checksum and not check_integrity(filepath, self.md5):
-                raise RuntimeError("Dataset found, but corrupted.")
-            extract_archive(filepath)
+        if all(exists):
             return
 
-        # Check if the user requested to download the dataset
-        if not self.download:
-            raise RuntimeError(
-                "Dataset not found in `root` directory, either specify a different"
-                + " `root` directory or manually download "
-                + "the dataset to this directory."
-            )
-
-        # else download the dataset
-        self._download()
+        # Check if .tar.gz files already exists (if so then extract)
+        exists = []
+        for split_info in self.metadata.values():
+            filepath = os.path.join(self.root, split_info["filename"])
+            if os.path.isfile(filepath):
+                if self.checksum and not check_integrity(filepath, split_info["md5"]):
+                    raise RuntimeError("Dataset found, but corrupted.")
+                exists.append(True)
+                extract_archive(filepath)
+            else:
+                exists.append(False)
 
-    def _download(self) -> None:
-        """Download the dataset and extract it.
+        if all(exists):
+            return
 
-        Raises:
-            AssertionError: if the checksum does not match
-        """
-        download_and_extract_archive(
-            self.url,
-            self.root,
-            filename=self.data_dir + ".zip",
-            md5=self.md5 if self.checksum else None,
+        # Check if the user requested to download the dataset
+        raise RuntimeError(
+            "Dataset not found in `root` directory, either specify a different"
+            + " `root` directory or manually download the dataset to this directory."
         )
 
     def plot(
         self,
         sample: Dict[str, Tensor],
         show_titles: bool = True,
         suptitle: Optional[str] = None,
+        alpha: float = 0.5,
     ) -> plt.Figure:
         """Plot a sample from the dataset.
 
         Args:
             sample: a sample returned by :meth:`__getitem__`
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional string to use as a suptitle
+            alpha: opacity with which to render predictions on top of the imagery
 
         Returns:
             a matplotlib Figure with the rendered sample
         """
-        image = sample["image"].permute((1, 2, 0)).numpy()
-
-        ncols = 1
-        showing_predictions = "prediction_boxes" in sample
-        if showing_predictions:
+        ncols = 2
+        image1 = draw_semantic_segmentation_masks(
+            sample["image"][0], sample["mask"][0], alpha=alpha, colors=self.colormap
+        )
+        image2 = draw_semantic_segmentation_masks(
+            sample["image"][1], sample["mask"][1], alpha=alpha, colors=self.colormap
+        )
+        if "prediction" in sample:  # NOTE: this assumes predictions are made for post
             ncols += 1
+            image3 = draw_semantic_segmentation_masks(
+                sample["image"][1],
+                sample["prediction"],
+                alpha=alpha,
+                colors=self.colormap,
+            )
 
         fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
-        if not showing_predictions:
-            axs = [axs]
-
-        axs[0].imshow(image)
+        axs[0].imshow(image1)
         axs[0].axis("off")
-
-        bboxes = [
-            patches.Rectangle(
-                (bbox[0], bbox[1]),
-                bbox[2] - bbox[0],
-                bbox[3] - bbox[1],
-                linewidth=1,
-                edgecolor="r",
-                facecolor="none",
-            )
-            for bbox in sample["boxes"].numpy()
-        ]
-        for bbox in bboxes:
-            axs[0].add_patch(bbox)
+        axs[1].imshow(image2)
+        axs[1].axis("off")
+        if ncols > 2:
+            axs[2].imshow(image3)
+            axs[2].axis("off")
 
         if show_titles:
-            axs[0].set_title("Ground Truth")
-
-        if showing_predictions:
-            axs[1].imshow(image)
-            axs[1].axis("off")
-
-            pred_bboxes = [
-                patches.Rectangle(
-                    (bbox[0], bbox[1]),
-                    bbox[2] - bbox[0],
-                    bbox[3] - bbox[1],
-                    linewidth=1,
-                    edgecolor="r",
-                    facecolor="none",
-                )
-                for bbox in sample["prediction_boxes"].numpy()
-            ]
-            for bbox in pred_bboxes:
-                axs[1].add_patch(bbox)
-
-            if show_titles:
-                axs[1].set_title("Predictions")
+            axs[0].set_title("Pre disaster")
+            axs[1].set_title("Post disaster")
+            if ncols > 2:
+                axs[2].set_title("Predictions")
 
         if suptitle is not None:
             plt.suptitle(suptitle)
 
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/gbif.py` & `torchgeo-0.4.0/torchgeo/datasets/gbif.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 
     `GBIF <https://www.gbif.org/>`__, the Global Biodiversity Information Facility,
     is an international network and data infrastructure funded by the world's
     governments and aimed at providing anyone, anywhere, open access to data about
     all types of life on Earth.
 
     This dataset is intended for use with GBIF's
-    `occurrence records <https://www.gbif.org/dataset/search>`_. It may or may not work
-    for other GBIF `datasets <https://www.gbif.org/dataset/search>`_. Data for a
+    `occurrence records <https://www.gbif.org/occurrence/search>`_. It may or may not
+    work for other GBIF `datasets <https://www.gbif.org/dataset/search>`_. Data for a
     particular species or region of interest can be downloaded from the above link.
 
     If you use a GBIF dataset in your research, please cite it according to:
 
     * https://www.gbif.org/citation-guidelines
 
     .. note::
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/geo.py` & `torchgeo-0.4.0/torchgeo/datasets/geo.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import abc
 import functools
 import glob
 import os
 import re
 import sys
-import warnings
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, cast
 
 import fiona
 import fiona.transform
 import numpy as np
 import pyproj
 import rasterio
@@ -28,19 +27,14 @@
 from torch import Tensor
 from torch.utils.data import Dataset
 from torchvision.datasets import ImageFolder
 from torchvision.datasets.folder import default_loader as pil_loader
 
 from .utils import BoundingBox, concat_samples, disambiguate_timestamp, merge_samples
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Dataset.__module__ = "torch.utils.data"
-ImageFolder.__module__ = "torchvision.datasets"
-
 
 class GeoDataset(Dataset[Dict[str, Any]], abc.ABC):
     """Abstract base class for datasets containing geospatial information.
 
     Geospatial information includes things like:
 
     * coordinates (latitude, longitude)
@@ -176,18 +170,15 @@
     size: {len(self)}"""
 
     # NOTE: This hack should be removed once the following issue is fixed:
     # https://github.com/Toblerity/rtree/issues/87
 
     def __getstate__(
         self,
-    ) -> Tuple[
-        Dict[Any, Any],
-        List[Tuple[int, Tuple[float, float, float, float, float, float], str]],
-    ]:
+    ) -> Tuple[Dict[str, Any], List[Tuple[Any, Any, Optional[Any]]]]:
         """Define how instances are pickled.
 
         Returns:
             the state necessary to unpickle the instance
         """
         objects = self.index.intersection(self.index.bounds, objects=True)
         tuples = [(item.id, item.bounds, item.object) for item in objects]
@@ -274,16 +265,16 @@
     #: Regular expression used to extract date from filename.
     #:
     #: The expression should use named groups. The expression may contain any number of
     #: groups. The following groups are specifically searched for by the base class:
     #:
     #: * ``date``: used to calculate ``mint`` and ``maxt`` for ``index`` insertion
     #:
-    #: When :attr:`separate_files`` is True, the following additional groups are
-    #: searched for to find other files:
+    #: When :attr:`~RasterDataset.separate_files` is True, the following additional
+    #: groups are searched for to find other files:
     #:
     #: * ``band``: replaced with requested band name
     filename_regex = ".*"
 
     #: Date format string used to parse date from filename.
     #:
     #: Not used if :attr:`filename_regex` does not contain a ``date`` group.
@@ -302,28 +293,30 @@
     rgb_bands: List[str] = []
 
     #: Color map for the dataset, used for plotting
     cmap: Dict[int, Tuple[int, int, int, int]] = {}
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         crs: Optional[CRS] = None,
         res: Optional[float] = None,
+        bands: Optional[Sequence[str]] = None,
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         cache: bool = True,
     ) -> None:
         """Initialize a new Dataset instance.
 
         Args:
             root: root directory where dataset can be found
             crs: :term:`coordinate reference system (CRS)` to warp to
                 (defaults to the CRS of the first file found)
             res: resolution of the dataset in units of CRS
                 (defaults to the resolution of the first file found)
+            bands: bands to return (defaults to all bands)
             transforms: a function/transform that takes an input sample
                 and returns a transformed version
             cache: if True, cache file handle to speed up repeated sampling
 
         Raises:
             FileNotFoundError: if no files are found in ``root``
         """
@@ -370,14 +363,29 @@
                     i += 1
 
         if i == 0:
             raise FileNotFoundError(
                 f"No {self.__class__.__name__} data was found in '{root}'"
             )
 
+        if bands and self.all_bands:
+            band_indexes = [self.all_bands.index(i) + 1 for i in bands]
+            self.bands = bands
+            assert len(band_indexes) == len(self.bands)
+        elif bands:
+            msg = (
+                f"{self.__class__.__name__} is missing an `all_bands` attribute,"
+                " so `bands` cannot be specified."
+            )
+            raise AssertionError(msg)
+        else:
+            band_indexes = None
+            self.bands = self.all_bands
+
+        self.band_indexes = band_indexes
         self._crs = cast(CRS, crs)
         self.res = cast(float, res)
 
     def __getitem__(self, query: BoundingBox) -> Dict[str, Any]:
         """Retrieve image/mask and metadata indexed by query.
 
         Args:
@@ -386,25 +394,25 @@
         Returns:
             sample of image/mask and metadata at that index
 
         Raises:
             IndexError: if query is not found in the index
         """
         hits = self.index.intersection(tuple(query), objects=True)
-        filepaths = [hit.object for hit in hits]
+        filepaths = cast(List[str], [hit.object for hit in hits])
 
         if not filepaths:
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
 
         if self.separate_files:
             data_list: List[Tensor] = []
             filename_regex = re.compile(self.filename_regex, re.VERBOSE)
-            for band in getattr(self, "bands", self.all_bands):
+            for band in self.bands:
                 band_filepaths = []
                 for filepath in filepaths:
                     filename = os.path.basename(filepath)
                     directory = os.path.dirname(filepath)
                     match = re.match(filename_regex, filename)
                     if match:
                         if "date" in match.groupdict():
@@ -412,50 +420,64 @@
                             end = match.end("band")
                             filename = filename[:start] + band + filename[end:]
                     filepath = glob.glob(os.path.join(directory, filename))[0]
                     band_filepaths.append(filepath)
                 data_list.append(self._merge_files(band_filepaths, query))
             data = torch.cat(data_list)
         else:
-            data = self._merge_files(filepaths, query)
+            data = self._merge_files(filepaths, query, self.band_indexes)
 
-        key = "image" if self.is_image else "mask"
-        sample = {key: data, "crs": self.crs, "bbox": query}
+        sample = {"crs": self.crs, "bbox": query}
+        if self.is_image:
+            sample["image"] = data.float()
+        else:
+            sample["mask"] = data.long()
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
-    def _merge_files(self, filepaths: Sequence[str], query: BoundingBox) -> Tensor:
+    def _merge_files(
+        self,
+        filepaths: Sequence[str],
+        query: BoundingBox,
+        band_indexes: Optional[Sequence[int]] = None,
+    ) -> Tensor:
         """Load and merge one or more files.
 
         Args:
             filepaths: one or more files to load and merge
             query: (minx, maxx, miny, maxy, mint, maxt) coordinates to index
+            band_indexes: indexes of bands to be used
 
         Returns:
             image/mask at that index
         """
         if self.cache:
             vrt_fhs = [self._cached_load_warp_file(fp) for fp in filepaths]
         else:
             vrt_fhs = [self._load_warp_file(fp) for fp in filepaths]
 
         bounds = (query.minx, query.miny, query.maxx, query.maxy)
         if len(vrt_fhs) == 1:
             src = vrt_fhs[0]
             out_width = round((query.maxx - query.minx) / self.res)
             out_height = round((query.maxy - query.miny) / self.res)
-            out_shape = (src.count, out_height, out_width)
+            count = len(band_indexes) if band_indexes else src.count
+            out_shape = (count, out_height, out_width)
             dest = src.read(
-                out_shape=out_shape, window=from_bounds(*bounds, src.transform)
+                indexes=band_indexes,
+                out_shape=out_shape,
+                window=from_bounds(*bounds, src.transform),
             )
         else:
-            dest, _ = rasterio.merge.merge(vrt_fhs, bounds, self.res)
+            dest, _ = rasterio.merge.merge(
+                vrt_fhs, bounds, self.res, indexes=band_indexes
+            )
 
         # fix numpy dtypes which are not supported by pytorch tensors
         if dest.dtype == np.uint16:
             dest = dest.astype(np.int32)
         elif dest.dtype == np.uint32:
             dest = dest.astype(np.int64)
 
@@ -506,32 +528,39 @@
 
     def __init__(
         self,
         root: str = "data",
         crs: Optional[CRS] = None,
         res: float = 0.0001,
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
+        label_name: Optional[str] = None,
     ) -> None:
         """Initialize a new Dataset instance.
 
         Args:
             root: root directory where dataset can be found
             crs: :term:`coordinate reference system (CRS)` to warp to
                 (defaults to the CRS of the first file found)
             res: resolution of the dataset in units of CRS
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
+            label_name: name of the dataset property that has the label to be
+                rasterized into the mask
 
         Raises:
             FileNotFoundError: if no files are found in ``root``
+
+        .. versionadded:: 0.4
+            The *label_name* parameter.
         """
         super().__init__(transforms)
 
         self.root = root
         self.res = res
+        self.label_name = label_name
 
         # Populate the dataset index
         i = 0
         pathname = os.path.join(root, "**", self.filename_glob)
         for filepath in glob.iglob(pathname, recursive=True):
             try:
                 with fiona.open(filepath) as src:
@@ -592,14 +621,16 @@
 
                 # Filter geometries to those that intersect with the bounding box
                 for feature in src.filter(bbox=(minx, miny, maxx, maxy)):
                     # Warp geometries to requested CRS
                     shape = fiona.transform.transform_geom(
                         src.crs, self.crs.to_dict(), feature["geometry"]
                     )
+                    if self.label_name:
+                        shape = (shape, feature["properties"][self.label_name])
                     shapes.append(shape)
 
         # Rasterize geometries
         width = (query.maxx - query.minx) / self.res
         height = (query.maxy - query.miny) / self.res
         transform = rasterio.transform.from_bounds(
             query.minx, query.miny, query.maxx, query.maxy, width, height
@@ -657,38 +688,24 @@
         """
         return f"""\
 {self.__class__.__name__} Dataset
     type: NonGeoDataset
     size: {len(self)}"""
 
 
-class VisionDataset(NonGeoDataset):
-    """Abstract base class for datasets lacking geospatial information.
-
-    .. deprecated:: 0.3
-       Use :class:`NonGeoDataset` instead.
-    """
-
-    def __new__(cls, *args: Any, **kwargs: Any) -> "VisionDataset":
-        """Create a new instance of VisionDataset."""
-        msg = "VisionDataset is deprecated, use NonGeoDataset instead."
-        warnings.warn(msg, DeprecationWarning)
-        return super().__new__(cls, *args, **kwargs)
-
-
 class NonGeoClassificationDataset(NonGeoDataset, ImageFolder):  # type: ignore[misc]
     """Abstract base class for classification datasets lacking geospatial information.
 
     This base class is designed for datasets with pre-defined image chips which
     are separated into separate folders per class.
     """
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         loader: Optional[Callable[[str], Any]] = pil_loader,
         is_valid_file: Optional[Callable[[str], bool]] = None,
     ) -> None:
         """Initialize a new NonGeoClassificationDataset instance.
 
         Args:
@@ -744,36 +761,21 @@
             index: index to return
         Returns:
             the image
             the image class label
         """
         img, label = ImageFolder.__getitem__(self, index)
         array: "np.typing.NDArray[np.int_]" = np.array(img)
-        tensor = torch.from_numpy(array)
+        tensor = torch.from_numpy(array).float()
         # Convert from HxWxC to CxHxW
         tensor = tensor.permute((2, 0, 1))
         label = torch.tensor(label)
         return tensor, label
 
 
-class VisionClassificationDataset(NonGeoClassificationDataset):
-    """Abstract base class for classification datasets lacking geospatial information.
-
-    .. deprecated:: 0.3
-       Use :class:`NonGeoClassificationDataset` instead.
-    """
-
-    def __new__(cls, *args: Any, **kwargs: Any) -> "VisionClassificationDataset":
-        """Create a new instance of VisionClassificationDataset."""
-        msg = "VisionClassificationDataset is deprecated, "
-        msg += "use NonGeoClassificationDataset instead."
-        warnings.warn(msg, DeprecationWarning)
-        return cast(VisionClassificationDataset, super().__new__(cls))
-
-
 class IntersectionDataset(GeoDataset):
     """Dataset representing the intersection of two GeoDatasets.
 
     This allows users to do things like:
 
     * Combine image and target labels and sample from both simultaneously
       (e.g. Landsat and CDL)
@@ -793,26 +795,32 @@
     def __init__(
         self,
         dataset1: GeoDataset,
         dataset2: GeoDataset,
         collate_fn: Callable[
             [Sequence[Dict[str, Any]]], Dict[str, Any]
         ] = concat_samples,
+        transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
     ) -> None:
         """Initialize a new Dataset instance.
 
         Args:
             dataset1: the first dataset
             dataset2: the second dataset
             collate_fn: function used to collate samples
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
 
         Raises:
             ValueError: if either dataset is not a :class:`GeoDataset`
+
+        .. versionadded:: 0.4
+            The *transforms* parameter.
         """
-        super().__init__()
+        super().__init__(transforms)
         self.datasets = [dataset1, dataset2]
         self.collate_fn = collate_fn
 
         for ds in self.datasets:
             if not isinstance(ds, GeoDataset):
                 raise ValueError("IntersectionDataset only supports GeoDatasets")
 
@@ -863,15 +871,20 @@
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
 
         # All datasets are guaranteed to have a valid query
         samples = [ds[query] for ds in self.datasets]
 
-        return self.collate_fn(samples)
+        sample = self.collate_fn(samples)
+
+        if self.transforms is not None:
+            sample = self.transforms(sample)
+
+        return sample
 
     def __str__(self) -> str:
         """Return the informal string representation of the object.
 
         Returns:
             informal string representation
         """
@@ -905,26 +918,32 @@
     def __init__(
         self,
         dataset1: GeoDataset,
         dataset2: GeoDataset,
         collate_fn: Callable[
             [Sequence[Dict[str, Any]]], Dict[str, Any]
         ] = merge_samples,
+        transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
     ) -> None:
         """Initialize a new Dataset instance.
 
         Args:
             dataset1: the first dataset
             dataset2: the second dataset
             collate_fn: function used to collate samples
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
 
         Raises:
             ValueError: if either dataset is not a :class:`GeoDataset`
+
+        .. versionadded:: 0.4
+            The *transforms* parameter.
         """
-        super().__init__()
+        super().__init__(transforms)
         self.datasets = [dataset1, dataset2]
         self.collate_fn = collate_fn
 
         for ds in self.datasets:
             if not isinstance(ds, GeoDataset):
                 raise ValueError("UnionDataset only supports GeoDatasets")
 
@@ -973,18 +992,23 @@
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
 
         # Not all datasets are guaranteed to have a valid query
         samples = []
         for ds in self.datasets:
-            if ds.index.intersection(tuple(query)):
+            if list(ds.index.intersection(tuple(query))):
                 samples.append(ds[query])
 
-        return self.collate_fn(samples)
+        sample = self.collate_fn(samples)
+
+        if self.transforms is not None:
+            sample = self.transforms(sample)
+
+        return sample
 
     def __str__(self) -> str:
         """Return the informal string representation of the object.
 
         Returns:
             informal string representation
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/gid15.py` & `torchgeo-0.4.0/torchgeo/datasets/gid15.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             the image
         """
         filename = os.path.join(path)
         with Image.open(filename) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
             tensor = torch.from_numpy(array)
             # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
+            tensor = tensor.permute((2, 0, 1)).float()
             return tensor
 
     def _load_target(self, path: str) -> Tensor:
         """Load the target mask for a single image.
 
         Args:
             path: path to the image
@@ -246,15 +246,15 @@
     ) -> plt.Figure:
         """Plot a sample from the dataset.
 
         Args:
             sample: a sample return by :meth:`__getitem__`
             suptitle: optional suptitle to use for figure
 
-        Returns;
+        Returns:
             a matplotlib Figure with the rendered sample
 
         .. versionadded:: 0.2
         """
         if self.split != "test":
             image, mask = sample["image"], sample["mask"]
             ncols = 2
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/globbiomass.py` & `torchgeo-0.4.0/torchgeo/datasets/globbiomass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 """GlobBiomass dataset."""
 
 import glob
 import os
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, List, Optional, cast
 
 import matplotlib.pyplot as plt
 import torch
 from rasterio.crs import CRS
 
 from .geo import RasterDataset
 from .utils import BoundingBox, check_integrity, extract_archive
@@ -156,15 +156,15 @@
         self.measurement = measurement
 
         self.filename_glob = f"*0_{self.measurement}*.tif"
         self.zipfile_glob = f"*0_{self.measurement}.zip"
 
         self._verify()
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, transforms=transforms, cache=cache)
 
     def __getitem__(self, query: BoundingBox) -> Dict[str, Any]:
         """Retrieve image/mask and metadata indexed by query.
 
         Args:
             query: (minx, maxx, miny, maxy, mint, maxt) coordinates to index
 
@@ -172,15 +172,15 @@
             sample at index consisting of measurement mask with 2 channels,
             where the first is the measurement and the second the error map
 
         Raises:
             IndexError: if query is not found in the index
         """
         hits = self.index.intersection(tuple(query), objects=True)
-        filepaths = [hit.object for hit in hits]
+        filepaths = cast(List[str], [hit.object for hit in hits])
 
         if not filepaths:
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
 
         measurement_paths = [f for f in filepaths if "err" not in f]
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/idtrees.py` & `torchgeo-0.4.0/torchgeo/datasets/idtrees.py`

 * *Files 5% similar despite different names*

```diff
@@ -562,56 +562,47 @@
                 axs[3].set_title("Predictions")
 
         if suptitle is not None:
             plt.suptitle(suptitle)
 
         return fig
 
-    def plot_las(self, index: int, colormap: Optional[str] = None) -> Any:
+    def plot_las(
+        self, index: int
+    ) -> "pyvista.Plotter":  # type: ignore[name-defined] # noqa: F821
         """Plot a sample point cloud at the index.
 
         Args:
             index: index to plot
-            colormap: a valid matplotlib colormap
 
         Returns:
-            a open3d.visualizer.Visualizer object. Use
-                Visualizer.run() to display
+            pyvista.PolyData object. Run pyvista.plot(point_cloud, ...) to display
 
         Raises:
-            ImportError: if open3d is not installed
+            ImportError: if pyvista is not installed
+
+        .. versionchanged:: 0.4
+           Ported from Open3D to PyVista, *colormap* parameter removed.
         """
         try:
-            import open3d  # noqa: F401
+            import pyvista  # noqa: F401
         except ImportError:
             raise ImportError(
-                "open3d is not installed and is required to plot point clouds"
+                "pyvista is not installed and is required to plot point clouds"
             )
         import laspy
 
         path = self.images[index]
         path = path.replace("RGB", "LAS").replace(".tif", ".las")
         las = laspy.read(path)
         points: "np.typing.NDArray[np.int_]" = np.stack(
             [las.x, las.y, las.z], axis=0
         ).transpose((1, 0))
+        point_cloud = pyvista.PolyData(points)  # type: ignore[attr-defined]
+
+        # Some point cloud files have no color->points mapping
+        if hasattr(las, "red"):
+            colors = np.stack([las.red, las.green, las.blue], axis=0)
+            colors = colors.transpose((1, 0)) / np.iinfo(np.uint16).max
+            point_cloud["colors"] = colors
 
-        if colormap:
-            cm = plt.cm.get_cmap(colormap)
-            norm = plt.Normalize()
-            colors = cm(norm(points[:, 2]))[:, :3]
-        else:
-            # Some point cloud files have no color->points mapping
-            if hasattr(las, "red"):
-                colors = np.stack([las.red, las.green, las.blue], axis=0)
-                colors = colors.transpose((1, 0)) / 65535
-            # Default to no colormap if no colors exist in las file
-            else:
-                colors = np.zeros_like(points)
-
-        pcd = open3d.geometry.PointCloud()
-        pcd.points = open3d.utility.Vector3dVector(points)
-        pcd.colors = open3d.utility.Vector3dVector(colors)
-        vis = open3d.visualization.Visualizer()
-        vis.create_window()
-        vis.add_geometry(pcd)
-        return vis
+        return point_cloud
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/inaturalist.py` & `torchgeo-0.4.0/torchgeo/datasets/inaturalist.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .geo import GeoDataset
 from .utils import BoundingBox, disambiguate_timestamp
 
 
 class INaturalist(GeoDataset):
     """Dataset for iNaturalist.
 
-    `iNaturalist <https://www.inaturalist.org/>`_ is a joint initiative of the
+    `iNaturalist <https://www.inaturalist.org/>`__ is a joint initiative of the
     California Academy of Sciences and the National Geographic Society. It allows
     citizen scientists to upload observations of organisms that can be downloaded by
     scientists and researchers.
 
     If you use an iNaturalist dataset in your research, please cite it according to:
 
     * https://www.inaturalist.org/pages/help#cite
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/inria.py` & `torchgeo-0.4.0/torchgeo/datasets/inria.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     directory = "AerialImageDataset"
     filename = "NEW2-AerialImageDataset.zip"
     md5 = "4b1acfe84ae9961edc1a6049f940380f"
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         split: str = "train",
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         checksum: bool = False,
     ) -> None:
         """Initialize a new InriaAerialImageLabeling Dataset instance.
 
         Args:
@@ -112,30 +112,30 @@
             path: path to the image
 
         Returns:
             the image
         """
         with rio.open(path) as img:
             array = img.read().astype(np.int32)
-            tensor = torch.from_numpy(array)
+            tensor = torch.from_numpy(array).float()
             return tensor
 
     def _load_target(self, path: str) -> Tensor:
         """Loads the target mask.
 
         Args:
             path: path to the mask
 
         Returns:
             the target mask
         """
         with rio.open(path) as img:
             array = img.read().astype(np.int32)
             array = np.clip(array, 0, 1)
-            mask = torch.from_numpy(array[0])
+            mask = torch.from_numpy(array[0]).long()
             return mask
 
     def __len__(self) -> int:
         """Return the number of samples in the dataset.
 
         Returns:
             length of the dataset
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/landcoverai.py` & `torchgeo-0.4.0/torchgeo/datasets/seco.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,194 +1,214 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""LandCover.ai dataset."""
+"""Sentinel 2 imagery from the Seasonal Contrast paper."""
 
-import glob
-import hashlib
 import os
-from functools import lru_cache
-from typing import Callable, Dict, Optional
+from collections import defaultdict
+from typing import Callable, Dict, List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
+import rasterio
 import torch
-from matplotlib.colors import ListedColormap
 from PIL import Image
 from torch import Tensor
 
 from .geo import NonGeoDataset
-from .utils import download_url, extract_archive, working_dir
+from .utils import download_url, extract_archive, percentile_normalization
 
 
-class LandCoverAI(NonGeoDataset):
-    r"""LandCover.ai dataset.
+class SeasonalContrastS2(NonGeoDataset):
+    """Sentinel 2 imagery from the Seasonal Contrast paper.
 
-    The `LandCover.ai <https://landcover.ai/>`__ (Land Cover from Aerial Imagery)
-    dataset is a dataset for automatic mapping of buildings, woodlands, water and
-    roads from aerial images. This implementation is specifically for Version 1 of
-    Landcover.ai.
+    The `Seasonal Contrast imagery <https://github.com/ElementAI/seasonal-contrast/>`_
+    dataset contains Sentinel 2 imagery patches sampled from different points in time
+    around the 10k most populated cities on Earth.
 
     Dataset features:
 
-    * land cover from Poland, Central Europe
-    * three spectral bands - RGB
-    * 33 orthophotos with 25 cm per pixel resolution (~9000x9500 px)
-    * 8 orthophotos with 50 cm per pixel resolution (~4200x4700 px)
-    * total area of 216.27 km\ :sup:`2`
-
-    Dataset format:
-
-    * rasters are three-channel GeoTiffs with EPSG:2180 spatial reference system
-    * masks are single-channel GeoTiffs with EPSG:2180 spatial reference system
-
-    Dataset classes:
-
-    1. building (1.85 km\ :sup:`2`\ )
-    2. woodland (72.02 km\ :sup:`2`\ )
-    3. water (13.15 km\ :sup:`2`\ )
-    4. road (3.5 km\ :sup:`2`\ )
+    * Two versions: 100K and 1M patches
+    * 12 band Sentinel 2 imagery from 5 points in time at each location
 
     If you use this dataset in your research, please cite the following paper:
 
-    * https://arxiv.org/abs/2005.02264v3
-
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `opencv-python <https://pypi.org/project/opencv-python/>`_ to generate
-         the train/val/test split
+    * https://arxiv.org/pdf/2103.16607.pdf
     """
 
-    url = "https://landcover.ai.linuxpolska.com/download/landcover.ai.v1.zip"
-    filename = "landcover.ai.v1.zip"
-    md5 = "3268c89070e8734b4e91d531c0617e03"
-    sha256 = "15ee4ca9e3fd187957addfa8f0d74ac31bc928a966f76926e11b3c33ea76daa1"
-    classes = ["Background", "Building", "Woodland", "Water", "Road"]
-    cmap = ListedColormap(
-        [
-            [0.63921569, 1.0, 0.45098039],
-            [0.61176471, 0.61176471, 0.61176471],
-            [0.14901961, 0.45098039, 0.0],
-            [0.0, 0.77254902, 1.0],
-            [0.0, 0.0, 0.0],
-        ]
-    )
+    all_bands = [
+        "B1",
+        "B2",
+        "B3",
+        "B4",
+        "B5",
+        "B6",
+        "B7",
+        "B8",
+        "B8A",
+        "B9",
+        "B11",
+        "B12",
+    ]
+    rgb_bands = ["B4", "B3", "B2"]
+
+    urls = {
+        # 7.3 GB
+        "100k": "https://zenodo.org/record/4728033/files/seco_100k.zip?download=1",
+        # 36.3 GB
+        "1m": "https://zenodo.org/record/4728033/files/seco_1m.zip?download=1",
+    }
+    filenames = {"100k": "seco_100k.zip", "1m": "seco_1m.zip"}
+    md5s = {
+        "100k": "ebf2d5e03adc6e657f9a69a20ad863e0",
+        "1m": "187963d852d4d3ce6637743ec3a4bd9e",
+    }
+    directory_names = {"100k": "seasonal_contrast_100k", "1m": "seasonal_contrast_1m"}
 
     def __init__(
         self,
         root: str = "data",
-        split: str = "train",
+        version: str = "100k",
+        bands: List[str] = rgb_bands,
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new LandCover.ai dataset instance.
+        """Initialize a new SeCo dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            split: one of "train", "val", or "test"
+            version: one of "100k" or "1m" for the version of the dataset to use
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
             download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
 
         Raises:
-            AssertionError: if ``split`` argument is invalid
+            AssertionError: if ``version`` argument is invalid
             RuntimeError: if ``download=False`` and data is not found, or checksums
                 don't match
         """
-        assert split in ["train", "val", "test"]
+        assert version in ["100k", "1m"]
+        for band in bands:
+            assert band in self.all_bands
 
         self.root = root
-        self.split = split
+        self.bands = bands
+        self.url = self.urls[version]
+        self.filename = self.filenames[version]
+        self.md5 = self.md5s[version]
+        self.directory_name = self.directory_names[version]
         self.transforms = transforms
         self.download = download
         self.checksum = checksum
 
         self._verify()
 
-        with open(os.path.join(self.root, split + ".txt")) as f:
-            self.ids = f.readlines()
+        # TODO: This is slow, I think this should be generated on download and then
+        # loaded in the constructor
+        self.scene_to_patches = defaultdict(list)
+        for root_directory, directories, fns in os.walk(
+            os.path.join(self.root, self.directory_name)
+        ):
+            if len(directories) == 0 and len(fns) > 0:
+                root_directory, patch_name = os.path.split(root_directory)
+                _, scene_name = os.path.split(root_directory)
+                self.scene_to_patches[scene_name].append(patch_name)
+
+        self.scenes = sorted(self.scene_to_patches.keys())
+        for scene_name in self.scenes:
+            self.scene_to_patches[scene_name] = sorted(
+                self.scene_to_patches[scene_name]
+            )
 
     def __getitem__(self, index: int) -> Dict[str, Tensor]:
         """Return an index within the dataset.
 
         Args:
             index: index to return
 
         Returns:
-            data and label at that index
+            sample with an "image" in 5xCxHxW format where the 5 indexes over the same
+                patch sampled from different points in time by the SeCo method
         """
-        id_ = self.ids[index].rstrip()
-        sample = {"image": self._load_image(id_), "mask": self._load_target(id_)}
+        scene_name = self.scenes[index]
+        patch_names = self.scene_to_patches[scene_name]
+
+        imagery = [
+            self._load_patch(scene_name, patch_name) for patch_name in patch_names
+        ]
+
+        sample = {"image": torch.stack(imagery, dim=0)}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
 
         Returns:
             length of the dataset
         """
-        return len(self.ids)
+        return len(self.scenes)
 
-    @lru_cache()
-    def _load_image(self, id_: str) -> Tensor:
-        """Load a single image.
+    def _load_patch(self, scene_name: str, patch_name: str) -> Tensor:
+        """Load a single image patch.
 
         Args:
-            id_: unique ID of the image
+            scene_name: the name of the scene to load from, e.g. '019999'
+            patch_name: the name of the patch to load, e.g.
+                '20200713T075609_20200713T081050_T36QZH'
 
         Returns:
-            the image
+            the image with the subset of bands specified by ``self.bands``
         """
-        filename = os.path.join(self.root, "output", id_ + ".jpg")
-        with Image.open(filename) as img:
-            array: "np.typing.NDArray[np.int_]" = np.array(img)
-            tensor = torch.from_numpy(array)
-            # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
-            return tensor
-
-    @lru_cache()
-    def _load_target(self, id_: str) -> Tensor:
-        """Load the target mask for a single image.
-
-        Args:
-            id_: unique ID of the image
-
-        Returns:
-            the target mask
-        """
-        filename = os.path.join(self.root, "output", id_ + "_m.png")
-        with Image.open(filename) as img:
-            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("L"))
-            tensor = torch.from_numpy(array)
-            return tensor
+        all_data = []
+        for band in self.bands:
+            fn = os.path.join(
+                self.root, self.directory_name, scene_name, patch_name, f"{band}.tif"
+            )
+            with rasterio.open(fn) as f:
+                band_data = f.read(1)
+                height, width = band_data.shape
+                size = min(height, width)
+                if size < 264:
+                    # TODO: PIL resize is much slower than cv2, we should check to see
+                    # what could be sped up throughout later. There is also a potential
+                    # slowdown here from converting to/from a PIL Image just to resize.
+                    # https://gist.github.com/calebrob6/748045ac8d844154067b2eefa47de92f
+                    pil_image = Image.fromarray(band_data)
+                    # Moved in PIL 9.1.0
+                    try:
+                        resample = Image.Resampling.BILINEAR
+                    except AttributeError:
+                        resample = Image.BILINEAR
+                    band_data = np.array(
+                        pil_image.resize((264, 264), resample=resample)
+                    )
+                all_data.append(band_data)
+        image = torch.from_numpy(np.stack(all_data, axis=0))
+        return image
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
         # Check if the extracted files already exist
-        jpg = os.path.join(self.root, "output", "*_*.jpg")
-        png = os.path.join(self.root, "output", "*_*_m.png")
-        if glob.glob(jpg) and glob.glob(png):
+        directory_path = os.path.join(self.root, self.directory_name)
+        if os.path.exists(directory_path):
             return
 
-        # Check if the zip file has already been downloaded
-        pathname = os.path.join(self.root, self.filename)
-        if os.path.exists(pathname):
+        # Check if the zip files have already been downloaded
+        zip_path = os.path.join(self.root, self.filename)
+        if os.path.exists(zip_path):
             self._extract()
             return
 
         # Check if the user requested to download the dataset
         if not self.download:
             raise RuntimeError(
                 f"Dataset not found in `root={self.root}` and `download=False`, "
@@ -198,33 +218,25 @@
 
         # Download the dataset
         self._download()
         self._extract()
 
     def _download(self) -> None:
         """Download the dataset."""
-        download_url(self.url, self.root, md5=self.md5 if self.checksum else None)
+        download_url(
+            self.url,
+            self.root,
+            filename=self.filename,
+            md5=self.md5 if self.checksum else None,
+        )
 
     def _extract(self) -> None:
-        """Extract the dataset.
-
-        Raises:
-            AssertionError: if the checksum of split.py does not match
-        """
+        """Extract the dataset."""
         extract_archive(os.path.join(self.root, self.filename))
 
-        # Generate train/val/test splits
-        # Always check the sha256 of this file before executing
-        # to avoid malicious code injection
-        with working_dir(self.root):
-            with open("split.py") as f:
-                split = f.read().encode("utf-8")
-                assert hashlib.sha256(split).hexdigest() == self.sha256
-                exec(split)
-
     def plot(
         self,
         sample: Dict[str, Tensor],
         show_titles: bool = True,
         suptitle: Optional[str] = None,
     ) -> plt.Figure:
         """Plot a sample from the dataset.
@@ -233,38 +245,39 @@
             sample: a sample returned by :meth:`__getitem__`
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
 
+        Raises:
+            ValueError: if the RGB bands are included in ``self.bands`` or the sample
+                contains a "prediction" key
+
         .. versionadded:: 0.2
         """
-        image = np.rollaxis(sample["image"].numpy(), 0, 3)
-        mask = sample["mask"].numpy()
+        if "prediction" in sample:
+            raise ValueError("This dataset doesn't support plotting predictions")
 
-        num_panels = 2
-        showing_predictions = "prediction" in sample
-        if showing_predictions:
-            predictions = sample["prediction"].numpy()
-            num_panels += 1
-
-        fig, axs = plt.subplots(1, num_panels, figsize=(num_panels * 4, 5))
-        axs[0].imshow(image)
-        axs[0].axis("off")
-        axs[1].imshow(mask, vmin=0, vmax=4, cmap=self.cmap, interpolation="none")
-        axs[1].axis("off")
-        if show_titles:
-            axs[0].set_title("Image")
-            axs[1].set_title("Mask")
-
-        if showing_predictions:
-            axs[2].imshow(
-                predictions, vmin=0, vmax=4, cmap=self.cmap, interpolation="none"
-            )
-            axs[2].axis("off")
+        rgb_indices = []
+        for band in self.rgb_bands:
+            if band in self.bands:
+                rgb_indices.append(self.bands.index(band))
+            else:
+                raise ValueError("Dataset doesn't contain some of the RGB bands")
+
+        images = []
+        for i in range(5):
+            image = np.rollaxis(sample["image"][i, rgb_indices].numpy(), 0, 3)
+            image = percentile_normalization(image, 0, 100)
+            images.append(image)
+
+        fig, axs = plt.subplots(ncols=5, figsize=(20, 4))
+        for i in range(5):
+            axs[i].imshow(images[i])
+            axs[i].axis("off")
             if show_titles:
-                axs[2].set_title("Predictions")
+                axs[i].set_title(f"t={i+1}")
 
         if suptitle is not None:
             plt.suptitle(suptitle)
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/landsat.py` & `torchgeo-0.4.0/torchgeo/datasets/landsat.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     separate_files = True
 
     def __init__(
         self,
         root: str = "data",
         crs: Optional[CRS] = None,
         res: Optional[float] = None,
-        bands: Sequence[str] = [],
+        bands: Optional[Sequence[str]] = None,
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         cache: bool = True,
     ) -> None:
         """Initialize a new Dataset instance.
 
         Args:
             root: root directory where dataset can be found
@@ -70,18 +70,18 @@
             transforms: a function/transform that takes an input sample
                 and returns a transformed version
             cache: if True, cache file handle to speed up repeated sampling
 
         Raises:
             FileNotFoundError: if no files are found in ``root``
         """
-        self.bands = bands if bands else self.all_bands
-        self.filename_glob = self.filename_glob.format(self.bands[0])
+        bands = bands or self.all_bands
+        self.filename_glob = self.filename_glob.format(bands[0])
 
-        super().__init__(root, crs, res, transforms, cache)
+        super().__init__(root, crs, res, bands, transforms, cache)
 
     def plot(
         self,
         sample: Dict[str, Any],
         show_titles: bool = True,
         suptitle: Optional[str] = None,
     ) -> plt.Figure:
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/levircd.py` & `torchgeo-0.4.0/torchgeo/datasets/levircd.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/loveda.py` & `torchgeo-0.4.0/torchgeo/datasets/resisc45.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,282 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""LoveDA dataset."""
+"""RESISC45 dataset."""
 
-import glob
 import os
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Dict, Optional, cast
 
 import matplotlib.pyplot as plt
 import numpy as np
-import torch
-from PIL import Image
 from torch import Tensor
 
-from .geo import NonGeoDataset
-from .utils import download_and_extract_archive
+from .geo import NonGeoClassificationDataset
+from .utils import download_url, extract_archive
 
 
-class LoveDA(NonGeoDataset):
-    """LoveDA dataset.
+class RESISC45(NonGeoClassificationDataset):
+    """NWPU-RESISC45 dataset.
 
-    The `LoveDA <https://github.com/Junjue-Wang/LoveDA>`__ datataset is a
-    semantic segmentation dataset.
+    The `RESISC45 <http://www.escience.cn/people/JunweiHan/NWPU-RESISC45.html>`__
+    dataset is a dataset for remote sensing image scene classification.
 
     Dataset features:
 
-    * 2713 urban scene and 3274 rural scene HSR images, spatial resolution of 0.3m
-    * image source is Google Earth platform
-    * total of 166768 annotated objects from Nanjing, Changzhou and Wuhan cities
-    * dataset comes with predefined train, validation, and test set
-    * dataset differentiates between 'rural' and 'urban' images
+    * 31,500 images with 0.2-30 m per pixel resolution (256x256 px)
+    * three spectral bands - RGB
+    * 45 scene classes, 700 images per class
+    * images extracted from Google Earth from over 100 countries
+    * images conditions with high variability (resolution, weather, illumination)
 
     Dataset format:
 
-    * images are three-channel pngs with dimension 1024x1024
-    * segmentation masks are single-channel pngs
+    * images are three-channel jpgs
 
     Dataset classes:
 
-    1. background
-    2. building
-    3. road
-    4. water
-    5. barren
-    6. forest
-    7. agriculture
+    0. airplane
+    1. airport
+    2. baseball_diamond
+    3. basketball_court
+    4. beach
+    5. bridge
+    6. chaparral
+    7. church
+    8. circular_farmland
+    9. cloud
+    10. commercial_area
+    11. dense_residential
+    12. desert
+    13. forest
+    14. freeway
+    15. golf_course
+    16. ground_track_field
+    17. harbor
+    18. industrial_area
+    19. intersection
+    20. island
+    21. lake
+    22. meadow
+    23. medium_residential
+    24. mobile_home_park
+    25. mountain
+    26. overpass
+    27. palace
+    28. parking_lot
+    29. railway
+    30. railway_station
+    31. rectangular_farmland
+    32. river
+    33. roundabout
+    34. runway
+    35. sea_ice
+    36. ship
+    37. snowberg
+    38. sparse_residential
+    39. stadium
+    40. storage_tank
+    41. tennis_court
+    42. terrace
+    43. thermal_power_station
+    44. wetland
 
-    No-data regions assigned with 0 and should be ignored.
+    This dataset uses the train/val/test splits defined in the "In-domain representation
+    learning for remote sensing" paper:
+
+    * https://arxiv.org/abs/1911.06721
 
     If you use this dataset in your research, please cite the following paper:
 
-    * <https://arxiv.org/abs/2110.08733>
+    * https://doi.org/10.1109/jproc.2017.2675998
 
-    .. versionadded:: 0.2
     """
 
-    scenes = ["urban", "rural"]
-    splits = ["train", "val", "test"]
+    url = "https://drive.google.com/file/d/1DnPSU5nVSN7xv95bpZ3XQ0JhKXZOKgIv"
+    md5 = "d824acb73957502b00efd559fc6cfbbb"
+    filename = "NWPU-RESISC45.rar"
+    directory = "NWPU-RESISC45"
 
-    info_dict = {
-        "train": {
-            "url": "https://zenodo.org/record/5706578/files/Train.zip?download=1",
-            "filename": "Train.zip",
-            "md5": "de2b196043ed9b4af1690b3f9a7d558f",
-        },
-        "val": {
-            "url": "https://zenodo.org/record/5706578/files/Val.zip?download=1",
-            "filename": "Val.zip",
-            "md5": "84cae2577468ff0b5386758bb386d31d",
-        },
-        "test": {
-            "url": "https://zenodo.org/record/5706578/files/Test.zip?download=1",
-            "filename": "Test.zip",
-            "md5": "a489be0090465e01fb067795d24e6b47",
-        },
+    splits = ["train", "val", "test"]
+    split_urls = {
+        "train": "https://storage.googleapis.com/remote_sensing_representations/resisc45-train.txt",  # noqa: E501
+        "val": "https://storage.googleapis.com/remote_sensing_representations/resisc45-val.txt",  # noqa: E501
+        "test": "https://storage.googleapis.com/remote_sensing_representations/resisc45-test.txt",  # noqa: E501
+    }
+    split_md5s = {
+        "train": "b5a4c05a37de15e4ca886696a85c403e",
+        "val": "a0770cee4c5ca20b8c32bbd61e114805",
+        "test": "3dda9e4988b47eb1de9f07993653eb08",
     }
-
     classes = [
-        "background",
-        "building",
-        "road",
-        "water",
-        "barren",
+        "airplane",
+        "airport",
+        "baseball_diamond",
+        "basketball_court",
+        "beach",
+        "bridge",
+        "chaparral",
+        "church",
+        "circular_farmland",
+        "cloud",
+        "commercial_area",
+        "dense_residential",
+        "desert",
         "forest",
-        "agriculture",
-        "no-data",
+        "freeway",
+        "golf_course",
+        "ground_track_field",
+        "harbor",
+        "industrial_area",
+        "intersection",
+        "island",
+        "lake",
+        "meadow",
+        "medium_residential",
+        "mobile_home_park",
+        "mountain",
+        "overpass",
+        "palace",
+        "parking_lot",
+        "railway",
+        "railway_station",
+        "rectangular_farmland",
+        "river",
+        "roundabout",
+        "runway",
+        "sea_ice",
+        "ship",
+        "snowberg",
+        "sparse_residential",
+        "stadium",
+        "storage_tank",
+        "tennis_court",
+        "terrace",
+        "thermal_power_station",
+        "wetland",
     ]
 
     def __init__(
         self,
         root: str = "data",
         split: str = "train",
-        scene: List[str] = ["urban", "rural"],
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new LoveDA dataset instance.
+        """Initialize a new RESISC45 dataset instance.
 
         Args:
             root: root directory where dataset can be found
             split: one of "train", "val", or "test"
-            scene: specify whether to load only 'urban', only 'rural' or both
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
             download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
-
-        Raises:
-            AssertionError: if ``split`` argument is invalid
-            AssertionError: if ``scene`` argument is invalid
-            RuntimeError: if ``download=False`` and data is not found, or checksums
-                don't match
         """
-        print(split)
         assert split in self.splits
-        assert set(scene).intersection(
-            set(self.scenes)
-        ), "The possible scenes are 'rural' and/or 'urban'"
-        assert len(scene) <= 2, "There are no other scenes than 'rural' or 'urban'"
-
         self.root = root
-        self.split = split
-        self.scene = scene
-        self.transforms = transforms
+        self.download = download
         self.checksum = checksum
+        self._verify()
 
-        self.url = self.info_dict[self.split]["url"]
-        self.filename = self.info_dict[self.split]["filename"]
-        self.md5 = self.info_dict[self.split]["md5"]
-
-        self.directory = os.path.join(self.root, split.capitalize())
-        self.scene_paths = [
-            os.path.join(self.directory, s.capitalize()) for s in self.scene
-        ]
-
-        if download:
-            self._download()
-
-        if not self._check_integrity():
-            raise RuntimeError(
-                "Dataset not found at root directory or corrupted. "
-                + "You can use download=True to download it"
-            )
-
-        self.files = self._load_files(self.scene_paths, self.split)
-
-    def __getitem__(self, index: int) -> Dict[str, Tensor]:
-        """Return an index within the dataset.
-
-        Args:
-            index: index to return
-
-        Returns:
-            image and mask at that index with image of dimension 3x1024x1024
-            and mask of dimension 1024x1024
-        """
-        files = self.files[index]
-        image = self._load_image(files["image"])
-
-        if self.split != "test":
-            mask = self._load_target(files["mask"])
-            sample = {"image": image, "mask": mask}
-        else:
-            sample = {"image": image}
-
-        if self.transforms is not None:
-            sample = self.transforms(sample)
-
-        return sample
-
-    def __len__(self) -> int:
-        """Return the number of datapoints in the dataset.
-
-        Returns:
-            length of dataset
-        """
-        return len(self.files)
-
-    def _load_files(self, scene_paths: List[str], split: str) -> List[Dict[str, str]]:
-        """Return the paths of the files in the dataset.
-
-        Args:
-            scene_paths: contains one or two paths, depending on whether user has
-                         specified only 'rural', 'only 'urban' or both
-            split: subset of dataset, one of [train, val, test]
-        """
-        images = []
-
-        for s in scene_paths:
-            images.extend(glob.glob(os.path.join(s, "images_png", "*.png")))
-
-        images = sorted(images)
-
-        if self.split != "test":
-            masks = [image.replace("images_png", "masks_png") for image in images]
-            files = [
-                dict(image=image, mask=mask) for image, mask, in zip(images, masks)
-            ]
-        else:
-            files = [dict(image=image) for image in images]
-
-        return files
-
-    def _load_image(self, path: str) -> Tensor:
-        """Load a single image.
-
-        Args:
-            path: path to the image
-
-        Returns:
-            the loaded image
-        """
-        filename = os.path.join(path)
-        with Image.open(filename) as img:
-            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
-            tensor = torch.from_numpy(array)
-            # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
-            return tensor
-
-    def _load_target(self, path: str) -> Tensor:
-        """Load a single mask corresponding to image.
+        valid_fns = set()
+        with open(os.path.join(self.root, f"resisc45-{split}.txt")) as f:
+            for fn in f:
+                valid_fns.add(fn.strip())
+        is_in_split: Callable[[str], bool] = lambda x: os.path.basename(x) in valid_fns
+
+        super().__init__(
+            root=os.path.join(root, self.directory),
+            transforms=transforms,
+            is_valid_file=is_in_split,
+        )
 
-        Args:
-            path: path to the mask
+    def _verify(self) -> None:
+        """Verify the integrity of the dataset.
 
-        Returns:
-            the mask of the image
+        Raises:
+            RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
-        filename = os.path.join(path)
-        with Image.open(filename) as img:
-            array: "np.typing.NDArray[np.int_]" = np.array(img.convert("L"))
-            tensor = torch.from_numpy(array)
-            tensor = tensor.to(torch.long)
-            return tensor
+        # Check if the files already exist
+        filepath = os.path.join(self.root, self.directory)
+        if os.path.exists(filepath):
+            return
 
-    def _check_integrity(self) -> bool:
-        """Check the integrity of the dataset structure.
+        # Check if zip file already exists (if so then extract)
+        filepath = os.path.join(self.root, self.filename)
+        if os.path.exists(filepath):
+            self._extract()
+            return
 
-        Returns:
-            True if the dataset directories and split files are found, else False
-        """
-        for s in self.scene_paths:
-            if not os.path.exists(s):
-                return False
+        # Check if the user requested to download the dataset
+        if not self.download:
+            raise RuntimeError(
+                "Dataset not found in `root` directory and `download=False`, "
+                "either specify a different `root` directory or use `download=True` "
+                "to automatically download the dataset."
+            )
 
-        return True
+        # Download and extract the dataset
+        self._download()
+        self._extract()
 
     def _download(self) -> None:
-        """Download the dataset and extract it.
-
-        Raises:
-            AssertionError: if the checksum of split.py does not match
-        """
-        if self._check_integrity():
-            print("Files already downloaded and verified")
-            return
-
-        download_and_extract_archive(
+        """Download the dataset."""
+        download_url(
             self.url,
             self.root,
             filename=self.filename,
             md5=self.md5 if self.checksum else None,
         )
+        for split in self.splits:
+            download_url(
+                self.split_urls[split],
+                self.root,
+                filename=f"resisc45-{split}.txt",
+                md5=self.split_md5s[split] if self.checksum else None,
+            )
+
+    def _extract(self) -> None:
+        """Extract the dataset."""
+        filepath = os.path.join(self.root, self.filename)
+        extract_archive(filepath)
 
     def plot(
-        self, sample: Dict[str, Tensor], suptitle: Optional[str] = None
+        self,
+        sample: Dict[str, Tensor],
+        show_titles: bool = True,
+        suptitle: Optional[str] = None,
     ) -> plt.Figure:
         """Plot a sample from the dataset.
 
         Args:
-            sample: a sample return by :meth:`__getitem__`
-            suptitle: optional suptitle to use for figure
+            sample: a sample returned by :meth:`NonGeoClassificationDataset.__getitem__`
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
+
+        .. versionadded:: 0.2
         """
-        if self.split != "test":
-            image, mask = sample["image"], sample["mask"]
-            ncols = 2
-        else:
-            image = sample["image"]
-            ncols = 1
-
-        fig, axs = plt.subplots(nrows=1, ncols=ncols, figsize=(10, ncols * 10))
-
-        if self.split != "test":
-            axs[0].imshow(image.permute(1, 2, 0))
-            axs[0].axis("off")
-            axs[1].imshow(mask)
-            axs[1].axis("off")
-        else:
-            axs.imshow(image.permute(1, 2, 0))
-            axs.axis("off")
+        image = np.rollaxis(sample["image"].numpy(), 0, 3)
+        label = cast(int, sample["label"].item())
+        label_class = self.classes[label]
+
+        showing_predictions = "prediction" in sample
+        if showing_predictions:
+            prediction = cast(int, sample["prediction"].item())
+            prediction_class = self.classes[prediction]
+
+        fig, ax = plt.subplots(figsize=(4, 4))
+        ax.imshow(image)
+        ax.axis("off")
+        if show_titles:
+            title = f"Label: {label_class}"
+            if showing_predictions:
+                title += f"\nPrediction: {prediction_class}"
+            ax.set_title(title)
 
         if suptitle is not None:
             plt.suptitle(suptitle)
-
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/millionaid.py` & `torchgeo-0.4.0/torchgeo/datasets/millionaid.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/naip.py` & `torchgeo-0.4.0/torchgeo/datasets/naip.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/nasa_marine_debris.py` & `torchgeo-0.4.0/torchgeo/datasets/nasa_marine_debris.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,20 @@
         Returns:
             data and labels at that index
         """
         image = self._load_image(self.files[index]["image"])
         boxes = self._load_target(self.files[index]["target"])
         sample = {"image": image, "boxes": boxes}
 
+        # Filter invalid boxes
+        w_check = (sample["boxes"][:, 2] - sample["boxes"][:, 0]) > 0
+        h_check = (sample["boxes"][:, 3] - sample["boxes"][:, 1]) > 0
+        indices = w_check & h_check
+        sample["boxes"] = sample["boxes"][indices]
+
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
@@ -119,15 +125,15 @@
             path: path to the image
 
         Returns:
             the image
         """
         with rasterio.open(path) as f:
             array = f.read()
-        tensor = torch.from_numpy(array)
+        tensor = torch.from_numpy(array).float()
         return tensor
 
     def _load_target(self, path: str) -> Tensor:
         """Load the target bounding boxes for a single image.
 
         Args:
             path: path to the labels
@@ -223,18 +229,21 @@
             suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
         """
         ncols = 1
 
-        image = draw_bounding_boxes(image=sample["image"], boxes=sample["boxes"])
+        sample["image"] = sample["image"].byte()
+        image = sample["image"]
+        if "boxes" in sample and len(sample["boxes"]):
+            image = draw_bounding_boxes(image=sample["image"], boxes=sample["boxes"])
         image = image.permute((1, 2, 0)).numpy()
 
-        if "prediction_boxes" in sample:
+        if "prediction_boxes" in sample and len(sample["prediction_boxes"]):
             ncols += 1
             preds = draw_bounding_boxes(
                 image=sample["image"], boxes=sample["prediction_boxes"]
             )
             preds = preds.permute((1, 2, 0)).numpy()
 
         fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/nwpu.py` & `torchgeo-0.4.0/torchgeo/datasets/potsdam.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,246 +1,293 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""NWPU VHR-10 dataset."""
+"""Potsdam dataset."""
 
 import os
-from typing import Any, Callable, Dict, Optional
+from typing import Callable, Dict, Optional
 
+import matplotlib.pyplot as plt
 import numpy as np
+import rasterio
 import torch
+from matplotlib.figure import Figure
 from PIL import Image
 from torch import Tensor
 
 from .geo import NonGeoDataset
-from .utils import check_integrity, download_and_extract_archive, download_url
-
-
-class VHR10(NonGeoDataset):
-    """NWPU VHR-10 dataset.
-
-    Northwestern Polytechnical University (NWPU) very-high-resolution ten-class (VHR-10)
-    remote sensing image dataset.
-
-    Consists of 800 VHR optical remote sensing images, where 715 color images were
-    acquired from Google Earth with the spatial resolution ranging from 0.5 to 2 m,
-    and 85 pansharpened color infrared (CIR) images were acquired from Vaihingen data
-    with a spatial resolution of 0.08 m.
-
-    The data set is divided into two sets:
-
-    * Positive image set (650 images) which contains at least one target in an image
-    * Negative image set (150 images) does not contain any targets
-
-    The positive image set consists of objects from ten classes:
-
-    1. Airplanes (757)
-    2. Ships (302)
-    3. Storage tanks (655)
-    4. Baseball diamonds (390)
-    5. Tennis courts (524)
-    6. Basketball courts (159)
-    7. Ground track fields (163)
-    8. Harbors (224)
-    9. Bridges (124)
-    10. Vehicles (477)
-
-    Includes object detection bounding boxes from original paper and instance
-    segmentation masks from follow-up publications. If you use this dataset in your
-    research, please cite the following papers:
-
-    * https://doi.org/10.1016/j.isprsjprs.2014.10.002
-    * https://doi.org/10.1109/IGARSS.2019.8898573
-    * https://doi.org/10.3390/rs12060989
-
-    .. note::
-
-       This dataset requires the following additional libraries to be installed:
-
-       * `pycocotools <https://pypi.org/project/pycocotools/>`_ to load the
-         ``annotations.json`` file for the "positive" image set
-       * `rarfile <https://pypi.org/project/rarfile/>`_ to extract the dataset,
-         which is stored in a RAR file
-    """
-
-    image_meta = {
-        "url": "https://drive.google.com/file/d/1--foZ3dV5OCsqXQXT84UeKtrAqc5CkAE",
-        "filename": "NWPU VHR-10 dataset.rar",
-        "md5": "d30a7ff99d92123ebb0b3a14d9102081",
-    }
-    target_meta = {
-        "url": (
-            "https://raw.githubusercontent.com/chaozhong2010/VHR-10_dataset_coco/"
-            "master/NWPU%20VHR-10_dataset_coco/annotations.json"
-        ),
-        "filename": "annotations.json",
-        "md5": "7c76ec50c17a61bb0514050d20f22c08",
+from .utils import (
+    check_integrity,
+    draw_semantic_segmentation_masks,
+    extract_archive,
+    rgb_to_mask,
+)
+
+
+class Potsdam2D(NonGeoDataset):
+    """Potsdam 2D Semantic Segmentation dataset.
+
+    The `Potsdam <https://www2.isprs.org/commissions/comm2/wg4/benchmark/2d-sem-label-potsdam/>`__
+    dataset is a dataset for urban semantic segmentation used in the 2D Semantic Labeling
+    Contest - Potsdam. This dataset uses the "4_Ortho_RGBIR.zip" and "5_Labels_all.zip"
+    files to create the train/test sets used in the challenge. The dataset can be
+    requested at the challenge homepage. Note, the server contains additional data
+    for 3D Semantic Labeling which are currently not supported.
+
+    Dataset format:
+
+    * images are 4-channel geotiffs
+    * masks are 3-channel geotiffs with unique RGB values representing the class
+
+    Dataset classes:
+
+    0. Clutter/background
+    1. Impervious surfaces
+    2. Building
+    3. Low Vegetation
+    4. Tree
+    5. Car
+
+    If you use this dataset in your research, please cite the following paper:
+
+    * https://doi.org/10.5194/isprsannals-I-3-293-2012
+
+    .. versionadded:: 0.2
+    """  # noqa: E501
+
+    filenames = ["4_Ortho_RGBIR.zip", "5_Labels_all.zip"]
+    md5s = ["c4a8f7d8c7196dd4eba4addd0aae10c1", "cf7403c1a97c0d279414db"]
+    image_root = "4_Ortho_RGBIR"
+    splits = {
+        "train": [
+            "top_potsdam_2_10",
+            "top_potsdam_2_11",
+            "top_potsdam_2_12",
+            "top_potsdam_3_10",
+            "top_potsdam_3_11",
+            "top_potsdam_3_12",
+            "top_potsdam_4_10",
+            "top_potsdam_4_11",
+            "top_potsdam_4_12",
+            "top_potsdam_5_10",
+            "top_potsdam_5_11",
+            "top_potsdam_5_12",
+            "top_potsdam_6_10",
+            "top_potsdam_6_11",
+            "top_potsdam_6_12",
+            "top_potsdam_6_7",
+            "top_potsdam_6_8",
+            "top_potsdam_6_9",
+            "top_potsdam_7_10",
+            "top_potsdam_7_11",
+            "top_potsdam_7_12",
+            "top_potsdam_7_7",
+            "top_potsdam_7_8",
+            "top_potsdam_7_9",
+        ],
+        "test": [
+            "top_potsdam_5_15",
+            "top_potsdam_6_15",
+            "top_potsdam_6_13",
+            "top_potsdam_3_13",
+            "top_potsdam_4_14",
+            "top_potsdam_6_14",
+            "top_potsdam_5_14",
+            "top_potsdam_2_13",
+            "top_potsdam_4_15",
+            "top_potsdam_2_14",
+            "top_potsdam_5_13",
+            "top_potsdam_4_13",
+            "top_potsdam_3_14",
+            "top_potsdam_7_13",
+        ],
     }
+    classes = [
+        "Clutter/background",
+        "Impervious surfaces",
+        "Building",
+        "Low Vegetation",
+        "Tree",
+        "Car",
+    ]
+    colormap = [
+        (255, 0, 0),
+        (255, 255, 255),
+        (0, 0, 255),
+        (0, 255, 255),
+        (0, 255, 0),
+        (255, 255, 0),
+    ]
 
     def __init__(
         self,
         root: str = "data",
-        split: str = "positive",
-        transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
-        download: bool = False,
+        split: str = "train",
+        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new VHR-10 dataset instance.
+        """Initialize a new Potsdam dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            split: one of "postive" or "negative"
+            split: one of "train" or "test"
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
-            download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
-
-        Raises:
-            AssertionError: if ``split`` argument is invalid
-            RuntimeError: if ``download=False`` and data is not found, or checksums
-                don't match
         """
-        assert split in ["positive", "negative"]
-
+        assert split in self.splits
         self.root = root
         self.split = split
         self.transforms = transforms
         self.checksum = checksum
 
-        if download:
-            self._download()
+        self._verify()
 
-        if not self._check_integrity():
-            raise RuntimeError(
-                "Dataset not found or corrupted. "
-                + "You can use download=True to download it"
-            )
-
-        if split == "positive":
-            # Must be installed to parse annotations file
-            try:
-                from pycocotools.coco import COCO  # noqa: F401
-            except ImportError:
-                raise ImportError(
-                    "pycocotools is not installed and is required to use this dataset"
-                )
-
-            self.coco = COCO(
-                os.path.join(
-                    self.root, "NWPU VHR-10 dataset", self.target_meta["filename"]
-                )
-            )
+        self.files = []
+        for name in self.splits[split]:
+            image = os.path.join(root, self.image_root, name) + "_RGBIR.tif"
+            mask = os.path.join(root, name) + "_label.tif"
+            if os.path.exists(image) and os.path.exists(mask):
+                self.files.append(dict(image=image, mask=mask))
 
-    def __getitem__(self, index: int) -> Dict[str, Any]:
+    def __getitem__(self, index: int) -> Dict[str, Tensor]:
         """Return an index within the dataset.
 
         Args:
             index: index to return
 
         Returns:
             data and label at that index
         """
-        id_ = index % len(self) + 1
-        sample = {"image": self._load_image(id_), "label": self._load_target(id_)}
+        image = self._load_image(index)
+        mask = self._load_target(index)
+        sample = {"image": image, "mask": mask}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
 
         Returns:
             length of the dataset
         """
-        if self.split == "positive":
-            return 650
-        else:
-            return 150
+        return len(self.files)
 
-    def _load_image(self, id_: int) -> Tensor:
+    def _load_image(self, index: int) -> Tensor:
         """Load a single image.
 
         Args:
-            id_: unique ID of the image
+            index: index to return
 
         Returns:
             the image
         """
-        filename = os.path.join(
-            self.root,
-            "NWPU VHR-10 dataset",
-            self.split + " image set",
-            f"{id_:03d}.jpg",
-        )
-        with Image.open(filename) as img:
-            array: "np.typing.NDArray[np.int_]" = np.array(img)
-            tensor = torch.from_numpy(array)
-            # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
+        path = self.files[index]["image"]
+        with rasterio.open(path) as f:
+            array = f.read()
+            tensor = torch.from_numpy(array).float()
             return tensor
 
-    def _load_target(self, id_: int) -> Dict[str, Any]:
-        """Load the annotations for a single image.
+    def _load_target(self, index: int) -> Tensor:
+        """Load the target mask for a single image.
 
         Args:
-            id_: unique ID of the image
+            index: index to return
 
         Returns:
-            the annotations
+            the target mask
         """
-        # Images in the "negative" image set have no annotations
-        annot = []
-        if self.split == "positive":
-            annot = self.coco.loadAnns(self.coco.getAnnIds(id_))
+        path = self.files[index]["mask"]
+        with Image.open(path) as img:
+            array: "np.typing.NDArray[np.uint8]" = np.array(img.convert("RGB"))
+            array = rgb_to_mask(array, self.colormap)
+            tensor = torch.from_numpy(array)
+            # Convert from HxWxC to CxHxW
+            tensor = tensor.to(torch.long)
+        return tensor
+
+    def _verify(self) -> None:
+        """Verify the integrity of the dataset.
+
+        Raises:
+            RuntimeError: if checksum fails or the dataset is not downloaded
+        """
+        # Check if the files already exist
+        if os.path.exists(os.path.join(self.root, self.image_root)):
+            return
 
-        target = dict(image_id=id_, annotations=annot)
+        # Check if .zip files already exists (if so extract)
+        exists = []
+        for filename, md5 in zip(self.filenames, self.md5s):
+            filepath = os.path.join(self.root, filename)
+            if os.path.isfile(filepath):
+                if self.checksum and not check_integrity(filepath, md5):
+                    raise RuntimeError("Dataset found, but corrupted.")
+                exists.append(True)
+                extract_archive(filepath)
+            else:
+                exists.append(False)
 
-        return target
+        if all(exists):
+            return
+
+        # Check if the user requested to download the dataset
+        raise RuntimeError(
+            "Dataset not found in `root` directory, either specify a different"
+            + " `root` directory or manually download the dataset to this directory."
+        )
 
-    def _check_integrity(self) -> bool:
-        """Check integrity of dataset.
+    def plot(
+        self,
+        sample: Dict[str, Tensor],
+        show_titles: bool = True,
+        suptitle: Optional[str] = None,
+        alpha: float = 0.5,
+    ) -> Figure:
+        """Plot a sample from the dataset.
+
+        Args:
+            sample: a sample returned by :meth:`__getitem__`
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional string to use as a suptitle
+            alpha: opacity with which to render predictions on top of the imagery
 
         Returns:
-            True if dataset files are found and/or MD5s match, else False
+            a matplotlib Figure with the rendered sample
         """
-        image: bool = check_integrity(
-            os.path.join(self.root, self.image_meta["filename"]),
-            self.image_meta["md5"] if self.checksum else None,
+        ncols = 1
+        image1 = draw_semantic_segmentation_masks(
+            sample["image"][:3], sample["mask"], alpha=alpha, colors=self.colormap
         )
-
-        # Annotations only needed for "positive" image set
-        target = True
-        if self.split == "positive":
-            target = check_integrity(
-                os.path.join(
-                    self.root, "NWPU VHR-10 dataset", self.target_meta["filename"]
-                ),
-                self.target_meta["md5"] if self.checksum else None,
+        if "prediction" in sample:
+            ncols += 1
+            image2 = draw_semantic_segmentation_masks(
+                sample["image"][:3],
+                sample["prediction"],
+                alpha=alpha,
+                colors=self.colormap,
             )
 
-        return image and target
+        fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
+        if ncols > 1:
+            (ax0, ax1) = axs
+        else:
+            ax0 = axs
 
-    def _download(self) -> None:
-        """Download the dataset and extract it."""
-        if self._check_integrity():
-            print("Files already downloaded and verified")
-            return
+        ax0.imshow(image1)
+        ax0.axis("off")
+        if ncols > 1:
+            ax1.imshow(image2)
+            ax1.axis("off")
+
+        if show_titles:
+            ax0.set_title("Ground Truth")
+            if ncols > 1:
+                ax1.set_title("Predictions")
 
-        # Download images
-        download_and_extract_archive(
-            self.image_meta["url"],
-            self.root,
-            filename=self.image_meta["filename"],
-            md5=self.image_meta["md5"] if self.checksum else None,
-        )
+        if suptitle is not None:
+            plt.suptitle(suptitle)
 
-        # Annotations only needed for "positive" image set
-        if self.split == "positive":
-            # Download annotations
-            download_url(
-                self.target_meta["url"],
-                os.path.join(self.root, "NWPU VHR-10 dataset"),
-                self.target_meta["filename"],
-                self.target_meta["md5"] if self.checksum else None,
-            )
+        return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/openbuildings.py` & `torchgeo-0.4.0/torchgeo/datasets/openbuildings.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 """Open Buildings datasets."""
 
 import glob
 import json
 import os
 import sys
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, cast
 
 import fiona
 import fiona.transform
 import matplotlib.pyplot as plt
 import rasterio
 import shapely
 import shapely.wkt as wkt
 import torch
-from packaging.version import parse
 from rasterio.crs import CRS
 from rtree.index import Index, Property
 
 from .geo import VectorDataset
 from .utils import BoundingBox, check_integrity
 
 
@@ -303,15 +302,15 @@
             sample of image/mask and metadata for the given query. If there are
             not matching shapes found within the query, an empty raster is returned
 
         Raises:
             IndexError: if query is not found in the index
         """
         hits = self.index.intersection(tuple(query), objects=True)
-        filepaths = [hit.object for hit in hits]
+        filepaths = cast(List[str], [hit.object for hit in hits])
 
         if not filepaths:
             raise IndexError(
                 f"query: {query} not found in index with bounds: {self.bounds}"
             )
 
         shapes = self._filter_geometries(query, filepaths)
@@ -383,15 +382,15 @@
             transformed geometry in geojson format
 
         """
         x = json.dumps(shapely.geometry.mapping(wkt.loads(x)))
         x = json.loads(x.replace("'", '"'))
         import fiona
 
-        if parse(fiona.__version__) >= parse("1.9a1"):
+        if hasattr(fiona, "model"):
             import fiona.model
 
             geom = fiona.model.Geometry(**x)
         else:
             geom = x
         transformed: Dict[str, Any] = fiona.transform.transform_geom(
             self._source_crs.to_dict(), self._crs.to_dict(), geom
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/oscd.py` & `torchgeo-0.4.0/torchgeo/datasets/oscd.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             data and label at that index
         """
         files = self.files[index]
         image1 = self._load_image(files["images1"])
         image2 = self._load_image(files["images2"])
         mask = self._load_target(str(files["mask"]))
 
-        image = torch.stack(tensors=[image1, image2], dim=0)
+        image = torch.cat([image1, image2])
         sample = {"image": image, "mask": mask}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
@@ -302,15 +302,17 @@
                 torch.from_numpy(rgb_img),
                 sample["mask"],
                 alpha=alpha,
                 colors=self.colormap,
             )
             return array
 
-        image1, image2 = get_masked(sample["image"][0]), get_masked(sample["image"][1])
+        idx = sample["image"].shape[0] // 2
+        image1 = get_masked(sample["image"][:idx])
+        image2 = get_masked(sample["image"][idx:])
         fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
         axs[0].imshow(image1)
         axs[0].axis("off")
         axs[1].imshow(image2)
         axs[1].axis("off")
 
         if show_titles:
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/patternnet.py` & `torchgeo-0.4.0/torchgeo/datasets/patternnet.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/potsdam.py` & `torchgeo-0.4.0/torchgeo/datasets/ucmerced.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,293 +1,244 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""Potsdam dataset."""
-
+"""UC Merced dataset."""
 import os
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, Optional, cast
 
 import matplotlib.pyplot as plt
 import numpy as np
-import rasterio
-import torch
-from matplotlib.figure import Figure
-from PIL import Image
 from torch import Tensor
 
-from .geo import NonGeoDataset
-from .utils import (
-    check_integrity,
-    draw_semantic_segmentation_masks,
-    extract_archive,
-    rgb_to_mask,
-)
-
-
-class Potsdam2D(NonGeoDataset):
-    """Potsdam 2D Semantic Segmentation dataset.
-
-    The `Potsdam <https://www2.isprs.org/commissions/comm2/wg4/benchmark/2d-sem-label-potsdam/>`__
-    dataset is a dataset for urban semantic segmentation used in the 2D Semantic Labeling
-    Contest - Potsdam. This dataset uses the "4_Ortho_RGBIR.zip" and "5_Labels_all.zip"
-    files to create the train/test sets used in the challenge. The dataset can be
-    requested at the challenge homepage. Note, the server contains additional data
-    for 3D Semantic Labeling which are currently not supported.
+from .geo import NonGeoClassificationDataset
+from .utils import check_integrity, download_url, extract_archive
+
+
+class UCMerced(NonGeoClassificationDataset):
+    """UC Merced dataset.
 
-    Dataset format:
+    The `UC Merced <http://weegee.vision.ucmerced.edu/datasets/landuse.html>`__
+    dataset is a land use classification dataset of 2.1k 256x256 1ft resolution RGB
+    images of urban locations around the U.S. extracted from the USGS National Map Urban
+    Area Imagery collection with 21 land use classes (100 images per class).
 
-    * images are 4-channel geotiffs
-    * masks are 3-channel geotiffs with unique RGB values representing the class
+    Dataset features:
+
+    * land use class labels from around the U.S.
+    * three spectral bands - RGB
+    * 21 classes
 
     Dataset classes:
 
-    0. Clutter/background
-    1. Impervious surfaces
-    2. Building
-    3. Low Vegetation
-    4. Tree
-    5. Car
+    * agricultural
+    * airplane
+    * baseballdiamond
+    * beach
+    * buildings
+    * chaparral
+    * denseresidential
+    * forest
+    * freeway
+    * golfcourse
+    * harbor
+    * intersection
+    * mediumresidential
+    * mobilehomepark
+    * overpass
+    * parkinglot
+    * river
+    * runway
+    * sparseresidential
+    * storagetanks
+    * tenniscourt
+
+    This dataset uses the train/val/test splits defined in the "In-domain representation
+    learning for remote sensing" paper:
+
+    * https://arxiv.org/abs/1911.06721
 
     If you use this dataset in your research, please cite the following paper:
 
-    * https://doi.org/10.5194/isprsannals-I-3-293-2012
+    * https://dl.acm.org/doi/10.1145/1869790.1869829
+    """
 
-    .. versionadded:: 0.2
-    """  # noqa: E501
+    url = "http://weegee.vision.ucmerced.edu/datasets/UCMerced_LandUse.zip"  # 318 MB
+    filename = "UCMerced_LandUse.zip"
+    md5 = "5b7ec56793786b6dc8a908e8854ac0e4"
 
-    filenames = ["4_Ortho_RGBIR.zip", "5_Labels_all.zip"]
-    md5s = ["c4a8f7d8c7196dd4eba4addd0aae10c1", "cf7403c1a97c0d279414db"]
-    image_root = "4_Ortho_RGBIR"
-    splits = {
-        "train": [
-            "top_potsdam_2_10",
-            "top_potsdam_2_11",
-            "top_potsdam_2_12",
-            "top_potsdam_3_10",
-            "top_potsdam_3_11",
-            "top_potsdam_3_12",
-            "top_potsdam_4_10",
-            "top_potsdam_4_11",
-            "top_potsdam_4_12",
-            "top_potsdam_5_10",
-            "top_potsdam_5_11",
-            "top_potsdam_5_12",
-            "top_potsdam_6_10",
-            "top_potsdam_6_11",
-            "top_potsdam_6_12",
-            "top_potsdam_6_7",
-            "top_potsdam_6_8",
-            "top_potsdam_6_9",
-            "top_potsdam_7_10",
-            "top_potsdam_7_11",
-            "top_potsdam_7_12",
-            "top_potsdam_7_7",
-            "top_potsdam_7_8",
-            "top_potsdam_7_9",
-        ],
-        "test": [
-            "top_potsdam_5_15",
-            "top_potsdam_6_15",
-            "top_potsdam_6_13",
-            "top_potsdam_3_13",
-            "top_potsdam_4_14",
-            "top_potsdam_6_14",
-            "top_potsdam_5_14",
-            "top_potsdam_2_13",
-            "top_potsdam_4_15",
-            "top_potsdam_2_14",
-            "top_potsdam_5_13",
-            "top_potsdam_4_13",
-            "top_potsdam_3_14",
-            "top_potsdam_7_13",
-        ],
-    }
+    base_dir = os.path.join("UCMerced_LandUse", "Images")
     classes = [
-        "Clutter/background",
-        "Impervious surfaces",
-        "Building",
-        "Low Vegetation",
-        "Tree",
-        "Car",
-    ]
-    colormap = [
-        (255, 0, 0),
-        (255, 255, 255),
-        (0, 0, 255),
-        (0, 255, 255),
-        (0, 255, 0),
-        (255, 255, 0),
+        "agricultural",
+        "airplane",
+        "baseballdiamond",
+        "beach",
+        "buildings",
+        "chaparral",
+        "denseresidential",
+        "forest",
+        "freeway",
+        "golfcourse",
+        "harbor",
+        "intersection",
+        "mediumresidential",
+        "mobilehomepark",
+        "overpass",
+        "parkinglot",
+        "river",
+        "runway",
+        "sparseresidential",
+        "storagetanks",
+        "tenniscourt",
     ]
 
+    splits = ["train", "val", "test"]
+    split_urls = {
+        "train": "https://storage.googleapis.com/remote_sensing_representations/uc_merced-train.txt",  # noqa: E501
+        "val": "https://storage.googleapis.com/remote_sensing_representations/uc_merced-val.txt",  # noqa: E501
+        "test": "https://storage.googleapis.com/remote_sensing_representations/uc_merced-test.txt",  # noqa: E501
+    }
+    split_md5s = {
+        "train": "f2fb12eb2210cfb53f93f063a35ff374",
+        "val": "11ecabfc52782e5ea6a9c7c0d263aca0",
+        "test": "046aff88472d8fc07c4678d03749e28d",
+    }
+
     def __init__(
         self,
         root: str = "data",
         split: str = "train",
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
+        download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new Potsdam dataset instance.
+        """Initialize a new UC Merced dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            split: one of "train" or "test"
+            split: one of "train", "val", or "test"
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
+            download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
+
+        Raises:
+            RuntimeError: if ``download=False`` and data is not found, or checksums
+                don't match
         """
         assert split in self.splits
         self.root = root
-        self.split = split
         self.transforms = transforms
+        self.download = download
         self.checksum = checksum
-
         self._verify()
 
-        self.files = []
-        for name in self.splits[split]:
-            image = os.path.join(root, self.image_root, name) + "_RGBIR.tif"
-            mask = os.path.join(root, name) + "_label.tif"
-            if os.path.exists(image) and os.path.exists(mask):
-                self.files.append(dict(image=image, mask=mask))
-
-    def __getitem__(self, index: int) -> Dict[str, Tensor]:
-        """Return an index within the dataset.
-
-        Args:
-            index: index to return
-
-        Returns:
-            data and label at that index
-        """
-        image = self._load_image(index)
-        mask = self._load_target(index)
-        sample = {"image": image, "mask": mask}
-
-        if self.transforms is not None:
-            sample = self.transforms(sample)
-
-        return sample
-
-    def __len__(self) -> int:
-        """Return the number of data points in the dataset.
-
-        Returns:
-            length of the dataset
-        """
-        return len(self.files)
-
-    def _load_image(self, index: int) -> Tensor:
-        """Load a single image.
-
-        Args:
-            index: index to return
-
-        Returns:
-            the image
-        """
-        path = self.files[index]["image"]
-        with rasterio.open(path) as f:
-            array = f.read()
-            tensor = torch.from_numpy(array)
-            return tensor
-
-    def _load_target(self, index: int) -> Tensor:
-        """Load the target mask for a single image.
+        valid_fns = set()
+        with open(os.path.join(self.root, f"uc_merced-{split}.txt")) as f:
+            for fn in f:
+                valid_fns.add(fn.strip())
+        is_in_split: Callable[[str], bool] = lambda x: os.path.basename(x) in valid_fns
+
+        super().__init__(
+            root=os.path.join(root, self.base_dir),
+            transforms=transforms,
+            is_valid_file=is_in_split,
+        )
 
-        Args:
-            index: index to return
+    def _check_integrity(self) -> bool:
+        """Check integrity of dataset.
 
         Returns:
-            the target mask
+            True if dataset files are found and/or MD5s match, else False
         """
-        path = self.files[index]["mask"]
-        with Image.open(path) as img:
-            array: "np.typing.NDArray[np.uint8]" = np.array(img.convert("RGB"))
-            array = rgb_to_mask(array, self.colormap)
-            tensor = torch.from_numpy(array)
-            # Convert from HxWxC to CxHxW
-            tensor = tensor.to(torch.long)
-        return tensor
+        integrity: bool = check_integrity(
+            os.path.join(self.root, self.filename), self.md5 if self.checksum else None
+        )
+        return integrity
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
-            RuntimeError: if checksum fails or the dataset is not downloaded
+            RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
         # Check if the files already exist
-        if os.path.exists(os.path.join(self.root, self.image_root)):
+        filepath = os.path.join(self.root, self.base_dir)
+        if os.path.exists(filepath):
             return
 
-        # Check if .zip files already exists (if so extract)
-        exists = []
-        for filename, md5 in zip(self.filenames, self.md5s):
-            filepath = os.path.join(self.root, filename)
-            if os.path.isfile(filepath):
-                if self.checksum and not check_integrity(filepath, md5):
-                    raise RuntimeError("Dataset found, but corrupted.")
-                exists.append(True)
-                extract_archive(filepath)
-            else:
-                exists.append(False)
-
-        if all(exists):
+        # Check if zip file already exists (if so then extract)
+        if self._check_integrity():
+            self._extract()
             return
 
         # Check if the user requested to download the dataset
-        raise RuntimeError(
-            "Dataset not found in `root` directory, either specify a different"
-            + " `root` directory or manually download the dataset to this directory."
+        if not self.download:
+            raise RuntimeError(
+                "Dataset not found in `root` directory and `download=False`, "
+                "either specify a different `root` directory or use `download=True` "
+                "to automatically download the dataset."
+            )
+
+        # Download and extract the dataset
+        self._download()
+        self._extract()
+
+    def _download(self) -> None:
+        """Download the dataset."""
+        download_url(
+            self.url,
+            self.root,
+            filename=self.filename,
+            md5=self.md5 if self.checksum else None,
         )
+        for split in self.splits:
+            download_url(
+                self.split_urls[split],
+                self.root,
+                filename=f"uc_merced-{split}.txt",
+                md5=self.split_md5s[split] if self.checksum else None,
+            )
+
+    def _extract(self) -> None:
+        """Extract the dataset."""
+        filepath = os.path.join(self.root, self.filename)
+        extract_archive(filepath)
 
     def plot(
         self,
         sample: Dict[str, Tensor],
         show_titles: bool = True,
         suptitle: Optional[str] = None,
-        alpha: float = 0.5,
-    ) -> Figure:
+    ) -> plt.Figure:
         """Plot a sample from the dataset.
 
         Args:
-            sample: a sample returned by :meth:`__getitem__`
+            sample: a sample returned by :meth:`NonGeoClassificationDataset.__getitem__`
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional string to use as a suptitle
-            alpha: opacity with which to render predictions on top of the imagery
 
         Returns:
             a matplotlib Figure with the rendered sample
-        """
-        ncols = 1
-        image1 = draw_semantic_segmentation_masks(
-            sample["image"][:3], sample["mask"], alpha=alpha, colors=self.colormap
-        )
-        if "prediction" in sample:
-            ncols += 1
-            image2 = draw_semantic_segmentation_masks(
-                sample["image"][:3],
-                sample["prediction"],
-                alpha=alpha,
-                colors=self.colormap,
-            )
-
-        fig, axs = plt.subplots(ncols=ncols, figsize=(ncols * 10, 10))
-        if ncols > 1:
-            (ax0, ax1) = axs
-        else:
-            ax0 = axs
-
-        ax0.imshow(image1)
-        ax0.axis("off")
-        if ncols > 1:
-            ax1.imshow(image2)
-            ax1.axis("off")
 
+        .. versionadded:: 0.2
+        """
+        image = np.rollaxis(sample["image"].numpy(), 0, 3)
+        label = cast(int, sample["label"].item())
+        label_class = self.classes[label]
+
+        showing_predictions = "prediction" in sample
+        if showing_predictions:
+            prediction = cast(int, sample["prediction"].item())
+            prediction_class = self.classes[prediction]
+
+        fig, ax = plt.subplots(figsize=(4, 4))
+        ax.imshow(image)
+        ax.axis("off")
         if show_titles:
-            ax0.set_title("Ground Truth")
-            if ncols > 1:
-                ax1.set_title("Predictions")
+            title = f"Label: {label_class}"
+            if showing_predictions:
+                title += f"\nPrediction: {prediction_class}"
+            ax.set_title(title)
 
         if suptitle is not None:
             plt.suptitle(suptitle)
-
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/reforestree.py` & `torchgeo-0.4.0/torchgeo/datasets/reforestree.py`

 * *Files identical despite different names*

### Comparing `torchgeo-0.3.1/torchgeo/datasets/resisc45.py` & `torchgeo-0.4.0/torchgeo/datasets/usavars.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,284 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""RESISC45 dataset."""
+"""USAVars dataset."""
 
+import glob
 import os
-from typing import Callable, Dict, Optional, cast
+from typing import Callable, Dict, List, Optional, Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
+import rasterio
+import torch
+from matplotlib.figure import Figure
 from torch import Tensor
 
-from .geo import NonGeoClassificationDataset
+from .geo import NonGeoDataset
 from .utils import download_url, extract_archive
 
 
-class RESISC45(NonGeoClassificationDataset):
-    """RESISC45 dataset.
+class USAVars(NonGeoDataset):
+    """USAVars dataset.
 
-    The `RESISC45 <http://www.escience.cn/people/JunweiHan/NWPU-RESISC45.html>`__
-    dataset is a dataset for remote sensing image scene classification.
-
-    Dataset features:
-
-    * 31,500 images with 0.2-30 m per pixel resolution (256x256 px)
-    * three spectral bands - RGB
-    * 45 scene classes, 700 images per class
-    * images extracted from Google Earth from over 100 countries
-    * images conditions with high variability (resolution, weather, illumination)
+    The USAVars dataset is reproduction of the dataset used in the paper "`A
+    generalizable and accessible approach to machine learning with global satellite
+    imagery <https://doi.org/10.1038/s41467-021-24638-z>`_". Specifically, this dataset
+    includes 1 sq km. crops of NAIP imagery resampled to 4m/px cenetered on ~100k points
+    that are sampled randomly from the contiguous states in the USA. Each point contains
+    three continuous valued labels (taken from the dataset released in the paper): tree
+    cover percentage, elevation, and population density.
 
     Dataset format:
+    * images are 4-channel GeoTIFFs
+    * labels are singular float values
 
-    * images are three-channel jpgs
-
-    Dataset classes:
-
-    0. airplane
-    1. airport
-    2. baseball_diamond
-    3. basketball_court
-    4. beach
-    5. bridge
-    6. chaparral
-    7. church
-    8. circular_farmland
-    9. cloud
-    10. commercial_area
-    11. dense_residential
-    12. desert
-    13. forest
-    14. freeway
-    15. golf_course
-    16. ground_track_field
-    17. harbor
-    18. industrial_area
-    19. intersection
-    20. island
-    21. lake
-    22. meadow
-    23. medium_residential
-    24. mobile_home_park
-    25. mountain
-    26. overpass
-    27. palace
-    28. parking_lot
-    29. railway
-    30. railway_station
-    31. rectangular_farmland
-    32. river
-    33. roundabout
-    34. runway
-    35. sea_ice
-    36. ship
-    37. snowberg
-    38. sparse_residential
-    39. stadium
-    40. storage_tank
-    41. tennis_court
-    42. terrace
-    43. thermal_power_station
-    44. wetland
-
-    This dataset uses the train/val/test splits defined in the "In-domain representation
-    learning for remote sensing" paper:
-
-    * https://arxiv.org/abs/1911.06721
+    Dataset labels:
+    * tree cover
+    * elevation
+    * population density
 
     If you use this dataset in your research, please cite the following paper:
 
-    * https://doi.org/10.1109/jproc.2017.2675998
+    * https://doi.org/10.1038/s41467-021-24638-z
 
+    .. versionadded:: 0.3
     """
 
-    url = "https://drive.google.com/file/d/1DnPSU5nVSN7xv95bpZ3XQ0JhKXZOKgIv"
-    md5 = "d824acb73957502b00efd559fc6cfbbb"
-    filename = "NWPU-RESISC45.rar"
-    directory = "NWPU-RESISC45"
-
-    splits = ["train", "val", "test"]
-    split_urls = {
-        "train": "https://storage.googleapis.com/remote_sensing_representations/resisc45-train.txt",  # noqa: E501
-        "val": "https://storage.googleapis.com/remote_sensing_representations/resisc45-val.txt",  # noqa: E501
-        "test": "https://storage.googleapis.com/remote_sensing_representations/resisc45-test.txt",  # noqa: E501
+    url_prefix = (
+        "https://files.codeocean.com/files/verified/"
+        + "fa908bbc-11f9-4421-8bd3-72a4bf00427f_v2.0/data/int/applications"
+    )
+    pop_csv_suffix = "CONTUS_16_640_POP_100000_0.csv?download"
+    uar_csv_suffix = "CONTUS_16_640_UAR_100000_0.csv?download"
+
+    data_url = "https://mosaiks.blob.core.windows.net/datasets/uar.zip"
+    dirname = "uar"
+
+    md5 = "677e89fd20e5dd0fe4d29b61827c2456"
+
+    label_urls = {
+        "housing": f"{url_prefix}/housing/outcomes_sampled_housing_{pop_csv_suffix}",
+        "income": f"{url_prefix}/income/outcomes_sampled_income_{pop_csv_suffix}",
+        "roads": f"{url_prefix}/roads/outcomes_sampled_roads_{pop_csv_suffix}",
+        "nightlights": f"{url_prefix}/nightlights/"
+        + f"outcomes_sampled_nightlights_{pop_csv_suffix}",
+        "population": f"{url_prefix}/population/"
+        + f"outcomes_sampled_population_{uar_csv_suffix}",
+        "elevation": f"{url_prefix}/elevation/"
+        + f"outcomes_sampled_elevation_{uar_csv_suffix}",
+        "treecover": f"{url_prefix}/treecover/"
+        + f"outcomes_sampled_treecover_{uar_csv_suffix}",
     }
-    split_md5s = {
-        "train": "b5a4c05a37de15e4ca886696a85c403e",
-        "val": "a0770cee4c5ca20b8c32bbd61e114805",
-        "test": "3dda9e4988b47eb1de9f07993653eb08",
+
+    split_metadata = {
+        "train": {
+            "url": "https://mosaiks.blob.core.windows.net/datasets/train_split.txt",
+            "filename": "train_split.txt",
+            "md5": "3f58fffbf5fe177611112550297200e7",
+        },
+        "val": {
+            "url": "https://mosaiks.blob.core.windows.net/datasets/val_split.txt",
+            "filename": "val_split.txt",
+            "md5": "bca7183b132b919dec0fc24fb11662a0",
+        },
+        "test": {
+            "url": "https://mosaiks.blob.core.windows.net/datasets/test_split.txt",
+            "filename": "test_split.txt",
+            "md5": "97bb36bc003ae0bf556a8d6e8f77141a",
+        },
     }
-    classes = [
-        "airplane",
-        "airport",
-        "baseball_diamond",
-        "basketball_court",
-        "beach",
-        "bridge",
-        "chaparral",
-        "church",
-        "circular_farmland",
-        "cloud",
-        "commercial_area",
-        "dense_residential",
-        "desert",
-        "forest",
-        "freeway",
-        "golf_course",
-        "ground_track_field",
-        "harbor",
-        "industrial_area",
-        "intersection",
-        "island",
-        "lake",
-        "meadow",
-        "medium_residential",
-        "mobile_home_park",
-        "mountain",
-        "overpass",
-        "palace",
-        "parking_lot",
-        "railway",
-        "railway_station",
-        "rectangular_farmland",
-        "river",
-        "roundabout",
-        "runway",
-        "sea_ice",
-        "ship",
-        "snowberg",
-        "sparse_residential",
-        "stadium",
-        "storage_tank",
-        "tennis_court",
-        "terrace",
-        "thermal_power_station",
-        "wetland",
-    ]
+
+    ALL_LABELS = list(label_urls.keys())
 
     def __init__(
         self,
         root: str = "data",
         split: str = "train",
+        labels: Sequence[str] = ALL_LABELS,
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new RESISC45 dataset instance.
+        """Initialize a new USAVars dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            split: one of "train", "val", or "test"
+            split: train/val/test split to load
+            labels: list of labels to include
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
             download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
+
+        Raises:
+            AssertionError: if invalid labels are provided
+            ImportError: if pandas is not installed
+            RuntimeError: if ``download=False`` and data is not found, or checksums
+                don't match
         """
-        assert split in self.splits
         self.root = root
+
+        assert split in self.split_metadata
+        self.split = split
+
+        for lab in labels:
+            assert lab in self.ALL_LABELS
+
+        self.labels = labels
+        self.transforms = transforms
         self.download = download
         self.checksum = checksum
+
         self._verify()
 
-        valid_fns = set()
-        with open(os.path.join(self.root, f"resisc45-{split}.txt")) as f:
-            for fn in f:
-                valid_fns.add(fn.strip())
-        is_in_split: Callable[[str], bool] = lambda x: os.path.basename(x) in valid_fns
-
-        super().__init__(
-            root=os.path.join(root, self.directory),
-            transforms=transforms,
-            is_valid_file=is_in_split,
-        )
+        try:
+            import pandas as pd  # noqa: F401
+        except ImportError:
+            raise ImportError(
+                "pandas is not installed and is required to use this dataset"
+            )
+
+        self.files = self._load_files()
+
+        self.label_dfs = {
+            lab: pd.read_csv(os.path.join(self.root, lab + ".csv"), index_col="ID")
+            for lab in self.labels
+        }
+
+    def __getitem__(self, index: int) -> Dict[str, Tensor]:
+        """Return an index within the dataset.
+
+        Args:
+            index: index to return
+
+        Returns:
+            data and label at that index
+        """
+        tif_file = self.files[index]
+        id_ = tif_file[5:-4]
+
+        sample = {
+            "labels": Tensor(
+                [self.label_dfs[lab].loc[id_][lab] for lab in self.labels]
+            ),
+            "image": self._load_image(os.path.join(self.root, "uar", tif_file)),
+        }
+
+        if self.transforms is not None:
+            sample = self.transforms(sample)
+
+        return sample
+
+    def __len__(self) -> int:
+        """Return the number of data points in the dataset.
+
+        Returns:
+            length of the dataset
+        """
+        return len(self.files)
+
+    def _load_files(self) -> List[str]:
+        """Loads file names."""
+        with open(os.path.join(self.root, f"{self.split}_split.txt")) as f:
+            files = f.read().splitlines()
+        return files
+
+    def _load_image(self, path: str) -> Tensor:
+        """Load a single image.
+
+        Args:
+            path: path to the image
+
+        Returns:
+            the image
+        """
+        with rasterio.open(path) as f:
+            array: "np.typing.NDArray[np.int_]" = f.read()
+            tensor = torch.from_numpy(array)
+            return tensor
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
-        # Check if the files already exist
-        filepath = os.path.join(self.root, self.directory)
-        if os.path.exists(filepath):
+        # Check if the extracted files already exist
+        pathname = os.path.join(self.root, "uar")
+        csv_pathname = os.path.join(self.root, "*.csv")
+        split_pathname = os.path.join(self.root, "*_split.txt")
+
+        csv_split_count = (len(glob.glob(csv_pathname)), len(glob.glob(split_pathname)))
+        if glob.glob(pathname) and csv_split_count == (7, 3):
             return
 
-        # Check if zip file already exists (if so then extract)
-        filepath = os.path.join(self.root, self.filename)
-        if os.path.exists(filepath):
+        # Check if the zip files have already been downloaded
+        pathname = os.path.join(self.root, self.dirname + ".zip")
+        if glob.glob(pathname) and csv_split_count == (7, 3):
             self._extract()
             return
 
         # Check if the user requested to download the dataset
         if not self.download:
             raise RuntimeError(
-                "Dataset not found in `root` directory and `download=False`, "
+                f"Dataset not found in `root={self.root}` and `download=False`, "
                 "either specify a different `root` directory or use `download=True` "
                 "to automatically download the dataset."
             )
 
-        # Download and extract the dataset
         self._download()
         self._extract()
 
     def _download(self) -> None:
         """Download the dataset."""
-        download_url(
-            self.url,
-            self.root,
-            filename=self.filename,
-            md5=self.md5 if self.checksum else None,
-        )
-        for split in self.splits:
+        for f_name in self.label_urls:
+            download_url(self.label_urls[f_name], self.root, filename=f_name + ".csv")
+
+        download_url(self.data_url, self.root, md5=self.md5 if self.checksum else None)
+
+        for metadata in self.split_metadata.values():
             download_url(
-                self.split_urls[split],
+                metadata["url"],
                 self.root,
-                filename=f"resisc45-{split}.txt",
-                md5=self.split_md5s[split] if self.checksum else None,
+                md5=metadata["md5"] if self.checksum else None,
             )
 
     def _extract(self) -> None:
         """Extract the dataset."""
-        filepath = os.path.join(self.root, self.filename)
-        extract_archive(filepath)
+        extract_archive(os.path.join(self.root, self.dirname + ".zip"))
 
     def plot(
         self,
         sample: Dict[str, Tensor],
-        show_titles: bool = True,
+        show_labels: bool = True,
         suptitle: Optional[str] = None,
-    ) -> plt.Figure:
+    ) -> Figure:
         """Plot a sample from the dataset.
 
         Args:
-            sample: a sample returned by :meth:`NonGeoClassificationDataset.__getitem__`
-            show_titles: flag indicating whether to show titles above each panel
+            sample: a sample returned by :meth:`__getitem__`
+            show_labels: flag indicating whether to show labels above panel
             suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
-
-        .. versionadded:: 0.2
         """
-        image = np.rollaxis(sample["image"].numpy(), 0, 3)
-        label = cast(int, sample["label"].item())
-        label_class = self.classes[label]
-
-        showing_predictions = "prediction" in sample
-        if showing_predictions:
-            prediction = cast(int, sample["prediction"].item())
-            prediction_class = self.classes[prediction]
-
-        fig, ax = plt.subplots(figsize=(4, 4))
-        ax.imshow(image)
-        ax.axis("off")
-        if show_titles:
-            title = f"Label: {label_class}"
-            if showing_predictions:
-                title += f"\nPrediction: {prediction_class}"
-            ax.set_title(title)
+        image = sample["image"][:3].numpy()  # get RGB inds
+        image = np.moveaxis(image, 0, 2)
+
+        fig, axs = plt.subplots(figsize=(10, 10))
+        axs.imshow(image)
+        axs.axis("off")
+
+        if show_labels:
+            labels = [(lab, val) for lab, val in sample.items() if lab != "image"]
+            label_string = ""
+            for lab, val in labels:
+                label_string += f"{lab}={round(val[0].item(), 2)} "
+            axs.set_title(label_string)
 
         if suptitle is not None:
             plt.suptitle(suptitle)
+
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/seco.py` & `torchgeo-0.4.0/torchgeo/datasets/so2sat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,241 +1,285 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""Sentinel 2 imagery from the Seasonal Contrast paper."""
+"""So2Sat dataset."""
 
 import os
-from collections import defaultdict
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Dict, Optional, Sequence, cast
 
 import matplotlib.pyplot as plt
 import numpy as np
-import rasterio
 import torch
-from PIL import Image
 from torch import Tensor
 
 from .geo import NonGeoDataset
-from .utils import download_url, extract_archive, percentile_normalization
+from .utils import check_integrity, percentile_normalization
 
 
-class SeasonalContrastS2(NonGeoDataset):
-    """Sentinel 2 imagery from the Seasonal Contrast paper.
+class So2Sat(NonGeoDataset):
+    """So2Sat dataset.
 
-    The `Seasonal Contrast imagery <https://github.com/ElementAI/seasonal-contrast/>`_
-    dataset contains Sentinel 2 imagery patches sampled from different points in time
-    around the 10k most populated cities on Earth.
+    The `So2Sat <https://doi.org/10.1109/MGRS.2020.2964708>`__ dataset consists of
+    corresponding synthetic aperture radar and multispectral optical image data
+    acquired by the Sentinel-1 and Sentinel-2 remote sensing satellites, and a
+    corresponding local climate zones (LCZ) label. The dataset is distributed over
+    42 cities across different continents and cultural regions of the world, and comes
+    with a split into fully independent, non-overlapping training, validation,
+    and test sets.
+
+    This implementation focuses on the *2nd* version of the dataset as described in
+    the author's github repository https://github.com/zhu-xlab/So2Sat-LCZ42 and hosted
+    at https://mediatum.ub.tum.de/1483140. This version is identical to the first
+    version of the dataset but includes the test data. The splits are defined as
+    follows:
+
+    * Training: 42 cities around the world
+    * Validation: western half of 10 other cities covering 10 cultural zones
+    * Testing: eastern half of the 10 other cities
+
+    Dataset classes:
+
+    0. Compact high rise
+    1. Compact middle rise
+    2. Compact low rise
+    3. Open high rise
+    4. Open mid rise
+    5. Open low rise
+    6. Lightweight low rise
+    7. Large low rise
+    8. Sparsely built
+    9. Heavy industry
+    10. Dense trees
+    11. Scattered trees
+    12. Bush, scrub
+    13. Low plants
+    14. Bare rock or paved
+    15. Bare soil or sand
+    16. Water
 
-    Dataset features:
+    If you use this dataset in your research, please cite the following paper:
 
-    * Two versions: 100K and 1M patches
-    * 12 band Sentinel 2 imagery from 5 points in time at each location
+    * https://doi.org/10.1109/MGRS.2020.2964708
 
-    If you use this dataset in your research, please cite the following paper:
+    .. note::
 
-    * https://arxiv.org/pdf/2103.16607.pdf
-    """
+       This dataset can be automatically downloaded using the following bash script:
 
-    ALL_BANDS = [
-        "B1",
-        "B2",
-        "B3",
-        "B4",
-        "B5",
-        "B6",
-        "B7",
-        "B8",
-        "B8A",
-        "B9",
-        "B11",
-        "B12",
-    ]
-    RGB_BANDS = ["B4", "B3", "B2"]
+       .. code-block:: bash
+
+          for split in training validation testing
+          do
+              wget ftp://m1483140:m1483140@dataserv.ub.tum.de/$split.h5
+          done
 
-    urls = {
-        # 7.3 GB
-        "100k": "https://zenodo.org/record/4728033/files/seco_100k.zip?download=1",
-        # 36.3 GB
-        "1m": "https://zenodo.org/record/4728033/files/seco_1m.zip?download=1",
+       or manually downloaded from https://dataserv.ub.tum.de/index.php/s/m1483140
+       This download will likely take several hours.
+    """
+
+    filenames = {
+        "train": "training.h5",
+        "validation": "validation.h5",
+        "test": "testing.h5",
     }
-    filenames = {"100k": "seco_100k.zip", "1m": "seco_1m.zip"}
     md5s = {
-        "100k": "ebf2d5e03adc6e657f9a69a20ad863e0",
-        "1m": "187963d852d4d3ce6637743ec3a4bd9e",
+        "train": "702bc6a9368ebff4542d791e53469244",
+        "validation": "71cfa6795de3e22207229d06d6f8775d",
+        "test": "e81426102b488623a723beab52b31a8a",
+    }
+    classes = [
+        "Compact high rise",
+        "Compact mid rise",
+        "Compact low rise",
+        "Open high rise",
+        "Open mid rise",
+        "Open low rise",
+        "Lightweight low rise",
+        "Large low rise",
+        "Sparsely built",
+        "Heavy industry",
+        "Dense trees",
+        "Scattered trees",
+        "Bush, scrub",
+        "Low plants",
+        "Bare rock or paved",
+        "Bare soil or sand",
+        "Water",
+    ]
+
+    all_s1_band_names = (
+        "S1_B1",
+        "S1_B2",
+        "S1_B3",
+        "S1_B4",
+        "S1_B5",
+        "S1_B6",
+        "S1_B7",
+        "S1_B8",
+    )
+    all_s2_band_names = (
+        "S2_B02",
+        "S2_B03",
+        "S2_B04",
+        "S2_B05",
+        "S2_B06",
+        "S2_B07",
+        "S2_B08",
+        "S2_B8A",
+        "S2_B11",
+        "S2_B12",
+    )
+    all_band_names = all_s1_band_names + all_s2_band_names
+
+    rgb_bands = ["S2_B04", "S2_B03", "S2_B02"]
+
+    BAND_SETS = {
+        "all": all_band_names,
+        "s1": all_s1_band_names,
+        "s2": all_s2_band_names,
     }
-    directory_names = {"100k": "seasonal_contrast_100k", "1m": "seasonal_contrast_1m"}
 
     def __init__(
         self,
         root: str = "data",
-        version: str = "100k",
-        bands: List[str] = RGB_BANDS,
+        split: str = "train",
+        bands: Sequence[str] = BAND_SETS["all"],
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
-        download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new SeCo dataset instance.
+        """Initialize a new So2Sat dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            version: one of "100k" or "1m" for the version of the dataset to use
+            split: one of "train", "validation", or "test"
+            bands: a sequence of band names to use where the indices correspond to the
+                array index of combined Sentinel 1 and Sentinel 2
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
-            download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
 
         Raises:
-            AssertionError: if ``version`` argument is invalid
-            RuntimeError: if ``download=False`` and data is not found, or checksums
-                don't match
+            AssertionError: if ``split`` argument is invalid
+            RuntimeError: if data is not found in ``root``, or checksums don't match
+
+        .. versionadded:: 0.3
+           The *bands* parameter.
         """
-        assert version in ["100k", "1m"]
-        for band in bands:
-            assert band in self.ALL_BANDS
+        try:
+            import h5py  # noqa: F401
+        except ImportError:
+            raise ImportError(
+                "h5py is not installed and is required to use this dataset"
+            )
+
+        assert split in ["train", "validation", "test"]
+
+        self._validate_bands(bands)
+        self.s1_band_indices: "np.typing.NDArray[np.int_]" = np.array(
+            [
+                self.all_s1_band_names.index(b)
+                for b in bands
+                if b in self.all_s1_band_names
+            ]
+        ).astype(int)
+
+        self.s1_band_names = [self.all_s1_band_names[i] for i in self.s1_band_indices]
+
+        self.s2_band_indices: "np.typing.NDArray[np.int_]" = np.array(
+            [
+                self.all_s2_band_names.index(b)
+                for b in bands
+                if b in self.all_s2_band_names
+            ]
+        ).astype(int)
+
+        self.s2_band_names = [self.all_s2_band_names[i] for i in self.s2_band_indices]
 
-        self.root = root
         self.bands = bands
-        self.url = self.urls[version]
-        self.filename = self.filenames[version]
-        self.md5 = self.md5s[version]
-        self.directory_name = self.directory_names[version]
+
+        self.root = root
+        self.split = split
         self.transforms = transforms
-        self.download = download
         self.checksum = checksum
 
-        self._verify()
+        self.fn = os.path.join(self.root, self.filenames[split])
 
-        # TODO: This is slow, I think this should be generated on download and then
-        # loaded in the constructor
-        self.scene_to_patches = defaultdict(list)
-        for root_directory, directories, fns in os.walk(
-            os.path.join(self.root, self.directory_name)
-        ):
-            if len(directories) == 0 and len(fns) > 0:
-                root_directory, patch_name = os.path.split(root_directory)
-                _, scene_name = os.path.split(root_directory)
-                self.scene_to_patches[scene_name].append(patch_name)
-
-        self.scenes = sorted(self.scene_to_patches.keys())
-        for scene_name in self.scenes:
-            self.scene_to_patches[scene_name] = sorted(
-                self.scene_to_patches[scene_name]
-            )
+        if not self._check_integrity():
+            raise RuntimeError("Dataset not found or corrupted.")
+
+        with h5py.File(self.fn, "r") as f:
+            self.size: int = f["label"].shape[0]
 
     def __getitem__(self, index: int) -> Dict[str, Tensor]:
         """Return an index within the dataset.
 
         Args:
             index: index to return
 
         Returns:
-            sample with an "image" in 5xCxHxW format where the 5 indexes over the same
-                patch sampled from different points in time by the SeCo method
+            data and label at that index
         """
-        scene_name = self.scenes[index]
-        patch_names = self.scene_to_patches[scene_name]
+        import h5py
+
+        with h5py.File(self.fn, "r") as f:
+            s1 = f["sen1"][index].astype(np.float64)  # convert from <f8 to float64
+            s1 = np.take(s1, indices=self.s1_band_indices, axis=2)
+            s2 = f["sen2"][index].astype(np.float64)  # convert from <f8 to float64
+            s2 = np.take(s2, indices=self.s2_band_indices, axis=2)
 
-        imagery = [
-            self._load_patch(scene_name, patch_name) for patch_name in patch_names
-        ]
+            # convert one-hot encoding to int64 then torch int
+            label = torch.tensor(f["label"][index].argmax())
 
-        sample = {"image": torch.stack(imagery, dim=0)}
+            s1 = np.rollaxis(s1, 2, 0)  # convert to CxHxW format
+            s2 = np.rollaxis(s2, 2, 0)  # convert to CxHxW format
+
+            s1 = torch.from_numpy(s1)
+            s2 = torch.from_numpy(s2)
+
+        sample = {"image": torch.cat([s1, s2]).float(), "label": label}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
 
         Returns:
             length of the dataset
         """
-        return len(self.scenes)
+        return self.size
 
-    def _load_patch(self, scene_name: str, patch_name: str) -> Tensor:
-        """Load a single image patch.
-
-        Args:
-            scene_name: the name of the scene to load from, e.g. '019999'
-            patch_name: the name of the patch to load, e.g.
-                '20200713T075609_20200713T081050_T36QZH'
+    def _check_integrity(self) -> bool:
+        """Check integrity of dataset.
 
         Returns:
-            the image with the subset of bands specified by ``self.bands``
+            True if dataset files are found and/or MD5s match, else False
         """
-        all_data = []
-        for band in self.bands:
-            fn = os.path.join(
-                self.root, self.directory_name, scene_name, patch_name, f"{band}.tif"
-            )
-            with rasterio.open(fn) as f:
-                band_data = f.read(1)
-                height, width = band_data.shape
-                size = min(height, width)
-                if size < 264:
-                    # TODO: PIL resize is much slower than cv2, we should check to see
-                    # what could be sped up throughout later. There is also a potential
-                    # slowdown here from converting to/from a PIL Image just to resize.
-                    # https://gist.github.com/calebrob6/748045ac8d844154067b2eefa47de92f
-                    pil_image = Image.fromarray(band_data)
-                    # Moved in PIL 9.1.0
-                    try:
-                        resample = Image.Resampling.BILINEAR
-                    except AttributeError:
-                        resample = Image.BILINEAR
-                    band_data = np.array(
-                        pil_image.resize((264, 264), resample=resample)
-                    )
-                all_data.append(band_data)
-        image = torch.from_numpy(np.stack(all_data, axis=0))
-        return image
+        md5 = self.md5s[self.split]
+        if not check_integrity(self.fn, md5 if self.checksum else None):
+            return False
+        return True
+
+    def _validate_bands(self, bands: Sequence[str]) -> None:
+        """Validate list of bands.
 
-    def _verify(self) -> None:
-        """Verify the integrity of the dataset.
+        Args:
+            bands: user-provided sequence of bands to load
 
         Raises:
-            RuntimeError: if ``download=False`` but dataset is missing or checksum fails
-        """
-        # Check if the extracted files already exist
-        directory_path = os.path.join(self.root, self.directory_name)
-        if os.path.exists(directory_path):
-            return
-
-        # Check if the zip files have already been downloaded
-        zip_path = os.path.join(self.root, self.filename)
-        if os.path.exists(zip_path):
-            self._extract()
-            return
-
-        # Check if the user requested to download the dataset
-        if not self.download:
-            raise RuntimeError(
-                f"Dataset not found in `root={self.root}` and `download=False`, "
-                "either specify a different `root` directory or use `download=True` "
-                "to automatically download the dataset."
-            )
+            AssertionError: if ``bands`` is not a sequence
+            ValueError: if an invalid band name is provided
 
-        # Download the dataset
-        self._download()
-        self._extract()
-
-    def _download(self) -> None:
-        """Download the dataset."""
-        download_url(
-            self.url,
-            self.root,
-            filename=self.filename,
-            md5=self.md5 if self.checksum else None,
-        )
-
-    def _extract(self) -> None:
-        """Extract the dataset."""
-        extract_archive(os.path.join(self.root, self.filename))
+        .. versionadded:: 0.3
+        """
+        assert isinstance(bands, Sequence), "'bands' must be a sequence"
+        for band in bands:
+            if band not in self.all_band_names:
+                raise ValueError(f"'{band}' is an invalid band name.")
 
     def plot(
         self,
         sample: Dict[str, Tensor],
         show_titles: bool = True,
         suptitle: Optional[str] = None,
     ) -> plt.Figure:
@@ -246,38 +290,43 @@
             show_titles: flag indicating whether to show titles above each panel
             suptitle: optional string to use as a suptitle
 
         Returns:
             a matplotlib Figure with the rendered sample
 
         Raises:
-            ValueError: if the RGB bands are included in ``self.bands`` or the sample
-                contains a "prediction" key
+            ValueError: if RGB bands are not found in dataset
 
         .. versionadded:: 0.2
         """
-        if "prediction" in sample:
-            raise ValueError("This dataset doesn't support plotting predictions")
-
         rgb_indices = []
-        for band in self.RGB_BANDS:
-            if band in self.bands:
-                rgb_indices.append(self.bands.index(band))
+        for band in self.rgb_bands:
+            if band in self.s2_band_names:
+                idx = self.s2_band_names.index(band) + len(self.s1_band_names)
+                rgb_indices.append(idx)
             else:
                 raise ValueError("Dataset doesn't contain some of the RGB bands")
 
-        images = []
-        for i in range(5):
-            image = np.rollaxis(sample["image"][i, rgb_indices].numpy(), 0, 3)
-            image = percentile_normalization(image, 0, 100)
-            images.append(image)
-
-        fig, axs = plt.subplots(ncols=5, figsize=(20, 4))
-        for i in range(5):
-            axs[i].imshow(images[i])
-            axs[i].axis("off")
-            if show_titles:
-                axs[i].set_title(f"t={i+1}")
+        image = np.take(sample["image"].numpy(), indices=rgb_indices, axis=0)
+        image = np.rollaxis(image, 0, 3)
+        image = percentile_normalization(image, 0, 100)
+
+        label = cast(int, sample["label"].item())
+        label_class = self.classes[label]
+
+        showing_predictions = "prediction" in sample
+        if showing_predictions:
+            prediction = cast(int, sample["prediction"].item())
+            prediction_class = self.classes[prediction]
+
+        fig, ax = plt.subplots(figsize=(4, 4))
+        ax.imshow(image)
+        ax.axis("off")
+        if show_titles:
+            title = f"Label: {label_class}"
+            if showing_predictions:
+                title += f"\nPrediction: {prediction_class}"
+            ax.set_title(title)
 
         if suptitle is not None:
             plt.suptitle(suptitle)
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/sen12ms.py` & `torchgeo-0.4.0/torchgeo/datasets/sen12ms.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         "B8A",
         "B09",
         "B10",
         "B11",
         "B12",
     )
 
-    RGB_BANDS = ["B04", "B03", "B02"]
+    rgb_bands = ["B04", "B03", "B02"]
 
     filenames = [
         "ROIs1158_spring_lc.tar.gz",
         "ROIs1158_spring_s1.tar.gz",
         "ROIs1158_spring_s2.tar.gz",
         "ROIs1868_summer_lc.tar.gz",
         "ROIs1868_summer_s1.tar.gz",
@@ -219,22 +219,22 @@
             index: index to return
 
         Returns:
             data and label at that index
         """
         filename = self.ids[index]
 
-        lc = self._load_raster(filename, "lc")
+        lc = self._load_raster(filename, "lc").long()
         s1 = self._load_raster(filename, "s1")
         s2 = self._load_raster(filename, "s2")
 
         image = torch.cat(tensors=[s1, s2], dim=0)
         image = torch.index_select(image, dim=0, index=self.band_indices)
 
-        sample: Dict[str, Tensor] = {"image": image, "mask": lc}
+        sample: Dict[str, Tensor] = {"image": image, "mask": lc[0]}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
@@ -326,27 +326,27 @@
 
         Returns:
             a matplotlib Figure with the rendered sample
 
         .. versionadded:: 0.2
         """
         rgb_indices = []
-        for band in self.RGB_BANDS:
+        for band in self.rgb_bands:
             if band in self.bands:
                 rgb_indices.append(self.bands.index(band))
             else:
                 raise ValueError("Dataset doesn't contain some of the RGB bands")
 
-        image, mask = sample["image"][rgb_indices].numpy(), sample["mask"][0]
+        image, mask = sample["image"][rgb_indices].numpy(), sample["mask"]
         image = percentile_normalization(image)
         ncols = 2
 
         showing_predictions = "prediction" in sample
         if showing_predictions:
-            prediction = sample["prediction"][0]
+            prediction = sample["prediction"]
             ncols += 1
 
         fig, axs = plt.subplots(nrows=1, ncols=ncols, figsize=(10, ncols * 5))
 
         axs[0].imshow(np.transpose(image, (1, 2, 0)))
         axs[0].axis("off")
         axs[1].imshow(mask)
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/so2sat.py` & `torchgeo-0.4.0/torchgeo/trainers/detection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,327 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""So2Sat dataset."""
+"""Detection tasks."""
 
-import os
-from typing import Callable, Dict, Optional, Sequence, cast
+from functools import partial
+from typing import Any, Dict, List, cast
 
 import matplotlib.pyplot as plt
-import numpy as np
+import pytorch_lightning as pl
 import torch
 from torch import Tensor
+from torch.optim.lr_scheduler import ReduceLROnPlateau
+from torchmetrics.detection.mean_ap import MeanAveragePrecision
+from torchvision.models import resnet as R
+from torchvision.models.detection import FCOS, FasterRCNN, RetinaNet
+from torchvision.models.detection.backbone_utils import resnet_fpn_backbone
+from torchvision.models.detection.retinanet import RetinaNetHead
+from torchvision.models.detection.rpn import AnchorGenerator
+from torchvision.ops import MultiScaleRoIAlign, feature_pyramid_network, misc
+
+from ..datasets.utils import unbind_samples
+
+BACKBONE_LAT_DIM_MAP = {
+    "resnet18": 512,
+    "resnet34": 512,
+    "resnet50": 2048,
+    "resnet101": 2048,
+    "resnet152": 2048,
+    "resnext50_32x4d": 2048,
+    "resnext101_32x8d": 2048,
+    "wide_resnet50_2": 2048,
+    "wide_resnet101_2": 2048,
+}
+
+BACKBONE_WEIGHT_MAP = {
+    "resnet18": R.ResNet18_Weights.DEFAULT,
+    "resnet34": R.ResNet34_Weights.DEFAULT,
+    "resnet50": R.ResNet50_Weights.DEFAULT,
+    "resnet101": R.ResNet101_Weights.DEFAULT,
+    "resnet152": R.ResNet152_Weights.DEFAULT,
+    "resnext50_32x4d": R.ResNeXt50_32X4D_Weights.DEFAULT,
+    "resnext101_32x8d": R.ResNeXt101_32X8D_Weights.DEFAULT,
+    "wide_resnet50_2": R.Wide_ResNet50_2_Weights.DEFAULT,
+    "wide_resnet101_2": R.Wide_ResNet101_2_Weights.DEFAULT,
+}
+
+
+class ObjectDetectionTask(pl.LightningModule):
+    """LightningModule for object detection of images.
+
+    Currently, supports Faster R-CNN, FCOS, and RetinaNet models from
+    `torchvision
+    <https://pytorch.org/vision/stable/models.html
+    #object-detection-instance-segmentation-and-person-keypoint-detection>`_ with
+    one of the following *backbone* arguments:
+
+    .. code-block:: python
+
+        ['resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152',
+        'resnext50_32x4d','resnext101_32x8d', 'wide_resnet50_2',
+        'wide_resnet101_2']
 
-from .geo import NonGeoDataset
-from .utils import check_integrity, percentile_normalization
+    .. versionadded:: 0.4
+    """
 
+    def config_task(self) -> None:
+        """Configures the task based on kwargs parameters passed to the constructor."""
+        backbone_pretrained = self.hyperparams.get("pretrained", True)
+
+        if self.hyperparams["backbone"] in BACKBONE_LAT_DIM_MAP:
+            kwargs = {
+                "backbone_name": self.hyperparams["backbone"],
+                "trainable_layers": self.hyperparams.get("trainable_layers", 3),
+            }
+            if backbone_pretrained:
+                kwargs["weights"] = BACKBONE_WEIGHT_MAP[self.hyperparams["backbone"]]
+            else:
+                kwargs["weights"] = None
 
-class So2Sat(NonGeoDataset):
-    """So2Sat dataset.
+            latent_dim = BACKBONE_LAT_DIM_MAP[self.hyperparams["backbone"]]
+        else:
+            raise ValueError(
+                f"Backbone type '{self.hyperparams['backbone']}' is not valid."
+            )
 
-    The `So2Sat <https://doi.org/10.1109/MGRS.2020.2964708>`__ dataset consists of
-    corresponding synthetic aperture radar and multispectral optical image data
-    acquired by the Sentinel-1 and Sentinel-2 remote sensing satellites, and a
-    corresponding local climate zones (LCZ) label. The dataset is distributed over
-    42 cities across different continents and cultural regions of the world, and comes
-    with a split into fully independent, non-overlapping training, validation,
-    and test sets.
-
-    This implementation focuses on the *2nd* version of the dataset as described in
-    the author's github repository https://github.com/zhu-xlab/So2Sat-LCZ42 and hosted
-    at https://mediatum.ub.tum.de/1483140. This version is identical to the first
-    version of the dataset but includes the test data. The splits are defined as
-    follows:
-
-    * Training: 42 cities around the world
-    * Validation: western half of 10 other cities covering 10 cultural zones
-    * Testing: eastern half of the 10 other cities
-
-    Dataset classes:
-
-    0. Compact high rise
-    1. Compact middle rise
-    2. Compact low rise
-    3. Open high rise
-    4. Open mid rise
-    5. Open low rise
-    6. Lightweight low rise
-    7. Large low rise
-    8. Sparsely built
-    9. Heavy industry
-    10. Dense trees
-    11. Scattered trees
-    12. Bush, scrub
-    13. Low plants
-    14. Bare rock or paved
-    15. Bare soil or sand
-    16. Water
-
-    If you use this dataset in your research, please cite the following paper:
-
-    * https://doi.org/10.1109/MGRS.2020.2964708
-
-    .. note::
-
-       This dataset can be automatically downloaded using the following bash script:
-
-       .. code-block:: bash
-
-          for split in training validation testing
-          do
-              wget ftp://m1483140:m1483140@dataserv.ub.tum.de/$split.h5
-          done
+        num_classes = self.hyperparams["num_classes"]
 
-       or manually downloaded from https://dataserv.ub.tum.de/index.php/s/m1483140
-       This download will likely take several hours.
-    """
+        if self.hyperparams["model"] == "faster-rcnn":
+            backbone = resnet_fpn_backbone(**kwargs)
+            anchor_generator = AnchorGenerator(
+                sizes=((32), (64), (128), (256), (512)), aspect_ratios=((0.5, 1.0, 2.0))
+            )
 
-    filenames = {
-        "train": "training.h5",
-        "validation": "validation.h5",
-        "test": "testing.h5",
-    }
-    md5s = {
-        "train": "702bc6a9368ebff4542d791e53469244",
-        "validation": "71cfa6795de3e22207229d06d6f8775d",
-        "test": "e81426102b488623a723beab52b31a8a",
-    }
-    classes = [
-        "Compact high rise",
-        "Compact mid rise",
-        "Compact low rise",
-        "Open high rise",
-        "Open mid rise",
-        "Open low rise",
-        "Lightweight low rise",
-        "Large low rise",
-        "Sparsely built",
-        "Heavy industry",
-        "Dense trees",
-        "Scattered trees",
-        "Bush, scrub",
-        "Low plants",
-        "Bare rock or paved",
-        "Bare soil or sand",
-        "Water",
-    ]
-
-    all_s1_band_names = ("S1B1", "S1B2", "S1B3", "S1B4", "S1B5", "S1B6", "S1B7", "S1B8")
-    all_s2_band_names = (
-        "B02",
-        "B03",
-        "B04",
-        "B05",
-        "B06",
-        "B07",
-        "B08",
-        "B08A",
-        "B11 SWIR",
-        "B12 SWIR",
-    )
-    all_band_names = all_s1_band_names + all_s2_band_names
-
-    RGB_BANDS = ["B04", "B03", "B02"]
-
-    BAND_SETS = {
-        "all": all_band_names,
-        "s1": all_s1_band_names,
-        "s2": all_s2_band_names,
-    }
-
-    def __init__(
-        self,
-        root: str = "data",
-        split: str = "train",
-        bands: Sequence[str] = BAND_SETS["all"],
-        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
-        checksum: bool = False,
-    ) -> None:
-        """Initialize a new So2Sat dataset instance.
+            roi_pooler = MultiScaleRoIAlign(
+                featmap_names=["0", "1", "2", "3"], output_size=7, sampling_ratio=2
+            )
+            self.model = FasterRCNN(
+                backbone,
+                num_classes,
+                rpn_anchor_generator=anchor_generator,
+                box_roi_pool=roi_pooler,
+            )
+        elif self.hyperparams["model"] == "fcos":
+            kwargs["extra_blocks"] = feature_pyramid_network.LastLevelP6P7(256, 256)
+            kwargs["norm_layer"] = (
+                misc.FrozenBatchNorm2d if kwargs["weights"] else torch.nn.BatchNorm2d
+            )
 
-        Args:
-            root: root directory where dataset can be found
-            split: one of "train", "validation", or "test"
-            bands: a sequence of band names to use where the indices correspond to the
-                array index of combined Sentinel 1 and Sentinel 2
-            transforms: a function/transform that takes input sample and its target as
-                entry and returns a transformed version
-            checksum: if True, check the MD5 of the downloaded files (may be slow)
+            backbone = resnet_fpn_backbone(**kwargs)
+            anchor_generator = AnchorGenerator(
+                sizes=((8,), (16,), (32,), (64,), (128,), (256,)),
+                aspect_ratios=((1.0,), (1.0,), (1.0,), (1.0,), (1.0,), (1.0,)),
+            )
 
-        Raises:
-            AssertionError: if ``split`` argument is invalid
-            RuntimeError: if data is not found in ``root``, or checksums don't match
+            self.model = FCOS(backbone, num_classes, anchor_generator=anchor_generator)
 
-        .. versionadded:: 0.3
-           The *bands* parameter.
-        """
-        try:
-            import h5py  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "h5py is not installed and is required to use this dataset"
+        elif self.hyperparams["model"] == "retinanet":
+            kwargs["extra_blocks"] = feature_pyramid_network.LastLevelP6P7(
+                latent_dim, 256
             )
+            backbone = resnet_fpn_backbone(**kwargs)
 
-        assert split in ["train", "validation", "test"]
+            anchor_sizes = (
+                (16, 20, 25),
+                (32, 40, 50),
+                (64, 80, 101),
+                (128, 161, 203),
+                (256, 322, 406),
+                (512, 645, 812),
+            )
+            aspect_ratios = ((0.5, 1.0, 2.0),) * len(anchor_sizes)
+            anchor_generator = AnchorGenerator(anchor_sizes, aspect_ratios)
 
-        self._validate_bands(bands)
-        self.s1_band_indices: "np.typing.NDArray[np.int_]" = np.array(
-            [
-                self.all_s1_band_names.index(b)
-                for b in bands
-                if b in self.all_s1_band_names
-            ]
-        ).astype(int)
-
-        self.s1_band_names = [self.all_s1_band_names[i] for i in self.s1_band_indices]
-
-        self.s2_band_indices: "np.typing.NDArray[np.int_]" = np.array(
-            [
-                self.all_s2_band_names.index(b)
-                for b in bands
-                if b in self.all_s2_band_names
-            ]
-        ).astype(int)
-
-        self.s2_band_names = [self.all_s2_band_names[i] for i in self.s2_band_indices]
-
-        self.bands = bands
-
-        self.root = root
-        self.split = split
-        self.transforms = transforms
-        self.checksum = checksum
-
-        self.fn = os.path.join(self.root, self.filenames[split])
+            head = RetinaNetHead(
+                backbone.out_channels,
+                anchor_generator.num_anchors_per_location()[0],
+                num_classes,
+                norm_layer=partial(torch.nn.GroupNorm, 32),
+            )
 
-        if not self._check_integrity():
-            raise RuntimeError("Dataset not found or corrupted.")
+            self.model = RetinaNet(
+                backbone, num_classes, anchor_generator=anchor_generator, head=head
+            )
+        else:
+            raise ValueError(f"Model type '{self.hyperparams['model']}' is not valid.")
 
-        with h5py.File(self.fn, "r") as f:
-            self.size: int = f["label"].shape[0]
+    def __init__(self, **kwargs: Any) -> None:
+        """Initialize the LightningModule with a model and loss function.
 
-    def __getitem__(self, index: int) -> Dict[str, Tensor]:
-        """Return an index within the dataset.
+        Keyword Args:
+            model: Name of the detection model type to use
+            backbone: Name of the model backbone to use
+            in_channels: Number of channels in input image
+            num_classes: Number of semantic classes to predict
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
 
-        Args:
-            index: index to return
+        Raises:
+            ValueError: if kwargs arguments are invalid
 
-        Returns:
-            data and label at that index
+        .. versionchanged:: 0.4
+           The *detection_model* parameter was renamed to *model*.
         """
-        import h5py
-
-        with h5py.File(self.fn, "r") as f:
-            s1 = f["sen1"][index].astype(np.float64)  # convert from <f8 to float64
-            s1 = np.take(s1, indices=self.s1_band_indices, axis=2)
-            s2 = f["sen2"][index].astype(np.float64)  # convert from <f8 to float64
-            s2 = np.take(s2, indices=self.s2_band_indices, axis=2)
+        super().__init__()
+        # Creates `self.hparams` from kwargs
+        self.save_hyperparameters()  # type: ignore[operator]
+        self.hyperparams = cast(Dict[str, Any], self.hparams)
 
-            # convert one-hot encoding to int64 then torch int
-            label = torch.tensor(f["label"][index].argmax())
+        self.config_task()
 
-            s1 = np.rollaxis(s1, 2, 0)  # convert to CxHxW format
-            s2 = np.rollaxis(s2, 2, 0)  # convert to CxHxW format
+        self.val_metrics = MeanAveragePrecision()
+        self.test_metrics = MeanAveragePrecision()
 
-            s1 = torch.from_numpy(s1)
-            s2 = torch.from_numpy(s2)
+    def forward(self, *args: Any, **kwargs: Any) -> Any:
+        """Forward pass of the model.
 
-        sample = {"image": torch.cat([s1, s2]), "label": label}
+        Args:
+            x: tensor of data to run through the model
 
-        if self.transforms is not None:
-            sample = self.transforms(sample)
+        Returns:
+            output from the model
+        """
+        return self.model(*args, **kwargs)
 
-        return sample
+    def training_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the training loss.
 
-    def __len__(self) -> int:
-        """Return the number of data points in the dataset.
+        Args:
+            batch: the output of your DataLoader
 
         Returns:
-            length of the dataset
+            training loss
         """
-        return self.size
+        batch = args[0]
+        x = batch["image"]
+        batch_size = x.shape[0]
+        y = [
+            {"boxes": batch["boxes"][i], "labels": batch["labels"][i]}
+            for i in range(batch_size)
+        ]
+        loss_dict = self(x, y)
+        train_loss = sum(loss_dict.values())
 
-    def _check_integrity(self) -> bool:
-        """Check integrity of dataset.
+        self.log_dict(loss_dict)
 
-        Returns:
-            True if dataset files are found and/or MD5s match, else False
+        return cast(Tensor, train_loss)
+
+    def validation_step(self, *args: Any, **kwargs: Any) -> None:
+        """Compute validation loss and log example predictions.
+
+        Args:
+            batch: the output of your DataLoader
+            batch_idx: the index of this batch
         """
-        md5 = self.md5s[self.split]
-        if not check_integrity(self.fn, md5 if self.checksum else None):
-            return False
-        return True
+        batch = args[0]
+        batch_idx = args[1]
+        x = batch["image"]
+        batch_size = x.shape[0]
+        y = [
+            {"boxes": batch["boxes"][i], "labels": batch["labels"][i]}
+            for i in range(batch_size)
+        ]
+        y_hat = self(x)
+
+        self.val_metrics.update(y_hat, y)
+
+        if (
+            batch_idx < 10
+            and hasattr(self.trainer, "datamodule")
+            and self.logger
+            and hasattr(self.logger, "experiment")
+        ):
+            try:
+                datamodule = self.trainer.datamodule
+                batch["prediction_boxes"] = [b["boxes"].cpu() for b in y_hat]
+                batch["prediction_labels"] = [b["labels"].cpu() for b in y_hat]
+                batch["prediction_scores"] = [b["scores"].cpu() for b in y_hat]
+                batch["image"] = batch["image"].cpu()
+                sample = unbind_samples(batch)[0]
+                # Convert image to uint8 for plotting
+                if torch.is_floating_point(sample["image"]):
+                    sample["image"] *= 255
+                    sample["image"] = sample["image"].to(torch.uint8)
+                fig = datamodule.plot(sample)
+                summary_writer = self.logger.experiment
+                summary_writer.add_figure(
+                    f"image/{batch_idx}", fig, global_step=self.global_step
+                )
+                plt.close()
+            except ValueError:
+                pass
 
-    def _validate_bands(self, bands: Sequence[str]) -> None:
-        """Validate list of bands.
+    def validation_epoch_end(self, outputs: Any) -> None:
+        """Logs epoch level validation metrics.
 
         Args:
-            bands: user-provided sequence of bands to load
+            outputs: list of items returned by validation_step
+        """
+        metrics = self.val_metrics.compute()
+        renamed_metrics = {f"val_{i}": metrics[i] for i in metrics.keys()}
+        self.log_dict(renamed_metrics)
+        self.val_metrics.reset()
 
-        Raises:
-            AssertionError: if ``bands`` is not a sequence
-            ValueError: if an invalid band name is provided
+    def test_step(self, *args: Any, **kwargs: Any) -> None:
+        """Compute test MAP.
+
+        Args:
+            batch: the output of your DataLoader
+        """
+        batch = args[0]
+        x = batch["image"]
+        batch_size = x.shape[0]
+        y = [
+            {"boxes": batch["boxes"][i], "labels": batch["labels"][i]}
+            for i in range(batch_size)
+        ]
+        y_hat = self(x)
+
+        self.test_metrics.update(y_hat, y)
+
+    def test_epoch_end(self, outputs: Any) -> None:
+        """Logs epoch level test metrics.
 
-        .. versionadded:: 0.3
+        Args:
+            outputs: list of items returned by test_step
         """
-        assert isinstance(bands, Sequence), "'bands' must be a sequence"
-        for band in bands:
-            if band not in self.all_band_names:
-                raise ValueError(f"'{band}' is an invalid band name.")
-
-    def plot(
-        self,
-        sample: Dict[str, Tensor],
-        show_titles: bool = True,
-        suptitle: Optional[str] = None,
-    ) -> plt.Figure:
-        """Plot a sample from the dataset.
+        metrics = self.test_metrics.compute()
+        renamed_metrics = {f"test_{i}": metrics[i] for i in metrics.keys()}
+        self.log_dict(renamed_metrics)
+        self.test_metrics.reset()
+
+    def predict_step(self, *args: Any, **kwargs: Any) -> List[Dict[str, Tensor]]:
+        """Compute and return the predictions.
 
         Args:
-            sample: a sample returned by :meth:`__getitem__`
-            show_titles: flag indicating whether to show titles above each panel
-            suptitle: optional string to use as a suptitle
+            batch: the output of your DataLoader
 
         Returns:
-            a matplotlib Figure with the rendered sample
+            list of predicted boxes, labels and scores
+        """
+        batch = args[0]
+        x = batch["image"]
+        y_hat: List[Dict[str, Tensor]] = self(x)
+        return y_hat
 
-        Raises:
-            ValueError: if RGB bands are not found in dataset
+    def configure_optimizers(self) -> Dict[str, Any]:
+        """Initialize the optimizer and learning rate scheduler.
 
-        .. versionadded:: 0.2
+        Returns:
+            a "lr dict" according to the pytorch lightning documentation --
+            https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         """
-        rgb_indices = []
-        for band in self.RGB_BANDS:
-            if band in self.s2_band_names:
-                idx = self.s2_band_names.index(band) + len(self.s1_band_names)
-                rgb_indices.append(idx)
-            else:
-                raise ValueError("Dataset doesn't contain some of the RGB bands")
-
-        image = np.take(sample["image"].numpy(), indices=rgb_indices, axis=0)
-        image = np.rollaxis(image, 0, 3)
-        image = percentile_normalization(image, 0, 100)
-
-        label = cast(int, sample["label"].item())
-        label_class = self.classes[label]
-
-        showing_predictions = "prediction" in sample
-        if showing_predictions:
-            prediction = cast(int, sample["prediction"].item())
-            prediction_class = self.classes[prediction]
-
-        fig, ax = plt.subplots(figsize=(4, 4))
-        ax.imshow(image)
-        ax.axis("off")
-        if show_titles:
-            title = f"Label: {label_class}"
-            if showing_predictions:
-                title += f"\nPrediction: {prediction_class}"
-            ax.set_title(title)
-
-        if suptitle is not None:
-            plt.suptitle(suptitle)
-        return fig
+        optimizer = torch.optim.Adam(
+            self.model.parameters(), lr=self.hyperparams["learning_rate"]
+        )
+        return {
+            "optimizer": optimizer,
+            "lr_scheduler": {
+                "scheduler": ReduceLROnPlateau(
+                    optimizer,
+                    mode="max",
+                    patience=self.hyperparams["learning_rate_schedule_patience"],
+                ),
+                "monitor": "val_map",
+            },
+        }
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/spacenet.py` & `torchgeo-0.4.0/torchgeo/datasets/spacenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,34 @@
 from rasterio.transform import Affine
 from torch import Tensor
 
 from .geo import NonGeoDataset
 from .utils import (
     check_integrity,
     download_radiant_mlhub_collection,
+    download_radiant_mlhub_dataset,
     extract_archive,
     percentile_normalization,
 )
 
 
 class SpaceNet(NonGeoDataset, abc.ABC):
     """Abstract base class for the SpaceNet datasets.
 
     The `SpaceNet <https://spacenet.ai/datasets/>`__ datasets are a set of
     datasets that all together contain >11M building footprints and ~20,000 km
     of road labels mapped over high-resolution satellite imagery obtained from
     a variety of sensors such as Worldview-2, Worldview-3 and Dove.
+
+    .. note::
+
+       The SpaceNet datasets require the following additional library to be installed:
+
+       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
+           imagery and labels from the Radiant Earth MLHub
     """
 
     @property
     @abc.abstractmethod
     def dataset_id(self) -> str:
         """Dataset ID."""
 
@@ -146,15 +154,15 @@
 
         Returns:
             the image
         """
         filename = os.path.join(path)
         with rio.open(filename) as img:
             array = img.read().astype(np.int32)
-            tensor = torch.from_numpy(array)
+            tensor = torch.from_numpy(array).float()
             return tensor, img.transform, img.crs
 
     def _load_mask(
         self, path: str, tfm: Affine, raster_crs: CRS, shape: Tuple[int, int]
     ) -> Tensor:
         """Rasterizes the dataset's labels (in geojson format).
 
@@ -380,32 +388,25 @@
 
         * labels.geojson
 
     If you use this dataset in your research, please cite the following paper:
 
     * https://arxiv.org/abs/1807.01232
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     """
 
     dataset_id = "spacenet1"
     imagery = {"rgb": "RGB.tif", "8band": "8Band.tif"}
     chip_size = {"rgb": (406, 438), "8band": (101, 110)}
     label_glob = "labels.geojson"
     collection_md5_dict = {"sn1_AOI_1_RIO": "e6ea35331636fa0c036c04b3d1cbf226"}
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         image: str = "rgb",
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
     ) -> None:
         """Initialize a new SpaceNet 1 Dataset instance.
@@ -486,21 +487,14 @@
 
         * label.geojson
 
     If you use this dataset in your research, please cite the following paper:
 
     * https://arxiv.org/abs/1807.01232
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     """
 
     dataset_id = "spacenet2"
     collection_md5_dict = {
         "sn2_AOI_2_Vegas": "a5a8de355290783b88ac4d69c7ef0694",
         "sn2_AOI_3_Paris": "8299186b7bbfb9a256d515bad1b7f146",
         "sn2_AOI_4_Shanghai": "4e3e80f2f437faca10ca2e6e6df0ef99",
@@ -519,15 +513,15 @@
         "PS-MS": (650, 650),
         "PS-RGB": (650, 650),
     }
     label_glob = "label.geojson"
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         image: str = "PS-RGB",
         collections: List[str] = [],
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
     ) -> None:
@@ -612,21 +606,14 @@
 
         * labels.geojson
 
     If you use this dataset in your research, please cite the following paper:
 
     * https://arxiv.org/abs/1807.01232
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     .. versionadded:: 0.3
     """
 
     dataset_id = "spacenet3"
     collection_md5_dict = {
         "sn3_AOI_2_Vegas": "8ce7e6abffb8849eb88885035f061ee8",
         "sn3_AOI_3_Paris": "90b9ebd64cd83dc8d3d4773f45050d8f",
@@ -646,15 +633,15 @@
         "PS-MS": (1300, 1300),
         "PS-RGB": (1300, 1300),
     }
     label_glob = "labels.geojson"
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         image: str = "PS-RGB",
         speed_mask: Optional[bool] = False,
         collections: List[str] = [],
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
@@ -849,21 +836,14 @@
 
         * labels.geojson
 
     If you use this dataset in your research, please cite the following paper:
 
     * https://arxiv.org/abs/1903.12239
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     """
 
     dataset_id = "spacenet4"
     collection_md5_dict = {"sn4_AOI_6_Atlanta": "c597d639cba5257927a97e3eff07b753"}
 
     imagery = {"MS": "MS.tif", "PAN": "PAN.tif", "PS-RGBNIR": "PS-RGBNIR.tif"}
     chip_size = {"MS": (225, 225), "PAN": (900, 900), "PS-RGBNIR": (900, 900)}
@@ -903,15 +883,15 @@
             "1030010003CD4300",
             "1030010003193D00",
         ],
     }
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         image: str = "PS-RGBNIR",
         angles: List[str] = [],
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
     ) -> None:
@@ -1046,21 +1026,14 @@
 
     If you use this dataset in your research, please use the following citation:
 
     * The SpaceNet Partners, “SpaceNet5: Automated Road Network Extraction and
       Route Travel Time Estimation from Satellite Imagery”,
       https://spacenet.ai/sn5-challenge/
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     .. versionadded:: 0.2
     """
 
     dataset_id = "spacenet5"
     collection_md5_dict = {
         "sn5_AOI_7_Moscow": "b18107f878152fe7e75444373c320cba",
         "sn5_AOI_8_Mumbai": "1f1e2b3c26fbd15bfbcdbb6b02ae051c",
@@ -1078,15 +1051,15 @@
         "PS-MS": (1300, 1300),
         "PS-RGB": (1300, 1300),
     }
     label_glob = "labels.geojson"
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         image: str = "PS-RGB",
         speed_mask: Optional[bool] = False,
         collections: List[str] = [],
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
@@ -1118,14 +1091,157 @@
             transforms,
             download,
             api_key,
             checksum,
         )
 
 
+class SpaceNet6(SpaceNet):
+    r"""SpaceNet 6: Multi-Sensor All-Weather Mapping.
+
+    `SpaceNet 6 <https://spacenet.ai/sn6-challenge/>`_ is a dataset
+    of optical and SAR imagery over the city of Rotterdam.
+
+    Collection features:
+
+    +------------+---------------------+------------+-----------------------------+
+    |    AOI     | Area (km\ :sup:`2`\)| # Images   | # Building Footprint Labels |
+    +============+=====================+============+=============================+
+    | Rotterdam  |    120              |   3401     |         48000               |
+    +------------+---------------------+------------+-----------------------------+
+
+
+    Imagery features:
+
+    .. list-table::
+        :widths: 10 10 10 10 10 10
+        :header-rows: 1
+        :stub-columns: 1
+
+        *   -
+            - PAN
+            - RGBNIR
+            - PS-RGB
+            - PS-RGBNIR
+            - SAR-Intensity
+        *   - GSD (m)
+            - 0.5
+            - 2.0
+            - 0.5
+            - 0.5
+            - 0.5
+        *   - Chip size (px)
+            - 900 x 900
+            - 450 x 450
+            - 900 x 900
+            - 900 x 900
+            - 900 x 900
+
+
+    Dataset format:
+
+    * Imagery - GeoTIFFs from Worldview-2 (optical) and Capella Space (SAR)
+
+        * PAN.tif (Panchromatic)
+        * RGBNIR.tif (Multispectral)
+        * PS-RGB (Pansharpened RGB)
+        * PS-RGBNIR (Pansharpened RGBNIR)
+        * SAR-Intensity (SAR Intensity)
+
+    * Labels - GeoJSON
+
+        * labels.geojson
+
+    If you use this dataset in your research, please cite the following paper:
+
+    * https://arxiv.org/abs/2004.06500
+
+    .. note::
+
+       This dataset requires the following additional library to be installed:
+
+       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
+         imagery and labels from the Radiant Earth MLHub
+
+    .. versionadded:: 0.4
+    """
+
+    dataset_id = "spacenet6"
+    collections = ["sn6_AOI_11_Rotterdam"]
+    # This is actually the metadata hash
+    collection_md5_dict = {"sn6_AOI_11_Rotterdam": "66f7312218fec67a1e0b3b02b22c95cc"}
+    imagery = {
+        "PAN": "PAN.tif",
+        "RGBNIR": "RGBNIR.tif",
+        "PS-RGB": "PS-RGB.tif",
+        "PS-RGBNIR": "PS-RGBNIR.tif",
+        "SAR-Intensity": "SAR-Intensity.tif",
+    }
+    chip_size = {
+        "PAN": (900, 900),
+        "RGBNIR": (450, 450),
+        "PS-RGB": (900, 900),
+        "PS-RGBNIR": (900, 900),
+        "SAR-Intensity": (900, 900),
+    }
+    label_glob = "labels.geojson"
+
+    def __init__(
+        self,
+        root: str = "data",
+        image: str = "PS-RGB",
+        transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
+        download: bool = False,
+        api_key: Optional[str] = None,
+    ) -> None:
+        """Initialize a new SpaceNet 6 Dataset instance.
+
+        Args:
+            root: root directory where dataset can be found
+            image: image selection which must be in ["PAN", "RGBNIR",
+                "PS-RGB", "PS-RGBNIR", "SAR-Intensity"]
+            transforms: a function/transform that takes input sample and its target as
+                entry and returns a transformed version
+            download: if True, download dataset and store it in the root directory.
+            api_key: a RadiantEarth MLHub API key to use for downloading the dataset
+
+        Raises:
+            RuntimeError: if ``download=False`` but dataset is missing
+        """
+        self.root = root
+        self.image = image  # For testing
+
+        self.filename = self.imagery[image]
+        self.transforms = transforms
+
+        if download:
+            self.__download(api_key)
+
+        self.files = self._load_files(os.path.join(root, self.dataset_id))
+
+    def __download(self, api_key: Optional[str] = None) -> None:
+        """Download the dataset and extract it.
+
+        Args:
+            api_key: a RadiantEarth MLHub API key to use for downloading the dataset
+
+        Raises:
+            RuntimeError: if download doesn't work correctly or checksums don't match
+        """
+        if os.path.exists(
+            os.path.join(
+                self.root, self.dataset_id, self.collections[0], "collection.json"
+            )
+        ):
+            print("Files already downloaded and verified")
+            return
+
+        download_radiant_mlhub_dataset(self.dataset_id, self.root, api_key)
+
+
 class SpaceNet7(SpaceNet):
     """SpaceNet 7: Multi-Temporal Urban Development Challenge.
 
     `SpaceNet 7 <https://spacenet.ai/sn7-challenge/>`_ is a dataset which
     consist of medium resolution (4.0m) satellite imagery mosaics acquired from
     Planet Labs’ Dove constellation between 2017 and 2020. It includes ≈ 24
     images (one per month) covering > 100 unique geographies, and comprises >
@@ -1151,21 +1267,14 @@
 
         * labels.geojson
 
     If you use this dataset in your research, please cite the following paper:
 
     * https://arxiv.org/abs/2102.04420
 
-    .. note::
-
-       This dataset requires the following additional library to be installed:
-
-       * `radiant-mlhub <https://pypi.org/project/radiant-mlhub/>`_ to download the
-         imagery and labels from the Radiant Earth MLHub
-
     .. versionadded:: 0.2
     """
 
     dataset_id = "spacenet7"
     collection_md5_dict = {
         "sn7_train_source": "9f8cc109d744537d087bd6ff33132340",
         "sn7_train_labels": "16f873e3f0f914d95a916fb39b5111b5",
@@ -1175,15 +1284,15 @@
     imagery = {"img": "mosaic.tif"}
     chip_size = {"img": (1023, 1023)}
 
     label_glob = "labels.geojson"
 
     def __init__(
         self,
-        root: str,
+        root: str = "data",
         split: str = "train",
         transforms: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
         download: bool = False,
         api_key: Optional[str] = None,
         checksum: bool = False,
     ) -> None:
         """Initialize a new SpaceNet 7 Dataset instance.
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/usavars.py` & `torchgeo-0.4.0/torchgeo/datasets/zuericrop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,284 +1,323 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""USAVars dataset."""
+"""ZueriCrop dataset."""
 
-import glob
 import os
-from typing import Callable, Dict, List, Optional, Sequence
+from typing import Callable, Dict, Optional, Sequence, Tuple
 
 import matplotlib.pyplot as plt
-import numpy as np
-import rasterio
 import torch
-from matplotlib.figure import Figure
 from torch import Tensor
 
 from .geo import NonGeoDataset
-from .utils import download_url, extract_archive
+from .utils import download_url, percentile_normalization
 
 
-class USAVars(NonGeoDataset):
-    """USAVars dataset.
+class ZueriCrop(NonGeoDataset):
+    """ZueriCrop dataset.
 
-    The USAVars dataset is reproduction of the dataset used in the paper "`A
-    generalizable and accessible approach to machine learning with global satellite
-    imagery <https://doi.org/10.1038/s41467-021-24638-z>`_". Specifically, this dataset
-    includes 1 sq km. crops of NAIP imagery resampled to 4m/px cenetered on ~100k points
-    that are sampled randomly from the contiguous states in the USA. Each point contains
-    three continous valued labels (taken from the dataset released in the paper): tree
-    cover percentage, elevation, and population density.
+    The `ZueriCrop <https://github.com/0zgur0/ms-convSTAR>`__
+    dataset is a dataset for time-series instance segmentation of crops.
+
+    Dataset features:
+
+    * Sentinel-2 multispectral imagery
+    * instance masks of 48 crop categories
+    * nine multispectral bands
+    * 116k images with 10 m per pixel resolution (24x24 px)
+    * ~28k time-series containing 142 images each
 
     Dataset format:
-    * images are 4-channel GeoTIFFs
-    * labels are singular float values
 
-    Dataset labels:
-    * tree cover
-    * elevation
-    * population density
+    * single hdf5 dataset containing images, semantic masks, and instance masks
+    * data is parsed into images and instance masks, boxes, and labels
+    * one mask per time-series
+
+    Dataset classes:
+
+    * 48 fine-grained hierarchical crop
+      `categories <https://github.com/0zgur0/ms-convSTAR/blob/master/labels.csv>`_
 
     If you use this dataset in your research, please cite the following paper:
 
-    * https://doi.org/10.1038/s41467-021-24638-z
+    * https://doi.org/10.1016/j.rse.2021.112603
 
-    .. versionadded:: 0.3
+    .. note::
+
+       This dataset requires the following additional library to be installed:
+
+       * `h5py <https://pypi.org/project/h5py/>`_ to load the dataset
     """
 
-    url_prefix = (
-        "https://files.codeocean.com/files/verified/"
-        + "fa908bbc-11f9-4421-8bd3-72a4bf00427f_v2.0/data/int/applications"
-    )
-    pop_csv_suffix = "CONTUS_16_640_POP_100000_0.csv?download"
-    uar_csv_suffix = "CONTUS_16_640_UAR_100000_0.csv?download"
-
-    data_url = "https://mosaiks.blob.core.windows.net/datasets/uar.zip"
-    dirname = "uar"
-
-    md5 = "677e89fd20e5dd0fe4d29b61827c2456"
-
-    label_urls = {
-        "housing": f"{url_prefix}/housing/outcomes_sampled_housing_{pop_csv_suffix}",
-        "income": f"{url_prefix}/income/outcomes_sampled_income_{pop_csv_suffix}",
-        "roads": f"{url_prefix}/roads/outcomes_sampled_roads_{pop_csv_suffix}",
-        "nightlights": f"{url_prefix}/nightlights/"
-        + f"outcomes_sampled_nightlights_{pop_csv_suffix}",
-        "population": f"{url_prefix}/population/"
-        + f"outcomes_sampled_population_{uar_csv_suffix}",
-        "elevation": f"{url_prefix}/elevation/"
-        + f"outcomes_sampled_elevation_{uar_csv_suffix}",
-        "treecover": f"{url_prefix}/treecover/"
-        + f"outcomes_sampled_treecover_{uar_csv_suffix}",
-    }
-
-    split_metadata = {
-        "train": {
-            "url": "https://mosaiks.blob.core.windows.net/datasets/train_split.txt",
-            "filename": "train_split.txt",
-            "md5": "3f58fffbf5fe177611112550297200e7",
-        },
-        "val": {
-            "url": "https://mosaiks.blob.core.windows.net/datasets/val_split.txt",
-            "filename": "val_split.txt",
-            "md5": "bca7183b132b919dec0fc24fb11662a0",
-        },
-        "test": {
-            "url": "https://mosaiks.blob.core.windows.net/datasets/test_split.txt",
-            "filename": "test_split.txt",
-            "md5": "97bb36bc003ae0bf556a8d6e8f77141a",
-        },
-    }
+    urls = [
+        "https://polybox.ethz.ch/index.php/s/uXfdr2AcXE3QNB6/download",
+        "https://raw.githubusercontent.com/0zgur0/ms-convSTAR/master/labels.csv",
+    ]
+    md5s = ["1635231df67f3d25f4f1e62c98e221a4", "5118398c7a5bbc246f5f6bb35d8d529b"]
+    filenames = ["ZueriCrop.hdf5", "labels.csv"]
 
-    ALL_LABELS = list(label_urls.keys())
+    band_names = ("NIR", "B03", "B02", "B04", "B05", "B06", "B07", "B11", "B12")
+    rgb_bands = ["B04", "B03", "B02"]
 
     def __init__(
         self,
         root: str = "data",
-        split: str = "train",
-        labels: Sequence[str] = ALL_LABELS,
+        bands: Sequence[str] = band_names,
         transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
         download: bool = False,
         checksum: bool = False,
     ) -> None:
-        """Initialize a new USAVars dataset instance.
+        """Initialize a new ZueriCrop dataset instance.
 
         Args:
             root: root directory where dataset can be found
-            split: train/val/test split to load
-            labels: list of labels to include
+            bands: the subset of bands to load
             transforms: a function/transform that takes input sample and its target as
                 entry and returns a transformed version
             download: if True, download dataset and store it in the root directory
             checksum: if True, check the MD5 of the downloaded files (may be slow)
 
         Raises:
-            AssertionError: if invalid labels are provided
-            ImportError: if pandas is not installed
             RuntimeError: if ``download=False`` and data is not found, or checksums
                 don't match
         """
-        self.root = root
-
-        assert split in self.split_metadata
-        self.split = split
+        self._validate_bands(bands)
+        self.band_indices = torch.tensor(
+            [self.band_names.index(b) for b in bands]
+        ).long()
 
-        for lab in labels:
-            assert lab in self.ALL_LABELS
-
-        self.labels = labels
+        self.root = root
+        self.bands = bands
         self.transforms = transforms
         self.download = download
         self.checksum = checksum
+        self.filepath = os.path.join(root, "ZueriCrop.hdf5")
 
         self._verify()
 
         try:
-            import pandas as pd  # noqa: F401
+            import h5py  # noqa: F401
         except ImportError:
             raise ImportError(
-                "pandas is not installed and is required to use this dataset"
+                "h5py is not installed and is required to use this dataset"
             )
 
-        self.files = self._load_files()
-
-        self.label_dfs = {
-            lab: pd.read_csv(os.path.join(self.root, lab + ".csv"), index_col="ID")
-            for lab in self.labels
-        }
-
     def __getitem__(self, index: int) -> Dict[str, Tensor]:
         """Return an index within the dataset.
 
         Args:
             index: index to return
 
         Returns:
-            data and label at that index
+            sample containing image, mask, bounding boxes, and target label
         """
-        tif_file = self.files[index]
-        id_ = tif_file[5:-4]
+        image = self._load_image(index)
+        mask, boxes, label = self._load_target(index)
 
-        sample = {
-            "labels": Tensor(
-                [self.label_dfs[lab].loc[id_][lab] for lab in self.labels]
-            ),
-            "image": self._load_image(os.path.join(self.root, "uar", tif_file)),
-        }
+        sample = {"image": image, "mask": mask, "boxes": boxes, "label": label}
 
         if self.transforms is not None:
             sample = self.transforms(sample)
 
         return sample
 
     def __len__(self) -> int:
         """Return the number of data points in the dataset.
 
         Returns:
             length of the dataset
         """
-        return len(self.files)
+        import h5py
 
-    def _load_files(self) -> List[str]:
-        """Loads file names."""
-        with open(os.path.join(self.root, f"{self.split}_split.txt")) as f:
-            files = f.read().splitlines()
-        return files
+        with h5py.File(self.filepath, "r") as f:
+            length: int = f["data"].shape[0]
+        return length
 
-    def _load_image(self, path: str) -> Tensor:
+    def _load_image(self, index: int) -> Tensor:
         """Load a single image.
 
         Args:
-            path: path to the image
+            index: index to return
 
         Returns:
             the image
         """
-        with rasterio.open(path) as f:
-            array: "np.typing.NDArray[np.int_]" = f.read()
-            tensor = torch.from_numpy(array)
-            return tensor
+        import h5py
+
+        with h5py.File(self.filepath, "r") as f:
+            array = f["data"][index, ...]
+
+        tensor = torch.from_numpy(array)
+        # Convert from TxHxWxC to TxCxHxW
+        tensor = tensor.permute((0, 3, 1, 2))
+        tensor = torch.index_select(tensor, dim=1, index=self.band_indices)
+        return tensor
+
+    def _load_target(self, index: int) -> Tuple[Tensor, Tensor, Tensor]:
+        """Load the target mask for a single image.
+
+        Args:
+            index: index to return
+
+        Returns:
+            the target mask and label for each mask
+        """
+        import h5py
+
+        with h5py.File(self.filepath, "r") as f:
+            mask_array = f["gt"][index, ...]
+            instance_array = f["gt_instance"][index, ...]
+
+        mask_tensor = torch.from_numpy(mask_array)
+        instance_tensor = torch.from_numpy(instance_array)
+
+        # Convert from HxWxC to CxHxW
+        mask_tensor = mask_tensor.permute((2, 0, 1))
+        instance_tensor = instance_tensor.permute((2, 0, 1))
+
+        # Convert instance mask of N instances to N binary instance masks
+        instance_ids = torch.unique(instance_tensor)
+        # Exclude a mask for unknown/background
+        instance_ids = instance_ids[instance_ids != 0]
+        instance_ids = instance_ids[:, None, None]
+        masks = instance_tensor == instance_ids
+
+        # Parse labels for each instance
+        labels_list = []
+        for mask in masks:
+            label = mask_tensor[mask[None, :, :]]
+            label = torch.unique(label)[0]
+            labels_list.append(label)
+
+        # Get bounding boxes for each instance
+        boxes_list = []
+        for mask in masks:
+            pos = torch.where(mask)
+            xmin = torch.min(pos[1])
+            xmax = torch.max(pos[1])
+            ymin = torch.min(pos[0])
+            ymax = torch.max(pos[0])
+            boxes_list.append([xmin, ymin, xmax, ymax])
+
+        masks = masks.to(torch.uint8)
+        boxes = torch.tensor(boxes_list).to(torch.float)
+        labels = torch.tensor(labels_list).to(torch.long)
+
+        return masks, boxes, labels
 
     def _verify(self) -> None:
         """Verify the integrity of the dataset.
 
         Raises:
             RuntimeError: if ``download=False`` but dataset is missing or checksum fails
         """
-        # Check if the extracted files already exist
-        pathname = os.path.join(self.root, "uar")
-        csv_pathname = os.path.join(self.root, "*.csv")
-        split_pathname = os.path.join(self.root, "*_split.txt")
+        # Check if the files already exist
+        exists = []
+        for filename in self.filenames:
+            filepath = os.path.join(self.root, filename)
+            exists.append(os.path.exists(filepath))
 
-        csv_split_count = (len(glob.glob(csv_pathname)), len(glob.glob(split_pathname)))
-        if glob.glob(pathname) and csv_split_count == (7, 3):
-            return
-
-        # Check if the zip files have already been downloaded
-        pathname = os.path.join(self.root, self.dirname + ".zip")
-        if glob.glob(pathname) and csv_split_count == (7, 3):
-            self._extract()
+        if all(exists):
             return
 
         # Check if the user requested to download the dataset
         if not self.download:
             raise RuntimeError(
-                f"Dataset not found in `root={self.root}` and `download=False`, "
+                "Dataset not found in `root` directory and `download=False`, "
                 "either specify a different `root` directory or use `download=True` "
                 "to automatically download the dataset."
             )
 
+        # Download the dataset
         self._download()
-        self._extract()
 
     def _download(self) -> None:
         """Download the dataset."""
-        for f_name in self.label_urls:
-            download_url(self.label_urls[f_name], self.root, filename=f_name + ".csv")
+        for url, filename, md5 in zip(self.urls, self.filenames, self.md5s):
+            filepath = os.path.join(self.root, filename)
+            if not os.path.exists(filepath):
+                download_url(
+                    url,
+                    self.root,
+                    filename=filename,
+                    md5=md5 if self.checksum else None,
+                )
 
-        download_url(self.data_url, self.root, md5=self.md5 if self.checksum else None)
+    def _validate_bands(self, bands: Sequence[str]) -> None:
+        """Validate list of bands.
 
-        for metadata in self.split_metadata.values():
-            download_url(
-                metadata["url"],
-                self.root,
-                md5=metadata["md5"] if self.checksum else None,
-            )
+        Args:
+            bands: user-provided sequence of bands to load
+        Raises:
+            AssertionError: if ``bands`` is not a sequence
+            ValueError: if an invalid band name is provided
 
-    def _extract(self) -> None:
-        """Extract the dataset."""
-        extract_archive(os.path.join(self.root, self.dirname + ".zip"))
+        .. versionadded:: 0.2
+        """
+        assert isinstance(bands, Sequence), "'bands' must be a sequence"
+        for band in bands:
+            if band not in self.band_names:
+                raise ValueError(f"'{band}' is an invalid band name.")
 
     def plot(
         self,
         sample: Dict[str, Tensor],
-        show_labels: bool = True,
+        time_step: int = 0,
+        show_titles: bool = True,
         suptitle: Optional[str] = None,
-    ) -> Figure:
+    ) -> plt.Figure:
         """Plot a sample from the dataset.
 
         Args:
             sample: a sample returned by :meth:`__getitem__`
-            show_labels: flag indicating whether to show labels above panel
-            suptitle: optional string to use as a suptitle
+            time_step: time step at which to access image, beginning with 0
+            show_titles: flag indicating whether to show titles above each panel
+            suptitle: optional suptitle to use for figure
 
         Returns:
             a matplotlib Figure with the rendered sample
-        """
-        image = sample["image"][:3].numpy()  # get RGB inds
-        image = np.moveaxis(image, 0, 2)
 
-        fig, axs = plt.subplots(figsize=(10, 10))
-        axs.imshow(image)
-        axs.axis("off")
-
-        if show_labels:
-            labels = [(lab, val) for lab, val in sample.items() if lab != "image"]
-            label_string = ""
-            for lab, val in labels:
-                label_string += f"{lab}={round(val[0].item(), 2)} "
-            axs.set_title(label_string)
+        .. versionadded:: 0.2
+        """
+        rgb_indices = []
+        for band in self.rgb_bands:
+            if band in self.bands:
+                rgb_indices.append(self.bands.index(band))
+            else:
+                raise ValueError("Dataset doesn't contain some of the RGB bands")
+
+        ncols = 2
+        image, mask = sample["image"][time_step, rgb_indices], sample["mask"]
+
+        image = torch.tensor(
+            percentile_normalization(image.numpy()) * 255, dtype=torch.uint8
+        )
+
+        mask = torch.argmax(mask, dim=0)
+
+        if "prediction" in sample:
+            ncols += 1
+            preds = torch.argmax(sample["prediction"], dim=0)
+
+        fig, axs = plt.subplots(ncols=ncols, figsize=(10, 10 * ncols))
+
+        axs[0].imshow(image.permute(1, 2, 0))
+        axs[0].axis("off")
+        axs[1].imshow(mask)
+        axs[1].axis("off")
+
+        if show_titles:
+            axs[0].set_title("Image")
+            axs[1].set_title("Mask")
+
+        if "prediction" in sample:
+            axs[2].imshow(preds)
+            axs[2].axis("off")
+            if show_titles:
+                axs[2].set_title("Prediction")
 
         if suptitle is not None:
             plt.suptitle(suptitle)
 
         return fig
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/utils.py` & `torchgeo-0.4.0/torchgeo/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,15 +641,15 @@
     Returns:
         a version of ``image`` overlayed with the colors given by ``mask`` and
             ``colors``
     """
     classes = torch.from_numpy(np.arange(len(colors) if colors else 0, dtype=np.uint8))
     class_masks = mask == classes[:, None, None]
     img = draw_segmentation_masks(
-        image=image, masks=class_masks, alpha=alpha, colors=colors
+        image=image.byte(), masks=class_masks, alpha=alpha, colors=colors
     )
     img = img.permute((1, 2, 0)).numpy().astype(np.uint8)
     return cast("np.typing.NDArray[np.uint8]", img)
 
 
 def rgb_to_mask(
     rgb: "np.typing.NDArray[np.uint8]", colors: List[Tuple[int, int, int]]
@@ -700,10 +700,10 @@
 
     .. versionadded:: 0.2
     """
     assert lower < upper
     lower_percentile = np.percentile(img, lower, axis=axis)
     upper_percentile = np.percentile(img, upper, axis=axis)
     img_normalized: "np.typing.NDArray[np.int_]" = np.clip(
-        (img - lower_percentile) / (upper_percentile - lower_percentile), 0, 1
+        (img - lower_percentile) / (upper_percentile - lower_percentile + 1e-5), 0, 1
     )
     return img_normalized
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/vaihingen.py` & `torchgeo-0.4.0/torchgeo/datasets/vaihingen.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,21 @@
     rgb_to_mask,
 )
 
 
 class Vaihingen2D(NonGeoDataset):
     """Vaihingen 2D Semantic Segmentation dataset.
 
-    The `Vaihingen <https://www2.isprs.org/commissions/comm2/wg4/benchmark/2d-sem-label-vaihingen/>`__
+    The `Vaihingen <https://www.isprs.org/education/benchmarks/UrbanSemLab/semantic-labeling.aspx>`__
     dataset is a dataset for urban semantic segmentation used in the 2D Semantic Labeling
     Contest - Vaihingen. This dataset uses the "ISPRS_semantic_labeling_Vaihingen.zip"
     and "ISPRS_semantic_labeling_Vaihingen_ground_truth_COMPLETE.zip" files to create the
-    train/test sets used in the challenge. The dataset can be requested at the challenge
-    homepage. Note, the server contains additional data for 3D Semantic Labeling which
+    train/test sets used in the challenge. The dataset can be downloaded from
+    `here <https://www.isprs.org/education/benchmarks/UrbanSemLab/default.aspx>`__.
+    Note, the server contains additional data for 3D Semantic Labeling which
     are currently not supported.
 
     Dataset format:
 
     * images are 3-channel RGB geotiffs
     * masks are 3-channel geotiffs with unique RGB values representing the class
 
@@ -183,15 +184,15 @@
             the image
         """
         path = self.files[index]["image"]
         with Image.open(path) as img:
             array: "np.typing.NDArray[np.int_]" = np.array(img.convert("RGB"))
             tensor = torch.from_numpy(array)
             # Convert from HxWxC to CxHxW
-            tensor = tensor.permute((2, 0, 1))
+            tensor = tensor.permute((2, 0, 1)).float()
         return tensor
 
     def _load_target(self, index: int) -> Tensor:
         """Load the target mask for a single image.
 
         Args:
             index: index to return
```

### Comparing `torchgeo-0.3.1/torchgeo/datasets/zuericrop.py` & `torchgeo-0.4.0/torchgeo/samplers/single.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,323 +1,323 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-"""ZueriCrop dataset."""
+"""TorchGeo samplers."""
 
-import os
-from typing import Callable, Dict, Optional, Sequence, Tuple
+import abc
+from typing import Callable, Iterable, Iterator, Optional, Tuple, Union
 
-import matplotlib.pyplot as plt
 import torch
-from torch import Tensor
+from rtree.index import Index, Property
+from torch.utils.data import Sampler
 
-from .geo import NonGeoDataset
-from .utils import download_url, percentile_normalization
+from ..datasets import BoundingBox, GeoDataset
+from .constants import Units
+from .utils import _to_tuple, get_random_bounding_box, tile_to_chips
 
 
-class ZueriCrop(NonGeoDataset):
-    """ZueriCrop dataset.
+class GeoSampler(Sampler[BoundingBox], abc.ABC):
+    """Abstract base class for sampling from :class:`~torchgeo.datasets.GeoDataset`.
 
-    The `ZueriCrop <https://github.com/0zgur0/ms-convSTAR>`__
-    dataset is a dataset for time-series instance segmentation of crops.
-
-    Dataset features:
-
-    * Sentinel-2 multispectral imagery
-    * instance masks of 48 crop categories
-    * nine multispectral bands
-    * 116k images with 10 m per pixel resolution (24x24 px)
-    * ~28k time-series containing 142 images each
-
-    Dataset format:
-
-    * single hdf5 dataset containing images, semantic masks, and instance masks
-    * data is parsed into images and instance masks, boxes, and labels
-    * one mask per time-series
+    Unlike PyTorch's :class:`~torch.utils.data.Sampler`, :class:`GeoSampler`
+    returns enough geospatial information to uniquely index any
+    :class:`~torchgeo.datasets.GeoDataset`. This includes things like latitude,
+    longitude, height, width, projection, coordinate system, and time.
+    """
 
-    Dataset classes:
+    def __init__(self, dataset: GeoDataset, roi: Optional[BoundingBox] = None) -> None:
+        """Initialize a new Sampler instance.
 
-    * 48 fine-grained hierarchical crop
-      `categories <https://github.com/0zgur0/ms-convSTAR/blob/master/labels.csv>`_
+        Args:
+            dataset: dataset to index from
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+        """
+        if roi is None:
+            self.index = dataset.index
+            roi = BoundingBox(*self.index.bounds)
+        else:
+            self.index = Index(interleaved=False, properties=Property(dimension=3))
+            hits = dataset.index.intersection(tuple(roi), objects=True)
+            for hit in hits:
+                bbox = BoundingBox(*hit.bounds) & roi
+                self.index.insert(hit.id, tuple(bbox), hit.object)
+
+        self.res = dataset.res
+        self.roi = roi
+
+    @abc.abstractmethod
+    def __iter__(self) -> Iterator[BoundingBox]:
+        """Return the index of a dataset.
 
-    If you use this dataset in your research, please cite the following paper:
+        Returns:
+            (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
+        """
 
-    * https://doi.org/10.1016/j.rse.2021.112603
 
-    .. note::
+class RandomGeoSampler(GeoSampler):
+    """Samples elements from a region of interest randomly.
 
-       This dataset requires the following additional library to be installed:
+    This is particularly useful during training when you want to maximize the size of
+    the dataset and return as many random :term:`chips <chip>` as possible. Note that
+    randomly sampled chips may overlap.
 
-       * `h5py <https://pypi.org/project/h5py/>`_ to load the dataset
+    This sampler is not recommended for use with tile-based datasets. Use
+    :class:`RandomBatchGeoSampler` instead.
     """
 
-    urls = [
-        "https://polybox.ethz.ch/index.php/s/uXfdr2AcXE3QNB6/download",
-        "https://raw.githubusercontent.com/0zgur0/ms-convSTAR/master/labels.csv",
-    ]
-    md5s = ["1635231df67f3d25f4f1e62c98e221a4", "5118398c7a5bbc246f5f6bb35d8d529b"]
-    filenames = ["ZueriCrop.hdf5", "labels.csv"]
-
-    band_names = ("NIR", "B03", "B02", "B04", "B05", "B06", "B07", "B11", "B12")
-    RGB_BANDS = ["B04", "B03", "B02"]
-
     def __init__(
         self,
-        root: str = "data",
-        bands: Sequence[str] = band_names,
-        transforms: Optional[Callable[[Dict[str, Tensor]], Dict[str, Tensor]]] = None,
-        download: bool = False,
-        checksum: bool = False,
+        dataset: GeoDataset,
+        size: Union[Tuple[float, float], float],
+        length: Optional[int],
+        roi: Optional[BoundingBox] = None,
+        units: Units = Units.PIXELS,
     ) -> None:
-        """Initialize a new ZueriCrop dataset instance.
+        """Initialize a new Sampler instance.
 
-        Args:
-            root: root directory where dataset can be found
-            bands: the subset of bands to load
-            transforms: a function/transform that takes input sample and its target as
-                entry and returns a transformed version
-            download: if True, download dataset and store it in the root directory
-            checksum: if True, check the MD5 of the downloaded files (may be slow)
-
-        Raises:
-            RuntimeError: if ``download=False`` and data is not found, or checksums
-                don't match
-        """
-        self._validate_bands(bands)
-        self.band_indices = torch.tensor(
-            [self.band_names.index(b) for b in bands]
-        ).long()
-
-        self.root = root
-        self.bands = bands
-        self.transforms = transforms
-        self.download = download
-        self.checksum = checksum
-        self.filepath = os.path.join(root, "ZueriCrop.hdf5")
-
-        self._verify()
-
-        try:
-            import h5py  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "h5py is not installed and is required to use this dataset"
-            )
+        The ``size`` argument can either be:
 
-    def __getitem__(self, index: int) -> Dict[str, Tensor]:
-        """Return an index within the dataset.
+        * a single ``float`` - in which case the same value is used for the height and
+          width dimension
+        * a ``tuple`` of two floats - in which case, the first *float* is used for the
+          height dimension, and the second *float* for the width dimension
 
-        Args:
-            index: index to return
+        .. versionchanged:: 0.3
+           Added ``units`` parameter, changed default to pixel units
 
-        Returns:
-            sample containing image, mask, bounding boxes, and target label
-        """
-        image = self._load_image(index)
-        mask, boxes, label = self._load_target(index)
+        .. versionchanged:: 0.4
+           ``length`` parameter is now optional, a reasonable default will be used
 
-        sample = {"image": image, "mask": mask, "boxes": boxes, "label": label}
+        Args:
+            dataset: dataset to index from
+            size: dimensions of each :term:`patch`
+            length: number of random samples to draw per epoch
+                (defaults to approximately the maximal number of non-overlapping
+                :term:`chips <chip>` of size ``size`` that could be sampled from
+                the dataset)
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+            units: defines if ``size`` is in pixel or CRS units
+        """
+        super().__init__(dataset, roi)
+        self.size = _to_tuple(size)
 
-        if self.transforms is not None:
-            sample = self.transforms(sample)
+        if units == Units.PIXELS:
+            self.size = (self.size[0] * self.res, self.size[1] * self.res)
 
-        return sample
+        self.length = 0
+        self.hits = []
+        areas = []
+        for hit in self.index.intersection(tuple(self.roi), objects=True):
+            bounds = BoundingBox(*hit.bounds)
+            if (
+                bounds.maxx - bounds.minx >= self.size[1]
+                and bounds.maxy - bounds.miny >= self.size[0]
+            ):
+                if bounds.area > 0:
+                    rows, cols = tile_to_chips(bounds, self.size)
+                    self.length += rows * cols
+                else:
+                    self.length += 1
+                self.hits.append(hit)
+                areas.append(bounds.area)
+        if length is not None:
+            self.length = length
+
+        # torch.multinomial requires float probabilities > 0
+        self.areas = torch.tensor(areas, dtype=torch.float)
+        if torch.sum(self.areas) == 0:
+            self.areas += 1
 
-    def __len__(self) -> int:
-        """Return the number of data points in the dataset.
+    def __iter__(self) -> Iterator[BoundingBox]:
+        """Return the index of a dataset.
 
         Returns:
-            length of the dataset
+            (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
         """
-        import h5py
+        for _ in range(len(self)):
+            # Choose a random tile, weighted by area
+            idx = torch.multinomial(self.areas, 1)
+            hit = self.hits[idx]
+            bounds = BoundingBox(*hit.bounds)
 
-        with h5py.File(self.filepath, "r") as f:
-            length: int = f["data"].shape[0]
-        return length
+            # Choose a random index within that tile
+            bounding_box = get_random_bounding_box(bounds, self.size, self.res)
 
-    def _load_image(self, index: int) -> Tensor:
-        """Load a single image.
+            yield bounding_box
 
-        Args:
-            index: index to return
+    def __len__(self) -> int:
+        """Return the number of samples in a single epoch.
 
         Returns:
-            the image
+            length of the epoch
         """
-        import h5py
+        return self.length
 
-        with h5py.File(self.filepath, "r") as f:
-            array = f["data"][index, ...]
 
-        tensor = torch.from_numpy(array)
-        # Convert from TxHxWxC to TxCxHxW
-        tensor = tensor.permute((0, 3, 1, 2))
-        tensor = torch.index_select(tensor, dim=1, index=self.band_indices)
-        return tensor
+class GridGeoSampler(GeoSampler):
+    """Samples elements in a grid-like fashion.
 
-    def _load_target(self, index: int) -> Tuple[Tensor, Tensor, Tensor]:
-        """Load the target mask for a single image.
+    This is particularly useful during evaluation when you want to make predictions for
+    an entire region of interest. You want to minimize the amount of redundant
+    computation by minimizing overlap between :term:`chips <chip>`.
 
-        Args:
-            index: index to return
+    Usually the stride should be slightly smaller than the chip size such that each chip
+    has some small overlap with surrounding chips. This is used to prevent `stitching
+    artifacts <https://arxiv.org/abs/1805.12219>`_ when combining each prediction patch.
+    The overlap between each chip (``chip_size - stride``) should be approximately equal
+    to the `receptive field <https://distill.pub/2019/computing-receptive-fields/>`_ of
+    the CNN.
 
-        Returns:
-            the target mask and label for each mask
-        """
-        import h5py
+    Note that the stride of the final set of chips in each row/column may be adjusted so
+    that the entire :term:`tile` is sampled without exceeding the bounds of the dataset.
+    """
 
-        with h5py.File(self.filepath, "r") as f:
-            mask_array = f["gt"][index, ...]
-            instance_array = f["gt_instance"][index, ...]
-
-        mask_tensor = torch.from_numpy(mask_array)
-        instance_tensor = torch.from_numpy(instance_array)
-
-        # Convert from HxWxC to CxHxW
-        mask_tensor = mask_tensor.permute((2, 0, 1))
-        instance_tensor = instance_tensor.permute((2, 0, 1))
-
-        # Convert instance mask of N instances to N binary instance masks
-        instance_ids = torch.unique(instance_tensor)
-        # Exclude a mask for unknown/background
-        instance_ids = instance_ids[instance_ids != 0]
-        instance_ids = instance_ids[:, None, None]
-        masks = instance_tensor == instance_ids
-
-        # Parse labels for each instance
-        labels_list = []
-        for mask in masks:
-            label = mask_tensor[mask[None, :, :]]
-            label = torch.unique(label)[0]
-            labels_list.append(label)
-
-        # Get bounding boxes for each instance
-        boxes_list = []
-        for mask in masks:
-            pos = torch.where(mask)
-            xmin = torch.min(pos[1])
-            xmax = torch.max(pos[1])
-            ymin = torch.min(pos[0])
-            ymax = torch.max(pos[0])
-            boxes_list.append([xmin, ymin, xmax, ymax])
-
-        masks = masks.to(torch.uint8)
-        boxes = torch.tensor(boxes_list).to(torch.float)
-        labels = torch.tensor(labels_list).to(torch.long)
-
-        return masks, boxes, labels
-
-    def _verify(self) -> None:
-        """Verify the integrity of the dataset.
-
-        Raises:
-            RuntimeError: if ``download=False`` but dataset is missing or checksum fails
-        """
-        # Check if the files already exist
-        exists = []
-        for filename in self.filenames:
-            filepath = os.path.join(self.root, filename)
-            exists.append(os.path.exists(filepath))
-
-        if all(exists):
-            return
-
-        # Check if the user requested to download the dataset
-        if not self.download:
-            raise RuntimeError(
-                "Dataset not found in `root` directory and `download=False`, "
-                "either specify a different `root` directory or use `download=True` "
-                "to automatically download the dataset."
-            )
-
-        # Download the dataset
-        self._download()
-
-    def _download(self) -> None:
-        """Download the dataset."""
-        for url, filename, md5 in zip(self.urls, self.filenames, self.md5s):
-            filepath = os.path.join(self.root, filename)
-            if not os.path.exists(filepath):
-                download_url(
-                    url,
-                    self.root,
-                    filename=filename,
-                    md5=md5 if self.checksum else None,
-                )
+    def __init__(
+        self,
+        dataset: GeoDataset,
+        size: Union[Tuple[float, float], float],
+        stride: Union[Tuple[float, float], float],
+        roi: Optional[BoundingBox] = None,
+        units: Units = Units.PIXELS,
+    ) -> None:
+        """Initialize a new Sampler instance.
 
-    def _validate_bands(self, bands: Sequence[str]) -> None:
-        """Validate list of bands.
+        The ``size`` and ``stride`` arguments can either be:
 
-        Args:
-            bands: user-provided sequence of bands to load
-        Raises:
-            AssertionError: if ``bands`` is not a sequence
-            ValueError: if an invalid band name is provided
-
-        .. versionadded:: 0.2
-        """
-        assert isinstance(bands, Sequence), "'bands' must be a sequence"
-        for band in bands:
-            if band not in self.band_names:
-                raise ValueError(f"'{band}' is an invalid band name.")
+        * a single ``float`` - in which case the same value is used for the height and
+          width dimension
+        * a ``tuple`` of two floats - in which case, the first *float* is used for the
+          height dimension, and the second *float* for the width dimension
 
-    def plot(
-        self,
-        sample: Dict[str, Tensor],
-        time_step: int = 0,
-        show_titles: bool = True,
-        suptitle: Optional[str] = None,
-    ) -> plt.Figure:
-        """Plot a sample from the dataset.
+        .. versionchanged:: 0.3
+           Added ``units`` parameter, changed default to pixel units
 
         Args:
-            sample: a sample returned by :meth:`__getitem__`
-            time_step: time step at which to access image, beginning with 0
-            show_titles: flag indicating whether to show titles above each panel
-            suptitle: optional suptitle to use for figure
+            dataset: dataset to index from
+            size: dimensions of each :term:`patch`
+            stride: distance to skip between each patch
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+            units: defines if ``size`` and ``stride`` are in pixel or CRS units
+        """
+        super().__init__(dataset, roi)
+        self.size = _to_tuple(size)
+        self.stride = _to_tuple(stride)
+
+        if units == Units.PIXELS:
+            self.size = (self.size[0] * self.res, self.size[1] * self.res)
+            self.stride = (self.stride[0] * self.res, self.stride[1] * self.res)
+
+        self.hits = []
+        for hit in self.index.intersection(tuple(self.roi), objects=True):
+            bounds = BoundingBox(*hit.bounds)
+            if (
+                bounds.maxx - bounds.minx >= self.size[1]
+                and bounds.maxy - bounds.miny >= self.size[0]
+            ):
+                self.hits.append(hit)
+
+        self.length = 0
+        for hit in self.hits:
+            bounds = BoundingBox(*hit.bounds)
+            rows, cols = tile_to_chips(bounds, self.size, self.stride)
+            self.length += rows * cols
+
+    def __iter__(self) -> Iterator[BoundingBox]:
+        """Return the index of a dataset.
 
         Returns:
-            a matplotlib Figure with the rendered sample
+            (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
+        """
+        # For each tile...
+        for hit in self.hits:
+            bounds = BoundingBox(*hit.bounds)
+            rows, cols = tile_to_chips(bounds, self.size, self.stride)
+            mint = bounds.mint
+            maxt = bounds.maxt
+
+            # For each row...
+            for i in range(rows):
+                miny = bounds.miny + i * self.stride[0]
+                maxy = miny + self.size[0]
+                if maxy > bounds.maxy:
+                    maxy = bounds.maxy
+                    miny = bounds.maxy - self.size[0]
+
+                # For each column...
+                for j in range(cols):
+                    minx = bounds.minx + j * self.stride[1]
+                    maxx = minx + self.size[1]
+                    if maxx > bounds.maxx:
+                        maxx = bounds.maxx
+                        minx = bounds.maxx - self.size[1]
 
-        .. versionadded:: 0.2
+                    yield BoundingBox(minx, maxx, miny, maxy, mint, maxt)
+
+    def __len__(self) -> int:
+        """Return the number of samples over the ROI.
+
+        Returns:
+            number of patches that will be sampled
         """
-        rgb_indices = []
-        for band in self.RGB_BANDS:
-            if band in self.bands:
-                rgb_indices.append(self.bands.index(band))
-            else:
-                raise ValueError("Dataset doesn't contain some of the RGB bands")
+        return self.length
 
-        ncols = 2
-        image, mask = sample["image"][time_step, rgb_indices], sample["mask"]
 
-        image = torch.tensor(
-            percentile_normalization(image.numpy()) * 255, dtype=torch.uint8
-        )
+class PreChippedGeoSampler(GeoSampler):
+    """Samples entire files at a time.
 
-        mask = torch.argmax(mask, dim=0)
+    This is particularly useful for datasets that contain geospatial metadata
+    and subclass :class:`~torchgeo.datasets.GeoDataset` but have already been
+    pre-processed into :term:`chips <chip>`.
 
-        if "prediction" in sample:
-            ncols += 1
-            preds = torch.argmax(sample["prediction"], dim=0)
+    This sampler should not be used with :class:`~torchgeo.datasets.NonGeoDataset`.
+    You may encounter problems when using an :term:`ROI <region of interest (ROI)>`
+    that partially intersects with one of the file bounding boxes, when using an
+    :class:`~torchgeo.datasets.IntersectionDataset`, or when each file is in a
+    different CRS. These issues can be solved by adding padding.
+    """
 
-        fig, axs = plt.subplots(ncols=ncols, figsize=(10, 10 * ncols))
+    def __init__(
+        self,
+        dataset: GeoDataset,
+        roi: Optional[BoundingBox] = None,
+        shuffle: bool = False,
+    ) -> None:
+        """Initialize a new Sampler instance.
+
+        .. versionadded:: 0.3
+
+        Args:
+            dataset: dataset to index from
+            roi: region of interest to sample from (minx, maxx, miny, maxy, mint, maxt)
+                (defaults to the bounds of ``dataset.index``)
+            shuffle: if True, reshuffle data at every epoch
+        """
+        super().__init__(dataset, roi)
+        self.shuffle = shuffle
 
-        axs[0].imshow(image.permute(1, 2, 0))
-        axs[0].axis("off")
-        axs[1].imshow(mask)
-        axs[1].axis("off")
+        self.hits = []
+        for hit in self.index.intersection(tuple(self.roi), objects=True):
+            self.hits.append(hit)
 
-        if show_titles:
-            axs[0].set_title("Image")
-            axs[1].set_title("Mask")
+    def __iter__(self) -> Iterator[BoundingBox]:
+        """Return the index of a dataset.
 
-        if "prediction" in sample:
-            axs[2].imshow(preds)
-            axs[2].axis("off")
-            if show_titles:
-                axs[2].set_title("Prediction")
+        Returns:
+            (minx, maxx, miny, maxy, mint, maxt) coordinates to index a dataset
+        """
+        generator: Callable[[int], Iterable[int]] = range
+        if self.shuffle:
+            generator = torch.randperm
+
+        for idx in generator(len(self)):
+            yield BoundingBox(*self.hits[idx].bounds)
 
-        if suptitle is not None:
-            plt.suptitle(suptitle)
+    def __len__(self) -> int:
+        """Return the number of samples over the ROI.
 
-        return fig
+        Returns:
+            number of patches that will be sampled
+        """
+        return len(self.hits)
```

### Comparing `torchgeo-0.3.1/torchgeo/losses/qr.py` & `torchgeo-0.4.0/torchgeo/losses/qr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """Loss functions for learing on the prior."""
 
 import torch
 import torch.nn.functional as F
 from torch.nn.modules import Module
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
-
 
 class QRLoss(Module):
     """The QR (forward) loss between class probabilities and predictions.
 
     This loss is defined in `'Resolving label uncertainty with implicit generative
     models' <https://openreview.net/forum?id=AEa_UepnMDX>`_.
```

### Comparing `torchgeo-0.3.1/torchgeo/models/changestar.py` & `torchgeo-0.4.0/torchgeo/models/changestar.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 import torch.nn as nn
 from einops import rearrange
 from torch import Tensor
 from torch.nn.modules import Module
 
 from .farseg import FarSeg
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
-
 
 class ChangeMixin(Module):
     """This module enables any segmentation model to detect binary change.
 
     The common usage is to attach this module on a segmentation model without the
     classification head.
```

### Comparing `torchgeo-0.3.1/torchgeo/models/farseg.py` & `torchgeo-0.4.0/torchgeo/models/farseg.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import math
 from collections import OrderedDict
 from typing import List, cast
 
 import torch.nn.functional as F
 import torchvision
-from packaging.version import parse
 from torch import Tensor
 from torch.nn.modules import (
     BatchNorm2d,
     Conv2d,
     Identity,
     Module,
     ModuleList,
@@ -21,26 +20,14 @@
     Sequential,
     Sigmoid,
     UpsamplingBilinear2d,
 )
 from torchvision.models import resnet
 from torchvision.ops import FeaturePyramidNetwork as FPN
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
-ModuleList.__module__ = "nn.ModuleList"
-Sequential.__module__ = "nn.Sequential"
-Conv2d.__module__ = "nn.Conv2d"
-BatchNorm2d.__module__ = "nn.BatchNorm2d"
-ReLU.__module__ = "nn.ReLU"
-UpsamplingBilinear2d.__module__ = "nn.UpsamplingBilinear2d"
-Sigmoid.__module__ = "nn.Sigmoid"
-Identity.__module__ = "nn.Identity"
-
 
 class FarSeg(Module):
     """Foreground-Aware Relation Network (FarSeg).
 
     This model can be used for binary- or multi-class object segmentation, such as
     building, road, ship, and airplane segmentation. It can be also extended as a change
     detection model. It features a foreground-scene relation module to model the
@@ -70,25 +57,22 @@
         if backbone in ["resnet18", "resnet34"]:
             max_channels = 512
         elif backbone in ["resnet50", "resnet101"]:
             max_channels = 2048
         else:
             raise ValueError(f"unknown backbone: {backbone}.")
         kwargs = {}
-        if parse(torchvision.__version__) >= parse("0.13"):
-            if backbone_pretrained:
-                kwargs = {
-                    "weights": getattr(
-                        torchvision.models, f"ResNet{backbone[6:]}_Weights"
-                    ).DEFAULT
-                }
-            else:
-                kwargs = {"weights": None}
+        if backbone_pretrained:
+            kwargs = {
+                "weights": getattr(
+                    torchvision.models, f"ResNet{backbone[6:]}_Weights"
+                ).DEFAULT
+            }
         else:
-            kwargs = {"pretrained": backbone_pretrained}
+            kwargs = {"weights": None}
 
         self.backbone = getattr(resnet, backbone)(**kwargs)
 
         self.fpn = FPN(
             in_channels_list=[max_channels // (2 ** (3 - i)) for i in range(4)],
             out_channels=256,
         )
```

### Comparing `torchgeo-0.3.1/torchgeo/models/fcn.py` & `torchgeo-0.4.0/torchgeo/models/fcn.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 """Simple fully convolutional neural network (FCN) implementations."""
 
 import torch.nn as nn
 from torch import Tensor
 from torch.nn.modules import Module
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
-
 
 class FCN(Module):
     """A simple 5 layer FCN with leaky relus and 'same' padding."""
 
     def __init__(self, in_channels: int, classes: int, num_filters: int = 64) -> None:
         """Initializes the 5 layer FCN model.
```

### Comparing `torchgeo-0.3.1/torchgeo/models/fcsiam.py` & `torchgeo-0.4.0/torchgeo/models/fcsiam.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 import segmentation_models_pytorch as smp
 import torch
 from segmentation_models_pytorch import Unet
 from segmentation_models_pytorch.base.model import SegmentationModel
 from torch import Tensor
 
-Unet.__module__ = "segmentation_models_pytorch"
-
 
 class FCSiamConc(SegmentationModel):  # type: ignore[misc]
     """Fully-convolutional Siamese Concatenation (FC-Siam-conc).
 
     If you use this model in your research, please cite the following paper:
 
     * https://doi.org/10.1109/ICIP.2018.8451652
```

### Comparing `torchgeo-0.3.1/torchgeo/models/rcf.py` & `torchgeo-0.4.0/torchgeo/models/rcf.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 """Implementation of a random convolutional feature projection model."""
 
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
-from torch.nn.modules import Conv2d, Module
-
-Module.__module__ = "torch.nn"
-Conv2d.__module__ = "torch.nn"
+from torch.nn.modules import Module
 
 
 class RCF(Module):
     """This model extracts random convolutional features (RCFs) from its input.
 
     RCFs are used in Multi-task Observation using Satellite Imagery & Kitchen Sinks
     (MOSAIKS) method proposed in https://www.nature.com/articles/s41467-021-24638-z.
@@ -37,23 +34,23 @@
         seed: Optional[int] = None,
     ) -> None:
         """Initializes the RCF model.
 
         This is a static model that serves to extract fixed length feature vectors from
         input patches.
 
+        .. versionadded:: 0.2
+           The *seed* parameter.
+
         Args:
             in_channels: number of input channels
             features: number of features to compute, must be divisible by 2
             kernel_size: size of the kernel used to compute the RCFs
             bias: bias of the convolutional layer
             seed: random seed used to initialize the convolutional layer
-
-        .. versionadded:: 0.2
-           The *seed* parameter.
         """
         super().__init__()
 
         assert features % 2 == 0
 
         if seed is None:
             generator = None
```

### Comparing `torchgeo-0.3.1/torchgeo/samplers/__init__.py` & `torchgeo-0.4.0/torchgeo/samplers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Licensed under the MIT License.
 
 """TorchGeo samplers."""
 
 from .batch import BatchGeoSampler, RandomBatchGeoSampler
 from .constants import Units
 from .single import GeoSampler, GridGeoSampler, PreChippedGeoSampler, RandomGeoSampler
+from .utils import get_random_bounding_box, tile_to_chips
 
 __all__ = (
     # Samplers
     "GridGeoSampler",
     "PreChippedGeoSampler",
     "RandomGeoSampler",
     # Batch samplers
     "RandomBatchGeoSampler",
     # Base classes
     "GeoSampler",
     "BatchGeoSampler",
+    # Utilities
+    "get_random_bounding_box",
+    "tile_to_chips",
     # Constants
     "Units",
 )
-
-# https://stackoverflow.com/questions/40018681
-for module in __all__:
-    globals()[module].__module__ = "torchgeo.samplers"
```

### Comparing `torchgeo-0.3.1/torchgeo/trainers/byol.py` & `torchgeo-0.4.0/torchgeo/trainers/byol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 """BYOL tasks."""
 
-import random
-from typing import Any, Callable, Dict, Optional, Tuple, cast
+import os
+from typing import Any, Dict, Optional, Tuple, cast
 
 import pytorch_lightning as pl
+import timm
 import torch
+import torch.nn as nn
 import torch.nn.functional as F
-import torchvision
 from kornia import augmentation as K
-from kornia import filters
-from kornia.geometry import transform as KorniaTransform
-from packaging.version import parse
 from torch import Tensor, optim
-from torch.autograd import Variable
-from torch.nn.modules import BatchNorm1d, Conv2d, Linear, Module, ReLU, Sequential
 from torch.optim.lr_scheduler import ReduceLROnPlateau
+from torchvision.models._api import WeightsEnum
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
+from ..models import get_weight
+from . import utils
 
 
 def normalized_mse(x: Tensor, y: Tensor) -> Tensor:
     """Computes the normalized mean squared error between x and y.
 
     Args:
         x: tensor x
@@ -36,46 +32,18 @@
     """
     x = F.normalize(x, dim=-1)
     y = F.normalize(y, dim=-1)
     mse = torch.mean(2 - 2 * (x * y).sum(dim=-1))
     return mse
 
 
-# TODO: Move this to transforms
-class RandomApply(Module):
-    """Applies augmentation function (augm) with probability p."""
-
-    def __init__(self, augm: Callable[[Tensor], Tensor], p: float) -> None:
-        """Initialize RandomApply.
-
-        Args:
-            augm: augmentation function to apply
-            p: probability with which the augmentation function is applied
-        """
-        super().__init__()
-        self.augm = augm
-        self.p = p
-
-    def forward(self, x: Tensor) -> Tensor:
-        """Applies an augmentation to the input with some probability.
-
-        Args:
-            x: a batch of imagery
-
-        Returns
-            augmented version of ``x`` with probability ``self.p`` else an un-augmented
-                version
-        """
-        return x if random.random() > self.p else self.augm(x)
-
-
 # TODO: This isn't _really_ applying the augmentations from SimCLR as we have
 # multispectral imagery and thus can't naively apply color jittering or grayscale
 # conversions. We should think more about what makes sense here.
-class SimCLRAugmentation(Module):
+class SimCLRAugmentation(nn.Module):
     """A module for applying SimCLR augmentations.
 
     SimCLR was one of the first papers to show the effectiveness of random data
     augmentation in self-supervised-learning setups. See
     https://arxiv.org/pdf/2002.05709.pdf for more details.
     """
 
@@ -84,21 +52,21 @@
 
         Args:
             image_size: Tuple of integers defining the image size
         """
         super().__init__()
         self.size = image_size
 
-        self.augmentation = Sequential(
-            KorniaTransform.Resize(size=image_size, align_corners=False),
+        self.augmentation = nn.Sequential(
+            K.Resize(size=image_size, align_corners=False),
             # Not suitable for multispectral adapt
-            # RandomApply(K.ColorJitter(0.8, 0.8, 0.8, 0.2), p=0.8),
+            # K.ColorJitter(0.8, 0.8, 0.8, 0.8, 0.2),
             # K.RandomGrayscale(p=0.2),
             K.RandomHorizontalFlip(),
-            RandomApply(filters.GaussianBlur2d((3, 3), (1.5, 1.5)), p=0.1),
+            K.RandomGaussianBlur((3, 3), (1.5, 1.5), p=0.1),
             K.RandomResizedCrop(size=image_size),
         )
 
     def forward(self, x: Tensor) -> Tensor:
         """Applys SimCLR augmentations to the input tensor.
 
         Args:
@@ -106,87 +74,90 @@
 
         Returns:
             an augmented batch of imagery
         """
         return cast(Tensor, self.augmentation(x))
 
 
-class MLP(Module):
+class MLP(nn.Module):
     """MLP used in the BYOL projection head."""
 
     def __init__(
         self, dim: int, projection_size: int = 256, hidden_size: int = 4096
     ) -> None:
         """Initializes the MLP projection head.
 
         Args:
             dim: size of layer to project
             projection_size: size of the output layer
             hidden_size: size of the hidden layer
         """
         super().__init__()
-        self.mlp = Sequential(
-            Linear(dim, hidden_size),
-            BatchNorm1d(hidden_size),
-            ReLU(inplace=True),
-            Linear(hidden_size, projection_size),
+        self.mlp = nn.Sequential(
+            nn.Linear(dim, hidden_size),
+            nn.BatchNorm1d(hidden_size),
+            nn.ReLU(inplace=True),
+            nn.Linear(hidden_size, projection_size),
         )
 
     def forward(self, x: Tensor) -> Tensor:
         """Forward pass of the MLP model.
 
         Args:
             x: batch of imagery
 
         Returns:
             embedded version of the input
         """
         return cast(Tensor, self.mlp(x))
 
 
-class EncoderWrapper(Module):
-    """Encoder wrapper for joining a model and a projection head.
+class BackboneWrapper(nn.Module):
+    """Backbone wrapper for joining a model and a projection head.
 
     When we call .forward() on this module the following steps happen:
 
     * The input is passed through the base model
     * When the encoding layer is reached a hook is called
     * The output of the encoding layer is passed through the projection head
     * The forward call returns the output of the projection head
+
+    .. versionchanged 0.4: Name changed from *EncoderWrapper* to
+        *BackboneWrapper*.
     """
 
     def __init__(
         self,
-        model: Module,
+        model: nn.Module,
         projection_size: int = 256,
         hidden_size: int = 4096,
         layer: int = -2,
     ) -> None:
-        """Initializes EncoderWrapper.
+        """Initializes BackboneWrapper.
 
         Args:
             model: model to encode
             projection_size: size of the ouput layer of the projector MLP
             hidden_size: size of hidden layer of the projector MLP
             layer: layer from model to project
         """
         super().__init__()
 
         self.model = model
         self.projection_size = projection_size
         self.hidden_size = hidden_size
         self.layer = layer
 
-        self._projector: Optional[Module] = None
+        self._projector: Optional[nn.Module] = None
         self._projector_dim: Optional[int] = None
         self._encoded = torch.empty(0)
         self._register_hook()
 
     @property
-    def projector(self) -> Module:
+    def projector(self) -> nn.Module:
         """Wrapper module for the projector head."""
         assert self._projector_dim is not None
         if self._projector is None:
             self._projector = MLP(
                 self._projector_dim, self.projection_size, self.hidden_size
             )
         return self._projector
@@ -207,14 +178,17 @@
             # If we haven't already, measure the output size
             self._projector_dim = output.shape[-1]
 
         # Project the output to get encodings, the projector model is created the first
         # time this is called
         self._encoded = self.projector(output)
 
+        # Store the image embeddings
+        self._embedding = output
+
     def _register_hook(self) -> None:
         """Register a hook for layer that we will extract features from."""
         layer = list(self.model.children())[self.layer]
         layer.register_forward_hook(self._hook)
 
     def forward(self, x: Tensor) -> Tensor:
         """Pass through the model, and collect the representation from our forward hook.
@@ -225,150 +199,144 @@
         Returns:
             output from the model
         """
         _ = self.model(x)
         return self._encoded
 
 
-class BYOL(Module):
+class BYOL(nn.Module):
     """BYOL implementation.
 
-    BYOL contains two identical encoder networks. The first is trained as usual, and its
-    weights are updated with each training batch. The second, "target" network, is
-    updated using a running average of the first encoder's weights.
+    BYOL contains two identical backbone networks. The first is trained as usual, and
+    its weights are updated with each training batch. The second, "target" network,
+    is updated using a running average of the first backbone's weights.
 
     See https://arxiv.org/abs/2006.07733 for more details (and please cite it if you
     use it in your own work).
     """
 
     def __init__(
         self,
-        model: Module,
+        model: nn.Module,
         image_size: Tuple[int, int] = (256, 256),
         hidden_layer: int = -2,
         in_channels: int = 4,
         projection_size: int = 256,
         hidden_size: int = 4096,
-        augment_fn: Optional[Module] = None,
+        augment_fn: Optional[nn.Module] = None,
         beta: float = 0.99,
         **kwargs: Any,
     ) -> None:
         """Sets up a model for pre-training with BYOL using projection heads.
 
         Args:
             model: the model to pretrain using BYOL
             image_size: the size of the training images
             hidden_layer: the hidden layer in ``model`` to attach the projection
                 head to, can be the name of the layer or index of the layer
             in_channels: number of input channels to the model
             projection_size: size of first layer of the projection MLP
             hidden_size: size of the hidden layer of the projection MLP
             augment_fn: an instance of a module that performs data augmentation
-            beta: the speed at which the target encoder is updated using the main
-                encoder
+            beta: the speed at which the target backbone is updated using the main
+                backbone
         """
         super().__init__()
 
-        self.augment: Module
+        self.augment: nn.Module
         if augment_fn is None:
             self.augment = SimCLRAugmentation(image_size)
         else:
             self.augment = augment_fn
 
         self.beta = beta
         self.in_channels = in_channels
-        self.encoder = EncoderWrapper(
+        self.backbone = BackboneWrapper(
             model, projection_size, hidden_size, layer=hidden_layer
         )
         self.predictor = MLP(projection_size, projection_size, hidden_size)
-        self.target = EncoderWrapper(
+        self.target = BackboneWrapper(
             model, projection_size, hidden_size, layer=hidden_layer
         )
 
         # Perform a single forward pass to initialize the wrapper correctly
-        self.encoder(torch.zeros(2, self.in_channels, *image_size))
+        self.backbone(torch.zeros(2, self.in_channels, *image_size))
 
     def forward(self, x: Tensor) -> Tensor:
-        """Forward pass of the encoder model through the MLP and prediction head.
+        """Forward pass of the backbone model through the MLP and prediction head.
 
         Args:
             x: tensor of data to run through the model
 
         Returns:
             output from the model
         """
-        return cast(Tensor, self.predictor(self.encoder(x)))
+        return cast(Tensor, self.predictor(self.backbone(x)))
 
     def update_target(self) -> None:
         """Method to update the "target" model weights."""
-        for p, pt in zip(self.encoder.parameters(), self.target.parameters()):
+        for p, pt in zip(self.backbone.parameters(), self.target.parameters()):
             pt.data = self.beta * pt.data + (1 - self.beta) * p.data
 
 
 class BYOLTask(pl.LightningModule):
-    """Class for pre-training any PyTorch model using BYOL."""
+    """Class for pre-training any PyTorch model using BYOL.
+
+    Supports any available `Timm model
+    <https://rwightman.github.io/pytorch-image-models/>`_
+    as an architecture choice. To see a list of available pretrained
+    models, you can do:
+
+    .. code-block:: python
+
+        import timm
+        print(timm.list_models())
+    """
 
     def config_task(self) -> None:
         """Configures the task based on kwargs parameters passed to the constructor."""
+        # Create model
         in_channels = self.hyperparams["in_channels"]
-        pretrained = self.hyperparams["imagenet_pretraining"]
-        encoder_name = self.hyperparams["encoder_name"]
+        weights = self.hyperparams["weights"]
+        backbone = timm.create_model(
+            self.hyperparams["backbone"],
+            in_chans=in_channels,
+            pretrained=weights is True,
+        )
 
-        if parse(torchvision.__version__) >= parse("0.13"):
-            if pretrained:
-                kwargs = {
-                    "weights": getattr(
-                        torchvision.models, f"ResNet{encoder_name[6:]}_Weights"
-                    ).DEFAULT
-                }
+        # Load weights
+        if weights and weights is not True:
+            if isinstance(weights, WeightsEnum):
+                state_dict = weights.get_state_dict(progress=True)
+            elif os.path.exists(weights):
+                _, state_dict = utils.extract_backbone(weights)
             else:
-                kwargs = {"weights": None}
-        else:
-            kwargs = {"pretrained": pretrained}
+                state_dict = get_weight(weights).get_state_dict(progress=True)
+            backbone = utils.load_state_dict(backbone, state_dict)
 
-        encoder = getattr(torchvision.models, encoder_name)(**kwargs)
-
-        layer = encoder.conv1
-        # Creating new Conv2d layer
-        new_layer = Conv2d(
-            in_channels=in_channels,
-            out_channels=layer.out_channels,
-            kernel_size=layer.kernel_size,
-            stride=layer.stride,
-            padding=layer.padding,
-            bias=layer.bias,
-        ).requires_grad_()
-        # initialize the weights from new channel with the red channel weights
-        copy_weights = 0
-        # Copying the weights from the old to the new layer
-        new_layer.weight[:, : layer.in_channels, :, :].data[:] = Variable(
-            layer.weight.clone(), requires_grad=True
-        )
-        # Copying the weights of the old layer to the extra channels
-        for i in range(in_channels - layer.in_channels):
-            channel = layer.in_channels + i
-            new_layer.weight[:, channel : channel + 1, :, :].data[:] = Variable(
-                layer.weight[:, copy_weights : copy_weights + 1, ::].clone(),
-                requires_grad=True,
-            )
-
-        encoder.conv1 = new_layer
-        self.model = BYOL(encoder, in_channels=in_channels, image_size=(256, 256))
+        self.model = BYOL(backbone, in_channels=in_channels, image_size=(256, 256))
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize a LightningModule for pre-training a model with BYOL.
 
         Keyword Args:
-            in_channels: number of channels on the input imagery
-            encoder_name: either "resnet18" or "resnet50"
-            imagenet_pretraining: bool indicating whether to use imagenet pretrained
-                weights
+            in_channels: Number of input channels to model
+            backbone: Name of the timm model to use
+            weights: Either a weight enum, the string representation of a weight enum,
+                True for ImageNet weights, False or None for random weights,
+                or the path to a saved model state dict.
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
 
         Raises:
             ValueError: if kwargs arguments are invalid
+
+        .. versionchanged:: 0.4
+           The *backbone_name* parameter was renamed to *backbone*. Change backbone
+           support from torchvision.models to timm.
         """
         super().__init__()
 
         # Creates `self.hparams` from kwargs
         self.save_hyperparameters()  # type: ignore[operator]
         self.hyperparams = cast(Dict[str, Any], self.hparams)
 
@@ -389,15 +357,15 @@
         """Initialize the optimizer and learning rate scheduler.
 
         Returns:
             a "lr dict" according to the pytorch lightning documentation --
             https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         """
         optimizer_class = getattr(optim, self.hyperparams.get("optimizer", "Adam"))
-        lr = self.hyperparams.get("lr", 1e-4)
+        lr = self.hyperparams.get("learning_rate", 1e-4)
         weight_decay = self.hyperparams.get("weight_decay", 1e-6)
         optimizer = optimizer_class(self.parameters(), lr=lr, weight_decay=weight_decay)
 
         return {
             "optimizer": optimizer,
             "lr_scheduler": {
                 "scheduler": ReduceLROnPlateau(
@@ -418,15 +386,15 @@
             training loss
         """
         batch = args[0]
         x = batch["image"]
         with torch.no_grad():
             x1, x2 = self.model.augment(x), self.model.augment(x)
 
-        pred1, pred2 = self.forward(x1), self.forward(x2)
+        pred1, pred2 = self(x1), self(x2)
         with torch.no_grad():
             targ1, targ2 = self.model.target(x1), self.model.target(x2)
         loss = torch.mean(normalized_mse(pred1, targ2) + normalized_mse(pred2, targ1))
 
         self.log("train_loss", loss, on_step=True, on_epoch=False)
         self.model.update_target()
 
@@ -437,15 +405,29 @@
 
         Args:
             batch: the output of your DataLoader
         """
         batch = args[0]
         x = batch["image"]
         x1, x2 = self.model.augment(x), self.model.augment(x)
-        pred1, pred2 = self.forward(x1), self.forward(x2)
+        pred1, pred2 = self(x1), self(x2)
         targ1, targ2 = self.model.target(x1), self.model.target(x2)
         loss = torch.mean(normalized_mse(pred1, targ2) + normalized_mse(pred2, targ1))
 
         self.log("val_loss", loss, on_step=False, on_epoch=True)
 
     def test_step(self, *args: Any, **kwargs: Any) -> Any:
         """No-op, does nothing."""
+
+    def predict_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the output embeddings of the image backbone.
+
+        Args:
+            batch: the output of your DataLoader
+
+        Returns:
+            image embeddings
+        """
+        batch = args[0]
+        x = batch["image"]
+        self(x)
+        return self.model.backbone._embedding
```

### Comparing `torchgeo-0.3.1/torchgeo/trainers/classification.py` & `torchgeo-0.4.0/torchgeo/trainers/classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,78 +2,70 @@
 # Licensed under the MIT License.
 
 """Classification tasks."""
 
 import os
 from typing import Any, Dict, cast
 
+import matplotlib.pyplot as plt
 import pytorch_lightning as pl
 import timm
 import torch
 import torch.nn as nn
 from segmentation_models_pytorch.losses import FocalLoss, JaccardLoss
 from torch import Tensor
-from torch.nn.modules import Conv2d, Linear
 from torch.optim.lr_scheduler import ReduceLROnPlateau
-from torchmetrics import Accuracy, FBetaScore, JaccardIndex, MetricCollection
+from torchmetrics import MetricCollection
+from torchmetrics.classification import (
+    MulticlassAccuracy,
+    MulticlassFBetaScore,
+    MulticlassJaccardIndex,
+    MultilabelAccuracy,
+    MultilabelFBetaScore,
+)
+from torchvision.models._api import WeightsEnum
 
-from ..datasets.utils import unbind_samples
+from ..datasets import unbind_samples
+from ..models import get_weight
 from . import utils
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Conv2d.__module__ = "nn.Conv2d"
-Linear.__module__ = "nn.Linear"
-
 
 class ClassificationTask(pl.LightningModule):
-    """LightningModule for image classification."""
+    """LightningModule for image classification.
+
+    Supports any available `Timm model
+    <https://rwightman.github.io/pytorch-image-models/>`_
+    as an architecture choice. To see a list of available
+    models, you can do:
+
+    .. code-block:: python
+
+        import timm
+        print(timm.list_models())
+    """
 
     def config_model(self) -> None:
         """Configures the model based on kwargs parameters passed to the constructor."""
-        in_channels = self.hyperparams["in_channels"]
-        classification_model = self.hyperparams["classification_model"]
+        # Create model
+        weights = self.hyperparams["weights"]
+        self.model = timm.create_model(
+            self.hyperparams["model"],
+            num_classes=self.hyperparams["num_classes"],
+            in_chans=self.hyperparams["in_channels"],
+            pretrained=weights is True,
+        )
 
-        imagenet_pretrained = False
-        custom_pretrained = False
-        if self.hyperparams["weights"] and not os.path.exists(
-            self.hyperparams["weights"]
-        ):
-            if self.hyperparams["weights"] not in ["imagenet", "random"]:
-                raise ValueError(
-                    f"Weight type '{self.hyperparams['weights']}' is not valid."
-                )
+        # Load weights
+        if weights and weights is not True:
+            if isinstance(weights, WeightsEnum):
+                state_dict = weights.get_state_dict(progress=True)
+            elif os.path.exists(weights):
+                _, state_dict = utils.extract_backbone(weights)
             else:
-                imagenet_pretrained = self.hyperparams["weights"] == "imagenet"
-            custom_pretrained = False
-        else:
-            custom_pretrained = True
-
-        # Create the model
-        valid_models = timm.list_models(pretrained=True)
-        if classification_model in valid_models:
-            self.model = timm.create_model(
-                classification_model,
-                num_classes=self.hyperparams["num_classes"],
-                in_chans=in_channels,
-                pretrained=imagenet_pretrained,
-            )
-        else:
-            raise ValueError(
-                f"Model type '{classification_model}' is not a valid timm model."
-            )
-
-        if custom_pretrained:
-            name, state_dict = utils.extract_encoder(self.hyperparams["weights"])
-
-            if self.hyperparams["classification_model"] != name:
-                raise ValueError(
-                    f"Trying to load {name} weights into a "
-                    f"{self.hyperparams['classification_model']}"
-                )
+                state_dict = get_weight(weights).get_state_dict(progress=True)
             self.model = utils.load_state_dict(self.model, state_dict)
 
     def config_task(self) -> None:
         """Configures the task based on kwargs parameters passed to the constructor."""
         self.config_model()
 
         if self.hyperparams["loss"] == "ce":
@@ -85,39 +77,47 @@
         else:
             raise ValueError(f"Loss type '{self.hyperparams['loss']}' is not valid.")
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize the LightningModule with a model and loss function.
 
         Keyword Args:
-            classification_model: Name of the classification model use
-            loss: Name of the loss function
-            weights: Either "random", "imagenet_only", "imagenet_and_random", or
-                "random_rgb"
+            model: Name of the classification model use
+            loss: Name of the loss function, accepts 'ce', 'jaccard', or 'focal'
+            weights: Either a weight enum, the string representation of a weight enum,
+                True for ImageNet weights, False or None for random weights,
+                or the path to a saved model state dict.
+            num_classes: Number of prediction classes
+            in_channels: Number of input channels to model
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
+
+        .. versionchanged:: 0.4
+           The *classification_model* parameter was renamed to *model*.
         """
         super().__init__()
 
         # Creates `self.hparams` from kwargs
         self.save_hyperparameters()  # type: ignore[operator]
         self.hyperparams = cast(Dict[str, Any], self.hparams)
 
         self.config_task()
 
         self.train_metrics = MetricCollection(
             {
-                "OverallAccuracy": Accuracy(
+                "OverallAccuracy": MulticlassAccuracy(
                     num_classes=self.hyperparams["num_classes"], average="micro"
                 ),
-                "AverageAccuracy": Accuracy(
+                "AverageAccuracy": MulticlassAccuracy(
                     num_classes=self.hyperparams["num_classes"], average="macro"
                 ),
-                "JaccardIndex": JaccardIndex(
+                "JaccardIndex": MulticlassJaccardIndex(
                     num_classes=self.hyperparams["num_classes"]
                 ),
-                "F1Score": FBetaScore(
+                "F1Score": MulticlassFBetaScore(
                     num_classes=self.hyperparams["num_classes"],
                     beta=1.0,
                     average="micro",
                 ),
             },
             prefix="train_",
         )
@@ -143,15 +143,15 @@
 
         Returns:
             training loss
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         # by default, the train step logs every `log_every_n_steps` steps where
         # `log_every_n_steps` is a parameter to the `Trainer` object
         self.log("train_loss", loss, on_step=True, on_epoch=False)
@@ -175,35 +175,41 @@
             batch: the output of your DataLoader
             batch_idx: the index of this batch
         """
         batch = args[0]
         batch_idx = args[1]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         self.log("val_loss", loss, on_step=False, on_epoch=True)
         self.val_metrics(y_hat_hard, y)
 
-        if batch_idx < 10:
+        if (
+            batch_idx < 10
+            and hasattr(self.trainer, "datamodule")
+            and self.logger
+            and hasattr(self.logger, "experiment")
+        ):
             try:
-                datamodule = self.trainer.datamodule  # type: ignore[attr-defined]
+                datamodule = self.trainer.datamodule
                 batch["prediction"] = y_hat_hard
                 for key in ["image", "label", "prediction"]:
                     batch[key] = batch[key].cpu()
                 sample = unbind_samples(batch)[0]
                 fig = datamodule.plot(sample)
-                summary_writer = self.logger.experiment  # type: ignore[union-attr]
+                summary_writer = self.logger.experiment
                 summary_writer.add_figure(
                     f"image/{batch_idx}", fig, global_step=self.global_step
                 )
-            except AttributeError:
+                plt.close()
+            except ValueError:
                 pass
 
     def validation_epoch_end(self, outputs: Any) -> None:
         """Logs epoch level validation metrics.
 
         Args:
             outputs: list of items returned by validation_step
@@ -216,15 +222,15 @@
 
         Args:
             batch: the output of your DataLoader
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         # by default, the test and validation steps only log per *epoch*
         self.log("test_loss", loss, on_step=False, on_epoch=True)
         self.test_metrics(y_hat_hard, y)
@@ -234,14 +240,28 @@
 
         Args:
             outputs: list of items returned by test_step
         """
         self.log_dict(self.test_metrics.compute())
         self.test_metrics.reset()
 
+    def predict_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the predictions.
+
+        Args:
+            batch: the output of your DataLoader
+
+        Returns:
+            predicted softmax probabilities
+        """
+        batch = args[0]
+        x = batch["image"]
+        y_hat: Tensor = self(x).softmax(dim=-1)
+        return y_hat
+
     def configure_optimizers(self) -> Dict[str, Any]:
         """Initialize the optimizer and learning rate scheduler.
 
         Returns:
             a "lr dict" according to the pytorch lightning documentation --
             https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         """
@@ -272,44 +292,39 @@
         else:
             raise ValueError(f"Loss type '{self.hyperparams['loss']}' is not valid.")
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize the LightningModule with a model and loss function.
 
         Keyword Args:
-            classification_model: Name of the classification model use
-            loss: Name of the loss function
-            weights: Either "random", "imagenet_only", "imagenet_and_random", or
-                "random_rgb"
+            model: Name of the classification model use
+            loss: Name of the loss function, currently only supports 'bce'
+            weights: Either "random" or 'imagenet'
+            num_classes: Number of prediction classes
+            in_channels: Number of input channels to model
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
+
+        .. versionchanged:: 0.4
+           The *classification_model* parameter was renamed to *model*.
         """
         super().__init__(**kwargs)
 
-        # Creates `self.hparams` from kwargs
-        self.save_hyperparameters()  # type: ignore[operator]
-        self.hyperparams = cast(Dict[str, Any], self.hparams)
-
-        self.config_task()
-
         self.train_metrics = MetricCollection(
             {
-                "OverallAccuracy": Accuracy(
-                    num_classes=self.hyperparams["num_classes"],
-                    average="micro",
-                    multiclass=False,
+                "OverallAccuracy": MultilabelAccuracy(
+                    num_labels=self.hyperparams["num_classes"], average="micro"
                 ),
-                "AverageAccuracy": Accuracy(
-                    num_classes=self.hyperparams["num_classes"],
-                    average="macro",
-                    multiclass=False,
+                "AverageAccuracy": MultilabelAccuracy(
+                    num_labels=self.hyperparams["num_classes"], average="macro"
                 ),
-                "F1Score": FBetaScore(
-                    num_classes=self.hyperparams["num_classes"],
+                "F1Score": MultilabelFBetaScore(
+                    num_labels=self.hyperparams["num_classes"],
                     beta=1.0,
                     average="micro",
-                    multiclass=False,
                 ),
             },
             prefix="train_",
         )
         self.val_metrics = self.train_metrics.clone(prefix="val_")
         self.test_metrics = self.train_metrics.clone(prefix="test_")
 
@@ -321,16 +336,16 @@
 
         Returns:
             training loss
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
-        y_hat_hard = torch.softmax(y_hat, dim=-1)
+        y_hat = self(x)
+        y_hat_hard = torch.sigmoid(y_hat)
 
         loss = self.loss(y_hat, y.to(torch.float))
 
         # by default, the train step logs every `log_every_n_steps` steps where
         # `log_every_n_steps` is a parameter to the `Trainer` object
         self.log("train_loss", loss, on_step=True, on_epoch=False)
         self.train_metrics(y_hat_hard, y)
@@ -344,47 +359,65 @@
             batch: the output of your DataLoader
             batch_idx: the index of this batch
         """
         batch = args[0]
         batch_idx = args[1]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
-        y_hat_hard = torch.softmax(y_hat, dim=-1)
+        y_hat = self(x)
+        y_hat_hard = torch.sigmoid(y_hat)
 
         loss = self.loss(y_hat, y.to(torch.float))
 
         self.log("val_loss", loss, on_step=False, on_epoch=True)
         self.val_metrics(y_hat_hard, y)
 
-        if batch_idx < 10:
+        if (
+            batch_idx < 10
+            and hasattr(self.trainer, "datamodule")
+            and self.logger
+            and hasattr(self.logger, "experiment")
+        ):
             try:
-                datamodule = self.trainer.datamodule  # type: ignore[attr-defined]
+                datamodule = self.trainer.datamodule
                 batch["prediction"] = y_hat_hard
                 for key in ["image", "label", "prediction"]:
                     batch[key] = batch[key].cpu()
                 sample = unbind_samples(batch)[0]
                 fig = datamodule.plot(sample)
-                summary_writer = self.logger.experiment  # type: ignore[union-attr]
+                summary_writer = self.logger.experiment
                 summary_writer.add_figure(
                     f"image/{batch_idx}", fig, global_step=self.global_step
                 )
-            except AttributeError:
+            except ValueError:
                 pass
 
     def test_step(self, *args: Any, **kwargs: Any) -> None:
         """Compute test loss.
 
         Args:
             batch: the output of your DataLoader
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"]
-        y_hat = self.forward(x)
-        y_hat_hard = torch.softmax(y_hat, dim=-1)
+        y_hat = self(x)
+        y_hat_hard = torch.sigmoid(y_hat)
 
         loss = self.loss(y_hat, y.to(torch.float))
 
         # by default, the test and validation steps only log per *epoch*
         self.log("test_loss", loss, on_step=False, on_epoch=True)
         self.test_metrics(y_hat_hard, y)
+
+    def predict_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the predictions.
+
+        Args:
+            batch: the output of your DataLoader
+        Returns:
+            predicted sigmoid probabilities
+        """
+        batch = args[0]
+        x = batch["image"]
+        y_hat = torch.sigmoid(self(x))
+        return y_hat
```

### Comparing `torchgeo-0.3.1/torchgeo/trainers/regression.py` & `torchgeo-0.4.0/torchgeo/trainers/regression.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,80 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
 """Regression tasks."""
 
+import os
 from typing import Any, Dict, cast
 
+import matplotlib.pyplot as plt
 import pytorch_lightning as pl
+import timm
 import torch
-import torch.nn as nn
 import torch.nn.functional as F
-import torchvision
-from packaging.version import parse
 from torch import Tensor
-from torch.nn.modules import Conv2d, Linear
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torchmetrics import MeanAbsoluteError, MeanSquaredError, MetricCollection
-from torchvision import models
+from torchvision.models._api import WeightsEnum
 
-from ..datasets.utils import unbind_samples
-
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Conv2d.__module__ = "nn.Conv2d"
-Linear.__module__ = "nn.Linear"
+from ..datasets import unbind_samples
+from ..models import get_weight
+from . import utils
 
 
 class RegressionTask(pl.LightningModule):
-    """LightningModule for training models on regression datasets."""
+    """LightningModule for training models on regression datasets.
+
+    Supports any available `Timm model
+    <https://rwightman.github.io/pytorch-image-models/>`_
+    as an architecture choice. To see a list of available
+    models, you can do:
+
+    .. code-block:: python
+
+        import timm
+        print(timm.list_models())
+    """
 
     def config_task(self) -> None:
         """Configures the task based on kwargs parameters."""
-        if self.hyperparams["model"] == "resnet18":
-            pretrained = self.hyperparams["pretrained"]
-            if parse(torchvision.__version__) >= parse("0.13"):
-                if pretrained:
-                    kwargs = {"weights": models.ResNet18_Weights.DEFAULT}
-                else:
-                    kwargs = {"weights": None}
+        # Create model
+        weights = self.hyperparams["weights"]
+        self.model = timm.create_model(
+            self.hyperparams["model"],
+            num_classes=self.hyperparams["num_outputs"],
+            in_chans=self.hyperparams["in_channels"],
+            pretrained=weights is True,
+        )
+
+        # Load weights
+        if weights and weights is not True:
+            if isinstance(weights, WeightsEnum):
+                state_dict = weights.get_state_dict(progress=True)
+            elif os.path.exists(weights):
+                _, state_dict = utils.extract_backbone(weights)
             else:
-                kwargs = {"pretrained": pretrained}
-            self.model = models.resnet18(**kwargs)
-            in_features = self.model.fc.in_features
-            self.model.fc = nn.Linear(in_features, out_features=1)
-        else:
-            raise ValueError(f"Model type '{self.hyperparams['model']}' is not valid.")
+                state_dict = get_weight(weights).get_state_dict(progress=True)
+            self.model = utils.load_state_dict(self.model, state_dict)
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize a new LightningModule for training simple regression models.
 
         Keyword Args:
-            model: Name of the model to use
-            learning_rate: Initial learning rate to use in the optimizer
-            learning_rate_schedule_patience: Patience parameter for the LR scheduler
+            model: Name of the timm model to use
+            weights: Either a weight enum, the string representation of a weight enum,
+                True for ImageNet weights, False or None for random weights,
+                or the path to a saved model state dict.
+            num_outputs: Number of prediction outputs
+            in_channels: Number of input channels to model
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
+
+        .. versionchanged:: 0.4
+            Change regression model support from torchvision.models to timm
         """
         super().__init__()
 
         # Creates `self.hparams` from kwargs
         self.save_hyperparameters()  # type: ignore[operator]
         self.hyperparams = cast(Dict[str, Any], self.hparams)
         self.config_task()
@@ -86,15 +105,15 @@
 
         Returns:
             training loss
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"].view(-1, 1)
-        y_hat = self.forward(x)
+        y_hat = self(x)
 
         loss = F.mse_loss(y_hat, y)
 
         self.log("train_loss", loss)  # logging to TensorBoard
         self.train_metrics(y_hat, y)
 
         return loss
@@ -115,33 +134,39 @@
             batch: the output of your DataLoader
             batch_idx: the index of this batch
         """
         batch = args[0]
         batch_idx = args[1]
         x = batch["image"]
         y = batch["label"].view(-1, 1)
-        y_hat = self.forward(x)
+        y_hat = self(x)
 
         loss = F.mse_loss(y_hat, y)
         self.log("val_loss", loss)
         self.val_metrics(y_hat, y)
 
-        if batch_idx < 10:
+        if (
+            batch_idx < 10
+            and hasattr(self.trainer, "datamodule")
+            and self.logger
+            and hasattr(self.logger, "experiment")
+        ):
             try:
-                datamodule = self.trainer.datamodule  # type: ignore[attr-defined]
+                datamodule = self.trainer.datamodule
                 batch["prediction"] = y_hat
                 for key in ["image", "label", "prediction"]:
                     batch[key] = batch[key].cpu()
                 sample = unbind_samples(batch)[0]
                 fig = datamodule.plot(sample)
-                summary_writer = self.logger.experiment  # type: ignore[union-attr]
+                summary_writer = self.logger.experiment
                 summary_writer.add_figure(
                     f"image/{batch_idx}", fig, global_step=self.global_step
                 )
-            except AttributeError:
+                plt.close()
+            except ValueError:
                 pass
 
     def validation_epoch_end(self, outputs: Any) -> None:
         """Logs epoch level validation metrics.
 
         Args:
             outputs: list of items returned by validation_step
@@ -154,29 +179,42 @@
 
         Args:
             batch: the output of your DataLoader
         """
         batch = args[0]
         x = batch["image"]
         y = batch["label"].view(-1, 1)
-        y_hat = self.forward(x)
+        y_hat = self(x)
 
         loss = F.mse_loss(y_hat, y)
         self.log("test_loss", loss)
         self.test_metrics(y_hat, y)
 
     def test_epoch_end(self, outputs: Any) -> None:
         """Logs epoch level test metrics.
 
         Args:
             outputs: list of items returned by test_step
         """
         self.log_dict(self.test_metrics.compute())
         self.test_metrics.reset()
 
+    def predict_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the predictions.
+
+        Args:
+            batch: the output of your DataLoader
+        Returns:
+            predicted values
+        """
+        batch = args[0]
+        x = batch["image"]
+        y_hat: Tensor = self(x)
+        return y_hat
+
     def configure_optimizers(self) -> Dict[str, Any]:
         """Initialize the optimizer and learning rate scheduler.
 
         Returns:
             a "lr dict" according to the pytorch lightning documentation --
             https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/trainers/segmentation.py` & `torchgeo-0.4.0/torchgeo/trainers/segmentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,93 +2,108 @@
 # Licensed under the MIT License.
 
 """Segmentation tasks."""
 
 import warnings
 from typing import Any, Dict, cast
 
+import matplotlib.pyplot as plt
 import pytorch_lightning as pl
 import segmentation_models_pytorch as smp
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim.lr_scheduler import ReduceLROnPlateau
-from torch.utils.data import DataLoader
-from torchmetrics import Accuracy, JaccardIndex, MetricCollection
+from torchmetrics import MetricCollection
+from torchmetrics.classification import MulticlassAccuracy, MulticlassJaccardIndex
 
 from ..datasets.utils import unbind_samples
 from ..models import FCN
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-DataLoader.__module__ = "torch.utils.data"
-
 
 class SemanticSegmentationTask(pl.LightningModule):
-    """LightningModule for semantic segmentation of images."""
+    """LightningModule for semantic segmentation of images.
+
+    Supports `Segmentation Models Pytorch
+    <https://github.com/qubvel/segmentation_models.pytorch>`_
+    as an architecture choice in combination with any of these
+    `TIMM backbones <https://smp.readthedocs.io/en/latest/encoders_timm.html>`_.
+    """
 
     def config_task(self) -> None:
         """Configures the task based on kwargs parameters passed to the constructor."""
-        if self.hyperparams["segmentation_model"] == "unet":
+        if self.hyperparams["model"] == "unet":
             self.model = smp.Unet(
-                encoder_name=self.hyperparams["encoder_name"],
-                encoder_weights=self.hyperparams["encoder_weights"],
+                encoder_name=self.hyperparams["backbone"],
+                encoder_weights=self.hyperparams["weights"],
                 in_channels=self.hyperparams["in_channels"],
                 classes=self.hyperparams["num_classes"],
             )
-        elif self.hyperparams["segmentation_model"] == "deeplabv3+":
+        elif self.hyperparams["model"] == "deeplabv3+":
             self.model = smp.DeepLabV3Plus(
-                encoder_name=self.hyperparams["encoder_name"],
-                encoder_weights=self.hyperparams["encoder_weights"],
+                encoder_name=self.hyperparams["backbone"],
+                encoder_weights=self.hyperparams["weights"],
                 in_channels=self.hyperparams["in_channels"],
                 classes=self.hyperparams["num_classes"],
             )
-        elif self.hyperparams["segmentation_model"] == "fcn":
+        elif self.hyperparams["model"] == "fcn":
             self.model = FCN(
                 in_channels=self.hyperparams["in_channels"],
                 classes=self.hyperparams["num_classes"],
                 num_filters=self.hyperparams["num_filters"],
             )
         else:
             raise ValueError(
-                f"Model type '{self.hyperparams['segmentation_model']}' is not valid."
+                f"Model type '{self.hyperparams['model']}' is not valid. "
+                f"Currently, only supports 'unet', 'deeplabv3+' and 'fcn'."
             )
 
         if self.hyperparams["loss"] == "ce":
             ignore_value = -1000 if self.ignore_index is None else self.ignore_index
             self.loss = nn.CrossEntropyLoss(ignore_index=ignore_value)
         elif self.hyperparams["loss"] == "jaccard":
             self.loss = smp.losses.JaccardLoss(
                 mode="multiclass", classes=self.hyperparams["num_classes"]
             )
         elif self.hyperparams["loss"] == "focal":
             self.loss = smp.losses.FocalLoss(
                 "multiclass", ignore_index=self.ignore_index, normalized=True
             )
         else:
-            raise ValueError(f"Loss type '{self.hyperparams['loss']}' is not valid.")
+            raise ValueError(
+                f"Loss type '{self.hyperparams['loss']}' is not valid. "
+                f"Currently, supports 'ce', 'jaccard' or 'focal' loss."
+            )
 
     def __init__(self, **kwargs: Any) -> None:
         """Initialize the LightningModule with a model and loss function.
 
         Keyword Args:
-            segmentation_model: Name of the segmentation model type to use
-            encoder_name: Name of the encoder model backbone to use
-            encoder_weights: None or "imagenet" to use imagenet pretrained weights in
-                the encoder model
+            model: Name of the segmentation model type to use
+            backbone: Name of the timm backbone to use
+            weights: None or "imagenet" to use imagenet pretrained weights in
+                the backbone
             in_channels: Number of channels in input image
             num_classes: Number of semantic classes to predict
-            loss: Name of the loss function
+            loss: Name of the loss function, currently supports
+                'ce', 'jaccard' or 'focal' loss
             ignore_index: Optional integer class index to ignore in the loss and metrics
+            learning_rate: Learning rate for optimizer
+            learning_rate_schedule_patience: Patience for learning rate scheduler
 
         Raises:
             ValueError: if kwargs arguments are invalid
 
         .. versionchanged:: 0.3
            The *ignore_zeros* parameter was renamed to *ignore_index*.
+
+        .. versionchanged:: 0.4
+           The *segmentation_model* parameter was renamed to *model*,
+           *encoder_name* renamed to *backbone*, and
+           *encoder_weights* to *weights*.
         """
         super().__init__()
 
         # Creates `self.hparams` from kwargs
         self.save_hyperparameters()  # type: ignore[operator]
         self.hyperparams = cast(Dict[str, Any], self.hparams)
 
@@ -100,20 +115,20 @@
                 UserWarning,
             )
         self.ignore_index = kwargs["ignore_index"]
         self.config_task()
 
         self.train_metrics = MetricCollection(
             [
-                Accuracy(
+                MulticlassAccuracy(
                     num_classes=self.hyperparams["num_classes"],
                     ignore_index=self.ignore_index,
                     mdmc_average="global",
                 ),
-                JaccardIndex(
+                MulticlassJaccardIndex(
                     num_classes=self.hyperparams["num_classes"],
                     ignore_index=self.ignore_index,
                 ),
             ],
             prefix="train_",
         )
         self.val_metrics = self.train_metrics.clone(prefix="val_")
@@ -138,15 +153,15 @@
 
         Returns:
             training loss
         """
         batch = args[0]
         x = batch["image"]
         y = batch["mask"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         # by default, the train step logs every `log_every_n_steps` steps where
         # `log_every_n_steps` is a parameter to the `Trainer` object
         self.log("train_loss", loss, on_step=True, on_epoch=False)
@@ -170,35 +185,41 @@
             batch: the output of your DataLoader
             batch_idx: the index of this batch
         """
         batch = args[0]
         batch_idx = args[1]
         x = batch["image"]
         y = batch["mask"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         self.log("val_loss", loss, on_step=False, on_epoch=True)
         self.val_metrics(y_hat_hard, y)
 
-        if batch_idx < 10:
+        if (
+            batch_idx < 10
+            and hasattr(self.trainer, "datamodule")
+            and self.logger
+            and hasattr(self.logger, "experiment")
+        ):
             try:
-                datamodule = self.trainer.datamodule  # type: ignore[attr-defined]
+                datamodule = self.trainer.datamodule
                 batch["prediction"] = y_hat_hard
                 for key in ["image", "mask", "prediction"]:
                     batch[key] = batch[key].cpu()
                 sample = unbind_samples(batch)[0]
                 fig = datamodule.plot(sample)
-                summary_writer = self.logger.experiment  # type: ignore[union-attr]
+                summary_writer = self.logger.experiment
                 summary_writer.add_figure(
                     f"image/{batch_idx}", fig, global_step=self.global_step
                 )
-            except AttributeError:
+                plt.close()
+            except ValueError:
                 pass
 
     def validation_epoch_end(self, outputs: Any) -> None:
         """Logs epoch level validation metrics.
 
         Args:
             outputs: list of items returned by validation_step
@@ -211,15 +232,15 @@
 
         Args:
             batch: the output of your DataLoader
         """
         batch = args[0]
         x = batch["image"]
         y = batch["mask"]
-        y_hat = self.forward(x)
+        y_hat = self(x)
         y_hat_hard = y_hat.argmax(dim=1)
 
         loss = self.loss(y_hat, y)
 
         # by default, the test and validation steps only log per *epoch*
         self.log("test_loss", loss, on_step=False, on_epoch=True)
         self.test_metrics(y_hat_hard, y)
@@ -229,14 +250,33 @@
 
         Args:
             outputs: list of items returned by test_step
         """
         self.log_dict(self.test_metrics.compute())
         self.test_metrics.reset()
 
+    def predict_step(self, *args: Any, **kwargs: Any) -> Tensor:
+        """Compute and return the predictions.
+
+        By default, this will loop over images in a dataloader and aggregate
+        predictions into a list. This may not be desirable if you have many images
+        or large images which could cause out of memory errors. In this case
+        it's recommended to override this with a custom predict_step.
+
+        Args:
+            batch: the output of your DataLoader
+
+        Returns:
+            predicted softmax probabilities
+        """
+        batch = args[0]
+        x = batch["image"]
+        y_hat: Tensor = self(x).softmax(dim=1)
+        return y_hat
+
     def configure_optimizers(self) -> Dict[str, Any]:
         """Initialize the optimizer and learning rate scheduler.
 
         Returns:
             a "lr dict" according to the pytorch lightning documentation --
             https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#configure-optimizers
         """
```

### Comparing `torchgeo-0.3.1/torchgeo/trainers/utils.py` & `torchgeo-0.4.0/torchgeo/trainers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,57 +8,51 @@
 from typing import Optional, Tuple, Union, cast
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.nn.modules import Conv2d, Module
 
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "nn.Module"
-Conv2d.__module__ = "nn.Conv2d"
 
-
-def extract_encoder(path: str) -> Tuple[str, "OrderedDict[str, Tensor]"]:
-    """Extracts an encoder from a pytorch lightning checkpoint file.
+def extract_backbone(path: str) -> Tuple[str, "OrderedDict[str, Tensor]"]:
+    """Extracts a backbone from a pytorch lightning checkpoint file.
 
     Args:
         path: path to checkpoint file (.ckpt)
 
     Returns:
         tuple containing model name and state dict
 
     Raises:
-        ValueError: if 'classification_model' or 'encoder' not in
+        ValueError: if 'model' or 'backbone' not in
             checkpoint['hyper_parameters']
-    """
-    checkpoint = torch.load(  # type: ignore[no-untyped-call]
-        path, map_location=torch.device("cpu")
-    )
 
-    if "classification_model" in checkpoint["hyper_parameters"]:
-        name = checkpoint["hyper_parameters"]["classification_model"]
+    .. versionchanged:: 0.4
+        Renamed from *extract_encoder* to *extract_backbone*
+    """
+    checkpoint = torch.load(path, map_location=torch.device("cpu"))
+    if "model" in checkpoint["hyper_parameters"]:
+        name = checkpoint["hyper_parameters"]["model"]
         state_dict = checkpoint["state_dict"]
         state_dict = OrderedDict({k: v for k, v in state_dict.items() if "model." in k})
         state_dict = OrderedDict(
             {k.replace("model.", ""): v for k, v in state_dict.items()}
         )
-    elif "encoder_name" in checkpoint["hyper_parameters"]:
-        name = checkpoint["hyper_parameters"]["encoder_name"]
+    elif "backbone" in checkpoint["hyper_parameters"]:
+        name = checkpoint["hyper_parameters"]["backbone"]
         state_dict = checkpoint["state_dict"]
         state_dict = OrderedDict(
-            {k: v for k, v in state_dict.items() if "model.encoder.model" in k}
+            {k: v for k, v in state_dict.items() if "model.backbone.model" in k}
         )
         state_dict = OrderedDict(
-            {k.replace("model.encoder.model.", ""): v for k, v in state_dict.items()}
+            {k.replace("model.backbone.model.", ""): v for k, v in state_dict.items()}
         )
     else:
         raise ValueError(
-            "Unknown checkpoint task. Only encoder or classification_model"
-            " extraction is supported"
+            "Unknown checkpoint task. Only backbone or model extraction is supported"
         )
 
     return name, state_dict
 
 
 def load_state_dict(model: Module, state_dict: "OrderedDict[str, Tensor]") -> Module:
     """Load pretrained resnet weights to a model.
@@ -72,33 +66,35 @@
 
     Warns:
         If input channels in model != pretrained model input channels
         If num output classes in model != pretrained model num classes
     """
     in_channels = cast(nn.Module, model.conv1).in_channels
     expected_in_channels = state_dict["conv1.weight"].shape[1]
+
     num_classes = cast(nn.Module, model.fc).out_features
-    expected_num_classes = state_dict["fc.weight"].shape[0]
+    expected_num_classes = None
+    if "fc.weight" in state_dict:
+        expected_num_classes = state_dict["fc.weight"].shape[0]
 
     if in_channels != expected_in_channels:
         warnings.warn(
             f"input channels {in_channels} != input channels in pretrained"
             f" model {expected_in_channels}. Overriding with new input channels"
         )
         del state_dict["conv1.weight"]
 
-    if num_classes != expected_num_classes:
+    if expected_num_classes and num_classes != expected_num_classes:
         warnings.warn(
             f"num classes {num_classes} != num classes in pretrained model"
             f" {expected_num_classes}. Overriding with new num classes"
         )
         del state_dict["fc.weight"], state_dict["fc.bias"]
 
     model.load_state_dict(state_dict, strict=False)
-
     return model
 
 
 def reinit_initial_conv_layer(
     layer: Conv2d,
     new_in_channels: int,
     keep_rgb_weights: bool,
```

### Comparing `torchgeo-0.3.1/torchgeo/transforms/indices.py` & `torchgeo-0.4.0/torchgeo/transforms/indices.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,24 @@
 """TorchGeo indices transforms.
 
 For more information about indices see the following references:
 - https://www.indexdatabase.de/db/i.php
 - https://github.com/davemlz/awesome-spectral-indices
 """
 
-from typing import Dict
+from typing import Dict, Optional
 
 import torch
+from kornia.augmentation import IntensityAugmentationBase2D
 from torch import Tensor
-from torch.nn.modules import Module
-
-# https://github.com/pytorch/pytorch/issues/60979
-# https://github.com/pytorch/pytorch/pull/61045
-Module.__module__ = "torch.nn"
-
 
 _EPSILON = 1e-10
 
 
-class AppendNormalizedDifferenceIndex(Module):
+class AppendNormalizedDifferenceIndex(IntensityAugmentationBase2D):
     r"""Append normalized difference index as channel to image tensor.
 
     Computes the following index:
 
     .. math::
 
        \text{NDI} = \frac{A - B}{A + B}
@@ -37,50 +32,41 @@
     def __init__(self, index_a: int, index_b: int) -> None:
         """Initialize a new transform instance.
 
         Args:
             index_a: reference band channel index
             index_b: difference band channel index
         """
-        super().__init__()
-        self.dim = -3
-        self.index_a = index_a
-        self.index_b = index_b
-
-    def _compute_index(self, band_a: Tensor, band_b: Tensor) -> Tensor:
-        """Compute normalized difference index.
+        super().__init__(p=1)
+        self.flags = {"index_a": index_a, "index_b": index_b}
 
-        Args:
-            band_a: reference band tensor
-            band_b: difference band tensor
+    def apply_transform(
+        self,
+        input: Tensor,
+        params: Dict[str, Tensor],
+        flags: Dict[str, int],
+        transform: Optional[Tensor] = None,
+    ) -> Tensor:
+        """Apply the transform.
+
+        Args:
+            input: the input tensor
+            params: generated parameters
+            flags: static parameters
+            transform: the geometric transformation tensor
 
         Returns:
-            the index
+            the augmented input
         """
-        return (band_a - band_b) / ((band_a + band_b) + _EPSILON)
-
-    def forward(self, sample: Dict[str, Tensor]) -> Dict[str, Tensor]:
-        """Compute and append normalized difference index to image.
-
-        Args:
-            sample: a sample or batch dict
-
-        Returns:
-            the transformed sample
-        """
-        if "image" in sample:
-            index = self._compute_index(
-                band_a=sample["image"][..., self.index_a, :, :],
-                band_b=sample["image"][..., self.index_b, :, :],
-            )
-            index = index.unsqueeze(self.dim)
-
-            sample["image"] = torch.cat([sample["image"], index], dim=self.dim)
-
-        return sample
+        band_a = input[..., flags["index_a"], :, :]
+        band_b = input[..., flags["index_b"], :, :]
+        ndi = (band_a - band_b) / (band_a + band_b + _EPSILON)
+        ndi = torch.unsqueeze(ndi, -3)
+        input = torch.cat((input, ndi), dim=-3)
+        return input
 
 
 class AppendNBR(AppendNormalizedDifferenceIndex):
     r"""Normalized Burn Ratio (NBR).
 
     Computes the following index:
 
@@ -88,15 +74,15 @@
 
        \text{NBR} = \frac{\text{NIR} - \text{SWIR}}{\text{NIR} + \text{SWIR}}
 
     If you use this index in your research, please cite the following paper:
 
     * https://www.sciencebase.gov/catalog/item/4f4e4b20e4b07f02db6abb36
 
-    .. versionadded:: 0.2.0
+    .. versionadded:: 0.2
     """
 
     def __init__(self, index_nir: int, index_swir: int) -> None:
         """Initialize a new transform instance.
 
         Args:
             index_nir: index of the Near Infrared (NIR) band in the image
@@ -301,73 +287,63 @@
         Args:
             index_nir: index of the NIR band, e.g. B8 in Sentinel 2 imagery
             index_vre1: index of the Red Edge band, B5 in Sentinel 2 imagery
         """
         super().__init__(index_a=index_nir, index_b=index_vre1)
 
 
-class AppendTriBandNormalizedDifferenceIndex(Module):
+class AppendTriBandNormalizedDifferenceIndex(IntensityAugmentationBase2D):
     r"""Append normalized difference index involving 3 bands as channel to image tensor.
 
     Computes the following index:
 
     .. math::
 
-       \text{NDI} = \frac{A - (B + C)}{A + (B + C)}
+       \text{TBNDI} = \frac{A - (B + C)}{A + (B + C)}
 
     .. versionadded:: 0.3
     """
 
     def __init__(self, index_a: int, index_b: int, index_c: int) -> None:
         """Initialize a new transform instance.
 
         Args:
             index_a: reference band channel index
             index_b: difference band channel index of component 1
             index_c: difference band channel index of component 2
         """
-        super().__init__()
-        self.dim = -3
-        self.index_a = index_a
-        self.index_b = index_b
-        self.index_c = index_c
-
-    def _compute_index(self, band_a: Tensor, band_b: Tensor, band_c: Tensor) -> Tensor:
-        """Compute tri-band normalized difference index.
+        super().__init__(p=1)
+        self.flags = {"index_a": index_a, "index_b": index_b, "index_c": index_c}
 
-        Args:
-            band_a: reference band tensor
-            band_b: difference band tensor component 1
-            band_c: difference band tensor component 2
+    def apply_transform(
+        self,
+        input: Tensor,
+        params: Dict[str, Tensor],
+        flags: Dict[str, int],
+        transform: Optional[Tensor] = None,
+    ) -> Tensor:
+        """Apply the transform.
+
+        Args:
+            input: the input tensor
+            params: generated parameters
+            flags: static parameters
+            transform: the geometric transformation tensor
 
         Returns:
-            the index
+            the augmented input
         """
-        return (band_a - (band_b + band_c)) / ((band_a + band_b + band_c) + _EPSILON)
-
-    def forward(self, sample: Dict[str, Tensor]) -> Dict[str, Tensor]:
-        """Compute and append tri-band normalized difference index to image.
-
-        Args:
-            sample: a sample or batch dict
-
-        Returns:
-            the transformed sample
-        """
-        if "image" in sample:
-            index = self._compute_index(
-                band_a=sample["image"][..., self.index_a, :, :],
-                band_b=sample["image"][..., self.index_b, :, :],
-                band_c=sample["image"][..., self.index_c, :, :],
-            )
-            index = index.unsqueeze(self.dim)
-
-            sample["image"] = torch.cat([sample["image"], index], dim=self.dim)
-
-        return sample
+        band_a = input[..., flags["index_a"], :, :]
+        band_b = input[..., flags["index_b"], :, :]
+        band_c = input[..., flags["index_c"], :, :]
+        band_d = band_b + band_c
+        tbndi = (band_a - band_d) / (band_a + band_d + _EPSILON)
+        tbndi = torch.unsqueeze(tbndi, -3)
+        input = torch.cat((input, tbndi), dim=-3)
+        return input
 
 
 class AppendGRNDVI(AppendTriBandNormalizedDifferenceIndex):
     r"""Green-Red Normalized Difference Vegetation Index (GRNDVI).
 
     Computes the following index:
```

### Comparing `torchgeo-0.3.1/torchgeo.egg-info/PKG-INFO` & `torchgeo-0.4.0/torchgeo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgeo
-Version: 0.3.1
+Version: 0.4.0
 Summary: TorchGeo: datasets, samplers, transforms, and pre-trained models for geospatial data
 Home-page: https://github.com/microsoft/torchgeo
 Author: Adam J. Stewart
 Author-email: ajstewart426@gmail.com
 Keywords: pytorch,deep learning,machine learning,remote sensing,satellite imagery,earth observation,geospatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -53,15 +53,15 @@
 $ pip install torchgeo
 ```
 
 For [conda](https://docs.conda.io/) and [spack](https://spack.io/) installation instructions, see the [documentation](https://torchgeo.readthedocs.io/en/stable/user/installation.html).
 
 ## Documentation
 
-You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://arxiv.org/abs/2111.08872) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
+You can find the documentation for TorchGeo on [ReadTheDocs](https://torchgeo.readthedocs.io). This includes API documentation, contributing instructions, and several [tutorials](https://torchgeo.readthedocs.io/en/stable/tutorials/getting_started.html). For more details, check out our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953) and [blog](https://pytorch.org/blog/geospatial-deep-learning-with-torchgeo/).
 
 ## Example Usage
 
 The following sections give basic examples of what you can do with TorchGeo.
 
 First we'll import various classes and functions used in the following sections:
 
@@ -137,24 +137,24 @@
 for batch in dataloader:
     image = batch["image"]
     label = batch["label"]
 
     # train a model, or make predictions using a pre-trained model
 ```
 
-<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the NWPU VHR-10 dataset"/>
+<img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/vhr10.png" alt="Example predictions from a Mask R-CNN model trained on the VHR-10 dataset"/>
 
 All TorchGeo datasets are compatible with PyTorch data loaders, making them easy to integrate into existing training workflows. The only difference between a benchmark dataset in TorchGeo and a similar dataset in torchvision is that each dataset returns a dictionary with keys for each PyTorch `Tensor`.
 
 ### Reproducibility with PyTorch Lightning
 
 In order to facilitate direct comparisons between results published in the literature and further reduce the boilerplate code needed to run experiments with datasets in TorchGeo, we have created PyTorch Lightning [*datamodules*](https://torchgeo.readthedocs.io/en/stable/api/datamodules.html) with well-defined train-val-test splits and [*trainers*](https://torchgeo.readthedocs.io/en/stable/api/trainers.html) for various tasks like classification, regression, and semantic segmentation. These datamodules show how to incorporate augmentations from the kornia library, include preprocessing transforms (with pre-calculated channel statistics), and let users easily experiment with hyperparameters related to the data itself (as opposed to the modeling process). Training a semantic segmentation model on the [Inria Aerial Image Labeling](https://project.inria.fr/aerialimagelabeling/) dataset is as easy as a few imports and four lines of code.
 
 ```python
-datamodule = InriaAerialImageLabelingDataModule(root_dir="...", batch_size=64, num_workers=6)
+datamodule = InriaAerialImageLabelingDataModule(root="...", batch_size=64, num_workers=6)
 task = SemanticSegmentationTask(segmentation_model="unet", encoder_weights="imagenet", learning_rate=0.1)
 trainer = Trainer(gpus=1, default_root_dir="...")
 
 trainer.fit(model=task, datamodule=datamodule)
 ```
 
 <img src="https://raw.githubusercontent.com/microsoft/torchgeo/main/images/inria.png" alt="Building segmentations produced by a U-Net model trained on the Inria Aerial Image Labeling dataset"/>
@@ -163,23 +163,28 @@
 
 ```console
 $ python train.py config_file=conf/landcoverai.yaml
 ```
 
 ## Citation
 
-If you use this software in your work, please cite our [paper](https://arxiv.org/abs/2111.08872):
+If you use this software in your work, please cite our [paper](https://dl.acm.org/doi/10.1145/3557915.3560953):
 ```
-@article{Stewart_TorchGeo_deep_learning_2021,
+@inproceedings{Stewart_TorchGeo_Deep_Learning_2022,
+    address = {Seattle, Washington},
     author = {Stewart, Adam J. and Robinson, Caleb and Corley, Isaac A. and Ortiz, Anthony and Lavista Ferres, Juan M. and Banerjee, Arindam},
-    journal = {arXiv preprint arXiv:2111.08872},
+    booktitle = {Proceedings of the 30th International Conference on Advances in Geographic Information Systems},
+    doi = {10.1145/3557915.3560953},
     month = {11},
+    pages = {1--12},
+    publisher = {Association for Computing Machinery},
+    series = {SIGSPATIAL '22},
     title = {{TorchGeo}: Deep Learning With Geospatial Data},
-    url = {https://github.com/microsoft/torchgeo},
-    year = {2021}
+    url = {https://dl.acm.org/doi/10.1145/3557915.3560953},
+    year = {2022}
 }
 ```
 
 ## Contributing
 
 This project welcomes contributions and suggestions. If you would like to submit a pull request, see our [Contribution Guide](https://torchgeo.readthedocs.io/en/stable/user/contributing.html) for more information.
```

### Comparing `torchgeo-0.3.1/torchgeo.egg-info/SOURCES.txt` & `torchgeo-0.4.0/torchgeo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,38 +14,42 @@
 torchgeo/datamodules/chesapeake.py
 torchgeo/datamodules/cowc.py
 torchgeo/datamodules/cyclone.py
 torchgeo/datamodules/deepglobelandcover.py
 torchgeo/datamodules/etci2021.py
 torchgeo/datamodules/eurosat.py
 torchgeo/datamodules/fair1m.py
+torchgeo/datamodules/geo.py
+torchgeo/datamodules/gid15.py
 torchgeo/datamodules/inria.py
 torchgeo/datamodules/landcoverai.py
 torchgeo/datamodules/loveda.py
 torchgeo/datamodules/naip.py
 torchgeo/datamodules/nasa_marine_debris.py
 torchgeo/datamodules/oscd.py
 torchgeo/datamodules/potsdam.py
 torchgeo/datamodules/resisc45.py
 torchgeo/datamodules/sen12ms.py
 torchgeo/datamodules/so2sat.py
+torchgeo/datamodules/spacenet.py
 torchgeo/datamodules/ucmerced.py
 torchgeo/datamodules/usavars.py
 torchgeo/datamodules/utils.py
 torchgeo/datamodules/vaihingen.py
 torchgeo/datamodules/xview.py
 torchgeo/datasets/__init__.py
 torchgeo/datasets/advance.py
 torchgeo/datasets/agb_live_woody_density.py
 torchgeo/datasets/astergdem.py
 torchgeo/datasets/benin_cashews.py
 torchgeo/datasets/bigearthnet.py
 torchgeo/datasets/cbf.py
 torchgeo/datasets/cdl.py
 torchgeo/datasets/chesapeake.py
+torchgeo/datasets/cloud_cover.py
 torchgeo/datasets/cms_mangrove_canopy.py
 torchgeo/datasets/cowc.py
 torchgeo/datasets/cv4a_kenya_crop_type.py
 torchgeo/datasets/cyclone.py
 torchgeo/datasets/deepglobelandcover.py
 torchgeo/datasets/dfc2022.py
 torchgeo/datasets/eddmaps.py
@@ -66,15 +70,14 @@
 torchgeo/datasets/landcoverai.py
 torchgeo/datasets/landsat.py
 torchgeo/datasets/levircd.py
 torchgeo/datasets/loveda.py
 torchgeo/datasets/millionaid.py
 torchgeo/datasets/naip.py
 torchgeo/datasets/nasa_marine_debris.py
-torchgeo/datasets/nwpu.py
 torchgeo/datasets/openbuildings.py
 torchgeo/datasets/oscd.py
 torchgeo/datasets/patternnet.py
 torchgeo/datasets/potsdam.py
 torchgeo/datasets/reforestree.py
 torchgeo/datasets/resisc45.py
 torchgeo/datasets/seco.py
@@ -82,32 +85,36 @@
 torchgeo/datasets/sentinel.py
 torchgeo/datasets/so2sat.py
 torchgeo/datasets/spacenet.py
 torchgeo/datasets/ucmerced.py
 torchgeo/datasets/usavars.py
 torchgeo/datasets/utils.py
 torchgeo/datasets/vaihingen.py
+torchgeo/datasets/vhr10.py
 torchgeo/datasets/xview.py
 torchgeo/datasets/zuericrop.py
 torchgeo/losses/__init__.py
 torchgeo/losses/qr.py
 torchgeo/models/__init__.py
+torchgeo/models/api.py
 torchgeo/models/changestar.py
 torchgeo/models/farseg.py
 torchgeo/models/fcn.py
 torchgeo/models/fcsiam.py
 torchgeo/models/rcf.py
 torchgeo/models/resnet.py
+torchgeo/models/vit.py
 torchgeo/samplers/__init__.py
 torchgeo/samplers/batch.py
 torchgeo/samplers/constants.py
 torchgeo/samplers/single.py
 torchgeo/samplers/utils.py
 torchgeo/trainers/__init__.py
 torchgeo/trainers/byol.py
 torchgeo/trainers/classification.py
+torchgeo/trainers/detection.py
 torchgeo/trainers/regression.py
 torchgeo/trainers/segmentation.py
 torchgeo/trainers/utils.py
 torchgeo/transforms/__init__.py
 torchgeo/transforms/indices.py
 torchgeo/transforms/transforms.py
```

### Comparing `torchgeo-0.3.1/torchgeo.egg-info/requires.txt` & `torchgeo-0.4.0/torchgeo.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-einops<0.5,>=0.3
+einops<0.7,>=0.3
 fiona<2,>=1.8
-kornia<0.7,>=0.6.4
+kornia<0.7,>=0.6.5
 matplotlib<4,>=3.3
 numpy<2,>=1.17.2
 omegaconf<3,>=2.1
-packaging<22,>=17
 pillow<10,>=6.2
 pyproj<4,>=2.2
-pytorch-lightning<2,>=1.5.1
+pytorch-lightning[extra]<2,>=1.5.1
 rasterio<2,>=1.0.20
 rtree<2,>=1
 scikit-learn<2,>=0.21
 segmentation-models-pytorch<0.4,>=0.2
-shapely<2,>=1.3
-timm<0.5,>=0.4.12
-torch<2,>=1.9
-torchmetrics<0.10,>=0.7
-torchvision<0.14,>=0.10
+shapely<3,>=1.3
+timm<0.7,>=0.4.12
+torch<2,>=1.12
+torchmetrics<0.12,>=0.10
+torchvision<0.15,>=0.13
 
 [datasets]
 h5py<4,>=2.6
 laspy<3,>=2
 opencv-python<5,>=3.4.2.17
 pandas<2,>=0.23.2
 pycocotools<3,>=2
+pyvista<0.38,>=0.20
 radiant-mlhub<0.5,>=0.2.1
 rarfile<5,>=3
-scipy<2,>=1.2
+scikit-image<0.20,>=0.18
+scipy<2,>=1.6.2
 zipfile-deflate64<0.3,>=0.2
 
-[datasets:python_version < "3.10"]
-open3d<0.15,>=0.11.2
-
 [docs]
 ipywidgets<9,>=7
 nbsphinx<0.9,>=0.8.5
 pytorch-sphinx-theme
-sphinx<6,>=4
+sphinx<7,>=4
 
 [style]
 black[jupyter]<23,>=21.8
-flake8<6,>=3.8
+flake8<7,>=3.8
 isort[colors]<6,>=5.8
 pydocstyle[toml]<7,>=6.1
-pyupgrade<3,>=1.24
+pyupgrade<4,>=1.24
 
 [tests]
-mypy<0.972,>=0.900
+mypy<0.992,>=0.900
 nbmake<2,>=0.1
 pytest<8,>=6.1.2
-pytest-cov<4,>=2.4
+pytest-cov<5,>=2.4
```

