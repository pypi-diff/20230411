# Comparing `tmp/icotest-voice-1.0.32.tar.gz` & `tmp/icotest-voice-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.32.tar", last modified: Tue Mar 28 06:02:43 2023, max compression
+gzip compressed data, was "icotest-voice-1.0.33.tar", last modified: Tue Apr 11 16:58:42 2023, max compression
```

## Comparing `icotest-voice-1.0.32.tar` & `icotest-voice-1.0.33.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.710197 icotest-voice-1.0.32/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.32/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.32/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8390 2023-03-28 06:02:43.710197 icotest-voice-1.0.32/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6802 2023-03-28 05:59:26.000000 icotest-voice-1.0.32/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.706197 icotest-voice-1.0.32/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      785 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8572 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37192 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      325 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/InlineObject.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/InlineResponse200Files.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/Message.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.706197 icotest-voice-1.0.32/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1376 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.706197 icotest-voice-1.0.32/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   105234 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.710197 icotest-voice-1.0.32/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      777 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9253 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14073 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3558 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.706197 icotest-voice-1.0.32/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8390 2023-03-28 06:02:43.000000 icotest-voice-1.0.32/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1339 2023-03-28 06:02:43.000000 icotest-voice-1.0.32/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-03-28 06:02:43.000000 icotest-voice-1.0.32/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-03-28 06:02:43.000000 icotest-voice-1.0.32/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-03-28 06:02:43.000000 icotest-voice-1.0.32/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-03-28 06:00:53.000000 icotest-voice-1.0.32/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-03-28 06:02:43.710197 icotest-voice-1.0.32/setup.cfg
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-03-28 06:02:43.710197 icotest-voice-1.0.32/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1618 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1831 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1404 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-03-28 05:51:41.000000 icotest-voice-1.0.32/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.33/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.33/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8426 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6838 2023-04-11 16:53:31.000000 icotest-voice-1.0.33/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.429165 icotest-voice-1.0.33/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      832 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37038 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineObject.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineObject1.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineResponse200.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/InlineResponse200Files.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Message.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10413 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14073 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.433166 icotest-voice-1.0.33/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8426 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-04-11 16:58:42.000000 icotest-voice-1.0.33/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-04-11 16:48:26.000000 icotest-voice-1.0.33/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-04-11 16:58:42.437166 icotest-voice-1.0.33/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1831 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-04-11 16:45:14.000000 icotest-voice-1.0.33/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.32/LICENSE` & `icotest-voice-1.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.32/PKG-INFO` & `icotest-voice-1.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.32
+Version: 1.0.33
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.32
-- Package version: 1.0.32
+- API version: 1.0.33
+- Package version: 1.0.33
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -69,16 +69,15 @@
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
     controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
-        print("Exception when calling ControllersApi.delete_controller(): %s\n" % e)
-    
+        print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
@@ -119,14 +118,15 @@
 
 ## Documentation For Models
 
  - [Controller](docs/Controller.md)
  - [Device](docs/Device.md)
  - [HostConfig](docs/HostConfig.md)
  - [InlineObject](docs/InlineObject.md)
+ - [InlineObject1](docs/InlineObject1.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse200Files](docs/InlineResponse200Files.md)
  - [Message](docs/Message.md)
  - [Request](docs/Request.md)
 
 
 ## Documentation For Authorization
```

### Comparing `icotest-voice-1.0.32/README.md` & `icotest-voice-1.0.33/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.32
-- Package version: 1.0.32
+- API version: 1.0.33
+- Package version: 1.0.33
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -48,16 +48,15 @@
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
     controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
-        print("Exception when calling ControllersApi.delete_controller(): %s\n" % e)
-    
+        print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
@@ -98,14 +97,15 @@
 
 ## Documentation For Models
 
  - [Controller](docs/Controller.md)
  - [Device](docs/Device.md)
  - [HostConfig](docs/HostConfig.md)
  - [InlineObject](docs/InlineObject.md)
