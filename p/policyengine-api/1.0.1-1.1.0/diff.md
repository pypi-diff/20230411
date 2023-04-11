# Comparing `tmp/policyengine-api-1.0.1.tar.gz` & `tmp/policyengine-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-api-1.0.1.tar", last modified: Fri Apr  7 12:08:21 2023, max compression
+gzip compressed data, was "policyengine-api-1.1.0.tar", last modified: Tue Apr 11 13:00:59 2023, max compression
```

## Comparing `policyengine-api-1.0.1.tar` & `policyengine-api-1.1.0.tar`

### file list

```diff
@@ -1,78 +1,83 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.998529 policyengine-api-1.0.1/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.988125 policyengine-api-1.0.1/.github/
--rw-r--r--   0 nikhil     (501) staff       (20)      267 2022-12-19 15:37:36.000000 policyengine-api-1.0.1/.github/changelog_template.md
--rwxr-xr-x   0 nikhil     (501) staff       (20)      122 2022-12-19 15:37:36.000000 policyengine-api-1.0.1/.github/get-changelog-diff.sh
--rwxr-xr-x   0 nikhil     (501) staff       (20)      642 2022-12-19 15:37:36.000000 policyengine-api-1.0.1/.github/has-functional-changes.sh
--rwxr-xr-x   0 nikhil     (501) staff       (20)     1013 2022-12-19 15:37:36.000000 policyengine-api-1.0.1/.github/is-version-number-acceptable.sh
--rwxr-xr-x   0 nikhil     (501) staff       (20)      115 2022-12-19 15:37:36.000000 policyengine-api-1.0.1/.github/publish-git-tag.sh
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.988623 policyengine-api-1.0.1/.github/workflows/
--rw-r--r--   0 nikhil     (501) staff       (20)     1729 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/.github/workflows/pr.yml
--rw-r--r--   0 nikhil     (501) staff       (20)     2395 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/.github/workflows/push.yml
--rw-r--r--   0 nikhil     (501) staff       (20)      142 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/.gitignore
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.989002 policyengine-api-1.0.1/.vscode/
--rw-r--r--   0 nikhil     (501) staff       (20)      692 2022-11-22 22:32:04.000000 policyengine-api-1.0.1/.vscode/launch.json
--rw-r--r--   0 nikhil     (501) staff       (20)    30179 2023-04-07 12:06:14.000000 policyengine-api-1.0.1/CHANGELOG.md
--rw-r--r--   0 nikhil     (501) staff       (20)    34523 2022-12-06 22:08:46.000000 policyengine-api-1.0.1/LICENSE
--rw-r--r--   0 nikhil     (501) staff       (20)      826 2023-04-07 11:35:57.000000 policyengine-api-1.0.1/Makefile
--rw-r--r--   0 nikhil     (501) staff       (20)      211 2023-04-07 12:08:21.998283 policyengine-api-1.0.1/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      391 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/README.md
--rw-r--r--   0 nikhil     (501) staff       (20)    19239 2023-04-07 12:06:13.000000 policyengine-api-1.0.1/changelog.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)        0 2023-04-07 12:06:14.000000 policyengine-api-1.0.1/changelog_entry.yaml
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.989164 policyengine-api-1.0.1/dashboard/
--rw-r--r--   0 nikhil     (501) staff       (20)     1990 2023-01-11 13:17:41.000000 policyengine-api-1.0.1/dashboard/app.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.989489 policyengine-api-1.0.1/dashboard/experiments/
--rw-r--r--   0 nikhil     (501) staff       (20)     4252 2023-04-03 21:42:12.000000 policyengine-api-1.0.1/dashboard/experiments/gpt4_api_user.py
--rw-r--r--   0 nikhil     (501) staff       (20)       41 2023-04-03 21:42:12.000000 policyengine-api-1.0.1/dashboard/experiments/requirements.txt
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.990760 policyengine-api-1.0.1/gcp/
--rw-r--r--   0 nikhil     (501) staff       (20)      640 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/Dockerfile
--rw-r--r--   0 nikhil     (501) staff       (20)      697 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/README.md
--rw-r--r--   0 nikhil     (501) staff       (20)     2906 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/bump_country_package.py
--rw-r--r--   0 nikhil     (501) staff       (20)      133 2022-12-08 00:06:30.000000 policyengine-api-1.0.1/gcp/dispatch.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)     1129 2023-04-07 11:37:10.000000 policyengine-api-1.0.1/gcp/export.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.991466 policyengine-api-1.0.1/gcp/policyengine_api/
--rw-r--r--   0 nikhil     (501) staff       (20)      295 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/policyengine_api/Dockerfile
--rw-r--r--   0 nikhil     (501) staff       (20)      358 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/policyengine_api/app.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)      177 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/gcp/policyengine_api/start.sh
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.992384 policyengine-api-1.0.1/policyengine_api/
--rw-r--r--   0 nikhil     (501) staff       (20)     1783 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/api.py
--rw-r--r--   0 nikhil     (501) staff       (20)      611 2023-04-07 12:06:14.000000 policyengine-api-1.0.1/policyengine_api/constants.py
--rw-r--r--   0 nikhil     (501) staff       (20)    17718 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/country.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.994545 policyengine-api-1.0.1/policyengine_api/data/
--rw-r--r--   0 nikhil     (501) staff       (20)     2003 2023-04-04 11:36:53.000000 policyengine-api-1.0.1/policyengine_api/data/README.md
--rw-r--r--   0 nikhil     (501) staff       (20)       65 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/data/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     4488 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/data/data.py
--rw-r--r--   0 nikhil     (501) staff       (20)     1922 2023-04-04 11:36:53.000000 policyengine-api-1.0.1/policyengine_api/data/initialise.sql
--rw-r--r--   0 nikhil     (501) staff       (20)     2043 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/data/initialise_local.sql
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.995413 policyengine-api-1.0.1/policyengine_api/endpoints/
--rw-r--r--   0 nikhil     (501) staff       (20)      317 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)     3229 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/analysis.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.996203 policyengine-api-1.0.1/policyengine_api/endpoints/economy/
--rw-r--r--   0 nikhil     (501) staff       (20)       41 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/economy/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)    13764 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/economy/compare.py
--rw-r--r--   0 nikhil     (501) staff       (20)     6275 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/economy/economy.py
--rw-r--r--   0 nikhil     (501) staff       (20)     8300 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/economy/reform_impact.py
--rw-r--r--   0 nikhil     (501) staff       (20)     5846 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/economy/single_economy.py
--rw-r--r--   0 nikhil     (501) staff       (20)      258 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/home.py
--rw-r--r--   0 nikhil     (501) staff       (20)     7379 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/household.py
--rw-r--r--   0 nikhil     (501) staff       (20)      359 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/metadata.py
--rw-r--r--   0 nikhil     (501) staff       (20)     3769 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/endpoints/policy.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.996477 policyengine-api-1.0.1/policyengine_api/utils/
--rw-r--r--   0 nikhil     (501) staff       (20)       20 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/utils/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)      979 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/utils/json.py
--rw-r--r--   0 nikhil     (501) staff       (20)      282 2023-04-07 11:35:54.000000 policyengine-api-1.0.1/policyengine_api/worker.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.993431 policyengine-api-1.0.1/policyengine_api.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)      211 2023-04-07 12:08:21.000000 policyengine-api-1.0.1/policyengine_api.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)     1811 2023-04-07 12:08:21.000000 policyengine-api-1.0.1/policyengine_api.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2023-04-07 12:08:21.000000 policyengine-api-1.0.1/policyengine_api.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      284 2023-04-07 12:08:21.000000 policyengine-api-1.0.1/policyengine_api.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2023-04-07 12:08:21.000000 policyengine-api-1.0.1/policyengine_api.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2023-04-07 12:08:21.998592 policyengine-api-1.0.1/setup.cfg
--rw-r--r--   0 nikhil     (501) staff       (20)      807 2023-04-07 12:06:14.000000 policyengine-api-1.0.1/setup.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.985626 policyengine-api-1.0.1/tests/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-07 12:08:21.997939 policyengine-api-1.0.1/tests/api/
--rw-r--r--   0 nikhil     (501) staff       (20)     2332 2023-03-22 20:58:23.000000 policyengine-api-1.0.1/tests/api/test_api.py
--rw-r--r--   0 nikhil     (501) staff       (20)       54 2022-12-08 00:06:30.000000 policyengine-api-1.0.1/tests/api/test_hello_world.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)       65 2023-03-23 00:33:05.000000 policyengine-api-1.0.1/tests/api/test_liveness.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)       67 2023-03-23 00:33:13.000000 policyengine-api-1.0.1/tests/api/test_readiness.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)      154 2023-03-22 18:03:54.000000 policyengine-api-1.0.1/tests/api/test_uk_baseline_policy.yaml
--rw-r--r--   0 nikhil     (501) staff       (20)       65 2022-12-08 00:06:30.000000 policyengine-api-1.0.1/tests/api/test_uk_metadata.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.931115 policyengine-api-1.1.0/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.916804 policyengine-api-1.1.0/.github/
+-rw-r--r--   0 nikhil     (501) staff       (20)      267 2022-12-19 15:37:36.000000 policyengine-api-1.1.0/.github/changelog_template.md
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      122 2022-12-19 15:37:36.000000 policyengine-api-1.1.0/.github/get-changelog-diff.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      642 2022-12-19 15:37:36.000000 policyengine-api-1.1.0/.github/has-functional-changes.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)     1013 2022-12-19 15:37:36.000000 policyengine-api-1.1.0/.github/is-version-number-acceptable.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      115 2022-12-19 15:37:36.000000 policyengine-api-1.1.0/.github/publish-git-tag.sh
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.917250 policyengine-api-1.1.0/.github/workflows/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1724 2023-04-07 13:27:50.000000 policyengine-api-1.1.0/.github/workflows/pr.yml
+-rw-r--r--   0 nikhil     (501) staff       (20)     2390 2023-04-07 13:27:56.000000 policyengine-api-1.1.0/.github/workflows/push.yml
+-rw-r--r--   0 nikhil     (501) staff       (20)      162 2023-04-10 14:08:43.000000 policyengine-api-1.1.0/.gitignore
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.917530 policyengine-api-1.1.0/.vscode/
+-rw-r--r--   0 nikhil     (501) staff       (20)      692 2022-11-22 22:32:04.000000 policyengine-api-1.1.0/.vscode/launch.json
+-rw-r--r--   0 nikhil     (501) staff       (20)    30343 2023-04-07 19:07:02.000000 policyengine-api-1.1.0/CHANGELOG.md
+-rw-r--r--   0 nikhil     (501) staff       (20)    34523 2022-12-06 22:08:46.000000 policyengine-api-1.1.0/LICENSE
+-rw-r--r--   0 nikhil     (501) staff       (20)      826 2023-04-07 11:35:57.000000 policyengine-api-1.1.0/Makefile
+-rw-r--r--   0 nikhil     (501) staff       (20)      211 2023-04-11 13:00:59.930872 policyengine-api-1.1.0/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      391 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)    19345 2023-04-07 19:07:02.000000 policyengine-api-1.1.0/changelog.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)       89 2023-04-11 00:07:10.000000 policyengine-api-1.1.0/changelog_entry.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.917691 policyengine-api-1.1.0/dashboard/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1990 2023-01-11 13:17:41.000000 policyengine-api-1.1.0/dashboard/app.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.918398 policyengine-api-1.1.0/dashboard/experiments/
+-rw-r--r--   0 nikhil     (501) staff       (20)     4252 2023-04-03 21:42:12.000000 policyengine-api-1.1.0/dashboard/experiments/gpt4_api_user.py
+-rw-r--r--   0 nikhil     (501) staff       (20)       41 2023-04-03 21:42:12.000000 policyengine-api-1.1.0/dashboard/experiments/requirements.txt
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.919624 policyengine-api-1.1.0/gcp/
+-rw-r--r--   0 nikhil     (501) staff       (20)      658 2023-04-11 12:44:05.000000 policyengine-api-1.1.0/gcp/Dockerfile
+-rw-r--r--   0 nikhil     (501) staff       (20)      697 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/gcp/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)     2906 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/gcp/bump_country_package.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      133 2022-12-08 00:06:30.000000 policyengine-api-1.1.0/gcp/dispatch.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)     1129 2023-04-07 11:37:10.000000 policyengine-api-1.1.0/gcp/export.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.920470 policyengine-api-1.1.0/gcp/policyengine_api/
+-rw-r--r--   0 nikhil     (501) staff       (20)      295 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/gcp/policyengine_api/Dockerfile
+-rw-r--r--   0 nikhil     (501) staff       (20)      327 2023-04-07 13:28:29.000000 policyengine-api-1.1.0/gcp/policyengine_api/app.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      180 2023-04-07 16:38:53.000000 policyengine-api-1.1.0/gcp/policyengine_api/start.sh
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.921359 policyengine-api-1.1.0/policyengine_api/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1863 2023-04-10 14:16:02.000000 policyengine-api-1.1.0/policyengine_api/api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      611 2023-04-11 13:00:49.000000 policyengine-api-1.1.0/policyengine_api/constants.py
+-rw-r--r--   0 nikhil     (501) staff       (20)    17718 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/country.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.923398 policyengine-api-1.1.0/policyengine_api/data/
+-rw-r--r--   0 nikhil     (501) staff       (20)     2003 2023-04-04 11:36:53.000000 policyengine-api-1.1.0/policyengine_api/data/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)       65 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/data/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     4488 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/data/data.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1922 2023-04-04 11:36:53.000000 policyengine-api-1.1.0/policyengine_api/data/initialise.sql
+-rw-r--r--   0 nikhil     (501) staff       (20)     2043 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/data/initialise_local.sql
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.925257 policyengine-api-1.1.0/policyengine_api/endpoints/
+-rw-r--r--   0 nikhil     (501) staff       (20)      348 2023-04-10 14:14:41.000000 policyengine-api-1.1.0/policyengine_api/endpoints/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     3229 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/analysis.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.926435 policyengine-api-1.1.0/policyengine_api/endpoints/economy/
+-rw-r--r--   0 nikhil     (501) staff       (20)       41 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/economy/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)    13764 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/economy/compare.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     6275 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/economy/economy.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     8300 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/economy/reform_impact.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     5846 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/economy/single_economy.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      258 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/home.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     7379 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/household.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      359 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/metadata.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     3769 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/endpoints/policy.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.928021 policyengine-api-1.1.0/policyengine_api/endpoints/search/
+-rw-r--r--   0 nikhil     (501) staff       (20)       93 2023-04-09 09:09:50.000000 policyengine-api-1.1.0/policyengine_api/endpoints/search/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)       31 2023-04-10 14:27:59.000000 policyengine-api-1.1.0/policyengine_api/endpoints/search/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     2901 2023-04-10 14:27:59.000000 policyengine-api-1.1.0/policyengine_api/endpoints/search/create_embeddings.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     2888 2023-04-11 12:43:00.000000 policyengine-api-1.1.0/policyengine_api/endpoints/search/search.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.928410 policyengine-api-1.1.0/policyengine_api/utils/
+-rw-r--r--   0 nikhil     (501) staff       (20)       20 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/utils/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      979 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/utils/json.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      282 2023-04-07 11:35:54.000000 policyengine-api-1.1.0/policyengine_api/worker.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.922341 policyengine-api-1.1.0/policyengine_api.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)      211 2023-04-11 13:00:59.000000 policyengine-api-1.1.0/policyengine_api.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)     2000 2023-04-11 13:00:59.000000 policyengine-api-1.1.0/policyengine_api.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2023-04-11 13:00:59.000000 policyengine-api-1.1.0/policyengine_api.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      312 2023-04-11 13:00:59.000000 policyengine-api-1.1.0/policyengine_api.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2023-04-11 13:00:59.000000 policyengine-api-1.1.0/policyengine_api.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2023-04-11 13:00:59.931175 policyengine-api-1.1.0/setup.cfg
+-rw-r--r--   0 nikhil     (501) staff       (20)      857 2023-04-11 12:42:11.000000 policyengine-api-1.1.0/setup.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.912732 policyengine-api-1.1.0/tests/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-11 13:00:59.930484 policyengine-api-1.1.0/tests/api/
+-rw-r--r--   0 nikhil     (501) staff       (20)     2332 2023-03-22 20:58:23.000000 policyengine-api-1.1.0/tests/api/test_api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)       54 2022-12-08 00:06:30.000000 policyengine-api-1.1.0/tests/api/test_hello_world.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)       65 2023-03-23 00:33:05.000000 policyengine-api-1.1.0/tests/api/test_liveness.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)       67 2023-03-23 00:33:13.000000 policyengine-api-1.1.0/tests/api/test_readiness.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      154 2023-03-22 18:03:54.000000 policyengine-api-1.1.0/tests/api/test_uk_baseline_policy.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)       65 2022-12-08 00:06:30.000000 policyengine-api-1.1.0/tests/api/test_uk_metadata.yaml
```

### Comparing `policyengine-api-1.0.1/.github/has-functional-changes.sh` & `policyengine-api-1.1.0/.github/has-functional-changes.sh`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/.github/is-version-number-acceptable.sh` & `policyengine-api-1.1.0/.github/is-version-number-acceptable.sh`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/.github/workflows/pr.yml` & `policyengine-api-1.1.0/.github/workflows/pr.yml`

 * *Files 0% similar despite different names*

```diff
@@ -43,13 +43,13 @@
         uses: google-github-actions/setup-gcloud@v0
         with:
           project_id: policyengine-api
           service_account_key: ${{ secrets.GCP_SA_KEY }}
           export_default_credentials: true
       - name: Install dependencies
         run: make install
