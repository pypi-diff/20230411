# Comparing `tmp/kubernetes-dynamic-0.1.1.tar.gz` & `tmp/kubernetes-dynamic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes-dynamic-0.1.1.tar", last modified: Thu Apr  6 17:38:40 2023, max compression
+gzip compressed data, was "kubernetes-dynamic-0.1.2.tar", last modified: Tue Apr 11 15:50:54 2023, max compression
```

## Comparing `kubernetes-dynamic-0.1.1.tar` & `kubernetes-dynamic-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,53 @@
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.472063 kubernetes-dynamic-0.1.1/
--rw-r--r--   0 akobor    (1000) akobor    (1000)      538 2023-03-28 15:57:58.000000 kubernetes-dynamic-0.1.1/LICENSE
--rw-r--r--   0 akobor    (1000) akobor    (1000)     3312 2023-04-06 17:38:40.472063 kubernetes-dynamic-0.1.1/PKG-INFO
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2434 2023-04-04 08:18:12.000000 kubernetes-dynamic-0.1.1/README.md
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.462063 kubernetes-dynamic-0.1.1/kubernetes_dynamic/
--rw-r--r--   0 akobor    (1000) akobor    (1000)      713 2023-04-06 10:41:23.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/__init__.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      821 2023-04-06 09:49:15.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/_kubernetes.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)       22 2023-04-06 17:38:25.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/_version.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    14313 2023-04-06 12:50:21.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/client.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1636 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/config.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     3373 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/events.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1279 2023-04-06 09:06:15.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/exceptions.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2195 2023-04-06 12:50:11.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/formatters.py
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.462063 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/
--rw-r--r--   0 akobor    (1000) akobor    (1000)        0 2023-04-06 08:52:24.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/__init__.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2620 2023-04-06 08:55:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/dateutil.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    17528 2023-04-06 10:34:53.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/discovery.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     3895 2023-04-06 09:13:20.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/exceptions.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     3618 2023-04-06 08:58:17.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/exec_provider.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     4499 2023-04-06 08:58:21.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/incluster_config.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    32113 2023-04-06 09:30:16.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/kube_config.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    20042 2023-04-06 15:56:41.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/resource_api.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    22528 2023-04-06 09:12:10.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/ws_client.py
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.462063 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/
--rw-r--r--   0 akobor    (1000) akobor    (1000)    28915 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/__init__.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)   140097 2023-04-06 12:52:17.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/all.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2483 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/common.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1855 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/configmap.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      830 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/ingress.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1092 2023-04-06 10:50:43.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/namespace.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     4659 2023-04-06 13:00:47.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/pod.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      843 2023-04-06 12:52:00.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/replica_set.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     8305 2023-04-06 10:50:03.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/resource_item.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2857 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/resource_value.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2944 2023-04-06 10:50:56.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/secret.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1333 2023-04-06 15:52:26.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/service.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      761 2023-04-06 12:35:43.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/stateful_set.py
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.472063 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/
--rw-r--r--   0 akobor    (1000) akobor    (1000)        0 2023-04-06 08:45:10.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/__init__.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    27737 2023-04-06 10:42:24.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/api_client.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    15174 2023-04-06 09:13:43.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/configuration.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     5104 2023-04-06 08:50:35.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/exceptions.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)    12499 2023-04-06 09:14:24.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/rest.py
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.462063 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/
--rw-r--r--   0 akobor    (1000) akobor    (1000)     3312 2023-04-06 17:38:40.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/PKG-INFO
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1823 2023-04-06 17:38:40.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/SOURCES.txt
--rw-r--r--   0 akobor    (1000) akobor    (1000)        1 2023-04-06 17:38:40.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/dependency_links.txt
--rw-r--r--   0 akobor    (1000) akobor    (1000)      117 2023-04-06 17:38:40.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/requires.txt
--rw-r--r--   0 akobor    (1000) akobor    (1000)       19 2023-04-06 17:38:40.000000 kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/top_level.txt
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1415 2023-04-03 12:59:55.000000 kubernetes-dynamic-0.1.1/pyproject.toml
--rw-r--r--   0 akobor    (1000) akobor    (1000)      117 2023-04-06 10:42:13.000000 kubernetes-dynamic-0.1.1/requirements.txt
--rw-r--r--   0 akobor    (1000) akobor    (1000)       38 2023-04-06 17:38:40.472063 kubernetes-dynamic-0.1.1/setup.cfg
-drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-06 17:38:40.472063 kubernetes-dynamic-0.1.1/tests/
--rw-r--r--   0 akobor    (1000) akobor    (1000)     7240 2023-04-06 11:16:08.000000 kubernetes-dynamic-0.1.1/tests/test_client.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      921 2023-03-30 08:05:36.000000 kubernetes-dynamic-0.1.1/tests/test_config.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2010 2023-04-03 11:54:29.000000 kubernetes-dynamic-0.1.1/tests/test_configmap.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      623 2023-04-03 11:54:58.000000 kubernetes-dynamic-0.1.1/tests/test_ingress.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     1636 2023-04-06 10:51:07.000000 kubernetes-dynamic-0.1.1/tests/test_namespace.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     5097 2023-04-06 11:09:52.000000 kubernetes-dynamic-0.1.1/tests/test_pod.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     4222 2023-04-06 11:30:59.000000 kubernetes-dynamic-0.1.1/tests/test_resource_api.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     4804 2023-04-06 10:50:03.000000 kubernetes-dynamic-0.1.1/tests/test_resource_item.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)      761 2023-04-03 20:50:33.000000 kubernetes-dynamic-0.1.1/tests/test_resource_value.py
--rw-r--r--   0 akobor    (1000) akobor    (1000)     2770 2023-04-03 12:49:49.000000 kubernetes-dynamic-0.1.1/tests/test_secret.py
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      538 2023-03-28 15:57:58.000000 kubernetes-dynamic-0.1.2/LICENSE
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     3312 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/PKG-INFO
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2434 2023-04-04 08:18:12.000000 kubernetes-dynamic-0.1.2/README.md
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/kubernetes_dynamic/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      713 2023-04-06 10:41:23.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/__init__.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      821 2023-04-06 09:49:15.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/_kubernetes.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)       22 2023-04-11 15:50:43.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/_version.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    14510 2023-04-06 19:11:24.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/client.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1637 2023-04-11 14:34:32.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/config.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     3466 2023-04-11 15:45:05.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/events.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1279 2023-04-06 09:06:15.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/exceptions.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2195 2023-04-06 12:50:11.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/formatters.py
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)        0 2023-04-06 08:52:24.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/__init__.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    17599 2023-04-11 13:40:09.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/discovery.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     3907 2023-04-11 13:36:44.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/exceptions.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     3618 2023-04-06 08:58:17.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/exec_provider.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     4499 2023-04-06 08:58:21.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/incluster_config.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    31901 2023-04-11 13:40:58.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/kube_config.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    20445 2023-04-11 15:45:14.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/resource_api.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     6339 2023-04-06 18:32:16.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/ws_client.py
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    28915 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/__init__.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)   140097 2023-04-06 12:52:17.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/all.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2483 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/common.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1855 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/configmap.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      830 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/ingress.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1092 2023-04-06 10:50:43.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/namespace.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     4659 2023-04-06 13:00:47.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/pod.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      843 2023-04-06 12:52:00.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/replica_set.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     9542 2023-04-11 15:20:39.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/resource_item.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2857 2023-04-05 15:49:31.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/resource_value.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2737 2023-04-06 18:53:11.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/secret.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1333 2023-04-06 15:52:26.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/service.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      761 2023-04-06 12:35:43.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/stateful_set.py
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)        0 2023-04-06 08:45:10.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/__init__.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    19359 2023-04-11 13:12:19.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/api_client.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    15174 2023-04-11 13:22:32.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/configuration.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     2811 2023-04-06 19:20:16.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/exceptions.py
+-rw-r--r--   0 akobor    (1000) akobor    (1000)    11263 2023-04-11 12:29:45.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/rest.py
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     3312 2023-04-11 15:50:54.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/PKG-INFO
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1574 2023-04-11 15:50:54.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 akobor    (1000) akobor    (1000)        1 2023-04-11 15:50:54.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      117 2023-04-11 15:50:54.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/requires.txt
+-rw-r--r--   0 akobor    (1000) akobor    (1000)       19 2023-04-11 15:50:54.000000 kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/top_level.txt
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1415 2023-04-03 12:59:55.000000 kubernetes-dynamic-0.1.2/pyproject.toml
+-rw-r--r--   0 akobor    (1000) akobor    (1000)      117 2023-04-06 10:42:13.000000 kubernetes-dynamic-0.1.2/requirements.txt
+-rw-r--r--   0 akobor    (1000) akobor    (1000)       38 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/setup.cfg
+drwxr-xr-x   0 akobor    (1000) akobor    (1000)        0 2023-04-11 15:50:54.551307 kubernetes-dynamic-0.1.2/tests/
+-rw-r--r--   0 akobor    (1000) akobor    (1000)     1154 2023-04-11 15:47:38.000000 kubernetes-dynamic-0.1.2/tests/test_sandbox.py
```

### Comparing `kubernetes-dynamic-0.1.1/LICENSE` & `kubernetes-dynamic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/PKG-INFO` & `kubernetes-dynamic-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernetes-dynamic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kubernetes Dynamic client
 Author-email: Attila Kobor <atti92@gmail.com>, Balazs Hamorszky <balihb@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/atti92/kubernetes-dynamic
 Project-URL: documentation, https://github.com/atti92/kubernetes-dynamic
 Project-URL: repository, https://github.com/atti92/kubernetes-dynamic.git
 Project-URL: changelog, https://github.com/atti92/kubernetes-dynamic/blob/main/README.md
