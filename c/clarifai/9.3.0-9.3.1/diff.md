# Comparing `tmp/clarifai-9.3.0.tar.gz` & `tmp/clarifai-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.3.0.tar", last modified: Mon Apr  3 17:28:50 2023, max compression
+gzip compressed data, was "clarifai-9.3.1.tar", last modified: Tue Apr 11 15:56:54 2023, max compression
```

## Comparing `clarifai-9.3.0.tar` & `clarifai-9.3.1.tar`

### file list

```diff
@@ -1,90 +1,97 @@
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.978394 clarifai-9.3.0/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-01-17 09:53:52.000000 clarifai-9.3.0/LICENSE
--rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-01-17 09:53:52.000000 clarifai-9.3.0/MANIFEST.in
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-04-03 17:28:50.977886 clarifai-9.3.0/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-01-17 09:53:52.000000 clarifai-9.3.0/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.934040 clarifai-9.3.0/clarifai/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.937933 clarifai-9.3.0/clarifai/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12387 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.940534 clarifai-9.3.0/clarifai/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.942608 clarifai-9.3.0/clarifai/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.947116 clarifai-9.3.0/clarifai/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1089 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     9235 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.949613 clarifai-9.3.0/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10917 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.955912 clarifai-9.3.0/clarifai/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7710 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.957885 clarifai-9.3.0/clarifai/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai/modules/pages.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.936946 clarifai-9.3.0/clarifai.egg-info/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-04-03 17:28:50.000000 clarifai-9.3.0/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2416 2023-04-03 17:28:50.000000 clarifai-9.3.0/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-04-03 17:28:50.000000 clarifai-9.3.0/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-04-03 17:28:50.000000 clarifai-9.3.0/clarifai.egg-info/requires.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-04-03 17:28:50.000000 clarifai-9.3.0/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.958906 clarifai-9.3.0/clarifai_utils/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.960050 clarifai-9.3.0/clarifai_utils/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12387 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.961690 clarifai-9.3.0/clarifai_utils/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.963133 clarifai-9.3.0/clarifai_utils/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.966064 clarifai-9.3.0/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1089 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     9235 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.968634 clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10917 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.974231 clarifai-9.3.0/clarifai_utils/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7710 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-04-03 17:20:53.000000 clarifai-9.3.0/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-04-03 17:28:50.976791 clarifai-9.3.0/clarifai_utils/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-01-17 09:53:52.000000 clarifai-9.3.0/clarifai_utils/modules/pages.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4131 2023-03-01 14:52:28.000000 clarifai-9.3.0/clarifai_utils/modules/style.css
--rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-04-03 17:28:50.978634 clarifai-9.3.0/setup.cfg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      887 2023-04-03 17:28:40.000000 clarifai-9.3.0/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734809 clarifai-9.3.1/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.3.1/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.3.1/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-11 15:56:54.734598 clarifai-9.3.1/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.3.1/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.721911 clarifai-9.3.1/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.722861 clarifai-9.3.1/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.723595 clarifai-9.3.1/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.724118 clarifai-9.3.1/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.725368 clarifai-9.3.1/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.726019 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.727920 clarifai-9.3.1/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7710 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.728681 clarifai-9.3.1/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729052 clarifai-9.3.1/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.1/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.1/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.722612 clarifai-9.3.1/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2555 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-04-11 15:56:54.000000 clarifai-9.3.1/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729314 clarifai-9.3.1/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729546 clarifai-9.3.1/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.729960 clarifai-9.3.1/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.730339 clarifai-9.3.1/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.731032 clarifai-9.3.1/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.731654 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.733324 clarifai-9.3.1/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7710 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.3.1/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734064 clarifai-9.3.1/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.3.1/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.3.1/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-04-11 15:56:54.734373 clarifai-9.3.1/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.3.1/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.3.1/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-04-11 15:56:54.734866 clarifai-9.3.1/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)      887 2023-04-11 15:55:59.000000 clarifai-9.3.1/setup.py
```

### Comparing `clarifai-9.3.0/LICENSE` & `clarifai-9.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/PKG-INFO` & `clarifai-9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.0
+Version: 9.3.1
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.0/README.md` & `clarifai-9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/auth/helper.py` & `clarifai-9.3.1/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/client/abc.py` & `clarifai-9.3.1/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/client/stub.py` & `clarifai-9.3.1/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/base.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/features.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/image.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/text.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/examples.py` & `clarifai-9.3.1/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/data_upload/upload.py` & `clarifai-9.3.1/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/concepts.py` & `clarifai-9.3.1/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/datasets.py` & `clarifai-9.3.1/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/inputs.py` & `clarifai-9.3.1/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/installed_module_versions.py` & `clarifai-9.3.1/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/lister.py` & `clarifai-9.3.1/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/models.py` & `clarifai-9.3.1/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/module_versions.py` & `clarifai-9.3.1/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/listing/modules.py` & `clarifai-9.3.1/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/modules/css.py` & `clarifai-9.3.1/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai/modules/pages.py` & `clarifai-9.3.1/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai.egg-info/PKG-INFO` & `clarifai-9.3.1/clarifai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.3.0
+Version: 9.3.1
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.3.0/clarifai.egg-info/SOURCES.txt` & `clarifai-9.3.1/clarifai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 clarifai/listing/lister.py
 clarifai/listing/models.py
 clarifai/listing/module_versions.py
 clarifai/listing/modules.py
 clarifai/modules/__init__.py
 clarifai/modules/css.py
 clarifai/modules/pages.py
+clarifai/modules/style.css
+clarifai/urls/__init__.py
+clarifai/urls/helper.py
 clarifai_utils/__init__.py
 clarifai_utils/auth/__init__.py
 clarifai_utils/auth/helper.py
 clarifai_utils/client/__init__.py
 clarifai_utils/client/abc.py
 clarifai_utils/client/stub.py
 clarifai_utils/data_upload/__init__.py
@@ -63,8 +66,10 @@
 clarifai_utils/listing/lister.py
 clarifai_utils/listing/models.py
 clarifai_utils/listing/module_versions.py
 clarifai_utils/listing/modules.py
 clarifai_utils/modules/__init__.py
 clarifai_utils/modules/css.py
 clarifai_utils/modules/pages.py
-clarifai_utils/modules/style.css
+clarifai_utils/modules/style.css
+clarifai_utils/urls/__init__.py
+clarifai_utils/urls/helper.py
```

### Comparing `clarifai-9.3.0/clarifai_utils/auth/helper.py` & `clarifai-9.3.1/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/client/abc.py` & `clarifai-9.3.1/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/client/stub.py` & `clarifai-9.3.1/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.3.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/examples.py` & `clarifai-9.3.1/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/data_upload/upload.py` & `clarifai-9.3.1/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/concepts.py` & `clarifai-9.3.1/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/datasets.py` & `clarifai-9.3.1/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/inputs.py` & `clarifai-9.3.1/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.3.1/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/lister.py` & `clarifai-9.3.1/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/models.py` & `clarifai-9.3.1/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/module_versions.py` & `clarifai-9.3.1/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/listing/modules.py` & `clarifai-9.3.1/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/modules/css.py` & `clarifai-9.3.1/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/modules/pages.py` & `clarifai-9.3.1/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/clarifai_utils/modules/style.css` & `clarifai-9.3.1/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.3.0/setup.py` & `clarifai-9.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.3.0",
+    version="9.3.1",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

