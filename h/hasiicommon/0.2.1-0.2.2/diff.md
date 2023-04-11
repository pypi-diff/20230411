# Comparing `tmp/hasiicommon-0.2.1.tar.gz` & `tmp/hasiicommon-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasiicommon-0.2.1.tar", last modified: Wed Mar 29 22:09:09 2023, max compression
+gzip compressed data, was "hasiicommon-0.2.2.tar", last modified: Tue Apr 11 20:51:40 2023, max compression
```

## Comparing `hasiicommon-0.2.1.tar` & `hasiicommon-0.2.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.140161 hasiicommon-0.2.1/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-02-08 21:38:24.000000 hasiicommon-0.2.1/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1604 2023-03-29 22:09:09.140044 hasiicommon-0.2.1/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1239 2023-03-26 21:16:33.000000 hasiicommon-0.2.1/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.131259 hasiicommon-0.2.1/hasiicommon/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiicommon-0.2.1/hasiicommon/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.132040 hasiicommon-0.2.1/hasiicommon/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:51:36.000000 hasiicommon-0.2.1/hasiicommon/resources/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.132343 hasiicommon-0.2.1/hasiicommon/resources/images/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2774 2021-02-03 02:11:03.000000 hasiicommon-0.2.1/hasiicommon/resources/images/DefaultPreferences.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 16:13:15.000000 hasiicommon-0.2.1/hasiicommon/resources/images/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.132439 hasiicommon-0.2.1/hasiicommon/resources/images/icons/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-10-17 00:02:24.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.135512 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8370 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1334 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1186 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1330 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1170 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8522 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1286 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1378 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1098 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1102 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1122 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1066 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1114 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1482 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1046 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1402 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8346 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1382 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1366 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.138825 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-24 17:56:38.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1522 2021-01-24 17:56:39.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1742 2021-01-24 17:56:39.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9478 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9878 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9486 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      962 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2410 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2770 2021-01-24 17:56:44.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8570 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8226 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      714 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8254 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2954 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8846 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8582 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1666 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2762 2021-01-24 17:56:54.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2021-01-24 17:56:55.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3198 2021-01-25 02:00:22.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3166 2021-01-24 17:56:56.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/resources/images/py.typed
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/resources/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.139176 hasiicommon-0.2.1/hasiicommon/ui/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      739 2023-03-26 22:09:23.000000 hasiicommon-0.2.1/hasiicommon/ui/UnitTestBaseW.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:39.000000 hasiicommon-0.2.1/hasiicommon/ui/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/ui/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.139916 hasiicommon-0.2.1/hasiicommon/ui/widgets/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2384 2023-03-26 21:09:16.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/DimensionsControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      224 2022-11-09 03:57:30.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/DirectionEnum.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-09 02:19:53.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/DualSpinnerControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2306 2023-03-26 21:09:22.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/PositionControl.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:58.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.1/hasiicommon/ui/widgets/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 22:09:09.131832 hasiicommon-0.2.1/hasiicommon.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1604 2023-03-29 22:09:09.000000 hasiicommon-0.2.1/hasiicommon.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4526 2023-03-29 22:09:09.000000 hasiicommon-0.2.1/hasiicommon.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-29 22:09:09.000000 hasiicommon-0.2.1/hasiicommon.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       54 2023-03-29 22:09:09.000000 hasiicommon-0.2.1/hasiicommon.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-03-29 22:09:09.000000 hasiicommon-0.2.1/hasiicommon.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-29 22:09:09.140195 hasiicommon-0.2.1/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1556 2023-03-29 22:07:43.000000 hasiicommon-0.2.1/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.646577 hasiicommon-0.2.2/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-02-08 21:38:24.000000 hasiicommon-0.2.2/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-04-11 20:51:40.646456 hasiicommon-0.2.2/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1608 2023-04-11 01:34:23.000000 hasiicommon-0.2.2/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.637791 hasiicommon-0.2.2/hasiicommon/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:24.000000 hasiicommon-0.2.2/hasiicommon/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.638576 hasiicommon-0.2.2/hasiicommon/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 15:51:36.000000 hasiicommon-0.2.2/hasiicommon/resources/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.638884 hasiicommon-0.2.2/hasiicommon/resources/images/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2774 2021-02-03 02:11:03.000000 hasiicommon-0.2.2/hasiicommon/resources/images/DefaultPreferences.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-09 16:13:15.000000 hasiicommon-0.2.2/hasiicommon/resources/images/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.638982 hasiicommon-0.2.2/hasiicommon/resources/images/icons/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2020-10-17 00:02:24.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.642084 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8370 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1334 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1186 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1330 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1170 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8522 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1286 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1378 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1098 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1102 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1122 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1066 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1114 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1482 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1162 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1046 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1402 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8346 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1382 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1366 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.645288 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1190 2021-01-24 17:56:38.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1522 2021-01-24 17:56:39.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1742 2021-01-24 17:56:39.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9478 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3210 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9878 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     9486 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      962 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2410 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2770 2021-01-24 17:56:44.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8570 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8226 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      714 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8254 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8446 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2954 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8846 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8582 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1666 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2762 2021-01-24 17:56:54.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1662 2021-01-24 17:56:55.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3198 2021-01-25 02:00:22.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3166 2021-01-24 17:56:56.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2021-01-19 21:01:31.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/resources/images/py.typed
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/resources/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.645605 hasiicommon-0.2.2/hasiicommon/ui/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      739 2023-03-26 22:09:23.000000 hasiicommon-0.2.2/hasiicommon/ui/UnitTestBaseW.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:39.000000 hasiicommon-0.2.2/hasiicommon/ui/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/ui/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.646306 hasiicommon-0.2.2/hasiicommon/ui/widgets/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2384 2023-03-26 21:09:16.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/DimensionsControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      224 2022-11-09 03:57:30.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/DirectionEnum.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4602 2023-02-09 02:19:53.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/DualSpinnerControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2306 2023-03-26 21:09:22.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/PositionControl.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-08 21:59:58.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-08 16:33:36.000000 hasiicommon-0.2.2/hasiicommon/ui/widgets/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 20:51:40.638375 hasiicommon-0.2.2/hasiicommon.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-04-11 20:51:40.000000 hasiicommon-0.2.2/hasiicommon.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4526 2023-04-11 20:51:40.000000 hasiicommon-0.2.2/hasiicommon.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-11 20:51:40.000000 hasiicommon-0.2.2/hasiicommon.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       54 2023-04-11 20:51:40.000000 hasiicommon-0.2.2/hasiicommon.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-11 20:51:40.000000 hasiicommon-0.2.2/hasiicommon.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-11 20:51:40.646614 hasiicommon-0.2.2/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1557 2023-04-11 20:41:23.000000 hasiicommon-0.2.2/setup.py
```

### Comparing `hasiicommon-0.2.1/LICENSE` & `hasiicommon-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/PKG-INFO` & `hasiicommon-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6861 7369  : 2.1.Name: hasi
 00000020: 6963 6f6d 6d6f 6e0a 5665 7273 696f 6e3a  icommon.Version:
