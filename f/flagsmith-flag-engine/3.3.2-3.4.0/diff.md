# Comparing `tmp/flagsmith-flag-engine-3.3.2.tar.gz` & `tmp/flagsmith-flag-engine-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-flag-engine-3.3.2.tar", last modified: Wed Mar 29 09:22:54 2023, max compression
+gzip compressed data, was "flagsmith-flag-engine-3.4.0.tar", last modified: Tue Apr 11 08:39:11 2023, max compression
```

## Comparing `flagsmith-flag-engine-3.3.2.tar` & `flagsmith-flag-engine-3.4.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.325092 flagsmith-flag-engine-3.3.2/flag_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.325092 flagsmith-flag-engine-3.3.2/flag_engine/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/document_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.325092 flagsmith-flag-engine-3.3.2/flag_engine/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.325092 flagsmith-flag-engine-3.3.2/flag_engine/environments/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/integrations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/integrations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/environments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/features/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/features/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/identities/traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/traits/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/identities/traits/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/organisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/organisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/organisations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/organisations/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/projects/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/segments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/segments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/segments/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/segments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/segments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/utils/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/json/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flag_engine/utils/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/marshmallow/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/marshmallow/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/semver.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/flag_engine/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-29 09:22:54.000000 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-29 09:22:54.000000 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:22:54.000000 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-29 09:22:54.000000 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-29 09:22:54.000000 flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-29 09:22:54.329092 flagsmith-flag-engine-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-29 09:22:53.000000 flagsmith-flag-engine-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/document_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/environments/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/integrations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/integrations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/environments/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/features/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/features/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/identities/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/traits/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/identities/traits/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/organisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/organisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/organisations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/organisations/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.944601 flagsmith-flag-engine-3.4.0/flag_engine/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/projects/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/projects/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/flag_engine/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/segments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/segments/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/segments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/segments/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/flag_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/flag_engine/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/json/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/flag_engine/utils/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/marshmallow/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/marshmallow/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/flag_engine/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-11 08:39:11.000000 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-11 08:39:11.000000 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:39:11.000000 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 08:39:11.000000 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 08:39:11.000000 flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 08:39:11.948602 flagsmith-flag-engine-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-11 08:39:10.000000 flagsmith-flag-engine-3.4.0/setup.py
```

### Comparing `flagsmith-flag-engine-3.3.2/LICENSE.txt` & `flagsmith-flag-engine-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/PKG-INFO` & `flagsmith-flag-engine-3.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 3.3.2
+Version: 3.4.0
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-3.3.2/README.md` & `flagsmith-flag-engine-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/api/document_builders.py` & `flagsmith-flag-engine-3.4.0/flag_engine/api/document_builders.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/api/fields.py` & `flagsmith-flag-engine-3.4.0/flag_engine/api/fields.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/api/filters.py` & `flagsmith-flag-engine-3.4.0/flag_engine/api/filters.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/api/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/api/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/engine.py` & `flagsmith-flag-engine-3.4.0/flag_engine/engine.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/environments/builders.py` & `flagsmith-flag-engine-3.4.0/flag_engine/environments/builders.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/environments/models.py` & `flagsmith-flag-engine-3.4.0/flag_engine/environments/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     project: ProjectModel
     feature_states: typing.List[FeatureStateModel] = field(default_factory=list)
 
     name: str = None
     allow_client_traits: bool = True
     updated_at: datetime = field(default_factory=utcnow_with_tz)
     use_mv_v2_evaluation: bool = False
+    hide_sensitive_data: bool = False
 
     amplitude_config: IntegrationModel = None
     segment_config: IntegrationModel = None
     mixpanel_config: IntegrationModel = None
     heap_config: IntegrationModel = None
     dynatrace_config: IntegrationModel = None
     webhook_config: WebhookModel = None
```

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/environments/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/environments/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     api_key = fields.Str()
     updated_at = fields.DateTime()
 
     name = fields.Str(required=False)
     allow_client_traits = fields.Bool(required=False, default=True)
     hide_disabled_flags = fields.Bool(required=False, allow_none=True)
     use_mv_v2_evaluation = fields.Bool(required=False, default=False)
+    hide_sensitive_data = fields.Bool(required=False, default=False)
 
     segment_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     heap_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     mixpanel_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     amplitude_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     dynatrace_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     webhook_config = fields.Nested(WebhookSchema, required=False, allow_none=True)
```

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/features/models.py` & `flagsmith-flag-engine-3.4.0/flag_engine/features/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/features/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/features/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/identities/models.py` & `flagsmith-flag-engine-3.4.0/flag_engine/identities/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/identities/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/identities/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/identities/traits/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/identities/traits/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/projects/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/projects/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/segments/constants.py` & `flagsmith-flag-engine-3.4.0/flag_engine/segments/constants.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/segments/evaluator.py` & `flagsmith-flag-engine-3.4.0/flag_engine/segments/evaluator.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/segments/models.py` & `flagsmith-flag-engine-3.4.0/flag_engine/segments/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/segments/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/segments/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/utils/hashing.py` & `flagsmith-flag-engine-3.4.0/flag_engine/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/utils/marshmallow/schemas.py` & `flagsmith-flag-engine-3.4.0/flag_engine/utils/marshmallow/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/utils/semver.py` & `flagsmith-flag-engine-3.4.0/flag_engine/utils/semver.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flag_engine/utils/types.py` & `flagsmith-flag-engine-3.4.0/flag_engine/utils/types.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/PKG-INFO` & `flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 3.3.2
+Version: 3.4.0
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-3.3.2/flagsmith_flag_engine.egg-info/SOURCES.txt` & `flagsmith-flag-engine-3.4.0/flagsmith_flag_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.3.2/setup.py` & `flagsmith-flag-engine-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="flagsmith-flag-engine",
-    version="3.3.2",
+    version="3.4.0",
     author="Flagsmith",
     author_email="support@flagsmith.com",
     packages=find_packages(include=["flag_engine", "flag_engine.*"]),
     url="https://github.com/Flagsmith/flagsmith-engine",
     license="BSD3",
     description="Flag engine for the Flagsmith API.",
     long_description=open("README.md").read(),
```