-      - name: Test the main API
+      - name: Test the API
         run: make test
         env:
           POLICYENGINE_DB_PASSWORD: ${{ secrets.POLICYENGINE_DB_PASSWORD }}
           POLICYENGINE_GITHUB_MICRODATA_AUTH_TOKEN: ${{ secrets.POLICYENGINE_GITHUB_MICRODATA_AUTH_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
```

### Comparing `policyengine-api-1.0.1/.github/workflows/push.yml` & `policyengine-api-1.1.0/.github/workflows/push.yml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         uses: EndBug/add-and-commit@v8
         with:
           add: "."
           committer_name: Github Actions[bot]
           author_name: Github Actions[bot]
           message: Update PolicyEngine API
   deploy:
-    name: Deploy main API
+    name: Deploy API
     runs-on: ubuntu-latest
     if: |
       (github.repository == 'PolicyEngine/policyengine-api')
       && (github.event.head_commit.message == 'Update PolicyEngine API')
     steps:
       - name: Checkout repo
         uses: actions/checkout@v2
```

### Comparing `policyengine-api-1.0.1/.vscode/launch.json` & `policyengine-api-1.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/CHANGELOG.md` & `policyengine-api-1.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.2] - 2023-04-07 17:24:42
+
+### Changed
+
+- Update PolicyEngine us to 0.279.0
+
 ## [1.0.1] - 2023-04-07 13:06:13
 
 ### Added
 
 - Added missing `redis` Python dependency.
 
 ## [1.0.0] - 2023-04-07 11:34:18
@@ -1075,14 +1081,15 @@
 
 ### Added
 
 - Initial API.
 
 
 
+[1.0.2]: https://github.com/PolicyEngine/policyengine-api/compare/1.0.1...1.0.2
 [1.0.1]: https://github.com/PolicyEngine/policyengine-api/compare/1.0.0...1.0.1
 [1.0.0]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.25...1.0.0
 [0.13.25]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.24...0.13.25
 [0.13.24]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.23...0.13.24
 [0.13.23]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.22...0.13.23
 [0.13.22]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.21...0.13.22
 [0.13.21]: https://github.com/PolicyEngine/policyengine-api/compare/0.13.20...0.13.21
```

### Comparing `policyengine-api-1.0.1/LICENSE` & `policyengine-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/Makefile` & `policyengine-api-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/changelog.yaml` & `policyengine-api-1.1.0/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -892,7 +892,12 @@
     - Combine main and compute servers into a single server.
   date: 2023-04-07 11:34:18
 - bump: patch
   changes:
     added:
     - Added missing `redis` Python dependency.
   date: 2023-04-07 13:06:13
+- bump: patch
+  changes:
+    changed:
+    - Update PolicyEngine us to 0.279.0
+  date: 2023-04-07 17:24:42
```

### Comparing `policyengine-api-1.0.1/dashboard/app.py` & `policyengine-api-1.1.0/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/dashboard/experiments/gpt4_api_user.py` & `policyengine-api-1.1.0/dashboard/experiments/gpt4_api_user.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/gcp/README.md` & `policyengine-api-1.1.0/gcp/README.md`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/gcp/bump_country_package.py` & `policyengine-api-1.1.0/gcp/bump_country_package.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/gcp/export.py` & `policyengine-api-1.1.0/gcp/export.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/api.py` & `policyengine-api-1.1.0/policyengine_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     get_policy,
     set_policy,
     get_policy_search,
     get_household_under_policy,
     get_calculate,
     get_economic_impact,
     get_analysis,
+    get_search,
 )
 
 app = application = flask.Flask(__name__)
 
 CORS(app)
 
 app.route("/", methods=["GET"])(get_home)
@@ -57,14 +58,16 @@
 
 app.route("/<country_id>/analysis", methods=["POST"])(
     app.route("/<country_id>/analysis/<prompt_id>", methods=["GET"])(
         get_analysis
     )
 )
 
+app.route("/<country_id>/search", methods=["GET"])(get_search)
+
 
 @app.route("/liveness_check", methods=["GET"])
 def liveness_check():
     return flask.Response(
         "OK", status=200, headers={"Content-Type": "text/plain"}
     )
```

### Comparing `policyengine-api-1.0.1/policyengine_api/constants.py` & `policyengine-api-1.1.0/policyengine_api/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pkg_resources
 
 REPO = Path(__file__).parents[1]
 GET = "GET"
 POST = "POST"
 UPDATE = "UPDATE"
 LIST = "LIST"
-VERSION = "1.0.1"
+VERSION = "1.1.0"
 COUNTRIES = ("uk", "us", "ca", "ng")
 COUNTRY_PACKAGE_NAMES = (
     "policyengine_uk",
     "policyengine_us",
     "policyengine_canada",
     "policyengine_ng",
 )
```

### Comparing `policyengine-api-1.0.1/policyengine_api/country.py` & `policyengine-api-1.1.0/policyengine_api/country.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/data/README.md` & `policyengine-api-1.1.0/policyengine_api/data/README.md`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/data/data.py` & `policyengine-api-1.1.0/policyengine_api/data/data.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/data/initialise.sql` & `policyengine-api-1.1.0/policyengine_api/data/initialise.sql`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/data/initialise_local.sql` & `policyengine-api-1.1.0/policyengine_api/data/initialise_local.sql`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/analysis.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/analysis.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/economy/compare.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/economy/compare.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/economy/economy.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/economy/economy.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/economy/reform_impact.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/economy/reform_impact.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/economy/single_economy.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/economy/single_economy.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/household.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/household.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/endpoints/policy.py` & `policyengine-api-1.1.0/policyengine_api/endpoints/policy.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api/utils/json.py` & `policyengine-api-1.1.0/policyengine_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `policyengine-api-1.0.1/policyengine_api.egg-info/SOURCES.txt` & `policyengine-api-1.1.0/policyengine_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 policyengine_api/endpoints/metadata.py
 policyengine_api/endpoints/policy.py
 policyengine_api/endpoints/economy/__init__.py
 policyengine_api/endpoints/economy/compare.py
 policyengine_api/endpoints/economy/economy.py
 policyengine_api/endpoints/economy/reform_impact.py
 policyengine_api/endpoints/economy/single_economy.py
+policyengine_api/endpoints/search/README.md
+policyengine_api/endpoints/search/__init__.py
+policyengine_api/endpoints/search/create_embeddings.py
+policyengine_api/endpoints/search/search.py
 policyengine_api/utils/__init__.py
 policyengine_api/utils/json.py
 tests/api/test_api.py
 tests/api/test_hello_world.yaml
 tests/api/test_liveness.yaml
 tests/api/test_readiness.yaml
 tests/api/test_uk_baseline_policy.yaml
```

### Comparing `policyengine-api-1.0.1/setup.py` & `policyengine-api-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,24 @@
     packages=find_packages(),
     install_requires=[
         "click>=8",
         "flask>=1",
         "flask-cors>=3",
         "PolicyEngine-Core>=2,<3",
         "policyengine_uk==0.45.0",
-        "policyengine_us==0.278.0",
+        "policyengine_us==0.279.0",
         "policyengine_canada==0.45.0",
         "policyengine-ng==0.4.2",
         "gunicorn",
         "cloud-sql-python-connector",
         "google-cloud-logging",
         "pymysql",
         "sqlalchemy>=1.4,<2",
         "streamlit",
         "markupsafe==2.0.1",
         "openai",
         "rq",
         "redis",
+        "sentence-transformers",
+        "faiss",
     ],
 )
```

### Comparing `policyengine-api-1.0.1/tests/api/test_api.py` & `policyengine-api-1.1.0/tests/api/test_api.py`

 * *Files identical despite different names*