-00000030: 2030 2e32 2e31 0a53 756d 6d61 7279 3a20   0.2.1.Summary: 
+00000030: 2030 2e32 2e32 0a53 756d 6d61 7279 3a20   0.2.2.Summary: 
 00000040: 4875 6d62 6572 746f 6073 2043 6f6d 6d6f  Humberto`s Commo
 00000050: 6e20 5374 7566 660a 486f 6d65 2d70 6167  n Stuff.Home-pag
 00000060: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000070: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
 00000080: 6861 7369 6963 6f6d 6d6f 6e0a 4175 7468  hasiicommon.Auth
 00000090: 6f72 3a20 4875 6d62 6572 746f 2041 2e20  or: Humberto A. 
 000000a0: 5361 6e63 6865 7a20 4949 0a41 7574 686f  Sanchez II.Autho
@@ -44,58 +44,81 @@
 000002b0: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
 000002c0: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
 000002d0: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
 000002e0: 7974 686f 6e2e 6f72 672f 290a 0a48 6f73  ython.org/)..Hos
 000002f0: 7420 636f 6d6d 6f6e 2055 4920 6172 7469  t common UI arti
 00000300: 6661 6374 7320 666f 7220 7661 7269 6f75  facts for variou
 00000310: 7320 7072 6f6a 6563 7473 2049 2061 6d20  s projects I am 
-00000320: 6465 7665 6c6f 7069 6e67 0a0a 0a21 5b48  developing...![H
-00000330: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
-00000340: 6564 204c 6f67 6f5d 282e 2f64 6576 656c  ed Logo](./devel
-00000350: 6f70 6572 2f53 696c 6c79 4769 7448 7562  oper/SillyGitHub
-00000360: 2e70 6e67 290a 0a49 2061 6d20 636f 6e63  .png)..I am conc
-00000370: 6572 6e65 6420 6162 6f75 7420 4769 7448  erned about GitH
-00000380: 7562 2773 2043 6f70 696c 6f74 2070 726f  ub's Copilot pro
-00000390: 6a65 6374 0a0a 0a0a 4920 7572 6765 2079  ject....I urge y
-000003a0: 6f75 2074 6f20 7265 6164 2061 626f 7574  ou to read about
-000003b0: 2074 6865 0a5b 4769 7665 2075 7020 4769   the.[Give up Gi
-000003c0: 7448 7562 5d28 6874 7470 733a 2f2f 4769  tHub](https://Gi
-000003d0: 7665 5570 4769 7448 7562 2e6f 7267 2920  veUpGitHub.org) 
-000003e0: 6361 6d70 6169 676e 2066 726f 6d0a 5b74  campaign from.[t
-000003f0: 6865 2053 6f66 7477 6172 6520 4672 6565  he Software Free
-00000400: 646f 6d20 436f 6e73 6572 7661 6e63 795d  dom Conservancy]
-00000410: 2868 7474 7073 3a2f 2f73 6663 6f6e 7365  (https://sfconse
-00000420: 7276 616e 6379 2e6f 7267 292e 0a0a 5768  rvancy.org)...Wh
-00000430: 696c 6520 4920 646f 206e 6f74 2061 6476  ile I do not adv
-00000440: 6f63 6174 6520 666f 7220 616c 6c20 7468  ocate for all th
-00000450: 6520 6973 7375 6573 206c 6973 7465 6420  e issues listed 
-00000460: 7468 6572 6520 4920 646f 206e 6f74 206c  there I do not l
-00000470: 696b 6520 7468 6174 0a61 2063 6f6d 7061  ike that.a compa
-00000480: 6e79 206c 696b 6520 4d69 6372 6f73 6f66  ny like Microsof
-00000490: 7420 6d61 7920 7072 6f66 6974 2066 726f  t may profit fro
-000004a0: 6d20 6f70 656e 2073 6f75 7263 6520 7072  m open source pr
-000004b0: 6f6a 6563 7473 2e0a 0a49 2063 6f6e 7469  ojects...I conti
-000004c0: 6e75 6520 746f 2075 7365 2047 6974 4875  nue to use GitHu
-000004d0: 6220 6265 6361 7573 6520 6974 206f 6666  b because it off
-000004e0: 6572 7320 7468 6520 7365 7276 6963 6573  ers the services
-000004f0: 2049 206e 6565 6420 666f 7220 6672 6565   I need for free
-00000500: 2e20 2042 7574 2c20 4920 636f 6e74 696e  .  But, I contin
-00000510: 7565 0a74 6f20 6d6f 6e69 746f 7220 7468  ue.to monitor th
-00000520: 6569 7220 7465 726d 7320 6f66 2073 6572  eir terms of ser
-00000530: 7669 6365 2e0a 0a41 6e79 2075 7365 206f  vice...Any use o
-00000540: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-00000550: 2063 6f64 6520 6279 2047 6974 4875 6220   code by GitHub 
-00000560: 436f 7069 6c6f 742c 2070 6173 7420 6f72  Copilot, past or
-00000570: 2070 7265 7365 6e74 2c20 6973 2064 6f6e   present, is don
-00000580: 650a 7769 7468 6f75 7420 6d79 2070 6572  e.without my per
-00000590: 6d69 7373 696f 6e2e 2020 4920 646f 206e  mission.  I do n
-000005a0: 6f74 2063 6f6e 7365 6e74 2074 6f20 4769  ot consent to Gi
-000005b0: 7448 7562 2773 2075 7365 206f 6620 7468  tHub's use of th
-000005c0: 6973 2070 726f 6a65 6374 2773 0a63 6f64  is project's.cod
-000005d0: 6520 696e 2043 6f70 696c 6f74 2e0a 0a41  e in Copilot...A
-000005e0: 2072 6570 6f73 6974 6f72 7920 6f77 6e65   repository owne
-000005f0: 7220 6d61 7920 6f70 7420 6f75 7420 6f66  r may opt out of
-00000600: 2043 6f70 696c 6f74 2062 7920 6368 616e   Copilot by chan
-00000610: 6769 6e67 2053 6574 7469 6e67 7320 2d2d  ging Settings --
-00000620: 3e20 4769 7448 7562 2043 6f70 696c 6f74  > GitHub Copilot
-00000630: 2e0a 0a49 2068 6176 6520 646f 6e65 2073  ...I have done s
-00000640: 6f2e 0a0a                                o...
+00000320: 6465 7665 6c6f 7069 6e67 0a0a 5f5f 5f0a  developing..___.
+00000330: 0a57 7269 7474 656e 2062 7920 3c61 2068  .Written by <a h
+00000340: 7265 663d 226d 6169 6c74 6f3a 656d 6169  ref="mailto:emai
+00000350: 6c40 6875 6d62 6572 746f 2e61 2e73 616e  l@humberto.a.san
+00000360: 6368 657a 2e69 6940 676d 6169 6c2e 636f  chez.ii@gmail.co
+00000370: 6d3f 7375 626a 6563 743d 4865 6c6c 6f20  m?subject=Hello 
+00000380: 4875 6d62 6572 746f 223e 4875 6d62 6572  Humberto">Humber
+00000390: 746f 2041 2e20 5361 6e63 6865 7a20 4949  to A. Sanchez II
+000003a0: 3c2f 613e 2020 2843 2920 3230 3233 0a0a  </a>  (C) 2023..
+000003b0: 2323 204e 6f74 650a 466f 7220 616c 6c20  ## Note.For all 
+000003c0: 6b69 6e64 206f 6620 7072 6f62 6c65 6d73  kind of problems
+000003d0: 2c20 7265 7175 6573 7473 2c20 656e 6861  , requests, enha
+000003e0: 6e63 656d 656e 7473 2c20 6275 6720 7265  ncements, bug re
+000003f0: 706f 7274 732c 2065 7463 2e2c 0a70 6c65  ports, etc.,.ple
+00000400: 6173 6520 6472 6f70 206d 6520 616e 2065  ase drop me an e
+00000410: 2d6d 6169 6c2e 0a0a 2323 2044 6576 656c  -mail...## Devel
+00000420: 6f70 6572 204e 6f74 6573 0a54 6869 7320  oper Notes.This 
+00000430: 7072 6f6a 6563 7420 7573 6573 205b 6275  project uses [bu
+00000440: 696c 646c 6163 6b65 795d 2868 7474 7073  ildlackey](https
+00000450: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
+00000460: 7369 6932 3031 312f 6275 696c 646c 6163  sii2011/buildlac
+00000470: 6b65 7929 2066 6f72 2064 6179 2074 6f20  key) for day to 
+00000480: 6461 7920 6465 7665 6c6f 706d 656e 7420  day development 
+00000490: 6275 696c 6473 0a0a 2d2d 2d0a 0a0a 215b  builds..---...![
+000004a0: 4875 6d62 6572 746f 2773 204d 6f64 6966  Humberto's Modif
+000004b0: 6965 6420 4c6f 676f 5d28 2e2f 6465 7665  ied Logo](./deve
+000004c0: 6c6f 7065 722f 5369 6c6c 7947 6974 4875  loper/SillyGitHu
+000004d0: 622e 706e 6729 0a0a 4920 616d 2063 6f6e  b.png)..I am con
+000004e0: 6365 726e 6564 2061 626f 7574 2047 6974  cerned about Git
+000004f0: 4875 6227 7320 436f 7069 6c6f 7420 7072  Hub's Copilot pr
+00000500: 6f6a 6563 740a 0a0a 0a49 2075 7267 6520  oject....I urge 
+00000510: 796f 7520 746f 2072 6561 6420 6162 6f75  you to read abou
+00000520: 7420 7468 650a 5b47 6976 6520 7570 2047  t the.[Give up G
+00000530: 6974 4875 625d 2868 7474 7073 3a2f 2f47  itHub](https://G
+00000540: 6976 6555 7047 6974 4875 622e 6f72 6729  iveUpGitHub.org)
+00000550: 2063 616d 7061 6967 6e20 6672 6f6d 0a5b   campaign from.[
+00000560: 7468 6520 536f 6674 7761 7265 2046 7265  the Software Fre
+00000570: 6564 6f6d 2043 6f6e 7365 7276 616e 6379  edom Conservancy
+00000580: 5d28 6874 7470 733a 2f2f 7366 636f 6e73  ](https://sfcons
+00000590: 6572 7661 6e63 792e 6f72 6729 2e0a 0a57  ervancy.org)...W
+000005a0: 6869 6c65 2049 2064 6f20 6e6f 7420 6164  hile I do not ad
+000005b0: 766f 6361 7465 2066 6f72 2061 6c6c 2074  vocate for all t
+000005c0: 6865 2069 7373 7565 7320 6c69 7374 6564  he issues listed
+000005d0: 2074 6865 7265 2049 2064 6f20 6e6f 7420   there I do not 
+000005e0: 6c69 6b65 2074 6861 740a 6120 636f 6d70  like that.a comp
+000005f0: 616e 7920 6c69 6b65 204d 6963 726f 736f  any like Microso
+00000600: 6674 206d 6179 2070 726f 6669 7420 6672  ft may profit fr
+00000610: 6f6d 206f 7065 6e20 736f 7572 6365 2070  om open source p
+00000620: 726f 6a65 6374 732e 0a0a 4920 636f 6e74  rojects...I cont
+00000630: 696e 7565 2074 6f20 7573 6520 4769 7448  inue to use GitH
+00000640: 7562 2062 6563 6175 7365 2069 7420 6f66  ub because it of
+00000650: 6665 7273 2074 6865 2073 6572 7669 6365  fers the service
+00000660: 7320 4920 6e65 6564 2066 6f72 2066 7265  s I need for fre
+00000670: 652e 2020 4275 742c 2049 2063 6f6e 7469  e.  But, I conti
+00000680: 6e75 650a 746f 206d 6f6e 6974 6f72 2074  nue.to monitor t
+00000690: 6865 6972 2074 6572 6d73 206f 6620 7365  heir terms of se
+000006a0: 7276 6963 652e 0a0a 416e 7920 7573 6520  rvice...Any use 
+000006b0: 6f66 2074 6869 7320 7072 6f6a 6563 7427  of this project'
+000006c0: 7320 636f 6465 2062 7920 4769 7448 7562  s code by GitHub
+000006d0: 2043 6f70 696c 6f74 2c20 7061 7374 206f   Copilot, past o
+000006e0: 7220 7072 6573 656e 742c 2069 7320 646f  r present, is do
+000006f0: 6e65 0a77 6974 686f 7574 206d 7920 7065  ne.without my pe
+00000700: 726d 6973 7369 6f6e 2e20 2049 2064 6f20  rmission.  I do 
+00000710: 6e6f 7420 636f 6e73 656e 7420 746f 2047  not consent to G
+00000720: 6974 4875 6227 7320 7573 6520 6f66 2074  itHub's use of t
+00000730: 6869 7320 7072 6f6a 6563 7427 730a 636f  his project's.co
+00000740: 6465 2069 6e20 436f 7069 6c6f 742e 0a0a  de in Copilot...
+00000750: 4120 7265 706f 7369 746f 7279 206f 776e  A repository own
+00000760: 6572 206d 6179 206f 7074 206f 7574 206f  er may opt out o
+00000770: 6620 436f 7069 6c6f 7420 6279 2063 6861  f Copilot by cha
+00000780: 6e67 696e 6720 5365 7474 696e 6773 202d  nging Settings -
+00000790: 2d3e 2047 6974 4875 6220 436f 7069 6c6f  -> GitHub Copilo
+000007a0: 742e 0a0a 4920 6861 7665 2064 6f6e 6520  t...I have done 
+000007b0: 736f 2e0a 0a                             so...
```