```

### Comparing `kubernetes-dynamic-0.1.1/README.md` & `kubernetes-dynamic-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/__init__.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/_kubernetes.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/_kubernetes.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/client.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import pydantic
 import yaml
 
 import kubernetes_dynamic.kube.ws_client as ws_client
 import kubernetes_dynamic.models as models
 from kubernetes_dynamic.formatters import to_lower_camel
+from kubernetes_dynamic.kube.exceptions import api_exception
+from kubernetes_dynamic.openapi_client.exceptions import ApiException
 
 from . import _kubernetes
 from .config import K8sConfig
 from .exceptions import (
     ConfigException,
     InvalidParameter,
     ResourceNotUniqueError,
@@ -238,15 +240,15 @@
         **filter_dict,
     ) -> ResourceApi[T]:
         ...
 
     def get_api(
         self,
         name: Optional[str] = None,
-        object_type: Optional[Type[T]] = ResourceItem,
+        object_type: Optional[Type[T]] = None,
         api_version: Optional[str] = None,
         kind: Optional[str] = None,
         **filter_dict,
     ) -> ResourceApi[T]:
         if api_version:
             filter_dict["api_version"] = api_version
         if kind:
@@ -294,16 +296,16 @@
                 serialize=False,
             )
         finally:
             self.client.request = prev_request
 
     def stream(self, func: Callable, name=None, namespace=MISSING, *args, **kwargs) -> str:
         client = self.websocket(func, name, namespace, *args, **kwargs)
-        client.run_forever(timeout=kwargs.get("_request_timeout", 0))  # type: ignore
-        return ws_client.WSResponse("%s" % "".join(client.read_all())).data
+        client.run_forever()  # type: ignore
+        return "".join(client.read_all())
 
     @meta_request
     def request(self, method: str, path: str, body=None, **params) -> Any:
         if not path.startswith("/"):
             path = "/" + path
 
         path_params = params.pop("path_params", {})
@@ -327,29 +329,32 @@
         # Authentication setting
         auth_settings = ["BearerToken"]
 
         for key, value in params.items():
             if value is not None:
                 query_params.append((to_lower_camel(key.lstrip("_")), value))
 