+ - [InlineObject1](docs/InlineObject1.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse200Files](docs/InlineResponse200Files.md)
  - [Message](docs/Message.md)
  - [Request](docs/Request.md)
 
 
 ## Documentation For Authorization
```

### Comparing `icotest-voice-1.0.32/docs/Controller.md` & `icotest-voice-1.0.33/docs/Controller.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Controller
 
 The model of a controller
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **controller_id** | **str** | the unique id of the controller | [optional] 
+**controller_type** | **str** |  | [optional] 
 **description** | **str** | the description of the controller | [optional] 
 **location** | **str** | the location of the controller | [optional] 
 **callback_url** | **str** | the url to contact the controller | [optional] 
 **created** | **datetime** | The date the controller was added | [optional] 
 **last_contact** | **datetime** | The last contact date time with the controller | [optional] 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `icotest-voice-1.0.32/docs/ControllersApi.md` & `icotest-voice-1.0.33/docs/ControllersApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 )
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller = {"controller_id":"10cda64a-0dce-4663-8b47-6ec1867f9568","description":"example controller","location":"server 1 rack 1","callback_url":"https://server:port","created":"2021-06-24T14:15:22Z","last_contact":"2021-06-24T14:15:22Z"} # Controller | The model of a controller (optional)
+    controller = {"controller_id":"10cda64a-0dce-4663-8b47-6ec1867f9568","controller_type":"dect","description":"example controller","location":"server 1 rack 1","callback_url":"https://server:port","created":"2021-06-24T14:15:22Z","last_contact":"2021-06-24T14:15:22Z"} # Controller | The model of a controller (optional)
 
     try:
         # PUT controller
         api_instance.put_controller(controller=controller)
     except ApiException as e:
         print("Exception when calling ControllersApi->put_controller: %s\n" % e)
 ```
```

### Comparing `icotest-voice-1.0.32/docs/Device.md` & `icotest-voice-1.0.33/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.32/docs/DevicesApi.md` & `icotest-voice-1.0.33/docs/DevicesApi.md`

 * *Files 2% similar despite different names*

```diff
@@ -715,15 +715,15 @@
 **403** | Forbidden |  -  |
 **404** | Not Found |  -  |
 **500** | Internal Server Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **post_device_register**
-> str post_device_register(device_id, channel_number=channel_number, pin_code=pin_code)
+> str post_device_register(device_id, inline_object=inline_object)
 
 POST register device
 
 Post request to perform a device register to base station
 
 ### Example
 
@@ -741,44 +741,42 @@
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.DevicesApi(api_client)
     device_id = 'bc331ccb-5841-44ec-9d32-4f4fe0c3c16c' # str | the unique id of the device
-channel_number = 56 # int | the number of the channel (optional)
-pin_code = '1234' # str | the 4 to 8-digit PIN code (optional)
+inline_object = icotest_voice.InlineObject() # InlineObject |  (optional)
 
     try:
         # POST register device
-        api_response = api_instance.post_device_register(device_id, channel_number=channel_number, pin_code=pin_code)
+        api_response = api_instance.post_device_register(device_id, inline_object=inline_object)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling DevicesApi->post_device_register: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **device_id** | [**str**](.md)| the unique id of the device | 
- **channel_number** | **int**| the number of the channel | [optional] 
- **pin_code** | **str**| the 4 to 8-digit PIN code | [optional] 
+ **inline_object** | [**InlineObject**](InlineObject.md)|  | [optional] 
 
 ### Return type
 
 **str**
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: Not defined
+ - **Content-Type**: application/json
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Example response |  -  |
 **400** | Bad Request |  -  |
