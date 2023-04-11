# Comparing `tmp/sbol3-1.0rc1.tar.gz` & `tmp/sbol3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbol3-1.0rc1.tar", last modified: Tue Feb 15 16:09:07 2022, max compression
+gzip compressed data, was "sbol3-1.1.tar", last modified: Tue Apr 11 14:49:54 2023, max compression
```

## Comparing `sbol3-1.0rc1.tar` & `sbol3-1.1.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2022-02-15 16:09:07.620834 sbol3-1.0rc1/
--rw-r--r--   0 tmitchel (385877172) staff       (20)      725 2022-02-15 16:09:07.621037 sbol3-1.0rc1/PKG-INFO
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1095 2022-02-15 15:55:31.000000 sbol3-1.0rc1/README.md
-drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2022-02-15 16:09:07.597632 sbol3-1.0rc1/sbol3/
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1864 2022-02-15 16:07:10.000000 sbol3-1.0rc1/sbol3/__init__.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2892 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/attachment.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2116 2021-04-21 21:17:59.000000 sbol3-1.0rc1/sbol3/boolean_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3573 2021-04-30 19:21:10.000000 sbol3-1.0rc1/sbol3/collection.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3404 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/combderiv.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3680 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/component.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2795 2021-10-08 19:54:45.000000 sbol3-1.0rc1/sbol3/compref.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      788 2021-10-27 18:15:39.000000 sbol3-1.0rc1/sbol3/config.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    10573 2022-02-11 18:09:28.000000 sbol3-1.0rc1/sbol3/constants.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3108 2021-04-30 19:21:10.000000 sbol3-1.0rc1/sbol3/constraint.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2219 2021-04-21 21:17:59.000000 sbol3-1.0rc1/sbol3/custom.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1859 2020-09-02 17:04:34.000000 sbol3-1.0rc1/sbol3/datetime_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    31525 2022-02-10 16:26:22.000000 sbol3-1.0rc1/sbol3/document.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      398 2021-04-21 20:58:26.000000 sbol3-1.0rc1/sbol3/error.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1674 2021-04-30 19:21:10.000000 sbol3-1.0rc1/sbol3/expdata.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2790 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/extdef.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1699 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/feature.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1601 2022-01-17 14:36:50.000000 sbol3-1.0rc1/sbol3/float_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    13145 2022-02-14 17:44:12.000000 sbol3-1.0rc1/sbol3/identified.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2146 2021-04-30 19:21:10.000000 sbol3-1.0rc1/sbol3/implementation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2049 2021-04-21 21:17:59.000000 sbol3-1.0rc1/sbol3/int_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2668 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/interaction.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1981 2021-09-27 15:30:45.000000 sbol3-1.0rc1/sbol3/interface.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2450 2022-02-11 18:09:28.000000 sbol3-1.0rc1/sbol3/localsub.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     7454 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/location.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3502 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/model.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     5688 2022-02-08 20:19:42.000000 sbol3-1.0rc1/sbol3/object.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     9893 2021-05-26 13:23:53.000000 sbol3-1.0rc1/sbol3/om_compound.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     7654 2021-05-26 13:23:53.000000 sbol3-1.0rc1/sbol3/om_prefix.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     9825 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/om_unit.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     5813 2022-01-21 20:27:33.000000 sbol3-1.0rc1/sbol3/ownedobject.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2559 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/participation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     6828 2021-07-13 19:40:24.000000 sbol3-1.0rc1/sbol3/property_base.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    10652 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/provenance.py
-drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2022-02-15 16:09:07.600156 sbol3-1.0rc1/sbol3/rdf/
--rw-r--r--   0 tmitchel (385877172) staff       (20)    67451 2021-11-12 16:26:18.000000 sbol3-1.0rc1/sbol3/rdf/sbol3-shapes.ttl
--rw-r--r--   0 tmitchel (385877172) staff       (20)     4179 2021-11-30 12:09:15.000000 sbol3-1.0rc1/sbol3/refobj_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2064 2022-02-11 18:09:28.000000 sbol3-1.0rc1/sbol3/seqfeat.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2664 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/sequence.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3116 2022-02-11 18:09:28.000000 sbol3-1.0rc1/sbol3/subcomponent.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2514 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/text_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    10391 2022-02-08 20:19:42.000000 sbol3-1.0rc1/sbol3/toplevel.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      480 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/typing.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2368 2021-11-16 16:30:04.000000 sbol3-1.0rc1/sbol3/uri_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1177 2021-08-04 19:19:43.000000 sbol3-1.0rc1/sbol3/util.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      586 2020-10-13 14:37:11.000000 sbol3-1.0rc1/sbol3/utils.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1891 2022-01-13 16:21:50.000000 sbol3-1.0rc1/sbol3/validation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     4595 2022-02-11 18:09:28.000000 sbol3-1.0rc1/sbol3/varcomp.py
-drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2022-02-15 16:09:07.599728 sbol3-1.0rc1/sbol3.egg-info/
--rw-r--r--   0 tmitchel (385877172) staff       (20)      725 2022-02-15 16:09:07.000000 sbol3-1.0rc1/sbol3.egg-info/PKG-INFO
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1998 2022-02-15 16:09:07.000000 sbol3-1.0rc1/sbol3.egg-info/SOURCES.txt
--rw-r--r--   0 tmitchel (385877172) staff       (20)        1 2022-02-15 16:09:07.000000 sbol3-1.0rc1/sbol3.egg-info/dependency_links.txt
--rw-r--r--   0 tmitchel (385877172) staff       (20)       59 2022-02-15 16:09:07.000000 sbol3-1.0rc1/sbol3.egg-info/requires.txt
--rw-r--r--   0 tmitchel (385877172) staff       (20)        6 2022-02-15 16:09:07.000000 sbol3-1.0rc1/sbol3.egg-info/top_level.txt
--rw-r--r--   0 tmitchel (385877172) staff       (20)       75 2022-02-15 16:09:07.621605 sbol3-1.0rc1/setup.cfg
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1780 2022-02-15 16:07:10.000000 sbol3-1.0rc1/setup.py
-drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2022-02-15 16:09:07.620323 sbol3-1.0rc1/test/
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1315 2021-02-01 20:16:49.000000 sbol3-1.0rc1/test/test_annotation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1553 2021-04-21 21:17:59.000000 sbol3-1.0rc1/test/test_attachment.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3908 2021-10-25 20:23:20.000000 sbol3-1.0rc1/test/test_collection.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1869 2021-10-08 19:54:45.000000 sbol3-1.0rc1/test/test_combderiv.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    10572 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_component.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1522 2021-10-08 19:54:45.000000 sbol3-1.0rc1/test/test_compref.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2094 2021-05-26 13:23:53.000000 sbol3-1.0rc1/test/test_config.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     6241 2021-04-21 21:17:59.000000 sbol3-1.0rc1/test/test_custom.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)    29991 2022-02-14 17:02:17.000000 sbol3-1.0rc1/test/test_document.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2139 2021-08-04 19:51:11.000000 sbol3-1.0rc1/test/test_examples.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1405 2021-04-21 20:58:26.000000 sbol3-1.0rc1/test/test_expdata.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2382 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_extdef.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1612 2021-04-21 21:17:59.000000 sbol3-1.0rc1/test/test_extension.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     4418 2022-02-14 17:44:12.000000 sbol3-1.0rc1/test/test_identified.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1725 2021-04-21 20:58:26.000000 sbol3-1.0rc1/test/test_implementation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1915 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_interaction.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1548 2021-09-27 15:30:45.000000 sbol3-1.0rc1/test/test_interface.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1299 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_localsub.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3426 2021-04-21 20:58:26.000000 sbol3-1.0rc1/test/test_location.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     5229 2021-04-30 19:21:10.000000 sbol3-1.0rc1/test/test_module.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2658 2022-02-08 20:19:42.000000 sbol3-1.0rc1/test/test_object.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     5290 2021-02-01 20:16:50.000000 sbol3-1.0rc1/test/test_om_compound.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2595 2021-02-01 20:16:50.000000 sbol3-1.0rc1/test/test_om_prefix.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     7045 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_om_unit.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     8516 2021-04-21 21:17:59.000000 sbol3-1.0rc1/test/test_ownedobject.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2031 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_participation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     6416 2022-02-10 16:51:57.000000 sbol3-1.0rc1/test/test_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     4297 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_provenance.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     5359 2021-11-30 12:09:15.000000 sbol3-1.0rc1/test/test_referenced_object.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     7988 2022-02-11 17:13:16.000000 sbol3-1.0rc1/test/test_roundtrip.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     1802 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_seqfeat.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     4903 2021-11-16 16:30:04.000000 sbol3-1.0rc1/test/test_sequence.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2069 2021-06-23 19:04:26.000000 sbol3-1.0rc1/test/test_style.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2659 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_subcomponent.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     2283 2021-11-16 16:30:04.000000 sbol3-1.0rc1/test/test_text_property.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     7477 2022-02-08 20:19:42.000000 sbol3-1.0rc1/test/test_toplevel.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      853 2021-08-04 19:19:43.000000 sbol3-1.0rc1/test/test_util.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)      966 2021-02-01 20:16:50.000000 sbol3-1.0rc1/test/test_utils.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3989 2022-02-08 20:19:42.000000 sbol3-1.0rc1/test/test_validation.py
--rw-r--r--   0 tmitchel (385877172) staff       (20)     3878 2022-02-11 18:09:28.000000 sbol3-1.0rc1/test/test_varcomp.py
+drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2023-04-11 14:49:54.333029 sbol3-1.1/
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1082 2021-05-14 19:52:14.000000 sbol3-1.1/LICENSE.txt
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      773 2023-04-11 14:49:54.333230 sbol3-1.1/PKG-INFO
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1384 2022-07-12 16:55:12.000000 sbol3-1.1/README.md
+drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2023-04-11 14:49:54.283857 sbol3-1.1/sbol3/
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1861 2022-02-18 20:59:16.000000 sbol3-1.1/sbol3/__init__.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2892 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/attachment.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2116 2021-04-21 21:17:59.000000 sbol3-1.1/sbol3/boolean_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3573 2021-04-30 19:21:10.000000 sbol3-1.1/sbol3/collection.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3404 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/combderiv.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3680 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/component.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2795 2021-10-08 19:54:45.000000 sbol3-1.1/sbol3/compref.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      788 2021-10-27 18:15:39.000000 sbol3-1.1/sbol3/config.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    10572 2023-04-04 14:40:15.000000 sbol3-1.1/sbol3/constants.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3108 2021-04-30 19:21:10.000000 sbol3-1.1/sbol3/constraint.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2219 2022-10-20 17:43:05.000000 sbol3-1.1/sbol3/custom.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1859 2020-09-02 17:04:34.000000 sbol3-1.1/sbol3/datetime_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    33245 2022-10-20 17:40:16.000000 sbol3-1.1/sbol3/document.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      398 2021-04-21 20:58:26.000000 sbol3-1.1/sbol3/error.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1674 2021-04-30 19:21:10.000000 sbol3-1.1/sbol3/expdata.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2790 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/extdef.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1699 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/feature.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1601 2022-01-17 14:36:50.000000 sbol3-1.1/sbol3/float_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    13145 2022-02-14 17:44:12.000000 sbol3-1.1/sbol3/identified.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2146 2021-04-30 19:21:10.000000 sbol3-1.1/sbol3/implementation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2049 2021-04-21 21:17:59.000000 sbol3-1.1/sbol3/int_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2668 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/interaction.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1981 2021-09-27 15:30:45.000000 sbol3-1.1/sbol3/interface.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2450 2022-02-11 18:09:28.000000 sbol3-1.1/sbol3/localsub.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     7472 2022-10-20 17:59:11.000000 sbol3-1.1/sbol3/location.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3502 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/model.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     5856 2023-04-11 14:28:17.000000 sbol3-1.1/sbol3/object.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     9893 2021-05-26 13:23:53.000000 sbol3-1.1/sbol3/om_compound.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     7654 2021-05-26 13:23:53.000000 sbol3-1.1/sbol3/om_prefix.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     9825 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/om_unit.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     5813 2022-01-21 20:27:33.000000 sbol3-1.1/sbol3/ownedobject.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2559 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/participation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     6828 2021-07-13 19:40:24.000000 sbol3-1.1/sbol3/property_base.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    10652 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/provenance.py
+drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2023-04-11 14:49:54.287371 sbol3-1.1/sbol3/rdf/
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    67451 2023-04-04 14:40:42.000000 sbol3-1.1/sbol3/rdf/sbol3-shapes.ttl
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     4179 2023-04-11 14:28:04.000000 sbol3-1.1/sbol3/refobj_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2064 2022-02-11 18:09:28.000000 sbol3-1.1/sbol3/seqfeat.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2664 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/sequence.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3116 2022-02-11 18:09:28.000000 sbol3-1.1/sbol3/subcomponent.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2514 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/text_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    10541 2023-04-04 14:40:18.000000 sbol3-1.1/sbol3/toplevel.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      480 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/typing.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2368 2021-11-16 16:30:04.000000 sbol3-1.1/sbol3/uri_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1177 2021-08-04 19:19:43.000000 sbol3-1.1/sbol3/util.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      586 2020-10-13 14:37:11.000000 sbol3-1.1/sbol3/utils.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1891 2022-01-13 16:21:50.000000 sbol3-1.1/sbol3/validation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     4595 2022-02-11 18:09:28.000000 sbol3-1.1/sbol3/varcomp.py
+drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2023-04-11 14:49:54.286929 sbol3-1.1/sbol3.egg-info/
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      773 2023-04-11 14:49:54.000000 sbol3-1.1/sbol3.egg-info/PKG-INFO
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2031 2023-04-11 14:49:54.000000 sbol3-1.1/sbol3.egg-info/SOURCES.txt
+-rw-r--r--   0 tmitchel (385877172) staff       (20)        1 2023-04-11 14:49:54.000000 sbol3-1.1/sbol3.egg-info/dependency_links.txt
+-rw-r--r--   0 tmitchel (385877172) staff       (20)       57 2023-04-11 14:49:54.000000 sbol3-1.1/sbol3.egg-info/requires.txt
+-rw-r--r--   0 tmitchel (385877172) staff       (20)        6 2023-04-11 14:49:54.000000 sbol3-1.1/sbol3.egg-info/top_level.txt
+-rw-r--r--   0 tmitchel (385877172) staff       (20)       75 2023-04-11 14:49:54.334126 sbol3-1.1/setup.cfg
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1841 2023-03-31 19:00:53.000000 sbol3-1.1/setup.py
+drwxr-xr-x   0 tmitchel (385877172) staff       (20)        0 2023-04-11 14:49:54.332043 sbol3-1.1/test/
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1315 2021-02-01 20:16:49.000000 sbol3-1.1/test/test_annotation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1553 2021-04-21 21:17:59.000000 sbol3-1.1/test/test_attachment.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3908 2021-10-25 20:23:20.000000 sbol3-1.1/test/test_collection.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1869 2021-10-08 19:54:45.000000 sbol3-1.1/test/test_combderiv.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    10572 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_component.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1522 2021-10-08 19:54:45.000000 sbol3-1.1/test/test_compref.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2094 2021-05-26 13:23:53.000000 sbol3-1.1/test/test_config.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     9052 2023-04-11 14:28:17.000000 sbol3-1.1/test/test_custom.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)    31574 2022-10-20 17:40:16.000000 sbol3-1.1/test/test_document.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2139 2021-08-04 19:51:11.000000 sbol3-1.1/test/test_examples.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1405 2021-04-21 20:58:26.000000 sbol3-1.1/test/test_expdata.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2382 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_extdef.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1612 2021-04-21 21:17:59.000000 sbol3-1.1/test/test_extension.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1292 2023-04-04 14:40:15.000000 sbol3-1.1/test/test_feature.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     4418 2022-02-14 17:44:12.000000 sbol3-1.1/test/test_identified.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1725 2021-04-21 20:58:26.000000 sbol3-1.1/test/test_implementation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1915 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_interaction.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1548 2021-09-27 15:30:45.000000 sbol3-1.1/test/test_interface.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1299 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_localsub.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3426 2021-04-21 20:58:26.000000 sbol3-1.1/test/test_location.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     5229 2021-04-30 19:21:10.000000 sbol3-1.1/test/test_module.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2658 2022-02-08 20:19:42.000000 sbol3-1.1/test/test_object.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     5290 2021-02-01 20:16:50.000000 sbol3-1.1/test/test_om_compound.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2595 2021-02-01 20:16:50.000000 sbol3-1.1/test/test_om_prefix.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     7045 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_om_unit.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     8516 2021-04-21 21:17:59.000000 sbol3-1.1/test/test_ownedobject.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2031 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_participation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     6416 2022-02-10 16:51:57.000000 sbol3-1.1/test/test_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     4297 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_provenance.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     5359 2023-04-04 15:07:10.000000 sbol3-1.1/test/test_referenced_object.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     7988 2022-02-11 17:13:16.000000 sbol3-1.1/test/test_roundtrip.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     1802 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_seqfeat.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     4903 2021-11-16 16:30:04.000000 sbol3-1.1/test/test_sequence.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2069 2022-06-14 17:20:34.000000 sbol3-1.1/test/test_style.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2659 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_subcomponent.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     2283 2021-11-16 16:30:04.000000 sbol3-1.1/test/test_text_property.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     7477 2022-02-08 20:19:42.000000 sbol3-1.1/test/test_toplevel.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      853 2021-08-04 19:19:43.000000 sbol3-1.1/test/test_util.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)      966 2021-02-01 20:16:50.000000 sbol3-1.1/test/test_utils.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3989 2022-02-08 20:19:42.000000 sbol3-1.1/test/test_validation.py
+-rw-r--r--   0 tmitchel (385877172) staff       (20)     3878 2022-02-11 18:09:28.000000 sbol3-1.1/test/test_varcomp.py
```

### Comparing `sbol3-1.0rc1/PKG-INFO` & `sbol3-1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sbol3
-Version: 1.0rc1
+Version: 1.1
 Summary: Python implementation of SBOL 3 standard
 Home-page: https://github.com/SynBioDex/pySBOL3
 Author: Tom Mitchell
 Author-email: tcmitchell@users.noreply.github.com
 License: MIT License