-        api_response = self.client.call_api(
-            path,
-            method.upper(),
-            path_params,
-            query_params,
-            header_params,
-            body=body,
-            post_params=form_params,
-            async_req=async_req,
-            files=local_var_files,
-            auth_settings=auth_settings,
-            _preload_content=False,
-            _return_http_data_only=_return_http_data_only,
-            _request_timeout=_request_timeout,
-        )
+        try:
+            api_response = self.client.call_api(
+                path,
+                method.upper(),
+                path_params,
+                query_params,
+                header_params,
+                body=body,
+                post_params=form_params,
+                async_req=async_req,
+                files=local_var_files,
+                auth_settings=auth_settings,
+                _preload_content=False,
+                _return_http_data_only=_return_http_data_only,
+                _request_timeout=_request_timeout,
+            )
+        except ApiException as e:
+            raise api_exception(e) from e
         return api_response.get() if async_req else api_response  # type: ignore
 
     def apply(
         self,
         *,
         namespace: Optional[str | _Missing] = MISSING,
         file_path: Optional[str | Path] = None,
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/config.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Dict, Optional
 
-from . import _kubernetes
 import pydantic
 
+from . import _kubernetes
+
 
 class MutedSecretsSettingsSource:
     """Disable warning when secrets dir does not exist."""
 
     def __init__(self, source: pydantic.env_settings.SecretsSettingsSource):
         self.source = source
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/events.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,41 +67,43 @@
         timeout_seconds=None,
         **kwargs,
     ):
         self._stop = False
         self.resource_version = resource_version or self.resource_version
         self.timeout_seconds = timeout_seconds
         retry_after_410 = False
+        kwargs.pop("serialize", None)
         while not self._stop:
             resp: HTTPResponse = func(
                 *args,
                 resource_version=self.resource_version,
                 watch=watch,
                 _preload_content=_preload_content,
                 timeout_seconds=timeout_seconds or 5,
+                serialize=False,
                 **kwargs,
             )
             try:
                 yield from self._parse_response_iter(resp)
             except ApiException as e:
                 if e.status == 410 and not retry_after_410:
-                    self.resource_version = func(*args, **kwargs).metadata.resourceVersion
+                    self.resource_version = func(*args, serialize=True, **kwargs).metadata.resourceVersion
                     retry_after_410 = True
                     continue
                 raise api_exception(e) from e
             finally:
                 resp.close()
                 resp.release_conn()
                 if timeout_seconds or self.resource_version is None:
                     self._stop = True
 
     def _parse_response_iter(self, resp: HTTPResponse):
         for line in resp:
             event = pydantic.parse_raw_as(Event, line)
-            if event.type == EventType.ERROR:
+            if event.type == EventType.ERROR.value:
                 raise ApiException(event.object.code)
 
             event.object = self._return_type(event.object)
             self.resource_version = event.raw_object.get("metadata", {}).get("resourceVersion")
             yield event
 
             if self._stop:
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/exceptions.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/exceptions.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/formatters.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/formatters.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/discovery.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import json
 import logging
 import os
 import tempfile
 from abc import abstractmethod, abstractproperty
 from collections import defaultdict
 from functools import partial
+from typing import Any
 
 from urllib3.exceptions import MaxRetryError, ProtocolError
 
 from kubernetes_dynamic import __version__
 
 from .exceptions import NotFoundError, ResourceNotFoundError, ResourceNotUniqueError, ServiceUnavailableError
 from .resource_api import ResourceApi, ResourceList
@@ -41,30 +42,30 @@
 
     def __init__(self, client, cache_file):
         self.client = client
         default_cache_id = self.client.configuration.host
         default_cache_id = default_cache_id.encode("utf-8")
         try:
             default_cachefile_name = "osrcp-{0}.json".format(
-                hashlib.md5(default_cache_id, usedforsecurity=False).hexdigest()
+                hashlib.md5(default_cache_id, usedforsecurity=False).hexdigest()  # type: ignore
             )
         except TypeError:
             # usedforsecurity is only supported in 3.9+
             default_cachefile_name = "osrcp-{0}.json".format(hashlib.md5(default_cache_id).hexdigest())
         self.__cache_file = cache_file or os.path.join(tempfile.gettempdir(), default_cachefile_name)
         self.__init_cache()
 
     def __init_cache(self, refresh=False):
         if refresh or not os.path.exists(self.__cache_file):
             self._cache = {"library_version": __version__}
             refresh = True
         else:
             try:
                 with open(self.__cache_file, "r") as f:
-                    self._cache = json.load(f, cls=partial(CacheDecoder, self.client))
+                    self._cache: dict[str, Any] = json.load(f, cls=partial(CacheDecoder, self.client))  # type: ignore
                 if self._cache.get("library_version") != __version__:
                     # Version mismatch, need to refresh cache
                     self.invalidate_cache()
             except Exception as e:
                 logging.error("load cache error: %s", e)
                 self.invalidate_cache()
         self._load_server_info()
@@ -190,15 +191,15 @@
             resourceobj = ResourceApi(
                 prefix=prefix,
                 group=group,
                 api_version=version,
                 client=self.client,
                 preferred=preferred,
                 subresources=subresources.get(resource["name"]),
-                **resource
+                **resource,
             )
             resources[resource["kind"]].append(resourceobj)
 
             resource_list = ResourceList(self.client, group=group, api_version=version, base_kind=resource["kind"])
             resources[resource_list.kind].append(resource_list)
         return resources
 
@@ -256,15 +257,14 @@
             results = self.__search(self.__build_search(**kwargs), self.__resources, [])
         self.__maybe_write_cache()
         return results
 
     def __search(self, parts, resources, reqParams):
         part = parts[0]
         if part != "*":
-
             resourcePart = resources.get(part)
             if not resourcePart:
                 return []
             elif isinstance(resourcePart, ResourceGroup):
                 if len(reqParams) != 2:
                     raise ValueError("prefix and group params should be present, have %s" % reqParams)
                 # Check if we've requested resources for this group
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/exceptions.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import json
 import sys
 import traceback
 
 from kubernetes_dynamic.openapi_client.exceptions import ApiException
 
 
 class ConfigException(Exception):
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/exec_provider.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/exec_provider.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/incluster_config.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/incluster_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/kube_config.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/kube_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 import atexit
 import base64
 import copy
 import datetime
 import json
 import logging
 import os