```

### Comparing `icotest-voice-1.0.32/docs/Request.md` & `icotest-voice-1.0.33/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.32/docs/RequestsApi.md` & `icotest-voice-1.0.33/docs/RequestsApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.32/icotest_voice/__init__.py` & `icotest-voice-1.0.33/icotest_voice/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.32"
+__version__ = "1.0.33"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
@@ -31,12 +31,13 @@
 from icotest_voice.exceptions import ApiKeyError
 from icotest_voice.exceptions import ApiException
 # import models into sdk package
 from icotest_voice.models.controller import Controller
 from icotest_voice.models.device import Device
 from icotest_voice.models.host_config import HostConfig
 from icotest_voice.models.inline_object import InlineObject
+from icotest_voice.models.inline_object1 import InlineObject1
 from icotest_voice.models.inline_response200 import InlineResponse200
 from icotest_voice.models.inline_response200_files import InlineResponse200Files
 from icotest_voice.models.message import Message
 from icotest_voice.models.request import Request
```

### Comparing `icotest-voice-1.0.32/icotest_voice/api/controllers_api.py` & `icotest-voice-1.0.33/icotest_voice/api/controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/icotest_voice/api/devices_api.py` & `icotest-voice-1.0.33/icotest_voice/api/devices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -1330,16 +1330,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.post_device_register(device_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str device_id: the unique id of the device (required)
-        :param int channel_number: the number of the channel
-        :param str pin_code: the 4 to 8-digit PIN code
+        :param InlineObject inline_object:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1357,16 +1356,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.post_device_register_with_http_info(device_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str device_id: the unique id of the device (required)
-        :param int channel_number: the number of the channel
-        :param str pin_code: the 4 to 8-digit PIN code
+        :param InlineObject inline_object:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1377,16 +1375,15 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'device_id',
-            'channel_number',
-            'pin_code'
+            'inline_object'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -1410,56 +1407,38 @@
                                                         len(local_var_params['device_id']) > 36):  # noqa: E501
             raise ApiValueError("Invalid value for parameter `device_id` when calling `post_device_register`, length must be less than or equal to `36`")  # noqa: E501
         if self.api_client.client_side_validation and ('device_id' in local_var_params and  # noqa: E501
                                                         len(local_var_params['device_id']) < 36):  # noqa: E501
             raise ApiValueError("Invalid value for parameter `device_id` when calling `post_device_register`, length must be greater than or equal to `36`")  # noqa: E501
         if self.api_client.client_side_validation and 'device_id' in local_var_params and not re.search(r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}', local_var_params['device_id']):  # noqa: E501
             raise ApiValueError("Invalid value for parameter `device_id` when calling `post_device_register`, must conform to the pattern `/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('channel_number' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['channel_number']) > 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `channel_number` when calling `post_device_register`, length must be less than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and ('channel_number' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['channel_number']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `channel_number` when calling `post_device_register`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'channel_number' in local_var_params and local_var_params['channel_number'] > 9:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `channel_number` when calling `post_device_register`, must be a value less than or equal to `9`")  # noqa: E501
-        if self.api_client.client_side_validation and 'channel_number' in local_var_params and local_var_params['channel_number'] < 0:  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `channel_number` when calling `post_device_register`, must be a value greater than or equal to `0`")  # noqa: E501
-        if self.api_client.client_side_validation and 'channel_number' in local_var_params and not re.search(r'[0-9]', local_var_params['channel_number']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `channel_number` when calling `post_device_register`, must conform to the pattern `/[0-9]/`")  # noqa: E501
-        if self.api_client.client_side_validation and ('pin_code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['pin_code']) > 8):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `pin_code` when calling `post_device_register`, length must be less than or equal to `8`")  # noqa: E501
-        if self.api_client.client_side_validation and ('pin_code' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['pin_code']) < 4):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `pin_code` when calling `post_device_register`, length must be greater than or equal to `4`")  # noqa: E501
-        if self.api_client.client_side_validation and 'pin_code' in local_var_params and not re.search(r'^\d{4,8}$', local_var_params['pin_code']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `pin_code` when calling `post_device_register`, must conform to the pattern `/^\d{4,8}$/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
         if 'device_id' in local_var_params:
             path_params['device_id'] = local_var_params['device_id']  # noqa: E501
 
         query_params = []
-        if 'channel_number' in local_var_params and local_var_params['channel_number'] is not None:  # noqa: E501
-            query_params.append(('channel_number', local_var_params['channel_number']))  # noqa: E501
-        if 'pin_code' in local_var_params and local_var_params['pin_code'] is not None:  # noqa: E501
-            query_params.append(('pin_code', local_var_params['pin_code']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'inline_object' in local_var_params:
+            body_params = local_var_params['inline_object']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
             '/devices/{device_id}/register', 'POST',
             path_params,
             query_params,
```

### Comparing `icotest-voice-1.0.32/icotest_voice/api/requests_api.py` & `icotest-voice-1.0.33/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/icotest_voice/api_client.py` & `icotest-voice-1.0.33/icotest_voice/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.32/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.33/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `icotest-voice-1.0.32/icotest_voice/configuration.py` & `icotest-voice-1.0.33/icotest_voice/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -251,16 +251,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.32\n"\
-               "SDK Package Version: 1.0.32".\
+               "Version of the API: 1.0.33\n"\
+               "SDK Package Version: 1.0.33".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.32/icotest_voice/exceptions.py` & `icotest-voice-1.0.33/icotest_voice/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/__init__.py` & `icotest-voice-1.0.33/icotest_voice/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from icotest_voice.models.controller import Controller
 from icotest_voice.models.device import Device
 from icotest_voice.models.host_config import HostConfig
 from icotest_voice.models.inline_object import InlineObject
+from icotest_voice.models.inline_object1 import InlineObject1
 from icotest_voice.models.inline_response200 import InlineResponse200
 from icotest_voice.models.inline_response200_files import InlineResponse200Files
 from icotest_voice.models.message import Message
 from icotest_voice.models.request import Request
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/controller.py` & `icotest-voice-1.0.33/icotest_voice/models/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -31,46 +31,51 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'controller_id': 'str',
+        'controller_type': 'str',
         'description': 'str',
         'location': 'str',
         'callback_url': 'str',
         'created': 'datetime',
         'last_contact': 'datetime'
     }
 
     attribute_map = {
         'controller_id': 'controller_id',
+        'controller_type': 'controller_type',
         'description': 'description',
         'location': 'location',
         'callback_url': 'callback_url',
         'created': 'created',
         'last_contact': 'last_contact'
     }
 
-    def __init__(self, controller_id=None, description=None, location=None, callback_url=None, created=None, last_contact=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, controller_id=None, controller_type=None, description=None, location=None, callback_url=None, created=None, last_contact=None, local_vars_configuration=None):  # noqa: E501
         """Controller - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._controller_id = None
+        self._controller_type = None
         self._description = None
         self._location = None
         self._callback_url = None
         self._created = None
         self._last_contact = None
         self.discriminator = None
 
         if controller_id is not None:
             self.controller_id = controller_id
+        if controller_type is not None:
+            self.controller_type = controller_type
         if description is not None:
             self.description = description
         if location is not None:
             self.location = location
         if callback_url is not None:
             self.callback_url = callback_url
         if created is not None:
@@ -107,14 +112,41 @@
         if (self.local_vars_configuration.client_side_validation and
                 controller_id is not None and not re.search(r'[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}', controller_id)):  # noqa: E501
             raise ValueError(r"Invalid value for `controller_id`, must be a follow pattern or equal to `/[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}/`")  # noqa: E501
 
         self._controller_id = controller_id
 
     @property
+    def controller_type(self):
+        """Gets the controller_type of this Controller.  # noqa: E501
+
+
+        :return: The controller_type of this Controller.  # noqa: E501
+        :rtype: str
+        """
+        return self._controller_type
+
+    @controller_type.setter
+    def controller_type(self, controller_type):
+        """Sets the controller_type of this Controller.
+
+
+        :param controller_type: The controller_type of this Controller.  # noqa: E501
+        :type: str
+        """
+        allowed_values = ["dect", "sip"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and controller_type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `controller_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(controller_type, allowed_values)
+            )
+
+        self._controller_type = controller_type
+
+    @property
     def description(self):
         """Gets the description of this Controller.  # noqa: E501
 
         the description of the controller  # noqa: E501
 
         :return: The description of this Controller.  # noqa: E501
         :rtype: str
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/device.py` & `icotest-voice-1.0.33/icotest_voice/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/host_config.py` & `icotest-voice-1.0.33/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/inline_object.py` & `icotest-voice-1.0.33/icotest_voice/models/inline_object1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from icotest_voice.configuration import Configuration
 
 
-class InlineObject(object):
+class InlineObject1(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -38,40 +38,40 @@
     }
 
     attribute_map = {
         'playback_file': 'playback_file'
     }
 
     def __init__(self, playback_file=None, local_vars_configuration=None):  # noqa: E501
-        """InlineObject - a model defined in OpenAPI"""  # noqa: E501
+        """InlineObject1 - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._playback_file = None
         self.discriminator = None
 
         self.playback_file = playback_file
 
     @property
     def playback_file(self):
-        """Gets the playback_file of this InlineObject.  # noqa: E501
+        """Gets the playback_file of this InlineObject1.  # noqa: E501
 
 
-        :return: The playback_file of this InlineObject.  # noqa: E501
+        :return: The playback_file of this InlineObject1.  # noqa: E501
         :rtype: file
         """
         return self._playback_file
 
     @playback_file.setter
     def playback_file(self, playback_file):
-        """Sets the playback_file of this InlineObject.
+        """Sets the playback_file of this InlineObject1.
 
 
-        :param playback_file: The playback_file of this InlineObject.  # noqa: E501
+        :param playback_file: The playback_file of this InlineObject1.  # noqa: E501
         :type: file
         """
         if self.local_vars_configuration.client_side_validation and playback_file is None:  # noqa: E501
             raise ValueError("Invalid value for `playback_file`, must not be `None`")  # noqa: E501
 
         self._playback_file = playback_file
 
@@ -105,18 +105,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineObject):
+        if not isinstance(other, InlineObject1):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineObject):
+        if not isinstance(other, InlineObject1):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/inline_response200.py` & `icotest-voice-1.0.33/icotest_voice/models/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/inline_response200_files.py` & `icotest-voice-1.0.33/icotest_voice/models/inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/message.py` & `icotest-voice-1.0.33/icotest_voice/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/models/request.py` & `icotest-voice-1.0.33/icotest_voice/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.32/icotest_voice/rest.py` & `icotest-voice-1.0.33/icotest_voice/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/icotest_voice.egg-info/PKG-INFO` & `icotest-voice-1.0.33/icotest_voice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.32
+Version: 1.0.33
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.32
-- Package version: 1.0.32
+- API version: 1.0.33
+- Package version: 1.0.33
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -69,16 +69,15 @@
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
     controller_id = 'ac331ccb-5841-44ec-9d32-4f4fe0c3c16c'  # str: the unique id of the controller
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
-        print("Exception when calling ControllersApi.delete_controller(): %s\n" % e)
-    
+        print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://localhost/icotest_voice*
 
 Class | Method | HTTP request | Description
@@ -119,14 +118,15 @@
 
 ## Documentation For Models
 
  - [Controller](docs/Controller.md)
  - [Device](docs/Device.md)
  - [HostConfig](docs/HostConfig.md)
  - [InlineObject](docs/InlineObject.md)
+ - [InlineObject1](docs/InlineObject1.md)
  - [InlineResponse200](docs/InlineResponse200.md)
  - [InlineResponse200Files](docs/InlineResponse200Files.md)
  - [Message](docs/Message.md)
  - [Request](docs/Request.md)
 
 
 ## Documentation For Authorization
```

### Comparing `icotest-voice-1.0.32/icotest_voice.egg-info/SOURCES.txt` & `icotest-voice-1.0.33/icotest_voice.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 docs/Controller.md
 docs/ControllersApi.md
 docs/Device.md
 docs/DevicesApi.md
 docs/HostConfig.md
 docs/InlineObject.md
+docs/InlineObject1.md
 docs/InlineResponse200.md
 docs/InlineResponse200Files.md
 docs/Message.md
 docs/Request.md
 docs/RequestsApi.md
 icotest_voice/__init__.py
 icotest_voice/api_client.py
@@ -28,22 +29,24 @@
 icotest_voice/api/devices_api.py
 icotest_voice/api/requests_api.py
 icotest_voice/models/__init__.py
 icotest_voice/models/controller.py
 icotest_voice/models/device.py
 icotest_voice/models/host_config.py
 icotest_voice/models/inline_object.py
+icotest_voice/models/inline_object1.py
 icotest_voice/models/inline_response200.py
 icotest_voice/models/inline_response200_files.py
 icotest_voice/models/message.py
 icotest_voice/models/request.py
 test/test_controller.py
 test/test_controllers_api.py
 test/test_device.py
 test/test_devices_api.py
 test/test_host_config.py
 test/test_inline_object.py
+test/test_inline_object1.py
 test/test_inline_response200.py
 test/test_inline_response200_files.py
 test/test_message.py
 test/test_request.py
 test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.32/pyproject.toml` & `icotest-voice-1.0.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.32"
+version = "1.0.33"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email =  "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" }
 ]
```

### Comparing `icotest-voice-1.0.32/test/test_controller.py` & `icotest-voice-1.0.33/test/test_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -34,14 +34,15 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = icotest_voice.models.controller.Controller()  # noqa: E501
         if include_optional :
             return Controller(
                 controller_id = '10cda64a-0dce-4663-8b47-6ec1867f9568', 
+                controller_type = 'dect', 
                 description = 'example controller', 
                 location = 'server 1 rack 1', 
                 callback_url = 'https://server:port', 
                 created = '2021-06-24T14:15:22Z', 
                 last_contact = '2021-06-24T14:15:22Z'
             )
         else :
```

### Comparing `icotest-voice-1.0.32/test/test_controllers_api.py` & `icotest-voice-1.0.33/test/test_controllers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_device.py` & `icotest-voice-1.0.33/test/test_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_devices_api.py` & `icotest-voice-1.0.33/test/test_devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_host_config.py` & `icotest-voice-1.0.33/test/test_host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_inline_object.py` & `icotest-voice-1.0.33/test/test_inline_object1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import icotest_voice
-from icotest_voice.models.inline_object import InlineObject  # noqa: E501
+from icotest_voice.models.inline_object1 import InlineObject1  # noqa: E501
 from icotest_voice.rest import ApiException
 
-class TestInlineObject(unittest.TestCase):
-    """InlineObject unit test stubs"""
+class TestInlineObject1(unittest.TestCase):
+    """InlineObject1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test InlineObject
+        """Test InlineObject1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = icotest_voice.models.inline_object.InlineObject()  # noqa: E501
+        # model = icotest_voice.models.inline_object1.InlineObject1()  # noqa: E501
         if include_optional :
-            return InlineObject(
+            return InlineObject1(
                 playback_file = bytes(b'blah')
             )
         else :
-            return InlineObject(
+            return InlineObject1(
                 playback_file = bytes(b'blah'),
         )
 
-    def testInlineObject(self):
-        """Test InlineObject"""
+    def testInlineObject1(self):
+        """Test InlineObject1"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `icotest-voice-1.0.32/test/test_inline_response200.py` & `icotest-voice-1.0.33/test/test_inline_response200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_inline_response200_files.py` & `icotest-voice-1.0.33/test/test_inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_message.py` & `icotest-voice-1.0.33/test/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_request.py` & `icotest-voice-1.0.33/test/test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.32/test/test_requests_api.py` & `icotest-voice-1.0.33/test/test_requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.32
+    The version of the OpenAPI document: 1.0.33
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