-Description: UNKNOWN
 Keywords: synthetic biology
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE.txt
```

### Comparing `sbol3-1.0rc1/README.md` & `sbol3-1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+![pySBOL3 logo](logos/pySBOL3-logo-small.jpeg)
+# pySBOL3
 ![gh-action badge](https://github.com/SynBioDex/pySBOL3/workflows/Python%20package/badge.svg)
 ![readthedocs badge](https://readthedocs.org/projects/pysbol3/badge/)
-# pySBOL3
 
-This is a [Python](https://www.python.org/) implementation of the
-[SBOL 3 specification](https://sbolstandard.org/datamodel-specification/).
-pySBOL3 implements [SBOL 3.0.1](https://sbolstandard.org/docs/SBOL3.0.1.pdf).
+pySBOL3 is a
+[Python](https://www.python.org/) implementation of the [SBOL 3
+specification](https://sbolstandard.org/datamodel-specification/).
+pySBOL3 implements [SBOL
+3.0.1](https://sbolstandard.org/docs/SBOL3.0.1.pdf).
 
 ## Installation
 
 pySBOL3 requires [Python 3.7](https://www.python.org) or newer.
 
 Use `pip` (or `pip3`) to install the library:
 
@@ -26,10 +29,15 @@
 [fork the GitHub repository](https://guides.github.com/activities/forking/),
 and follow
 [GitHub flow](https://guides.github.com/introduction/flow/)
 for development.
 
 ## Acknowledgements
 
+If you use pySBOL3 please cite:
+> Tom Mitchell, Jacob Beal, and Bryan Bartley.
+> [pySBOL3: SBOL3 for Python Programmers](https://doi.org/10.1021/acssynbio.2c00249).
+> ACS Synthetic Biology, available online June 29, 2022. PMID: 35767721.
+
 Development of this library has been supported by the 
 [DARPA Synergistic Discovery and Design (SD2)](https://www.darpa.mil/program/synergistic-discovery-and-design)
 program and [Raytheon BBN Technologies](http://bbn.com/).
```

### Comparing `sbol3-1.0rc1/sbol3/__init__.py` & `sbol3-1.1/sbol3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0rc1'
+__version__ = '1.1'
 
 from .constants import *
 from .config import set_defaults, get_namespace, set_namespace
 from .error import *
 from .validation import *
 from .object import SBOLObject
 from .property_base import Property, SingletonProperty, ListProperty
```

### Comparing `sbol3-1.0rc1/sbol3/attachment.py` & `sbol3-1.1/sbol3/attachment.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/boolean_property.py` & `sbol3-1.1/sbol3/boolean_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/collection.py` & `sbol3-1.1/sbol3/collection.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/combderiv.py` & `sbol3-1.1/sbol3/combderiv.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/component.py` & `sbol3-1.1/sbol3/component.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/compref.py` & `sbol3-1.1/sbol3/compref.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/config.py` & `sbol3-1.1/sbol3/config.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/constants.py` & `sbol3-1.1/sbol3/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------
 # Constants to support SBOL 3
 #
-# See https://sbolstandard.org/data-model-specification/ for the latest version.
+# See https://sbolstandard.org/datamodel-specification/ for the latest version.
 # --------------------------------------------------
 
 SBOL_LOGGER_NAME = 'sbol3'
 
 # ----------
 # Namespaces
 # ----------
```

### Comparing `sbol3-1.0rc1/sbol3/constraint.py` & `sbol3-1.1/sbol3/constraint.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/custom.py` & `sbol3-1.1/sbol3/custom.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/datetime_property.py` & `sbol3-1.1/sbol3/datetime_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/document.py` & `sbol3-1.1/sbol3/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import collections
 import logging
 import os
 import posixpath
 import warnings
+from pathlib import Path
 from typing import Dict, Callable, List, Optional, Any, Union, Iterable
 
 # import typing for typing.Sequence, which we don't want to confuse
 # with sbol3.Sequence
 import typing as pytyping
 
 import pyshacl
@@ -45,14 +48,20 @@
         """
         Document._uri_type_map[type_uri] = builder
 
     # Map type URIs to a builder function to construct entities from
     # RDF triples.
     _uri_type_map: Dict[str, Callable[[str, str], Identified]] = BUILDER_REGISTER
 
+    @staticmethod
+    def open(location: Union[Path, str], file_format: str = None) -> Document:
+        doc = Document()
+        doc.read(location, file_format=file_format)
+        return doc
+
     def __init__(self):
         self.logger = logging.getLogger(SBOL_LOGGER_NAME)
         self.objects: List[TopLevel] = []
         # Orphans are non-TopLevel objects that are not otherwise linked
         # into the object hierarchy.
         self.orphans: List[Identified] = []
         self._namespaces: Dict[str, str] = _default_bindings.copy()
@@ -182,36 +191,42 @@
             obj = self._build_object(identity, types)
             if obj:
                 obj.document = self
                 result[obj.identity] = obj
         return result
 
     @staticmethod
-    def _parse_attributes(objects, graph):
+    def _parse_attributes(objects, graph) -> dict[str, Identified]:
+        # Track the child objects that get assigned to optimize the
+        # search for orphans later in the loading process.
+        child_objects = dict()
         for s, p, o in graph.triples((None, None, None)):
             str_s = str(s)
             str_p = str(p)
             try:
                 obj = objects[str_s]
             except KeyError:
                 # Object is not an SBOL object, skip it
                 continue
             if str_p in obj._owned_objects:
                 other_identity = str(o)
                 other = objects[other_identity]
                 obj._owned_objects[str_p].append(other)
+                # Record the assigned object as a child
+                child_objects[other_identity] = other
             elif str_p == RDF_TYPE:
                 # Handle rdf:type specially because the main type(s)
                 # will already be in the list from the build_object
                 # phase and those entries need to be maintained and
                 # we don't want duplicates
                 if o not in obj._properties[str_p]:
                     obj._properties[str_p].append(o)
             else:
                 obj._properties[str_p].append(o)
+        return child_objects
 
     @staticmethod
     def _clean_up_singletons(objects: Dict[str, SBOLObject]):
         """Clean up singleton properties after reading an SBOL file.
 
         When an SBOL file is read, values are appended to the property
         stores without knowledge of which stores are singletons and
@@ -233,31 +248,35 @@
 
     def clear(self) -> None:
         self.objects.clear()
         self._namespaces = _default_bindings.copy()
 
     def _parse_graph(self, graph) -> None:
         objects = self._parse_objects(graph)
-        self._parse_attributes(objects, graph)
+        child_objects = self._parse_attributes(objects, graph)
         self._clean_up_singletons(objects)
         # Validate all the objects
         # TODO: Where does this belong? Is this automatic?
         #       Or should a user invoke validate?
         # for obj in objects.values():
         #     obj.validate()
+
+        # Extract the top_levels to a dictionary to speed up the search
+        # for orphans below.
+        top_levels = {uri: obj for uri, obj in objects.items()
+                      if isinstance(obj, TopLevel)}
         # Store the TopLevel objects in the Document
-        self.objects = [obj for uri, obj in objects.items()
-                        if isinstance(obj, TopLevel)]
+        self.objects = list(top_levels.values())
         # Gather Orphans for future writing.
         # These are expected to be non-TopLevel annotation objects whose owners
         # have no custom implementation (i.e. no builder registered). These objects
         # will be written out as part of Document.write_string()
         self.orphans = []
         for uri, obj in objects.items():
-            if obj in self.objects:
+            if uri in top_levels or uri in child_objects:
                 continue
             found = self.find(uri)
             if found:
                 continue
             self.orphans.append(obj)
         # Store the namespaces in the Document for later use
         for prefix, uri in graph.namespaces():
@@ -297,23 +316,24 @@
         }
         if file_format in types_with_standard_extension:
             return types_with_standard_extension[file_format]
         else:
             raise ValueError('Provided file format is not a valid one.')
 
     # Formats: 'n3', 'nt', 'turtle', 'xml'
-    def read(self, location: str, file_format: str = None) -> None:
+    def read(self, location: Union[Path, str], file_format: str = None) -> None:
+        _location = str(location)  # normalize location to a string
         if file_format is None:
-            file_format = self._guess_format(location)
+            file_format = self._guess_format(_location)
         if file_format is None:
             raise ValueError('Unable to determine file format')
         if file_format == SORTED_NTRIPLES:
             file_format = NTRIPLES
         graph = rdflib.Graph()
-        graph.parse(location, format=file_format)
+        graph.parse(_location, format=file_format)
         return self._parse_graph(graph)
 
     # Formats: 'n3', 'nt', 'turtle', 'xml'
     def read_string(self, data: str, file_format: str) -> None:
         # TODO: clear the document, this isn't append
         if file_format == SORTED_NTRIPLES:
             file_format = NTRIPLES
@@ -408,52 +428,56 @@
         a list of bytes, and a str if the input was a list of str.
         """
         if not lines:
             return ''
         lines_type = type(lines[0])
         if lines_type is bytes:
             # rdflib 5
-            return b''.join(lines)
+            return b'\n'.join(lines) + b'\n'
         elif lines_type is str:
             # rdflib 6
-            return ''.join(lines)
+            return '\n'.join(lines) + '\n'
 
     def write_string(self, file_format: str) -> str:
         graph = self.graph()
-        if file_format == SORTED_NTRIPLES:
-            # have RDFlib give us the ntriples as a string
+        if file_format in (NTRIPLES, SORTED_NTRIPLES):
+            # RDFlib puts in an extra blank line so we handle N-Triples
+            # in a special way to get rid of the extra line.
+
+            # Have RDFlib give us the n-triples as a string
             nt_text = graph.serialize(format=NTRIPLES)
-            # split it into lines
-            lines = nt_text.splitlines(keepends=True)
-            # sort those lines
-            lines.sort()
-            # write out the lines
-            # RDFlib gives us bytes, so open file in binary mode
+            # Split it into lines and filter out the blank lines
+            lines = [line for line in nt_text.splitlines() if line]
+            if file_format == SORTED_NTRIPLES:
+                # sort the lines
+                lines.sort()
+            # Join the lines together
             result = self.join_lines(lines)
         elif file_format == JSONLD:
             context = {f'@{prefix}': uri for prefix, uri in self._namespaces.items()}
             result = graph.serialize(format=file_format, context=context)
         else:
             result = graph.serialize(format=file_format)
         if type(result) is bytes:
             result = result.decode()
         return result
 
-    def write(self, fpath: str, file_format: str = None) -> None:
+    def write(self, fpath: Union[Path, str], file_format: str = None) -> None:
         """Write the document to file.
 
         If file_format is None the desired format is guessed from the
         extension of fpath. If file_format cannot be guessed a ValueError
         is raised.
         """
+        _fpath = str(fpath)  # normalize fpath to a string
         if file_format is None:
-            file_format = self._guess_format(fpath)
+            file_format = self._guess_format(_fpath)
         if file_format is None:
             raise ValueError('Unable to determine file format')
-        with open(fpath, 'w') as outfile:
+        with open(_fpath, 'w') as outfile:
             outfile.write(self.write_string(file_format))
 
     def graph(self) -> rdflib.Graph:
         """Convert document to an RDF Graph.
 
         The returned graph is a snapshot of the document and will
         not be updated by subsequent changes to the document.
@@ -691,29 +715,33 @@
         for obj in objects:
             obj.remove_from_document()
         # Add each document to this document
         self.add(objects)
 
     @staticmethod
     def change_object_namespace(top_levels: Iterable[TopLevel],
-                                new_namespace: str) -> Any:
+                                new_namespace: str,
+                                update_references: Iterable[TopLevel] = None
+                                ) -> Any:
         """Change the namespace of all TopLevel objects in `top_levels` to
         new_namespace, regardless of the previous value, while
         maintaining referential integrity among all the top level
         objects in top_levels, including their dependents. The
         namespace change is "in place". No new objects are allocated.
 
         Note: this operation can result in an invalid Document if the
         change in namespace creates a naming collision. This method
         does not check for this case either before or after the
         operation. It is up to the caller to decide whether this
         operation is safe.
 
         :param top_levels: objects to change
         :param new_namespace: new namespace for objects
+        :param update_references: objects that should have their references
+                                  updated without changing their namespace
         :return: Nothing
         """
         # Validate the objects and build a map of old name to new name
         objects = []
         identity_map = {}
         for top_level in top_levels:
             if not isinstance(top_level, TopLevel):
@@ -726,14 +754,20 @@
             identity_map[top_level.identity] = top_level
             objects.append((top_level, new_identity))
         # Now change the object identities, and then remap the referenced objects
         for top_level, new_identity in objects:
             top_level.namespace = new_namespace
             top_level.set_identity(new_identity)
             top_level.update_all_dependents(identity_map)
+        # Now update any TopLevels in the update_references group. These are
+        # objects that may have references to the objects that had their
+        # namespace changed.
+        if update_references is not None:
+            for top_level in update_references:
+                top_level.update_all_dependents(identity_map)
         return None
 
     def clone(self) -> List[TopLevel]:
         """Clone the top level objects in this document.
 
         :return: A list of cloned TopLevel objects
         """
```

### Comparing `sbol3-1.0rc1/sbol3/expdata.py` & `sbol3-1.1/sbol3/expdata.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/extdef.py` & `sbol3-1.1/sbol3/extdef.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/feature.py` & `sbol3-1.1/sbol3/feature.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/float_property.py` & `sbol3-1.1/sbol3/float_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/identified.py` & `sbol3-1.1/sbol3/identified.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/implementation.py` & `sbol3-1.1/sbol3/implementation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/int_property.py` & `sbol3-1.1/sbol3/int_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/interaction.py` & `sbol3-1.1/sbol3/interaction.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/interface.py` & `sbol3-1.1/sbol3/interface.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/localsub.py` & `sbol3-1.1/sbol3/localsub.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/location.py` & `sbol3-1.1/sbol3/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     """
 
     def __init__(self, sequence: Union[Sequence, str],
                  identity: str, type_uri: str,
                  *, orientation: Optional[str] = None,
                  order: int = None) -> None:
-        super().__init__(identity, type_uri)
+        super().__init__(identity=identity, type_uri=type_uri)
         self.orientation: uri_singleton = URIProperty(self, SBOL_ORIENTATION, 0, 1,
                                                       initial_value=orientation)
         self.order = IntProperty(self, SBOL_ORDER, 0, 1,
                                  initial_value=order)
         self.sequence = ReferencedObject(self, SBOL_SEQUENCES, 1, 1,
                                          initial_value=sequence)
```

### Comparing `sbol3-1.0rc1/sbol3/model.py` & `sbol3-1.1/sbol3/model.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/object.py` & `sbol3-1.1/sbol3/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import posixpath
 import uuid
 import warnings
 from collections import defaultdict
 from urllib.parse import urlparse
 from typing import Dict, Callable, Optional, Union
 
@@ -107,16 +108,20 @@
         if target_namespace:
 
             # Map the identity of self into the target namespace
             if hasattr(self, 'identity'):
                 old_uri = self.identity
                 new_uri = replace_namespace(old_uri, target_namespace, self.getTypeURI())
 
-        new_obj = BUILDER_REGISTER[self.type_uri](**dict(identity=new_uri,
-                                                         type_uri=self.type_uri))
+        try:
+            builder = BUILDER_REGISTER[self.type_uri]
+        except KeyError:
+            logging.warning(f'No builder found for {self.type_uri}; assuming {self.__class__.__name__}')
+            builder = self.__class__
+        new_obj = builder(**dict(identity=new_uri, type_uri=self.type_uri))
 
         # Copy properties
         for property_uri, value_store in self._properties.items():
             new_obj._properties[property_uri] = value_store.copy()
 
             # TODO: Map into new namespace
```

### Comparing `sbol3-1.0rc1/sbol3/om_compound.py` & `sbol3-1.1/sbol3/om_compound.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/om_prefix.py` & `sbol3-1.1/sbol3/om_prefix.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/om_unit.py` & `sbol3-1.1/sbol3/om_unit.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/ownedobject.py` & `sbol3-1.1/sbol3/ownedobject.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/participation.py` & `sbol3-1.1/sbol3/participation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/property_base.py` & `sbol3-1.1/sbol3/property_base.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/provenance.py` & `sbol3-1.1/sbol3/provenance.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/rdf/sbol3-shapes.ttl` & `sbol3-1.1/sbol3/rdf/sbol3-shapes.ttl`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/refobj_property.py` & `sbol3-1.1/sbol3/refobj_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/seqfeat.py` & `sbol3-1.1/sbol3/seqfeat.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/sequence.py` & `sbol3-1.1/sbol3/sequence.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/subcomponent.py` & `sbol3-1.1/sbol3/subcomponent.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/text_property.py` & `sbol3-1.1/sbol3/text_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/toplevel.py` & `sbol3-1.1/sbol3/toplevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         :return: Nothing
         """
         self._identity = self._make_identity(new_identity)
         # Set display_id of new object
         self._display_id = self._extract_display_id(self._identity)
 
     def clone(self, new_identity: str = None) -> 'TopLevel':
+        # https://stackoverflow.com/questions/1500718/how-to-override-the-copy-deepcopy-operations-for-a-python-object
         obj = copy.deepcopy(self)
         identity_map = {self.identity: obj}
         # Set identity of new object
         if new_identity is not None:
             obj.set_identity(new_identity)
         # Drop the document pointer
         obj.document = None
@@ -169,15 +170,15 @@
         self._reparent_child_objects()
         # Now remap any properties that reference old identities in the
         # identity_map
         self.traverse(make_update_references_traverser(identity_map))
 
     def copy(self, target_doc=None, target_namespace=None):
         # Delete this method in v1.1
-        warnings.warn('Use sbol3.copy() instead', DeprecationWarning)
+        warnings.warn('Toplevel.copy() is deprecated; use sbol3.copy() instead', DeprecationWarning)
         new_obj = super().copy(target_doc=target_doc, target_namespace=target_namespace)
         # Need to set `document` on all children recursively. That's what happens when
         # you assign to the `document` property of an Identified
         new_obj.document = target_doc
         # Comply with the contract of super.copy()
         return new_obj
```

### Comparing `sbol3-1.0rc1/sbol3/uri_property.py` & `sbol3-1.1/sbol3/uri_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/util.py` & `sbol3-1.1/sbol3/util.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/utils.py` & `sbol3-1.1/sbol3/utils.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/validation.py` & `sbol3-1.1/sbol3/validation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3/varcomp.py` & `sbol3-1.1/sbol3/varcomp.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/sbol3.egg-info/PKG-INFO` & `sbol3-1.1/sbol3.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sbol3
-Version: 1.0rc1
+Version: 1.1
 Summary: Python implementation of SBOL 3 standard
 Home-page: https://github.com/SynBioDex/pySBOL3
 Author: Tom Mitchell
 Author-email: tcmitchell@users.noreply.github.com
 License: MIT License
-Description: UNKNOWN
 Keywords: synthetic biology
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+License-File: LICENSE.txt
```

### Comparing `sbol3-1.0rc1/sbol3.egg-info/SOURCES.txt` & `sbol3-1.1/sbol3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 sbol3/__init__.py
 sbol3/attachment.py
 sbol3/boolean_property.py
 sbol3/collection.py
@@ -62,14 +63,15 @@
 test/test_config.py
 test/test_custom.py
 test/test_document.py
 test/test_examples.py
 test/test_expdata.py
 test/test_extdef.py
 test/test_extension.py
+test/test_feature.py
 test/test_identified.py
 test/test_implementation.py
 test/test_interaction.py
 test/test_interface.py
 test/test_localsub.py
 test/test_location.py
 test/test_module.py
```

### Comparing `sbol3-1.0rc1/setup.py` & `sbol3-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from setuptools import setup
 
 setup(name='sbol3',
-      version='1.0rc1',
+      version='1.1',
       description='Python implementation of SBOL 3 standard',
       python_requires='>=3.7',
       url='https://github.com/SynBioDex/pySBOL3',
       author='Tom Mitchell',
       author_email='tcmitchell@users.noreply.github.com',
       license='MIT License',
       # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
             # How mature is this project? Common values are
             #   3 - Alpha
             #   4 - Beta
             #   5 - Production/Stable
-            'Development Status :: 4 - Beta',
+            'Development Status :: 5 - Production/Stable',
 
             # Indicate who your project is intended for
             'Intended Audience :: Developers',
 
             # Pick your license as you wish (should match "license" above)
             'License :: OSI Approved :: MIT License',
 
             # Specify the Python versions you support here. In particular, ensure
             # that you indicate whether you support Python 2, Python 3 or both.
             'Programming Language :: Python :: 3 :: Only',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
-
+            'Programming Language :: Python :: 3.11',
       ],
       # What does your project relate to?
       keywords='synthetic biology',
       packages=['sbol3'],
       package_data={'sbol3': ['rdf/sbol3-shapes.ttl']},
       install_requires=[
-            # Require at least rdflib 6.0.1, and allow newer versions
+            # Require at least rdflib 6.1.1, and allow newer versions
             # of rdflib 6.x
             'rdflib>=6.1.1,==6.*',
             'python-dateutil~=2.8.2',
-            'pyshacl~=0.18.1',
+            'pyshacl~=0.19',
       ],
       test_suite='test',
       tests_require=[
             'pycodestyle~=2.8.0'
       ])
```

### Comparing `sbol3-1.0rc1/test/test_annotation.py` & `sbol3-1.1/test/test_annotation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_attachment.py` & `sbol3-1.1/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_collection.py` & `sbol3-1.1/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_combderiv.py` & `sbol3-1.1/test/test_combderiv.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_component.py` & `sbol3-1.1/test/test_component.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_compref.py` & `sbol3-1.1/test/test_compref.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_config.py` & `sbol3-1.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_custom.py` & `sbol3-1.1/test/test_custom.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,61 @@
 import math
 import os
 import tempfile
 import unittest
-
-import rdflib
+import warnings
+from typing import Union
 
 import sbol3
 
 
 PYSBOL3_CUSTOM_TOP = 'https://github.com/synbiodex/pysbol3#customTop'
+PYSBOL3_CUSTOM_UNREGISTERED_TOP = 'https://github.com/synbiodex/pysbol3#customUnregisteredTop'
 PYSBOL3_CUSTOM_BOOL = 'https://github.com/synbiodex/pysbol3#customBool'
 PYSBOL3_CUSTOM_CHILD = 'https://github.com/synbiodex/pysbol3#customChildren'
 PYSBOL3_CUSTOM_IDENTIFIED = 'https://github.com/synbiodex/pysbol3#customIdentified'
 PYSBOL3_CUSTOM_INT = 'https://github.com/synbiodex/pysbol3#customInt'
+PYSBOL3_CUSTOM_LOCATION = 'https://github.com/synbiodex/pysbol3#customLocation'
 
 
 class CustomTopClass(sbol3.CustomTopLevel):
     def __init__(self, identity, type_uri=PYSBOL3_CUSTOM_TOP):
         super().__init__(identity, type_uri)
         # Also test the boolean list while we're here
         self.foo_bool = sbol3.BooleanProperty(self, PYSBOL3_CUSTOM_BOOL,
                                               0, math.inf)
         self.children = sbol3.OwnedObject(self, PYSBOL3_CUSTOM_CHILD, 0, math.inf)
 
 
+class CustomUnregisteredTopClass(sbol3.CustomTopLevel):
+    def __init__(self, identity, type_uri=PYSBOL3_CUSTOM_UNREGISTERED_TOP):
+        super().__init__(identity, type_uri)
+        # Also test the boolean list while we're here
+        self.foo_bool = sbol3.BooleanProperty(self, PYSBOL3_CUSTOM_BOOL,
+                                              0, math.inf)
+        self.children = sbol3.OwnedObject(self, PYSBOL3_CUSTOM_CHILD, 0, math.inf)
+
+
 class CustomIdentifiedClass(sbol3.CustomIdentified):
     def __init__(self, type_uri=PYSBOL3_CUSTOM_IDENTIFIED, identity=None):
         super().__init__(type_uri, identity=identity)
         # Also test the int list while we're here
         self.foo_int = sbol3.IntProperty(self, PYSBOL3_CUSTOM_INT,
                                          0, math.inf)
 
 
+class CustomLocationClass(sbol3.Location, sbol3.CustomIdentified):
+    def __init__(self, sequence: Union[sbol3.Sequence, str],
+                 *, type_uri=PYSBOL3_CUSTOM_LOCATION, identity=None):
+        super().__init__(sequence=sequence, type_uri=type_uri, identity=identity)
+        # Also test the int list while we're here
+        self.foo_int = sbol3.IntProperty(self, PYSBOL3_CUSTOM_INT,
+                                         0, math.inf)
+
+
 class TestCustomTopLevel(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         sbol3.Document.register_builder(PYSBOL3_CUSTOM_TOP, CustomTopClass)
 
     @classmethod
@@ -70,26 +90,47 @@
         sbol3.set_namespace('https://github.com/synbiodex/pysbol3')
         obj_name = 'bool_test'
         obj = CustomTopClass(obj_name)
         self.assertEqual([], obj.foo_bool)
         obj.foo_bool.append(True)
         obj.foo_bool.append(False)
         self.assertEqual([True, False], obj.foo_bool)
+        obj_unregistered_name = 'bool_test_unregistered'
+        obj_u = CustomUnregisteredTopClass(obj_unregistered_name)
+        obj_u.foo_bool.append(True)
+        self.assertEqual([True], obj_u.foo_bool)
         doc = sbol3.Document()
         doc.add(obj)
+        doc.add(obj_u)
         doc2 = sbol3.Document()
         # Round trip the document
         with tempfile.TemporaryDirectory() as tmpdirname:
             test_file = os.path.join(tmpdirname, 'custom.nt')
             doc.write(test_file, sbol3.NTRIPLES)
             doc2.read(test_file, sbol3.NTRIPLES)
         obj2 = doc2.find(obj_name)
+        obj_u2 = doc2.find(obj_unregistered_name)
         # The lists are necessarily unordered because of RDF
-        # Compare specially
-        self.assertCountEqual([True, False], obj2.foo_bool)
+        self.assertCountEqual([False, True], obj2.foo_bool)
+        unregistered_values = obj_u2._properties['https://github.com/synbiodex/pysbol3#customBool']
+        self.assertEqual(['true'], [str(x) for x in unregistered_values])
+
+        # Finally, make sure the objects can be copied into a new document
+        doc3 = sbol3.Document()
+        # This test deliberately uses the old copy function, as that was where an error previously occurred
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", DeprecationWarning)
+            obj2.copy(doc3)
+            obj_u2.copy(doc3)
+        obj3 = doc3.find(obj_name)
+        obj_u3 = doc3.find(obj_unregistered_name)
+        # The lists are necessarily unordered because of RDF
+        self.assertCountEqual([False, True], obj3.foo_bool)
+        unregistered_values = obj_u3._properties['https://github.com/synbiodex/pysbol3#customBool']
+        self.assertEqual(['true'], [str(x) for x in unregistered_values])
 
     def test_none_identity(self):
         # Make sure a ValueError is raised if None is passed
         # as a CustomTopLevel identity. And also if identity
         # is an empty string or not a string.
         with self.assertRaises(ValueError):
             obj = CustomTopClass(None)
@@ -159,9 +200,23 @@
         tl2 = doc2.find(tl_name)
         obj2 = tl2.children[0]
         # The lists are necessarily unordered because of RDF
         # Compare specially
         self.assertCountEqual([7, 14], obj2.foo_int)
 
 
+class TestCustomLocation(unittest.TestCase):
+
+    def test_constructor(self):
+        """Test construction of a custom `Location`.
+
+        See https://github.com/SynBioDex/pySBOL3/issues/414
+        """
+        sbol3.set_namespace('https://github.com/synbiodex/pysbol3')
+        seq = sbol3.Sequence('my_seq', elements='atcg')
+        custom_loc = CustomLocationClass(sequence=seq)
+        # Simply creating the above class indicates that this fixes bug 414
+        self.assertIsInstance(custom_loc, CustomLocationClass)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sbol3-1.0rc1/test/test_document.py` & `sbol3-1.1/test/test_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 import tempfile
 import unittest
+from pathlib import Path
 from typing import Optional
 
 import rdflib
 
 import sbol3
 
 MODULE_LOCATION = os.path.dirname(os.path.abspath(__file__))
@@ -52,20 +53,18 @@
         # 3. for invalid file formats, valueError must be raised
         with self.assertRaises(ValueError):
             extension_3 = sbol3.Document.file_extension(file_format_3)
 
     def test_read_ntriples(self):
         # Initial test of Document.read
         filename = 'model.nt'
-        test_path = os.path.join(SBOL3_LOCATION, 'entity', 'model',
-                                 filename)
-        doc = sbol3.Document()
-        doc.read(test_path)
+        test_path = Path(SBOL3_LOCATION) / 'entity' / 'model' / filename
+        doc = sbol3.Document.open(test_path)
         with tempfile.TemporaryDirectory() as tmpdirname:
-            test_file = os.path.join(tmpdirname, filename)
+            test_file = Path(tmpdirname) / filename
             doc.write(test_file, sbol3.NTRIPLES)
 
     def test_read_turtle(self):
         # Initial test of Document.read
         test_path = os.path.join(SBOL3_LOCATION, 'entity', 'model',
                                  'model.ttl')
         doc = sbol3.Document()
@@ -613,14 +612,30 @@
         sbol3.set_namespace(namespace)
         doc = sbol3.Document()
         # Non-TopLevel should raise ValueError
         i1 = sbol3.Interaction([sbol3.SBO_INHIBITION])
         with self.assertRaises(ValueError):
             doc.change_object_namespace([i1], new_namespace)
 
+    def test_change_object_namespace_with_references(self):
+        """Test Document.change_object_namespace with outside references.
+
+        See https://github.com/SynBioDex/pySBOL3/issues/412
+        """
+        doc = sbol3.Document()
+        comp = sbol3.Component('http://sbolstandard.org/testfiles/hello',
+                               sbol3.SBO_DNA)
+        seq = sbol3.Sequence('http://sbolstandard.org/testfiles/hello_sequence',
+                             elements='ATGC')
+        doc.add(comp)
+        doc.add(seq)
+        comp.sequences = [seq]
+        doc.change_object_namespace([seq], 'http://parts.igem.org', doc)
+        self.assertEqual(seq.identity, comp.sequences[0])
+
     def test_clone(self):
         namespace = 'https://github.com/synbiodex/pysbol3'
         sbol3.set_namespace(namespace)
         test_path = os.path.join(SBOL3_LOCATION, 'multicellular',
                                  'multicellular.ttl')
         doc = sbol3.Document()
         doc.read(test_path)
@@ -704,10 +719,33 @@
         # Copy the top level into a new document
         doc2 = sbol3.Document()
         sbol3.copy([tmp_c1], into_document=doc2)
         doc2_string = doc2.write_string(sbol3.SORTED_NTRIPLES)
         # Verify that the serializations are identical
         self.assertEqual(doc1_string, doc2_string)
 
+    def test_ntriples_blank_line(self):
+        """Test that ntriples output does not contain an extra blank
+        line due to RDFlib.
+
+        See https://github.com/SynBioDex/pySBOL3/issues/404
+        """
+        sbol3.set_namespace('https://github.com/synbiodex/pysbol3')
+        c1 = sbol3.Component('c1', types=[sbol3.SBO_DNA])
+        doc = sbol3.Document()
+        doc.add(c1)
+        output = doc.write_string(file_format=sbol3.NTRIPLES)
+        lines = output.splitlines()
+        num_blanks = sum([1 for line in lines if not line])
+        # Expecting no blank lines
+        self.assertEqual(0, num_blanks)
+
+        # Now test sorted n-triples
+        sorted_output = doc.write_string(file_format=sbol3.SORTED_NTRIPLES)
+        sorted_lines = sorted_output.splitlines()
+        num_blanks = sum([1 for line in sorted_lines if not line])
+        # Expecting no blank lines
+        self.assertEqual(0, num_blanks)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sbol3-1.0rc1/test/test_examples.py` & `sbol3-1.1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_expdata.py` & `sbol3-1.1/test/test_expdata.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_extdef.py` & `sbol3-1.1/test/test_extdef.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_extension.py` & `sbol3-1.1/test/test_extension.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_identified.py` & `sbol3-1.1/test/test_identified.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_implementation.py` & `sbol3-1.1/test/test_implementation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_interaction.py` & `sbol3-1.1/test/test_interaction.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_interface.py` & `sbol3-1.1/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_localsub.py` & `sbol3-1.1/test/test_localsub.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_location.py` & `sbol3-1.1/test/test_location.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_module.py` & `sbol3-1.1/test/test_module.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_object.py` & `sbol3-1.1/test/test_object.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_om_compound.py` & `sbol3-1.1/test/test_om_compound.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_om_prefix.py` & `sbol3-1.1/test/test_om_prefix.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_om_unit.py` & `sbol3-1.1/test/test_om_unit.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_ownedobject.py` & `sbol3-1.1/test/test_ownedobject.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_participation.py` & `sbol3-1.1/test/test_participation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_property.py` & `sbol3-1.1/test/test_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_provenance.py` & `sbol3-1.1/test/test_provenance.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_referenced_object.py` & `sbol3-1.1/test/test_referenced_object.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_roundtrip.py` & `sbol3-1.1/test/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_seqfeat.py` & `sbol3-1.1/test/test_seqfeat.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_sequence.py` & `sbol3-1.1/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_style.py` & `sbol3-1.1/test/test_style.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_subcomponent.py` & `sbol3-1.1/test/test_subcomponent.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_text_property.py` & `sbol3-1.1/test/test_text_property.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_toplevel.py` & `sbol3-1.1/test/test_toplevel.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_util.py` & `sbol3-1.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_utils.py` & `sbol3-1.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_validation.py` & `sbol3-1.1/test/test_validation.py`

 * *Files identical despite different names*

### Comparing `sbol3-1.0rc1/test/test_varcomp.py` & `sbol3-1.1/test/test_varcomp.py`

 * *Files identical despite different names*