-import platform
 import subprocess
 import tempfile
 import time
 from collections import namedtuple
 
 import google.auth
 import google.auth.transport.requests
 import oauthlib.oauth2
+import oauthlib.oauth2.rfc6749.errors
 import urllib3
 import yaml
+from dateutil.parser import parse
+from dateutil.tz import UTC
 from requests_oauthlib import OAuth2Session
 
 from ..openapi_client.api_client import ApiClient
 from ..openapi_client.configuration import Configuration
-from .dateutil import UTC, format_rfc3339, parse_rfc3339
 from .exceptions import ConfigException
 from .exec_provider import ExecProvider
 
 try:
-    import adal
+    import adal  # type: ignore
 except ImportError:
     pass
 
 EXPIRY_SKEW_PREVENTION_DELAY = datetime.timedelta(minutes=5)
 KUBE_CONFIG_DEFAULT_LOCATION = os.environ.get("KUBECONFIG", "~/.kube/config")
-ENV_KUBECONFIG_PATH_SEPARATOR = ";" if platform.system() == "Windows" else ":"
 _temp_files = {}
 
 
 def _cleanup_temp_files():
     global _temp_files
     for temp_file in _temp_files.values():
         try:
@@ -74,15 +74,15 @@
     _temp_files[content_key] = name
     with open(name, "wb") as fd:
         fd.write(content.encode() if isinstance(content, str) else content)
     return name
 
 
 def _is_expired(expiry):