### Comparing `hasiicommon-0.2.1/README.md` & `hasiicommon-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -21,58 +21,81 @@
 00000140: 2f69 6d61 6765 732f 6261 6467 6573 2f6d  /images/badges/m
 00000150: 6164 652d 7769 7468 2d70 7974 686f 6e2e  ade-with-python.
 00000160: 7376 6729 5d28 6874 7470 733a 2f2f 7777  svg)](https://ww
 00000170: 772e 7079 7468 6f6e 2e6f 7267 2f29 0a0a  w.python.org/)..
 00000180: 486f 7374 2063 6f6d 6d6f 6e20 5549 2061  Host common UI a
 00000190: 7274 6966 6163 7473 2066 6f72 2076 6172  rtifacts for var
 000001a0: 696f 7573 2070 726f 6a65 6374 7320 4920  ious projects I 
-000001b0: 616d 2064 6576 656c 6f70 696e 670a 0a0a  am developing...
-000001c0: 215b 4875 6d62 6572 746f 2773 204d 6f64  ![Humberto's Mod
-000001d0: 6966 6965 6420 4c6f 676f 5d28 2e2f 6465  ified Logo](./de
-000001e0: 7665 6c6f 7065 722f 5369 6c6c 7947 6974  veloper/SillyGit
-000001f0: 4875 622e 706e 6729 0a0a 4920 616d 2063  Hub.png)..I am c
-00000200: 6f6e 6365 726e 6564 2061 626f 7574 2047  oncerned about G
-00000210: 6974 4875 6227 7320 436f 7069 6c6f 7420  itHub's Copilot 
-00000220: 7072 6f6a 6563 740a 0a0a 0a49 2075 7267  project....I urg
-00000230: 6520 796f 7520 746f 2072 6561 6420 6162  e you to read ab
-00000240: 6f75 7420 7468 650a 5b47 6976 6520 7570  out the.[Give up
-00000250: 2047 6974 4875 625d 2868 7474 7073 3a2f   GitHub](https:/
-00000260: 2f47 6976 6555 7047 6974 4875 622e 6f72  /GiveUpGitHub.or
-00000270: 6729 2063 616d 7061 6967 6e20 6672 6f6d  g) campaign from
-00000280: 0a5b 7468 6520 536f 6674 7761 7265 2046  .[the Software F
-00000290: 7265 6564 6f6d 2043 6f6e 7365 7276 616e  reedom Conservan
-000002a0: 6379 5d28 6874 7470 733a 2f2f 7366 636f  cy](https://sfco
-000002b0: 6e73 6572 7661 6e63 792e 6f72 6729 2e0a  nservancy.org)..
-000002c0: 0a57 6869 6c65 2049 2064 6f20 6e6f 7420  .While I do not 
-000002d0: 6164 766f 6361 7465 2066 6f72 2061 6c6c  advocate for all
-000002e0: 2074 6865 2069 7373 7565 7320 6c69 7374   the issues list
-000002f0: 6564 2074 6865 7265 2049 2064 6f20 6e6f  ed there I do no
-00000300: 7420 6c69 6b65 2074 6861 740a 6120 636f  t like that.a co
-00000310: 6d70 616e 7920 6c69 6b65 204d 6963 726f  mpany like Micro
-00000320: 736f 6674 206d 6179 2070 726f 6669 7420  soft may profit 
-00000330: 6672 6f6d 206f 7065 6e20 736f 7572 6365  from open source
-00000340: 2070 726f 6a65 6374 732e 0a0a 4920 636f   projects...I co
-00000350: 6e74 696e 7565 2074 6f20 7573 6520 4769  ntinue to use Gi
-00000360: 7448 7562 2062 6563 6175 7365 2069 7420  tHub because it 
-00000370: 6f66 6665 7273 2074 6865 2073 6572 7669  offers the servi
-00000380: 6365 7320 4920 6e65 6564 2066 6f72 2066  ces I need for f
-00000390: 7265 652e 2020 4275 742c 2049 2063 6f6e  ree.  But, I con
-000003a0: 7469 6e75 650a 746f 206d 6f6e 6974 6f72  tinue.to monitor
-000003b0: 2074 6865 6972 2074 6572 6d73 206f 6620   their terms of 
-000003c0: 7365 7276 6963 652e 0a0a 416e 7920 7573  service...Any us
-000003d0: 6520 6f66 2074 6869 7320 7072 6f6a 6563  e of this projec
-000003e0: 7427 7320 636f 6465 2062 7920 4769 7448  t's code by GitH
-000003f0: 7562 2043 6f70 696c 6f74 2c20 7061 7374  ub Copilot, past
-00000400: 206f 7220 7072 6573 656e 742c 2069 7320   or present, is 
-00000410: 646f 6e65 0a77 6974 686f 7574 206d 7920  done.without my 
-00000420: 7065 726d 6973 7369 6f6e 2e20 2049 2064  permission.  I d
-00000430: 6f20 6e6f 7420 636f 6e73 656e 7420 746f  o not consent to
-00000440: 2047 6974 4875 6227 7320 7573 6520 6f66   GitHub's use of
-00000450: 2074 6869 7320 7072 6f6a 6563 7427 730a   this project's.
-00000460: 636f 6465 2069 6e20 436f 7069 6c6f 742e  code in Copilot.
-00000470: 0a0a 4120 7265 706f 7369 746f 7279 206f  ..A repository o
-00000480: 776e 6572 206d 6179 206f 7074 206f 7574  wner may opt out
-00000490: 206f 6620 436f 7069 6c6f 7420 6279 2063   of Copilot by c
-000004a0: 6861 6e67 696e 6720 5365 7474 696e 6773  hanging Settings
-000004b0: 202d 2d3e 2047 6974 4875 6220 436f 7069   --> GitHub Copi
-000004c0: 6c6f 742e 0a0a 4920 6861 7665 2064 6f6e  lot...I have don
-000004d0: 6520 736f 2e0a 0a                        e so...
+000001b0: 616d 2064 6576 656c 6f70 696e 670a 0a5f  am developing.._
+000001c0: 5f5f 0a0a 5772 6974 7465 6e20 6279 203c  __..Written by <
+000001d0: 6120 6872 6566 3d22 6d61 696c 746f 3a65  a href="mailto:e
+000001e0: 6d61 696c 4068 756d 6265 7274 6f2e 612e  mail@humberto.a.
+000001f0: 7361 6e63 6865 7a2e 6969 4067 6d61 696c  sanchez.ii@gmail
+00000200: 2e63 6f6d 3f73 7562 6a65 6374 3d48 656c  .com?subject=Hel
+00000210: 6c6f 2048 756d 6265 7274 6f22 3e48 756d  lo Humberto">Hum
+00000220: 6265 7274 6f20 412e 2053 616e 6368 657a  berto A. Sanchez
+00000230: 2049 493c 2f61 3e20 2028 4329 2032 3032   II</a>  (C) 202
+00000240: 330a 0a23 2320 4e6f 7465 0a46 6f72 2061  3..## Note.For a
+00000250: 6c6c 206b 696e 6420 6f66 2070 726f 626c  ll kind of probl
+00000260: 656d 732c 2072 6571 7565 7374 732c 2065  ems, requests, e
+00000270: 6e68 616e 6365 6d65 6e74 732c 2062 7567  nhancements, bug
+00000280: 2072 6570 6f72 7473 2c20 6574 632e 2c0a   reports, etc.,.
+00000290: 706c 6561 7365 2064 726f 7020 6d65 2061  please drop me a
+000002a0: 6e20 652d 6d61 696c 2e0a 0a23 2320 4465  n e-mail...## De
+000002b0: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+000002c0: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+000002d0: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+000002e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002f0: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+00000300: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+00000310: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+00000320: 6e74 2062 7569 6c64 730a 0a2d 2d2d 0a0a  nt builds..---..
+00000330: 0a21 5b48 756d 6265 7274 6f27 7320 4d6f  .![Humberto's Mo
+00000340: 6469 6669 6564 204c 6f67 6f5d 282e 2f64  dified Logo](./d
+00000350: 6576 656c 6f70 6572 2f53 696c 6c79 4769  eveloper/SillyGi
+00000360: 7448 7562 2e70 6e67 290a 0a49 2061 6d20  tHub.png)..I am 
+00000370: 636f 6e63 6572 6e65 6420 6162 6f75 7420  concerned about 
+00000380: 4769 7448 7562 2773 2043 6f70 696c 6f74  GitHub's Copilot
+00000390: 2070 726f 6a65 6374 0a0a 0a0a 4920 7572   project....I ur
+000003a0: 6765 2079 6f75 2074 6f20 7265 6164 2061  ge you to read a
+000003b0: 626f 7574 2074 6865 0a5b 4769 7665 2075  bout the.[Give u
+000003c0: 7020 4769 7448 7562 5d28 6874 7470 733a  p GitHub](https:
+000003d0: 2f2f 4769 7665 5570 4769 7448 7562 2e6f  //GiveUpGitHub.o
+000003e0: 7267 2920 6361 6d70 6169 676e 2066 726f  rg) campaign fro
+000003f0: 6d0a 5b74 6865 2053 6f66 7477 6172 6520  m.[the Software 
+00000400: 4672 6565 646f 6d20 436f 6e73 6572 7661  Freedom Conserva
+00000410: 6e63 795d 2868 7474 7073 3a2f 2f73 6663  ncy](https://sfc
+00000420: 6f6e 7365 7276 616e 6379 2e6f 7267 292e  onservancy.org).
+00000430: 0a0a 5768 696c 6520 4920 646f 206e 6f74  ..While I do not
+00000440: 2061 6476 6f63 6174 6520 666f 7220 616c   advocate for al
+00000450: 6c20 7468 6520 6973 7375 6573 206c 6973  l the issues lis
+00000460: 7465 6420 7468 6572 6520 4920 646f 206e  ted there I do n
+00000470: 6f74 206c 696b 6520 7468 6174 0a61 2063  ot like that.a c
+00000480: 6f6d 7061 6e79 206c 696b 6520 4d69 6372  ompany like Micr
+00000490: 6f73 6f66 7420 6d61 7920 7072 6f66 6974  osoft may profit
+000004a0: 2066 726f 6d20 6f70 656e 2073 6f75 7263   from open sourc
+000004b0: 6520 7072 6f6a 6563 7473 2e0a 0a49 2063  e projects...I c
+000004c0: 6f6e 7469 6e75 6520 746f 2075 7365 2047  ontinue to use G
+000004d0: 6974 4875 6220 6265 6361 7573 6520 6974  itHub because it
+000004e0: 206f 6666 6572 7320 7468 6520 7365 7276   offers the serv
+000004f0: 6963 6573 2049 206e 6565 6420 666f 7220  ices I need for 
+00000500: 6672 6565 2e20 2042 7574 2c20 4920 636f  free.  But, I co
+00000510: 6e74 696e 7565 0a74 6f20 6d6f 6e69 746f  ntinue.to monito
+00000520: 7220 7468 6569 7220 7465 726d 7320 6f66  r their terms of
+00000530: 2073 6572 7669 6365 2e0a 0a41 6e79 2075   service...Any u
+00000540: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
+00000550: 6374 2773 2063 6f64 6520 6279 2047 6974  ct's code by Git
+00000560: 4875 6220 436f 7069 6c6f 742c 2070 6173  Hub Copilot, pas
+00000570: 7420 6f72 2070 7265 7365 6e74 2c20 6973  t or present, is
+00000580: 2064 6f6e 650a 7769 7468 6f75 7420 6d79   done.without my
+00000590: 2070 6572 6d69 7373 696f 6e2e 2020 4920   permission.  I 
+000005a0: 646f 206e 6f74 2063 6f6e 7365 6e74 2074  do not consent t
+000005b0: 6f20 4769 7448 7562 2773 2075 7365 206f  o GitHub's use o
+000005c0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
+000005d0: 0a63 6f64 6520 696e 2043 6f70 696c 6f74  .code in Copilot
+000005e0: 2e0a 0a41 2072 6570 6f73 6974 6f72 7920  ...A repository 
+000005f0: 6f77 6e65 7220 6d61 7920 6f70 7420 6f75  owner may opt ou
+00000600: 7420 6f66 2043 6f70 696c 6f74 2062 7920  t of Copilot by 
+00000610: 6368 616e 6769 6e67 2053 6574 7469 6e67  changing Setting
+00000620: 7320 2d2d 3e20 4769 7448 7562 2043 6f70  s --> GitHub Cop
+00000630: 696c 6f74 2e0a 0a49 2068 6176 6520 646f  ilot...I have do
+00000640: 6e65 2073 6f2e 0a0a                      ne so...
```

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/DefaultPreferences.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/DefaultPreferences.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxActor.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxArrow.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxClass.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewClassDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewProject.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNewUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxOpenFile.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRedo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAggregation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipAssociation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipComposition.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipInheritance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxRelationshipRealization.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSaveDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramInstance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxSequenceDiagramMessage.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxText.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxUndo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxUseCase.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomIn.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded16/ImgToolboxZoomOut.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxActor.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxArrow.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxClass.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewClassDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewProject.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewSequenceDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNewUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxOpenFile.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRedo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAggregation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipAssociation.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipComposition.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipInheritance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipNote.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxRelationshipRealization.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSaveDiagram.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramInstance.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxSequenceDiagramMessage.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxText.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxUndo.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxUseCase.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomIn.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py` & `hasiicommon-0.2.2/hasiicommon/resources/images/icons/embedded32/ImgToolboxZoomOut.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/ui/UnitTestBaseW.py` & `hasiicommon-0.2.2/hasiicommon/ui/UnitTestBaseW.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/ui/widgets/DimensionsControl.py` & `hasiicommon-0.2.2/hasiicommon/ui/widgets/DimensionsControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/ui/widgets/DualSpinnerControl.py` & `hasiicommon-0.2.2/hasiicommon/ui/widgets/DualSpinnerControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon/ui/widgets/PositionControl.py` & `hasiicommon-0.2.2/hasiicommon/ui/widgets/PositionControl.py`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/hasiicommon.egg-info/PKG-INFO` & `hasiicommon-0.2.2/hasiicommon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6861 7369  : 2.1.Name: hasi
 00000020: 6963 6f6d 6d6f 6e0a 5665 7273 696f 6e3a  icommon.Version:
-00000030: 2030 2e32 2e31 0a53 756d 6d61 7279 3a20   0.2.1.Summary: 
+00000030: 2030 2e32 2e32 0a53 756d 6d61 7279 3a20   0.2.2.Summary: 
 00000040: 4875 6d62 6572 746f 6073 2043 6f6d 6d6f  Humberto`s Commo
 00000050: 6e20 5374 7566 660a 486f 6d65 2d70 6167  n Stuff.Home-pag
 00000060: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
 00000070: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
 00000080: 6861 7369 6963 6f6d 6d6f 6e0a 4175 7468  hasiicommon.Auth
 00000090: 6f72 3a20 4875 6d62 6572 746f 2041 2e20  or: Humberto A. 
 000000a0: 5361 6e63 6865 7a20 4949 0a41 7574 686f  Sanchez II.Autho
@@ -44,58 +44,81 @@
 000002b0: 6167 6573 2f62 6164 6765 732f 6d61 6465  ages/badges/made
 000002c0: 2d77 6974 682d 7079 7468 6f6e 2e73 7667  -with-python.svg
 000002d0: 295d 2868 7474 7073 3a2f 2f77 7777 2e70  )](https://www.p
 000002e0: 7974 686f 6e2e 6f72 672f 290a 0a48 6f73  ython.org/)..Hos
 000002f0: 7420 636f 6d6d 6f6e 2055 4920 6172 7469  t common UI arti
 00000300: 6661 6374 7320 666f 7220 7661 7269 6f75  facts for variou
 00000310: 7320 7072 6f6a 6563 7473 2049 2061 6d20  s projects I am 
-00000320: 6465 7665 6c6f 7069 6e67 0a0a 0a21 5b48  developing...![H
-00000330: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
-00000340: 6564 204c 6f67 6f5d 282e 2f64 6576 656c  ed Logo](./devel
-00000350: 6f70 6572 2f53 696c 6c79 4769 7448 7562  oper/SillyGitHub
-00000360: 2e70 6e67 290a 0a49 2061 6d20 636f 6e63  .png)..I am conc
-00000370: 6572 6e65 6420 6162 6f75 7420 4769 7448  erned about GitH
-00000380: 7562 2773 2043 6f70 696c 6f74 2070 726f  ub's Copilot pro
-00000390: 6a65 6374 0a0a 0a0a 4920 7572 6765 2079  ject....I urge y
-000003a0: 6f75 2074 6f20 7265 6164 2061 626f 7574  ou to read about
-000003b0: 2074 6865 0a5b 4769 7665 2075 7020 4769   the.[Give up Gi
-000003c0: 7448 7562 5d28 6874 7470 733a 2f2f 4769  tHub](https://Gi
-000003d0: 7665 5570 4769 7448 7562 2e6f 7267 2920  veUpGitHub.org) 
-000003e0: 6361 6d70 6169 676e 2066 726f 6d0a 5b74  campaign from.[t
-000003f0: 6865 2053 6f66 7477 6172 6520 4672 6565  he Software Free
-00000400: 646f 6d20 436f 6e73 6572 7661 6e63 795d  dom Conservancy]
-00000410: 2868 7474 7073 3a2f 2f73 6663 6f6e 7365  (https://sfconse
-00000420: 7276 616e 6379 2e6f 7267 292e 0a0a 5768  rvancy.org)...Wh
-00000430: 696c 6520 4920 646f 206e 6f74 2061 6476  ile I do not adv
-00000440: 6f63 6174 6520 666f 7220 616c 6c20 7468  ocate for all th
-00000450: 6520 6973 7375 6573 206c 6973 7465 6420  e issues listed 
-00000460: 7468 6572 6520 4920 646f 206e 6f74 206c  there I do not l
-00000470: 696b 6520 7468 6174 0a61 2063 6f6d 7061  ike that.a compa
-00000480: 6e79 206c 696b 6520 4d69 6372 6f73 6f66  ny like Microsof
-00000490: 7420 6d61 7920 7072 6f66 6974 2066 726f  t may profit fro
-000004a0: 6d20 6f70 656e 2073 6f75 7263 6520 7072  m open source pr
-000004b0: 6f6a 6563 7473 2e0a 0a49 2063 6f6e 7469  ojects...I conti
-000004c0: 6e75 6520 746f 2075 7365 2047 6974 4875  nue to use GitHu
-000004d0: 6220 6265 6361 7573 6520 6974 206f 6666  b because it off
-000004e0: 6572 7320 7468 6520 7365 7276 6963 6573  ers the services
-000004f0: 2049 206e 6565 6420 666f 7220 6672 6565   I need for free
-00000500: 2e20 2042 7574 2c20 4920 636f 6e74 696e  .  But, I contin
-00000510: 7565 0a74 6f20 6d6f 6e69 746f 7220 7468  ue.to monitor th
-00000520: 6569 7220 7465 726d 7320 6f66 2073 6572  eir terms of ser
-00000530: 7669 6365 2e0a 0a41 6e79 2075 7365 206f  vice...Any use o
-00000540: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-00000550: 2063 6f64 6520 6279 2047 6974 4875 6220   code by GitHub 
-00000560: 436f 7069 6c6f 742c 2070 6173 7420 6f72  Copilot, past or
-00000570: 2070 7265 7365 6e74 2c20 6973 2064 6f6e   present, is don
-00000580: 650a 7769 7468 6f75 7420 6d79 2070 6572  e.without my per
-00000590: 6d69 7373 696f 6e2e 2020 4920 646f 206e  mission.  I do n
-000005a0: 6f74 2063 6f6e 7365 6e74 2074 6f20 4769  ot consent to Gi
-000005b0: 7448 7562 2773 2075 7365 206f 6620 7468  tHub's use of th
-000005c0: 6973 2070 726f 6a65 6374 2773 0a63 6f64  is project's.cod
-000005d0: 6520 696e 2043 6f70 696c 6f74 2e0a 0a41  e in Copilot...A
-000005e0: 2072 6570 6f73 6974 6f72 7920 6f77 6e65   repository owne
-000005f0: 7220 6d61 7920 6f70 7420 6f75 7420 6f66  r may opt out of
-00000600: 2043 6f70 696c 6f74 2062 7920 6368 616e   Copilot by chan
-00000610: 6769 6e67 2053 6574 7469 6e67 7320 2d2d  ging Settings --
-00000620: 3e20 4769 7448 7562 2043 6f70 696c 6f74  > GitHub Copilot
-00000630: 2e0a 0a49 2068 6176 6520 646f 6e65 2073  ...I have done s
-00000640: 6f2e 0a0a                                o...
+00000320: 6465 7665 6c6f 7069 6e67 0a0a 5f5f 5f0a  developing..___.
+00000330: 0a57 7269 7474 656e 2062 7920 3c61 2068  .Written by <a h
+00000340: 7265 663d 226d 6169 6c74 6f3a 656d 6169  ref="mailto:emai
+00000350: 6c40 6875 6d62 6572 746f 2e61 2e73 616e  l@humberto.a.san
+00000360: 6368 657a 2e69 6940 676d 6169 6c2e 636f  chez.ii@gmail.co
+00000370: 6d3f 7375 626a 6563 743d 4865 6c6c 6f20  m?subject=Hello 
+00000380: 4875 6d62 6572 746f 223e 4875 6d62 6572  Humberto">Humber
+00000390: 746f 2041 2e20 5361 6e63 6865 7a20 4949  to A. Sanchez II
+000003a0: 3c2f 613e 2020 2843 2920 3230 3233 0a0a  </a>  (C) 2023..
+000003b0: 2323 204e 6f74 650a 466f 7220 616c 6c20  ## Note.For all 
+000003c0: 6b69 6e64 206f 6620 7072 6f62 6c65 6d73  kind of problems
+000003d0: 2c20 7265 7175 6573 7473 2c20 656e 6861  , requests, enha
+000003e0: 6e63 656d 656e 7473 2c20 6275 6720 7265  ncements, bug re
+000003f0: 706f 7274 732c 2065 7463 2e2c 0a70 6c65  ports, etc.,.ple
+00000400: 6173 6520 6472 6f70 206d 6520 616e 2065  ase drop me an e
+00000410: 2d6d 6169 6c2e 0a0a 2323 2044 6576 656c  -mail...## Devel
+00000420: 6f70 6572 204e 6f74 6573 0a54 6869 7320  oper Notes.This 
+00000430: 7072 6f6a 6563 7420 7573 6573 205b 6275  project uses [bu
+00000440: 696c 646c 6163 6b65 795d 2868 7474 7073  ildlackey](https
+00000450: 3a2f 2f67 6974 6875 622e 636f 6d2f 6861  ://github.com/ha
+00000460: 7369 6932 3031 312f 6275 696c 646c 6163  sii2011/buildlac
+00000470: 6b65 7929 2066 6f72 2064 6179 2074 6f20  key) for day to 
+00000480: 6461 7920 6465 7665 6c6f 706d 656e 7420  day development 
+00000490: 6275 696c 6473 0a0a 2d2d 2d0a 0a0a 215b  builds..---...![
+000004a0: 4875 6d62 6572 746f 2773 204d 6f64 6966  Humberto's Modif
+000004b0: 6965 6420 4c6f 676f 5d28 2e2f 6465 7665  ied Logo](./deve
+000004c0: 6c6f 7065 722f 5369 6c6c 7947 6974 4875  loper/SillyGitHu
+000004d0: 622e 706e 6729 0a0a 4920 616d 2063 6f6e  b.png)..I am con
+000004e0: 6365 726e 6564 2061 626f 7574 2047 6974  cerned about Git
+000004f0: 4875 6227 7320 436f 7069 6c6f 7420 7072  Hub's Copilot pr
+00000500: 6f6a 6563 740a 0a0a 0a49 2075 7267 6520  oject....I urge 
+00000510: 796f 7520 746f 2072 6561 6420 6162 6f75  you to read abou
+00000520: 7420 7468 650a 5b47 6976 6520 7570 2047  t the.[Give up G
+00000530: 6974 4875 625d 2868 7474 7073 3a2f 2f47  itHub](https://G
+00000540: 6976 6555 7047 6974 4875 622e 6f72 6729  iveUpGitHub.org)
+00000550: 2063 616d 7061 6967 6e20 6672 6f6d 0a5b   campaign from.[
+00000560: 7468 6520 536f 6674 7761 7265 2046 7265  the Software Fre
+00000570: 6564 6f6d 2043 6f6e 7365 7276 616e 6379  edom Conservancy
+00000580: 5d28 6874 7470 733a 2f2f 7366 636f 6e73  ](https://sfcons
+00000590: 6572 7661 6e63 792e 6f72 6729 2e0a 0a57  ervancy.org)...W
+000005a0: 6869 6c65 2049 2064 6f20 6e6f 7420 6164  hile I do not ad
+000005b0: 766f 6361 7465 2066 6f72 2061 6c6c 2074  vocate for all t
+000005c0: 6865 2069 7373 7565 7320 6c69 7374 6564  he issues listed
+000005d0: 2074 6865 7265 2049 2064 6f20 6e6f 7420   there I do not 
+000005e0: 6c69 6b65 2074 6861 740a 6120 636f 6d70  like that.a comp
+000005f0: 616e 7920 6c69 6b65 204d 6963 726f 736f  any like Microso
+00000600: 6674 206d 6179 2070 726f 6669 7420 6672  ft may profit fr
+00000610: 6f6d 206f 7065 6e20 736f 7572 6365 2070  om open source p
+00000620: 726f 6a65 6374 732e 0a0a 4920 636f 6e74  rojects...I cont
+00000630: 696e 7565 2074 6f20 7573 6520 4769 7448  inue to use GitH
+00000640: 7562 2062 6563 6175 7365 2069 7420 6f66  ub because it of
+00000650: 6665 7273 2074 6865 2073 6572 7669 6365  fers the service
+00000660: 7320 4920 6e65 6564 2066 6f72 2066 7265  s I need for fre
+00000670: 652e 2020 4275 742c 2049 2063 6f6e 7469  e.  But, I conti
+00000680: 6e75 650a 746f 206d 6f6e 6974 6f72 2074  nue.to monitor t
+00000690: 6865 6972 2074 6572 6d73 206f 6620 7365  heir terms of se
+000006a0: 7276 6963 652e 0a0a 416e 7920 7573 6520  rvice...Any use 
+000006b0: 6f66 2074 6869 7320 7072 6f6a 6563 7427  of this project'
+000006c0: 7320 636f 6465 2062 7920 4769 7448 7562  s code by GitHub
+000006d0: 2043 6f70 696c 6f74 2c20 7061 7374 206f   Copilot, past o
+000006e0: 7220 7072 6573 656e 742c 2069 7320 646f  r present, is do
+000006f0: 6e65 0a77 6974 686f 7574 206d 7920 7065  ne.without my pe
+00000700: 726d 6973 7369 6f6e 2e20 2049 2064 6f20  rmission.  I do 
+00000710: 6e6f 7420 636f 6e73 656e 7420 746f 2047  not consent to G
+00000720: 6974 4875 6227 7320 7573 6520 6f66 2074  itHub's use of t
+00000730: 6869 7320 7072 6f6a 6563 7427 730a 636f  his project's.co
+00000740: 6465 2069 6e20 436f 7069 6c6f 742e 0a0a  de in Copilot...
+00000750: 4120 7265 706f 7369 746f 7279 206f 776e  A repository own
+00000760: 6572 206d 6179 206f 7074 206f 7574 206f  er may opt out o
+00000770: 6620 436f 7069 6c6f 7420 6279 2063 6861  f Copilot by cha
+00000780: 6e67 696e 6720 5365 7474 696e 6773 202d  nging Settings -
+00000790: 2d3e 2047 6974 4875 6220 436f 7069 6c6f  -> GitHub Copilo
+000007a0: 742e 0a0a 4920 6861 7665 2064 6f6e 6520  t...I have done 
+000007b0: 736f 2e0a 0a                             so...
```

### Comparing `hasiicommon-0.2.1/hasiicommon.egg-info/SOURCES.txt` & `hasiicommon-0.2.2/hasiicommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hasiicommon-0.2.1/setup.py` & `hasiicommon-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="hasiicommon",
-    version="0.2.1",
+    version="0.2.2",
     author='Humberto A. Sanchez II',
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Humberto`s Common Stuff',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -36,9 +36,9 @@
         'hasiicommon.resources',
         'hasiicommon.resources.images',
         'hasiicommon.resources.images.icons',
         'hasiicommon.resources.images.icons.embedded16',
         'hasiicommon.resources.images.icons.embedded32',
         'hasiicommon.ui', 'hasiicommon.ui.widgets'
     ],
-    install_requires=['hasiihelper==0.1.0','Deprecated~=1.2.13', 'wxPython~=4.2.0'],
+    install_requires=['hasiihelper==0.2.0', 'Deprecated~=1.2.13', 'wxPython~=4.2.0'],
 )
```

