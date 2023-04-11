# Comparing `tmp/duqtools-1.6.4.tar.gz` & `tmp/duqtools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duqtools-1.6.4.tar", last modified: Thu Mar 23 12:25:00 2023, max compression
+gzip compressed data, was "duqtools-1.7.0.tar", last modified: Tue Apr 11 09:45:53 2023, max compression
```

## Comparing `duqtools-1.6.4.tar` & `duqtools-1.7.0.tar`

### file list

```diff
@@ -1,107 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.663648 duqtools-1.6.4/
--rw-rw-rw-   0        0        0    11558 2022-05-16 07:57:55.000000 duqtools-1.6.4/LICENSE
--rw-rw-rw-   0        0        0       89 2022-09-20 13:39:43.000000 duqtools-1.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3479 2023-03-23 12:25:00.664622 duqtools-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     2316 2022-11-23 08:27:52.000000 duqtools-1.6.4/README.md
--rw-rw-rw-   0        0        0     2240 2023-03-08 09:57:06.000000 duqtools-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0     2432 2023-03-23 12:25:00.667616 duqtools-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-05-03 08:05:43.000000 duqtools-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:24:59.010753 duqtools-1.6.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-23 12:24:59.442018 duqtools-1.6.4/src/duqtools/
--rw-rw-rw-   0        0        0      747 2023-03-23 12:14:47.000000 duqtools-1.6.4/src/duqtools/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/_click_opt_groups.py
--rw-rw-rw-   0        0        0     1904 2022-10-06 08:24:23.000000 duqtools-1.6.4/src/duqtools/_logging_utils.py
--rw-rw-rw-   0        0        0     6653 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/_plot_utils.py
--rw-rw-rw-   0        0        0       91 2022-06-08 07:59:21.000000 duqtools-1.6.4/src/duqtools/_types.py
--rw-rw-rw-   0        0        0      977 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/api.py
--rw-rw-rw-   0        0        0     1097 2022-10-21 09:20:36.000000 duqtools-1.6.4/src/duqtools/apply_model.py
--rw-rw-rw-   0        0        0     2115 2022-11-15 09:50:36.000000 duqtools-1.6.4/src/duqtools/cleanup.py
--rw-rw-rw-   0        0        0    15073 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:24:59.815249 duqtools-1.6.4/src/duqtools/config/
--rw-rw-rw-   0        0        0      167 2022-11-22 08:11:23.000000 duqtools-1.6.4/src/duqtools/config/__init__.py
--rw-rw-rw-   0        0        0      874 2022-10-04 10:09:45.000000 duqtools-1.6.4/src/duqtools/config/_config.py
--rw-rw-rw-   0        0        0     5648 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/config/_variables.py
--rw-rw-rw-   0        0        0     9146 2023-03-23 12:14:47.000000 duqtools-1.6.4/src/duqtools/create.py
--rw-rw-rw-   0        0        0      712 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/dash.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:24:59.832253 duqtools-1.6.4/src/duqtools/data/
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.023016 duqtools-1.6.4/src/duqtools/data/dash/
--rw-rw-rw-   0        0        0     2141 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/data/dash/_shared.py
--rw-rw-rw-   0        0        0     2307 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/data/dash/dash.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.026027 duqtools-1.6.4/src/duqtools/data/dash/pages/
--rw-rw-rw-   0        0        0     3871 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/data/dash/pages/1_merge.py
--rw-rw-rw-   0        0        0      162 2022-06-28 11:49:08.000000 duqtools-1.6.4/src/duqtools/data/dash/readme.md
--rw-rw-rw-   0        0        0       45 2022-07-12 08:36:13.000000 duqtools-1.6.4/src/duqtools/data/dash/requirements.txt
--rw-rw-rw-   0        0        0      804 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/data/duqtools.yaml
--rw-rw-rw-   0        0        0     1765 2022-10-21 09:20:36.000000 duqtools-1.6.4/src/duqtools/data/jetto_tools_lookup.json
--rw-rw-rw-   0        0        0      607 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/data/variables.yaml
--rw-rw-rw-   0        0        0     2860 2022-11-25 09:34:04.000000 duqtools-1.6.4/src/duqtools/data/variables_core-profiles.yaml
--rw-rw-rw-   0        0        0     1356 2022-11-25 09:34:04.000000 duqtools-1.6.4/src/duqtools/data/variables_core-sources.yaml
--rw-rw-rw-   0        0        0     3279 2022-11-25 09:34:04.000000 duqtools-1.6.4/src/duqtools/data/variables_equilibrium.yaml
--rw-rw-rw-   0        0        0      731 2023-03-15 14:34:57.000000 duqtools-1.6.4/src/duqtools/data/variables_ids2jetto.yaml
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.232235 duqtools-1.6.4/src/duqtools/ids/
--rw-rw-rw-   0        0        0      655 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/ids/__init__.py
--rw-rw-rw-   0        0        0     2464 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/ids/_apply_model.py
--rw-rw-rw-   0        0        0     3467 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/ids/_copy.py
--rw-rw-rw-   0        0        0    10529 2023-03-23 12:14:47.000000 duqtools-1.6.4/src/duqtools/ids/_handle.py
--rw-rw-rw-   0        0        0     1498 2022-12-15 11:06:29.000000 duqtools-1.6.4/src/duqtools/ids/_imas.py
--rw-rw-rw-   0        0        0    11832 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/ids/_mapping.py
--rw-rw-rw-   0        0        0     2997 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/ids/_merge.py
--rw-rw-rw-   0        0        0     6660 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/ids/_rebase.py
--rw-rw-rw-   0        0        0     1328 2022-11-17 08:08:21.000000 duqtools-1.6.4/src/duqtools/init.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.243195 duqtools-1.6.4/src/duqtools/jetto/
--rw-rw-rw-   0        0        0      415 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/jetto/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-03-23 12:14:47.000000 duqtools-1.6.4/src/duqtools/jetto/_batchfile.py
--rw-rw-rw-   0        0        0     1227 2022-10-25 14:11:30.000000 duqtools-1.6.4/src/duqtools/jetto/_jettovar_to_json.py
--rw-rw-rw-   0        0        0    13075 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/jetto/_system.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.447811 duqtools-1.6.4/src/duqtools/large_scale_validation/
--rw-rw-rw-   0        0        0      102 2022-11-22 08:11:23.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/__init__.py
--rw-rw-rw-   0        0        0     3452 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/cli.py
--rw-rw-rw-   0        0        0      542 2023-03-21 11:06:02.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/create.py
--rw-rw-rw-   0        0        0     1917 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/merge.py
--rw-rw-rw-   0        0        0      483 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/setup.py
--rw-rw-rw-   0        0        0     1322 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/status.py
--rw-rw-rw-   0        0        0     1795 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/large_scale_validation/submit.py
--rw-rw-rw-   0        0        0     1770 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/list_variables.py
--rw-rw-rw-   0        0        0     3339 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/matrix_samplers.py
--rw-rw-rw-   0        0        0     2925 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/merge.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.456810 duqtools-1.6.4/src/duqtools/models/
--rw-rw-rw-   0        0        0      195 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/models/__init__.py
--rw-rw-rw-   0        0        0     3590 2023-03-17 07:51:38.000000 duqtools-1.6.4/src/duqtools/models/_job.py
--rw-rw-rw-   0        0        0     1777 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/models/_locations.py
--rw-rw-rw-   0        0        0     2506 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/models/_system.py
--rw-rw-rw-   0        0        0    11999 2023-03-08 15:22:32.000000 duqtools-1.6.4/src/duqtools/operations.py
--rw-rw-rw-   0        0        0     2237 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/plot.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.581333 duqtools-1.6.4/src/duqtools/schema/
--rw-rw-rw-   0        0        0      630 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/schema/__init__.py
--rw-rw-rw-   0        0        0      254 2022-08-25 13:08:52.000000 duqtools-1.6.4/src/duqtools/schema/_basemodel.py
--rw-rw-rw-   0        0        0      151 2022-07-13 07:00:32.000000 duqtools-1.6.4/src/duqtools/schema/_description_helpers.py
--rw-rw-rw-   0        0        0     5397 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/schema/_dimensions.py
--rw-rw-rw-   0        0        0      896 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/schema/_imas.py
--rw-rw-rw-   0        0        0     1491 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/schema/_jetto.py
--rw-rw-rw-   0        0        0     1368 2022-10-03 07:23:34.000000 duqtools-1.6.4/src/duqtools/schema/_ranges.py
--rw-rw-rw-   0        0        0     3283 2023-03-15 14:34:57.000000 duqtools-1.6.4/src/duqtools/schema/_variable.py
--rw-rw-rw-   0        0        0     8074 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/schema/cli.py
--rw-rw-rw-   0        0        0     1674 2022-12-15 11:06:29.000000 duqtools-1.6.4/src/duqtools/schema/data_location.py
--rw-rw-rw-   0        0        0     1046 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/schema/matrix_samplers.py
--rw-rw-rw-   0        0        0     1022 2023-01-18 11:39:13.000000 duqtools-1.6.4/src/duqtools/schema/runs.py
--rw-rw-rw-   0        0        0      593 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/schema/variables.py
--rw-rw-rw-   0        0        0     6994 2023-03-15 14:34:57.000000 duqtools-1.6.4/src/duqtools/setup.py
--rw-rw-rw-   0        0        0     6630 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/status.py
--rw-rw-rw-   0        0        0     6651 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/submit.py
--rw-rw-rw-   0        0        0     1393 2023-03-08 09:57:06.000000 duqtools-1.6.4/src/duqtools/system.py
--rw-rw-rw-   0        0        0     4119 2023-03-23 12:14:47.000000 duqtools-1.6.4/src/duqtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-23 12:24:59.721671 duqtools-1.6.4/src/duqtools.egg-info/
--rw-rw-rw-   0        0        0     3479 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2808 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-25 10:37:13.000000 duqtools-1.6.4/src/duqtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      570 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-23 12:24:58.000000 duqtools-1.6.4/src/duqtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-23 12:25:00.661615 duqtools-1.6.4/tests/
--rw-rw-rw-   0        0        0     5738 2023-03-08 09:57:06.000000 duqtools-1.6.4/tests/test_cmdline.py
--rw-rw-rw-   0        0        0     3579 2023-03-08 09:57:06.000000 duqtools-1.6.4/tests/test_dry_run.py
--rw-rw-rw-   0        0        0       74 2022-06-08 08:15:23.000000 duqtools-1.6.4/tests/test_duqtools.py
--rw-rw-rw-   0        0        0     2424 2023-03-15 14:34:57.000000 duqtools-1.6.4/tests/test_ids2jetto_variables.py
--rw-rw-rw-   0        0        0     3127 2023-03-08 09:57:06.000000 duqtools-1.6.4/tests/test_operations.py
--rw-rw-rw-   0        0        0      975 2023-03-08 09:57:06.000000 duqtools-1.6.4/tests/test_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.290567 duqtools-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 09:45:49.000000 duqtools-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 09:45:49.000000 duqtools-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 09:45:53.290567 duqtools-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-11 09:45:49.000000 duqtools-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-11 09:45:49.000000 duqtools-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-11 09:45:53.290567 duqtools-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:49.000000 duqtools-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.278567 duqtools-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_click_opt_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/apply_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/config/_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/dash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/data/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/dash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/data/dash/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/pages/1_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/dash/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/duqtools.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/jetto_tools_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_core-profiles.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_core-sources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_equilibrium.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/data/variables_ids2jetto.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/duqmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_apply_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_imas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/ids/_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/jetto/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_batchfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_jettovar_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/jetto/_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/large_scale_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/large_scale_validation/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/list_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/matrix_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.286567 duqtools-1.7.0/src/duqtools/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/models/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.290567 duqtools-1.7.0/src/duqtools/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_description_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_imas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_jetto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/matrix_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/schema/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-11 09:45:49.000000 duqtools-1.7.0/src/duqtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:53.282567 duqtools-1.7.0/src/duqtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:52.000000 duqtools-1.7.0/src/duqtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 09:45:53.000000 duqtools-1.7.0/src/duqtools.egg-info/top_level.txt
```

### Comparing `duqtools-1.6.4/LICENSE` & `duqtools-1.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `duqtools-1.6.4/PKG-INFO` & `duqtools-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,69 @@
-Metadata-Version: 2.1
-Name: duqtools
-Version: 1.6.4
-Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
-Home-page: https://github.com/duqtools/duqtools
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
-Project-URL: Documentation, https://duqtools.readthedocs.io
-Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-Provides-Extra: docs
-Provides-Extra: publishing
-Provides-Extra: imas
-License-File: LICENSE
-
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
-
-# Duqtools
-
-*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
-
-Features:
-
-- Set up 100s of simulation runs from a single template
-- Launch standard sets of sensitivity tests with minimal programming
-- Batch job submission and status tracking
-- Supports the Standardized Interface Data Structures (IDSs) data directory
-- Compare and visualize 100s of simulations in one overview
-- Display simulation results as confidence ranges and distributions
-
-*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
-
-To install:
-
-```console
-pip install duqtools
-```
-
-The source code is available from [Github](https://github.com/duqtools/duqtools).
-
-Suggestions, improvements, and edits are most welcome.
-
-
-## Development
-
-Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
+Metadata-Version: 2.1
+Name: duqtools
+Version: 1.7.0
+Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
+Home-page: https://github.com/duqtools/duqtools
+Author: Stef Smeets
+Author-email: s.smeets@esciencecenter.nl
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
+Project-URL: Documentation, https://duqtools.readthedocs.io
+Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+Provides-Extra: docs
+Provides-Extra: publishing
+Provides-Extra: imas
+License-File: LICENSE
+
+| Source | Badges |
+| --- | --- |
+| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
+| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
+| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
+| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
+| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+
+# Duqtools
+
+*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
+
+Features:
+
+- Set up 100s of simulation runs from a single template
+- Launch standard sets of sensitivity tests with minimal programming
+- Batch job submission and status tracking
+- Supports the Standardized Interface Data Structures (IDSs) data directory
+- Compare and visualize 100s of simulations in one overview
+- Display simulation results as confidence ranges and distributions
+
+*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
+
+To install:
+
+```console
+pip install duqtools
+```
+
+The source code is available from [Github](https://github.com/duqtools/duqtools).
+
+Suggestions, improvements, and edits are most welcome.
+
+
+## Development
+
+Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
+
+
```

### Comparing `duqtools-1.6.4/README.md` & `duqtools-1.7.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
-
-# Duqtools
-
-*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
-
-Features:
-
-- Set up 100s of simulation runs from a single template
-- Launch standard sets of sensitivity tests with minimal programming
-- Batch job submission and status tracking
-- Supports the Standardized Interface Data Structures (IDSs) data directory
-- Compare and visualize 100s of simulations in one overview
-- Display simulation results as confidence ranges and distributions
-
-*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
-
-To install:
-
-```console
-pip install duqtools
-```
-
-The source code is available from [Github](https://github.com/duqtools/duqtools).
-
-Suggestions, improvements, and edits are most welcome.
-
-
-## Development
-
-Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
+| Source | Badges |
+| --- | --- |
+| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
+| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
+| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
+| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
+| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+
+# Duqtools
+
+*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
+
+Features:
+
+- Set up 100s of simulation runs from a single template
+- Launch standard sets of sensitivity tests with minimal programming
+- Batch job submission and status tracking
+- Supports the Standardized Interface Data Structures (IDSs) data directory
+- Compare and visualize 100s of simulations in one overview
+- Display simulation results as confidence ranges and distributions
+
+*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
+
+To install:
+
+```console
+pip install duqtools
+```
+
+The source code is available from [Github](https://github.com/duqtools/duqtools).
+
+Suggestions, improvements, and edits are most welcome.
+
+
+## Development
+
+Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
```

### Comparing `duqtools-1.6.4/setup.cfg` & `duqtools-1.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,145 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6175 7468  [metadata]..auth
-00000010: 6f72 203d 2053 7465 6620 536d 6565 7473  or = Stef Smeets
-00000020: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
-00000030: 2073 2e73 6d65 6574 7340 6573 6369 656e   s.smeets@escien
-00000040: 6365 6365 6e74 6572 2e6e 6c0d 0a63 6c61  cecenter.nl..cla
-00000050: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
-00000060: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000070: 203a 3a20 3320 2d20 416c 7068 610d 0a09   :: 3 - Alpha...
-00000080: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000090: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-000000a0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
-000000b0: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-000000c0: 6573 6561 7263 680d 0a09 4c69 6365 6e73  esearch...Licens
-000000d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-000000e0: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
-000000f0: 7761 7265 204c 6963 656e 7365 0d0a 094e  ware License...N
-00000100: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
-00000110: 3a3a 2045 6e67 6c69 7368 0d0a 094f 7065  :: English...Ope
-00000120: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000130: 2050 4f53 4958 203a 3a20 4c69 6e75 780d   POSIX :: Linux.
-00000140: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000150: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000160: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
-00000170: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000180: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-00000190: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001b0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
-000001c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001d0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-000001e0: 0a09 546f 7069 6320 3a3a 2053 6369 656e  ..Topic :: Scien
-000001f0: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
-00000200: 670d 0a64 6573 6372 6970 7469 6f6e 203d  g..description =
-00000210: 2044 796e 616d 6963 2075 6e63 6572 7461   Dynamic uncerta
-00000220: 696e 7479 2071 7561 6e74 6966 6963 6174  inty quantificat
-00000230: 696f 6e20 666f 7220 546f 6b61 6d61 6b20  ion for Tokamak 
-00000240: 7265 6163 746f 7220 7369 6d75 6c61 7469  reactor simulati
-00000250: 6f6e 7320 6d6f 6465 6c6c 696e 670d 0a6b  ons modelling..k
-00000260: 6579 776f 7264 7320 3d20 0d0a 096d 6f64  eywords = ...mod
-00000270: 656c 6c69 6e67 0d0a 0975 6e63 6572 7461  elling...uncerta
-00000280: 696e 7479 2d71 7561 6e74 6966 6963 6174  inty-quantificat
-00000290: 696f 6e0d 0a09 746f 6b61 6d61 6b0d 0a09  ion...tokamak...
-000002a0: 6675 7369 6f6e 2d72 6561 6374 6f72 0d0a  fusion-reactor..
-000002b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000002c0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000002d0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000002e0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000002f0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000300: 6e0d 0a6e 616d 6520 3d20 6475 7174 6f6f  n..name = duqtoo
-00000310: 6c73 0d0a 7072 6f6a 6563 745f 7572 6c73  ls..project_urls
-00000320: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-00000330: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000340: 7562 2e63 6f6d 2f64 7571 746f 6f6c 732f  ub.com/duqtools/
-00000350: 6475 7174 6f6f 6c73 2f69 7373 7565 730d  duqtools/issues.
-00000360: 0a09 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
-00000370: 3d20 6874 7470 733a 2f2f 6475 7174 6f6f  = https://duqtoo
-00000380: 6c73 2e72 6561 6474 6865 646f 6373 2e69  ls.readthedocs.i
-00000390: 6f0d 0a75 726c 203d 2068 7474 7073 3a2f  o..url = https:/
-000003a0: 2f67 6974 6875 622e 636f 6d2f 6475 7174  /github.com/duqt
-000003b0: 6f6f 6c73 2f64 7571 746f 6f6c 730d 0a76  ools/duqtools..v
-000003c0: 6572 7369 6f6e 203d 2031 2e36 2e34 0d0a  ersion = 1.6.4..
-000003d0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a 6970  ..[options]..zip
-000003e0: 5f73 6166 6520 3d20 4661 6c73 650d 0a70  _safe = False..p
-000003f0: 6163 6b61 6765 7320 3d20 6669 6e64 5f6e  ackages = find_n
-00000400: 616d 6573 7061 6365 3a0d 0a70 6163 6b61  amespace:..packa
-00000410: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000420: 630d 0a69 6e63 6c75 6465 5f70 6163 6b61  c..include_packa
-00000430: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
-00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000450: 203d 200d 0a09 616c 7461 6972 0d0a 0963   = ...altair...c
-00000460: 6c69 636b 0d0a 0967 6974 7079 7468 6f6e  lick...gitpython
-00000470: 0d0a 096a 696e 6a61 3220 3e3d 2033 2e30  ...jinja2 >= 3.0
-00000480: 0d0a 0969 6d70 6f72 746c 6962 5f72 6573  ...importlib_res
-00000490: 6f75 7263 6573 3b70 7974 686f 6e5f 7665  ources;python_ve
-000004a0: 7273 696f 6e3c 2733 2e31 3027 0d0a 096e  rsion<'3.10'...n
-000004b0: 756d 7079 0d0a 0970 616e 6461 730d 0a09  umpy...pandas...
-000004c0: 7079 6461 6e74 6963 2021 3d31 2e31 302e  pydantic !=1.10.
-000004d0: 332c 2021 3d31 2e31 302e 342c 2021 3d31  3, !=1.10.4, !=1
-000004e0: 2e31 302e 350d 0a09 7079 6461 6e74 6963  .10.5...pydantic
-000004f0: 2d79 616d 6c0d 0a09 7363 6970 7920 3e3d  -yaml...scipy >=
-00000500: 2031 2e30 390d 0a09 7471 646d 0d0a 0978   1.09...tqdm...x
-00000510: 6172 7261 790d 0a09 6a65 7474 6f2d 746f  array...jetto-to
-00000520: 6f6c 7320 3e3d 2031 2e38 2e38 0d0a 0973  ols >= 1.8.8...s
-00000530: 7472 6561 6d6c 6974 203d 3d20 312e 3131  treamlit == 1.11
-00000540: 3b70 7974 686f 6e5f 6675 6c6c 5f76 6572  ;python_full_ver
-00000550: 7369 6f6e 3d3d 2733 2e39 2e37 270d 0a09  sion=='3.9.7'...
-00000560: 7374 7265 616d 6c69 7420 3e3d 2031 2e31  streamlit >= 1.1
-00000570: 323b 7079 7468 6f6e 5f66 756c 6c5f 7665  2;python_full_ve
-00000580: 7273 696f 6e21 3d27 332e 392e 3727 0d0a  rsion!='3.9.7'..
-00000590: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
-000005a0: 735f 7265 7175 6972 655d 0d0a 6465 7665  s_require]..deve
-000005b0: 6c6f 7020 3d20 0d0a 0962 756d 7032 7665  lop = ...bump2ve
-000005c0: 7273 696f 6e0d 0a09 7275 6666 0d0a 0970  rsion...ruff...p
-000005d0: 7265 2d63 6f6d 6d69 740d 0a09 7961 7066  re-commit...yapf
-000005e0: 0d0a 096d 7970 790d 0a09 636f 7665 7261  ...mypy...covera
-000005f0: 6765 0d0a 096e 626d 616b 650d 0a09 7079  ge...nbmake...py
-00000600: 7465 7374 0d0a 0970 7974 6573 742d 6465  test...pytest-de
-00000610: 7065 6e64 656e 6379 0d0a 0970 7963 6f64  pendency...pycod
-00000620: 6573 7479 6c65 0d0a 646f 6373 203d 200d  estyle..docs = .
-00000630: 0a09 6d61 7470 6c6f 746c 6962 0d0a 096a  ..matplotlib...j
-00000640: 696e 6a61 320d 0a09 6d61 726b 646f 776e  inja2...markdown
-00000650: 2d69 6e63 6c75 6465 0d0a 096d 6b64 6f63  -include...mkdoc
-00000660: 730d 0a09 6d6b 646f 6373 2d63 6c69 636b  s...mkdocs-click
-00000670: 0d0a 096d 6b64 6f63 732d 6a75 7079 7465  ...mkdocs-jupyte
-00000680: 720d 0a09 6d6b 646f 6373 2d67 656e 2d66  r...mkdocs-gen-f
-00000690: 696c 6573 0d0a 096d 6b64 6f63 732d 6d61  iles...mkdocs-ma
-000006a0: 7465 7269 616c 0d0a 096d 6b64 6f63 7374  terial...mkdocst
-000006b0: 7269 6e67 735b 7079 7468 6f6e 5d0d 0a70  rings[python]..p
-000006c0: 7562 6c69 7368 696e 6720 3d20 0d0a 0974  ublishing = ...t
-000006d0: 7769 6e65 0d0a 0977 6865 656c 0d0a 0962  wine...wheel...b
-000006e0: 7569 6c64 0d0a 696d 6173 203d 200d 0a09  uild..imas = ...
-000006f0: 696d 6173 0d0a 0d0a 5b6f 7074 696f 6e73  imas....[options
-00000700: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000710: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000720: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-00000730: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-00000740: 7363 7269 7074 7320 3d20 0d0a 0964 7571  scripts = ...duq
-00000750: 746f 6f6c 7320 3d20 6475 7174 6f6f 6c73  tools = duqtools
-00000760: 2e63 6c69 3a63 6c69 5f65 6e74 7279 0d0a  .cli:cli_entry..
-00000770: 0964 7571 6475 7120 3d20 6475 7174 6f6f  .duqduq = duqtoo
-00000780: 6c73 2e6c 6172 6765 5f73 6361 6c65 5f76  ls.large_scale_v
-00000790: 616c 6964 6174 696f 6e2e 636c 693a 636c  alidation.cli:cl
-000007a0: 695f 656e 7472 790d 0a0d 0a5b 636f 7665  i_entry....[cove
-000007b0: 7261 6765 3a72 756e 5d0d 0a62 7261 6e63  rage:run]..branc
-000007c0: 6820 3d20 5472 7565 0d0a 736f 7572 6365  h = True..source
-000007d0: 203d 2064 7571 746f 6f6c 730d 0a63 6f6e   = duqtools..con
-000007e0: 6375 7272 656e 6379 203d 206d 756c 7469  currency = multi
-000007f0: 7072 6f63 6573 7369 6e67 0d0a 6461 7461  processing..data
-00000800: 5f66 696c 6520 3d20 2e63 6f76 6572 6167  _file = .coverag
-00000810: 650d 0a0d 0a5b 746f 6f6c 3a70 7974 6573  e....[tool:pytes
-00000820: 745d 0d0a 7465 7374 7061 7468 7320 3d20  t]..testpaths = 
-00000830: 7465 7374 730d 0a6e 6f72 6563 7572 7365  tests..norecurse
-00000840: 6469 7273 203d 2074 6573 7473 2f68 656c  dirs = tests/hel
-00000850: 7065 7273 0d0a 0d0a 5b6d 7970 795d 0d0a  pers....[mypy]..
-00000860: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
-00000870: 6d70 6f72 7473 203d 2054 7275 650d 0a66  mports = True..f
-00000880: 696c 6573 203d 2064 7571 746f 6f6c 732c  iles = duqtools,
-00000890: 2074 6573 7473 0d0a 616c 6c6f 775f 7265   tests..allow_re
-000008a0: 6465 6669 6e69 7469 6f6e 203d 2054 7275  definition = Tru
-000008b0: 650d 0a0d 0a5b 6d79 7079 2d79 616d 6c2e  e....[mypy-yaml.
-000008c0: 2a5d 0d0a 6967 6e6f 7265 5f6d 6973 7369  *]..ignore_missi
-000008d0: 6e67 5f69 6d70 6f72 7473 203d 2054 7275  ng_imports = Tru
-000008e0: 650d 0a0d 0a5b 6d79 7079 2d70 6b67 5f72  e....[mypy-pkg_r
-000008f0: 6573 6f75 7263 6573 2e2a 5d0d 0a69 676e  esources.*]..ign
-00000900: 6f72 655f 6d69 7373 696e 675f 696d 706f  ore_missing_impo
-00000910: 7274 7320 3d20 5472 7565 0d0a 0d0a 5b79  rts = True....[y
-00000920: 6170 665d 0d0a 626c 616e 6b5f 6c69 6e65  apf]..blank_line
-00000930: 5f62 6566 6f72 655f 6e65 7374 6564 5f63  _before_nested_c
-00000940: 6c61 7373 5f6f 725f 6465 6620 3d20 5472  lass_or_def = Tr
-00000950: 7565 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ue....[egg_info]
-00000960: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000970: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a61 7574 686f  [metadata].autho
+00000010: 7220 3d20 5374 6566 2053 6d65 6574 730a  r = Stef Smeets.
+00000020: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
+00000030: 2e73 6d65 6574 7340 6573 6369 656e 6365  .smeets@escience
+00000040: 6365 6e74 6572 2e6e 6c0a 636c 6173 7369  center.nl.classi
+00000050: 6669 6572 7320 3d20 0a09 4465 7665 6c6f  fiers = ..Develo
+00000060: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000070: 3320 2d20 416c 7068 610a 0949 6e74 656e  3 - Alpha..Inten
+00000080: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000090: 4465 7665 6c6f 7065 7273 0a09 496e 7465  Developers..Inte
+000000a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000000b0: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+000000c0: 680a 094c 6963 656e 7365 203a 3a20 4f53  h..License :: OS
+000000d0: 4920 4170 7072 6f76 6564 203a 3a20 4170  I Approved :: Ap
+000000e0: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
+000000f0: 6365 6e73 650a 094e 6174 7572 616c 204c  cense..Natural L
+00000100: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000110: 7368 0a09 4f70 6572 6174 696e 6720 5379  sh..Operating Sy
+00000120: 7374 656d 203a 3a20 504f 5349 5820 3a3a  stem :: POSIX ::
+00000130: 204c 696e 7578 0a09 5072 6f67 7261 6d6d   Linux..Programm
+00000140: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000150: 5079 7468 6f6e 203a 3a20 330a 0950 726f  Python :: 3..Pro
+00000160: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000170: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000180: 2e39 0a09 5072 6f67 7261 6d6d 696e 6720  .9..Programming 
+00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001a0: 6f6e 203a 3a20 332e 3130 0a09 5072 6f67  on :: 3.10..Prog
+000001b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001d0: 3131 0a09 546f 7069 6320 3a3a 2053 6369  11..Topic :: Sci
+000001e0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+000001f0: 696e 670a 6465 7363 7269 7074 696f 6e20  ing.description 
+00000200: 3d20 4479 6e61 6d69 6320 756e 6365 7274  = Dynamic uncert
+00000210: 6169 6e74 7920 7175 616e 7469 6669 6361  ainty quantifica
+00000220: 7469 6f6e 2066 6f72 2054 6f6b 616d 616b  tion for Tokamak
+00000230: 2072 6561 6374 6f72 2073 696d 756c 6174   reactor simulat
+00000240: 696f 6e73 206d 6f64 656c 6c69 6e67 0a6b  ions modelling.k
+00000250: 6579 776f 7264 7320 3d20 0a09 6d6f 6465  eywords = ..mode
+00000260: 6c6c 696e 670a 0975 6e63 6572 7461 696e  lling..uncertain
+00000270: 7479 2d71 7561 6e74 6966 6963 6174 696f  ty-quantificatio
+00000280: 6e0a 0974 6f6b 616d 616b 0a09 6675 7369  n..tokamak..fusi
+00000290: 6f6e 2d72 6561 6374 6f72 0a6c 6f6e 675f  on-reactor.long_
+000002a0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000002b0: 6c65 3a20 5245 4144 4d45 2e6d 640a 6c6f  le: README.md.lo
+000002c0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000002d0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+000002e0: 7874 2f6d 6172 6b64 6f77 6e0a 6e61 6d65  xt/markdown.name
+000002f0: 203d 2064 7571 746f 6f6c 730a 7072 6f6a   = duqtools.proj
+00000300: 6563 745f 7572 6c73 203d 200a 0942 7567  ect_urls = ..Bug
+00000310: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000320: 3a2f 2f67 6974 6875 622e 636f 6d2f 6475  ://github.com/du
+00000330: 7174 6f6f 6c73 2f64 7571 746f 6f6c 732f  qtools/duqtools/
+00000340: 6973 7375 6573 0a09 446f 6375 6d65 6e74  issues..Document
+00000350: 6174 696f 6e20 3d20 6874 7470 733a 2f2f  ation = https://
+00000360: 6475 7174 6f6f 6c73 2e72 6561 6474 6865  duqtools.readthe
+00000370: 646f 6373 2e69 6f0a 7572 6c20 3d20 6874  docs.io.url = ht
+00000380: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000390: 2f64 7571 746f 6f6c 732f 6475 7174 6f6f  /duqtools/duqtoo
+000003a0: 6c73 0a76 6572 7369 6f6e 203d 2031 2e37  ls.version = 1.7
+000003b0: 2e30 0a0a 5b6f 7074 696f 6e73 5d0a 7a69  .0..[options].zi
+000003c0: 705f 7361 6665 203d 2046 616c 7365 0a70  p_safe = False.p
+000003d0: 6163 6b61 6765 7320 3d20 6669 6e64 5f6e  ackages = find_n
+000003e0: 616d 6573 7061 6365 3a0a 7061 636b 6167  amespace:.packag
+000003f0: 655f 6469 7220 3d20 0a09 3d20 7372 630a  e_dir = ..= src.
+00000400: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000410: 6461 7461 203d 2054 7275 650a 696e 7374  data = True.inst
+00000420: 616c 6c5f 7265 7175 6972 6573 203d 200a  all_requires = .
+00000430: 0961 6c74 6169 720a 0963 6c69 636b 0a09  .altair..click..
+00000440: 6769 7470 7974 686f 6e0a 096a 696e 6a61  gitpython..jinja
+00000450: 3220 3e3d 2033 2e30 0a09 696d 706f 7274  2 >= 3.0..import
+00000460: 6c69 625f 7265 736f 7572 6365 733b 7079  lib_resources;py
+00000470: 7468 6f6e 5f76 6572 7369 6f6e 3c27 332e  thon_version<'3.
+00000480: 3130 270a 096e 756d 7079 0a09 7061 6e64  10'..numpy..pand
+00000490: 6173 0a09 7079 6461 6e74 6963 2021 3d31  as..pydantic !=1
+000004a0: 2e31 302e 332c 2021 3d31 2e31 302e 342c  .10.3, !=1.10.4,
+000004b0: 2021 3d31 2e31 302e 350a 0970 7964 616e   !=1.10.5..pydan
+000004c0: 7469 632d 7961 6d6c 0a09 7363 6970 7920  tic-yaml..scipy 
+000004d0: 3e3d 2031 2e30 390a 0974 7164 6d0a 0978  >= 1.09..tqdm..x
+000004e0: 6172 7261 790a 096a 6574 746f 2d74 6f6f  array..jetto-too
+000004f0: 6c73 203e 3d20 312e 382e 380a 0973 7472  ls >= 1.8.8..str
+00000500: 6561 6d6c 6974 203d 3d20 312e 3131 3b70  eamlit == 1.11;p
+00000510: 7974 686f 6e5f 6675 6c6c 5f76 6572 7369  ython_full_versi
+00000520: 6f6e 3d3d 2733 2e39 2e37 270a 0973 7472  on=='3.9.7'..str
+00000530: 6561 6d6c 6974 203e 3d20 312e 3132 3b70  eamlit >= 1.12;p
+00000540: 7974 686f 6e5f 6675 6c6c 5f76 6572 7369  ython_full_versi
+00000550: 6f6e 213d 2733 2e39 2e37 270a 0a5b 6f70  on!='3.9.7'..[op
+00000560: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+00000570: 7569 7265 5d0a 6465 7665 6c6f 7020 3d20  uire].develop = 
+00000580: 0a09 6275 6d70 3276 6572 7369 6f6e 0a09  ..bump2version..
+00000590: 7275 6666 0a09 7072 652d 636f 6d6d 6974  ruff..pre-commit
+000005a0: 0a09 7961 7066 0a09 6d79 7079 0a09 636f  ..yapf..mypy..co
+000005b0: 7665 7261 6765 0a09 6e62 6d61 6b65 0a09  verage..nbmake..
+000005c0: 7079 7465 7374 0a09 7079 7465 7374 2d64  pytest..pytest-d
+000005d0: 6570 656e 6465 6e63 790a 0970 7963 6f64  ependency..pycod
+000005e0: 6573 7479 6c65 0a64 6f63 7320 3d20 0a09  estyle.docs = ..
+000005f0: 6d61 7470 6c6f 746c 6962 0a09 6a69 6e6a  matplotlib..jinj
+00000600: 6132 0a09 6d61 726b 646f 776e 2d69 6e63  a2..markdown-inc
+00000610: 6c75 6465 0a09 6d6b 646f 6373 0a09 6d6b  lude..mkdocs..mk
+00000620: 646f 6373 2d63 6c69 636b 0a09 6d6b 646f  docs-click..mkdo
+00000630: 6373 2d6a 7570 7974 6572 0a09 6d6b 646f  cs-jupyter..mkdo
+00000640: 6373 2d67 656e 2d66 696c 6573 0a09 6d6b  cs-gen-files..mk
+00000650: 646f 6373 2d6d 6174 6572 6961 6c0a 096d  docs-material..m
+00000660: 6b64 6f63 7374 7269 6e67 735b 7079 7468  kdocstrings[pyth
+00000670: 6f6e 5d0a 7075 626c 6973 6869 6e67 203d  on].publishing =
+00000680: 200a 0974 7769 6e65 0a09 7768 6565 6c0a   ..twine..wheel.
+00000690: 0962 7569 6c64 0a69 6d61 7320 3d20 0a09  .build.imas = ..
+000006a0: 696d 6173 0a0a 5b6f 7074 696f 6e73 2e70  imas..[options.p
+000006b0: 6163 6b61 6765 732e 6669 6e64 5d0a 7768  ackages.find].wh
+000006c0: 6572 6520 3d20 7372 630a 0a5b 6f70 7469  ere = src..[opti
+000006d0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000006e0: 5d0a 636f 6e73 6f6c 655f 7363 7269 7074  ].console_script
+000006f0: 7320 3d20 0a09 6475 7174 6f6f 6c73 203d  s = ..duqtools =
+00000700: 2064 7571 746f 6f6c 732e 636c 693a 636c   duqtools.cli:cl
+00000710: 695f 656e 7472 790a 0964 7571 6475 7120  i_entry..duqduq 
+00000720: 3d20 6475 7174 6f6f 6c73 2e6c 6172 6765  = duqtools.large
+00000730: 5f73 6361 6c65 5f76 616c 6964 6174 696f  _scale_validatio
+00000740: 6e2e 636c 693a 636c 695f 656e 7472 790a  n.cli:cli_entry.
+00000750: 0a5b 636f 7665 7261 6765 3a72 756e 5d0a  .[coverage:run].
+00000760: 6272 616e 6368 203d 2054 7275 650a 736f  branch = True.so
+00000770: 7572 6365 203d 2064 7571 746f 6f6c 730a  urce = duqtools.
+00000780: 636f 6e63 7572 7265 6e63 7920 3d20 6d75  concurrency = mu
+00000790: 6c74 6970 726f 6365 7373 696e 670a 6461  ltiprocessing.da
+000007a0: 7461 5f66 696c 6520 3d20 2e63 6f76 6572  ta_file = .cover
+000007b0: 6167 650a 0a5b 746f 6f6c 3a70 7974 6573  age..[tool:pytes
+000007c0: 745d 0a74 6573 7470 6174 6873 203d 2074  t].testpaths = t
+000007d0: 6573 7473 0a6e 6f72 6563 7572 7365 6469  ests.norecursedi
+000007e0: 7273 203d 2074 6573 7473 2f68 656c 7065  rs = tests/helpe
+000007f0: 7273 0a0a 5b6d 7970 795d 0a69 676e 6f72  rs..[mypy].ignor
+00000800: 655f 6d69 7373 696e 675f 696d 706f 7274  e_missing_import
+00000810: 7320 3d20 5472 7565 0a66 696c 6573 203d  s = True.files =
+00000820: 2064 7571 746f 6f6c 732c 2074 6573 7473   duqtools, tests
+00000830: 0a61 6c6c 6f77 5f72 6564 6566 696e 6974  .allow_redefinit
+00000840: 696f 6e20 3d20 5472 7565 0a0a 5b6d 7970  ion = True..[myp
+00000850: 792d 7961 6d6c 2e2a 5d0a 6967 6e6f 7265  y-yaml.*].ignore
+00000860: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
+00000870: 203d 2054 7275 650a 0a5b 6d79 7079 2d70   = True..[mypy-p
+00000880: 6b67 5f72 6573 6f75 7263 6573 2e2a 5d0a  kg_resources.*].
+00000890: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
+000008a0: 6d70 6f72 7473 203d 2054 7275 650a 0a5b  mports = True..[
+000008b0: 7961 7066 5d0a 626c 616e 6b5f 6c69 6e65  yapf].blank_line
+000008c0: 5f62 6566 6f72 655f 6e65 7374 6564 5f63  _before_nested_c
+000008d0: 6c61 7373 5f6f 725f 6465 6620 3d20 5472  lass_or_def = Tr
+000008e0: 7565 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  ue..[egg_info].t
+000008f0: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
+00000900: 6461 7465 203d 2030 0a0a                 date = 0..
```

### Comparing `duqtools-1.6.4/src/duqtools/__init__.py` & `duqtools-1.7.0/src/duqtools/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# https://setuptools.pypa.io/en/latest/pkg_resources.html#workingset-objects
-def fix_dependencies():
-    import __main__
-    __main__.__requires__ = [
-        'jetto_tools>=1.8.8',
-        'pydantic!=1.10.3',
-        'pydantic!=1.10.4',
-        'pydantic!=1.10.5',
-        'scipy>=1.09',
-        'jinja2>=3.0.0',
-    ]
-    import pkg_resources  # noqa
-
-
-fix_dependencies()
-
-__author__ = 'Stef Smeets'
-__email__ = 's.smeets@esciencecenter.nl'
-__version__ = '1.6.4'
-
-import logging  # noqa
-import warnings  # noqa
-
-logging.basicConfig(level=logging.INFO)
-
-# https://github.com/duqtools/duqtools/issues/264
-warnings.filterwarnings(
-    'ignore',
-    'Explicit custom root behavior not yet implemented for pydantic_yaml')
+# https://setuptools.pypa.io/en/latest/pkg_resources.html#workingset-objects
+def fix_dependencies():
+    import __main__
+    __main__.__requires__ = [
+        'jetto_tools>=1.8.8',
+        'pydantic!=1.10.3',
+        'pydantic!=1.10.4',
+        'pydantic!=1.10.5',
+        'scipy>=1.09',
+        'jinja2>=3.0.0',
+    ]
+    import pkg_resources  # noqa
+
+
+fix_dependencies()
+
+__author__ = 'Stef Smeets'
+__email__ = 's.smeets@esciencecenter.nl'
+__version__ = '1.7.0'
+
+import logging  # noqa
+import warnings  # noqa
+
+logging.basicConfig(level=logging.INFO)
+
+# https://github.com/duqtools/duqtools/issues/264
+warnings.filterwarnings(
+    'ignore',
+    'Explicit custom root behavior not yet implemented for pydantic_yaml')
```

### Comparing `duqtools-1.6.4/src/duqtools/_click_opt_groups.py` & `duqtools-1.7.0/src/duqtools/_click_opt_groups.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""Module with click subclasses to group options in `--help`output.
-
-Example:
-
-    python _click_opt_groups.py --help
-
-Implementation based on:
-https://github.com/pallets/click/issues/373#issuecomment-515293746
-"""
-
-from collections import defaultdict
-
-import click
-
-
-class GroupOpt(click.Option):
-
-    def __init__(self, *args, **kwargs):
-        self.group = kwargs.pop('group', None)
-        super().__init__(*args, **kwargs)
-
-
-class GroupCmd(click.Command):
-
-    def format_options(self, ctx, formatter):
-        """Writes all the options into the formatter if they exist.
-
-        Implementation based on:
-            https://github.com/pallets/click/issues/373#issuecomment-515293746
-        """
-        sections = defaultdict(list)
-
-        for param in self.get_params(ctx):
-            option = param.get_help_record(ctx)
-            if option:
-                try:
-                    title = str(param.group)
-                except AttributeError:
-                    title = 'Options'
-
-                sections[title].append(option)
-
-        for title, options in sections.items():
-            with formatter.section(title):
-                formatter.write_dl(options)
-
-
-if __name__ == '__main__':
-
-    @click.group()
-    def cli():
-        pass
-
-    @cli.command(cls=GroupCmd)
-    @click.option('-a')
-    @click.option('-b', cls=GroupOpt, group='Group 1')
-    @click.option('-c', cls=GroupOpt, group='Group 1')
-    @click.option('-d', cls=GroupOpt, group='Group 2')
-    @click.option('-e', cls=GroupOpt, group='Group 2')
-    def main(**kwargs):
-        print(kwargs)
-
-    main()
+"""Module with click subclasses to group options in `--help`output.
+
+Example:
+
+    python _click_opt_groups.py --help
+
+Implementation based on:
+https://github.com/pallets/click/issues/373#issuecomment-515293746
+"""
+
+from collections import defaultdict
+
+import click
+
+
+class GroupOpt(click.Option):
+
+    def __init__(self, *args, **kwargs):
+        self.group = kwargs.pop('group', None)
+        super().__init__(*args, **kwargs)
+
+
+class GroupCmd(click.Command):
+
+    def format_options(self, ctx, formatter):
+        """Writes all the options into the formatter if they exist.
+
+        Implementation based on:
+            https://github.com/pallets/click/issues/373#issuecomment-515293746
+        """
+        sections = defaultdict(list)
+
+        for param in self.get_params(ctx):
+            option = param.get_help_record(ctx)
+            if option:
+                try:
+                    title = str(param.group)
+                except AttributeError:
+                    title = 'Options'
+
+                sections[title].append(option)
+
+        for title, options in sections.items():
+            with formatter.section(title):
+                formatter.write_dl(options)
+
+
+if __name__ == '__main__':
+
+    @click.group()
+    def cli():
+        pass
+
+    @cli.command(cls=GroupCmd)
+    @click.option('-a')
+    @click.option('-b', cls=GroupOpt, group='Group 1')
+    @click.option('-c', cls=GroupOpt, group='Group 1')
+    @click.option('-d', cls=GroupOpt, group='Group 2')
+    @click.option('-e', cls=GroupOpt, group='Group 2')
+    def main(**kwargs):
+        print(kwargs)
+
+    main()
```

### Comparing `duqtools-1.6.4/src/duqtools/_logging_utils.py` & `duqtools-1.7.0/src/duqtools/_logging_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import logging
-
-import click
-
-
-class TermEscapeCodeFormatter(logging.Formatter):
-    """A class to strip the escape codes from the."""
-
-    def format(self, record):
-        record.msg = click.unstyle(record.msg)
-        return super().format(record)
-
-
-class LoggingContext:
-    """Context manager to Temporarily change logging configuration.
-
-    From https://docs.python.org/3/howto/logging-cookbook.html
-
-    Parameters
-    ----------
-    logger : None, optional
-        Logging instance to change, defaults to root logger.
-    level : None, optional
-        New log level, i.e. `logging.CRITICAL`.
-    handler : None, optional
-        Log handler to use.
-    close : bool, optional
-        Whether to close the handler after use.
-    """
-
-    def __init__(self, logger=None, level=None, handler=None, close=True):
-        if not logger:
-            logger = logging.getLogger()
-        self.logger = logger
-        self.level = level
-        self.handler = handler
-        self.close = close
-
-    def __enter__(self):
-        if self.level is not None:
-            self.old_level = self.logger.level
-            self.logger.setLevel(self.level)
-        if self.handler:
-            self.logger.addHandler(self.handler)
-
-    def __exit__(self, et, ev, tb):
-        if self.level is not None:
-            self.logger.setLevel(self.old_level)
-        if self.handler:
-            self.logger.removeHandler(self.handler)
-        if self.handler and self.close:
-            self.handler.close()
-
-
-# Logger to use in duqtools
-duqlog_screen = logging.getLogger(
-    'screen')  # logger to log to the screen (and the log)
-
-
-def initialize_duqlog_screen():
-    # Logger for stdout
-    stream = logging.StreamHandler()
-    stream.setFormatter(logging.Formatter('%(message)s'))
-    duqlog_screen.addHandler(stream)
-
-
-initialize_duqlog_screen()
+import logging
+
+import click
+
+
+class TermEscapeCodeFormatter(logging.Formatter):
+    """A class to strip the escape codes from the."""
+
+    def format(self, record):
+        record.msg = click.unstyle(record.msg)
+        return super().format(record)
+
+
+class LoggingContext:
+    """Context manager to Temporarily change logging configuration.
+
+    From https://docs.python.org/3/howto/logging-cookbook.html
+
+    Parameters
+    ----------
+    logger : None, optional
+        Logging instance to change, defaults to root logger.
+    level : None, optional
+        New log level, i.e. `logging.CRITICAL`.
+    handler : None, optional
+        Log handler to use.
+    close : bool, optional
+        Whether to close the handler after use.
+    """
+
+    def __init__(self, logger=None, level=None, handler=None, close=True):
+        if not logger:
+            logger = logging.getLogger()
+        self.logger = logger
+        self.level = level
+        self.handler = handler
+        self.close = close
+
+    def __enter__(self):
+        if self.level is not None:
+            self.old_level = self.logger.level
+            self.logger.setLevel(self.level)
+        if self.handler:
+            self.logger.addHandler(self.handler)
+
+    def __exit__(self, et, ev, tb):
+        if self.level is not None:
+            self.logger.setLevel(self.old_level)
+        if self.handler:
+            self.logger.removeHandler(self.handler)
+        if self.handler and self.close:
+            self.handler.close()
+
+
+# Logger to use in duqtools
+duqlog_screen = logging.getLogger(
+    'screen')  # logger to log to the screen (and the log)
+
+
+def initialize_duqlog_screen():
+    # Logger for stdout
+    stream = logging.StreamHandler()
+    stream.setFormatter(logging.Formatter('%(message)s'))
+    duqlog_screen.addHandler(stream)
+
+
+initialize_duqlog_screen()
```

### Comparing `duqtools-1.6.4/src/duqtools/api.py` & `duqtools-1.7.0/src/duqtools/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-"""All public packages, functions and classes are available in this module.
-
-Functions:
-
-- [rebase_on_grid][duqtools.api.rebase_on_grid]
-- [rebase_on_time][duqtools.api.rebase_on_time]
-- [standardize_grid_and_time][duqtools.api.standardize_grid_and_time]
-
-Data classes:
-
-- [ImasHandle][duqtools.api.ImasHandle]
-- [IDSMapping][duqtools.api.IDSMapping]
-- [Variable][duqtools.api.Variable]
-
-Plotting:
-
-- [alt_errorband_chart][duqtools.api.alt_errorband_chart]
-- [alt_line_chart][duqtools.api.alt_line_chart]
-"""
-
-from ._plot_utils import alt_errorband_chart, alt_line_chart
-from .ids import (
-    IDSMapping,
-    ImasHandle,
-    rebase_on_grid,
-    rebase_on_time,
-    standardize_grid_and_time,
-)
-from .schema import IDSVariableModel as Variable
-
-__all__ = [
-    'rebase_on_grid',
-    'rebase_on_time',
-    'standardize_grid_and_time',
-    'ImasHandle',
-    'IDSMapping',
-    'Variable',
-    'alt_line_chart',
-    'alt_errorband_chart',
-]
+"""All public packages, functions and classes are available in this module.
+
+Functions:
+
+- [rebase_on_grid][duqtools.api.rebase_on_grid]
+- [rebase_on_time][duqtools.api.rebase_on_time]
+- [standardize_grid_and_time][duqtools.api.standardize_grid_and_time]
+
+Data classes:
+
+- [ImasHandle][duqtools.api.ImasHandle]
+- [IDSMapping][duqtools.api.IDSMapping]
+- [Variable][duqtools.api.Variable]
+
+Plotting:
+
+- [alt_errorband_chart][duqtools.api.alt_errorband_chart]
+- [alt_line_chart][duqtools.api.alt_line_chart]
+"""
+
+from ._plot_utils import alt_errorband_chart, alt_line_chart
+from .duqmap import duqmap
+from .ids import (
+    IDSMapping,
+    ImasHandle,
+    rebase_all_coords,
+    rebase_on_grid,
+    rebase_on_time,
+    standardize_grid_and_time,
+)
+from .models import Run, Runs
+from .schema import IDSVariableModel as Variable
+
+__all__ = [
+    'duqmap',
+    'rebase_on_grid',
+    'rebase_on_time',
+    'rebase_all_coords',
+    'standardize_grid_and_time',
+    'ImasHandle',
+    'IDSMapping',
+    'Variable',
+    'alt_line_chart',
+    'alt_errorband_chart',
+    'Run',
+    'Runs',
+]
```

### Comparing `duqtools-1.6.4/src/duqtools/apply_model.py` & `duqtools-1.7.0/src/duqtools/apply_model.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from __future__ import annotations
-
-from collections import abc
-from functools import singledispatch
-from pathlib import Path
-
-from .schema import BaseModel, JettoOperation
-
-
-@singledispatch
-def apply_model(model: BaseModel, **kwargs):
-    """Apply operation in model to target. Data are modified in-place.
-
-    Parameters
-    ----------
-    model
-        The model describes the operation to apply to the data.
-
-    Raises
-    ------
-    NotImplementedError
-        When the model is unknown
-    """
-    raise NotImplementedError(f'Unknown model: {model}')
-
-
-@apply_model.register
-def _apply_coupled(model: abc.Iterable, **kwargs):  # type: ignore
-    for submodel in model:
-        apply_model(submodel, **kwargs)
-
-
-from .ids._apply_model import _apply_ids  # noqa: E402, F401
-
-
-@apply_model.register
-def _apply_jetto(model: JettoOperation, run_dir: Path, **kwargs):
-    from .system import get_system
-    system = get_system()
-    system.set_jetto_variable(run_dir, model.variable.name, model.value,
-                              model.variable.lookup)
+from __future__ import annotations
+
+from collections import abc
+from functools import singledispatch
+from pathlib import Path
+
+from .schema import BaseModel, JettoOperation
+
+
+@singledispatch
+def apply_model(model: BaseModel, **kwargs):
+    """Apply operation in model to target. Data are modified in-place.
+
+    Parameters
+    ----------
+    model
+        The model describes the operation to apply to the data.
+
+    Raises
+    ------
+    NotImplementedError
+        When the model is unknown
+    """
+    raise NotImplementedError(f'Unknown model: {model}')
+
+
+@apply_model.register
+def _apply_coupled(model: abc.Iterable, **kwargs):  # type: ignore
+    for submodel in model:
+        apply_model(submodel, **kwargs)
+
+
+from .ids._apply_model import _apply_ids  # noqa: E402, F401
+
+
+@apply_model.register
+def _apply_jetto(model: JettoOperation, run_dir: Path, **kwargs):
+    from .system import get_system
+    system = get_system()
+    system.set_jetto_variable(run_dir, model.variable.name, model.value,
+                              model.variable.lookup)
```

### Comparing `duqtools-1.6.4/src/duqtools/cleanup.py` & `duqtools-1.7.0/src/duqtools/cleanup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,81 @@
-from __future__ import annotations
-
-import logging
-import os
-import shutil
-from pathlib import Path
-
-from .ids import ImasHandle
-from .models import Locations
-from .operations import op_queue
-from .schema.runs import Run
-
-logger = logging.getLogger(__name__)
-
-
-def remove_files(*filenames: str):
-    for filename in filenames:
-        try:
-            os.unlink(filename)
-        except FileNotFoundError:
-            pass
-
-
-def remove_run(model: Run):
-    """Remove run directory if it exists."""
-    if Path(model.dirname).exists():
-        op_queue.add(
-            action=shutil.rmtree,
-            args=(model.dirname, ),
-            description='Removing run dir',
-            extra_description=f'{model.dirname}',
-        )
-
-
-def cleanup(out, force, **kwargs):
-    """Read runs.yaml and clean the current directory.
-
-    Parameters
-    ----------
-    out : bool
-        Remove output IDS.
-    """
-    try:
-        runs = Locations().runs
-    except OSError:
-        runs = ()
-    else:
-        if Locations().runs_yaml.exists() and not force:
-            if Locations().runs_yaml_old.exists():
-                raise OSError(
-                    '`runs.yaml.old` exists, use --force to overwrite anyway')
-
-    for run in runs:
-        data_in = ImasHandle.parse_obj(run.data_in)
-        data_out = ImasHandle.parse_obj(run.data_out)
-
-        data_in.delete()
-
-        if out:
-            data_out.delete()
-        else:
-            op_queue.add_no_op(description='NOT Removing',
-                               extra_description=f'{data_out}')
-
-        remove_run(run)
-
-    op_queue.add(
-        action=shutil.move,
-        args=(Locations().runs_yaml, Locations().runs_yaml_old),
-        description='Moving runs.yaml',
-        extra_description=f'{Locations().runs_yaml_old}',
-    )
-
-    op_queue.add(
-        action=remove_files,
-        args=(
-            'duqtools_slurm_array.err',
-            'duqtools_slurm_array.out',
-            'duqtools_slurm_array.sh',
-        ),
-        description='Removing other files',
-    )
+from __future__ import annotations
+
+import logging
+import os
+import shutil
+from pathlib import Path
+
+from .ids import ImasHandle
+from .models import Locations, Run
+from .operations import op_queue
+
+logger = logging.getLogger(__name__)
+
+
+def remove_files(*filenames: str):
+    for filename in filenames:
+        try:
+            os.unlink(filename)
+        except FileNotFoundError:
+            pass
+
+
+def remove_run(model: Run):
+    """Remove run directory if it exists."""
+    if Path(model.dirname).exists():
+        op_queue.add(
+            action=shutil.rmtree,
+            args=(model.dirname, ),
+            description='Removing run dir',
+            extra_description=f'{model.dirname}',
+        )
+
+
+def cleanup(out, force, **kwargs):
+    """Read runs.yaml and clean the current directory.
+
+    Parameters
+    ----------
+    out : bool
+        Remove output IDS.
+    """
+    try:
+        runs = Locations().runs
+    except OSError:
+        runs = ()
+    else:
+        if Locations().runs_yaml.exists() and not force:
+            if Locations().runs_yaml_old.exists():
+                raise OSError(
+                    '`runs.yaml.old` exists, use --force to overwrite anyway')
+
+    for run in runs:
+        data_in = ImasHandle.parse_obj(run.data_in)
+        data_out = ImasHandle.parse_obj(run.data_out)
+
+        data_in.delete()
+
+        if out:
+            data_out.delete()
+        else:
+            op_queue.add_no_op(description='NOT Removing',
+                               extra_description=f'{data_out}')
+
+        remove_run(run)
+
+    op_queue.add(
+        action=shutil.move,
+        args=(Locations().runs_yaml, Locations().runs_yaml_old),
+        description='Moving runs.yaml',
+        extra_description=f'{Locations().runs_yaml_old}',
+    )
+
+    op_queue.add(
+        action=remove_files,
+        args=(
+            'duqtools_slurm_array.err',
+            'duqtools_slurm_array.out',
+            'duqtools_slurm_array.sh',
+        ),
+        description='Removing other files',
+    )
```

### Comparing `duqtools-1.6.4/src/duqtools/config/_config.py` & `duqtools-1.7.0/src/duqtools/config/_config.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from __future__ import annotations
-
-from ..schema.cli import ConfigModel
-
-
-class Config(ConfigModel):
-    """Config class containing all configs, can be used with:
-
-        from duqtools.config import cfg
-        cfg.<variable you want>
-
-    To update the config:
-
-        cfg.parse_file('duqtools.yaml')
-    """
-    _instance = None
-
-    def __new__(cls, *args, **kwargs):
-        # Make it a singleton
-        if not Config._instance:
-            Config._instance = object.__new__(cls)
-        return Config._instance
-
-    def parse_file(self, *args, **kwargs):
-        """Add extra variables to variable lookup table."""
-        super().parse_file(*args, **kwargs)
-        from ._variables import var_lookup
-        if self.extra_variables:
-            var_lookup.update(self.extra_variables.to_variable_dict())
-
-
-cfg = Config.construct()
+from __future__ import annotations
+
+from ..schema.cli import ConfigModel
+
+
+class Config(ConfigModel):
+    """Config class containing all configs, can be used with:
+
+        from duqtools.config import cfg
+        cfg.<variable you want>
+
+    To update the config:
+
+        cfg.parse_file('duqtools.yaml')
+    """
+    _instance = None
+
+    def __new__(cls, *args, **kwargs):
+        # Make it a singleton
+        if not Config._instance:
+            Config._instance = object.__new__(cls)
+        return Config._instance
+
+    def parse_file(self, *args, **kwargs):
+        """Add extra variables to variable lookup table."""
+        super().parse_file(*args, **kwargs)
+        from ._variables import var_lookup
+        if self.extra_variables:
+            var_lookup.update(self.extra_variables.to_variable_dict())
+
+
+cfg = Config.construct()
```

### Comparing `duqtools-1.6.4/src/duqtools/config/_variables.py` & `duqtools-1.7.0/src/duqtools/config/_variables.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from __future__ import annotations
-
-import logging
-import operator
-import os
-import sys
-from collections import UserDict
-from pathlib import Path, PosixPath
-from typing import Hashable, Sequence
-
-from ..schema import IDSVariableModel
-from ..schema.variables import VariableConfigModel
-from ..utils import groupby
-
-if sys.version_info < (3, 10):
-    from importlib_resources import files
-else:
-    from importlib.resources import files
-
-logger = logging.getLogger(__name__)
-
-VAR_ENV = 'DUQTOOLS_VARDEF'
-USER_CONFIG_HOME = Path.home() / '.config'
-LOCAL_DIR = Path('.').absolute()
-DUQTOOLS_DIR = 'duqtools'
-VAR_FILENAME = 'variables.yaml'
-VAR_FILENAME_GLOB = 'variables*.yaml'
-ERROR_SUFFIX = '_error_upper'
-
-
-class VarLookup(UserDict):
-    _prefix = '$'
-    """Variable lookup table.
-
-    Subclasses `UserDict` to embed some commonly used operations, like
-    grouping and filtering.
-    """
-    _ids_variable_key = 'IDS-variable'
-
-    def __getitem__(self, key: str) -> IDSVariableModel:
-        return self.data[self.normalize(key)]
-
-    def error_upper(self, key: str) -> IDSVariableModel:
-        """Return error variable for given key.
-
-        i.e. `t_i_ave` -> `t_i_ave_error_upper`
-        """
-        var = self[key.removesuffix(ERROR_SUFFIX)].copy()
-        var.name += ERROR_SUFFIX
-        var.path += ERROR_SUFFIX
-        return var
-
-    def normalize(self, *keys: str) -> str | tuple[str, ...]:
-        """Normalize variable names (remove `$`)."""
-        keys = tuple(key.lstrip(self._prefix) for key in keys)
-        if len(keys) == 1:
-            return keys[0]
-        return keys
-
-    def filter_type(self, type: str, *, invert: bool = False) -> VarLookup:
-        """Filter all entries of given type."""
-        cmp = operator.ne if invert else operator.eq
-        return VarLookup({k: v for k, v in self.items() if cmp(v.type, type)})
-
-    def groupby_type(self) -> dict[Hashable, list[IDSVariableModel]]:
-        """Group entries by type."""
-        grouped_ids_vars = groupby(self.values(), keyfunc=lambda var: var.type)
-        return grouped_ids_vars
-
-    def filter_ids(self, ids: str) -> VarLookup:
-        """Filter all entries of given IDS."""
-        ids_vars = self.filter_type(self._ids_variable_key)
-
-        return VarLookup({k: v for k, v in ids_vars.items() if v.ids == ids})
-
-    def groupby_ids(self) -> dict[Hashable, list[IDSVariableModel]]:
-        """Group entries by IDS."""
-        ids_vars = self.filter_type(self._ids_variable_key).values()
-
-        grouped_ids_vars = groupby(ids_vars, keyfunc=lambda var: var.ids)
-        return grouped_ids_vars
-
-
-class VariableConfigLoader:
-
-    def __init__(self):
-        self.paths = self.get_config_path()
-
-    def load(self) -> VarLookup:
-        """Load the variables config."""
-        var_lookup = VarLookup()
-
-        for path in self.paths:
-            logger.debug(f'Loading variables from: {path}')
-
-            var_config = VariableConfigModel.parse_file(path)
-            var_lookup.update(var_config.to_variable_dict())
-
-        return var_lookup
-
-    def get_config_path(self) -> tuple[Path, ...]:
-        """Try to get the config file with variable definitions.
-
-        Search order:
-        1. environment variable
-        (2. local directory, not sure if this should be implemented)
-        3. config home (first $XDG_CONFIG_HOME/duqtools then `$HOME/.config/duqtools`)
-        4. fall back to variable definitions in package
-        """
-        for paths in (
-                self._get_paths_from_environment_variable(),
-                self._get_paths_from_config_home(),
-                self._get_paths_local_directory(),
-        ):
-            if paths:
-                return paths
-
-        return self._get_paths_fallback()
-
-    def _get_paths_from_environment_variable(self) -> tuple[Path, ...] | None:
-        env = os.environ.get(VAR_ENV)
-        if env:
-            path = Path(env)
-            drc = path.parent
-
-            if not drc.exists():
-                raise OSError(f'{path} defined by ${VAR_ENV} does not exist!')
-
-            return tuple(drc.glob(path.name))
-
-        return None
-
-    def _get_paths_local_directory(self) -> tuple[Path, ...] | None:
-        return None  # Not implemented
-
-    def _get_paths_from_config_home(self) -> tuple[Path, ...] | None:
-        config_home = os.environ.get('XDG_CONFIG_HOME', USER_CONFIG_HOME)
-
-        drc = Path(config_home) / DUQTOOLS_DIR
-        if drc.exists():
-            return tuple(drc.glob(VAR_FILENAME_GLOB))
-
-        return None
-
-    def _get_paths_fallback(self) -> tuple[Path, ...]:
-        module = files('duqtools.data')
-        assert module.is_dir()
-        drc: PosixPath = module._paths[0]  # type: ignore
-        return tuple(drc.glob(VAR_FILENAME_GLOB))
-
-
-def lookup_vars(
-        variables: Sequence[(str | IDSVariableModel)]
-) -> list[IDSVariableModel]:
-    """Helper function to look up a bunch of variables.
-
-    If str, look up the variable from the `var_lookup`. Else, check if
-    the variable is an `IDSVariableModel`.
-    """
-    var_models = []
-    for var in variables:
-        if isinstance(var, str):
-            if var.endswith(ERROR_SUFFIX):
-                var = var_lookup.error_upper(var)
-            else:
-                var = var_lookup[var]
-        if not isinstance(var, IDSVariableModel):
-            raise ValueError(f'Cannot lookup variable with type {type(var)}')
-        var_models.append(var)
-    return var_models
-
-
-var_lookup = VariableConfigLoader().load()
+from __future__ import annotations
+
+import logging
+import operator
+import os
+import sys
+from collections import UserDict
+from pathlib import Path, PosixPath
+from typing import Hashable, Sequence
+
+from ..schema import IDSVariableModel
+from ..schema.variables import VariableConfigModel
+from ..utils import groupby
+
+if sys.version_info < (3, 10):
+    from importlib_resources import files
+else:
+    from importlib.resources import files
+
+logger = logging.getLogger(__name__)
+
+VAR_ENV = 'DUQTOOLS_VARDEF'
+USER_CONFIG_HOME = Path.home() / '.config'
+LOCAL_DIR = Path('.').absolute()
+DUQTOOLS_DIR = 'duqtools'
+VAR_FILENAME = 'variables.yaml'
+VAR_FILENAME_GLOB = 'variables*.yaml'
+ERROR_SUFFIX = '_error_upper'
+
+
+class VarLookup(UserDict):
+    _prefix = '$'
+    """Variable lookup table.
+
+    Subclasses `UserDict` to embed some commonly used operations, like
+    grouping and filtering.
+    """
+    _ids_variable_key = 'IDS-variable'
+
+    def __getitem__(self, key: str) -> IDSVariableModel:
+        return self.data[self.normalize(key)]
+
+    def error_upper(self, key: str) -> IDSVariableModel:
+        """Return error variable for given key.
+
+        i.e. `t_i_ave` -> `t_i_ave_error_upper`
+        """
+        var = self[key.removesuffix(ERROR_SUFFIX)].copy()
+        var.name += ERROR_SUFFIX
+        var.path += ERROR_SUFFIX
+        return var
+
+    def normalize(self, *keys: str) -> str | tuple[str, ...]:
+        """Normalize variable names (remove `$`)."""
+        keys = tuple(key.lstrip(self._prefix) for key in keys)
+        if len(keys) == 1:
+            return keys[0]
+        return keys
+
+    def filter_type(self, type: str, *, invert: bool = False) -> VarLookup:
+        """Filter all entries of given type."""
+        cmp = operator.ne if invert else operator.eq
+        return VarLookup({k: v for k, v in self.items() if cmp(v.type, type)})
+
+    def groupby_type(self) -> dict[Hashable, list[IDSVariableModel]]:
+        """Group entries by type."""
+        grouped_ids_vars = groupby(self.values(), keyfunc=lambda var: var.type)
+        return grouped_ids_vars
+
+    def filter_ids(self, ids: str) -> VarLookup:
+        """Filter all entries of given IDS."""
+        ids_vars = self.filter_type(self._ids_variable_key)
+
+        return VarLookup({k: v for k, v in ids_vars.items() if v.ids == ids})
+
+    def groupby_ids(self) -> dict[Hashable, list[IDSVariableModel]]:
+        """Group entries by IDS."""
+        ids_vars = self.filter_type(self._ids_variable_key).values()
+
+        grouped_ids_vars = groupby(ids_vars, keyfunc=lambda var: var.ids)
+        return grouped_ids_vars
+
+
+class VariableConfigLoader:
+
+    def __init__(self):
+        self.paths = self.get_config_path()
+
+    def load(self) -> VarLookup:
+        """Load the variables config."""
+        var_lookup = VarLookup()
+
+        for path in self.paths:
+            logger.debug(f'Loading variables from: {path}')
+
+            var_config = VariableConfigModel.parse_file(path)
+            var_lookup.update(var_config.to_variable_dict())
+
+        return var_lookup
+
+    def get_config_path(self) -> tuple[Path, ...]:
+        """Try to get the config file with variable definitions.
+
+        Search order:
+        1. environment variable
+        (2. local directory, not sure if this should be implemented)
+        3. config home (first $XDG_CONFIG_HOME/duqtools then `$HOME/.config/duqtools`)
+        4. fall back to variable definitions in package
+        """
+        for paths in (
+                self._get_paths_from_environment_variable(),
+                self._get_paths_from_config_home(),
+                self._get_paths_local_directory(),
+        ):
+            if paths:
+                return paths
+
+        return self._get_paths_fallback()
+
+    def _get_paths_from_environment_variable(self) -> tuple[Path, ...] | None:
+        env = os.environ.get(VAR_ENV)
+        if env:
+            path = Path(env)
+            drc = path.parent
+
+            if not drc.exists():
+                raise OSError(f'{path} defined by ${VAR_ENV} does not exist!')
+
+            return tuple(drc.glob(path.name))
+
+        return None
+
+    def _get_paths_local_directory(self) -> tuple[Path, ...] | None:
+        return None  # Not implemented
+
+    def _get_paths_from_config_home(self) -> tuple[Path, ...] | None:
+        config_home = os.environ.get('XDG_CONFIG_HOME', USER_CONFIG_HOME)
+
+        drc = Path(config_home) / DUQTOOLS_DIR
+        if drc.exists():
+            return tuple(drc.glob(VAR_FILENAME_GLOB))
+
+        return None
+
+    def _get_paths_fallback(self) -> tuple[Path, ...]:
+        module = files('duqtools.data')
+        assert module.is_dir()
+        drc: PosixPath = module._paths[0]  # type: ignore
+        return tuple(drc.glob(VAR_FILENAME_GLOB))
+
+
+def lookup_vars(
+        variables: Sequence[(str | IDSVariableModel)]
+) -> list[IDSVariableModel]:
+    """Helper function to look up a bunch of variables.
+
+    If str, look up the variable from the `var_lookup`. Else, check if
+    the variable is an `IDSVariableModel`.
+    """
+    var_models = []
+    for var in variables:
+        if isinstance(var, str):
+            if var.endswith(ERROR_SUFFIX):
+                var = var_lookup.error_upper(var)
+            else:
+                var = var_lookup[var]
+        if not isinstance(var, IDSVariableModel):
+            raise ValueError(f'Cannot lookup variable with type {type(var)}')
+        var_models.append(var)
+    return var_models
+
+
+var_lookup = VariableConfigLoader().load()
```

### Comparing `duqtools-1.6.4/src/duqtools/data/dash/_shared.py` & `duqtools-1.7.0/src/duqtools/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,72 @@
-import sys
-from pathlib import Path
-from typing import Sequence
-
-import xarray as xr
-
-from duqtools.api import ImasHandle, standardize_grid_and_time
-from duqtools.config import var_lookup
-
-try:
-    from streamlit import cache_data
-except ImportError:
-    # work-around for streamlit<1.18
-    from streamlit import experimental_memo as cache_data
-
-try:
-    default_workdir = sys.argv[1]
-except IndexError:
-    default_workdir = str(Path.cwd())
-
-PREFIX = 'profiles_1d/*'
-PREFIX0 = 'profiles_1d/0'
-
-
-@cache_data
-def get_ids_options():
-    return tuple(var_lookup.filter_type('IDS-variable').keys())
-
-
-@cache_data
-def get_var_options(ids):
-    return list(var_lookup.filter_ids(ids).values())
-
-
-@cache_data
-def get_variables(*, ids: str, x_key: str, y_keys: Sequence[str]):
-    return {
-        'time_var': 'time',
-        'grid_var': x_key,
-        'data_vars': y_keys,
-    }
-
-
-@cache_data
-def _get_dataset(handles, variable, *, include_error: bool = False):
-    data_var = variable['name']
-    time_var = variable['dims'][0]
-    grid_var = variable['dims'][1]
-    variables = [data_var, time_var, grid_var]
-
-    datasets = []
-
-    if include_error:
-        variables.append(var_lookup.error_upper(data_var))
-
-    for name, handle in handles.items():
-        handle = ImasHandle(**handle)
-        ds = handle.get_variables(variables=variables)
-        datasets.append(ds)
-
-    grid_var_norm = var_lookup.normalize(grid_var)
-    time_var_norm = var_lookup.normalize(time_var)
-
-    datasets = standardize_grid_and_time(
-        datasets,
-        grid_var=grid_var_norm,
-        time_var=time_var_norm,
-    )
-
-    dataset = xr.concat(datasets, 'run')
-    dataset['run'] = list(handles.keys())
-
-    return dataset, time_var_norm, grid_var_norm, data_var
-
-
-def get_dataset(handles, variable, *, include_error: bool = False):
-    """Convert to hashable types before calling `_get_dataset`."""
-    handles = {name: handle.dict() for name, handle in handles.items()}
-    variable = variable.dict()
-
-    return _get_dataset(handles, variable, include_error=include_error)
+from __future__ import annotations
+
+import logging
+from pathlib import Path
+
+import click
+import xarray as xr
+
+from ._plot_utils import alt_line_chart
+from .config import var_lookup
+from .ids import ImasHandle, rebase_all_coords
+from .utils import read_imas_handles_from_file
+
+logger = logging.getLogger(__name__)
+info, debug = logger.info, logger.debug
+
+
+def plot(*, var_names, handles, input_files, extensions, errorbars, **kwargs):
+    handle_lst = []
+
+    for n, imas_str in enumerate(handles):
+        handle = ImasHandle.from_string(imas_str)
+        handle_lst.append(handle)
+
+    handles = {n: handle for n, handle in enumerate(handle_lst)}
+
+    for input_file in input_files:
+        handles.update(read_imas_handles_from_file(input_file))
+
+    if len(handles) == 0 or len(var_names) == 0:
+        raise SystemExit('No data to show.')
+
+    for n, variable in enumerate(var_lookup[var_name]
+                                 for var_name in var_names):
+        data_var = variable.name
+        time_var = variable.dims[0]
+        grid_var = variable.dims[1]
+
+        grid_var_norm = var_lookup.normalize(grid_var)
+
+        variables = [data_var, grid_var, time_var]
+
+        if errorbars:
+            variables.append(var_lookup.error_upper(data_var))
+
+        datasets = []
+        for handle in handles.values():
+            ds = handle.get_variables(variables=variables)
+            datasets.append(ds)
+
+        datasets = rebase_all_coords(datasets, datasets[0])
+        dataset = xr.concat(datasets, 'run')
+
+        chart = alt_line_chart(dataset,
+                               x=grid_var_norm,
+                               y=data_var,
+                               z=time_var,
+                               std=errorbars)
+
+        click.echo('You can now view your plot in your browser:')
+        click.echo('')
+
+        click.secho(f'  {grid_var_norm} vs. {data_var}:\n', fg='green')
+
+        for extension in extensions:
+
+            outfile = Path(f'chart_{grid_var_norm}-{data_var}.{extension}')
+            click.secho(f'    file:///{outfile.absolute()}', bold=True)
+
+            chart.save(outfile, scale_factor=2.0)
+
+        click.echo('')
```

### Comparing `duqtools-1.6.4/src/duqtools/data/dash/dash.py` & `duqtools-1.7.0/src/duqtools/data/dash/dash.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from pathlib import Path
-
-import pandas as pd
-import streamlit as st
-from _shared import default_workdir, get_dataset
-
-from duqtools._plot_utils import alt_errorband_chart, alt_line_chart
-from duqtools.config import var_lookup
-from duqtools.utils import read_imas_handles_from_file
-
-st.title('Plot IDS')
-
-with st.sidebar:
-    st.header('Input data')
-    work_dir = st.text_input('Work directory', default_workdir)
-    data_file = st.text_input('Data file', 'data.csv')
-
-inp = Path(work_dir) / data_file
-
-if not inp.exists():
-    raise ValueError(f'{inp} does not exist!')
-
-handles = read_imas_handles_from_file(inp)
-df = pd.DataFrame.from_dict(
-    {index: model.dict()
-     for index, model in handles.items()}, orient='index')
-
-with st.expander('Click to show runs'):
-    st.table(df)
-
-with st.sidebar:
-    ids_variables = var_lookup.filter_type('IDS-variable')
-
-    var_names = st.multiselect('Select variable',
-                               tuple(ids_variables),
-                               default=None)
-
-    st.header('Plotting options')
-
-    aggregate_data = st.checkbox(
-        'Aggregate data (mean)',
-        help=(
-            'Calculate mean y-value and standard deviation. All '
-            'y-values are interpolated to put them on a common basis for x.'),
-    )
-    show_errorbar = st.checkbox(
-        'Show error bars',
-        help=('Show standard deviation band around mean y-value.'),
-    )
-
-for variable in (var_lookup[var_name] for var_name in var_names):
-    source, time_var, grid_var, data_var = get_dataset(
-        handles, variable, include_error=show_errorbar)
-
-    st.header(f'{grid_var} vs. {data_var}')
-
-    if aggregate_data:
-        chart = alt_errorband_chart(source, x=grid_var, y=data_var, z=time_var)
-    else:
-        chart = alt_line_chart(source,
-                               x=grid_var,
-                               y=data_var,
-                               z=time_var,
-                               std=show_errorbar)
-
-    st.altair_chart(chart, use_container_width=True)
-
-    if st.button('Save this chart', key=f'download_{grid_var}-{data_var}'):
-        fname = f'chart_{grid_var}-{data_var}.html'
-        chart.save(fname)
-        st.success(f'✔️ Wrote chart to "{fname}"')
+from pathlib import Path
+
+import pandas as pd
+import streamlit as st
+from _shared import default_workdir, get_dataset
+
+from duqtools._plot_utils import alt_errorband_chart, alt_line_chart
+from duqtools.config import var_lookup
+from duqtools.utils import read_imas_handles_from_file
+
+st.title('Plot IDS')
+
+with st.sidebar:
+    st.header('Input data')
+    work_dir = st.text_input('Work directory', default_workdir)
+    data_file = st.text_input('Data file', 'data.csv')
+
+inp = Path(work_dir) / data_file
+
+if not inp.exists():
+    raise ValueError(f'{inp} does not exist!')
+
+handles = read_imas_handles_from_file(inp)
+df = pd.DataFrame.from_dict(
+    {index: model.dict()
+     for index, model in handles.items()}, orient='index')
+
+with st.expander('Click to show runs'):
+    st.table(df)
+
+with st.sidebar:
+    ids_variables = var_lookup.filter_type('IDS-variable')
+
+    var_names = st.multiselect('Select variable',
+                               tuple(ids_variables),
+                               default=None)
+
+    st.header('Plotting options')
+
+    aggregate_data = st.checkbox(
+        'Aggregate data (mean)',
+        help=(
+            'Calculate mean y-value and standard deviation. All '
+            'y-values are interpolated to put them on a common basis for x.'),
+    )
+    show_errorbar = st.checkbox(
+        'Show error bars',
+        help=('Show standard deviation band around mean y-value.'),
+    )
+
+for variable in (var_lookup[var_name] for var_name in var_names):
+    source, time_var, grid_var, data_var = get_dataset(
+        handles, variable, include_error=show_errorbar)
+
+    st.header(f'{grid_var} vs. {data_var}')
+
+    if aggregate_data:
+        chart = alt_errorband_chart(source, x=grid_var, y=data_var, z=time_var)
+    else:
+        chart = alt_line_chart(source,
+                               x=grid_var,
+                               y=data_var,
+                               z=time_var,
+                               std=show_errorbar)
+
+    st.altair_chart(chart, use_container_width=True)
+
+    if st.button('Save this chart', key=f'download_{grid_var}-{data_var}'):
+        fname = f'chart_{grid_var}-{data_var}.html'
+        chart.save(fname)
+        st.success(f'✔️ Wrote chart to "{fname}"')
```

### Comparing `duqtools-1.6.4/src/duqtools/data/duqtools.yaml` & `duqtools-1.7.0/src/duqtools/data/duqtools.yaml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-system: jetto
-quiet: false
-create:
-  runs_dir: ./runs_dir #TODO edit to output directory
-  template: ./template #TODO edit to directory with template
-  dimensions:
-  - operator: multiply
-    scale_to_error: false
-    values: [1.1, 1.2, 1.3]
-    variable: t_i_ave
-  - operator: multiply
-    scale_to_error: false
-    values: [1.1, 1.2, 1.3]
-    variable: zeff
-  - operator: copyto
-    scale_to_error: false
-    values: [296.0, 297.0]
-    variable: major_radius
-  sampler:
-    method: latin-hypercube
-    n_samples: 3
-status:
-  in_file: jetto.in
-  msg_completed: 'Status : Completed successfully'
-  msg_failed: 'Status : Failed'
-  msg_running: 'Status : Running'
-  out_file: jetto.out
-  status_file: jetto.status
-submit:
-  submit_command: sbatch
-  submit_script_name: .llcmd
+system: jetto
+quiet: false
+create:
+  runs_dir: ./runs_dir #TODO edit to output directory
+  template: ./template #TODO edit to directory with template
+  dimensions:
+  - operator: multiply
+    scale_to_error: false
+    values: [1.1, 1.2, 1.3]
+    variable: t_i_ave
+  - operator: multiply
+    scale_to_error: false
+    values: [1.1, 1.2, 1.3]
+    variable: zeff
+  - operator: copyto
+    scale_to_error: false
+    values: [296.0, 297.0]
+    variable: major_radius
+  sampler:
+    method: latin-hypercube
+    n_samples: 3
+status:
+  in_file: jetto.in
+  msg_completed: 'Status : Completed successfully'
+  msg_failed: 'Status : Failed'
+  msg_running: 'Status : Running'
+  out_file: jetto.out
+  status_file: jetto.status
+submit:
+  submit_command: sbatch
+  submit_script_name: .llcmd
```

### Comparing `duqtools-1.6.4/src/duqtools/data/jetto_tools_lookup.json` & `duqtools-1.7.0/src/duqtools/data/jetto_tools_lookup.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,106 @@
-00000000: 7b0d 0a20 2022 7368 6f74 5f69 6e22 3a20  {..  "shot_in": 
-00000010: 7b0d 0a20 2020 2022 6a73 6574 5f69 6422  {..    "jset_id"
-00000020: 3a20 2253 6574 5570 5061 6e65 6c2e 6964  : "SetUpPanel.id
-00000030: 7349 4d41 5344 4253 686f 7422 2c0d 0a20  sIMASDBShot",.. 
-00000040: 2020 2022 6a73 6574 5f66 6c65 785f 6964     "jset_flex_id
-00000050: 223a 205b 0d0a 2020 2020 2020 2241 6476  ": [..      "Adv
-00000060: 616e 6365 6450 616e 656c 2e63 6174 5368  ancedPanel.catSh
-00000070: 6f74 4944 222c 0d0a 2020 2020 2020 2241  otID",..      "A
-00000080: 6476 616e 6365 6450 616e 656c 2e63 6174  dvancedPanel.cat
-00000090: 5368 6f74 4944 5f52 225d 2c0d 0a20 2020  ShotID_R"],..   
-000000a0: 2022 6e6d 6c5f 6964 223a 207b 0d0a 2020   "nml_id": {..  
-000000b0: 2020 2020 226e 616d 656c 6973 7422 3a20      "namelist": 
-000000c0: 2249 4e45 5343 4f22 2c0d 0a20 2020 2020  "INESCO",..     
-000000d0: 2022 6669 656c 6422 3a20 224e 5055 4c53   "field": "NPULS
-000000e0: 4522 0d0a 2020 2020 7d2c 0d0a 2020 2020  E"..    },..    
-000000f0: 2274 7970 6522 3a20 2269 6e74 222c 0d0a  "type": "int",..
-00000100: 2020 2020 2264 696d 656e 7369 6f6e 223a      "dimension":
-00000110: 2022 7363 616c 6172 220d 0a20 207d 2c0d   "scalar"..  },.
-00000120: 0a20 2022 7368 6f74 5f6f 7574 223a 207b  .  "shot_out": {
-00000130: 0d0a 2020 2020 226a 7365 745f 6964 223a  ..    "jset_id":
-00000140: 2022 5365 7455 7050 616e 656c 2e73 686f   "SetUpPanel.sho
-00000150: 744e 756d 222c 0d0a 2020 2020 2274 7970  tNum",..    "typ
-00000160: 6522 3a20 2269 6e74 222c 0d0a 2020 2020  e": "int",..    
-00000170: 2264 696d 656e 7369 6f6e 223a 2022 7363  "dimension": "sc
-00000180: 616c 6172 220d 0a20 207d 2c0d 0a20 2022  alar"..  },..  "
-00000190: 7275 6e5f 696e 223a 207b 0d0a 2020 2020  run_in": {..    
-000001a0: 226a 7365 745f 6964 223a 2022 5365 7455  "jset_id": "SetU
-000001b0: 7050 616e 656c 2e69 6473 494d 4153 4442  pPanel.idsIMASDB
-000001c0: 5275 6e69 6422 2c0d 0a20 2020 2022 7479  Runid",..    "ty
-000001d0: 7065 223a 2022 696e 7422 2c0d 0a20 2020  pe": "int",..   
-000001e0: 2022 6469 6d65 6e73 696f 6e22 3a20 2273   "dimension": "s
-000001f0: 6361 6c61 7222 0d0a 2020 7d2c 0d0a 2020  calar"..  },..  
-00000200: 2272 756e 5f6f 7574 223a 207b 0d0a 2020  "run_out": {..  
-00000210: 2020 226a 7365 745f 6964 223a 2022 4a6f    "jset_id": "Jo
-00000220: 6250 726f 6365 7373 696e 6750 616e 656c  bProcessingPanel
-00000230: 2e69 6473 5275 6e69 6422 2c0d 0a20 2020  .idsRunid",..   
-00000240: 2022 7479 7065 223a 2022 696e 7422 2c0d   "type": "int",.
-00000250: 0a20 2020 2022 6469 6d65 6e73 696f 6e22  .    "dimension"
-00000260: 3a20 2273 6361 6c61 7222 0d0a 2020 7d2c  : "scalar"..  },
-00000270: 0d0a 2020 2275 7365 725f 696e 223a 207b  ..  "user_in": {
-00000280: 0d0a 2020 2020 226a 7365 745f 6964 223a  ..    "jset_id":
-00000290: 2022 5365 7455 7050 616e 656c 2e69 6473   "SetUpPanel.ids
-000002a0: 494d 4153 4442 5573 6572 222c 0d0a 2020  IMASDBUser",..  
-000002b0: 2020 226a 7365 745f 666c 6578 5f69 6422    "jset_flex_id"
-000002c0: 3a5b 0d0a 2020 2020 2020 2241 6476 616e  :[..      "Advan
-000002d0: 6365 6450 616e 656c 2e63 6174 4f77 6e65  cedPanel.catOwne
-000002e0: 7222 2c0d 0a20 2020 2020 2022 4164 7661  r",..      "Adva
-000002f0: 6e63 6564 5061 6e65 6c2e 6361 744f 776e  ncedPanel.catOwn
-00000300: 6572 5f52 225d 2c0d 0a20 2020 2022 7479  er_R"],..    "ty
-00000310: 7065 223a 2022 7374 7222 2c0d 0a20 2020  pe": "str",..   
-00000320: 2022 6469 6d65 6e73 696f 6e22 3a20 2273   "dimension": "s
-00000330: 6361 6c61 7222 0d0a 2020 7d2c 0d0a 2020  calar"..  },..  
-00000340: 226d 6163 6869 6e65 5f69 6e22 3a20 7b0d  "machine_in": {.
-00000350: 0a20 2020 2022 6a73 6574 5f69 6422 3a20  .    "jset_id": 
-00000360: 2253 6574 5570 5061 6e65 6c2e 6964 7349  "SetUpPanel.idsI
-00000370: 4d41 5344 424d 6163 6869 6e65 222c 0d0a  MASDBMachine",..
-00000380: 2020 2020 226a 7365 745f 666c 6578 5f69      "jset_flex_i
-00000390: 6422 3a5b 0d0a 2020 2020 2020 2241 6476  d":[..      "Adv
-000003a0: 616e 6365 6450 616e 656c 2e63 6174 4d61  ancedPanel.catMa
-000003b0: 6368 4944 222c 0d0a 2020 2020 2020 2241  chID",..      "A
-000003c0: 6476 616e 6365 6450 616e 656c 2e63 6174  dvancedPanel.cat
-000003d0: 4d61 6368 4944 5f52 225d 2c0d 0a20 2020  MachID_R"],..   
-000003e0: 2022 7479 7065 223a 2022 7374 7222 2c0d   "type": "str",.
-000003f0: 0a20 2020 2022 6469 6d65 6e73 696f 6e22  .    "dimension"
-00000400: 3a20 2273 6361 6c61 7222 0d0a 2020 7d2c  : "scalar"..  },
-00000410: 0d0a 2020 226d 6163 6869 6e65 5f6f 7574  ..  "machine_out
-00000420: 223a 207b 0d0a 2020 2020 226a 7365 745f  ": {..    "jset_
-00000430: 6964 223a 2022 5365 7455 7050 616e 656c  id": "SetUpPanel
-00000440: 2e6d 6163 6869 6e65 222c 0d0a 2020 2020  .machine",..    
-00000450: 226e 6d6c 5f69 6422 3a20 7b0d 0a20 2020  "nml_id": {..   
-00000460: 2020 2022 6e61 6d65 6c69 7374 223a 2022     "namelist": "
-00000470: 4e4c 4953 5431 222c 0d0a 2020 2020 2020  NLIST1",..      
-00000480: 2266 6965 6c64 223a 2022 4d41 4348 4944  "field": "MACHID
-00000490: 220d 0a20 2020 207d 2c0d 0a20 2020 2022  "..    },..    "
-000004a0: 7479 7065 223a 2022 7374 7222 2c0d 0a20  type": "str",.. 
-000004b0: 2020 2022 6469 6d65 6e73 696f 6e22 3a20     "dimension": 
-000004c0: 2273 6361 6c61 7222 0d0a 2020 7d2c 0d0a  "scalar"..  },..
-000004d0: 2020 226e 6f70 726f 6365 7373 6f72 7322    "noprocessors"
-000004e0: 3a20 7b0d 0a20 2020 2022 6a73 6574 5f69  : {..    "jset_i
-000004f0: 6422 3a20 224a 6f62 5072 6f63 6573 7369  d": "JobProcessi
-00000500: 6e67 5061 6e65 6c2e 6e75 6d50 726f 6365  ngPanel.numProce
-00000510: 7373 6f72 7322 2c0d 0a20 2020 2022 7479  ssors",..    "ty
-00000520: 7065 223a 2022 696e 7422 2c0d 0a20 2020  pe": "int",..   
-00000530: 2022 6469 6d65 6e73 696f 6e22 3a20 2273   "dimension": "s
-00000540: 6361 6c61 7222 0d0a 2020 7d2c 0d0a 2020  calar"..  },..  
-00000550: 2272 756e 5f64 6972 223a 207b 0d0a 2020  "run_dir": {..  
-00000560: 2020 226a 7365 745f 6964 223a 2022 4170    "jset_id": "Ap
-00000570: 7050 616e 656c 2e6f 7065 6e50 7276 5365  pPanel.openPrvSe
-00000580: 7444 6972 222c 0d0a 2020 2020 2274 7970  tDir",..    "typ
-00000590: 6522 3a20 2273 7472 222c 0d0a 2020 2020  e": "str",..    
-000005a0: 2264 696d 656e 7369 6f6e 223a 2022 7363  "dimension": "sc
-000005b0: 616c 6172 220d 0a20 207d 2c0d 0a20 2022  alar"..  },..  "
-000005c0: 7275 6e5f 6469 725f 6e61 6d65 223a 207b  run_dir_name": {
-000005d0: 0d0a 2020 2020 226a 7365 745f 6964 223a  ..    "jset_id":
-000005e0: 2022 4a6f 6250 726f 6365 7373 696e 6750   "JobProcessingP
-000005f0: 616e 656c 2e72 756e 4469 724e 756d 6265  anel.runDirNumbe
-00000600: 7222 2c0d 0a20 2020 2022 7479 7065 223a  r",..    "type":
-00000610: 2022 7374 7222 2c0d 0a20 2020 2022 6469   "str",..    "di
-00000620: 6d65 6e73 696f 6e22 3a20 2273 6361 6c61  mension": "scala
-00000630: 7222 0d0a 2020 7d2c 0d0a 2020 226b 776d  r"..  },..  "kwm
-00000640: 6169 6e22 3a20 7b0d 0a20 2020 2022 6a73  ain": {..    "js
-00000650: 6574 5f69 6422 3a20 6e75 6c6c 2c0d 0a20  et_id": null,.. 
-00000660: 2020 2022 6e6d 6c5f 6964 223a 207b 0d0a     "nml_id": {..
-00000670: 2020 2020 2020 226e 616d 656c 6973 7422        "namelist"
-00000680: 3a20 224e 4c49 5354 3222 2c0d 0a20 2020  : "NLIST2",..   
-00000690: 2020 2022 6669 656c 6422 3a20 224b 574d     "field": "KWM
-000006a0: 4149 4e22 0d0a 2020 2020 7d2c 0d0a 2020  AIN"..    },..  
-000006b0: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
-000006c0: 0d0a 2020 2020 2264 696d 656e 7369 6f6e  ..    "dimension
-000006d0: 223a 2022 7363 616c 6172 220d 0a20 207d  ": "scalar"..  }
-000006e0: 0d0a 7d0d 0a                             ..}..
+00000000: 7b0a 2020 2273 686f 745f 696e 223a 207b  {.  "shot_in": {
+00000010: 0a20 2020 2022 6a73 6574 5f69 6422 3a20  .    "jset_id": 
+00000020: 2253 6574 5570 5061 6e65 6c2e 6964 7349  "SetUpPanel.idsI
+00000030: 4d41 5344 4253 686f 7422 2c0a 2020 2020  MASDBShot",.    
+00000040: 226a 7365 745f 666c 6578 5f69 6422 3a20  "jset_flex_id": 
+00000050: 5b0a 2020 2020 2020 2241 6476 616e 6365  [.      "Advance
+00000060: 6450 616e 656c 2e63 6174 5368 6f74 4944  dPanel.catShotID
+00000070: 222c 0a20 2020 2020 2022 4164 7661 6e63  ",.      "Advanc
+00000080: 6564 5061 6e65 6c2e 6361 7453 686f 7449  edPanel.catShotI
+00000090: 445f 5222 5d2c 0a20 2020 2022 6e6d 6c5f  D_R"],.    "nml_
+000000a0: 6964 223a 207b 0a20 2020 2020 2022 6e61  id": {.      "na
+000000b0: 6d65 6c69 7374 223a 2022 494e 4553 434f  melist": "INESCO
+000000c0: 222c 0a20 2020 2020 2022 6669 656c 6422  ",.      "field"
+000000d0: 3a20 224e 5055 4c53 4522 0a20 2020 207d  : "NPULSE".    }
+000000e0: 2c0a 2020 2020 2274 7970 6522 3a20 2269  ,.    "type": "i
+000000f0: 6e74 222c 0a20 2020 2022 6469 6d65 6e73  nt",.    "dimens
+00000100: 696f 6e22 3a20 2273 6361 6c61 7222 0a20  ion": "scalar". 
+00000110: 207d 2c0a 2020 2273 686f 745f 6f75 7422   },.  "shot_out"
+00000120: 3a20 7b0a 2020 2020 226a 7365 745f 6964  : {.    "jset_id
+00000130: 223a 2022 5365 7455 7050 616e 656c 2e73  ": "SetUpPanel.s
+00000140: 686f 744e 756d 222c 0a20 2020 2022 7479  hotNum",.    "ty
+00000150: 7065 223a 2022 696e 7422 2c0a 2020 2020  pe": "int",.    
+00000160: 2264 696d 656e 7369 6f6e 223a 2022 7363  "dimension": "sc
+00000170: 616c 6172 220a 2020 7d2c 0a20 2022 7275  alar".  },.  "ru
+00000180: 6e5f 696e 223a 207b 0a20 2020 2022 6a73  n_in": {.    "js
+00000190: 6574 5f69 6422 3a20 2253 6574 5570 5061  et_id": "SetUpPa
+000001a0: 6e65 6c2e 6964 7349 4d41 5344 4252 756e  nel.idsIMASDBRun
+000001b0: 6964 222c 0a20 2020 2022 7479 7065 223a  id",.    "type":
+000001c0: 2022 696e 7422 2c0a 2020 2020 2264 696d   "int",.    "dim
+000001d0: 656e 7369 6f6e 223a 2022 7363 616c 6172  ension": "scalar
+000001e0: 220a 2020 7d2c 0a20 2022 7275 6e5f 6f75  ".  },.  "run_ou
+000001f0: 7422 3a20 7b0a 2020 2020 226a 7365 745f  t": {.    "jset_
+00000200: 6964 223a 2022 4a6f 6250 726f 6365 7373  id": "JobProcess
+00000210: 696e 6750 616e 656c 2e69 6473 5275 6e69  ingPanel.idsRuni
+00000220: 6422 2c0a 2020 2020 2274 7970 6522 3a20  d",.    "type": 
+00000230: 2269 6e74 222c 0a20 2020 2022 6469 6d65  "int",.    "dime
+00000240: 6e73 696f 6e22 3a20 2273 6361 6c61 7222  nsion": "scalar"
+00000250: 0a20 207d 2c0a 2020 2275 7365 725f 696e  .  },.  "user_in
+00000260: 223a 207b 0a20 2020 2022 6a73 6574 5f69  ": {.    "jset_i
+00000270: 6422 3a20 2253 6574 5570 5061 6e65 6c2e  d": "SetUpPanel.
+00000280: 6964 7349 4d41 5344 4255 7365 7222 2c0a  idsIMASDBUser",.
+00000290: 2020 2020 226a 7365 745f 666c 6578 5f69      "jset_flex_i
+000002a0: 6422 3a5b 0a20 2020 2020 2022 4164 7661  d":[.      "Adva
+000002b0: 6e63 6564 5061 6e65 6c2e 6361 744f 776e  ncedPanel.catOwn
+000002c0: 6572 222c 0a20 2020 2020 2022 4164 7661  er",.      "Adva
+000002d0: 6e63 6564 5061 6e65 6c2e 6361 744f 776e  ncedPanel.catOwn
+000002e0: 6572 5f52 225d 2c0a 2020 2020 2274 7970  er_R"],.    "typ
+000002f0: 6522 3a20 2273 7472 222c 0a20 2020 2022  e": "str",.    "
+00000300: 6469 6d65 6e73 696f 6e22 3a20 2273 6361  dimension": "sca
+00000310: 6c61 7222 0a20 207d 2c0a 2020 226d 6163  lar".  },.  "mac
+00000320: 6869 6e65 5f69 6e22 3a20 7b0a 2020 2020  hine_in": {.    
+00000330: 226a 7365 745f 6964 223a 2022 5365 7455  "jset_id": "SetU
+00000340: 7050 616e 656c 2e69 6473 494d 4153 4442  pPanel.idsIMASDB
+00000350: 4d61 6368 696e 6522 2c0a 2020 2020 226a  Machine",.    "j
+00000360: 7365 745f 666c 6578 5f69 6422 3a5b 0a20  set_flex_id":[. 
+00000370: 2020 2020 2022 4164 7661 6e63 6564 5061       "AdvancedPa
+00000380: 6e65 6c2e 6361 744d 6163 6849 4422 2c0a  nel.catMachID",.
+00000390: 2020 2020 2020 2241 6476 616e 6365 6450        "AdvancedP
+000003a0: 616e 656c 2e63 6174 4d61 6368 4944 5f52  anel.catMachID_R
+000003b0: 225d 2c0a 2020 2020 2274 7970 6522 3a20  "],.    "type": 
+000003c0: 2273 7472 222c 0a20 2020 2022 6469 6d65  "str",.    "dime
+000003d0: 6e73 696f 6e22 3a20 2273 6361 6c61 7222  nsion": "scalar"
+000003e0: 0a20 207d 2c0a 2020 226d 6163 6869 6e65  .  },.  "machine
+000003f0: 5f6f 7574 223a 207b 0a20 2020 2022 6a73  _out": {.    "js
+00000400: 6574 5f69 6422 3a20 2253 6574 5570 5061  et_id": "SetUpPa
+00000410: 6e65 6c2e 6d61 6368 696e 6522 2c0a 2020  nel.machine",.  
+00000420: 2020 226e 6d6c 5f69 6422 3a20 7b0a 2020    "nml_id": {.  
+00000430: 2020 2020 226e 616d 656c 6973 7422 3a20      "namelist": 
+00000440: 224e 4c49 5354 3122 2c0a 2020 2020 2020  "NLIST1",.      
+00000450: 2266 6965 6c64 223a 2022 4d41 4348 4944  "field": "MACHID
+00000460: 220a 2020 2020 7d2c 0a20 2020 2022 7479  ".    },.    "ty
+00000470: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
+00000480: 2264 696d 656e 7369 6f6e 223a 2022 7363  "dimension": "sc
+00000490: 616c 6172 220a 2020 7d2c 0a20 2022 6e6f  alar".  },.  "no
+000004a0: 7072 6f63 6573 736f 7273 223a 207b 0a20  processors": {. 
+000004b0: 2020 2022 6a73 6574 5f69 6422 3a20 224a     "jset_id": "J
+000004c0: 6f62 5072 6f63 6573 7369 6e67 5061 6e65  obProcessingPane
+000004d0: 6c2e 6e75 6d50 726f 6365 7373 6f72 7322  l.numProcessors"
+000004e0: 2c0a 2020 2020 2274 7970 6522 3a20 2269  ,.    "type": "i
+000004f0: 6e74 222c 0a20 2020 2022 6469 6d65 6e73  nt",.    "dimens
+00000500: 696f 6e22 3a20 2273 6361 6c61 7222 0a20  ion": "scalar". 
+00000510: 207d 2c0a 2020 2272 756e 5f64 6972 223a   },.  "run_dir":
+00000520: 207b 0a20 2020 2022 6a73 6574 5f69 6422   {.    "jset_id"
+00000530: 3a20 2241 7070 5061 6e65 6c2e 6f70 656e  : "AppPanel.open
+00000540: 5072 7653 6574 4469 7222 2c0a 2020 2020  PrvSetDir",.    
+00000550: 2274 7970 6522 3a20 2273 7472 222c 0a20  "type": "str",. 
+00000560: 2020 2022 6469 6d65 6e73 696f 6e22 3a20     "dimension": 
+00000570: 2273 6361 6c61 7222 0a20 207d 2c0a 2020  "scalar".  },.  
+00000580: 2272 756e 5f64 6972 5f6e 616d 6522 3a20  "run_dir_name": 
+00000590: 7b0a 2020 2020 226a 7365 745f 6964 223a  {.    "jset_id":
+000005a0: 2022 4a6f 6250 726f 6365 7373 696e 6750   "JobProcessingP
+000005b0: 616e 656c 2e72 756e 4469 724e 756d 6265  anel.runDirNumbe
+000005c0: 7222 2c0a 2020 2020 2274 7970 6522 3a20  r",.    "type": 
+000005d0: 2273 7472 222c 0a20 2020 2022 6469 6d65  "str",.    "dime
+000005e0: 6e73 696f 6e22 3a20 2273 6361 6c61 7222  nsion": "scalar"
+000005f0: 0a20 207d 2c0a 2020 226b 776d 6169 6e22  .  },.  "kwmain"
+00000600: 3a20 7b0a 2020 2020 226a 7365 745f 6964  : {.    "jset_id
+00000610: 223a 206e 756c 6c2c 0a20 2020 2022 6e6d  ": null,.    "nm
+00000620: 6c5f 6964 223a 207b 0a20 2020 2020 2022  l_id": {.      "
+00000630: 6e61 6d65 6c69 7374 223a 2022 4e4c 4953  namelist": "NLIS
+00000640: 5432 222c 0a20 2020 2020 2022 6669 656c  T2",.      "fiel
+00000650: 6422 3a20 224b 574d 4149 4e22 0a20 2020  d": "KWMAIN".   
+00000660: 207d 2c0a 2020 2020 2274 7970 6522 3a20   },.    "type": 
+00000670: 2273 7472 222c 0a20 2020 2022 6469 6d65  "str",.    "dime
+00000680: 6e73 696f 6e22 3a20 2273 6361 6c61 7222  nsion": "scalar"
+00000690: 0a20 207d 0a7d 0a                        .  }.}.
```

### Comparing `duqtools-1.6.4/src/duqtools/data/variables_equilibrium.yaml` & `duqtools-1.7.0/src/duqtools/data/variables_equilibrium.yaml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-### Equilibrium
-
-- name: beta_p_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/beta_pol
-  dims: [time_eq]
-  type: IDS-variable
-- name: beta_t_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/beta_tor
-  dims: [time_eq]
-  type: IDS-variable
-- name: beta_n_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/beta_normal
-  dims: [time_eq]
-  type: IDS-variable
-- name: ip_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/ip
-  dims: [time_eq]
-  type: IDS-variable
-- name: li3_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/li_3
-  dims: [time_eq]
-  type: IDS-variable
-- name: wmhd_eq
-  ids: equilibrium
-  path: time_slice/*/global_quantities/energy_mhd
-  dims: [time_eq]
-  type: IDS-variable
-- name: psi_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/psi
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: p_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/pressure
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: f_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/f
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: j_tor_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/j_tor
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: j_par_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/j_parallel
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: beta_pol_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/beta_pol
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: q_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/q
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: smag_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/magnetic_shear
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: kappa_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/elongation
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: delta_upper_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/triangularity_upper
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: delta_lower_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/triangularity_lower
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: r_inner_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/r_inboard
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: r_outer_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/r_outboard
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: volume_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/volume
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: area_xs_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/area
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: area_surf_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/surface
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: rho_tor_norm_eq
-  ids: equilibrium
-  path: time_slice/*/profiles_1d/rho_tor_norm
-  dims: [time_eq, $rho_tor_norm_eq]
-  type: IDS-variable
-- name: time_eq
-  ids: equilibrium
-  path: time
-  dims: [time_eq]
-  type: IDS-variable
+### Equilibrium
+
+- name: beta_p_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/beta_pol
+  dims: [time_eq]
+  type: IDS-variable
+- name: beta_t_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/beta_tor
+  dims: [time_eq]
+  type: IDS-variable
+- name: beta_n_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/beta_normal
+  dims: [time_eq]
+  type: IDS-variable
+- name: ip_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/ip
+  dims: [time_eq]
+  type: IDS-variable
+- name: li3_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/li_3
+  dims: [time_eq]
+  type: IDS-variable
+- name: wmhd_eq
+  ids: equilibrium
+  path: time_slice/*/global_quantities/energy_mhd
+  dims: [time_eq]
+  type: IDS-variable
+- name: psi_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/psi
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: p_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/pressure
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: f_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/f
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: j_tor_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/j_tor
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: j_par_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/j_parallel
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: beta_pol_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/beta_pol
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: q_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/q
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: smag_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/magnetic_shear
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: kappa_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/elongation
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: delta_upper_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/triangularity_upper
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: delta_lower_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/triangularity_lower
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: r_inner_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/r_inboard
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: r_outer_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/r_outboard
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: volume_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/volume
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: area_xs_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/area
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: area_surf_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/surface
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: rho_tor_norm_eq
+  ids: equilibrium
+  path: time_slice/*/profiles_1d/rho_tor_norm
+  dims: [time_eq, $rho_tor_norm_eq]
+  type: IDS-variable
+- name: time_eq
+  ids: equilibrium
+  path: time
+  dims: [time_eq]
+  type: IDS-variable
```

### Comparing `duqtools-1.6.4/src/duqtools/data/variables_ids2jetto.yaml` & `duqtools-1.7.0/src/duqtools/data/variables_ids2jetto.yaml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-### Convert from IDs to jetto/other variables
-
-- name: ids-t_start
-  type: IDS2jetto-variable
-  paths:
-    - ids: equilibrium
-      path: time/0
-    - ids: core_profiles
-      path: time/0
-  default: null  # raise if None
-
-- name: ids-b_field
-  type: IDS2jetto-variable
-  paths:
-    - ids: equilibrium
-      path: vacuum_toroidal_field/b0/0
-    - ids: equilibrium
-      path: time_slice/0/global_quantities/magnetic_axis/b_field_tor
-  default: null  # raise if None
-
-- name: ids-major_radius
-  type: IDS2jetto-variable
-  paths:
-    - ids: equilibrium
-      path: vacuum_toroidal_field/r0
-    - ids: equilibrium
-      path: time_slice/0/global_quantities/magnetic_axis/r
-  default: null  # raise if None
+### Convert from IDs to jetto/other variables
+
+- name: ids-t_start
+  type: IDS2jetto-variable
+  paths:
+    - ids: equilibrium
+      path: time/0
+    - ids: core_profiles
+      path: time/0
+  default: null  # raise if None
+
+- name: ids-b_field
+  type: IDS2jetto-variable
+  paths:
+    - ids: equilibrium
+      path: vacuum_toroidal_field/b0/0
+    - ids: equilibrium
+      path: time_slice/0/global_quantities/magnetic_axis/b_field_tor
+  default: null  # raise if None
+
+- name: ids-major_radius
+  type: IDS2jetto-variable
+  paths:
+    - ids: equilibrium
+      path: vacuum_toroidal_field/r0
+    - ids: equilibrium
+      path: time_slice/0/global_quantities/magnetic_axis/r
+  default: null  # raise if None
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/__init__.py` & `duqtools-1.7.0/src/duqtools/ids/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import logging
-
-from ._handle import ImasHandle
-from ._imas import imas_mocked
-from ._mapping import IDSMapping
-from ._merge import merge_data
-from ._rebase import (
-    rebase_all_coords,
-    rebase_on_grid,
-    rebase_on_time,
-    rezero_time,
-    squash_placeholders,
-    standardize_grid,
-    standardize_grid_and_time,
-)
-
-logger = logging.getLogger(__name__)
-
-__all__ = [
-    'IDSMapping',
-    'ImasHandle',
-    'merge_data',
-    'rebase_on_grid',
-    'rebase_on_time',
-    'rebase_all_coords',
-    'standardize_grid_and_time',
-    'standardize_grid',
-    'rezero_time',
-    'squash_placeholders',
-    'imas_mocked',
-]
+import logging
+
+from ._handle import ImasHandle
+from ._imas import imas_mocked
+from ._mapping import IDSMapping
+from ._merge import merge_data
+from ._rebase import (
+    rebase_all_coords,
+    rebase_on_grid,
+    rebase_on_time,
+    rezero_time,
+    squash_placeholders,
+    standardize_grid,
+    standardize_grid_and_time,
+)
+
+logger = logging.getLogger(__name__)
+
+__all__ = [
+    'IDSMapping',
+    'ImasHandle',
+    'merge_data',
+    'rebase_on_grid',
+    'rebase_on_time',
+    'rebase_all_coords',
+    'standardize_grid_and_time',
+    'standardize_grid',
+    'rezero_time',
+    'squash_placeholders',
+    'imas_mocked',
+]
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_apply_model.py` & `duqtools-1.7.0/src/duqtools/ids/_apply_model.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from __future__ import annotations
-
-import logging
-from typing import Union
-
-import numpy as np
-
-from .._logging_utils import duqlog_screen
-from ..apply_model import apply_model
-from ..schema import IDSOperation
-from ._handle import ImasHandle
-from ._mapping import IDSMapping
-
-logger = logging.getLogger(__name__)
-
-
-@apply_model.register  # type: ignore
-def _apply_ids(model: IDSOperation, *,
-               ids_mapping: Union[ImasHandle, IDSMapping], **kwargs) -> None:
-    """Implementation for IDS operations.
-
-    Parameters
-    ----------
-    model : IDSOperation
-        model
-    target_in : ImasHandle, IDSMapping
-        ImasHandle/IDSHandle, data to apply operation to.
-
-    Returns
-    -------
-    None
-    """
-    target_in = None
-    if isinstance(ids_mapping, ImasHandle):
-        target_in = ids_mapping
-        ids_mapping = ids_mapping.get(model.variable.ids)
-
-    if isinstance(model.variable, str):
-        raise TypeError('`model.variable` must have a `path` attribute.')
-
-    npfunc = getattr(np, model.operator)
-
-    data_map = ids_mapping.findall(model.variable.path)
-
-    if len(data_map) == 0:
-        # TODO this should be 'raise Error' but that breaks our tests,
-        # leave it as a message until we can fix it with a Jetto-IMAS container
-        duqlog_screen.error(
-            f'{model.variable.path} not found in IDS, cannot adjust value')
-
-    for path, data in data_map.items():
-        if model.scale_to_error:
-            sigma_key = path + model._upper_suffix
-
-            if model.value < 0:
-                lower_key = path + model._lower_suffix
-                if lower_key in ids_mapping:
-                    sigma_key = lower_key
-
-            if sigma_key not in ids_mapping:
-                raise ValueError(f'scale_to_error={model.scale_to_error} '
-                                 f'but `{sigma_key}` is empty.')
-
-            sigma_bound = ids_mapping[sigma_key]
-            sigma = abs(sigma_bound - data)
-
-            value = sigma * model.value
-        else:
-
-            value = model.value
-
-        logger.info('Apply %s', model)
-
-        logger.debug('data range before: %s - %s', data.min(), data.max())
-        npfunc(data, value, out=data)
-        logger.debug('data range after: %s - %s', data.min(), data.max())
-
-    if target_in:
-        logger.info('Writing data entry: %s', target_in)
-        ids_mapping.sync(target_in)
+from __future__ import annotations
+
+import logging
+from typing import Union
+
+import numpy as np
+
+from .._logging_utils import duqlog_screen
+from ..apply_model import apply_model
+from ..schema import IDSOperation
+from ._handle import ImasHandle
+from ._mapping import IDSMapping
+
+logger = logging.getLogger(__name__)
+
+
+@apply_model.register  # type: ignore
+def _apply_ids(model: IDSOperation, *,
+               ids_mapping: Union[ImasHandle, IDSMapping], **kwargs) -> None:
+    """Implementation for IDS operations.
+
+    Parameters
+    ----------
+    model : IDSOperation
+        model
+    target_in : ImasHandle, IDSMapping
+        ImasHandle/IDSHandle, data to apply operation to.
+
+    Returns
+    -------
+    None
+    """
+    target_in = None
+    if isinstance(ids_mapping, ImasHandle):
+        target_in = ids_mapping
+        ids_mapping = ids_mapping.get(model.variable.ids)
+
+    if isinstance(model.variable, str):
+        raise TypeError('`model.variable` must have a `path` attribute.')
+
+    npfunc = getattr(np, model.operator)
+
+    data_map = ids_mapping.findall(model.variable.path)
+
+    if len(data_map) == 0:
+        # TODO this should be 'raise Error' but that breaks our tests,
+        # leave it as a message until we can fix it with a Jetto-IMAS container
+        duqlog_screen.error(
+            f'{model.variable.path} not found in IDS, cannot adjust value')
+
+    for path, data in data_map.items():
+        if model.scale_to_error:
+            sigma_key = path + model._upper_suffix
+
+            if model.value < 0:
+                lower_key = path + model._lower_suffix
+                if lower_key in ids_mapping:
+                    sigma_key = lower_key
+
+            if sigma_key not in ids_mapping:
+                raise ValueError(f'scale_to_error={model.scale_to_error} '
+                                 f'but `{sigma_key}` is empty.')
+
+            sigma_bound = ids_mapping[sigma_key]
+            sigma = abs(sigma_bound - data)
+
+            value = sigma * model.value
+        else:
+
+            value = model.value
+
+        logger.info('Apply %s', model)
+
+        logger.debug('data range before: %s - %s', data.min(), data.max())
+        npfunc(data, value, out=data)
+        logger.debug('data range after: %s - %s', data.min(), data.max())
+
+    if target_in:
+        logger.info('Writing data entry: %s', target_in)
+        ids_mapping.sync(target_in)
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_handle.py` & `duqtools-1.7.0/src/duqtools/ids/_handle.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,363 +1,363 @@
-from __future__ import annotations
-
-import logging
-import os
-import re
-from contextlib import contextmanager
-from getpass import getuser
-from pathlib import Path
-from typing import TYPE_CHECKING, Sequence
-
-from pydantic import validator
-
-from ..config import lookup_vars, var_lookup
-from ..operations import add_to_op_queue
-from ..schema import IDSVariableModel, ImasBaseModel
-from ._copy import copy_ids_entry
-from ._imas import imas, imasdef
-from ._mapping import IDSMapping
-from ._rebase import squash_placeholders
-
-if TYPE_CHECKING:
-    import xarray as xr
-
-logger = logging.getLogger(__name__)
-
-_FILENAME = 'ids_{shot}{run:04d}{suffix}'
-_IMASDB = ('{db}', '3', '0')
-GLOBAL_PATH_TEMPLATE = str(Path.home().parent.joinpath('{user}', 'public',
-                                                       'imasdb', *_IMASDB,
-                                                       _FILENAME))
-LOCAL_PATH_TEMPLATE = str(Path('{user}', *_IMASDB, _FILENAME))
-
-SUFFIXES = (
-    '.datafile',
-    '.characteristics',
-    '.tree',
-)
-
-IMAS_PATTERN = re.compile(
-    r'^((?P<user>\w+)/)?(?P<db>\w+)/(?P<shot>\d+)/(?P<run>\d+)$')
-
-
-def _patch_str_repr(obj: object):
-    """Reset str/repr methods to default."""
-    import types
-
-    def true_repr(x):
-        type_ = type(x)
-        module = type_.__module__
-        qualname = type_.__qualname__
-        return f'<{module}.{qualname} object at {hex(id(x))}>'
-
-    obj.__str__ = types.MethodType(true_repr, obj)  # type: ignore
-    obj.__repr__ = types.MethodType(true_repr, obj)  # type: ignore
-
-
-class ImasHandle(ImasBaseModel):
-
-    def __str__(self):
-        return f'{self.user}/{self.db}/{self.shot}/{self.run}'
-
-    @classmethod
-    def from_string(cls, string: str) -> ImasHandle:
-        """Return location from formatted string.
-
-        Format:
-
-            <user>/<db>/<shot>/<run>
-            <db>/<shot>/<run>
-
-        Default to the current user if the user is not specified.
-
-        For example:
-
-            g2user/jet/91234/555
-
-        Parameters
-        ----------
-        string : str
-            Input string containing imas db path
-
-        Returns
-        -------
-        ImasHandle
-        """
-        match = IMAS_PATTERN.match(string)
-
-        if match:
-            return cls(**match.groupdict())
-
-        raise ValueError(f'Could not match {string!r}')
-
-    @validator('user')
-    def user_rel_path(cls, v, values):
-        # Override user if we have a relative location
-        if values['relative_location']:
-            logger.info(
-                f'Updating imasdb location with relative location {values["relative_location"]}'
-            )
-            return os.path.abspath(values['relative_location'])
-        return v
-
-    def validate(self):
-        """Validate the user.
-
-        If the user is a path, then create it.
-
-        Raises
-        ------
-        ValueError:
-            If the user is invalid.
-        """
-        if self.is_local_db:
-            # jintrac v220922
-            self.path().parent.mkdir(parents=True, exist_ok=True)
-        elif self.user == getuser() or self.user == 'public':
-            # jintrac v210921
-            pass
-        else:
-            raise ValueError(f'Invalid user: {self.user}')
-
-    def to_string(self) -> str:
-        """Generate string representation of Imas location."""
-        return f'{self.user}/{self.db}/{self.shot}/{self.run}'
-
-    @property
-    def is_local_db(self):
-        """Return True if the handle points to a local imas database."""
-        return self.user.startswith('/')
-
-    def path(self) -> Path:
-        """Return location as Path."""
-        if self.is_local_db:
-            template = LOCAL_PATH_TEMPLATE
-        else:
-            template = GLOBAL_PATH_TEMPLATE
-
-        return Path(
-            template.format(user=self.user,
-                            db=self.db,
-                            shot=self.shot,
-                            run=self.run,
-                            suffix=SUFFIXES[0]))
-
-    def imasdb_path(self) -> Path:
-        """Return path to imasdb."""
-        return self.path().parents[2]
-
-    def exists(self) -> bool:
-        """Return true if the directory exists.
-
-        Returns
-        -------
-        bool
-        """
-        path = self.path()
-        return all(path.with_suffix(sf).exists() for sf in SUFFIXES)
-
-    def copy_data_to(self, destination: ImasHandle):
-        """Copy ids entry to given destination.
-
-        Parameters
-        ----------
-        destination : ImasHandle
-            Copy data to a new location.
-        """
-        logger.debug('Copy %s to %s', self, destination)
-
-        try:
-            copy_ids_entry(self, destination)
-        except Exception as err:
-            raise OSError(f'Failed to copy {self}') from err
-
-    @add_to_op_queue('Removing ids', '{self}')
-    def delete(self):
-        """Remove data from entry."""
-        # ERASE_PULSE operation is yet supported by IMAS as of June 2022
-        path = self.path()
-        for suffix in SUFFIXES:
-            to_delete = path.with_suffix(suffix)
-            logger.debug('Removing %s', to_delete)
-            try:
-                to_delete.unlink()
-            except FileNotFoundError:
-                logger.warning('%s does not exist', to_delete)
-
-    def get_raw_data(self, ids: str = 'core_profiles', **kwargs):
-        """Get data from IDS entry.
-
-        Parameters
-        ----------
-        ids : str, optional
-            Name of profiles to open.
-        **kwargs
-            These keyword parameters are passed to `ImasHandle.open()`.
-
-        Returns
-        -------
-        data
-        """
-        with self.open(**kwargs) as data_entry:
-            data = data_entry.get(ids)
-
-        # reset string representation because output is extremely lengthy
-        _patch_str_repr(data)
-
-        return data
-
-    def get(self, ids: str = 'core_profiles') -> IDSMapping:
-        """Map the data to a dict-like structure.
-
-        Parameters
-        ----------
-        ids : str, optional
-            Name of profiles to open
-
-        Returns
-        -------
-        IDSMapping
-        """
-        raw_data = self.get_raw_data(ids)
-        return IDSMapping(raw_data)
-
-    def get_all_variables(
-        self,
-        extra_variables: Sequence[IDSVariableModel] = [],
-        squash: bool = True,
-        ids: str = 'core_profiles',
-        **kwargs,
-    ) -> xr.Dataset:
-        """Get all variables that duqtools knows of from selected ids from the
-        dataset.
-
-        This function looks up the data location from the
-        `duqtools.config.var_lookup` table
-
-        Parameters
-        ----------
-        variables : Sequence[IDSVariableModel]
-            Extra variables to load in addition to the ones known by duqtools.
-        squash : bool
-            Squash placeholder variables
-
-        Returns
-        -------
-        ds : xarray
-            The data in `xarray` format.
-        **kwargs
-            These keyword arguments are passed to `IDSMapping.to_xarray()`
-
-        Raises
-        ------
-        ValueError
-            When variables are from multiple IDSs.
-        """
-        idsvar_lookup = var_lookup.filter_ids(ids)
-        variables = list(
-            set(list(extra_variables) + list(idsvar_lookup.keys())))
-        return self.get_variables(variables,
-                                  squash,
-                                  empty_var_ok=True,
-                                  **kwargs)
-
-    def get_variables(
-        self,
-        variables: Sequence[str | IDSVariableModel],
-        squash: bool = True,
-        **kwargs,
-    ) -> xr.Dataset:
-        """Get variables from data set.
-
-        This function looks up the data location from the
-        `duqtools.config.var_lookup` table, and returns
-
-        Parameters
-        ----------
-        variables : Sequence[Union[str, IDSVariableModel]]
-            Variable names of the data to load.
-        squash : bool
-            Squash placeholder variables
-
-        Returns
-        -------
-        ds : xarray
-            The data in `xarray` format.
-        **kwargs
-            These keyword arguments are passed to `IDSMapping.to_xarray()`
-
-        Raises
-        ------
-        ValueError
-            When variables are from multiple IDSs.
-        """
-        var_models = lookup_vars(variables)
-
-        idss = {var.ids for var in var_models}
-
-        if len(idss) > 1:
-            raise ValueError(
-                f'All variables must belong to the same IDS, got {idss}')
-
-        ids = var_models[0].ids
-
-        data_map = self.get(ids)
-
-        ds = data_map.to_xarray(variables=var_models, **kwargs)
-
-        if squash:
-            ds = squash_placeholders(ds)
-
-        return ds
-
-    def entry(self, backend=imasdef.MDSPLUS_BACKEND):
-        """Return reference to `imas.DBEntry.`
-
-        Parameters
-        ----------
-        backend : optional
-            Which IMAS backend to use
-
-        Returns
-        ------
-        entry : `imas.DBEntry`
-            IMAS database entry
-        """
-        return imas.DBEntry(backend, self.db, self.shot, self.run, self.user)
-
-    @contextmanager
-    def open(self, backend=imasdef.MDSPLUS_BACKEND, create: bool = False):
-        """Context manager to open database entry.
-
-        Parameters
-        ----------
-        backend : optional
-            Which IMAS backend to use
-        create : bool, optional
-            Create empty database entry if it does not exist.
-
-        Yields
-        ------
-        entry : `imas.DBEntry`
-            Opened IMAS database entry
-        """
-        entry = self.entry(backend=backend)
-        opcode, _ = entry.open()
-
-        if opcode == 0:
-            logger.debug('Data entry opened: %s', self)
-        elif create:
-            cpcode, _ = entry.create()
-            if cpcode == 0:
-                logger.debug('Data entry created: %s', self)
-            else:
-                raise OSError(
-                    f'Cannot create data entry: {self}. '
-                    f'Create a new db first using `imasdb {self.db}`')
-        else:
-            raise OSError(f'Data entry does not exist: {self}')
-
-        try:
-            yield entry
-        finally:
-            entry.close()
+from __future__ import annotations
+
+import logging
+import os
+import re
+from contextlib import contextmanager
+from getpass import getuser
+from pathlib import Path
+from typing import TYPE_CHECKING, Sequence
+
+from pydantic import validator
+
+from ..config import lookup_vars, var_lookup
+from ..operations import add_to_op_queue
+from ..schema import IDSVariableModel, ImasBaseModel
+from ._copy import copy_ids_entry
+from ._imas import imas, imasdef
+from ._mapping import IDSMapping
+from ._rebase import squash_placeholders
+
+if TYPE_CHECKING:
+    import xarray as xr
+
+logger = logging.getLogger(__name__)
+
+_FILENAME = 'ids_{shot}{run:04d}{suffix}'
+_IMASDB = ('{db}', '3', '0')
+GLOBAL_PATH_TEMPLATE = str(Path.home().parent.joinpath('{user}', 'public',
+                                                       'imasdb', *_IMASDB,
+                                                       _FILENAME))
+LOCAL_PATH_TEMPLATE = str(Path('{user}', *_IMASDB, _FILENAME))
+
+SUFFIXES = (
+    '.datafile',
+    '.characteristics',
+    '.tree',
+)
+
+IMAS_PATTERN = re.compile(
+    r'^((?P<user>\w+)/)?(?P<db>\w+)/(?P<shot>\d+)/(?P<run>\d+)$')
+
+
+def _patch_str_repr(obj: object):
+    """Reset str/repr methods to default."""
+    import types
+
+    def true_repr(x):
+        type_ = type(x)
+        module = type_.__module__
+        qualname = type_.__qualname__
+        return f'<{module}.{qualname} object at {hex(id(x))}>'
+
+    obj.__str__ = types.MethodType(true_repr, obj)  # type: ignore
+    obj.__repr__ = types.MethodType(true_repr, obj)  # type: ignore
+
+
+class ImasHandle(ImasBaseModel):
+
+    def __str__(self):
+        return f'{self.user}/{self.db}/{self.shot}/{self.run}'
+
+    @classmethod
+    def from_string(cls, string: str) -> ImasHandle:
+        """Return location from formatted string.
+
+        Format:
+
+            <user>/<db>/<shot>/<run>
+            <db>/<shot>/<run>
+
+        Default to the current user if the user is not specified.
+
+        For example:
+
+            g2user/jet/91234/555
+
+        Parameters
+        ----------
+        string : str
+            Input string containing imas db path
+
+        Returns
+        -------
+        ImasHandle
+        """
+        match = IMAS_PATTERN.match(string)
+
+        if match:
+            return cls(**match.groupdict())
+
+        raise ValueError(f'Could not match {string!r}')
+
+    @validator('user')
+    def user_rel_path(cls, v, values):
+        # Override user if we have a relative location
+        if values['relative_location']:
+            logger.info(
+                f'Updating imasdb location with relative location {values["relative_location"]}'
+            )
+            return os.path.abspath(values['relative_location'])
+        return v
+
+    def validate(self):
+        """Validate the user.
+
+        If the user is a path, then create it.
+
+        Raises
+        ------
+        ValueError:
+            If the user is invalid.
+        """
+        if self.is_local_db:
+            # jintrac v220922
+            self.path().parent.mkdir(parents=True, exist_ok=True)
+        elif self.user == getuser() or self.user == 'public':
+            # jintrac v210921
+            pass
+        else:
+            raise ValueError(f'Invalid user: {self.user}')
+
+    def to_string(self) -> str:
+        """Generate string representation of Imas location."""
+        return f'{self.user}/{self.db}/{self.shot}/{self.run}'
+
+    @property
+    def is_local_db(self):
+        """Return True if the handle points to a local imas database."""
+        return self.user.startswith('/')
+
+    def path(self) -> Path:
+        """Return location as Path."""
+        if self.is_local_db:
+            template = LOCAL_PATH_TEMPLATE
+        else:
+            template = GLOBAL_PATH_TEMPLATE
+
+        return Path(
+            template.format(user=self.user,
+                            db=self.db,
+                            shot=self.shot,
+                            run=self.run,
+                            suffix=SUFFIXES[0]))
+
+    def imasdb_path(self) -> Path:
+        """Return path to imasdb."""
+        return self.path().parents[2]
+
+    def exists(self) -> bool:
+        """Return true if the directory exists.
+
+        Returns
+        -------
+        bool
+        """
+        path = self.path()
+        return all(path.with_suffix(sf).exists() for sf in SUFFIXES)
+
+    def copy_data_to(self, destination: ImasHandle):
+        """Copy ids entry to given destination.
+
+        Parameters
+        ----------
+        destination : ImasHandle
+            Copy data to a new location.
+        """
+        logger.debug('Copy %s to %s', self, destination)
+
+        try:
+            copy_ids_entry(self, destination)
+        except Exception as err:
+            raise OSError(f'Failed to copy {self}') from err
+
+    @add_to_op_queue('Removing ids', '{self}')
+    def delete(self):
+        """Remove data from entry."""
+        # ERASE_PULSE operation is yet supported by IMAS as of June 2022
+        path = self.path()
+        for suffix in SUFFIXES:
+            to_delete = path.with_suffix(suffix)
+            logger.debug('Removing %s', to_delete)
+            try:
+                to_delete.unlink()
+            except FileNotFoundError:
+                logger.warning('%s does not exist', to_delete)
+
+    def get_raw_data(self, ids: str = 'core_profiles', **kwargs):
+        """Get data from IDS entry.
+
+        Parameters
+        ----------
+        ids : str, optional
+            Name of profiles to open.
+        **kwargs
+            These keyword parameters are passed to `ImasHandle.open()`.
+
+        Returns
+        -------
+        data
+        """
+        with self.open(**kwargs) as data_entry:
+            data = data_entry.get(ids)
+
+        # reset string representation because output is extremely lengthy
+        _patch_str_repr(data)
+
+        return data
+
+    def get(self, ids: str = 'core_profiles') -> IDSMapping:
+        """Map the data to a dict-like structure.
+
+        Parameters
+        ----------
+        ids : str, optional
+            Name of profiles to open
+
+        Returns
+        -------
+        IDSMapping
+        """
+        raw_data = self.get_raw_data(ids)
+        return IDSMapping(raw_data)
+
+    def get_all_variables(
+        self,
+        extra_variables: Sequence[IDSVariableModel] = [],
+        squash: bool = True,
+        ids: str = 'core_profiles',
+        **kwargs,
+    ) -> xr.Dataset:
+        """Get all variables that duqtools knows of from selected ids from the
+        dataset.
+
+        This function looks up the data location from the
+        `duqtools.config.var_lookup` table
+
+        Parameters
+        ----------
+        variables : Sequence[IDSVariableModel]
+            Extra variables to load in addition to the ones known by duqtools.
+        squash : bool
+            Squash placeholder variables
+
+        Returns
+        -------
+        ds : xarray
+            The data in `xarray` format.
+        **kwargs
+            These keyword arguments are passed to `IDSMapping.to_xarray()`
+
+        Raises
+        ------
+        ValueError
+            When variables are from multiple IDSs.
+        """
+        idsvar_lookup = var_lookup.filter_ids(ids)
+        variables = list(
+            set(list(extra_variables) + list(idsvar_lookup.keys())))
+        return self.get_variables(variables,
+                                  squash,
+                                  empty_var_ok=True,
+                                  **kwargs)
+
+    def get_variables(
+        self,
+        variables: Sequence[str | IDSVariableModel],
+        squash: bool = True,
+        **kwargs,
+    ) -> xr.Dataset:
+        """Get variables from data set.
+
+        This function looks up the data location from the
+        `duqtools.config.var_lookup` table, and returns
+
+        Parameters
+        ----------
+        variables : Sequence[Union[str, IDSVariableModel]]
+            Variable names of the data to load.
+        squash : bool
+            Squash placeholder variables
+
+        Returns
+        -------
+        ds : xarray
+            The data in `xarray` format.
+        **kwargs
+            These keyword arguments are passed to `IDSMapping.to_xarray()`
+
+        Raises
+        ------
+        ValueError
+            When variables are from multiple IDSs.
+        """
+        var_models = lookup_vars(variables)
+
+        idss = {var.ids for var in var_models}
+
+        if len(idss) > 1:
+            raise ValueError(
+                f'All variables must belong to the same IDS, got {idss}')
+
+        ids = var_models[0].ids
+
+        data_map = self.get(ids)
+
+        ds = data_map.to_xarray(variables=var_models, **kwargs)
+
+        if squash:
+            ds = squash_placeholders(ds)
+
+        return ds
+
+    def entry(self, backend=imasdef.MDSPLUS_BACKEND):
+        """Return reference to `imas.DBEntry.`
+
+        Parameters
+        ----------
+        backend : optional
+            Which IMAS backend to use
+
+        Returns
+        ------
+        entry : `imas.DBEntry`
+            IMAS database entry
+        """
+        return imas.DBEntry(backend, self.db, self.shot, self.run, self.user)
+
+    @contextmanager
+    def open(self, backend=imasdef.MDSPLUS_BACKEND, create: bool = False):
+        """Context manager to open database entry.
+
+        Parameters
+        ----------
+        backend : optional
+            Which IMAS backend to use
+        create : bool, optional
+            Create empty database entry if it does not exist.
+
+        Yields
+        ------
+        entry : `imas.DBEntry`
+            Opened IMAS database entry
+        """
+        entry = self.entry(backend=backend)
+        opcode, _ = entry.open()
+
+        if opcode == 0:
+            logger.debug('Data entry opened: %s', self)
+        elif create:
+            cpcode, _ = entry.create()
+            if cpcode == 0:
+                logger.debug('Data entry created: %s', self)
+            else:
+                raise OSError(
+                    f'Cannot create data entry: {self}. '
+                    f'Create a new db first using `imasdb {self.db}`')
+        else:
+            raise OSError(f'Data entry does not exist: {self}')
+
+        try:
+            yield entry
+        finally:
+            entry.close()
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_imas.py` & `duqtools-1.7.0/src/duqtools/ids/_imas.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# https://github.com/duqtools/duqtools/issues/27
-
-import logging
-
-logger = logging.getLogger(__name__)
-imas_mocked = False
-
-try:
-    import os
-    import xml.sax
-    import xml.sax.handler
-
-    import imas
-    from imas import imasdef
-
-    IMAS_PREFIX = os.getenv('IMAS_PREFIX', '')
-    PATH_IDSDEF = f'{IMAS_PREFIX}/include/IDSDef.xml'
-
-    class Parser(xml.sax.handler.ContentHandler):
-        import xml.sax
-        import xml.sax.handler
-
-        def __init__(self):
-            xml.sax.handler.ContentHandler.__init__(self)
-            self.idss = []
-
-        def startElement(self, name: str, attrs):
-            if name == 'IDS':
-                ids = {}
-                for i in attrs.getNames():
-                    ids[i] = attrs.getValue(i)
-                self.idss.append(ids)
-
-        @classmethod
-        def load_idsdef(cls):
-            parser = cls()
-            xml.sax.parse(PATH_IDSDEF, parser)
-            return parser
-
-except (ModuleNotFoundError, ImportError):
-    from unittest.mock import MagicMock as Mock
-    imas_mocked = True
-    ids = Mock()
-    ids.open_env = lambda *_, **__: [1]
-
-    entry = Mock()
-    entry.open = lambda *_, **__: (0, Mock())
-
-    imas = Mock()
-    imas.names = ['imas_3_34_0_ual_4_9_3']
-    imas.ids = lambda *_, **__: ids
-    imas.DBEntry = lambda *_, **__: entry
-
-    imasdef = Mock()
-
-    Parser = Mock()  # type: ignore
-
-    logger.warning('Could not import IMAS:', exc_info=True)
+# https://github.com/duqtools/duqtools/issues/27
+
+import logging
+
+logger = logging.getLogger(__name__)
+imas_mocked = False
+
+try:
+    import os
+    import xml.sax
+    import xml.sax.handler
+
+    import imas
+    from imas import imasdef
+
+    IMAS_PREFIX = os.getenv('IMAS_PREFIX', '')
+    PATH_IDSDEF = f'{IMAS_PREFIX}/include/IDSDef.xml'
+
+    class Parser(xml.sax.handler.ContentHandler):
+        import xml.sax
+        import xml.sax.handler
+
+        def __init__(self):
+            xml.sax.handler.ContentHandler.__init__(self)
+            self.idss = []
+
+        def startElement(self, name: str, attrs):
+            if name == 'IDS':
+                ids = {}
+                for i in attrs.getNames():
+                    ids[i] = attrs.getValue(i)
+                self.idss.append(ids)
+
+        @classmethod
+        def load_idsdef(cls):
+            parser = cls()
+            xml.sax.parse(PATH_IDSDEF, parser)
+            return parser
+
+except (ModuleNotFoundError, ImportError):
+    from unittest.mock import MagicMock as Mock
+    imas_mocked = True
+    ids = Mock()
+    ids.open_env = lambda *_, **__: [1]
+
+    entry = Mock()
+    entry.open = lambda *_, **__: (0, Mock())
+
+    imas = Mock()
+    imas.names = ['imas_3_34_0_ual_4_9_3']
+    imas.ids = lambda *_, **__: ids
+    imas.DBEntry = lambda *_, **__: entry
+
+    imasdef = Mock()
+
+    Parser = Mock()  # type: ignore
+
+    logger.warning('Could not import IMAS:', exc_info=True)
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_mapping.py` & `duqtools-1.7.0/src/duqtools/ids/_mapping.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,414 +1,414 @@
-from __future__ import annotations
-
-import re
-from collections.abc import Mapping
-from typing import TYPE_CHECKING, Any, Sequence
-
-import numpy as np
-
-from duqtools.config import lookup_vars
-
-from ..schema import IDSVariableModel
-from ._copy import add_provenance_info
-
-if TYPE_CHECKING:
-    import xarray as xr
-
-    from ._handle import ImasHandle
-
-INDEX_STR = '*'
-
-
-class EmptyVarError(Exception):
-    ...
-
-
-def insert_re_caret_dollar(string: str) -> str:
-    """Insert regex start (^) / end ($) of line matching characters."""
-    if not string.startswith('^'):
-        string = f'^{string}'
-    if not string.endswith('$'):
-        string = f'{string}$'
-    return string
-
-
-def replace_index_str(string: str) -> str:
-    """Replaces template string with regex digit matching."""
-    return string.replace(INDEX_STR, r'(\d+)')
-
-
-class IDSMapping(Mapping):
-
-    def __init__(self, ids):
-        """Map the IMASDB object.
-
-        Empty arrays are excluded from the mapping.
-        You can still get/set these keys directly,
-        but `key in map` returns `False` if `map['key']` is an empty array.
-
-        Parameters
-        ----------
-        ids :
-            IMAS DB entry for the IDS.
-
-        Attributes
-        ----------
-        exclude_empty : bool
-        """
-        self._ids = ids
-
-        # All available data fields are stored in this set.
-        self._keys: set[str] = set()
-        self._paths: dict[str, Any] = {}
-
-        self.dive(ids, [])
-
-    def __repr__(self):
-        s = f'{self.__class__.__name__}(\n'
-        for key in self._paths:
-            s += f'  {key} = ...\n'
-        s += ')\n'
-
-        return s
-
-    @staticmethod
-    def _getattr(pointer: Any, attr: str) -> Any:
-        """Like `getattr`, but will return the index if `attr` is an int."""
-        try:
-            i = int(attr)
-        except (ValueError, TypeError):
-            ret = getattr(pointer, attr)
-        else:
-            ret = pointer[i]  # type: ignore
-
-        return ret
-
-    def _deconstruct_key(self, key: str) -> tuple[Any, str]:
-        """Break down key and return pointer + attr."""
-        *parts, attr = key.split('/')
-
-        pointer = self._ids
-
-        for part in parts:
-            pointer = self._getattr(pointer, part)
-
-        return pointer, attr
-
-    def __getitem__(self, key: str) -> Any:
-
-        try:
-            pointer, attr = self._deconstruct_key(key)
-            ret = self._getattr(pointer, attr)
-        except AttributeError as err:
-            raise KeyError(key) from err
-        except IndexError as err:
-            raise KeyError(key) from err
-
-        return ret
-
-    def __setitem__(self, key: str, value: np.ndarray):
-
-        try:
-            pointer, attr = self._deconstruct_key(key)
-            getattr(pointer, attr)
-        except AttributeError as err:
-            raise KeyError(key) from err
-        except IndexError as err:
-            raise KeyError(key) from err
-        else:
-            setattr(pointer, attr, value)
-
-    def __iter__(self):
-        yield from self._keys
-
-    def __len__(self):
-        return len(self._keys)
-
-    def __contains__(self, key):
-        return key in self._keys
-
-    @staticmethod
-    def _path_at_index(variable: str | IDSVariableModel,
-                       index: int | Sequence[int]):
-        path = variable.path if isinstance(variable,
-                                           IDSVariableModel) else variable
-
-        if isinstance(index, int):
-            index = (index, )
-
-        for i in index:
-            path = path.replace('*', str(i), 1)
-
-        return path
-
-    def get_at_index(self, variable: str | IDSVariableModel,
-                     index: int | Sequence[int], **kwargs) -> Any:
-        """Grab key with index replacement.
-
-        Example: `IDSMapping.get_at_index(var, index=0)`
-        """
-        path = self._path_at_index(variable, index)
-        return self[path]
-
-    def set_at_index(self, variable: str | IDSVariableModel,
-                     index: int | Sequence[int], value: Any, **kwargs):
-        """Grab key with index replacement.
-
-        Example: `IDSMapping.set_at_index(var, value, index=0)`
-        """
-        path = self._path_at_index(variable, index)
-        self[path] = value
-
-    def length_of_key(self, key: str):
-        """length_of_key gives you the number of entries of a (partial) ids
-        path, or None if the length does not exist.
-
-        Note: this is different then the length of an IDSMapping, which is defined
-        as the number of keys
-
-        Note: calling `len(map[key])` works as well
-
-        ## Example:
-
-
-        ```python
-        map.length_of_key('1d_profiles')
-        ```
-
-        Parameters
-        ----------
-        key : str
-            key
-        """
-        try:
-            return len(self[key])
-        except Exception:
-            pass
-
-    def sync(self, target: ImasHandle):
-        """Synchronize updated data back to IMAS db entry.
-
-        Shortcut for 'put' command.
-
-        Parameters
-        ----------
-        target : ImasHandle
-            Points to an IMAS db entry of where the data should be written.
-        """
-
-        add_provenance_info(handle=target)
-
-        with target.open() as db_entry:
-            self._ids.put(db_entry=db_entry)
-
-    def dive(self, val, path: list):
-        """Recursively find the data fields.
-
-        Parameters
-        ----------
-        val :
-            Current nested object being evaluated
-        path : list
-            Current path
-        """
-
-        if isinstance(val, str):
-            return
-
-        if hasattr(val,
-                   '__getitem__') and not isinstance(val,
-                                                     (np.ndarray, np.generic)):
-            for i in range(len(val)):
-                item = val[i]
-                self.dive(item, path + [str(i)])
-            return
-
-        if hasattr(val, '__dict__'):
-            for key, item in val.__dict__.items():
-                self.dive(item, path + [key])
-            return
-
-        if not isinstance(val, (np.ndarray, np.generic)):
-            return
-
-        if val.size == 0:
-            return
-
-        # We made it here, the value can be stored
-        str_path = '/'.join(path)
-        self._keys.add(str_path)
-
-        cur = self._paths
-        for part in path[:-1]:
-            cur.setdefault(part, {})
-            cur = cur[part]
-        cur[path[-1]] = str_path
-
-    def findall(self, pattern: str) -> dict[str, Any]:
-        """Find keys matching regex pattern.
-
-        Parameters
-        ----------
-        pattern : str
-            Regex pattern
-
-        Returns
-        -------
-        dict
-            New dict with all matching key/value pairs.
-        """
-        pattern = insert_re_caret_dollar(pattern)
-        pattern = replace_index_str(pattern)
-
-        pat = re.compile(pattern)
-
-        return {key: self[key] for key in self._keys if pat.match(key)}
-
-    def find_by_group(self, pattern: str) -> dict[tuple | str, Any]:
-        """Find keys matching regex pattern by group.
-
-        The dict key is defined by `match.groups()`.
-        Dict entries will be overwritten if the groups are not unique.
-
-        Parameters
-        ----------
-        pattern : str
-            Regex pattern (must contain groups)
-
-        Returns
-        -------
-        dict
-            New dict with all matching key/value pairs.
-        """
-        pattern = insert_re_caret_dollar(pattern)
-        pattern = replace_index_str(pattern)
-
-        pat = re.compile(pattern)
-
-        new = {}
-        for key in self._keys:
-            m = pat.match(key)
-            if m:
-                groups = m.groups()
-                idx = groups[0] if len(groups) == 1 else groups
-                new[idx] = self[key]
-
-        return new
-
-    def _read_array_from_parts(self, *parts: str):
-        arr = []
-        root, sub, *remaining = parts
-        nodes = self[root]
-
-        for index in range(len(nodes)):
-            path = f'{root}/{index}/{sub}'
-
-            if remaining:
-                sub_arr = self._read_array_from_parts(path, *remaining)
-            else:
-                sub_arr = self[path]
-
-            arr.append(sub_arr)
-
-        return arr
-
-    def to_xarray(
-        self,
-        variables: Sequence[str | IDSVariableModel],
-        empty_var_ok: bool = False,
-        **kwargs,
-    ) -> xr.Dataset:
-        """Return dataset for given variables.
-
-        Parameters
-        ----------
-        variables : Sequence[str | IDSVariableModel]]
-            Dictionary of data variables
-        empty_var_ok : bool
-            If True, silently skip data that are missing from the mapping.
-            If False (default), raise an error when data that are missing
-            from the dataset are requested.
-
-        Returns
-        -------
-        ds : xr.Dataset
-            Return query as Dataset
-        """
-
-        def _contains_empty(arr):
-            if isinstance(arr, list):
-                if len(arr) == 0:
-                    return True
-                return any(_contains_empty(sub_arr) for sub_arr in arr)
-            elif isinstance(arr, np.ndarray):
-                return arr.size == 0
-            elif isinstance(arr, (float, int)):
-                return False
-            else:
-                raise ValueError(
-                    f"Don't know how to deal with: {var.name}: {arr}")
-
-        import xarray as xr
-
-        xr_data_vars: dict[str, tuple[list[str], np.ndarray]] = {}
-
-        variables = lookup_vars(variables)
-
-        for var in variables:
-            parts = var.path.split('/*/')
-
-            if len(parts) == 1:
-                xr_data_vars[var.name] = (var.dims, self[var.path])
-                continue
-
-            arr = self._read_array_from_parts(*parts)
-
-            if _contains_empty(arr):
-                if empty_var_ok:
-                    continue
-                else:
-                    raise EmptyVarError(
-                        f'Variable {var.name!r} contains empty data.')
-            xr_data_vars[var.name] = ([*var.dims], arr)
-
-        ds = xr.Dataset(data_vars=xr_data_vars)  # type: ignore
-
-        return ds
-
-    def _write_array_in_parts(self, data, *parts: str) -> None:
-        """_write_array_in_parts.
-
-        inner function that determines the path and writes back the data
-        """
-        if len(parts) < 2:
-            # Write back
-            path, = parts
-            self[path] = data
-            return
-
-        root, sub, *remaining = parts
-        nodes = self[root]
-        for index in range(len(nodes)):
-            path = f'{root}/{index}/{sub}'
-            self._write_array_in_parts(data[index], path, *remaining)
-
-    def write_array_in_parts(self, variable_path: str,
-                             data: xr.DataArray) -> None:
-        """write_back data, give the data, and the variable path, where `*`
-        denotes the dimensions. This function will figure out how to write it
-        back to the IDS.
-
-        Parameters
-        ----------
-        variable_path : str
-            path of the variable in the IDS, something like 'profiles_1d/*/zeff'
-        data : xr.DataArray
-            data of the variable, in the correct dimensions (every star in the
-            `variable_path` is a dimension in this array)
-
-        Returns
-        -------
-        None
-        """
-        parts = variable_path.split('/*/')
-        self._write_array_in_parts(data.data, *parts)
+from __future__ import annotations
+
+import re
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Any, Sequence
+
+import numpy as np
+
+from duqtools.config import lookup_vars
+
+from ..schema import IDSVariableModel
+from ._copy import add_provenance_info
+
+if TYPE_CHECKING:
+    import xarray as xr
+
+    from ._handle import ImasHandle
+
+INDEX_STR = '*'
+
+
+class EmptyVarError(Exception):
+    ...
+
+
+def insert_re_caret_dollar(string: str) -> str:
+    """Insert regex start (^) / end ($) of line matching characters."""
+    if not string.startswith('^'):
+        string = f'^{string}'
+    if not string.endswith('$'):
+        string = f'{string}$'
+    return string
+
+
+def replace_index_str(string: str) -> str:
+    """Replaces template string with regex digit matching."""
+    return string.replace(INDEX_STR, r'(\d+)')
+
+
+class IDSMapping(Mapping):
+
+    def __init__(self, ids):
+        """Map the IMASDB object.
+
+        Empty arrays are excluded from the mapping.
+        You can still get/set these keys directly,
+        but `key in map` returns `False` if `map['key']` is an empty array.
+
+        Parameters
+        ----------
+        ids :
+            IMAS DB entry for the IDS.
+
+        Attributes
+        ----------
+        exclude_empty : bool
+        """
+        self._ids = ids
+
+        # All available data fields are stored in this set.
+        self._keys: set[str] = set()
+        self._paths: dict[str, Any] = {}
+
+        self.dive(ids, [])
+
+    def __repr__(self):
+        s = f'{self.__class__.__name__}(\n'
+        for key in self._paths:
+            s += f'  {key} = ...\n'
+        s += ')\n'
+
+        return s
+
+    @staticmethod
+    def _getattr(pointer: Any, attr: str) -> Any:
+        """Like `getattr`, but will return the index if `attr` is an int."""
+        try:
+            i = int(attr)
+        except (ValueError, TypeError):
+            ret = getattr(pointer, attr)
+        else:
+            ret = pointer[i]  # type: ignore
+
+        return ret
+
+    def _deconstruct_key(self, key: str) -> tuple[Any, str]:
+        """Break down key and return pointer + attr."""
+        *parts, attr = key.split('/')
+
+        pointer = self._ids
+
+        for part in parts:
+            pointer = self._getattr(pointer, part)
+
+        return pointer, attr
+
+    def __getitem__(self, key: str) -> Any:
+
+        try:
+            pointer, attr = self._deconstruct_key(key)
+            ret = self._getattr(pointer, attr)
+        except AttributeError as err:
+            raise KeyError(key) from err
+        except IndexError as err:
+            raise KeyError(key) from err
+
+        return ret
+
+    def __setitem__(self, key: str, value: np.ndarray):
+
+        try:
+            pointer, attr = self._deconstruct_key(key)
+            getattr(pointer, attr)
+        except AttributeError as err:
+            raise KeyError(key) from err
+        except IndexError as err:
+            raise KeyError(key) from err
+        else:
+            setattr(pointer, attr, value)
+
+    def __iter__(self):
+        yield from self._keys
+
+    def __len__(self):
+        return len(self._keys)
+
+    def __contains__(self, key):
+        return key in self._keys
+
+    @staticmethod
+    def _path_at_index(variable: str | IDSVariableModel,
+                       index: int | Sequence[int]):
+        path = variable.path if isinstance(variable,
+                                           IDSVariableModel) else variable
+
+        if isinstance(index, int):
+            index = (index, )
+
+        for i in index:
+            path = path.replace('*', str(i), 1)
+
+        return path
+
+    def get_at_index(self, variable: str | IDSVariableModel,
+                     index: int | Sequence[int], **kwargs) -> Any:
+        """Grab key with index replacement.
+
+        Example: `IDSMapping.get_at_index(var, index=0)`
+        """
+        path = self._path_at_index(variable, index)
+        return self[path]
+
+    def set_at_index(self, variable: str | IDSVariableModel,
+                     index: int | Sequence[int], value: Any, **kwargs):
+        """Grab key with index replacement.
+
+        Example: `IDSMapping.set_at_index(var, value, index=0)`
+        """
+        path = self._path_at_index(variable, index)
+        self[path] = value
+
+    def length_of_key(self, key: str):
+        """length_of_key gives you the number of entries of a (partial) ids
+        path, or None if the length does not exist.
+
+        Note: this is different then the length of an IDSMapping, which is defined
+        as the number of keys
+
+        Note: calling `len(map[key])` works as well
+
+        ## Example:
+
+
+        ```python
+        map.length_of_key('1d_profiles')
+        ```
+
+        Parameters
+        ----------
+        key : str
+            key
+        """
+        try:
+            return len(self[key])
+        except Exception:
+            pass
+
+    def sync(self, target: ImasHandle):
+        """Synchronize updated data back to IMAS db entry.
+
+        Shortcut for 'put' command.
+
+        Parameters
+        ----------
+        target : ImasHandle
+            Points to an IMAS db entry of where the data should be written.
+        """
+
+        add_provenance_info(handle=target)
+
+        with target.open() as db_entry:
+            self._ids.put(db_entry=db_entry)
+
+    def dive(self, val, path: list):
+        """Recursively find the data fields.
+
+        Parameters
+        ----------
+        val :
+            Current nested object being evaluated
+        path : list
+            Current path
+        """
+
+        if isinstance(val, str):
+            return
+
+        if hasattr(val,
+                   '__getitem__') and not isinstance(val,
+                                                     (np.ndarray, np.generic)):
+            for i in range(len(val)):
+                item = val[i]
+                self.dive(item, path + [str(i)])
+            return
+
+        if hasattr(val, '__dict__'):
+            for key, item in val.__dict__.items():
+                self.dive(item, path + [key])
+            return
+
+        if not isinstance(val, (np.ndarray, np.generic)):
+            return
+
+        if val.size == 0:
+            return
+
+        # We made it here, the value can be stored
+        str_path = '/'.join(path)
+        self._keys.add(str_path)
+
+        cur = self._paths
+        for part in path[:-1]:
+            cur.setdefault(part, {})
+            cur = cur[part]
+        cur[path[-1]] = str_path
+
+    def findall(self, pattern: str) -> dict[str, Any]:
+        """Find keys matching regex pattern.
+
+        Parameters
+        ----------
+        pattern : str
+            Regex pattern
+
+        Returns
+        -------
+        dict
+            New dict with all matching key/value pairs.
+        """
+        pattern = insert_re_caret_dollar(pattern)
+        pattern = replace_index_str(pattern)
+
+        pat = re.compile(pattern)
+
+        return {key: self[key] for key in self._keys if pat.match(key)}
+
+    def find_by_group(self, pattern: str) -> dict[tuple | str, Any]:
+        """Find keys matching regex pattern by group.
+
+        The dict key is defined by `match.groups()`.
+        Dict entries will be overwritten if the groups are not unique.
+
+        Parameters
+        ----------
+        pattern : str
+            Regex pattern (must contain groups)
+
+        Returns
+        -------
+        dict
+            New dict with all matching key/value pairs.
+        """
+        pattern = insert_re_caret_dollar(pattern)
+        pattern = replace_index_str(pattern)
+
+        pat = re.compile(pattern)
+
+        new = {}
+        for key in self._keys:
+            m = pat.match(key)
+            if m:
+                groups = m.groups()
+                idx = groups[0] if len(groups) == 1 else groups
+                new[idx] = self[key]
+
+        return new
+
+    def _read_array_from_parts(self, *parts: str):
+        arr = []
+        root, sub, *remaining = parts
+        nodes = self[root]
+
+        for index in range(len(nodes)):
+            path = f'{root}/{index}/{sub}'
+
+            if remaining:
+                sub_arr = self._read_array_from_parts(path, *remaining)
+            else:
+                sub_arr = self[path]
+
+            arr.append(sub_arr)
+
+        return arr
+
+    def to_xarray(
+        self,
+        variables: Sequence[str | IDSVariableModel],
+        empty_var_ok: bool = False,
+        **kwargs,
+    ) -> xr.Dataset:
+        """Return dataset for given variables.
+
+        Parameters
+        ----------
+        variables : Sequence[str | IDSVariableModel]]
+            Dictionary of data variables
+        empty_var_ok : bool
+            If True, silently skip data that are missing from the mapping.
+            If False (default), raise an error when data that are missing
+            from the dataset are requested.
+
+        Returns
+        -------
+        ds : xr.Dataset
+            Return query as Dataset
+        """
+
+        def _contains_empty(arr):
+            if isinstance(arr, list):
+                if len(arr) == 0:
+                    return True
+                return any(_contains_empty(sub_arr) for sub_arr in arr)
+            elif isinstance(arr, np.ndarray):
+                return arr.size == 0
+            elif isinstance(arr, (float, int)):
+                return False
+            else:
+                raise ValueError(
+                    f"Don't know how to deal with: {var.name}: {arr}")
+
+        import xarray as xr
+
+        xr_data_vars: dict[str, tuple[list[str], np.ndarray]] = {}
+
+        variables = lookup_vars(variables)
+
+        for var in variables:
+            parts = var.path.split('/*/')
+
+            if len(parts) == 1:
+                xr_data_vars[var.name] = (var.dims, self[var.path])
+                continue
+
+            arr = self._read_array_from_parts(*parts)
+
+            if _contains_empty(arr):
+                if empty_var_ok:
+                    continue
+                else:
+                    raise EmptyVarError(
+                        f'Variable {var.name!r} contains empty data.')
+            xr_data_vars[var.name] = ([*var.dims], arr)
+
+        ds = xr.Dataset(data_vars=xr_data_vars)  # type: ignore
+
+        return ds
+
+    def _write_array_in_parts(self, data, *parts: str) -> None:
+        """_write_array_in_parts.
+
+        inner function that determines the path and writes back the data
+        """
+        if len(parts) < 2:
+            # Write back
+            path, = parts
+            self[path] = data
+            return
+
+        root, sub, *remaining = parts
+        nodes = self[root]
+        for index in range(len(nodes)):
+            path = f'{root}/{index}/{sub}'
+            self._write_array_in_parts(data[index], path, *remaining)
+
+    def write_array_in_parts(self, variable_path: str,
+                             data: xr.DataArray) -> None:
+        """write_back data, give the data, and the variable path, where `*`
+        denotes the dimensions. This function will figure out how to write it
+        back to the IDS.
+
+        Parameters
+        ----------
+        variable_path : str
+            path of the variable in the IDS, something like 'profiles_1d/*/zeff'
+        data : xr.DataArray
+            data of the variable, in the correct dimensions (every star in the
+            `variable_path` is a dimension in this array)
+
+        Returns
+        -------
+        None
+        """
+        parts = variable_path.split('/*/')
+        self._write_array_in_parts(data.data, *parts)
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_merge.py` & `duqtools-1.7.0/src/duqtools/ids/_merge.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import logging
-from typing import Sequence
-
-import xarray as xr
-
-from ..config import var_lookup
-from ..operations import add_to_op_queue
-from ..schema import IDSVariableModel
-from ..utils import groupby
-from ._handle import ImasHandle
-from ._rebase import rebase_all_coords, squash_placeholders
-
-logger = logging.getLogger(__name__)
-
-info = logger.info
-
-
-@add_to_op_queue('Merging to', '{target}')
-def merge_data(
-    handles: Sequence[ImasHandle],
-    target: ImasHandle,
-    variables: list[IDSVariableModel],
-    callback=None,
-):
-    """merge_data merges the data from the handles to the target, only merges
-    over the listed variables, coordination variables are never overwritten,
-    and data is rebased according to the target coordination variable.
-
-    Parameters
-    ----------
-    handles : Sequence[ImasHandle]
-        handles
-    target : ImasHandle
-        target
-    variables : Sequence[IDSVariableModel]
-        variables
-    """
-    # Add dimensions to variables
-    variable_dict = {}
-
-    for variable in variables:
-        variable_dict[variable.name] = variable
-
-        for dim in variable.dims:
-            try:
-                dim_var = var_lookup[dim]
-                variable_dict.setdefault(dim_var.name, dim_var)
-            except KeyError:
-                # skip dimensions without coordinates like `ion`
-                pass
-
-    variables = tuple(variable_dict.values())
-
-    # Get all known variables per ids
-    grouped_ids_vars = groupby(variables, keyfunc=lambda var: var.ids)
-
-    i_tot = len(grouped_ids_vars)
-
-    for i, (ids_name, ids_vars) in enumerate(grouped_ids_vars.items()):
-        if callback:
-            callback(i / i_tot)
-
-        # Get all data, and rebase it
-        target_ids = target.get(ids_name)  # type: ignore
-
-        # Do not rebase to target if the target is empty
-        if not target_ids:
-            info('target %s:%s contains no data, skipping', target, ids_name)
-            continue
-
-        target_data = target_ids.to_xarray(variables=ids_vars,
-                                           empty_var_ok=True)
-        target_data = squash_placeholders(target_data)
-
-        ids_data = [
-            handle.get_variables(ids_vars, empty_var_ok=True)  # type: ignore
-            for handle in handles
-        ]
-
-        ids_data = rebase_all_coords(ids_data, target_data)
-        ids_data = xr.concat(ids_data, 'handle')
-
-        # Now we have to get the stddeviations
-        mean_data = ids_data.mean(dim='handle')
-        std_data = ids_data.std(dim='handle', skipna=True)
-
-        # Then, write it back to target
-        for name in ids_data.data_vars.keys():
-            path = variable_dict[name].path
-            target_ids.write_array_in_parts(path, mean_data[name])
-
-            path_upper = path + '_error_upper'
-            target_ids.write_array_in_parts(path_upper, std_data[name])
-
-        target_ids.sync(target)
+import logging
+from typing import Sequence
+
+import xarray as xr
+
+from ..config import var_lookup
+from ..operations import add_to_op_queue
+from ..schema import IDSVariableModel
+from ..utils import groupby
+from ._handle import ImasHandle
+from ._rebase import rebase_all_coords, squash_placeholders
+
+logger = logging.getLogger(__name__)
+
+info = logger.info
+
+
+@add_to_op_queue('Merging to', '{target}')
+def merge_data(
+    handles: Sequence[ImasHandle],
+    target: ImasHandle,
+    variables: list[IDSVariableModel],
+    callback=None,
+):
+    """merge_data merges the data from the handles to the target, only merges
+    over the listed variables, coordination variables are never overwritten,
+    and data is rebased according to the target coordination variable.
+
+    Parameters
+    ----------
+    handles : Sequence[ImasHandle]
+        handles
+    target : ImasHandle
+        target
+    variables : Sequence[IDSVariableModel]
+        variables
+    """
+    # Add dimensions to variables
+    variable_dict = {}
+
+    for variable in variables:
+        variable_dict[variable.name] = variable
+
+        for dim in variable.dims:
+            try:
+                dim_var = var_lookup[dim]
+                variable_dict.setdefault(dim_var.name, dim_var)
+            except KeyError:
+                # skip dimensions without coordinates like `ion`
+                pass
+
+    variables = tuple(variable_dict.values())
+
+    # Get all known variables per ids
+    grouped_ids_vars = groupby(variables, keyfunc=lambda var: var.ids)
+
+    i_tot = len(grouped_ids_vars)
+
+    for i, (ids_name, ids_vars) in enumerate(grouped_ids_vars.items()):
+        if callback:
+            callback(i / i_tot)
+
+        # Get all data, and rebase it
+        target_ids = target.get(ids_name)  # type: ignore
+
+        # Do not rebase to target if the target is empty
+        if not target_ids:
+            info('target %s:%s contains no data, skipping', target, ids_name)
+            continue
+
+        target_data = target_ids.to_xarray(variables=ids_vars,
+                                           empty_var_ok=True)
+        target_data = squash_placeholders(target_data)
+
+        ids_data = [
+            handle.get_variables(ids_vars, empty_var_ok=True)  # type: ignore
+            for handle in handles
+        ]
+
+        ids_data = rebase_all_coords(ids_data, target_data)
+        ids_data = xr.concat(ids_data, 'handle')
+
+        # Now we have to get the stddeviations
+        mean_data = ids_data.mean(dim='handle')
+        std_data = ids_data.std(dim='handle', skipna=True)
+
+        # Then, write it back to target
+        for name in ids_data.data_vars.keys():
+            path = variable_dict[name].path
+            target_ids.write_array_in_parts(path, mean_data[name])
+
+            path_upper = path + '_error_upper'
+            target_ids.write_array_in_parts(path_upper, std_data[name])
+
+        target_ids.sync(target)
```

### Comparing `duqtools-1.6.4/src/duqtools/ids/_rebase.py` & `duqtools-1.7.0/src/duqtools/ids/_rebase.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-import logging
-from typing import Optional, Sequence, Union
-
-import numpy as np
-import xarray as xr
-
-logger = logging.getLogger(__name__)
-
-
-def rezero_time(ds: xr.Dataset, *, start: int = 0) -> None:
-    """Standardize the time within a dataset by setting the first timestep to 0.
-
-    Simply subtracts time[0] from all time entries and adds `start`
-    Note: this does not interpolate the times between different datasets
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        Source dataset
-    start : int, optional
-        Where to start the returned time series
-    """
-    ds['time'] = ds['time'] - ds['time'][0] + start
-
-
-def squash_placeholders(ds: xr.Dataset) -> xr.Dataset:
-    """Squash placeholder variables. Data are grouped along the first dimension
-    (usually time).
-
-    If the data contains dimensions with a `$`-prefix,
-    these are all interpolated to the first array of that type.
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        xarray Dataset
-
-    Returns
-    -------
-    ds : xr.Dataset
-        xarray Dataset
-    """
-    prefix = '$'
-
-    dimensions = tuple(str(dim) for dim in ds.dims)
-
-    placeholder_vars = [dim for dim in dimensions if dim.startswith(prefix)]
-
-    for var in placeholder_vars:
-        new_dim = var.lstrip(prefix)
-
-        var_index = dimensions.index(var)
-        group_dims = dimensions[:var_index]
-
-        groupby = group_dims[0]
-
-        ds = standardize_grid(ds, new_dim=new_dim, old_dim=var, group=groupby)
-
-    return ds
-
-
-def standardize_grid(ds: xr.Dataset,
-                     *,
-                     new_dim: str,
-                     old_dim: str,
-                     group: Optional[str] = None,
-                     new_dim_data: Union[np.ndarray, int] = 0) -> xr.Dataset:
-    """Standardize the grid within a dataset.
-
-    Perform `split-apply-combine` routine on the data. Split
-    by the `group`, standardize the data in `new_dim` using
-    `new_dim_data` (interpolate if necessary),
-    and combine replacing `old_dim` by `new_dim`.
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        Source dataset
-    new_dim : str
-        Must be an existing variable with `group` as a dimension.
-    old_dim : str
-        Must be an existing dimension without coordinates.
-    group : str, optional
-        Split the data in groups over this dimension.
-    new_dim_data : Union[np.ndarray, int], optional
-        The data to be used for `new_dim`. If it is an integer,
-        use it as an index to grab the data from `new_dim`.
-
-    Returns
-    -------
-    xr.Dataset
-        New dataset with `new_dim` as a coordinate dimension.
-    """
-    if isinstance(new_dim_data, int):
-        new_dim_data = ds.isel(  # type: ignore
-            **{group: new_dim_data})[new_dim].data  # type:ignore
-
-    gb = ds.groupby(group)
-
-    interp_kwargs = {new_dim: new_dim_data}
-
-    def standardize(group):
-        group = group.swap_dims({old_dim: new_dim})
-        group = group.interp(**interp_kwargs)
-        return group
-
-    return gb.map(standardize)
-
-
-def rebase_on_grid(ds: xr.Dataset, *, coord_dim: str,
-                   new_coords: np.ndarray) -> xr.Dataset:
-    """Rebase (interpolate) the coordinate dimension to the new coordinates.
-
-    Thin wrapper around `xarray.Dataset.interp`.
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        Source dataset
-    coord_dim : str
-        Name of the grid dimension (i.e. grid variable).
-    new_coords : np.ndarray
-        The coordinates to interpolate to
-
-    Returns
-    -------
-    xr.Dataset
-        Rebased dataset
-    """
-    return ds.interp(coords={coord_dim: new_coords},
-                     kwargs={'fill_value': 'extrapolate'})
-
-
-def rebase_on_time(ds: xr.Dataset,
-                   *,
-                   time_dim='time',
-                   new_coords: np.ndarray) -> xr.Dataset:
-    """Rebase (interpolate) the time dimension to the new coordinates.
-
-    Thin wrapper around `xarray.Dataset.interp`.
-
-    Parameters
-    ----------
-    ds : xr.Dataset
-        Source dataset
-    time_dim : str
-        Name of the time dimension (i.e. time variable).
-    new_coords : np.ndarray
-        The coordinates to interpolate to
-
-    Returns
-    -------
-    xr.Dataset
-        Rebased dataset
-    """
-    if len(ds[time_dim]) < 2:
-        # nothing to rebase with only 1 timestep
-        return ds
-    else:
-        return rebase_on_grid(ds, coord_dim=time_dim, new_coords=new_coords)
-
-
-def standardize_grid_and_time(
-    datasets: Sequence[xr.Dataset],
-    *,
-    grid_var: str = 'rho_tor_norm',
-    time_var: str = 'time',
-    reference_dataset: int = 0,
-) -> tuple[xr.Dataset, ...]:
-    """Standardize list of datasets by applying standard rebase operations.
-
-    Applies, in sequence:
-    1. `rezero_time`
-    2. `standardize_grid`
-    3. `rebase_on_grid`
-    4. `rebase_on_time`
-
-    Parameters
-    ----------
-    datasets : Sequence[xr.Dataset]
-        List of source datasets
-    grid_var : str, optional
-        Name of the grid dimension (i.e. grid variable)
-    time_var : str, optional
-        Name of the time dimension (i.e. time variable)
-    reference_dataset : int, optional
-        The dataset with this index will be used as the reference for rebasing.
-        The grid and time coordinates of the other datasets will be rebased
-        to the reference.
-
-    Returns
-    -------
-    tuple[xr.Dataset]
-        Tuple of output datasets
-    """
-    reference_grid = datasets[reference_dataset][grid_var].data
-
-    datasets = tuple(
-        rebase_on_grid(ds, coord_dim=grid_var, new_coords=reference_grid)
-        for ds in datasets)
-
-    reference_time = datasets[reference_dataset][time_var].data
-
-    datasets = tuple(
-        rebase_on_time(ds, time_dim=time_var, new_coords=reference_time)
-        for ds in datasets)
-
-    return datasets
-
-
-def rebase_all_coords(
-    datasets: Sequence[xr.Dataset],
-    reference_dataset: xr.Dataset,
-) -> tuple[xr.Dataset, ...]:
-    """Rebase all coords, by applying rebase operations.
-
-    Parameters
-    ----------
-    datasets : Sequence[xr.Dataset]
-        datasets
-    reference_dataset : xr.Dataset
-        reference_dataset
-
-    Returns
-    -------
-    tuple[xr.Dataset, ...]
-    """
-
-    interp_dict = {
-        name: dim
-        for name, dim in reference_dataset.coords.items() if dim.size > 1
-    }
-
-    return tuple(
-        ds.interp(coords=interp_dict, kwargs={'fill_value': 'extrapolate'})
-        for ds in datasets)
+import logging
+from typing import Optional, Sequence, Union
+
+import numpy as np
+import xarray as xr
+
+logger = logging.getLogger(__name__)
+
+
+def rezero_time(ds: xr.Dataset, *, start: int = 0) -> None:
+    """Standardize the time within a dataset by setting the first timestep to 0.
+
+    Simply subtracts time[0] from all time entries and adds `start`
+    Note: this does not interpolate the times between different datasets
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        Source dataset
+    start : int, optional
+        Where to start the returned time series
+    """
+    ds['time'] = ds['time'] - ds['time'][0] + start
+
+
+def squash_placeholders(ds: xr.Dataset) -> xr.Dataset:
+    """Squash placeholder variables. Data are grouped along the first dimension
+    (usually time).
+
+    If the data contains dimensions with a `$`-prefix,
+    these are all interpolated to the first array of that type.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        xarray Dataset
+
+    Returns
+    -------
+    ds : xr.Dataset
+        xarray Dataset
+    """
+    prefix = '$'
+
+    dimensions = tuple(str(dim) for dim in ds.dims)
+
+    placeholder_vars = [dim for dim in dimensions if dim.startswith(prefix)]
+
+    for var in placeholder_vars:
+        new_dim = var.lstrip(prefix)
+
+        var_index = dimensions.index(var)
+        group_dims = dimensions[:var_index]
+
+        groupby = group_dims[0]
+
+        ds = standardize_grid(ds, new_dim=new_dim, old_dim=var, group=groupby)
+
+    return ds
+
+
+def standardize_grid(ds: xr.Dataset,
+                     *,
+                     new_dim: str,
+                     old_dim: str,
+                     group: Optional[str] = None,
+                     new_dim_data: Union[np.ndarray, int] = 0) -> xr.Dataset:
+    """Standardize the grid within a dataset.
+
+    Perform `split-apply-combine` routine on the data. Split
+    by the `group`, standardize the data in `new_dim` using
+    `new_dim_data` (interpolate if necessary),
+    and combine replacing `old_dim` by `new_dim`.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        Source dataset
+    new_dim : str
+        Must be an existing variable with `group` as a dimension.
+    old_dim : str
+        Must be an existing dimension without coordinates.
+    group : str, optional
+        Split the data in groups over this dimension.
+    new_dim_data : Union[np.ndarray, int], optional
+        The data to be used for `new_dim`. If it is an integer,
+        use it as an index to grab the data from `new_dim`.
+
+    Returns
+    -------
+    xr.Dataset
+        New dataset with `new_dim` as a coordinate dimension.
+    """
+    if isinstance(new_dim_data, int):
+        new_dim_data = ds.isel(  # type: ignore
+            **{group: new_dim_data})[new_dim].data  # type:ignore
+
+    gb = ds.groupby(group)
+
+    interp_kwargs = {new_dim: new_dim_data}
+
+    def standardize(group):
+        group = group.swap_dims({old_dim: new_dim})
+        group = group.interp(**interp_kwargs)
+        return group
+
+    return gb.map(standardize)
+
+
+def rebase_on_grid(ds: xr.Dataset, *, coord_dim: str,
+                   new_coords: np.ndarray) -> xr.Dataset:
+    """Rebase (interpolate) the coordinate dimension to the new coordinates.
+
+    Thin wrapper around `xarray.Dataset.interp`.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        Source dataset
+    coord_dim : str
+        Name of the grid dimension (i.e. grid variable).
+    new_coords : np.ndarray
+        The coordinates to interpolate to
+
+    Returns
+    -------
+    xr.Dataset
+        Rebased dataset
+    """
+    return ds.interp(coords={coord_dim: new_coords},
+                     kwargs={'fill_value': 'extrapolate'})
+
+
+def rebase_on_time(ds: xr.Dataset,
+                   *,
+                   time_dim='time',
+                   new_coords: np.ndarray) -> xr.Dataset:
+    """Rebase (interpolate) the time dimension to the new coordinates.
+
+    Thin wrapper around `xarray.Dataset.interp`.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        Source dataset
+    time_dim : str
+        Name of the time dimension (i.e. time variable).
+    new_coords : np.ndarray
+        The coordinates to interpolate to
+
+    Returns
+    -------
+    xr.Dataset
+        Rebased dataset
+    """
+    if len(ds[time_dim]) < 2:
+        # nothing to rebase with only 1 timestep
+        return ds
+    else:
+        return rebase_on_grid(ds, coord_dim=time_dim, new_coords=new_coords)
+
+
+def standardize_grid_and_time(
+    datasets: Sequence[xr.Dataset],
+    *,
+    grid_var: str = 'rho_tor_norm',
+    time_var: str = 'time',
+    reference_dataset: int = 0,
+) -> tuple[xr.Dataset, ...]:
+    """Standardize list of datasets by applying standard rebase operations.
+
+    Applies, in sequence:
+    1. `rezero_time`
+    2. `standardize_grid`
+    3. `rebase_on_grid`
+    4. `rebase_on_time`
+
+    Parameters
+    ----------
+    datasets : Sequence[xr.Dataset]
+        List of source datasets
+    grid_var : str, optional
+        Name of the grid dimension (i.e. grid variable)
+    time_var : str, optional
+        Name of the time dimension (i.e. time variable)
+    reference_dataset : int, optional
+        The dataset with this index will be used as the reference for rebasing.
+        The grid and time coordinates of the other datasets will be rebased
+        to the reference.
+
+    Returns
+    -------
+    tuple[xr.Dataset]
+        Tuple of output datasets
+    """
+    reference_grid = datasets[reference_dataset][grid_var].data
+
+    datasets = tuple(
+        rebase_on_grid(ds, coord_dim=grid_var, new_coords=reference_grid)
+        for ds in datasets)
+
+    reference_time = datasets[reference_dataset][time_var].data
+
+    datasets = tuple(
+        rebase_on_time(ds, time_dim=time_var, new_coords=reference_time)
+        for ds in datasets)
+
+    return datasets
+
+
+def rebase_all_coords(
+    datasets: Sequence[xr.Dataset],
+    reference_dataset: xr.Dataset,
+) -> tuple[xr.Dataset, ...]:
+    """Rebase all coords, by applying rebase operations.
+
+    Parameters
+    ----------
+    datasets : Sequence[xr.Dataset]
+        datasets
+    reference_dataset : xr.Dataset
+        reference_dataset
+
+    Returns
+    -------
+    tuple[xr.Dataset, ...]
+    """
+
+    interp_dict = {
+        name: dim
+        for name, dim in reference_dataset.coords.items() if dim.size > 1
+    }
+
+    return tuple(
+        ds.interp(coords=interp_dict, kwargs={'fill_value': 'extrapolate'})
+        for ds in datasets)
```

### Comparing `duqtools-1.6.4/src/duqtools/init.py` & `duqtools-1.7.0/src/duqtools/init.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import logging
-import shutil
-import sys
-from pathlib import Path
-
-from .operations import op_queue
-
-if sys.version_info < (3, 10):
-    from importlib_resources import files
-else:
-    from importlib.resources import files
-
-logger = logging.getLogger(__name__)
-
-
-def init(*, out_file: str, force: bool, **kwargs):
-    """Initialize a brand new config file with all the default values.
-
-    Parameters
-    ----------
-    out : str
-        Filename of the config.
-    force : bool
-        Overwrite config if it already exists.
-    **kwargs
-        Unused.
-
-    Raises
-    ------
-    RuntimeError
-        When the config already exists.
-    """
-    src = files('duqtools.data') / 'duqtools.yaml'
-
-    config_filepath = Path(out_file)
-
-    if config_filepath.exists() and not force:
-        raise RuntimeError(
-            f'Refusing to overwrite existing CONFIG, {config_filepath}, '
-            'use --force if you really want to')
-
-    logger.debug('Copying default config from %s to %s', src, config_filepath)
-
-    op_queue.add(action=shutil.copy,
-                 kwargs={
-                     'src': src,
-                     'dst': config_filepath,
-                 },
-                 description='Copying config to',
-                 extra_description=f'{config_filepath}')
+import logging
+import shutil
+import sys
+from pathlib import Path
+
+from .operations import op_queue
+
+if sys.version_info < (3, 10):
+    from importlib_resources import files
+else:
+    from importlib.resources import files
+
+logger = logging.getLogger(__name__)
+
+
+def init(*, out_file: str, force: bool, **kwargs):
+    """Initialize a brand new config file with all the default values.
+
+    Parameters
+    ----------
+    out : str
+        Filename of the config.
+    force : bool
+        Overwrite config if it already exists.
+    **kwargs
+        Unused.
+
+    Raises
+    ------
+    RuntimeError
+        When the config already exists.
+    """
+    src = files('duqtools.data') / 'duqtools.yaml'
+
+    config_filepath = Path(out_file)
+
+    if config_filepath.exists() and not force:
+        raise RuntimeError(
+            f'Refusing to overwrite existing CONFIG, {config_filepath}, '
+            'use --force if you really want to')
+
+    logger.debug('Copying default config from %s to %s', src, config_filepath)
+
+    op_queue.add(action=shutil.copy,
+                 kwargs={
+                     'src': src,
+                     'dst': config_filepath,
+                 },
+                 description='Copying config to',
+                 extra_description=f'{config_filepath}')
```

### Comparing `duqtools-1.6.4/src/duqtools/jetto/_jettovar_to_json.py` & `duqtools-1.7.0/src/duqtools/jetto/_jettovar_to_json.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import json
-
-from ..schema import JettoVar, JsetField, NamelistField
-
-
-def jettovar_to_json(variable: JettoVar):
-    jsetfields = []
-    nmlfields = []
-    for field in variable.keys:
-        if isinstance(field, JsetField):
-            jsetfields.append(field)
-        elif isinstance(field, NamelistField):
-            nmlfields.append(field)
-        else:
-            raise NotImplementedError(f'unknown Jetto field type {field}')
-
-    if len(nmlfields) > 1:
-        raise RuntimeError(
-            f'jetto_tools only support a single nml entry: {nmlfields}')
-
-    var_dict = {'type': variable.type, 'dimension': 'scalar'}
-    if var_dict['type'] == 'float':
-        var_dict['type'] = 'real'
-
-    if len(jsetfields) > 0:
-        var_dict['jset_id'] = jsetfields[0].field
-    if len(jsetfields) > 1:
-        var_dict['jset_flex_id'] = []  # type: ignore
-        for field in jsetfields[1:]:
-            var_dict['jset_flex_id'].append(field.field)  # type: ignore
-
-    if len(nmlfields) == 1:
-        var_dict['nml_id'] = {  # type: ignore
-            'namelist': nmlfields[0].section,
-            'field': nmlfields[0].field
-        }
-
-    return json.dumps({variable.name: var_dict})
+import json
+
+from ..schema import JettoVar, JsetField, NamelistField
+
+
+def jettovar_to_json(variable: JettoVar):
+    jsetfields = []
+    nmlfields = []
+    for field in variable.keys:
+        if isinstance(field, JsetField):
+            jsetfields.append(field)
+        elif isinstance(field, NamelistField):
+            nmlfields.append(field)
+        else:
+            raise NotImplementedError(f'unknown Jetto field type {field}')
+
+    if len(nmlfields) > 1:
+        raise RuntimeError(
+            f'jetto_tools only support a single nml entry: {nmlfields}')
+
+    var_dict = {'type': variable.type, 'dimension': 'scalar'}
+    if var_dict['type'] == 'float':
+        var_dict['type'] = 'real'
+
+    if len(jsetfields) > 0:
+        var_dict['jset_id'] = jsetfields[0].field
+    if len(jsetfields) > 1:
+        var_dict['jset_flex_id'] = []  # type: ignore
+        for field in jsetfields[1:]:
+            var_dict['jset_flex_id'].append(field.field)  # type: ignore
+
+    if len(nmlfields) == 1:
+        var_dict['nml_id'] = {  # type: ignore
+            'namelist': nmlfields[0].section,
+            'field': nmlfields[0].field
+        }
+
+    return json.dumps({variable.name: var_dict})
```

### Comparing `duqtools-1.6.4/src/duqtools/large_scale_validation/cli.py` & `duqtools-1.7.0/src/duqtools/large_scale_validation/cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import logging
-
-import click
-
-from ..cli import common_options, dry_run_option, logging_options, variables_option, yes_option
-from ..operations import op_queue_context
-
-logger = logging.getLogger(__name__)
-
-try:
-    import coverage
-    coverage.process_startup()
-except ImportError:
-    pass
-
-
-def cli_entry():
-    from duqtools import fix_dependencies
-    fix_dependencies()
-    cli()
-
-
-@click.group()
-def cli(**kwargs):
-    """For more information, check out the documentation:
-
-    https://duqtools.readthedocs.io/large_scale_validation
-    """
-
-
-@cli.command('setup')
-@click.option(
-    '-i',
-    '--input',
-    'input_file',
-    type=click.Path(exists=True),
-    help='Input file, i.e. `data.csv` or `runs.yaml`',
-    default='data.csv',
-)
-@click.option(
-    '-t',
-    '--template',
-    'template_file',
-    type=click.Path(exists=True),
-    help='Template duqtools.yaml',
-    default='duqtools.template.yaml',
-)
-@click.option('--force',
-              is_flag=True,
-              help='Overwrite existing run config directories')
-@common_options(*logging_options, yes_option, dry_run_option)
-def cli_setup(**kwargs):
-    """Set up large scale validation."""
-    from .setup import setup
-    with op_queue_context():
-        setup(**kwargs)
-
-
-@cli.command('create')
-@click.option('--force',
-              is_flag=True,
-              help='Overwrite existing run directories and IDS data.')
-@common_options(*logging_options, yes_option, dry_run_option)
-def cli_create(**kwargs):
-    """Create data sets for large scale validation."""
-    from .create import create
-    with op_queue_context():
-        create(**kwargs)
-
-
-@cli.command('submit')
-@click.option('--force',
-              is_flag=True,
-              help='Re-submit running or completed jobs.')
-@click.option(
-    '--schedule',
-    is_flag=True,
-    help='Schedule and submit jobs automatically. `max_jobs` must be defined.')
-@click.option('-j',
-              '--max_jobs',
-              type=int,
-              help='Maximum number of jobs to submit.')
-@click.option('-s',
-              '--status',
-              'status_filter',
-              type=str,
-              multiple=True,
-              help='Only submit jobs with this status.')
-@click.option('-a', '--array', is_flag=True, help='Submit jobs as array.')
-@common_options(*logging_options, yes_option, dry_run_option)
-def cli_submit(**kwargs):
-    """Submit large scale validation runs."""
-    from .submit import submit
-    with op_queue_context():
-        submit(**kwargs)
-
-
-@cli.command('status')
-@click.option('--detailed', is_flag=True, help='Detailed info on progress')
-@click.option('--progress', is_flag=True, help='Fancy progress bar')
-@common_options(*logging_options)
-def cli_status(**kwargs):
-    """Check status large scale validation runs."""
-    from .status import status
-    with op_queue_context():
-        status(**kwargs)
-
-
-@cli.command('merge')
-@click.option('--force', is_flag=True, help='Overwrite existing data')
-@variables_option
-@common_options(*logging_options, yes_option, dry_run_option)
-def cli_merge(**kwargs):
-    """Merge data sets with error propagation.
-
-    By default, `duqduq merge` attempts to merge all known variables.
-    Use `--variable` to select which variables to merge.
-    """
-    from .merge import merge
-    with op_queue_context():
-        merge(**kwargs)
+import logging
+
+import click
+
+from ..cli import common_options, dry_run_option, logging_options, variables_option, yes_option
+from ..operations import op_queue_context
+
+logger = logging.getLogger(__name__)
+
+try:
+    import coverage
+    coverage.process_startup()
+except ImportError:
+    pass
+
+
+def cli_entry():
+    from duqtools import fix_dependencies
+    fix_dependencies()
+    cli()
+
+
+@click.group()
+def cli(**kwargs):
+    """For more information, check out the documentation:
+
+    https://duqtools.readthedocs.io/large_scale_validation
+    """
+
+
+@cli.command('setup')
+@click.option(
+    '-i',
+    '--input',
+    'input_file',
+    type=click.Path(exists=True),
+    help='Input file, i.e. `data.csv` or `runs.yaml`',
+    default='data.csv',
+)
+@click.option(
+    '-t',
+    '--template',
+    'template_file',
+    type=click.Path(exists=True),
+    help='Template duqtools.yaml',
+    default='duqtools.template.yaml',
+)
+@click.option('--force',
+              is_flag=True,
+              help='Overwrite existing run config directories')
+@common_options(*logging_options, yes_option, dry_run_option)
+def cli_setup(**kwargs):
+    """Set up large scale validation."""
+    from .setup import setup
+    with op_queue_context():
+        setup(**kwargs)
+
+
+@cli.command('create')
+@click.option('--force',
+              is_flag=True,
+              help='Overwrite existing run directories and IDS data.')
+@common_options(*logging_options, yes_option, dry_run_option)
+def cli_create(**kwargs):
+    """Create data sets for large scale validation."""
+    from .create import create
+    with op_queue_context():
+        create(**kwargs)
+
+
+@cli.command('submit')
+@click.option('--force',
+              is_flag=True,
+              help='Re-submit running or completed jobs.')
+@click.option(
+    '--schedule',
+    is_flag=True,
+    help='Schedule and submit jobs automatically. `max_jobs` must be defined.')
+@click.option('-j',
+              '--max_jobs',
+              type=int,
+              help='Maximum number of jobs to submit.')
+@click.option('-s',
+              '--status',
+              'status_filter',
+              type=str,
+              multiple=True,
+              help='Only submit jobs with this status.')
+@click.option('-a', '--array', is_flag=True, help='Submit jobs as array.')
+@common_options(*logging_options, yes_option, dry_run_option)
+def cli_submit(**kwargs):
+    """Submit large scale validation runs."""
+    from .submit import submit
+    with op_queue_context():
+        submit(**kwargs)
+
+
+@cli.command('status')
+@click.option('--detailed', is_flag=True, help='Detailed info on progress')
+@click.option('--progress', is_flag=True, help='Fancy progress bar')
+@common_options(*logging_options)
+def cli_status(**kwargs):
+    """Check status large scale validation runs."""
+    from .status import status
+    with op_queue_context():
+        status(**kwargs)
+
+
+@cli.command('merge')
+@click.option('--force', is_flag=True, help='Overwrite existing data')
+@variables_option
+@common_options(*logging_options, yes_option, dry_run_option)
+def cli_merge(**kwargs):
+    """Merge data sets with error propagation.
+
+    By default, `duqduq merge` attempts to merge all known variables.
+    Use `--variable` to select which variables to merge.
+    """
+    from .merge import merge
+    with op_queue_context():
+        merge(**kwargs)
```

### Comparing `duqtools-1.6.4/src/duqtools/large_scale_validation/create.py` & `duqtools-1.7.0/src/duqtools/large_scale_validation/create.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from pathlib import Path
-
-from ..config import cfg
-from ..create import create as duqtools_create
-from ..utils import work_directory
-
-
-def create(**kwargs):
-    cwd = Path.cwd()
-
-    config_files = cwd.glob('**/duqtools.yaml')
-
-    for config_file in config_files:
-        cfg.parse_file(config_file)
-
-        config_dir = config_file.parent
-
-        with work_directory(config_dir):
-            duqtools_create(config=config_file,
-                            absolute_dirpath=True,
-                            **kwargs)
+from pathlib import Path
+
+from ..config import cfg
+from ..create import create as duqtools_create
+from ..utils import work_directory
+
+
+def create(**kwargs):
+    cwd = Path.cwd()
+
+    config_files = cwd.glob('**/duqtools.yaml')
+
+    for config_file in config_files:
+        cfg.parse_file(config_file)
+
+        config_dir = config_file.parent
+
+        with work_directory(config_dir):
+            duqtools_create(config=config_file,
+                            absolute_dirpath=True,
+                            **kwargs)
```

### Comparing `duqtools-1.6.4/src/duqtools/large_scale_validation/merge.py` & `duqtools-1.7.0/src/duqtools/large_scale_validation/merge.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import logging
-from pathlib import Path
-from typing import Sequence
-
-import pandas as pd
-
-from duqtools.api import ImasHandle
-
-from ..config import cfg
-from ..merge import _merge, _resolve_variables
-from ..models import Job, Locations
-from ..operations import add_to_op_queue, op_queue
-
-logger = logging.getLogger(__name__)
-
-
-@add_to_op_queue('Writing csv', '{fname}')
-def _write_data_csv(handles: dict[str, ImasHandle], fname: str = 'data.csv'):
-    """Write handles to a data.csv file."""
-    df = pd.DataFrame.from_dict(handles, orient='index')
-    df.to_csv(fname)
-
-
-def merge(force: bool, var_names: Sequence[str], **kwargs):
-    cwd = Path.cwd()
-
-    variables = _resolve_variables(var_names)
-
-    config_files = cwd.glob('**/duqtools.yaml')
-
-    target_handles = {}
-
-    for config_file in config_files:
-        run_name = config_file.parent.name
-
-        cfg.parse_file(config_file)
-
-        config_dir = config_file.parent
-
-        runs = Locations(config_dir).runs
-        runs = (run for run in runs if Job(run.dirname).is_completed)
-        handles = (ImasHandle.parse_obj(run.data_out) for run in runs)
-        handles = [handle for handle in handles if handle.exists()]
-
-        if not handles:
-            op_queue.warning(run_name, 'No data to merge.')
-            continue
-
-        op_queue.info(run_name,
-                      extra_description=f'Merging {len(handles)} datasets')
-
-        template_data = handles[0]
-
-        target_data = template_data.copy()
-        target_data.user = str(cfg.create.runs_dir / 'imasdb')
-        target_handles[f'{run_name}_merged'] = target_data.dict()
-
-        _merge(
-            variables=variables,
-            handles=handles,
-            target=target_data,
-            template=template_data,
-            force=force,
-        )
-
-    _write_data_csv(target_handles, fname='merge_data.csv')
+import logging
+from pathlib import Path
+from typing import Sequence
+
+import pandas as pd
+
+from duqtools.api import ImasHandle
+
+from ..config import cfg
+from ..merge import _merge, _resolve_variables
+from ..models import Job, Locations
+from ..operations import add_to_op_queue, op_queue
+
+logger = logging.getLogger(__name__)
+
+
+@add_to_op_queue('Writing csv', '{fname}')
+def _write_data_csv(handles: dict[str, ImasHandle], fname: str = 'data.csv'):
+    """Write handles to a data.csv file."""
+    df = pd.DataFrame.from_dict(handles, orient='index')
+    df.to_csv(fname)
+
+
+def merge(force: bool, var_names: Sequence[str], **kwargs):
+    cwd = Path.cwd()
+
+    variables = _resolve_variables(var_names)
+
+    config_files = cwd.glob('**/duqtools.yaml')
+
+    target_handles = {}
+
+    for config_file in config_files:
+        run_name = config_file.parent.name
+
+        cfg.parse_file(config_file)
+
+        config_dir = config_file.parent
+
+        runs = Locations(config_dir).runs
+        runs = (run for run in runs if Job(run.dirname).is_completed)
+        handles = (ImasHandle.parse_obj(run.data_out) for run in runs)
+        handles = [handle for handle in handles if handle.exists()]
+
+        if not handles:
+            op_queue.warning(run_name, 'No data to merge.')
+            continue
+
+        op_queue.info(run_name,
+                      extra_description=f'Merging {len(handles)} datasets')
+
+        template_data = handles[0]
+
+        target_data = template_data.copy()
+        target_data.user = str(cfg.create.runs_dir / 'imasdb')
+        target_handles[f'{run_name}_merged'] = target_data.dict()
+
+        _merge(
+            variables=variables,
+            handles=handles,
+            target=target_data,
+            template=template_data,
+            force=force,
+        )
+
+    _write_data_csv(target_handles, fname='merge_data.csv')
```

### Comparing `duqtools-1.6.4/src/duqtools/list_variables.py` & `duqtools-1.7.0/src/duqtools/list_variables.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import click
-from pydantic import ValidationError
-
-from duqtools.config import cfg, var_lookup
-
-cs = click.style
-
-ST_ITEMS = {'fg': 'green', 'bold': True}
-ST_HEADER = {'fg': 'red', 'bold': True}
-ST_INFO = {'fg': 'white', 'bold': False}
-
-
-def list_group(group: list, extra_variables: dict):
-    group = sorted(group, key=lambda var: var.name)
-
-    for var in group:
-        star = cs('*', **ST_HEADER) if var.name in extra_variables else ''
-
-        name = cs(f'{var.name}', **ST_ITEMS)
-
-        try:
-            sub = cs(f'({var.path})', **ST_INFO)
-        except AttributeError:
-            sub = cs(f'({var.type})', **ST_INFO)
-
-        click.echo(f'    - {star}{name} {sub}')
-
-
-def list_variables(*, config, **kwargs):
-    """List variables in `variables.yaml` and config/`duqtools.yaml` if
-    present.
-
-    Parameters
-    ----------
-    config : str
-        Name of the config file to use
-    **kwargs
-        Unused.
-    """
-    try:
-        cfg.parse_file(config)
-    except FileNotFoundError:
-        print(f'Could not find: {config}')
-    except ValidationError as e:
-        exit(e)
-        print(f'*: defined by {config}')
-    finally:
-        extra_variables = cfg.extra_variables.to_variable_dict(
-        ) if cfg.extra_variables else {}
-
-    grouped_ids_vars = var_lookup.groupby_ids()
-
-    for root_ids, group in grouped_ids_vars.items():
-        click.secho(f'\nIDS-variable - {root_ids}:', **ST_HEADER)
-        list_group(group, extra_variables)
-
-    grouped_other_vars = var_lookup.groupby_type()
-    grouped_other_vars.pop('IDS-variable')
-
-    for var_type, group in grouped_other_vars.items():
-        click.secho(f'\n{var_type}:', **ST_HEADER)
-        list_group(group, extra_variables)
+import click
+from pydantic import ValidationError
+
+from duqtools.config import cfg, var_lookup
+
+cs = click.style
+
+ST_ITEMS = {'fg': 'green', 'bold': True}
+ST_HEADER = {'fg': 'red', 'bold': True}
+ST_INFO = {'fg': 'white', 'bold': False}
+
+
+def list_group(group: list, extra_variables: dict):
+    group = sorted(group, key=lambda var: var.name)
+
+    for var in group:
+        star = cs('*', **ST_HEADER) if var.name in extra_variables else ''
+
+        name = cs(f'{var.name}', **ST_ITEMS)
+
+        try:
+            sub = cs(f'({var.path})', **ST_INFO)
+        except AttributeError:
+            sub = cs(f'({var.type})', **ST_INFO)
+
+        click.echo(f'    - {star}{name} {sub}')
+
+
+def list_variables(*, config, **kwargs):
+    """List variables in `variables.yaml` and config/`duqtools.yaml` if
+    present.
+
+    Parameters
+    ----------
+    config : str
+        Name of the config file to use
+    **kwargs
+        Unused.
+    """
+    try:
+        cfg.parse_file(config)
+    except FileNotFoundError:
+        print(f'Could not find: {config}')
+    except ValidationError as e:
+        exit(e)
+        print(f'*: defined by {config}')
+    finally:
+        extra_variables = cfg.extra_variables.to_variable_dict(
+        ) if cfg.extra_variables else {}
+
+    grouped_ids_vars = var_lookup.groupby_ids()
+
+    for root_ids, group in grouped_ids_vars.items():
+        click.secho(f'\nIDS-variable - {root_ids}:', **ST_HEADER)
+        list_group(group, extra_variables)
+
+    grouped_other_vars = var_lookup.groupby_type()
+    grouped_other_vars.pop('IDS-variable')
+
+    for var_type, group in grouped_other_vars.items():
+        click.secho(f'\n{var_type}:', **ST_HEADER)
+        list_group(group, extra_variables)
```

### Comparing `duqtools-1.6.4/src/duqtools/matrix_samplers.py` & `duqtools-1.7.0/src/duqtools/matrix_samplers.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import itertools
-from typing import Optional
-
-from scipy.stats import qmc
-
-
-def cartesian_product(*iterables, **kwargs):
-    """Return cartesian product of input iterables.
-
-    Uses `itertools.product`
-
-    Parameters
-    ----------
-    *iterables
-        Input iterables.
-
-    Returns
-    -------
-    list[Any]
-        List of product of input arguments.
-    """
-    return list(itertools.product(*iterables))
-
-
-def _sampler(func, *iterables, n_samples: int, **kwargs):
-    """Generic sampler."""
-    bounds = tuple(len(iterable) for iterable in iterables)
-
-    sampler = func(d=len(iterables), **kwargs)
-    indices = sampler.integers(l_bounds=bounds, n=n_samples)
-
-    samples = []
-    for row in indices:
-        samples.append(tuple(arg[col] for col, arg in zip(row, iterables)))
-
-    return samples
-
-
-def latin_hypercube(*iterables,
-                    n_samples: int,
-                    seed: Optional[int] = None,
-                    **kwargs):
-    """Sample input iterables using Latin hypercube sampling (LHS).
-
-    Uses `scipy.stats.qmc.LatinHyperCube`.
-
-    Parameters
-    ----------
-    *iterables
-        Iterables to sample from.
-    n_samples : int
-        Number of samples to return.
-    seed : int, optional
-        Seed to use for the randomizer
-
-    Returns
-    -------
-    samples : list[Any]
-        List of sampled input arguments.
-    """
-    return _sampler(qmc.LatinHypercube,
-                    *iterables,
-                    n_samples=n_samples,
-                    seed=seed)
-
-
-def sobol(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
-    """Sample input iterables using the Sobol sampling method for generating
-    low discrepancy sequences.
-
-    Uses `scipy.stats.qmc.Sobol`.
-
-    Parameters
-    ----------
-    *iterables
-        Iterables to sample from.
-    n_samples : int
-        Number of samples to return. Note that Sobol sequences lose their
-        balance  properties if one uses a sample size that is not a power
-        of two.
-    seed : int, optional
-        Seed to use for the randomizer
-
-    Returns
-    -------
-    samples : list[Any]
-        List of sampled input arguments.
-    """
-    return _sampler(qmc.Sobol, *iterables, n_samples=n_samples, seed=seed)
-
-
-def halton(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
-    """Sample input iterables using the Halton sampling method.
-
-    Uses `scipy.stats.qmc.Halton`.
-
-    Parameters
-    ----------
-    *iterables
-        Iterables to sample from.
-    n_samples : int
-        Number of samples to return.
-    seed : int, optional
-        Seed to use for the randomizer
-
-    Returns
-    -------
-    samples : list[Any]
-        List of sampled input arguments.
-    """
-    return _sampler(qmc.Halton, *iterables, n_samples=n_samples, seed=seed)
-
-
-_SAMPLERS = {
-    'latin-hypercube': latin_hypercube,
-    'halton': halton,
-    'sobol': sobol,
-    'low-discrepancy-sequence': sobol,
-    'cartesian-product': cartesian_product,
-}
-
-
-def get_matrix_sampler(name: str):
-    """Get sampler.
-
-    Parameters
-    ----------
-    name : str
-        Name of the sampler.
-
-    Returns
-    -------
-    Callable
-        Sampling function.
-    """
-    return _SAMPLERS[name]
+import itertools
+from typing import Optional
+
+from scipy.stats import qmc
+
+
+def cartesian_product(*iterables, **kwargs):
+    """Return cartesian product of input iterables.
+
+    Uses `itertools.product`
+
+    Parameters
+    ----------
+    *iterables
+        Input iterables.
+
+    Returns
+    -------
+    list[Any]
+        List of product of input arguments.
+    """
+    return list(itertools.product(*iterables))
+
+
+def _sampler(func, *iterables, n_samples: int, **kwargs):
+    """Generic sampler."""
+    bounds = tuple(len(iterable) for iterable in iterables)
+
+    sampler = func(d=len(iterables), **kwargs)
+    indices = sampler.integers(l_bounds=bounds, n=n_samples)
+
+    samples = []
+    for row in indices:
+        samples.append(tuple(arg[col] for col, arg in zip(row, iterables)))
+
+    return samples
+
+
+def latin_hypercube(*iterables,
+                    n_samples: int,
+                    seed: Optional[int] = None,
+                    **kwargs):
+    """Sample input iterables using Latin hypercube sampling (LHS).
+
+    Uses `scipy.stats.qmc.LatinHyperCube`.
+
+    Parameters
+    ----------
+    *iterables
+        Iterables to sample from.
+    n_samples : int
+        Number of samples to return.
+    seed : int, optional
+        Seed to use for the randomizer
+
+    Returns
+    -------
+    samples : list[Any]
+        List of sampled input arguments.
+    """
+    return _sampler(qmc.LatinHypercube,
+                    *iterables,
+                    n_samples=n_samples,
+                    seed=seed)
+
+
+def sobol(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
+    """Sample input iterables using the Sobol sampling method for generating
+    low discrepancy sequences.
+
+    Uses `scipy.stats.qmc.Sobol`.
+
+    Parameters
+    ----------
+    *iterables
+        Iterables to sample from.
+    n_samples : int
+        Number of samples to return. Note that Sobol sequences lose their
+        balance  properties if one uses a sample size that is not a power
+        of two.
+    seed : int, optional
+        Seed to use for the randomizer
+
+    Returns
+    -------
+    samples : list[Any]
+        List of sampled input arguments.
+    """
+    return _sampler(qmc.Sobol, *iterables, n_samples=n_samples, seed=seed)
+
+
+def halton(*iterables, n_samples: int, seed: Optional[int] = None, **kwargs):
+    """Sample input iterables using the Halton sampling method.
+
+    Uses `scipy.stats.qmc.Halton`.
+
+    Parameters
+    ----------
+    *iterables
+        Iterables to sample from.
+    n_samples : int
+        Number of samples to return.
+    seed : int, optional
+        Seed to use for the randomizer
+
+    Returns
+    -------
+    samples : list[Any]
+        List of sampled input arguments.
+    """
+    return _sampler(qmc.Halton, *iterables, n_samples=n_samples, seed=seed)
+
+
+_SAMPLERS = {
+    'latin-hypercube': latin_hypercube,
+    'halton': halton,
+    'sobol': sobol,
+    'low-discrepancy-sequence': sobol,
+    'cartesian-product': cartesian_product,
+}
+
+
+def get_matrix_sampler(name: str):
+    """Get sampler.
+
+    Parameters
+    ----------
+    name : str
+        Name of the sampler.
+
+    Returns
+    -------
+    Callable
+        Sampling function.
+    """
+    return _SAMPLERS[name]
```

### Comparing `duqtools-1.6.4/src/duqtools/merge.py` & `duqtools-1.7.0/src/duqtools/merge.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from __future__ import annotations
-
-import logging
-from typing import Sequence
-
-from .config import var_lookup
-from .ids import ImasHandle, merge_data
-from .operations import op_queue
-from .schema import IDSVariableModel
-from .utils import read_imas_handles_from_file
-
-logger = logging.getLogger(__name__)
-info, debug = logger.info, logger.debug
-
-
-def _resolve_variables(var_names: Sequence[str]) -> list[IDSVariableModel]:
-    """Looks up variables if specified, if empty return all variables."""
-    idsvar_lookup = var_lookup.filter_type('IDS-variable')
-
-    if not var_names:
-        variables = list(idsvar_lookup.values())
-        op_queue.info(description='Merging all known variables')
-    else:
-        variables = list(idsvar_lookup[name] for name in var_names)
-        for variable in variables:
-            op_queue.info(description='Variable for merge',
-                          extra_description=f'{variable.name}')
-
-    return variables
-
-
-def _merge(*,
-           handles: Sequence[ImasHandle],
-           template: ImasHandle,
-           target: ImasHandle,
-           variables: Sequence[IDSVariableModel],
-           force: bool = False):
-    """Merge mas data.
-
-    Parameters
-    ----------
-    handles : Sequence[ImasHandle]
-        These are the imas handles that will be merged.
-    template : ImasHandle
-        This handle is the template that is used for the new data.
-    target : ImasHandle
-        This handle is the target location where the merged data will be stored.
-    variables : Sequence[Variable
-        These are the IDS variables to be merged.
-    force : bool
-        Force overwriting existing files.
-    """
-    for handle in handles:
-        logger.debug('Source for merge %s', handle)
-
-    op_queue.info(description='Template for merge',
-                  extra_description=f'{template}')
-
-    if target.exists() and not force:
-        op_queue.add_no_op(description='Abort merge',
-                           extra_description=f'{target} already exists, '
-                           'use --force to overwrite')
-        return
-
-    template.copy_data_to(target)
-
-    merge_data(handles, target, variables)
-
-
-def merge(*, target: str, template: str, handles: list[str],
-          input_files: list[str], var_names: list[str], force: bool, **kwargs):
-    """Merge as many data as possible."""
-    template = ImasHandle.from_string(template)
-    target = ImasHandle.from_string(target)
-
-    handles = [ImasHandle.from_string(handle) for handle in handles]
-    for file in input_files:
-        handles = handles + list(read_imas_handles_from_file(file).values())
-
-    handles = list(set(handles))  # Remove duplicate handles
-
-    variables = _resolve_variables(var_names)
-
-    _merge(
-        handles=handles,
-        template=template,
-        target=target,
-        variables=variables,
-    )
+from __future__ import annotations
+
+import logging
+from typing import Sequence
+
+from .config import var_lookup
+from .ids import ImasHandle, merge_data
+from .operations import op_queue
+from .schema import IDSVariableModel
+from .utils import read_imas_handles_from_file
+
+logger = logging.getLogger(__name__)
+info, debug = logger.info, logger.debug
+
+
+def _resolve_variables(var_names: Sequence[str]) -> list[IDSVariableModel]:
+    """Looks up variables if specified, if empty return all variables."""
+    idsvar_lookup = var_lookup.filter_type('IDS-variable')
+
+    if not var_names:
+        variables = list(idsvar_lookup.values())
+        op_queue.info(description='Merging all known variables')
+    else:
+        variables = list(idsvar_lookup[name] for name in var_names)
+        for variable in variables:
+            op_queue.info(description='Variable for merge',
+                          extra_description=f'{variable.name}')
+
+    return variables
+
+
+def _merge(*,
+           handles: Sequence[ImasHandle],
+           template: ImasHandle,
+           target: ImasHandle,
+           variables: Sequence[IDSVariableModel],
+           force: bool = False):
+    """Merge mas data.
+
+    Parameters
+    ----------
+    handles : Sequence[ImasHandle]
+        These are the imas handles that will be merged.
+    template : ImasHandle
+        This handle is the template that is used for the new data.
+    target : ImasHandle
+        This handle is the target location where the merged data will be stored.
+    variables : Sequence[Variable
+        These are the IDS variables to be merged.
+    force : bool
+        Force overwriting existing files.
+    """
+    for handle in handles:
+        logger.debug('Source for merge %s', handle)
+
+    op_queue.info(description='Template for merge',
+                  extra_description=f'{template}')
+
+    if target.exists() and not force:
+        op_queue.add_no_op(description='Abort merge',
+                           extra_description=f'{target} already exists, '
+                           'use --force to overwrite')
+        return
+
+    template.copy_data_to(target)
+
+    merge_data(handles, target, variables)
+
+
+def merge(*, target: str, template: str, handles: list[str],
+          input_files: list[str], var_names: list[str], force: bool, **kwargs):
+    """Merge as many data as possible."""
+    template = ImasHandle.from_string(template)
+    target = ImasHandle.from_string(target)
+
+    handles = [ImasHandle.from_string(handle) for handle in handles]
+    for file in input_files:
+        handles = handles + list(read_imas_handles_from_file(file).values())
+
+    handles = list(set(handles))  # Remove duplicate handles
+
+    variables = _resolve_variables(var_names)
+
+    _merge(
+        handles=handles,
+        template=template,
+        target=target,
+        variables=variables,
+    )
```

### Comparing `duqtools-1.6.4/src/duqtools/models/_job.py` & `duqtools-1.7.0/src/duqtools/models/_job.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-import logging
-from enum import Enum
-from pathlib import Path
-
-import click
-
-from ..config import cfg
-
-logger = logging.getLogger(__name__)
-info, debug = logger.info, logger.debug
-
-cs = click.style
-
-STATUS_SYMBOLS = {
-    'no status': cs('_', fg='yellow'),
-    'completed': cs('.', fg='green'),
-    'failed': cs('f', fg='red'),
-    'running': cs('r', fg='yellow'),
-    'submitted': cs('s', fg='yellow'),
-    'unknown': cs('u', fg='yellow')
-}
-
-
-class JobStatus(str, Enum):
-    NOSTATUS = 'no status'
-    COMPLETED = 'completed'
-    FAILED = 'failed'
-    RUNNING = 'running'
-    SUBMITTED = 'submitted'
-    UNKNOWN = 'unknown'
-
-    @property
-    def symbol(self):
-        return STATUS_SYMBOLS[self.value]
-
-    @staticmethod
-    def symbol_help():
-        s = ', '.join(f'{code} : {status}'
-                      for status, code in STATUS_SYMBOLS.items())
-        return f'Status codes:\n{s}'
-
-
-class Job:
-
-    def __init__(self, dir: Path):
-        self.dir = Path(dir).resolve()
-        self.cfg = cfg
-
-    def __repr__(self):
-        run = str(self.dir)
-        return f'{self.__class__.__name__}({run!r})'
-
-    @staticmethod
-    def status_symbol_help():
-        """Return help string for status codes."""
-        return JobStatus.symbol_help()
-
-    @property
-    def status_symbol(self):
-        """One letter status symbol."""
-        return self.status().symbol
-
-    @property
-    def has_submit_script(self) -> bool:
-        return self.submit_script.exists()
-
-    @property
-    def has_status(self) -> bool:
-        return self.status_file.exists()
-
-    @property
-    def is_submitted(self) -> bool:
-        return (self.dir / 'duqtools.submit.lock').exists()
-
-    def status(self) -> str:
-        if not self.has_status:
-            return JobStatus.NOSTATUS
-
-        sf = self.status_file
-        with open(sf) as f:
-            content = f.read()
-            if self.cfg.status.msg_completed in content:
-                return JobStatus.COMPLETED
-            elif self.cfg.status.msg_failed in content:
-                return JobStatus.FAILED
-            elif self.cfg.status.msg_running in content:
-                return JobStatus.RUNNING
-
-        if self.is_submitted:
-            return JobStatus.SUBMITTED
-
-        return JobStatus.UNKNOWN
-
-    @property
-    def is_completed(self) -> bool:
-        return self.status() == JobStatus.COMPLETED
-
-    @property
-    def is_failed(self) -> bool:
-        return self.status() == JobStatus.FAILED
-
-    @property
-    def is_running(self) -> bool:
-        return self.status() == JobStatus.RUNNING
-
-    @property
-    def in_file(self) -> Path:
-        return self.dir / self.cfg.status.in_file
-
-    @property
-    def out_file(self) -> Path:
-        return self.dir / self.cfg.status.out_file
-
-    @property
-    def status_file(self) -> Path:
-        return self.dir / self.cfg.status.status_file
-
-    @property
-    def submit_script(self) -> Path:
-        return self.dir / self.cfg.submit.submit_script_name
-
-    @property
-    def lockfile(self) -> Path:
-        return self.dir / 'duqtools.submit.lock'
-
-    def submit(self):
-        from ..system import get_system
-        debug(f'Put lockfile in place for {self.lockfile}')
-        self.lockfile.touch()
-
-        get_system().submit_job(self)
-
-    def start(self):
-        click.echo(f'Submitting {self}\033[K')
-        self.submit()
-
-        while not self.has_status:
-            yield
-
-        while self.is_running:
-            yield
+import logging
+from enum import Enum
+from pathlib import Path
+
+import click
+
+from ..config import cfg
+
+logger = logging.getLogger(__name__)
+info, debug = logger.info, logger.debug
+
+cs = click.style
+
+STATUS_SYMBOLS = {
+    'no status': cs('_', fg='yellow'),
+    'completed': cs('.', fg='green'),
+    'failed': cs('f', fg='red'),
+    'running': cs('r', fg='yellow'),
+    'submitted': cs('s', fg='yellow'),
+    'unknown': cs('u', fg='yellow')
+}
+
+
+class JobStatus(str, Enum):
+    NOSTATUS = 'no status'
+    COMPLETED = 'completed'
+    FAILED = 'failed'
+    RUNNING = 'running'
+    SUBMITTED = 'submitted'
+    UNKNOWN = 'unknown'
+
+    @property
+    def symbol(self):
+        return STATUS_SYMBOLS[self.value]
+
+    @staticmethod
+    def symbol_help():
+        s = ', '.join(f'{code} : {status}'
+                      for status, code in STATUS_SYMBOLS.items())
+        return f'Status codes:\n{s}'
+
+
+class Job:
+
+    def __init__(self, dir: Path):
+        self.dir = Path(dir).resolve()
+        self.cfg = cfg
+
+    def __repr__(self):
+        run = str(self.dir)
+        return f'{self.__class__.__name__}({run!r})'
+
+    @staticmethod
+    def status_symbol_help():
+        """Return help string for status codes."""
+        return JobStatus.symbol_help()
+
+    @property
+    def status_symbol(self):
+        """One letter status symbol."""
+        return self.status().symbol
+
+    @property
+    def has_submit_script(self) -> bool:
+        return self.submit_script.exists()
+
+    @property
+    def has_status(self) -> bool:
+        return self.status_file.exists()
+
+    @property
+    def is_submitted(self) -> bool:
+        return (self.dir / 'duqtools.submit.lock').exists()
+
+    def status(self) -> str:
+        if not self.has_status:
+            return JobStatus.NOSTATUS
+
+        sf = self.status_file
+        with open(sf) as f:
+            content = f.read()
+            if self.cfg.status.msg_completed in content:
+                return JobStatus.COMPLETED
+            elif self.cfg.status.msg_failed in content:
+                return JobStatus.FAILED
+            elif self.cfg.status.msg_running in content:
+                return JobStatus.RUNNING
+
+        if self.is_submitted:
+            return JobStatus.SUBMITTED
+
+        return JobStatus.UNKNOWN
+
+    @property
+    def is_completed(self) -> bool:
+        return self.status() == JobStatus.COMPLETED
+
+    @property
+    def is_failed(self) -> bool:
+        return self.status() == JobStatus.FAILED
+
+    @property
+    def is_running(self) -> bool:
+        return self.status() == JobStatus.RUNNING
+
+    @property
+    def in_file(self) -> Path:
+        return self.dir / self.cfg.status.in_file
+
+    @property
+    def out_file(self) -> Path:
+        return self.dir / self.cfg.status.out_file
+
+    @property
+    def status_file(self) -> Path:
+        return self.dir / self.cfg.status.status_file
+
+    @property
+    def submit_script(self) -> Path:
+        return self.dir / self.cfg.submit.submit_script_name
+
+    @property
+    def lockfile(self) -> Path:
+        return self.dir / 'duqtools.submit.lock'
+
+    def submit(self):
+        from ..system import get_system
+        debug(f'Put lockfile in place for {self.lockfile}')
+        self.lockfile.touch()
+
+        get_system().submit_job(self)
+
+    def start(self):
+        click.echo(f'Submitting {self}\033[K')
+        self.submit()
+
+        while not self.has_status:
+            yield
+
+        while self.is_running:
+            yield
```

### Comparing `duqtools-1.6.4/src/duqtools/models/_locations.py` & `duqtools-1.7.0/src/duqtools/models/_locations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from os import getenv
-from pathlib import Path
-from typing import Optional
-
-from ..config import cfg
-from ..schema.runs import Run, Runs
-
-
-class Locations:
-    """Class that knows about locations within a duqtools config directory.
-
-    Defaults to local working directory, but can be initialized with a
-    known config directory.
-    """
-
-    def __init__(self, parent_dir: Optional[Path] = None):
-        if not parent_dir:
-            parent_dir = Path.cwd()
-
-        self.parent_dir = parent_dir
-
-    @property
-    def data_csv(self):
-        """Location of data.csv."""
-        return self.parent_dir / 'data.csv'
-
-    @property
-    def runs_yaml(self):
-        """Location of runs.yaml."""
-        return self.parent_dir / 'runs.yaml'
-
-    @property
-    def runs_yaml_old(self):
-        """Location of runs.yaml.old."""
-        return self.parent_dir / 'runs.yaml.old'
-
-    @property
-    def runs(self) -> list[Run]:
-        """Get a list of the runs currently created from this config."""
-        runs_yaml = self.runs_yaml
-
-        if not runs_yaml.exists():
-            raise OSError(f'Cannot find {runs_yaml}.')
-
-        return Runs.parse_file(runs_yaml)
-
-    @property
-    def jruns_path(self) -> Path:
-        """return the Path specified in the create->jruns config variable, or,
-        if that is empty, the `$JRUNS` environment variable, or, if `$JRUNS`
-        does not exists, return the current directory `./`.
-
-        Returns
-        -------
-        Path
-        """
-
-        if cfg.create.jruns:  # type: ignore
-            return cfg.create.jruns  # type: ignore
-        elif getenv('JRUNS'):
-            return Path(getenv('JRUNS'))  # type: ignore
-        else:
-            return Path()
+from os import getenv
+from pathlib import Path
+from typing import Optional
+
+from ..config import cfg
+from ._run import Run, Runs
+
+
+class Locations:
+    """Class that knows about locations within a duqtools config directory.
+
+    Defaults to local working directory, but can be initialized with a
+    known config directory.
+    """
+
+    def __init__(self, parent_dir: Optional[Path] = None):
+        if not parent_dir:
+            parent_dir = Path.cwd()
+
+        self.parent_dir = parent_dir
+
+    @property
+    def data_csv(self):
+        """Location of data.csv."""
+        return self.parent_dir / 'data.csv'
+
+    @property
+    def runs_yaml(self):
+        """Location of runs.yaml."""
+        return self.parent_dir / 'runs.yaml'
+
+    @property
+    def runs_yaml_old(self):
+        """Location of runs.yaml.old."""
+        return self.parent_dir / 'runs.yaml.old'
+
+    @property
+    def runs(self) -> list[Run]:
+        """Get a list of the runs currently created from this config."""
+        runs_yaml = self.runs_yaml
+
+        if not runs_yaml.exists():
+            raise OSError(f'Cannot find {runs_yaml}.')
+
+        return Runs.parse_file(runs_yaml)
+
+    @property
+    def jruns_path(self) -> Path:
+        """return the Path specified in the create->jruns config variable, or,
+        if that is empty, the `$JRUNS` environment variable, or, if `$JRUNS`
+        does not exists, return the current directory `./`.
+
+        Returns
+        -------
+        Path
+        """
+
+        if cfg.create.jruns:  # type: ignore
+            return cfg.create.jruns  # type: ignore
+        elif getenv('JRUNS'):
+            return Path(getenv('JRUNS'))  # type: ignore
+        else:
+            return Path()
```

### Comparing `duqtools-1.6.4/src/duqtools/models/_system.py` & `duqtools-1.7.0/src/duqtools/models/_system.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-from __future__ import annotations
-
-import logging
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING
-
-from ..config import Config
-from ..schema import BaseModel, ImasBaseModel
-
-if TYPE_CHECKING:
-    from pathlib import Path
-
-    from ..ids import ImasHandle
-    from ._job import Job
-
-logger = logging.getLogger(__name__)
-
-
-class AbstractSystem(ABC, BaseModel):
-
-    @staticmethod
-    @abstractmethod
-    def get_runs_dir() -> Path:
-        """Get the directory where the runs should be stored.
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-        Path
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def write_batchfile(run_dir: Path, cfg: Config):
-        """Write the batchfile used to submit the job inside run directory
-        `run_dir`.
-
-        Parameters
-        ----------
-        run_dir : Path
-            directory of run
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def submit_job(job: Job):
-        """submit the job specified by `job` to the system.
-
-        Parameters
-        ----------
-        job : Job
-            job
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def copy_from_template(source_drc: Path, target_drc: Path):
-        """copy from template directory `source_drc` to target directory
-        `target_drc`
-
-        Parameters
-        ----------
-        source_drc : Path
-            source directory
-        target_drc : Path
-            target directory
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def imas_from_path(template_drc: Path) -> ImasHandle:
-        """It takes a path, and finds out the IMAS entry associated with it.
-
-        Parameters
-        ----------
-        template_drc : Path
-            folder from which to extract IMAS location
-
-        Returns
-        -------
-        ImasHandle
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def update_imas_locations(run: Path, inp: ImasBaseModel,
-                              out: ImasBaseModel):
-        """Set the imas entries for the run, both input imas file `in` and
-        output imas file `out`.
-
-        Parameters
-        ----------
-        run : Path
-            run directory
-        inp : ImasBaseModel
-            Imas entry to use as input
-        out : ImasBaseModel
-            Imas entry to use as output
-        """
-        pass
+from __future__ import annotations
+
+import logging
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING
+
+from ..config import Config
+from ..schema import BaseModel, ImasBaseModel
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from ..ids import ImasHandle
+    from ._job import Job
+
+logger = logging.getLogger(__name__)
+
+
+class AbstractSystem(ABC, BaseModel):
+
+    @staticmethod
+    @abstractmethod
+    def get_runs_dir() -> Path:
+        """Get the directory where the runs should be stored.
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        Path
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def write_batchfile(run_dir: Path, cfg: Config):
+        """Write the batchfile used to submit the job inside run directory
+        `run_dir`.
+
+        Parameters
+        ----------
+        run_dir : Path
+            directory of run
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def submit_job(job: Job):
+        """submit the job specified by `job` to the system.
+
+        Parameters
+        ----------
+        job : Job
+            job
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def copy_from_template(source_drc: Path, target_drc: Path):
+        """copy from template directory `source_drc` to target directory
+        `target_drc`
+
+        Parameters
+        ----------
+        source_drc : Path
+            source directory
+        target_drc : Path
+            target directory
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def imas_from_path(template_drc: Path) -> ImasHandle:
+        """It takes a path, and finds out the IMAS entry associated with it.
+
+        Parameters
+        ----------
+        template_drc : Path
+            folder from which to extract IMAS location
+
+        Returns
+        -------
+        ImasHandle
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def update_imas_locations(run: Path, inp: ImasBaseModel,
+                              out: ImasBaseModel):
+        """Set the imas entries for the run, both input imas file `in` and
+        output imas file `out`.
+
+        Parameters
+        ----------
+        run : Path
+            run directory
+        inp : ImasBaseModel
+            Imas entry to use as input
+        out : ImasBaseModel
+            Imas entry to use as output
+        """
+        pass
```

### Comparing `duqtools-1.6.4/src/duqtools/operations.py` & `duqtools-1.7.0/src/duqtools/operations.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-from __future__ import annotations
-
-import atexit
-import logging
-from collections import deque
-from contextlib import contextmanager
-from inspect import signature
-from typing import Any, Callable, Optional, Sequence
-
-import click
-from pydantic import Field, validator
-
-from ._logging_utils import duqlog_screen
-from .config import cfg
-from .schema import BaseModel
-
-logger = logging.getLogger(__name__)
-
-OP_STYLE = {'fg': 'green'}
-
-INFO_STYLE = {'fg': 'blue'}
-
-NO_OP_STYLE = {
-    'fg': 'red',
-    'bold': True,
-}
-
-HEADER_STYLE = {
-    'fg': 'red',
-    'bold': True,
-}
-
-loginfo = duqlog_screen.info
-logwarning = duqlog_screen.warning
-style = click.style
-
-
-class LongDescriptionMixin:
-    description: str
-    extra_description: Optional[str]
-    style: dict
-
-    @property
-    def long_description(self) -> str:
-        description = style(self.description, **self.style)
-
-        if self.extra_description:
-            description = f'{description} : {self.extra_description}'
-
-        return description
-
-
-class Warning(LongDescriptionMixin):
-    """Warning item for screen log."""
-    style = NO_OP_STYLE
-
-    def __init__(self, description: str, extra_description: str):
-        self.description = description
-        self.extra_description = extra_description
-
-    def __hash__(self):
-        return hash((self.description, self.extra_description))
-
-    def __eq__(self, other):
-        return hash(self) == hash(other)
-
-
-class Operation(LongDescriptionMixin, BaseModel):
-    """Operation, simple class which has a callable action.
-
-    Usually not called directly but used through Operations. has the
-    following members:
-    """
-
-    quiet: bool = Field(False,
-                        description='print out this operation to the screen')
-    description: str = Field(
-        description='description of the operation to be done')
-    action: Optional[Callable] = Field(
-        description='a function which can be executed when we '
-        'decide to apply this operation')
-    extra_description: Optional[str] = Field(description='Extra description')
-    args: Optional[Sequence] = Field(
-        None,
-        description='positional arguments that have to be '
-        'passed to the action')
-    style: dict[str, Any] = Field(OP_STYLE,
-                                  description='Styling for op description')
-    kwargs: Optional[dict] = Field(
-        None,
-        description='keyword arguments that will be '
-        'passed to the action')
-
-    def __call__(self) -> Operation:
-        """Execute the action with the args and kwargs.
-
-        Returns
-        -------
-        Operation
-            The operation that was executed
-        """
-        if self.action:
-            logger.debug(self.long_description)
-            self.action(*self.args, **self.kwargs)  # type: ignore
-        return self
-
-    @validator('args', always=True)
-    def validate_args(cls, v):
-        if v is None:
-            v = ()
-        return v
-
-    @validator('kwargs', always=True)
-    def validate_kwargs(cls, v):
-        if v is None:
-            v = {}
-        return v
-
-
-class Operations(deque):
-    """Operations Queue which keeps track of all the operations that need to be
-    done.
-
-    It's basically dask_delayed, but custom made and a few drawbacks:
-    The return value from an action is eventually discarded,
-    communication between queue items is possible through references, or
-    global values, but not really recommended, and no guidance for this
-    is provided
-    """
-
-    _instance = None
-    yes = False  # Apply operations without prompt
-    enabled = False  # Actually do something
-    dry_run = False  # Never apply any operations (do not even ask)
-    warnings: set[Warning] = set()
-
-    def __new__(cls, *args, **kwargs):
-        # Make it a singleton
-        if not Operations._instance:
-            Operations._instance = super().__new__(cls)
-        return Operations._instance
-
-    @property
-    def n_actions(self):
-        """Return number of actions (no no-op)."""
-        return sum(op.action is not None for op in self)
-
-    def add(self, **kwargs) -> None:
-        """Convenience Operation wrapper around .append().
-
-        ```python
-        from duqtools.operations import add_to_op_queue.
-
-        op_queue.add(action=print, args=('Hello World,),
-        description="Function that prints hello world")
-        ```
-        """
-        self.append(Operation(**kwargs))
-
-    def add_no_op(self,
-                  description: str,
-                  extra_description: str | None = None):
-        """Adds a line to specify an action will not be undertaken."""
-        self.add(action=None,
-                 description=description,
-                 extra_description=extra_description,
-                 style=NO_OP_STYLE)
-
-    def info(self, description: str, extra_description: Optional[str] = None):
-        """Adds an info line."""
-        self.add(action=None,
-                 description=description,
-                 extra_description=extra_description,
-                 style=INFO_STYLE)
-
-    def warning(self, description: str, extra_description: str):
-        self.warnings.add(
-            Warning(description=description,
-                    extra_description=extra_description))
-
-    def put(self, item: Operation):
-        """synonym for append."""
-        self.append(item)
-
-    def append(self, item: Operation):  # type: ignore
-        """Restrict our diet to Operation objects only."""
-        if self.enabled:
-            logger.debug(
-                f'Appended {item.description} to the operations queue')
-            super().append(item)
-        else:
-            loginfo('- ' + item.long_description)
-            item()
-
-    def apply(self) -> Operation:
-        """Apply the next operation in the queue and remove it."""
-        op = self.popleft()
-        op()
-        return op
-
-    def _apply_all(self, callback: Optional[Callable] = None) -> None:
-        """Pop and apply all operations in the queue."""
-        while self:
-            op = self.apply()
-            if callback:
-                callback(op)
-
-    def apply_all(self) -> None:
-        """Apply all queued operations and empty the queue.
-
-        and show a fancy progress bar while applying
-        """
-        from tqdm import tqdm
-        loginfo(style('Applying Operations', **HEADER_STYLE))  # type: ignore
-
-        if cfg.quiet:
-            return self._apply_all()
-
-        print(self.n_actions)
-
-        with tqdm(total=self.n_actions, position=1) as pbar:
-            pbar.set_description('Progress')
-
-            with tqdm(bar_format='{desc}') as dbar:
-
-                def callback(op):
-                    if not op.action:
-                        return
-                    if not op.quiet:
-                        dbar.set_description(op.long_description)
-                    pbar.update()
-
-                self._apply_all(callback=callback)
-
-    def confirm_apply_all(self) -> bool:
-        """First asks the user if he wants to apply everything.
-
-        Returns
-        -------
-        bool: did we apply everything or not
-        """
-        # To print the descriptions we need to get them
-        loginfo('')
-        loginfo(style('Operations in the Queue:',
-                      **HEADER_STYLE))  # type: ignore
-        loginfo(style('========================',
-                      **HEADER_STYLE))  # type: ignore
-        for op in self:
-            if not op.quiet:
-                loginfo('- ' + op.long_description)
-
-        for warning in self.warnings:
-            loginfo('- ' + warning.long_description)
-
-        if self.dry_run:
-            loginfo('Dry run enabled, not applying op_queue')
-            return False
-
-        # Do not confirm if all actions are no-op
-        if all(op.action is None for op in self):
-            loginfo('\nNo actions to execute.')
-            return False
-
-        if n_no_op := sum(op.action is None for op in self):
-            loginfo(
-                f'\nThere are {n_no_op} operations that will not be applied.')
-
-        is_confirmed = self.yes or click.confirm(
-            f'\nDo you want to apply all {self.n_actions} operations?',
-            default=False)
-
-        if is_confirmed:
-            self.apply_all()
-
-        return is_confirmed
-
-    def check_unconfirmed_operations(self):
-        """Safety check, it should never happen that operations are not
-        executed."""
-        if self:
-            logwarning(
-                style((f'There are still {self.n_actions} operations '
-                       'in the queue at program exit!'), **HEADER_STYLE))
-
-
-op_queue = Operations()
-
-
-def confirm_operations(func):
-    """Decorator which confirms and applies queued operations after the
-    function.
-
-    ```python
-    from duqtools.operations import confirm_operations, op_queue
-
-    @confirm_operations
-    def complicated_stuff()
-        op_queue.add(action=print, args=('Hello World,),
-                description="Function that prints hello world")
-        op_queue.add(action=print, args=('Hello World again,),
-                description="Function that prints hello world, again")
-    ```
-    """
-
-    def wrapper(*args, **kwargs):
-        if op_queue.enabled:
-            raise RuntimeError('op_queue already enabled')
-        try:
-            op_queue.enabled = True
-            ret = func(*args, **kwargs)
-            op_queue.confirm_apply_all()
-            op_queue.clear()
-            op_queue.enabled = False
-        except Exception:
-            op_queue.clear()
-            op_queue.enabled = False
-            raise
-        return ret
-
-    return wrapper
-
-
-def add_to_op_queue(op_desc: str, extra_desc: str | None = None, quiet=False):
-    """Decorator which adds the function call to the op_queue, instead of
-    executing it directly, the string can be a format string and use the
-    function arguments.
-
-    ```python
-    from duqtools.operations import add_to_op_queue, op_queue
-
-    @add_to_op_queue("Printing hello world", "{name}")
-    def print_hello_world(name):
-        print(f"Hello World {name}")
-
-
-    print_hello_world("Snoozy")
-
-    op_queue.confirm_apply_all()
-    ```
-    """
-
-    def op_queue_real(func):
-
-        def wrapper(*args, **kwargs) -> None:
-            # For the description format we must convert args to kwargs
-            sig = signature(func)
-            args_to_kw = dict(zip(sig.parameters, args))
-            fkwargs = kwargs.copy()
-            fkwargs.update(args_to_kw)
-            extra_formatted = None
-            if extra_desc:
-                extra_formatted = extra_desc.format(**fkwargs)
-            op_formatted = op_desc.format(**fkwargs)
-
-            # add the function to the queue
-            op_queue.add(action=func,
-                         args=args,
-                         kwargs=kwargs,
-                         description=op_formatted,
-                         extra_description=extra_formatted,
-                         quiet=quiet)
-
-        return wrapper
-
-    return op_queue_real
-
-
-atexit.register(op_queue.check_unconfirmed_operations)
-
-
-@contextmanager
-def op_queue_context():
-    """Context manager to enable the op_queue, and confirm_operations on exit
-    Also disables the op_queue on exit.
-
-    Works more or less the same as the `@confirm_operations` decorator
-    """
-    if op_queue.enabled:
-        raise RuntimeError('op_queue already enabled')
-    try:
-        op_queue.enabled = True
-        yield
-        op_queue.confirm_apply_all()
-        op_queue.clear()
-        op_queue.enabled = False
-    except Exception:
-        op_queue.clear()
-        op_queue.enabled = False
-        raise
+from __future__ import annotations
+
+import atexit
+import logging
+from collections import deque
+from contextlib import contextmanager
+from inspect import signature
+from typing import Any, Callable, Optional, Sequence
+
+import click
+from pydantic import Field, validator
+
+from ._logging_utils import duqlog_screen
+from .config import cfg
+from .schema import BaseModel
+
+logger = logging.getLogger(__name__)
+
+OP_STYLE = {'fg': 'green'}
+
+INFO_STYLE = {'fg': 'blue'}
+
+NO_OP_STYLE = {
+    'fg': 'red',
+    'bold': True,
+}
+
+HEADER_STYLE = {
+    'fg': 'red',
+    'bold': True,
+}
+
+loginfo = duqlog_screen.info
+logwarning = duqlog_screen.warning
+style = click.style
+
+
+class LongDescriptionMixin:
+    description: str
+    extra_description: Optional[str]
+    style: dict
+
+    @property
+    def long_description(self) -> str:
+        description = style(self.description, **self.style)
+
+        if self.extra_description:
+            description = f'{description} : {self.extra_description}'
+
+        return description
+
+
+class Warning(LongDescriptionMixin):
+    """Warning item for screen log."""
+    style = NO_OP_STYLE
+
+    def __init__(self, description: str, extra_description: str):
+        self.description = description
+        self.extra_description = extra_description
+
+    def __hash__(self):
+        return hash((self.description, self.extra_description))
+
+    def __eq__(self, other):
+        return hash(self) == hash(other)
+
+
+class Operation(LongDescriptionMixin, BaseModel):
+    """Operation, simple class which has a callable action.
+
+    Usually not called directly but used through Operations. has the
+    following members:
+    """
+
+    quiet: bool = Field(False,
+                        description='print out this operation to the screen')
+    description: str = Field(
+        description='description of the operation to be done')
+    action: Optional[Callable] = Field(
+        description='a function which can be executed when we '
+        'decide to apply this operation')
+    extra_description: Optional[str] = Field(description='Extra description')
+    args: Optional[Sequence] = Field(
+        None,
+        description='positional arguments that have to be '
+        'passed to the action')
+    style: dict[str, Any] = Field(OP_STYLE,
+                                  description='Styling for op description')
+    kwargs: Optional[dict] = Field(
+        None,
+        description='keyword arguments that will be '
+        'passed to the action')
+
+    def __call__(self) -> Operation:
+        """Execute the action with the args and kwargs.
+
+        Returns
+        -------
+        Operation
+            The operation that was executed
+        """
+        if self.action:
+            logger.debug(self.long_description)
+            self.action(*self.args, **self.kwargs)  # type: ignore
+        return self
+
+    @validator('args', always=True)
+    def validate_args(cls, v):
+        if v is None:
+            v = ()
+        return v
+
+    @validator('kwargs', always=True)
+    def validate_kwargs(cls, v):
+        if v is None:
+            v = {}
+        return v
+
+
+class Operations(deque):
+    """Operations Queue which keeps track of all the operations that need to be
+    done.
+
+    It's basically dask_delayed, but custom made and a few drawbacks:
+    The return value from an action is eventually discarded,
+    communication between queue items is possible through references, or
+    global values, but not really recommended, and no guidance for this
+    is provided
+    """
+
+    _instance = None
+    yes = False  # Apply operations without prompt
+    enabled = False  # Actually do something
+    dry_run = False  # Never apply any operations (do not even ask)
+    warnings: set[Warning] = set()
+
+    def __new__(cls, *args, **kwargs):
+        # Make it a singleton
+        if not Operations._instance:
+            Operations._instance = super().__new__(cls)
+        return Operations._instance
+
+    @property
+    def n_actions(self):
+        """Return number of actions (no no-op)."""
+        return sum(op.action is not None for op in self)
+
+    def add(self, **kwargs) -> None:
+        """Convenience Operation wrapper around .append().
+
+        ```python
+        from duqtools.operations import add_to_op_queue.
+
+        op_queue.add(action=print, args=('Hello World,),
+        description="Function that prints hello world")
+        ```
+        """
+        self.append(Operation(**kwargs))
+
+    def add_no_op(self,
+                  description: str,
+                  extra_description: str | None = None):
+        """Adds a line to specify an action will not be undertaken."""
+        self.add(action=None,
+                 description=description,
+                 extra_description=extra_description,
+                 style=NO_OP_STYLE)
+
+    def info(self, description: str, extra_description: Optional[str] = None):
+        """Adds an info line."""
+        self.add(action=None,
+                 description=description,
+                 extra_description=extra_description,
+                 style=INFO_STYLE)
+
+    def warning(self, description: str, extra_description: str):
+        self.warnings.add(
+            Warning(description=description,
+                    extra_description=extra_description))
+
+    def put(self, item: Operation):
+        """synonym for append."""
+        self.append(item)
+
+    def append(self, item: Operation):  # type: ignore
+        """Restrict our diet to Operation objects only."""
+        if self.enabled:
+            logger.debug(
+                f'Appended {item.description} to the operations queue')
+            super().append(item)
+        else:
+            loginfo('- ' + item.long_description)
+            item()
+
+    def apply(self) -> Operation:
+        """Apply the next operation in the queue and remove it."""
+        op = self.popleft()
+        op()
+        return op
+
+    def _apply_all(self, callback: Optional[Callable] = None) -> None:
+        """Pop and apply all operations in the queue."""
+        while self:
+            op = self.apply()
+            if callback:
+                callback(op)
+
+    def apply_all(self) -> None:
+        """Apply all queued operations and empty the queue.
+
+        and show a fancy progress bar while applying
+        """
+        from tqdm import tqdm
+        loginfo(style('Applying Operations', **HEADER_STYLE))  # type: ignore
+
+        if cfg.quiet:
+            return self._apply_all()
+
+        print(self.n_actions)
+
+        with tqdm(total=self.n_actions, position=1) as pbar:
+            pbar.set_description('Progress')
+
+            with tqdm(bar_format='{desc}') as dbar:
+
+                def callback(op):
+                    if not op.action:
+                        return
+                    if not op.quiet:
+                        dbar.set_description(op.long_description)
+                    pbar.update()
+
+                self._apply_all(callback=callback)
+
+    def confirm_apply_all(self) -> bool:
+        """First asks the user if he wants to apply everything.
+
+        Returns
+        -------
+        bool: did we apply everything or not
+        """
+        # To print the descriptions we need to get them
+        loginfo('')
+        loginfo(style('Operations in the Queue:',
+                      **HEADER_STYLE))  # type: ignore
+        loginfo(style('========================',
+                      **HEADER_STYLE))  # type: ignore
+        for op in self:
+            if not op.quiet:
+                loginfo('- ' + op.long_description)
+
+        for warning in self.warnings:
+            loginfo('- ' + warning.long_description)
+
+        if self.dry_run:
+            loginfo('Dry run enabled, not applying op_queue')
+            return False
+
+        # Do not confirm if all actions are no-op
+        if all(op.action is None for op in self):
+            loginfo('\nNo actions to execute.')
+            return False
+
+        if n_no_op := sum(op.action is None for op in self):
+            loginfo(
+                f'\nThere are {n_no_op} operations that will not be applied.')
+
+        is_confirmed = self.yes or click.confirm(
+            f'\nDo you want to apply all {self.n_actions} operations?',
+            default=False)
+
+        if is_confirmed:
+            self.apply_all()
+
+        return is_confirmed
+
+    def check_unconfirmed_operations(self):
+        """Safety check, it should never happen that operations are not
+        executed."""
+        if self:
+            logwarning(
+                style((f'There are still {self.n_actions} operations '
+                       'in the queue at program exit!'), **HEADER_STYLE))
+
+
+op_queue = Operations()
+
+
+def confirm_operations(func):
+    """Decorator which confirms and applies queued operations after the
+    function.
+
+    ```python
+    from duqtools.operations import confirm_operations, op_queue
+
+    @confirm_operations
+    def complicated_stuff()
+        op_queue.add(action=print, args=('Hello World,),
+                description="Function that prints hello world")
+        op_queue.add(action=print, args=('Hello World again,),
+                description="Function that prints hello world, again")
+    ```
+    """
+
+    def wrapper(*args, **kwargs):
+        if op_queue.enabled:
+            raise RuntimeError('op_queue already enabled')
+        try:
+            op_queue.enabled = True
+            ret = func(*args, **kwargs)
+            op_queue.confirm_apply_all()
+            op_queue.clear()
+            op_queue.enabled = False
+        except Exception:
+            op_queue.clear()
+            op_queue.enabled = False
+            raise
+        return ret
+
+    return wrapper
+
+
+def add_to_op_queue(op_desc: str, extra_desc: str | None = None, quiet=False):
+    """Decorator which adds the function call to the op_queue, instead of
+    executing it directly, the string can be a format string and use the
+    function arguments.
+
+    ```python
+    from duqtools.operations import add_to_op_queue, op_queue
+
+    @add_to_op_queue("Printing hello world", "{name}")
+    def print_hello_world(name):
+        print(f"Hello World {name}")
+
+
+    print_hello_world("Snoozy")
+
+    op_queue.confirm_apply_all()
+    ```
+    """
+
+    def op_queue_real(func):
+
+        def wrapper(*args, **kwargs) -> None:
+            # For the description format we must convert args to kwargs
+            sig = signature(func)
+            args_to_kw = dict(zip(sig.parameters, args))
+            fkwargs = kwargs.copy()
+            fkwargs.update(args_to_kw)
+            extra_formatted = None
+            if extra_desc:
+                extra_formatted = extra_desc.format(**fkwargs)
+            op_formatted = op_desc.format(**fkwargs)
+
+            # add the function to the queue
+            op_queue.add(action=func,
+                         args=args,
+                         kwargs=kwargs,
+                         description=op_formatted,
+                         extra_description=extra_formatted,
+                         quiet=quiet)
+
+        return wrapper
+
+    return op_queue_real
+
+
+atexit.register(op_queue.check_unconfirmed_operations)
+
+
+@contextmanager
+def op_queue_context():
+    """Context manager to enable the op_queue, and confirm_operations on exit
+    Also disables the op_queue on exit.
+
+    Works more or less the same as the `@confirm_operations` decorator
+    """
+    if op_queue.enabled:
+        raise RuntimeError('op_queue already enabled')
+    try:
+        op_queue.enabled = True
+        yield
+        op_queue.confirm_apply_all()
+        op_queue.clear()
+        op_queue.enabled = False
+    except Exception:
+        op_queue.clear()
+        op_queue.enabled = False
+        raise
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/_dimensions.py` & `duqtools-1.7.0/src/duqtools/schema/_dimensions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from __future__ import annotations
-
-from typing import Literal, Union
-
-from pydantic import Field, validator
-
-from ._basemodel import BaseModel
-from ._description_helpers import formatter as f
-from ._ranges import ARange, LinSpace
-from ._variable import IDSVariableModel, JettoVariableModel
-
-
-class OperatorMixin(BaseModel):
-    operator: Literal['add', 'multiply', 'divide', 'power', 'subtract',
-                      'floor_divide', 'mod', 'copyto',
-                      'remainder'] = Field('multiply',
-                                           description=f("""
-        Which operator to apply to the data in combination with any of the
-        given values below. This can be any of the basic numpy arithmetic
-        operations. Available choices: `add`, `multiply`, `divide`, `power`,
-        `subtract`, `floor_divide`, `mod`, `none` and `remainder`. These directly map
-        to the equivalent numpy functions, i.e. `add` -> `np.add`.
-        """))
-    scale_to_error: bool = Field(False,
-                                 description=f("""
-        If True, multiply value(s) by the error (sigma).
-
-        With asymmetric errors (i.e. both lower/upper error nodes are available),
-        scale to the lower error node for values < 0, and to the upper error node
-        for values > 0.
-        """))
-
-    _upper_suffix: str = '_error_upper'
-    _lower_suffix: str = '_error_lower'
-
-
-class DimMixin(BaseModel):
-    values: Union[list[float], ARange, LinSpace] = Field(description=f("""
-            Values to use with operator on field to create sampling
-            space."""))
-
-    @validator('values')
-    def convert_to_list(cls, v):
-        if not isinstance(v, list):
-            v = v.values
-        return v
-
-
-class OperationDim(OperatorMixin, DimMixin, BaseModel):
-    variable: str = Field(description=f("""
-    PlaceHolder for the actual Operator
-    """))
-
-    def expand(self, *args, **kwargs):
-        from duqtools.config import var_lookup
-        variable = var_lookup[self.variable]
-
-        if isinstance(variable, JettoVariableModel):
-            return JettoOperationDim.expand(self,
-                                            *args,
-                                            variable=variable,
-                                            **kwargs)
-        elif isinstance(variable, IDSVariableModel):
-            return IDSOperationDim.expand(self,
-                                          *args,
-                                          variable=variable,
-                                          **kwargs)
-        else:
-            raise NotImplementedError(
-                f'{self.variable} expand not implemented')
-
-
-class CoupledDim(BaseModel):
-    __root__: list[OperationDim]
-
-    @validator('__root__')
-    def check_dimensions_match(cls, dims):
-        if len(dims) > 0:
-            refdim = len(dims[0].values)
-            for dim in dims[1:]:
-                if not len(dim.values) == refdim:
-                    raise ValueError('dimensions do not match in coupled dim')
-        return dims
-
-    def expand(self, *args, **kwargs):
-        expanded = [operation.expand() for operation in self.__root__]
-        return [entry for entry in zip(*expanded)]  # Transpose
-
-
-class IDSPathMixin(BaseModel):
-    variable: IDSVariableModel = Field(description=f("""
-            IDS variable for the data to modify.
-            The time slice can be denoted with '*', this will match all
-            time slices in the IDS. Alternatively, you can specify the time
-            slice directly, i.e. `profiles_1d/0/t_i_ave` to only
-            match and update the 0-th time slice.
-            """))
-
-
-class IDSOperation(IDSPathMixin, OperatorMixin, BaseModel):
-    """Apply arithmetic operation to IDS."""
-
-    value: float = Field(description=f("""
-        Values to use with operator on field to create sampling
-        space."""))
-
-
-class IDSOperationDim(IDSPathMixin, OperatorMixin, DimMixin, BaseModel):
-    """Apply set of arithmetic operations to IDS.
-
-    Takes the IDS data and subtracts, adds, multiplies, etc with each
-    the given values.
-    """
-
-    def expand(self, *args, variable, **kwargs) -> tuple[IDSOperation, ...]:
-        """Expand list of values into operations with its components."""
-        return tuple(
-            IDSOperation(variable=variable,
-                         operator=self.operator,
-                         value=value,
-                         scale_to_error=self.scale_to_error)
-            for value in self.values)
-
-
-class JettoPathMixin(BaseModel):
-    variable: JettoVariableModel
-
-
-class JettoOperation(JettoPathMixin, OperatorMixin, BaseModel):
-    value: float = Field(description=f("""
-        Values to use with operator on field to create sampling
-        space."""))
-
-
-class JettoOperationDim(JettoPathMixin, OperatorMixin, DimMixin, BaseModel):
-
-    def expand(self, *args, variable, **kwargs) -> tuple[JettoOperation, ...]:
-        """Expand list of values into operations with its components."""
-        return tuple(
-            JettoOperation(variable=variable,
-                           operator=self.operator,
-                           value=value,
-                           scale_to_error=self.scale_to_error)
-            for value in self.values)
+from __future__ import annotations
+
+from typing import Literal, Union
+
+from pydantic import Field, validator
+
+from ._basemodel import BaseModel
+from ._description_helpers import formatter as f
+from ._ranges import ARange, LinSpace
+from ._variable import IDSVariableModel, JettoVariableModel
+
+
+class OperatorMixin(BaseModel):
+    operator: Literal['add', 'multiply', 'divide', 'power', 'subtract',
+                      'floor_divide', 'mod', 'copyto',
+                      'remainder'] = Field('multiply',
+                                           description=f("""
+        Which operator to apply to the data in combination with any of the
+        given values below. This can be any of the basic numpy arithmetic
+        operations. Available choices: `add`, `multiply`, `divide`, `power`,
+        `subtract`, `floor_divide`, `mod`, `none` and `remainder`. These directly map
+        to the equivalent numpy functions, i.e. `add` -> `np.add`.
+        """))
+    scale_to_error: bool = Field(False,
+                                 description=f("""
+        If True, multiply value(s) by the error (sigma).
+
+        With asymmetric errors (i.e. both lower/upper error nodes are available),
+        scale to the lower error node for values < 0, and to the upper error node
+        for values > 0.
+        """))
+
+    _upper_suffix: str = '_error_upper'
+    _lower_suffix: str = '_error_lower'
+
+
+class DimMixin(BaseModel):
+    values: Union[list[float], ARange, LinSpace] = Field(description=f("""
+            Values to use with operator on field to create sampling
+            space."""))
+
+    @validator('values')
+    def convert_to_list(cls, v):
+        if not isinstance(v, list):
+            v = v.values
+        return v
+
+
+class OperationDim(OperatorMixin, DimMixin, BaseModel):
+    variable: str = Field(description=f("""
+    PlaceHolder for the actual Operator
+    """))
+
+    def expand(self, *args, **kwargs):
+        from duqtools.config import var_lookup
+        variable = var_lookup[self.variable]
+
+        if isinstance(variable, JettoVariableModel):
+            return JettoOperationDim.expand(self,
+                                            *args,
+                                            variable=variable,
+                                            **kwargs)
+        elif isinstance(variable, IDSVariableModel):
+            return IDSOperationDim.expand(self,
+                                          *args,
+                                          variable=variable,
+                                          **kwargs)
+        else:
+            raise NotImplementedError(
+                f'{self.variable} expand not implemented')
+
+
+class CoupledDim(BaseModel):
+    __root__: list[OperationDim]
+
+    @validator('__root__')
+    def check_dimensions_match(cls, dims):
+        if len(dims) > 0:
+            refdim = len(dims[0].values)
+            for dim in dims[1:]:
+                if not len(dim.values) == refdim:
+                    raise ValueError('dimensions do not match in coupled dim')
+        return dims
+
+    def expand(self, *args, **kwargs):
+        expanded = [operation.expand() for operation in self.__root__]
+        return [entry for entry in zip(*expanded)]  # Transpose
+
+
+class IDSPathMixin(BaseModel):
+    variable: IDSVariableModel = Field(description=f("""
+            IDS variable for the data to modify.
+            The time slice can be denoted with '*', this will match all
+            time slices in the IDS. Alternatively, you can specify the time
+            slice directly, i.e. `profiles_1d/0/t_i_ave` to only
+            match and update the 0-th time slice.
+            """))
+
+
+class IDSOperation(IDSPathMixin, OperatorMixin, BaseModel):
+    """Apply arithmetic operation to IDS."""
+
+    value: float = Field(description=f("""
+        Values to use with operator on field to create sampling
+        space."""))
+
+
+class IDSOperationDim(IDSPathMixin, OperatorMixin, DimMixin, BaseModel):
+    """Apply set of arithmetic operations to IDS.
+
+    Takes the IDS data and subtracts, adds, multiplies, etc with each
+    the given values.
+    """
+
+    def expand(self, *args, variable, **kwargs) -> tuple[IDSOperation, ...]:
+        """Expand list of values into operations with its components."""
+        return tuple(
+            IDSOperation(variable=variable,
+                         operator=self.operator,
+                         value=value,
+                         scale_to_error=self.scale_to_error)
+            for value in self.values)
+
+
+class JettoPathMixin(BaseModel):
+    variable: JettoVariableModel
+
+
+class JettoOperation(JettoPathMixin, OperatorMixin, BaseModel):
+    value: float = Field(description=f("""
+        Values to use with operator on field to create sampling
+        space."""))
+
+
+class JettoOperationDim(JettoPathMixin, OperatorMixin, DimMixin, BaseModel):
+
+    def expand(self, *args, variable, **kwargs) -> tuple[JettoOperation, ...]:
+        """Expand list of values into operations with its components."""
+        return tuple(
+            JettoOperation(variable=variable,
+                           operator=self.operator,
+                           value=value,
+                           scale_to_error=self.scale_to_error)
+            for value in self.values)
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/_imas.py` & `duqtools-1.7.0/src/duqtools/schema/_imas.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-
-from getpass import getuser
-from typing import Optional
-
-from pydantic import Field, validator
-
-from ._basemodel import BaseModel
-
-
-class ImasBaseModel(BaseModel):
-    """This model describes an IMAS data location."""
-    relative_location: Optional[str] = Field(
-        None,
-        description='Set as the relative location to the'
-        ' imasdb location if a local imasdb is used')
-    user: str = Field(None, description='Username.')
-    db: str = Field(description='IMAS db/machine name.')
-    shot: int = Field(description='IMAS Shot number.')
-    run: int = Field(description='IMAS Run number.')
-
-    @validator('user', pre=True, always=True)
-    def validate_user(cls, v):
-        return v or getuser()
-
-    def __hash__(self):  # Needed to compare handles
-        return hash((self.user, self.db, self.shot, self.run))
+from __future__ import annotations
+
+from getpass import getuser
+from typing import Optional
+
+from pydantic import Field, validator
+
+from ._basemodel import BaseModel
+
+
+class ImasBaseModel(BaseModel):
+    """This model describes an IMAS data location."""
+    relative_location: Optional[str] = Field(
+        None,
+        description='Set as the relative location to the'
+        ' imasdb location if a local imasdb is used')
+    user: str = Field(None, description='Username.')
+    db: str = Field(description='IMAS db/machine name.')
+    shot: int = Field(description='IMAS Shot number.')
+    run: int = Field(description='IMAS Run number.')
+
+    @validator('user', pre=True, always=True)
+    def validate_user(cls, v):
+        return v or getuser()
+
+    def __hash__(self):  # Needed to compare handles
+        return hash((self.user, self.db, self.shot, self.run))
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/_jetto.py` & `duqtools-1.7.0/src/duqtools/schema/_jetto.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from __future__ import annotations
-
-from typing import Annotated, Literal, Union
-
-from pydantic import Field, validator
-
-from ._basemodel import BaseModel
-from ._description_helpers import formatter as f
-
-
-class JsetField(BaseModel):
-    file: Literal['jetto.jset'] = Field('jetto.jset',
-                                        description='Name of the file.')
-    field: str = Field(description='Field name.')
-
-
-class NamelistField(BaseModel):
-    file: Literal['jetto.in'] = Field('jetto.in',
-                                      description='Name of the file.')
-    field: str = Field(description='Field name.')
-    section: str = Field(description='Section in the config.')
-
-    @validator('section')
-    def section_lower(cls, v):
-        return v.lower()
-
-
-JettoField = Annotated[Union[JsetField, NamelistField],
-                       Field(discriminator='file')]
-
-
-class JettoVar(BaseModel):
-    """These describe the jetto variables."""
-    doc: str = Field(description='Docstring for the variable.')
-    name: str = Field(description='Name of the variable.')
-    type: Literal['str', 'int', 'float'] = Field(
-        description=f('Type of the variable (str, int, float)'))
-    keys: list[JettoField] = Field(description=f(
-        'Jetto keys to update when this jetto variable is requested'))
-
-    def get_type(self):
-        return {
-            'str': str,
-            'int': int,
-            'float': float,
-        }[self.type]
+from __future__ import annotations
+
+from typing import Annotated, Literal, Union
+
+from pydantic import Field, validator
+
+from ._basemodel import BaseModel
+from ._description_helpers import formatter as f
+
+
+class JsetField(BaseModel):
+    file: Literal['jetto.jset'] = Field('jetto.jset',
+                                        description='Name of the file.')
+    field: str = Field(description='Field name.')
+
+
+class NamelistField(BaseModel):
+    file: Literal['jetto.in'] = Field('jetto.in',
+                                      description='Name of the file.')
+    field: str = Field(description='Field name.')
+    section: str = Field(description='Section in the config.')
+
+    @validator('section')
+    def section_lower(cls, v):
+        return v.lower()
+
+
+JettoField = Annotated[Union[JsetField, NamelistField],
+                       Field(discriminator='file')]
+
+
+class JettoVar(BaseModel):
+    """These describe the jetto variables."""
+    doc: str = Field(description='Docstring for the variable.')
+    name: str = Field(description='Name of the variable.')
+    type: Literal['str', 'int', 'float'] = Field(
+        description=f('Type of the variable (str, int, float)'))
+    keys: list[JettoField] = Field(description=f(
+        'Jetto keys to update when this jetto variable is requested'))
+
+    def get_type(self):
+        return {
+            'str': str,
+            'int': int,
+            'float': float,
+        }[self.type]
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/_ranges.py` & `duqtools-1.7.0/src/duqtools/schema/_ranges.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import numpy as np
-from pydantic import Field
-
-from ._basemodel import BaseModel
-
-
-class LinSpace(BaseModel):
-    """Generated evenly spaced numbers over a specified interval.
-
-    See the implementation of [numpy.linspace][] for more details.
-    """
-    start: float = Field(description='Start value of the sequence.')
-    stop: float = Field(description='End value of the sequence.')
-    num: int = Field(description='Number of samples to generate.')
-
-    @property
-    def values(self):
-        """Convert to list."""
-        # `val.item()` converts to native python types
-        return [
-            val.item() for val in np.linspace(self.start, self.stop, self.num)
-        ]
-
-
-class ARange(BaseModel):
-    """Generate evenly spaced numbers within a given interval.
-
-    See the implementation of [numpy.arange][] for more details.
-    """
-
-    start: float = Field(
-        description='Start of the interval. Includes this value.')
-    stop: float = Field(
-        description='End of the interval. Excludes this interval.')
-    step: float = Field(description='Spacing between values.')
-
-    @property
-    def values(self):
-        """Convert to list."""
-        # `val.item()` converts to native python types
-        return [
-            val.item() for val in np.arange(self.start, self.stop, self.step)
-        ]
+import numpy as np
+from pydantic import Field
+
+from ._basemodel import BaseModel
+
+
+class LinSpace(BaseModel):
+    """Generated evenly spaced numbers over a specified interval.
+
+    See the implementation of [numpy.linspace][] for more details.
+    """
+    start: float = Field(description='Start value of the sequence.')
+    stop: float = Field(description='End value of the sequence.')
+    num: int = Field(description='Number of samples to generate.')
+
+    @property
+    def values(self):
+        """Convert to list."""
+        # `val.item()` converts to native python types
+        return [
+            val.item() for val in np.linspace(self.start, self.stop, self.num)
+        ]
+
+
+class ARange(BaseModel):
+    """Generate evenly spaced numbers within a given interval.
+
+    See the implementation of [numpy.arange][] for more details.
+    """
+
+    start: float = Field(
+        description='Start of the interval. Includes this value.')
+    stop: float = Field(
+        description='End of the interval. Excludes this interval.')
+    step: float = Field(description='Spacing between values.')
+
+    @property
+    def values(self):
+        """Convert to list."""
+        # `val.item()` converts to native python types
+        return [
+            val.item() for val in np.arange(self.start, self.stop, self.step)
+        ]
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/_variable.py` & `duqtools-1.7.0/src/duqtools/schema/_variable.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import Optional
-
-from pydantic import Field
-
-from ._basemodel import BaseModel
-from ._description_helpers import formatter as f
-from ._jetto import JettoVar
-
-
-class JettoVariableModel(BaseModel):
-    """Variable for describing variables specific to Jetto, The lookup table
-    can be defined as a JettoVar under the lookup key."""
-
-    type: str = Field('jetto-variable',
-                      description='Discriminator for the variable type.')
-
-    name: str = Field(description=f("""
-        Name of the variable.
-        Used for the lookup table to find actual fields.
-        """))
-    lookup: Optional[JettoVar] = Field(description=f("""
-    Description of the fields that have to be updated for a Jetto Variable
-    """))
-
-
-class IDSPath(BaseModel):
-    ids: str = Field(description='Root IDS name.')
-    path: str = Field(description=f("""
-        Path to the data within the IDS.
-        The fields are separated by forward slashes (`\\`).
-    """))
-
-
-class IDSVariableModel(IDSPath):
-    """Variable for describing data within a IMAS database.
-
-    The variable can be given a name, which will be used in the rest of the config
-    to reference the variable. It will also be used as the column labels or
-    on plots.
-
-    The dimensions for each variable must be specified. This ensures the the data
-    will be self-consistent. For example for 1D data, you can use `[x]` and for 2D data,
-    `[x, y]`.
-
-    The IDS path may contain indices. You can point to a single index, by simply giving the
-    complete path (i.e. `profiles_1d/0/t_i_ave` for the 0th time slice).
-    To retrieve all time slices, you can use `profiles_1d/*/t_i_ave`.
-    """
-    type: str = Field('IDS-variable',
-                      description='discriminator for the variable type')
-
-    name: str = Field(description=f("""
-        Name of the variable.
-        This will be used to reference this variable.
-    """))
-    ids: str = Field(description='Root IDS name.')
-    path: str = Field(description=f("""
-        Path to the data within the IDS.
-        The fields are separated by forward slashes (`/`).
-    """))
-    dims: list[str] = Field(description=f("""
-        Give the dimensions of the data,
-        i.e. [x] for 1D, or [x, y] for 2D data.
-    """))
-
-
-class IDS2JettoVariableModel(BaseModel):
-    """Variable for describing the relation between IDS data and jetto
-    variables.
-
-    The variable can be given a name, which can be used in the config
-    template to reference the variable. It will also be used as the
-    column labels or on plots.
-    """
-    name: str = Field(description=f("""
-        Name of the variable.
-        This will be used to reference this variable.
-    """))
-    type: str = Field('IDS2jetto-variable',
-                      description='discriminator for the variable type')
-    paths: list[IDSPath] = Field(description=f("""
-        Search these variables in the given order until a match with the conditions
-        defined below is found.
-    """))
-    default: Optional[float] = Field(description=f("""
-        Default value if no match is found. Set to None to raise an exeption instead."""
-                                                   ))
+from typing import Optional
+
+from pydantic import Field
+
+from ._basemodel import BaseModel
+from ._description_helpers import formatter as f
+from ._jetto import JettoVar
+
+
+class JettoVariableModel(BaseModel):
+    """Variable for describing variables specific to Jetto, The lookup table
+    can be defined as a JettoVar under the lookup key."""
+
+    type: str = Field('jetto-variable',
+                      description='Discriminator for the variable type.')
+
+    name: str = Field(description=f("""
+        Name of the variable.
+        Used for the lookup table to find actual fields.
+        """))
+    lookup: Optional[JettoVar] = Field(description=f("""
+    Description of the fields that have to be updated for a Jetto Variable
+    """))
+
+
+class IDSPath(BaseModel):
+    ids: str = Field(description='Root IDS name.')
+    path: str = Field(description=f("""
+        Path to the data within the IDS.
+        The fields are separated by forward slashes (`\\`).
+    """))
+
+
+class IDSVariableModel(IDSPath):
+    """Variable for describing data within a IMAS database.
+
+    The variable can be given a name, which will be used in the rest of the config
+    to reference the variable. It will also be used as the column labels or
+    on plots.
+
+    The dimensions for each variable must be specified. This ensures the the data
+    will be self-consistent. For example for 1D data, you can use `[x]` and for 2D data,
+    `[x, y]`.
+
+    The IDS path may contain indices. You can point to a single index, by simply giving the
+    complete path (i.e. `profiles_1d/0/t_i_ave` for the 0th time slice).
+    To retrieve all time slices, you can use `profiles_1d/*/t_i_ave`.
+    """
+    type: str = Field('IDS-variable',
+                      description='discriminator for the variable type')
+
+    name: str = Field(description=f("""
+        Name of the variable.
+        This will be used to reference this variable.
+    """))
+    ids: str = Field(description='Root IDS name.')
+    path: str = Field(description=f("""
+        Path to the data within the IDS.
+        The fields are separated by forward slashes (`/`).
+    """))
+    dims: list[str] = Field(description=f("""
+        Give the dimensions of the data,
+        i.e. [x] for 1D, or [x, y] for 2D data.
+    """))
+
+
+class IDS2JettoVariableModel(BaseModel):
+    """Variable for describing the relation between IDS data and jetto
+    variables.
+
+    The variable can be given a name, which can be used in the config
+    template to reference the variable. It will also be used as the
+    column labels or on plots.
+    """
+    name: str = Field(description=f("""
+        Name of the variable.
+        This will be used to reference this variable.
+    """))
+    type: str = Field('IDS2jetto-variable',
+                      description='discriminator for the variable type')
+    paths: list[IDSPath] = Field(description=f("""
+        Search these variables in the given order until a match with the conditions
+        defined below is found.
+    """))
+    default: Optional[float] = Field(description=f("""
+        Default value if no match is found. Set to None to raise an exeption instead."""
+                                                   ))
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/cli.py` & `duqtools-1.7.0/src/duqtools/schema/cli.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-from pathlib import Path
-from typing import Literal, Optional, Union
-
-from pydantic import DirectoryPath, Field, validator
-
-from ._basemodel import BaseModel
-from ._description_helpers import formatter as f
-from ._dimensions import CoupledDim, OperationDim
-from ._imas import ImasBaseModel
-from .data_location import DataLocation
-from .matrix_samplers import CartesianProduct, HaltonSampler, LHSSampler, SobolSampler
-from .variables import VariableConfigModel
-
-
-class CreateConfigModel(BaseModel):
-    """The options of the `create` subcommand are stored in the `create` key in
-    the config."""
-    dimensions: list[Union[CoupledDim, OperationDim]] = Field(description=f("""
-        The `dimensions` specifies the dimensions of the matrix to sample
-        from. Each dimension is a compound set of operations to apply.
-        From this, a matrix all possible combinations is generated.
-        Essentially, it generates the
-        [Cartesian product](en.wikipedia.org/wiki/Cartesian_product)
-        of all operations. By specifying a different `sampler`, a subset of
-        this hypercube can be efficiently sampled.
-        """))
-
-    sampler: Union[LHSSampler, HaltonSampler, SobolSampler,
-                   CartesianProduct] = Field(default=CartesianProduct(),
-                                             discriminator='method',
-                                             description=f("""
-        For efficient UQ, it may not be necessary to sample the entire matrix
-        or hypercube. By default, the cartesian product is taken
-        (`method: cartesian-product`). For more efficient sampling of the space,
-        the following `method` choices are available:
-        [`latin-hypercube`](en.wikipedia.org/wiki/Latin_hypercube_sampling),
-        [`sobol`](en.wikipedia.org/wiki/Sobol_sequence),
-        [`halton`](en.wikipedia.org/wiki/Halton_sequence).
-        Where `n_samples` gives the number of samples to extract.
-        """))
-
-    template: DirectoryPath = Field(description=f("""
-        Template directory to modify. Duqtools copies and updates the settings
-        required for the specified system from this directory. This can be a
-        directory with a finished run, or one just stored by JAMS (but not yet
-        started). By default, duqtools extracts the input IMAS database entry
-        from the settings file (e.g. jetto.in) to find the data to modify for
-        the UQ runs.
-        """))
-
-    template_data: Optional[ImasBaseModel] = Field(description=f("""
-        Specify the location of the template data to modify. This overrides the
-        location of the data specified in settings file in the template
-        directory.
-        """))
-
-    data: Optional[DataLocation] = Field(description=f("""
-        Required for `system: jetto-v210921`, irrelevant for other systems.
-
-        Where to store the in/output IDS data.
-        The data key specifies the machine or imas
-        database name where to store the data (`imasdb`). duqtools will write the input
-        data files for UQ start with the run number given by `run_in_start_at`.
-        The data generated by the UQ runs (e.g. from jetto) will be stored
-        starting by the run number given by `run_out_start_at`.
-
-        """))
-
-    jruns: Optional[DirectoryPath] = Field(description=f(
-        """`jruns` defines the the root directory where all simulations are
-    run for the jetto system. Because the jettos system works with relative
-    directories from some root directory.
-
-    If this variable is not specified, duqtools will look for the `$JRUNS` environment
-    variable, and set it to that. If that fails, `jruns` is set to the current directory `./`
-
-    In this way, duqtools can ensure that the current work directory is
-    a subdirectory of the given root directory. All subdirectories are
-    calculated as relative to the root directory.
-
-    For example, for `rjettov`, the root directory must be set to
-    `/pfs/work/$USER/jetto/runs/`. Any UQ runs must therefore be
-    a subdirectory.
-
-    """))
-
-    runs_dir: Optional[Path] = Field(description=f(
-        """Relative location from the workspace, which specifies the folder where to
-    store all the created runs.
-
-    This defaults to `workspace/duqtools_experiment_x`
-    where `x` is a not yet existing integer."""))
-
-
-class SubmitConfigModel(BaseModel):
-    """The options of the `submit` subcommand are stored under the `submit` key
-    in the config.
-
-    The config describes the commands to start the UQ runs.
-    """
-
-    submit_script_name: str = Field(
-        '.llcmd', description='Name of the submission script.')
-    submit_command: str = Field('sbatch',
-                                description='Submission command for slurm.')
-    docker_image: str = Field('jintrac-imas',
-                              description='Docker image used for submission')
-    submit_system: Literal['prominence', 'slurm', 'docker'] = Field(
-        'slurm',
-        description='System to submit jobs to '
-        '[slurm (default), prominence, docker]')
-
-
-class StatusConfigModel(BaseModel):
-    """The options of the `status` subcommand are stored under the `status` key
-    in the config.
-
-    These only need to be changed if the modeling software changes.
-    """
-
-    status_file: str = Field('jetto.status',
-                             description='Name of the status file.')
-    in_file: str = Field('jetto.in',
-                         description=f("""
-            Name of the modelling input file, will be used to check
-            if the subprocess has started.
-            """))
-
-    out_file: str = Field('jetto.out',
-                          description=f("""
-            Name of the modelling output file, will be used to
-            check if the software is running.
-            """))
-
-    msg_completed: str = Field('Status : Completed successfully',
-                               description=f("""
-            Parse `status_file` for this message to check for
-            completion.
-            """))
-
-    msg_failed: str = Field('Status : Failed',
-                            description=f("""
-            Parse `status_file` for this message to check for
-            failures.
-            """))
-
-    msg_running: str = Field('Status : Running',
-                             description=f("""
-            Parse `status_file` for this message to check for
-            running status.
-            """))
-
-
-class ConfigModel(BaseModel):
-    """The options for the CLI are defined by this model."""
-    tag: str = Field(
-        '',
-        description=
-        'Create a tag for the runs to identify them in slurm or `data.csv`')
-
-    submit: SubmitConfigModel = Field(
-        SubmitConfigModel(),
-        description='Configuration for the submit subcommand')
-
-    create: Optional[CreateConfigModel] = Field(
-        description='Configuration for the create subcommand')
-
-    status: StatusConfigModel = Field(
-        StatusConfigModel(),
-        description='Configuration for the status subcommand')
-
-    workspace: Optional[str] = Field(description='Old field, currently unused')
-
-    extra_variables: Optional[VariableConfigModel] = Field(
-        description='Specify extra variables for this run.')
-
-    system: Literal['jetto', 'dummy', 'jetto-v210921',
-                    'jetto-v220922'] = Field(
-                        'jetto', description='backend system to use')
-
-    quiet: bool = Field(
-        False,
-        description='dont output to stdout, except for mandatory prompts')
-
-    @validator('workspace', pre=True)
-    def workspace_deprecated(cls, v):
-        if not v:
-            from warnings import warn
-            warn(f("""workspace key is Deprecated and unused, use create->jruns
-            and create->runs_dir to control where runs end up"""),
-                 DeprecationWarning,
-                 stacklevel=2)
-        return None
+from pathlib import Path
+from typing import Literal, Optional, Union
+
+from pydantic import DirectoryPath, Field, validator
+
+from ._basemodel import BaseModel
+from ._description_helpers import formatter as f
+from ._dimensions import CoupledDim, OperationDim
+from ._imas import ImasBaseModel
+from .data_location import DataLocation
+from .matrix_samplers import CartesianProduct, HaltonSampler, LHSSampler, SobolSampler
+from .variables import VariableConfigModel
+
+
+class CreateConfigModel(BaseModel):
+    """The options of the `create` subcommand are stored in the `create` key in
+    the config."""
+    dimensions: list[Union[CoupledDim, OperationDim]] = Field(description=f("""
+        The `dimensions` specifies the dimensions of the matrix to sample
+        from. Each dimension is a compound set of operations to apply.
+        From this, a matrix all possible combinations is generated.
+        Essentially, it generates the
+        [Cartesian product](en.wikipedia.org/wiki/Cartesian_product)
+        of all operations. By specifying a different `sampler`, a subset of
+        this hypercube can be efficiently sampled.
+        """))
+
+    sampler: Union[LHSSampler, HaltonSampler, SobolSampler,
+                   CartesianProduct] = Field(default=CartesianProduct(),
+                                             discriminator='method',
+                                             description=f("""
+        For efficient UQ, it may not be necessary to sample the entire matrix
+        or hypercube. By default, the cartesian product is taken
+        (`method: cartesian-product`). For more efficient sampling of the space,
+        the following `method` choices are available:
+        [`latin-hypercube`](en.wikipedia.org/wiki/Latin_hypercube_sampling),
+        [`sobol`](en.wikipedia.org/wiki/Sobol_sequence),
+        [`halton`](en.wikipedia.org/wiki/Halton_sequence).
+        Where `n_samples` gives the number of samples to extract.
+        """))
+
+    template: DirectoryPath = Field(description=f("""
+        Template directory to modify. Duqtools copies and updates the settings
+        required for the specified system from this directory. This can be a
+        directory with a finished run, or one just stored by JAMS (but not yet
+        started). By default, duqtools extracts the input IMAS database entry
+        from the settings file (e.g. jetto.in) to find the data to modify for
+        the UQ runs.
+        """))
+
+    template_data: Optional[ImasBaseModel] = Field(description=f("""
+        Specify the location of the template data to modify. This overrides the
+        location of the data specified in settings file in the template
+        directory.
+        """))
+
+    data: Optional[DataLocation] = Field(description=f("""
+        Required for `system: jetto-v210921`, irrelevant for other systems.
+
+        Where to store the in/output IDS data.
+        The data key specifies the machine or imas
+        database name where to store the data (`imasdb`). duqtools will write the input
+        data files for UQ start with the run number given by `run_in_start_at`.
+        The data generated by the UQ runs (e.g. from jetto) will be stored
+        starting by the run number given by `run_out_start_at`.
+
+        """))
+
+    jruns: Optional[DirectoryPath] = Field(description=f(
+        """`jruns` defines the the root directory where all simulations are
+    run for the jetto system. Because the jettos system works with relative
+    directories from some root directory.
+
+    If this variable is not specified, duqtools will look for the `$JRUNS` environment
+    variable, and set it to that. If that fails, `jruns` is set to the current directory `./`
+
+    In this way, duqtools can ensure that the current work directory is
+    a subdirectory of the given root directory. All subdirectories are
+    calculated as relative to the root directory.
+
+    For example, for `rjettov`, the root directory must be set to
+    `/pfs/work/$USER/jetto/runs/`. Any UQ runs must therefore be
+    a subdirectory.
+
+    """))
+
+    runs_dir: Optional[Path] = Field(description=f(
+        """Relative location from the workspace, which specifies the folder where to
+    store all the created runs.
+
+    This defaults to `workspace/duqtools_experiment_x`
+    where `x` is a not yet existing integer."""))
+
+
+class SubmitConfigModel(BaseModel):
+    """The options of the `submit` subcommand are stored under the `submit` key
+    in the config.
+
+    The config describes the commands to start the UQ runs.
+    """
+
+    submit_script_name: str = Field(
+        '.llcmd', description='Name of the submission script.')
+    submit_command: str = Field('sbatch',
+                                description='Submission command for slurm.')
+    docker_image: str = Field('jintrac-imas',
+                              description='Docker image used for submission')
+    submit_system: Literal['prominence', 'slurm', 'docker'] = Field(
+        'slurm',
+        description='System to submit jobs to '
+        '[slurm (default), prominence, docker]')
+
+
+class StatusConfigModel(BaseModel):
+    """The options of the `status` subcommand are stored under the `status` key
+    in the config.
+
+    These only need to be changed if the modeling software changes.
+    """
+
+    status_file: str = Field('jetto.status',
+                             description='Name of the status file.')
+    in_file: str = Field('jetto.in',
+                         description=f("""
+            Name of the modelling input file, will be used to check
+            if the subprocess has started.
+            """))
+
+    out_file: str = Field('jetto.out',
+                          description=f("""
+            Name of the modelling output file, will be used to
+            check if the software is running.
+            """))
+
+    msg_completed: str = Field('Status : Completed successfully',
+                               description=f("""
+            Parse `status_file` for this message to check for
+            completion.
+            """))
+
+    msg_failed: str = Field('Status : Failed',
+                            description=f("""
+            Parse `status_file` for this message to check for
+            failures.
+            """))
+
+    msg_running: str = Field('Status : Running',
+                             description=f("""
+            Parse `status_file` for this message to check for
+            running status.
+            """))
+
+
+class ConfigModel(BaseModel):
+    """The options for the CLI are defined by this model."""
+    tag: str = Field(
+        '',
+        description=
+        'Create a tag for the runs to identify them in slurm or `data.csv`')
+
+    submit: SubmitConfigModel = Field(
+        SubmitConfigModel(),
+        description='Configuration for the submit subcommand')
+
+    create: Optional[CreateConfigModel] = Field(
+        description='Configuration for the create subcommand')
+
+    status: StatusConfigModel = Field(
+        StatusConfigModel(),
+        description='Configuration for the status subcommand')
+
+    workspace: Optional[str] = Field(description='Old field, currently unused')
+
+    extra_variables: Optional[VariableConfigModel] = Field(
+        description='Specify extra variables for this run.')
+
+    system: Literal['jetto', 'dummy', 'jetto-v210921',
+                    'jetto-v220922'] = Field(
+                        'jetto', description='backend system to use')
+
+    quiet: bool = Field(
+        False,
+        description='dont output to stdout, except for mandatory prompts')
+
+    @validator('workspace', pre=True)
+    def workspace_deprecated(cls, v):
+        if not v:
+            from warnings import warn
+            warn(f("""workspace key is Deprecated and unused, use create->jruns
+            and create->runs_dir to control where runs end up"""),
+                 DeprecationWarning,
+                 stacklevel=2)
+        return None
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/data_location.py` & `duqtools-1.7.0/src/duqtools/schema/data_location.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Optional
-
-from pydantic import Field
-
-from ._basemodel import BaseModel
-from ._description_helpers import formatter as f
-
-
-class DataLocation(BaseModel):
-    """Specification for the data generated by the create step.
-
-    When setting up a sequence of UQ runs, duqtools reads the source data from
-    the template. For each individual UQ run needs, two locations must be
-    defined.
-        1. The location of the input data. This is where duqtools stores
-        the modified source data.
-        2. The location of the output data. The modelling software must know
-        in advance where to store the results of the simulation.
-
-    Input data are defined by `run_in_start_at`, and output data by
-    `run_out_start_at`. A sequence is generated starting from these numbers.
-
-    For example, with `run_in_start_at`: 7000 and `run_out_start_at`: 8000,
-    the generated input stored at run number 7000 would correspond to output
-    8000, 7001 to 8001, 7002 to 8002, etc.
-
-    Note that these sequences may overlap with existing data sets. Duqtools
-    will stop if it detects that data will be overwritten.
-    """
-
-    user: Optional[str] = Field(
-        description='Username for the IMAS database to use,'
-        ' defaults to current user')
-
-    imasdb: str = Field(description='IMAS database or machine name.')
-
-    run_in_start_at: int = Field(description=f("""
-            The sequence of input data files start with this run number.
-            """))
-
-    run_out_start_at: int = Field(description=f("""
-            The sequence of output data files start with this run number.
-            """))
+from typing import Optional
+
+from pydantic import Field
+
+from ._basemodel import BaseModel
+from ._description_helpers import formatter as f
+
+
+class DataLocation(BaseModel):
+    """Specification for the data generated by the create step.
+
+    When setting up a sequence of UQ runs, duqtools reads the source data from
+    the template. For each individual UQ run needs, two locations must be
+    defined.
+        1. The location of the input data. This is where duqtools stores
+        the modified source data.
+        2. The location of the output data. The modelling software must know
+        in advance where to store the results of the simulation.
+
+    Input data are defined by `run_in_start_at`, and output data by
+    `run_out_start_at`. A sequence is generated starting from these numbers.
+
+    For example, with `run_in_start_at`: 7000 and `run_out_start_at`: 8000,
+    the generated input stored at run number 7000 would correspond to output
+    8000, 7001 to 8001, 7002 to 8002, etc.
+
+    Note that these sequences may overlap with existing data sets. Duqtools
+    will stop if it detects that data will be overwritten.
+    """
+
+    user: Optional[str] = Field(
+        description='Username for the IMAS database to use,'
+        ' defaults to current user')
+
+    imasdb: str = Field(description='IMAS database or machine name.')
+
+    run_in_start_at: int = Field(description=f("""
+            The sequence of input data files start with this run number.
+            """))
+
+    run_out_start_at: int = Field(description=f("""
+            The sequence of output data files start with this run number.
+            """))
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/matrix_samplers.py` & `duqtools-1.7.0/src/duqtools/schema/matrix_samplers.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from __future__ import annotations
-
-from typing import Literal
-
-from pydantic import Field
-
-from ._basemodel import BaseModel
-
-
-class LHSSampler(BaseModel):
-    """Select the Latin Hypercube sampler by specifying
-    `method: latin-hypercube`."""
-
-    method: Literal['latin-hypercube'] = 'latin-hypercube'
-
-    n_samples: int = Field(3, description='Number of samples to take')
-
-
-class HaltonSampler(BaseModel):
-    """Select the Sobol sampler by specifying `method: halton`."""
-
-    method: Literal['halton']
-
-    n_samples: int = Field(3, description='Number of samples to take')
-
-
-class SobolSampler(BaseModel):
-    """Select the Sobol sampler by specifying `method: sobol`."""
-
-    method: Literal['sobol', 'low-discrepancy-sequence']
-
-    n_samples: int = Field(3, description='Number of samples to take')
-
-
-class CartesianProduct(BaseModel):
-    """Select the Cartesian product sampler by specifying
-    `method: cartesian-product`."""
-
-    method: Literal['cartesian-product'] = 'cartesian-product'
+from __future__ import annotations
+
+from typing import Literal
+
+from pydantic import Field
+
+from ._basemodel import BaseModel
+
+
+class LHSSampler(BaseModel):
+    """Select the Latin Hypercube sampler by specifying
+    `method: latin-hypercube`."""
+
+    method: Literal['latin-hypercube'] = 'latin-hypercube'
+
+    n_samples: int = Field(3, description='Number of samples to take')
+
+
+class HaltonSampler(BaseModel):
+    """Select the Sobol sampler by specifying `method: halton`."""
+
+    method: Literal['halton']
+
+    n_samples: int = Field(3, description='Number of samples to take')
+
+
+class SobolSampler(BaseModel):
+    """Select the Sobol sampler by specifying `method: sobol`."""
+
+    method: Literal['sobol', 'low-discrepancy-sequence']
+
+    n_samples: int = Field(3, description='Number of samples to take')
+
+
+class CartesianProduct(BaseModel):
+    """Select the Cartesian product sampler by specifying
+    `method: cartesian-product`."""
+
+    method: Literal['cartesian-product'] = 'cartesian-product'
```

### Comparing `duqtools-1.6.4/src/duqtools/schema/variables.py` & `duqtools-1.7.0/src/duqtools/schema/variables.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Union
-
-from ._basemodel import BaseModel
-from ._variable import IDS2JettoVariableModel, IDSVariableModel, JettoVariableModel
-
-
-class VariableConfigModel(BaseModel):
-    __root__: list[Union[JettoVariableModel, IDSVariableModel,
-                         IDS2JettoVariableModel]]
-
-    def __iter__(self):
-        yield from self.__root__
-
-    def __getitem__(self, index: int):
-        return self.__root__[index]
-
-    def to_variable_dict(self) -> dict:
-        """Return dict of variables."""
-        return {variable.name: variable for variable in self}
+from typing import Union
+
+from ._basemodel import BaseModel
+from ._variable import IDS2JettoVariableModel, IDSVariableModel, JettoVariableModel
+
+
+class VariableConfigModel(BaseModel):
+    __root__: list[Union[JettoVariableModel, IDSVariableModel,
+                         IDS2JettoVariableModel]]
+
+    def __iter__(self):
+        yield from self.__root__
+
+    def __getitem__(self, index: int):
+        return self.__root__[index]
+
+    def to_variable_dict(self) -> dict:
+        """Return dict of variables."""
+        return {variable.name: variable for variable in self}
```

### Comparing `duqtools-1.6.4/src/duqtools/setup.py` & `duqtools-1.7.0/src/duqtools/setup.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-from __future__ import annotations
-
-import logging
-from collections import defaultdict
-from pathlib import Path
-from types import SimpleNamespace
-from typing import TYPE_CHECKING, Any
-
-import yaml
-from jinja2 import Environment, FileSystemLoader
-
-from duqtools.api import ImasHandle
-from duqtools.config import var_lookup
-
-from .config import Config
-from .ids._imas import imasdef
-from .operations import op_queue
-from .utils import no_op
-
-if TYPE_CHECKING:
-    import jinja2
-
-    from duqtools.api import IDSMapping
-
-logger = logging.getLogger(__name__)
-
-
-class SetupError(Exception):
-    ...
-
-
-def get_template(filename: str) -> jinja2.Template:
-    """Load filename as a jinja2 template."""
-    path = Path(filename)
-    drc = Path(path).parent
-    file_loader = FileSystemLoader(str(drc))
-    environment = Environment(loader=file_loader, autoescape=True)
-    return environment.get_template(path.name)
-
-
-def _get_key(filename: str, *, key: str):
-    """Grab key from unrendered config file."""
-    with open(filename, 'rb') as f:
-        for line in f:
-            try:
-                item = yaml.safe_load(line)
-                return item[key]
-            except (yaml.YAMLError, TypeError, KeyError):
-                continue
-
-
-def _generate_run_dir(drc: Path, cfg: str, force: bool):
-    drc.mkdir(exist_ok=force, parents=True)
-
-    with open(drc / 'duqtools.yaml', 'w') as f:
-        f.write(cfg)
-
-
-class ExtrasV210921:
-    """Track run number to avoid overwriting existing data in sequential
-    runs."""
-    MAX_RUN = 9999
-
-    def __init__(self, template_file: str):
-        self.n_samples = self._get_n_samples(template_file)
-        self.run_numbers: dict[tuple[str, int],
-                               int] = defaultdict(lambda: 1000)
-
-    @staticmethod
-    def _get_n_samples(template_file: str) -> int:
-        """Grab number of samples generated by this config, from
-        `create.sampler.n_samples`."""
-        n_samples = _get_key(template_file, key='n_samples')
-
-        if not n_samples:
-            raise ValueError('`create.sampler.n_samples` must be defined for '
-                             'jintrac `v210921` config')
-
-        return n_samples
-
-    def add_system_attrs(self, *, handle: ImasHandle, run: SimpleNamespace):
-        """Add system specific attributes to run namespace."""
-        data_in_start = self.run_numbers[handle.db, handle.shot]
-        data_out_start = data_in_start + self.n_samples
-
-        self.run_numbers[handle.db,
-                         handle.shot] = data_out_start + self.n_samples
-
-        if self.run_numbers[handle.db, handle.shot] > self.MAX_RUN:
-            raise ValueError(
-                f'Cannot write data with run number > {self.MAX_RUN}')
-
-        run.data_in_start = data_in_start
-        run.data_out_start = data_out_start
-
-
-class Variables:
-    lookup = var_lookup.filter_type('IDS2jetto-variable')
-
-    def __init__(self, *, handle: ImasHandle):
-        self.handle = handle
-        self._ids_cache: dict[str, IDSMapping] = {}
-
-    def _get_ids(self, ids: str):
-        """Cache ids lookups to avoid repeated data reads."""
-        if ids in self._ids_cache:
-            mapping = self._ids_cache[ids]
-        else:
-            mapping = self.handle.get(ids)
-            self._ids_cache[ids] = mapping
-
-        return mapping
-
-    @staticmethod
-    def is_empty(value: Any) -> bool:
-        """Check against imasdef if variable is empty."""
-        if isinstance(value, float):
-            return value in (imasdef.EMPTY_FLOAT, imasdef.EMPTY_DOUBLE)
-        elif isinstance(value, int):
-            return value == imasdef.EMPTY_INT
-        elif isinstance(value, complex):
-            return value == imasdef.EMPTY_COMPLEX
-
-        return False
-
-    def __getattr__(self, key: str):
-        try:
-            spec = self.lookup[f'ids-{key}']
-        except KeyError as exc:
-            msg = f'Cannot find {key!r} in your variable listing (i.e. `variables.yaml`).'
-            raise AttributeError(msg) from exc
-
-        value = spec.default
-
-        for item in spec.paths:
-            mapping = self._get_ids(item.ids)
-            try:
-                trial = mapping[item.path]
-            except KeyError:
-                continue
-
-            if not self.is_empty(trial):
-                value = trial
-                break
-
-        if value is None:
-            raise AttributeError(
-                f'No value matches specifications given by: {spec}')
-
-        return value
-
-
-def substitute_templates(*, handles: dict[str, ImasHandle], template_file: str,
-                         force: bool):
-    """Handle template substitution.
-
-    Parameters
-    ----------
-    handles : dict[str, ImasHandle]
-        Dictionary with Imas handles
-    template_file : str
-        Path to template file.
-    force : bool
-        Overwrite files if set to true.
-    """
-    cwd = Path.cwd()
-
-    template = get_template(template_file)
-
-    if _get_key(template_file, key='system') == 'jetto-v210921':
-        add_system_attrs = ExtrasV210921(template_file).add_system_attrs
-    else:
-        add_system_attrs = no_op  # default to no-op
-
-    for name, handle in handles.items():
-        run = SimpleNamespace(name=name)
-
-        add_system_attrs(run=run, handle=handle)
-
-        variables = Variables(handle=handle)
-
-        cfg = template.render(run=run, variables=variables, handle=handle)
-
-        Config.parse_raw(cfg)  # make sure config is valid
-
-        out_drc = cwd / name
-
-        if out_drc.exists() and not force:
-            op_queue.add_no_op(description='Directory exists',
-                               extra_description=name)
-            op_queue.warning(description='Warning',
-                             extra_description='Some targets already exist, '
-                             'use --force to override')
-        else:
-            op_queue.add(
-                action=_generate_run_dir,
-                kwargs={
-                    'drc': out_drc,
-                    'cfg': cfg,
-                    'force': force
-                },
-                description='Setup run',
-                extra_description=name,
-            )
-
-
-def setup(*, handle, template_file, run_name, force, **kwargs):
-    """Setup large scale validation runs for template.
-
-    Parameters
-    ----------
-    handle : str
-        This is the handle to replace into the template.
-    template_file : Path
-        Path to the template file (jinja2 format).
-    run_name : str
-        Name of the output directory and run name.
-    force : bool
-        Set to true to overwrite previous files.
-    """
-    handles = {run_name: ImasHandle.from_string(handle)}
-
-    substitute_templates(handles=handles,
-                         template_file=template_file,
-                         force=force)
+from __future__ import annotations
+
+import logging
+from collections import defaultdict
+from pathlib import Path
+from types import SimpleNamespace
+from typing import TYPE_CHECKING, Any
+
+import yaml
+from jinja2 import Environment, FileSystemLoader
+
+from duqtools.api import ImasHandle
+from duqtools.config import var_lookup
+
+from .config import Config
+from .ids._imas import imasdef
+from .operations import op_queue
+from .utils import no_op
+
+if TYPE_CHECKING:
+    import jinja2
+
+    from duqtools.api import IDSMapping
+
+logger = logging.getLogger(__name__)
+
+
+class SetupError(Exception):
+    ...
+
+
+def get_template(filename: str) -> jinja2.Template:
+    """Load filename as a jinja2 template."""
+    path = Path(filename)
+    drc = Path(path).parent
+    file_loader = FileSystemLoader(str(drc))
+    environment = Environment(loader=file_loader, autoescape=True)
+    return environment.get_template(path.name)
+
+
+def _get_key(filename: str, *, key: str):
+    """Grab key from unrendered config file."""
+    with open(filename, 'rb') as f:
+        for line in f:
+            try:
+                item = yaml.safe_load(line)
+                return item[key]
+            except (yaml.YAMLError, TypeError, KeyError):
+                continue
+
+
+def _generate_run_dir(drc: Path, cfg: str, force: bool):
+    drc.mkdir(exist_ok=force, parents=True)
+
+    with open(drc / 'duqtools.yaml', 'w') as f:
+        f.write(cfg)
+
+
+class ExtrasV210921:
+    """Track run number to avoid overwriting existing data in sequential
+    runs."""
+    MAX_RUN = 9999
+
+    def __init__(self, template_file: str):
+        self.n_samples = self._get_n_samples(template_file)
+        self.run_numbers: dict[tuple[str, int],
+                               int] = defaultdict(lambda: 1000)
+
+    @staticmethod
+    def _get_n_samples(template_file: str) -> int:
+        """Grab number of samples generated by this config, from
+        `create.sampler.n_samples`."""
+        n_samples = _get_key(template_file, key='n_samples')
+
+        if not n_samples:
+            raise ValueError('`create.sampler.n_samples` must be defined for '
+                             'jintrac `v210921` config')
+
+        return n_samples
+
+    def add_system_attrs(self, *, handle: ImasHandle, run: SimpleNamespace):
+        """Add system specific attributes to run namespace."""
+        data_in_start = self.run_numbers[handle.db, handle.shot]
+        data_out_start = data_in_start + self.n_samples
+
+        self.run_numbers[handle.db,
+                         handle.shot] = data_out_start + self.n_samples
+
+        if self.run_numbers[handle.db, handle.shot] > self.MAX_RUN:
+            raise ValueError(
+                f'Cannot write data with run number > {self.MAX_RUN}')
+
+        run.data_in_start = data_in_start
+        run.data_out_start = data_out_start
+
+
+class Variables:
+    lookup = var_lookup.filter_type('IDS2jetto-variable')
+
+    def __init__(self, *, handle: ImasHandle):
+        self.handle = handle
+        self._ids_cache: dict[str, IDSMapping] = {}
+
+    def _get_ids(self, ids: str):
+        """Cache ids lookups to avoid repeated data reads."""
+        if ids in self._ids_cache:
+            mapping = self._ids_cache[ids]
+        else:
+            mapping = self.handle.get(ids)
+            self._ids_cache[ids] = mapping
+
+        return mapping
+
+    @staticmethod
+    def is_empty(value: Any) -> bool:
+        """Check against imasdef if variable is empty."""
+        if isinstance(value, float):
+            return value in (imasdef.EMPTY_FLOAT, imasdef.EMPTY_DOUBLE)
+        elif isinstance(value, int):
+            return value == imasdef.EMPTY_INT
+        elif isinstance(value, complex):
+            return value == imasdef.EMPTY_COMPLEX
+
+        return False
+
+    def __getattr__(self, key: str):
+        try:
+            spec = self.lookup[f'ids-{key}']
+        except KeyError as exc:
+            msg = f'Cannot find {key!r} in your variable listing (i.e. `variables.yaml`).'
+            raise AttributeError(msg) from exc
+
+        value = spec.default
+
+        for item in spec.paths:
+            mapping = self._get_ids(item.ids)
+            try:
+                trial = mapping[item.path]
+            except KeyError:
+                continue
+
+            if not self.is_empty(trial):
+                value = trial
+                break
+
+        if value is None:
+            raise AttributeError(
+                f'No value matches specifications given by: {spec}')
+
+        return value
+
+
+def substitute_templates(*, handles: dict[str, ImasHandle], template_file: str,
+                         force: bool):
+    """Handle template substitution.
+
+    Parameters
+    ----------
+    handles : dict[str, ImasHandle]
+        Dictionary with Imas handles
+    template_file : str
+        Path to template file.
+    force : bool
+        Overwrite files if set to true.
+    """
+    cwd = Path.cwd()
+
+    template = get_template(template_file)
+
+    if _get_key(template_file, key='system') == 'jetto-v210921':
+        add_system_attrs = ExtrasV210921(template_file).add_system_attrs
+    else:
+        add_system_attrs = no_op  # default to no-op
+
+    for name, handle in handles.items():
+        run = SimpleNamespace(name=name)
+
+        add_system_attrs(run=run, handle=handle)
+
+        variables = Variables(handle=handle)
+
+        cfg = template.render(run=run, variables=variables, handle=handle)
+
+        Config.parse_raw(cfg)  # make sure config is valid
+
+        out_drc = cwd / name
+
+        if out_drc.exists() and not force:
+            op_queue.add_no_op(description='Directory exists',
+                               extra_description=name)
+            op_queue.warning(description='Warning',
+                             extra_description='Some targets already exist, '
+                             'use --force to override')
+        else:
+            op_queue.add(
+                action=_generate_run_dir,
+                kwargs={
+                    'drc': out_drc,
+                    'cfg': cfg,
+                    'force': force
+                },
+                description='Setup run',
+                extra_description=name,
+            )
+
+
+def setup(*, handle, template_file, run_name, force, **kwargs):
+    """Setup large scale validation runs for template.
+
+    Parameters
+    ----------
+    handle : str
+        This is the handle to replace into the template.
+    template_file : Path
+        Path to the template file (jinja2 format).
+    run_name : str
+        Name of the output directory and run name.
+    force : bool
+        Set to true to overwrite previous files.
+    """
+    handles = {run_name: ImasHandle.from_string(handle)}
+
+    substitute_templates(handles=handles,
+                         template_file=template_file,
+                         force=force)
```

### Comparing `duqtools-1.6.4/src/duqtools/status.py` & `duqtools-1.7.0/src/duqtools/status.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import logging
-import subprocess as sp
-from collections import Counter
-from time import sleep
-from typing import Sequence
-
-from jetto_tools import config, template
-
-from .config import cfg
-from .jetto._system import jetto_lookup
-from .models import Job, JobStatus, Locations
-
-logger = logging.getLogger(__name__)
-info, debug = logger.info, logger.debug
-stream = logging.StreamHandler()
-stream.setFormatter(logging.Formatter('%(message)s'))
-logger.addHandler(stream)
-
-
-class StatusError(Exception):
-    ...
-
-
-class Status():
-
-    jobs: Sequence[Job]
-    jobs_submit: int
-    jobs_submitted: int
-    jobs_status: int
-    jobs_failed: int
-    jobs_running: int
-    jobs_unknown: int
-
-    def __init__(self, jobs=Sequence[Job]):
-        self.jobs = jobs
-
-        debug('Case directories: %s', self.jobs)
-
-        debug('Total number of jobs: %i', len(self.jobs))
-
-    def update_status(self):
-
-        self.n_submit_script = sum(job.has_submit_script for job in self.jobs)
-        self.n_status = sum(job.has_status for job in self.jobs)
-
-        counter = Counter(job.status() for job in self.jobs)
-
-        self.n_submitted = counter[JobStatus.SUBMITTED]
-        self.n_completed = counter[JobStatus.COMPLETED]
-        self.n_running = counter[JobStatus.RUNNING]
-        self.n_failed = counter[JobStatus.FAILED]
-        self.n_unknown = counter[JobStatus.UNKNOWN]
-
-    def simple_status(self):
-        """stateless status."""
-        self.update_status()
-
-        msg = 'Total number of directories with %-17s : %i'
-
-        info(msg, 'submit script', self.n_submit_script)
-        info(msg, 'unsubmitted jobs', self.n_submit_script - self.n_status)
-        info(msg, 'status script', self.n_status)
-        info(msg, 'completed status', self.n_completed)
-        info(msg, 'failed status', self.n_failed)
-        info(msg, 'running status', self.n_running)
-        info(msg, 'unknown status', self.n_unknown)
-
-    def progress_status(self):
-        """Monitor the directory for status changes."""
-        from tqdm import tqdm
-        pbar_a = tqdm(total=len(self.jobs), position=0)
-        pbar_a.set_description('Submitted jobs            ...')
-        pbar_b = tqdm(total=self.n_submit_script, position=1)
-        pbar_b.set_description('Running jobs              ...')
-        pbar_c = tqdm(total=self.n_submit_script, position=2)
-        pbar_c.set_description('Completed jobs            ...')
-        pbar_d = tqdm(total=self.n_submit_script, position=3)
-        pbar_d.set_description('Failed? jobs              ...')
-        while self.n_completed < self.n_submit_script:
-            pbar_a.n = self.n_submitted
-            pbar_b.n = self.n_running
-            pbar_c.n = self.n_completed
-            pbar_d.n = self.n_failed + self.n_unknown
-            pbar_a.refresh()
-            pbar_b.refresh()
-            pbar_c.refresh()
-            pbar_d.refresh()
-            sleep(5)
-            self.update_status()
-
-    def detailed_status(self):
-        from tqdm import tqdm
-        """detailed_status of all separate runs."""
-        monitors = []
-        for i, job in enumerate(self.jobs):
-            pbar = tqdm(total=100, position=i)
-            monitor = Monitor(pbar=pbar, job=job)
-            monitors.append(monitor)
-
-        while not all([monitor.finished for monitor in monitors]):
-            for monitor in monitors:
-                monitor.update()
-            sleep(5)
-
-
-class Monitor():
-    """Convenience class to keep track of submissions and update progress
-    bars."""
-
-    def __init__(self, pbar, job):
-        self.pbar = pbar
-        self.job = job
-        self.outfile = None
-
-        jetto_template = template.from_directory(job.dir)
-        jetto_template.lookup.update(jetto_lookup)
-        jetto_config = config.RunConfig(jetto_template)
-
-        self.check_kwmain_flag(jetto_config)
-
-        infile = job.in_file
-        if not infile.exists():
-            debug('%s does not exist, but the job is running', infile)
-            return
-
-        self.start = jetto_config.start_time
-        self.end = jetto_config.end_time
-        self.time = self.start
-
-        self.finished = False
-
-        self.set_status()
-
-    def check_kwmain_flag(self, jetto_config):
-        """Check for NLIST2/KWMAIN in jetto.jset. If this flag is not set, the
-        output in `job.out_file` does not contain the output that is grepped
-        for the progress.
-
-        More info: https://github.com/duqtools/duqtools/issues/337
-        """
-        msg = ('Cannot show detailed status, `nlist2.KWMAIN` flag'
-               ' is not set to 1 in `{self.job.status_file}`')
-        if jetto_config['kwmain'] != 1:
-            raise StatusError(msg)
-
-    def set_status(self):
-        status = self.job.status()
-
-        self.pbar.set_description(f'{self.job.dir.name:8s}, {status:12s}')
-        self.pbar.refresh()
-
-        return status
-
-    def get_steptime(self):
-        if not self.job.out_file.exists():
-            debug(
-                f'{self.job.out_file} does not exists, but the job is running')
-            return None
-
-        of = self.job.out_file
-        cmd = f'tac {of} | grep -m 1 ^\\s*STEP'
-        ret = sp.run(cmd, shell=True, capture_output=True)
-        if len(ret.stdout) > 0:
-            return float(ret.stdout.split('=')[2].lstrip(' ').split(' ')[0])
-        return None
-
-    def update(self):
-        status = self.set_status()
-        if status in (JobStatus.COMPLETED, JobStatus.FAILED):
-            self.pbar.n = 100 if status == JobStatus.COMPLETED else 0
-            self.pbar.refresh()
-            self.finished = True
-            return
-        if not status == JobStatus.RUNNING:
-            return
-
-        steptime = self.get_steptime()
-        if steptime:
-            self.time = steptime
-
-        self.pbar.n = int(100 * (self.time - self.start) /
-                          (self.end - self.start))
-        self.pbar.refresh()
-
-
-def status(*, progress: bool, detailed: bool, **kwargs):
-    """Show status of runs.
-
-    Parameters
-    ----------
-    progress : bool
-        Show progress bar.
-    detailed : bool
-        Show detailed progress for every job.
-    """
-    debug('Submit config: %s', cfg.submit)
-
-    runs = Locations().runs
-    jobs = [Job(run.dirname) for run in runs]
-
-    tracker = Status(jobs)
-
-    if detailed:
-        tracker.detailed_status()
-    elif progress:
-        tracker.progress_status()
-    else:
-        tracker.simple_status()
+import logging
+import subprocess as sp
+from collections import Counter
+from time import sleep
+from typing import Sequence
+
+from jetto_tools import config, template
+
+from .config import cfg
+from .jetto._system import jetto_lookup
+from .models import Job, JobStatus, Locations
+
+logger = logging.getLogger(__name__)
+info, debug = logger.info, logger.debug
+stream = logging.StreamHandler()
+stream.setFormatter(logging.Formatter('%(message)s'))
+logger.addHandler(stream)
+
+
+class StatusError(Exception):
+    ...
+
+
+class Status():
+
+    jobs: Sequence[Job]
+    jobs_submit: int
+    jobs_submitted: int
+    jobs_status: int
+    jobs_failed: int
+    jobs_running: int
+    jobs_unknown: int
+
+    def __init__(self, jobs=Sequence[Job]):
+        self.jobs = jobs
+
+        debug('Case directories: %s', self.jobs)
+
+        debug('Total number of jobs: %i', len(self.jobs))
+
+    def update_status(self):
+
+        self.n_submit_script = sum(job.has_submit_script for job in self.jobs)
+        self.n_status = sum(job.has_status for job in self.jobs)
+
+        counter = Counter(job.status() for job in self.jobs)
+
+        self.n_submitted = counter[JobStatus.SUBMITTED]
+        self.n_completed = counter[JobStatus.COMPLETED]
+        self.n_running = counter[JobStatus.RUNNING]
+        self.n_failed = counter[JobStatus.FAILED]
+        self.n_unknown = counter[JobStatus.UNKNOWN]
+
+    def simple_status(self):
+        """stateless status."""
+        self.update_status()
+
+        msg = 'Total number of directories with %-17s : %i'
+
+        info(msg, 'submit script', self.n_submit_script)
+        info(msg, 'unsubmitted jobs', self.n_submit_script - self.n_status)
+        info(msg, 'status script', self.n_status)
+        info(msg, 'completed status', self.n_completed)
+        info(msg, 'failed status', self.n_failed)
+        info(msg, 'running status', self.n_running)
+        info(msg, 'unknown status', self.n_unknown)
+
+    def progress_status(self):
+        """Monitor the directory for status changes."""
+        from tqdm import tqdm
+        pbar_a = tqdm(total=len(self.jobs), position=0)
+        pbar_a.set_description('Submitted jobs            ...')
+        pbar_b = tqdm(total=self.n_submit_script, position=1)
+        pbar_b.set_description('Running jobs              ...')
+        pbar_c = tqdm(total=self.n_submit_script, position=2)
+        pbar_c.set_description('Completed jobs            ...')
+        pbar_d = tqdm(total=self.n_submit_script, position=3)
+        pbar_d.set_description('Failed? jobs              ...')
+        while self.n_completed < self.n_submit_script:
+            pbar_a.n = self.n_submitted
+            pbar_b.n = self.n_running
+            pbar_c.n = self.n_completed
+            pbar_d.n = self.n_failed + self.n_unknown
+            pbar_a.refresh()
+            pbar_b.refresh()
+            pbar_c.refresh()
+            pbar_d.refresh()
+            sleep(5)
+            self.update_status()
+
+    def detailed_status(self):
+        from tqdm import tqdm
+        """detailed_status of all separate runs."""
+        monitors = []
+        for i, job in enumerate(self.jobs):
+            pbar = tqdm(total=100, position=i)
+            monitor = Monitor(pbar=pbar, job=job)
+            monitors.append(monitor)
+
+        while not all([monitor.finished for monitor in monitors]):
+            for monitor in monitors:
+                monitor.update()
+            sleep(5)
+
+
+class Monitor():
+    """Convenience class to keep track of submissions and update progress
+    bars."""
+
+    def __init__(self, pbar, job):
+        self.pbar = pbar
+        self.job = job
+        self.outfile = None
+
+        jetto_template = template.from_directory(job.dir)
+        jetto_template.lookup.update(jetto_lookup)
+        jetto_config = config.RunConfig(jetto_template)
+
+        self.check_kwmain_flag(jetto_config)
+
+        infile = job.in_file
+        if not infile.exists():
+            debug('%s does not exist, but the job is running', infile)
+            return
+
+        self.start = jetto_config.start_time
+        self.end = jetto_config.end_time
+        self.time = self.start
+
+        self.finished = False
+
+        self.set_status()
+
+    def check_kwmain_flag(self, jetto_config):
+        """Check for NLIST2/KWMAIN in jetto.jset. If this flag is not set, the
+        output in `job.out_file` does not contain the output that is grepped
+        for the progress.
+
+        More info: https://github.com/duqtools/duqtools/issues/337
+        """
+        msg = ('Cannot show detailed status, `nlist2.KWMAIN` flag'
+               ' is not set to 1 in `{self.job.status_file}`')
+        if jetto_config['kwmain'] != 1:
+            raise StatusError(msg)
+
+    def set_status(self):
+        status = self.job.status()
+
+        self.pbar.set_description(f'{self.job.dir.name:8s}, {status:12s}')
+        self.pbar.refresh()
+
+        return status
+
+    def get_steptime(self):
+        if not self.job.out_file.exists():
+            debug(
+                f'{self.job.out_file} does not exists, but the job is running')
+            return None
+
+        of = self.job.out_file
+        cmd = f'tac {of} | grep -m 1 ^\\s*STEP'
+        ret = sp.run(cmd, shell=True, capture_output=True)
+        if len(ret.stdout) > 0:
+            return float(ret.stdout.split('=')[2].lstrip(' ').split(' ')[0])
+        return None
+
+    def update(self):
+        status = self.set_status()
+        if status in (JobStatus.COMPLETED, JobStatus.FAILED):
+            self.pbar.n = 100 if status == JobStatus.COMPLETED else 0
+            self.pbar.refresh()
+            self.finished = True
+            return
+        if not status == JobStatus.RUNNING:
+            return
+
+        steptime = self.get_steptime()
+        if steptime:
+            self.time = steptime
+
+        self.pbar.n = int(100 * (self.time - self.start) /
+                          (self.end - self.start))
+        self.pbar.refresh()
+
+
+def status(*, progress: bool, detailed: bool, **kwargs):
+    """Show status of runs.
+
+    Parameters
+    ----------
+    progress : bool
+        Show progress bar.
+    detailed : bool
+        Show detailed progress for every job.
+    """
+    debug('Submit config: %s', cfg.submit)
+
+    runs = Locations().runs
+    jobs = [Job(run.dirname) for run in runs]
+
+    tracker = Status(jobs)
+
+    if detailed:
+        tracker.detailed_status()
+    elif progress:
+        tracker.progress_status()
+    else:
+        tracker.simple_status()
```

### Comparing `duqtools-1.6.4/src/duqtools/submit.py` & `duqtools-1.7.0/src/duqtools/submit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,224 +1,228 @@
-import logging
-import time
-from collections import deque
-from itertools import cycle
-from pathlib import Path
-from typing import Deque, Sequence
-
-from ._logging_utils import duqlog_screen
-from .config import cfg
-from .models import Job, Locations
-from .operations import add_to_op_queue, op_queue
-from .system import get_system
-
-logger = logging.getLogger(__name__)
-info, debug = logger.info, logger.debug
-
-
-class SubmitError(Exception):
-    ...
-
-
-def Spinner(frames='⠋⠙⠹⠸⠼⠴⠦⠧⠇⠏'):
-    """Simple spinner animation."""
-    yield from cycle(frames)
-
-
-@add_to_op_queue('Submitting', '{job}')
-def _submit_job(job: Job, *, delay: float = 0):
-    """
-    Parameters
-    ----------
-    delay : float
-        Add a delay to avoid all jobs starting at the same time.
-        This causes issues with slurm, for example.
-    """
-    if delay:
-        time.sleep(delay)
-    job.submit()
-
-
-def job_submitter(jobs: Sequence[Job], *, max_jobs):
-    for n, job in enumerate(jobs):
-        if max_jobs and (n >= max_jobs):
-            info(f'Max jobs ({max_jobs}) reached.')
-            break
-
-        _submit_job(job, delay=0.1)
-
-
-@add_to_op_queue('Start job scheduler')
-def job_scheduler(queue: Deque[Job], max_jobs=10):
-    interval = 1.0
-
-    s = Spinner()
-
-    tasks: Deque[Job] = deque()
-    completed: Deque[Job] = deque()
-
-    while tasks or queue:
-        while queue and len(tasks) < max_jobs:
-            job = queue.popleft()
-            task = job.start()
-            tasks.append(task)
-            # starting jobs at the same time causes issues
-            time.sleep(0.1)
-
-        time.sleep(interval)
-        task = tasks.popleft()
-        try:
-            next(task)  # Run to the next yield
-            tasks.append(task)  # Reschedule
-        except StopIteration:
-            completed.append(task)
-
-        print(
-            f' {next(s)} Running: {len(tasks)},'
-            f' queue: {len(queue)}, completed: {len(completed)}',
-            end='\033[K\r',
-        )
-
-
-def job_array_submitter(jobs: Sequence[Job], *, max_jobs):
-    if len(jobs) == 0:
-        duqlog_screen.error('No jobs to submit, not creating array ...')
-        return
-
-    for job in jobs:
-        op_queue.add(action=lambda: None,
-                     description='Adding to array',
-                     extra_description=f'{job}')
-
-    if not max_jobs:
-        logger.info('Max jobs not specified, defaulting to 10')
-        max_jobs = 10
-
-    get_system().submit_array(jobs, max_jobs)
-
-
-def submission_script_ok(job):
-    submission_script = job.submit_script
-    if not submission_script.is_file():
-        info('Did not found submission script %s ; Skipping directory...',
-             submission_script)
-        return False
-
-    return True
-
-
-def status_file_ok(job, *, force):
-    status_file = job.status_file
-    if job.has_status and not force:
-        if not status_file.is_file():
-            logger.warning('Status file %s is not a file', status_file)
-        with open(status_file) as f:
-            info('Status of %s: %s. To rerun enable the --force flag',
-                 status_file, f.read())
-        op_queue.add_no_op(
-            description='Not Submitting',
-            extra_description=f'{job} (reason: status file exists)')
-        return False
-
-    return True
-
-
-def lockfile_ok(job, *, force):
-    lockfile = job.lockfile
-    if lockfile.exists() and not force:
-        op_queue.add_no_op(
-            description='Not Submitting',
-            extra_description=f'{job} (reason: {lockfile} exists)')
-        return False
-
-    return True
-
-
-def get_resubmit_jobs(resubmit_names: Sequence[Path]) -> list[Job]:
-    """get_resubmit_jobs.
-
-    Parameters
-    ----------
-    resubmit_names : Sequence[Path]
-        The names (short or full path) of the jobs that need to be resubmitted
-
-    Returns
-    -------
-    list[Job]
-    """
-    jobs: list[Job] = []
-    run_dict = {run.shortname: run for run in Locations().runs}
-    for name in resubmit_names:
-        if name in run_dict:  # check for shortname
-            jobs.append(Job(run_dict[name].dirname))
-        else:
-            # It's not a short name, use the argument as the full path to the job
-            jobs.append(Job(Path(name)))
-    return jobs
-
-
-def submit(*,
-           force: bool,
-           max_jobs: int,
-           schedule: bool,
-           array: bool,
-           resubmit: Sequence[Path] = (),
-           status_filter: Sequence[str],
-           **kwargs):
-    """submit. Function which implements the functionality to submit jobs to
-    the cluster.
-
-    Parameters
-    ----------
-    force : bool
-        Force the submission even in the presence of lockfiles
-    max_jobs : int
-        Maximum number of jobs to submit at once
-    schedule : bool
-        Schedule `max_jobs` to run at once, keeps the process alive until
-        finished.
-    array : bool
-        Submit the jobs as a single array
-    resubmit : Sequence[Path]
-        If any jobs need to be resubmitted, this is has a nonzero length, and
-        contains a Sequence of Paths which either are the full Path to the run
-        that needs to be resubmitted, or the shortname
-    status_filter : list[str]
-        Only submit jobs with this status.
-    """
-    if not cfg.submit:
-        raise SubmitError('Submit field required in config file')
-
-    debug('Submit config: %s', cfg.submit)
-
-    if resubmit:
-        jobs = get_resubmit_jobs(resubmit)
-        force = True
-    else:
-        jobs = [Job(run.dirname) for run in Locations().runs]
-
-    debug('Case directories: %s', jobs)
-
-    job_queue: Deque[Job] = deque()
-
-    for job in jobs:
-        status = job.status()
-
-        if status_filter and (status not in status_filter):
-            continue
-        if not status_file_ok(job, force=force):
-            continue
-        if not lockfile_ok(job, force=force):
-            continue
-        job_queue.append(job)
-
-    if array and Path('./duqtools_slurm_array.sh').exists() and not force:
-        op_queue.add_no_op(
-            description='Not Creating Array',
-            extra_description='(reason: duqtools_slurm_array.sh exists)')
-        op_queue.add_no_op(description='Not Submitting Array',
-                           extra_description='use --force to override')
-        return
-
-    submitter = job_scheduler if schedule else job_submitter
-    submitter = job_array_submitter if array else submitter
-    submitter(job_queue, max_jobs=max_jobs)
+import logging
+import time
+from collections import deque
+from itertools import cycle
+from pathlib import Path
+from typing import Deque, Sequence
+
+from ._logging_utils import duqlog_screen
+from .config import cfg
+from .models import Job, Locations
+from .operations import add_to_op_queue, op_queue
+from .system import get_system
+
+logger = logging.getLogger(__name__)
+info, debug = logger.info, logger.debug
+
+
+class SubmitError(Exception):
+    ...
+
+
+def Spinner(frames='⠋⠙⠹⠸⠼⠴⠦⠧⠇⠏'):
+    """Simple spinner animation."""
+    yield from cycle(frames)
+
+
+@add_to_op_queue('Submitting', '{job}')
+def _submit_job(job: Job, *, delay: float = 0):
+    """
+    Parameters
+    ----------
+    delay : float
+        Add a delay to avoid all jobs starting at the same time.
+        This causes issues with slurm, for example.
+    """
+    if delay:
+        time.sleep(delay)
+    job.submit()
+
+
+def job_submitter(jobs: Sequence[Job], *, max_jobs, **kwargs):
+    for n, job in enumerate(jobs):
+        if max_jobs and (n >= max_jobs):
+            info(f'Max jobs ({max_jobs}) reached.')
+            break
+
+        _submit_job(job, delay=0.1)
+
+
+@add_to_op_queue('Start job scheduler')
+def job_scheduler(queue: Deque[Job], max_jobs=10, **kwargs):
+    interval = 1.0
+
+    s = Spinner()
+
+    tasks: Deque[Job] = deque()
+    completed: Deque[Job] = deque()
+
+    while tasks or queue:
+        while queue and len(tasks) < max_jobs:
+            job = queue.popleft()
+            task = job.start()
+            tasks.append(task)
+            # starting jobs at the same time causes issues
+            time.sleep(0.1)
+
+        time.sleep(interval)
+        task = tasks.popleft()
+        try:
+            next(task)  # Run to the next yield
+            tasks.append(task)  # Reschedule
+        except StopIteration:
+            completed.append(task)
+
+        print(
+            f' {next(s)} Running: {len(tasks)},'
+            f' queue: {len(queue)}, completed: {len(completed)}',
+            end='\033[K\r',
+        )
+
+
+def job_array_submitter(jobs: Sequence[Job], *, max_jobs, max_array_size,
+                        **kwargs):
+    if len(jobs) == 0:
+        duqlog_screen.error('No jobs to submit, not creating array ...')
+        return
+
+    for job in jobs:
+        op_queue.add(action=lambda: None,
+                     description='Adding to array',
+                     extra_description=f'{job}')
+
+    if not max_jobs:
+        logger.info('Max jobs not specified, defaulting to 10')
+        max_jobs = 10
+
+    get_system().submit_array(jobs, max_jobs, max_array_size)
+
+
+def submission_script_ok(job):
+    submission_script = job.submit_script
+    if not submission_script.is_file():
+        info('Did not found submission script %s ; Skipping directory...',
+             submission_script)
+        return False
+
+    return True
+
+
+def status_file_ok(job, *, force):
+    status_file = job.status_file
+    if job.has_status and not force:
+        if not status_file.is_file():
+            logger.warning('Status file %s is not a file', status_file)
+        with open(status_file) as f:
+            info('Status of %s: %s. To rerun enable the --force flag',
+                 status_file, f.read())
+        op_queue.add_no_op(
+            description='Not Submitting',
+            extra_description=f'{job} (reason: status file exists)')
+        return False
+
+    return True
+
+
+def lockfile_ok(job, *, force):
+    lockfile = job.lockfile
+    if lockfile.exists() and not force:
+        op_queue.add_no_op(
+            description='Not Submitting',
+            extra_description=f'{job} (reason: {lockfile} exists)')
+        return False
+
+    return True
+
+
+def get_resubmit_jobs(resubmit_names: Sequence[Path]) -> list[Job]:
+    """get_resubmit_jobs.
+
+    Parameters
+    ----------
+    resubmit_names : Sequence[Path]
+        The names (short or full path) of the jobs that need to be resubmitted
+
+    Returns
+    -------
+    list[Job]
+    """
+    jobs: list[Job] = []
+    run_dict = {run.shortname: run for run in Locations().runs}
+    for name in resubmit_names:
+        if name in run_dict:  # check for shortname
+            jobs.append(Job(run_dict[name].dirname))
+        else:
+            # It's not a short name, use the argument as the full path to the job
+            jobs.append(Job(Path(name)))
+    return jobs
+
+
+def submit(*,
+           force: bool,
+           max_jobs: int,
+           max_array_size: int,
+           schedule: bool,
+           array: bool,
+           resubmit: Sequence[Path] = (),
+           status_filter: Sequence[str],
+           **kwargs):
+    """submit. Function which implements the functionality to submit jobs to
+    the cluster.
+
+    Parameters
+    ----------
+    force : bool
+        Force the submission even in the presence of lockfiles
+    max_jobs : int
+        Maximum number of jobs to submit at once
+    max_array_size : int
+        Maximum array size for slurm (usually 1001, default = 100)
+    schedule : bool
+        Schedule `max_jobs` to run at once, keeps the process alive until
+        finished.
+    array : bool
+        Submit the jobs as a single array
+    resubmit : Sequence[Path]
+        If any jobs need to be resubmitted, this is has a nonzero length, and
+        contains a Sequence of Paths which either are the full Path to the run
+        that needs to be resubmitted, or the shortname
+    status_filter : list[str]
+        Only submit jobs with this status.
+    """
+    if not cfg.submit:
+        raise SubmitError('Submit field required in config file')
+
+    debug('Submit config: %s', cfg.submit)
+
+    if resubmit:
+        jobs = get_resubmit_jobs(resubmit)
+        force = True
+    else:
+        jobs = [Job(run.dirname) for run in Locations().runs]
+
+    debug('Case directories: %s', jobs)
+
+    job_queue: Deque[Job] = deque()
+
+    for job in jobs:
+        status = job.status()
+
+        if status_filter and (status not in status_filter):
+            continue
+        if not status_file_ok(job, force=force):
+            continue
+        if not lockfile_ok(job, force=force):
+            continue
+        job_queue.append(job)
+
+    if array and Path('./duqtools_slurm_array.sh').exists() and not force:
+        op_queue.add_no_op(
+            description='Not Creating Array',
+            extra_description='(reason: duqtools_slurm_array.sh exists)')
+        op_queue.add_no_op(description='Not Submitting Array',
+                           extra_description='use --force to override')
+        return
+
+    submitter = job_scheduler if schedule else job_submitter
+    submitter = job_array_submitter if array else submitter
+    submitter(job_queue, max_jobs=max_jobs, max_array_size=max_array_size)
```

### Comparing `duqtools-1.6.4/src/duqtools/system.py` & `duqtools-1.7.0/src/duqtools/system.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from pathlib import Path
-
-from .config import Config, cfg
-from .ids import ImasHandle
-from .jetto import JettoSystemV210921, JettoSystemV220922
-from .models import AbstractSystem, Job
-
-
-class DummySystem(AbstractSystem):
-    """This is a dummy system that implements the basic interfaces.
-
-    It exists for testing purposes in absence of actual modelling
-    software.
-    """
-
-    @staticmethod
-    def get_runs_dir() -> Path:
-        return Path()
-
-    @staticmethod
-    def write_batchfile(run_dir: Path, cfg: Config):
-        pass
-
-    @staticmethod
-    def submit_job(job: Job):
-        pass
-
-    @staticmethod
-    def copy_from_template(source_drc: Path, target_drc: Path):
-        pass
-
-    @staticmethod
-    def imas_from_path(template_drc: Path):
-        return ImasHandle(db='', shot='-1', run='-1')
-
-    @staticmethod
-    def update_imas_locations(run: Path, inp, out):
-        pass
-
-
-def get_system():
-    """get_system.
-
-    Get the system to do operations with TODO make it a variable, not a
-    function
-    """
-    if (cfg.system in ['jetto', 'jetto-v220922']):
-        return JettoSystemV220922
-    elif (cfg.system in ['jetto-v210921']):
-        return JettoSystemV210921
-    elif (cfg.system == 'dummy'):
-        return DummySystem
-    else:
-        raise NotImplementedError(f'system {cfg.system} is not implemented')
+from pathlib import Path
+
+from .config import Config, cfg
+from .ids import ImasHandle
+from .jetto import JettoSystemV210921, JettoSystemV220922
+from .models import AbstractSystem, Job
+
+
+class DummySystem(AbstractSystem):
+    """This is a dummy system that implements the basic interfaces.
+
+    It exists for testing purposes in absence of actual modelling
+    software.
+    """
+
+    @staticmethod
+    def get_runs_dir() -> Path:
+        return Path()
+
+    @staticmethod
+    def write_batchfile(run_dir: Path, cfg: Config):
+        pass
+
+    @staticmethod
+    def submit_job(job: Job):
+        pass
+
+    @staticmethod
+    def copy_from_template(source_drc: Path, target_drc: Path):
+        pass
+
+    @staticmethod
+    def imas_from_path(template_drc: Path):
+        return ImasHandle(db='', shot='-1', run='-1')
+
+    @staticmethod
+    def update_imas_locations(run: Path, inp, out):
+        pass
+
+
+def get_system():
+    """get_system.
+
+    Get the system to do operations with TODO make it a variable, not a
+    function
+    """
+    if (cfg.system in ['jetto', 'jetto-v220922']):
+        return JettoSystemV220922
+    elif (cfg.system in ['jetto-v210921']):
+        return JettoSystemV210921
+    elif (cfg.system == 'dummy'):
+        return DummySystem
+    else:
+        raise NotImplementedError(f'system {cfg.system} is not implemented')
```

### Comparing `duqtools-1.6.4/src/duqtools/utils.py` & `duqtools-1.7.0/src/duqtools/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-from __future__ import annotations
-
-import os
-from collections import defaultdict
-from contextlib import contextmanager
-from itertools import filterfalse, tee
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Hashable, Iterable
-
-from ._types import PathLike
-from .schema.runs import Runs
-
-if TYPE_CHECKING:
-    from .ids import ImasHandle
-
-
-def no_op(*args, **kwargs):
-    """Do nothing."""
-    pass
-
-
-@contextmanager
-def work_directory(path: PathLike):
-    """Changes working directory and returns to previous on exit.
-
-    Parameters
-    ----------
-    path : PathLike
-        Temporarily change to this directory.
-    """
-    prev_cwd = Path.cwd().resolve()
-    try:
-        os.chdir(path)
-        yield
-    finally:  # In any case, no matter what happens, go back eventually
-        os.chdir(prev_cwd)
-
-
-def read_imas_handles_from_file(inp: PathLike, ) -> dict[str, ImasHandle]:
-    """Read a collection of imas paths from a file.
-
-    Input can be a `Runs.yaml` file `data.csv` file.
-
-    The CSV file must have contain at least 5 columns, including: `user`,
-    `db`, `shot`, and `run`. The first column is used as the index.
-    The index can be any string or number, as long as it uniquely
-    identifies the row.
-
-    Parameters
-    ----------
-    inp : PathLike
-        Name of the file to read.
-    as_dataframe : bool, optional
-        Return imas handles in a dataframe instead.
-
-    Returns
-    -------
-    Union[dict[str, ImasHandle], 'pd.DataFrame']
-        Returns a dict with the Imas handles.
-
-    Raises
-    ------
-    ValueError
-        When the file cannot be opened.
-    """
-    import csv
-
-    from .ids import ImasHandle
-
-    inp = Path(inp)
-
-    if inp.suffix == '.csv':
-        handles = {}
-        with open(inp) as f:
-            has_header = csv.Sniffer().has_header(f.read(1024))
-            f.seek(0)
-
-            if not has_header:
-                raise IOError(
-                    f'`{inp}` does not have a header. Expecting at least'
-                    '`user`,`db`,`shot`,`run`.')
-
-            reader = csv.DictReader(f)
-
-            index_col = reader.fieldnames[0]  # type: ignore
-
-            for row in reader:
-                index = row.pop(index_col)
-                handles[index] = ImasHandle(**row)
-
-    elif inp.name == 'runs.yaml':
-        runs = Runs.parse_file(inp)
-        handles = {
-            str(run.dirname): ImasHandle.parse_obj(run.data_out)
-            for run in runs
-        }
-
-    else:
-        raise ValueError(f'Cannot open file: {inp}')
-
-    return handles
-
-
-def groupby(iterable: Iterable,
-            keyfunc: Callable) -> dict[Hashable, list[Any]]:
-    """Group iterable by key function. The items are grouped by the value that
-    is returned by the `keyfunc`
-
-    Parameters
-    ----------
-    iterable : list, tuple or iterable
-        List of items to group
-    keyfunc : callable
-        Used to determine the group of each item. These become the keys
-        of the returned dictionary
-
-    Returns
-    -------
-    grouped : dict
-        Returns a dictionary with the grouped values.
-    """
-    grouped = defaultdict(list)
-    for item in iterable:
-        key = keyfunc(item)
-        grouped[key].append(item)
-
-    return grouped
-
-
-def partition(pred: Callable, iterable: Iterable) -> tuple[Iterable, Iterable]:
-    """Use a predicate to partition entries into false entries and true
-    entries.
-
-    partition(is_odd, range(10)) --> 0 2 4 6 8   and  1 3 5 7 9
-
-    From: https://docs.python.org/3/library/itertools.html
-
-    Parameters
-    ----------
-    pred : Callable
-        Filter function called on every entry in the iterable to determine
-        whether to put it in the false or true bin
-    iterable : Iterable
-        List of items to partition
-
-    Returns
-    -------
-    tuple[Iterable, Iterable]
-        Two sequences with false and true entries, respectively.
-    """
-    t1, t2 = tee(iterable)
-    return filterfalse(pred, t1), filter(pred, t2)
+from __future__ import annotations
+
+import os
+from collections import defaultdict
+from contextlib import contextmanager
+from itertools import filterfalse, tee
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, Hashable, Iterable
+
+from ._types import PathLike
+
+if TYPE_CHECKING:
+    from .ids import ImasHandle
+
+
+def no_op(*args, **kwargs):
+    """Do nothing."""
+    pass
+
+
+@contextmanager
+def work_directory(path: PathLike):
+    """Changes working directory and returns to previous on exit.
+
+    Parameters
+    ----------
+    path : PathLike
+        Temporarily change to this directory.
+    """
+    prev_cwd = Path.cwd().resolve()
+    try:
+        os.chdir(path)
+        yield
+    finally:  # In any case, no matter what happens, go back eventually
+        os.chdir(prev_cwd)
+
+
+def read_imas_handles_from_file(inp: PathLike, ) -> dict[str, ImasHandle]:
+    """Read a collection of imas paths from a file.
+
+    Input can be a `Runs.yaml` file `data.csv` file.
+
+    The CSV file must have contain at least 5 columns, including: `user`,
+    `db`, `shot`, and `run`. The first column is used as the index.
+    The index can be any string or number, as long as it uniquely
+    identifies the row.
+
+    Parameters
+    ----------
+    inp : PathLike
+        Name of the file to read.
+    as_dataframe : bool, optional
+        Return imas handles in a dataframe instead.
+
+    Returns
+    -------
+    Union[dict[str, ImasHandle], 'pd.DataFrame']
+        Returns a dict with the Imas handles.
+
+    Raises
+    ------
+    ValueError
+        When the file cannot be opened.
+    """
+    import csv
+
+    from .ids import ImasHandle
+    from .models import Runs
+
+    inp = Path(inp)
+
+    if inp.suffix == '.csv':
+        handles = {}
+        with open(inp) as f:
+            has_header = csv.Sniffer().has_header(f.read(1024))
+            f.seek(0)
+
+            if not has_header:
+                raise IOError(
+                    f'`{inp}` does not have a header. Expecting at least'
+                    '`user`,`db`,`shot`,`run`.')
+
+            reader = csv.DictReader(f)
+
+            index_col = reader.fieldnames[0]  # type: ignore
+
+            for row in reader:
+                index = row.pop(index_col)
+                handles[index] = ImasHandle(**row)
+
+    elif inp.name == 'runs.yaml':
+        runs = Runs.parse_file(inp)
+        handles = {
+            str(run.dirname): ImasHandle.parse_obj(run.data_out)
+            for run in runs
+        }
+
+    else:
+        raise ValueError(f'Cannot open file: {inp}')
+
+    return handles
+
+
+def groupby(iterable: Iterable,
+            keyfunc: Callable) -> dict[Hashable, list[Any]]:
+    """Group iterable by key function. The items are grouped by the value that
+    is returned by the `keyfunc`
+
+    Parameters
+    ----------
+    iterable : list, tuple or iterable
+        List of items to group
+    keyfunc : callable
+        Used to determine the group of each item. These become the keys
+        of the returned dictionary
+
+    Returns
+    -------
+    grouped : dict
+        Returns a dictionary with the grouped values.
+    """
+    grouped = defaultdict(list)
+    for item in iterable:
+        key = keyfunc(item)
+        grouped[key].append(item)
+
+    return grouped
+
+
+def partition(pred: Callable, iterable: Iterable) -> tuple[Iterable, Iterable]:
+    """Use a predicate to partition entries into false entries and true
+    entries.
+
+    partition(is_odd, range(10)) --> 0 2 4 6 8   and  1 3 5 7 9
+
+    From: https://docs.python.org/3/library/itertools.html
+
+    Parameters
+    ----------
+    pred : Callable
+        Filter function called on every entry in the iterable to determine
+        whether to put it in the false or true bin
+    iterable : Iterable
+        List of items to partition
+
+    Returns
+    -------
+    tuple[Iterable, Iterable]
+        Two sequences with false and true entries, respectively.
+    """
+    t1, t2 = tee(iterable)
+    return filterfalse(pred, t1), filter(pred, t2)
```

### Comparing `duqtools-1.6.4/src/duqtools.egg-info/PKG-INFO` & `duqtools-1.7.0/src/duqtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,69 @@
-Metadata-Version: 2.1
-Name: duqtools
-Version: 1.6.4
-Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
-Home-page: https://github.com/duqtools/duqtools
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
-Project-URL: Documentation, https://duqtools.readthedocs.io
-Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-Provides-Extra: docs
-Provides-Extra: publishing
-Provides-Extra: imas
-License-File: LICENSE
-
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
-
-# Duqtools
-
-*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
-
-Features:
-
-- Set up 100s of simulation runs from a single template
-- Launch standard sets of sensitivity tests with minimal programming
-- Batch job submission and status tracking
-- Supports the Standardized Interface Data Structures (IDSs) data directory
-- Compare and visualize 100s of simulations in one overview
-- Display simulation results as confidence ranges and distributions
-
-*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
-
-To install:
-
-```console
-pip install duqtools
-```
-
-The source code is available from [Github](https://github.com/duqtools/duqtools).
-
-Suggestions, improvements, and edits are most welcome.
-
-
-## Development
-
-Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
+Metadata-Version: 2.1
+Name: duqtools
+Version: 1.7.0
+Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
+Home-page: https://github.com/duqtools/duqtools
+Author: Stef Smeets
+Author-email: s.smeets@esciencecenter.nl
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
+Project-URL: Documentation, https://duqtools.readthedocs.io
+Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+Provides-Extra: docs
+Provides-Extra: publishing
+Provides-Extra: imas
+License-File: LICENSE
+
+| Source | Badges |
+| --- | --- |
+| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
+| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
+| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
+| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
+| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+
+# Duqtools
+
+*Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
+
+Features:
+
+- Set up 100s of simulation runs from a single template
+- Launch standard sets of sensitivity tests with minimal programming
+- Batch job submission and status tracking
+- Supports the Standardized Interface Data Structures (IDSs) data directory
+- Compare and visualize 100s of simulations in one overview
+- Display simulation results as confidence ranges and distributions
+
+*Duqtools* is currently under active development. It runs on linux only and requires the [ITER](http://iter.org/) Integrated Modeling and Analysis Suite ([IMAS](https://confluence.iter.org/display/IMP)).
+
+To install:
+
+```console
+pip install duqtools
+```
+
+The source code is available from [Github](https://github.com/duqtools/duqtools).
+
+Suggestions, improvements, and edits are most welcome.
+
+
+## Development
+
+Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
+
+
```

### Comparing `duqtools-1.6.4/src/duqtools.egg-info/SOURCES.txt` & `duqtools-1.7.0/src/duqtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/duqtools/_types.py
 src/duqtools/api.py
 src/duqtools/apply_model.py
 src/duqtools/cleanup.py
 src/duqtools/cli.py
 src/duqtools/create.py
 src/duqtools/dash.py
+src/duqtools/duqmap.py
 src/duqtools/init.py
 src/duqtools/list_variables.py
 src/duqtools/matrix_samplers.py
 src/duqtools/merge.py
 src/duqtools/operations.py
 src/duqtools/plot.py
 src/duqtools/setup.py
@@ -66,27 +67,21 @@
 src/duqtools/large_scale_validation/merge.py
 src/duqtools/large_scale_validation/setup.py
 src/duqtools/large_scale_validation/status.py
 src/duqtools/large_scale_validation/submit.py
 src/duqtools/models/__init__.py
 src/duqtools/models/_job.py
 src/duqtools/models/_locations.py
+src/duqtools/models/_run.py
 src/duqtools/models/_system.py
 src/duqtools/schema/__init__.py
 src/duqtools/schema/_basemodel.py
 src/duqtools/schema/_description_helpers.py
 src/duqtools/schema/_dimensions.py
 src/duqtools/schema/_imas.py
 src/duqtools/schema/_jetto.py
 src/duqtools/schema/_ranges.py
 src/duqtools/schema/_variable.py
 src/duqtools/schema/cli.py
 src/duqtools/schema/data_location.py
 src/duqtools/schema/matrix_samplers.py
-src/duqtools/schema/runs.py
-src/duqtools/schema/variables.py
-tests/test_cmdline.py
-tests/test_dry_run.py
-tests/test_duqtools.py
-tests/test_ids2jetto_variables.py
-tests/test_operations.py
-tests/test_samplers.py
+src/duqtools/schema/variables.py
```

### Comparing `duqtools-1.6.4/src/duqtools.egg-info/requires.txt` & `duqtools-1.7.0/src/duqtools.egg-info/requires.txt`

 * *Files identical despite different names*