-    return (parse_rfc3339(expiry) - EXPIRY_SKEW_PREVENTION_DELAY) <= datetime.datetime.utcnow().replace(tzinfo=UTC)
+    return (expiry - EXPIRY_SKEW_PREVENTION_DELAY) <= datetime.datetime.utcnow().replace(tzinfo=UTC)
 
 
 class FileOrData(object):
     """Utility class to read content of obj[%data_key_name] or file's
     content of obj[%file_key_name] and represent it as file or data.
     Note that the data is preferred. The obj[%file_key_name] will be used iff
     obj['%data_key_name'] is not set or empty. Assumption is file content is
@@ -165,28 +165,27 @@
                 msg += "\nStderr: %s" % stderr
             raise ConfigException(msg)
         try:
             data = json.loads(stdout)
         except ValueError as de:
             raise ConfigException("exec: failed to decode process output: %s" % de)
         A = namedtuple("A", ["token", "expiry"])
-        return A(token=data["credential"]["access_token"], expiry=parse_rfc3339(data["credential"]["token_expiry"]))
+        return A(token=data["credential"]["access_token"], expiry=parse(data["credential"]["token_expiry"]))
 
 
 class KubeConfigLoader(object):
     def __init__(
         self,
         config_dict,
         active_context=None,
         get_google_credentials=None,
         config_base_path="",
         config_persister=None,
         temp_file_path=None,
     ):
-
         if config_dict is None:
             raise ConfigException("Invalid kube-config. " "Expected config_dict to not be None.")
         elif isinstance(config_dict, ConfigNode):
             self._config = config_dict
         else:
             self._config = ConfigNode("kube-config", config_dict)
 
@@ -342,24 +341,24 @@
             or ("expiry" in provider["config"] and _is_expired(provider["config"]["expiry"]))
         ):
             # token is not available or expired, refresh it
             self._refresh_gcp_token()
 
         self.token = "Bearer %s" % provider["config"]["access-token"]
         if "expiry" in provider["config"]:
-            self.expiry = parse_rfc3339(provider["config"]["expiry"])
+            self.expiry = parse(provider["config"]["expiry"])
         return self.token
 
     def _refresh_gcp_token(self):
         if "config" not in self._user["auth-provider"]:
             self._user["auth-provider"].value["config"] = {}
         provider = self._user["auth-provider"]["config"]
         credentials = self._get_google_credentials()
         provider.value["access-token"] = credentials.token
-        provider.value["expiry"] = format_rfc3339(credentials.expiry)
+        provider.value["expiry"] = credentials.expiry.isoformat()
         if self._config_persister:
             self._config_persister()
 
     def _load_oid_token(self, provider):
         if "config" not in provider:
             return
 
@@ -377,18 +376,15 @@
         padding = (4 - len(parts[1]) % 4) * "="
         if len(padding) == 3:
             # According to spec, 3 padding characters cannot occur
             # in a valid jwt
             # https://tools.ietf.org/html/rfc7515#appendix-C
             return
 
-        if PY3:
-            jwt_attributes = json.loads(base64.urlsafe_b64decode(parts[1] + padding).decode("utf-8"))
-        else:
-            jwt_attributes = json.loads(base64.b64decode(parts[1] + padding))
+        jwt_attributes = json.loads(base64.urlsafe_b64decode(parts[1] + padding).decode("utf-8"))
 
         expire = jwt_attributes.get("exp")
 
         if (expire is not None) and (_is_expired(datetime.datetime.fromtimestamp(expire, tz=UTC))):
             self._refresh_oidc(provider)
 
             if self._config_persister:
@@ -484,15 +480,15 @@
                     base64_file_content=False,
                     temp_file_path=self._temp_file_path,
                 ).as_file()
             else:
                 logging.error("exec: missing token or clientCertificateData " "field in plugin output")
                 return None
             if "expirationTimestamp" in status:
-                self.expiry = parse_rfc3339(status["expirationTimestamp"])
+                self.expiry = parse(status["expirationTimestamp"])
             return True
         except Exception as e:
             logging.error(str(e))
 
     def _load_user_token(self):
         base_path = self._get_base_path(self._user.path)
         token = FileOrData(
@@ -666,15 +662,15 @@
         if config is None:
             raise ConfigException("Invalid kube-config.")
         if self.config_merged is None:
             self.config_merged = copy.deepcopy(config)
         # doesn't need to do any further merging
 
     def _load_config_from_file_path(self, string):
-        for path in string.split(ENV_KUBECONFIG_PATH_SEPARATOR):
+        for path in string.split(os.pathsep):
             if path:
                 path = os.path.expanduser(path)
                 if os.path.exists(path):
                     self.paths.append(path)
                     self.load_config(path)
         self.config_saved = copy.deepcopy(self.config_files)
 
@@ -727,15 +723,14 @@
             raise ConfigException("Invalid kube-config file. " "No configuration found.")
         return KubeConfigLoader(config_dict=kcfg.config, config_base_path=None, **kwargs)
     else:
         return KubeConfigLoader(config_dict=config_dict, config_base_path=None, **kwargs)
 
 
 def list_kube_config_contexts(config_file=None):
-
     if config_file is None:
         config_file = KUBE_CONFIG_DEFAULT_LOCATION
 
     loader = _get_kube_config_loader(filename=config_file)
     return loader.list_contexts(), loader.current_context
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/kube/resource_api.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/kube/resource_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import re
 from typing import TYPE_CHECKING, Callable, Generic, Iterator, Optional, Type, TypeVar, cast, overload
 
 from kubernetes_dynamic.events import Event, Watch
 from kubernetes_dynamic.exceptions import EventTimeoutError
 from kubernetes_dynamic.formatters import format_selector
 from kubernetes_dynamic.kube.exceptions import ConflictError, NotFoundError, UnprocessibleEntityError
+from kubernetes_dynamic.models.common import get_type
 from kubernetes_dynamic.models.resource_value import ResourceValue
 
 R = TypeVar("R", bound=ResourceValue)
 
 if TYPE_CHECKING:
+    from kubernetes_dynamic import models
     from kubernetes_dynamic.client import K8sClient
     from kubernetes_dynamic.models.common import ItemList
     from kubernetes_dynamic.models.resource_item import CheckResult
 
 
 class _Missing:
     pass
@@ -57,15 +59,17 @@
         self.name = name
         self.preferred = preferred
         self.singular_name = singularName or (name[:-1] if name else "")
         self.short_names = shortNames
         self.categories = categories
         self.subresources = {k: Subresource(self, **v) for k, v in (subresources or {}).items()}
         self.client: K8sClient = client
-        self.resource_type: Optional[Type[R]] = resource_type
+        self.resource_type: Optional[Type[R]] = resource_type or get_type(
+            self.kind, self.api_version, None  # type: ignore
+        )
 
         self.extra_args = kwargs
 
     def to_dict(self):
         d = {
             "_type": "Resource",
             "prefix": self.prefix,
@@ -132,15 +136,15 @@
         return body or {}
 
     def ensure_namespace_param(self, namespace: Optional[str | _Missing], body=None, allow_all=False) -> Optional[str]:
         if not self.namespaced:
             return None
         if namespace is MISSING:
             if body:
-                namespace = body.get("metadata", {}).get("namespace", self.config.namespace)
+                namespace = body.get("metadata", {}).get("namespace") or self.client.config.namespace
             else:
                 namespace = self.client.config.namespace
         if not allow_all and not namespace:
             raise ValueError("Namespace is required for {}.{}".format(self.group_version, self.kind))
         return cast(Optional[str], namespace)
 
     def ensure_name_param(self, name, body=None) -> str:
@@ -244,23 +248,26 @@
         for item in data:
             if re.match(pattern, item.metadata.name):
                 items.append(item)
         return items
 
     def create(self, body: dict | R, namespace: Optional[str | _Missing] = MISSING, **kwargs) -> R:
         body = self.serialize_body(body)
+        body["metadata"]["resourceVersion"] = None
         namespace = self.ensure_namespace_param(namespace, body)
+        if namespace:
+            body["metadata"]["namespace"] = namespace
         path = self.path(namespace=namespace)
         kwargs.setdefault("serializer", self.resource_type)
         return self.client.request("post", path, body=body, **kwargs)
 
     @overload
     def delete(
         self, name: str, namespace: Optional[str | _Missing] = MISSING, body: Optional[dict | R] = None, **kwargs
-    ) -> R:
+    ) -> models.V1Status:
         ...  # pragma: no cover
 
     @overload
     def delete(
         self,
         *,
         namespace: Optional[str | _Missing] = MISSING,
@@ -275,21 +282,24 @@
         self,
         name: Optional[str] = None,
         namespace: Optional[str | _Missing] = MISSING,
         body: Optional[dict | R] = None,
         label_selector: Optional[str] = None,
         field_selector: Optional[str] = None,
         **kwargs,
-    ) -> ItemList[R] | R:
+    ) -> ItemList[R] | models.V1Status:
         if not (name or label_selector or field_selector):
             raise ValueError("At least one of name|label_selector|field_selector is required")
         if self.namespaced and not (label_selector or field_selector):
             namespace = self.ensure_namespace_param(namespace, allow_all=not name)
+        if namespace is MISSING:
+            namespace = None
+        if not name:
+            kwargs.setdefault("serializer", self.resource_type)
         path = self.path(name=name, namespace=namespace)
-        kwargs.setdefault("serializer", self.resource_type)
         return self.client.request(
             "delete", path, body=body, label_selector=label_selector, field_selector=field_selector, **kwargs
         )
 
     def replace(
         self, body: dict | R, name: Optional[str] = None, namespace: Optional[str | _Missing] = MISSING, **kwargs
     ) -> R:
@@ -327,16 +337,16 @@
         kwargs.update({"content_type": "application/apply-patch+yaml"})
         path = self.path(name=name, namespace=namespace)
         kwargs.setdefault("serializer", self.resource_type)
         return self.client.request("patch", path, body=body, force_conflicts=force_conflicts, **kwargs)
 
     def watch(
         self,
-        namespace: Optional[str | _Missing] = MISSING,
         name: Optional[str] = None,
+        namespace: Optional[str | _Missing] = MISSING,
         label_selector: Optional[str] = None,
         field_selector: Optional[str] = None,
         resource_version: Optional[str] = None,
         timeout: Optional[float] = None,
         watcher: Optional[Watch] = None,
     ) -> Iterator[Event[R]]:
         namespace = self.ensure_namespace_param(namespace, allow_all=True)
@@ -349,15 +359,14 @@
         return watcher.stream(
             self.get,
             namespace=namespace or self.client.config.namespace,
             name=None,
             field_selector=field_selector,
             label_selector=label_selector,
             resource_version=resource_version,
-            serialize=False,
             timeout_seconds=timeout,
         )
 
     def wait_until(
         self,
         *,
         namespace: Optional[str | _Missing] = MISSING,
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/__init__.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/all.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/all.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/common.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/common.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/configmap.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/configmap.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/ingress.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/ingress.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/namespace.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/namespace.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/pod.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/pod.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/replica_set.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/replica_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/resource_item.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/resource_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import typing
 from typing import Callable, Optional
 
 import pydantic
 from typing_extensions import Self
 
 from kubernetes_dynamic.events import Event, EventType
+from kubernetes_dynamic.kube.resource_api import MISSING, _Missing
 
 from ..exceptions import NotFoundError
-from .common import V1ObjectMeta
+from .common import ItemList, V1ObjectMeta
 from .resource_value import ResourceValue
 
 if typing.TYPE_CHECKING:
     from kubernetes_dynamic.kube.resource_api import ResourceApi
 
     from ..client import K8sClient
 
@@ -105,14 +106,48 @@
     @classmethod
     def default_client(cls) -> K8sClient:
         """Create a default K8sClient."""
         from ..client import K8sClient
 
         return K8sClient()
 
+    @classmethod
+    def default_api(cls, client: Optional[K8sClient] = None) -> ResourceApi:
+        """Create a default K8sClient."""
+        client = client or cls.default_client()
+        default_values = cls.get_defaults()
+        return client.get_api(kind=default_values["kind"], api_version=default_values["apiVersion"])
+
+    @classmethod
+    def list_(
+        cls,
+        *,
+        namespace: Optional[str | _Missing] = MISSING,
+        label_selector: Optional[str] = None,
+        field_selector: Optional[str] = None,
+        client: Optional[K8sClient] = None,
+        **kwargs,
+    ) -> ItemList[Self]:
+        """Create a default K8sClient."""
+        return cls.default_api(client).get(
+            namespace=namespace, label_selector=label_selector, field_selector=field_selector, **kwargs
+        )
+
+    @classmethod
+    def get_(
+        cls,
+        name: str,
+        *,
+        namespace: Optional[str | _Missing] = MISSING,
+        client: Optional[K8sClient] = None,
+        **kwargs,
+    ) -> Optional[Self]:
+        """Create a default K8sClient."""
+        return cls.default_api(client).get(name, namespace=namespace, **kwargs)
+
     def refresh_(self) -> Self:
         """Refreshes the local instance with kubernetes data."""
         data = self.read_()
         if data is None:
             raise NotFoundError(self)
         return self._update_attrs(data)
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/resource_value.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/resource_value.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/secret.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/secret.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,14 @@
     data: Dict[str, str] = Field(default_factory=dict)
     immutable: bool = False
     stringData: Dict[str, str] = Field(default_factory=dict)
     type: str = "Opaque"
 
     _required_keys: Union[tuple, List] = PrivateAttr(default_factory=tuple)
 
-    def __init__(
-        self,
-        *args,
-        required_keys: Union[tuple, List] = (),
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        self._required_keys = required_keys
-
     def exists(self) -> bool:
         """Checks if the secret exists in Kubernetes."""
         return self.read_() is not None
 
     def validate_keys(self) -> Tuple[bool, bool, list]:
         """Validates a secret exists and has the correct format."""
         secret = self.read_()
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/service.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/service.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/models/stateful_set.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/models/stateful_set.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/api_client.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/api_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,15 @@
-# coding: utf-8
-
-"""
-    Kubernetes
-
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
-
-    The version of the OpenAPI document: unversioned
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
-"""
-
-
 import atexit
 import datetime
 import json
 import mimetypes
 import os
-import re
-import tempfile
 from multiprocessing.pool import ThreadPool
 from urllib.parse import quote
 
-from dateutil.parser import parse
-
 from . import rest
 from .configuration import Configuration
 from .exceptions import ApiException, ApiValueError
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
@@ -46,15 +28,14 @@
     :param pool_threads: The number of threads to use for async requests
         to the API. More threads means more concurrent API requests.
     """
 
     PRIMITIVE_TYPES = (float, bool, bytes, str, int)
     NATIVE_TYPES_MAPPING = {
         "int": int,
-        "long": int,  # TODO remove as only py3 is supported?
         "float": float,
         "str": str,
         "bool": bool,
         "date": datetime.date,
         "datetime": datetime.datetime,
         "object": object,
     }
