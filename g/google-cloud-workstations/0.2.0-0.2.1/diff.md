# Comparing `tmp/google-cloud-workstations-0.2.0.tar.gz` & `tmp/google-cloud-workstations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-workstations-0.2.0.tar", last modified: Thu Apr  6 13:28:19 2023, max compression
+gzip compressed data, was "google-cloud-workstations-0.2.1.tar", last modified: Tue Apr 11 16:32:42 2023, max compression
```

## Comparing `google-cloud-workstations-0.2.0.tar` & `google-cloud-workstations-0.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.547753 google-cloud-workstations-0.2.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4600 2023-04-06 13:28:19.547753 google-cloud-workstations-0.2.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3682 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.531751 google-cloud-workstations-0.2.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.531751 google-cloud-workstations-0.2.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.535751 google-cloud-workstations-0.2.0/google/cloud/workstations/
--rw-rw-r--   0 root         (0)     1003     3048 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.535751 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/
--rw-rw-r--   0 root         (0)     1003     2904 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.535751 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.535751 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129387 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   140606 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27340 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.535751 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20457 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42986 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43817 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142624 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.539752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54336 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.539752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003     2908 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     8916 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.539752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.539752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129831 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   141050 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27504 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.539752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20465 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43078 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43909 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142768 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54082 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/
--rw-r--r--   0 root         (0)     1003     4600 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2717 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-06 13:28:19.000000 google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-06 13:28:19.547753 google-cloud-workstations-0.2.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   567497 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1/test_workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-06 13:28:19.543752 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   567385 2023-04-06 13:25:25.000000 google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1beta/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4600 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3682 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/workstations/
+-rw-rw-r--   0 root         (0)     1003     3048 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003     2904 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129387 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140606 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27340 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20457 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    42986 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43817 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142624 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54336 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003     2908 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8916 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129831 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   141050 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27504 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20465 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43078 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43909 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142768 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54080 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/
+-rw-r--r--   0 root         (0)     1003     4600 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2717 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   567497 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   567385 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/test_workstations.py
```

### Comparing `google-cloud-workstations-0.2.0/LICENSE` & `google-cloud-workstations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/MANIFEST.in` & `google-cloud-workstations-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/PKG-INFO` & `google-cloud-workstations-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.2.0/README.rst` & `google-cloud-workstations-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations/gapic_version.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/gapic_metadata.json` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/gapic_version.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/async_client.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/client.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/pagers.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/base.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/services/workstations/transports/rest.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/types/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1/types/workstations.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/gapic_metadata.json` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/gapic_version.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.0"  # {x-release-please-version}
+__version__ = "0.2.1"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/async_client.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/client.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/pagers.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/types/__init__.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/google/cloud/workstations_v1beta/types/workstations.py` & `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/workstations.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,21 +337,21 @@
         class GceInstance(proto.Message):
             r"""A runtime using a Compute Engine instance.
 
             Attributes:
                 machine_type (str):
                     The name of a Compute Engine machine type.
                 service_account (str):
-                    Email address of the service account that
-                    will be used on VM instances used to support
-                    this config. This service account must have
+                    Email address of the service account used on
+                    VM instances used to support this configuration.
+                    If not set, VMs run with a Google-managed
+                    service account. This service account must have
                     permission to pull the specified container
-                    image. If not set, VMs will run without a
-                    service account, in which case the image must be
-                    publicly accessible.
+                    image; otherwise, the image must be publicly
+                    accessible.
                 tags (MutableSequence[str]):
                     Network tags to add to the Compute Engine
                     machines backing the Workstations.
                 pool_size (int):
                     Number of instances to pool for faster
                     workstation starup.
                 disable_public_ip_addresses (bool):
```

### Comparing `google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/PKG-INFO` & `google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.2.0
+Version: 0.2.1
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.2.0/google_cloud_workstations.egg-info/SOURCES.txt` & `google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/setup.py` & `google-cloud-workstations-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/__init__.py` & `google-cloud-workstations-0.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/__init__.py` & `google-cloud-workstations-0.2.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/gapic/__init__.py` & `google-cloud-workstations-0.2.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1/__init__.py` & `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1/test_workstations.py` & `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/test_workstations.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.0/tests/unit/gapic/workstations_v1beta/test_workstations.py` & `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/test_workstations.py`

 * *Files identical despite different names*