@@ -153,15 +134,14 @@
         _return_http_data_only=None,
         collection_formats=None,
         _preload_content=True,
         _request_timeout=None,
         _host=None,
         _request_auth=None,
     ):
-
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params["Cookie"] = self.cookie
@@ -223,41 +203,15 @@
                 e.body = e.body.decode("utf-8")
             raise e
 
         self.last_response = response_data
 
         return_data = response_data
 
-        if not _preload_content:
-            return return_data
-
-        response_type = response_types_map.get(str(response_data.status), None)
-
-        if response_type == "bytearray":
-            response_data.data = response_data.data
-        else:
-            match = None
-            content_type = response_data.getheader("content-type")
-            if content_type is not None:
-                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
-            encoding = match.group(1) if match else "utf-8"
-            response_data.data = response_data.data.decode(encoding)
-
-        # deserialize response data
-        if response_type == "bytearray":
-            return_data = response_data.data
-        elif response_type:
-            return_data = self.deserialize(response_data, response_type)
-        else:
-            return_data = None
-
-        if _return_http_data_only:
-            return return_data
-        else:
-            return (return_data, response_data.status, response_data.getheaders())
+        return return_data
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
@@ -288,71 +242,14 @@
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
             obj_dict = obj.to_dict()
 
         return {key: self.sanitize_for_serialization(val) for key, val in obj_dict.items()}
 
-    def deserialize(self, response, response_type):
-        """Deserializes response into an object.
-
-        :param response: RESTResponse object to be deserialized.
-        :param response_type: class literal for
-            deserialized object, or string of class name.
-
-        :return: deserialized object.
-        """
-        # handle file downloading
-        # save response body into a tmp file and return the instance
-        if response_type == "file":
-            return self.__deserialize_file(response)
-
-        # fetch data from response object
-        try:
-            data = json.loads(response.data)
-        except ValueError:
-            data = response.data
-
-        return self.__deserialize(data, response_type)
-
-    def __deserialize(self, data, klass):
-        """Deserializes dict, list, str into an object.
-
-        :param data: dict, list or str.
-        :param klass: class literal, or string of class name.
-
-        :return: object.
-        """
-        if data is None:
-            return None
-
-        if type(klass) == str:
-            if klass.startswith("List["):
-                sub_kls = re.match(r"List\[(.*)]", klass).group(1)
-                return [self.__deserialize(sub_data, sub_kls) for sub_data in data]
-
-            if klass.startswith("Dict["):
-                sub_kls = re.match(r"Dict\[([^,]*), (.*)]", klass).group(2)
-                return {k: self.__deserialize(v, sub_kls) for k, v in data.items()}
-
-            # convert str to class
-            if klass in self.NATIVE_TYPES_MAPPING:
-                klass = self.NATIVE_TYPES_MAPPING[klass]
-
-        if klass in self.PRIMITIVE_TYPES:
-            return self.__deserialize_primitive(data, klass)
-        elif klass == object:
-            return self.__deserialize_object(data)
-        elif klass == datetime.date:
-            return self.__deserialize_date(data)
-        elif klass == datetime.datetime:
-            return self.__deserialize_datetime(data)
-        else:
-            return self.__deserialize_model(data, klass)
-
     def call_api(
         self,
         resource_path,
         method,
         path_params=None,
         query_params=None,
         header_params=None,
@@ -533,69 +430,35 @@
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
         new_params = []
-        if collection_formats is None:
-            collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
-            if k in collection_formats:
-                collection_format = collection_formats[k]
-                if collection_format == "multi":
-                    new_params.extend((k, value) for value in v)
-                else:
-                    if collection_format == "ssv":
-                        delimiter = " "
-                    elif collection_format == "tsv":
-                        delimiter = "\t"
-                    elif collection_format == "pipes":
-                        delimiter = "|"
-                    else:  # csv is the default
-                        delimiter = ","
-                    new_params.append((k, delimiter.join(str(value) for value in v)))
-            else:
-                new_params.append((k, v))
+            new_params.append((k, v))
         return new_params
 
     def parameters_to_url_query(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: URL query string (e.g. a=Hello%20World&b=123)
         """
         new_params = []
-        if collection_formats is None:
-            collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
             if isinstance(v, (int, float)):
                 v = str(v)
             if isinstance(v, bool):
                 v = str(v).lower()
             if isinstance(v, dict):
                 v = json.dumps(v)
 
-            if k in collection_formats:
-                collection_format = collection_formats[k]
-                if collection_format == "multi":
-                    new_params.extend((k, value) for value in v)
-                else:
-                    if collection_format == "ssv":
-                        delimiter = " "
-                    elif collection_format == "tsv":
-                        delimiter = "\t"
-                    elif collection_format == "pipes":
-                        delimiter = "|"
-                    else:  # csv is the default
-                        delimiter = ","
-                    new_params.append((k, delimiter.join(quote(str(value)) for value in v)))
-            else:
-                new_params.append((k, quote(str(v))))
+            new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(item) for item in new_params])
 
     def files_parameters(self, files=None):
         """Builds form parameters.
 
         :param files: File parameters.
@@ -613,44 +476,14 @@
                         filename = os.path.basename(f.name)
                         filedata = f.read()
                         mimetype = mimetypes.guess_type(filename)[0] or "application/octet-stream"
                         params.append(tuple([k, tuple([filename, filedata, mimetype])]))
 
         return params
 
-    def select_header_accept(self, accepts):
-        """Returns `Accept` based on an array of accepts provided.
-
-        :param accepts: List of headers.
-        :return: Accept (e.g. application/json).
-        """
-        if not accepts:
-            return
-
-        for accept in accepts:
-            if re.search("json", accept, re.IGNORECASE):
-                return accept
-
-        return accepts[0]
-
-    def select_header_content_type(self, content_types):
-        """Returns `Content-Type` based on an array of content_types provided.
-
-        :param content_types: List of content-types.
-        :return: Content-Type (e.g. application/json).
-        """
-        if not content_types:
-            return "application/json"
-
-        for content_type in content_types:
-            if re.search("json", content_type, re.IGNORECASE):
-                return content_type
-
-        return content_types[0]
-
     def update_params_for_auth(self, headers, queries, auth_settings, resource_path, method, body, request_auth=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :resource_path: A string representation of the HTTP request resource path.
@@ -688,90 +521,7 @@
         elif auth_setting["in"] == "header":
             if auth_setting["type"] != "http-signature":
                 headers[auth_setting["key"]] = auth_setting["value"]
         elif auth_setting["in"] == "query":
             queries.append((auth_setting["key"], auth_setting["value"]))
         else:
             raise ApiValueError("Authentication token must be in `query` or `header`")
-
-    def __deserialize_file(self, response):
-        """Deserializes body to file
-
-        Saves response body into a file in a temporary folder,
-        using the filename from the `Content-Disposition` header if provided.
-
-        :param response:  RESTResponse.
-        :return: file path.
-        """
-        fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
-        os.close(fd)
-        os.remove(path)
-
-        content_disposition = response.getheader("Content-Disposition")
-        if content_disposition:
-            filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?', content_disposition).group(1)
-            path = os.path.join(os.path.dirname(path), filename)
-
-        with open(path, "wb") as f:
-            f.write(response.data)
-
-        return path
-
-    def __deserialize_primitive(self, data, klass):
-        """Deserializes string to primitive type.
-
-        :param data: str.
-        :param klass: class literal.
-
-        :return: int, long, float, str, bool.
-        """
-        try:
-            return klass(data)
-        except UnicodeEncodeError:
-            return str(data)
-        except TypeError:
-            return data
-
-    def __deserialize_object(self, value):
-        """Return an original value.
-
-        :return: object.
-        """
-        return value
-
-    def __deserialize_date(self, string):
-        """Deserializes string to date.
-
-        :param string: str.
-        :return: date.
-        """
-        try:
-            return parse(string).date()
-        except ImportError:
-            return string
-        except ValueError:
-            raise rest.ApiException(status=0, reason="Failed to parse `{0}` as date object".format(string))
-
-    def __deserialize_datetime(self, string):
-        """Deserializes string to datetime.
-
-        The string should be in iso8601 datetime format.
-
-        :param string: str.
-        :return: datetime.
-        """
-        try:
-            return parse(string)
-        except ImportError:
-            return string
-        except ValueError:
-            raise rest.ApiException(status=0, reason=("Failed to parse `{0}` as datetime object".format(string)))
-
-    def __deserialize_model(self, data, klass):
-        """Deserializes list or dict to model.
-
-        :param data: dict, list.
-        :param klass: class literal.
-        :return: model object.
-        """
-
-        return klass.from_dict(data)
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/configuration.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic/openapi_client/rest.py` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic/openapi_client/rest.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     The version of the OpenAPI document: unversioned
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-import io
 import json
 import logging
 import re
 import ssl
 
 import urllib3
 import urllib3.exceptions
@@ -29,39 +28,16 @@
     ServiceException,
     UnauthorizedException,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class RESTResponse(io.IOBase):
-    def __init__(self, resp):
-        self.urllib3_response = resp
-        self.status = resp.status
-        self.reason = resp.reason
-        self.data = resp.data
-
-    def getheaders(self):
-        """Returns a dictionary of the response headers."""
-        return self.urllib3_response.headers
-
-    def getheader(self, name, default=None):
-        """Returns a given response header."""
-        return self.urllib3_response.headers.get(name, default)
-
-
 class RESTClientObject(object):
     def __init__(self, configuration, pools_size=4, maxsize=None):
-        # urllib3.PoolManager will pass all kw parameters to connectionpool
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
-        # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
-        # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
-        # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
-
-        # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
@@ -86,25 +62,25 @@
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
+                **addition_pool_args,
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
-                **addition_pool_args
+                **addition_pool_args,
             )
 
     def request(
         self,
         method,
         url,
         query_params=None,
@@ -149,15 +125,14 @@
                 timeout = urllib3.Timeout(total=_request_timeout)
             elif isinstance(_request_timeout, tuple) and len(_request_timeout) == 2:
                 timeout = urllib3.Timeout(connect=_request_timeout[0], read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
-
                 # no content type provided or payload is json
                 if not headers.get("Content-Type") or re.search("json", headers["Content-Type"], re.IGNORECASE):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
                         method,
@@ -215,20 +190,14 @@
                 r = self.pool_manager.request(
                     method, url, fields={}, preload_content=_preload_content, timeout=timeout, headers=headers
                 )
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
-        if _preload_content:
-            r = RESTResponse(r)
-
-            # log response body
-            logger.debug("response body: %s", r.data)
-
         if not 200 <= r.status <= 299:
             if r.status == 401:
                 raise UnauthorizedException(http_resp=r)
 
             if r.status == 403:
                 raise ForbiddenException(http_resp=r)
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/PKG-INFO` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernetes-dynamic
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kubernetes Dynamic client
 Author-email: Attila Kobor <atti92@gmail.com>, Balazs Hamorszky <balihb@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/atti92/kubernetes-dynamic
 Project-URL: documentation, https://github.com/atti92/kubernetes-dynamic
 Project-URL: repository, https://github.com/atti92/kubernetes-dynamic.git
 Project-URL: changelog, https://github.com/atti92/kubernetes-dynamic/blob/main/README.md
```

### Comparing `kubernetes-dynamic-0.1.1/kubernetes_dynamic.egg-info/SOURCES.txt` & `kubernetes-dynamic-0.1.2/kubernetes_dynamic.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 kubernetes_dynamic/formatters.py
 kubernetes_dynamic.egg-info/PKG-INFO
 kubernetes_dynamic.egg-info/SOURCES.txt
 kubernetes_dynamic.egg-info/dependency_links.txt
 kubernetes_dynamic.egg-info/requires.txt
 kubernetes_dynamic.egg-info/top_level.txt
 kubernetes_dynamic/kube/__init__.py
-kubernetes_dynamic/kube/dateutil.py
 kubernetes_dynamic/kube/discovery.py
 kubernetes_dynamic/kube/exceptions.py
 kubernetes_dynamic/kube/exec_provider.py
 kubernetes_dynamic/kube/incluster_config.py
 kubernetes_dynamic/kube/kube_config.py
 kubernetes_dynamic/kube/resource_api.py
 kubernetes_dynamic/kube/ws_client.py
@@ -38,17 +37,8 @@
 kubernetes_dynamic/models/service.py
 kubernetes_dynamic/models/stateful_set.py
 kubernetes_dynamic/openapi_client/__init__.py
 kubernetes_dynamic/openapi_client/api_client.py
 kubernetes_dynamic/openapi_client/configuration.py
 kubernetes_dynamic/openapi_client/exceptions.py
 kubernetes_dynamic/openapi_client/rest.py
-tests/test_client.py
-tests/test_config.py
-tests/test_configmap.py
-tests/test_ingress.py
-tests/test_namespace.py
-tests/test_pod.py
-tests/test_resource_api.py
-tests/test_resource_item.py
-tests/test_resource_value.py
-tests/test_secret.py
+tests/test_sandbox.py
```

### Comparing `kubernetes-dynamic-0.1.1/pyproject.toml` & `kubernetes-dynamic-0.1.2/pyproject.toml`

 * *Files identical despite different names*

