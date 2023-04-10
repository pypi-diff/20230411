# Comparing `tmp/flet-0.6.0.dev1296.tar.gz` & `tmp/flet-0.6.0.dev1298.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.6.0.dev1296.tar", max compression
+gzip compressed data, was "flet-0.6.0.dev1298.tar", max compression
```

## Comparing `flet-0.6.0.dev1296.tar` & `flet-0.6.0.dev1298.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     2145 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/README.md
--rw-r--r--   0        0        0     1066 2023-04-09 16:17:59.651249 flet-0.6.0.dev1296/pyproject.toml
--rw-r--r--   0        0        0      155 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3636 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     6192 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/async_local_socket_connection.py
--rw-r--r--   0        0        0     7183 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0     8919 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/group.py
--rw-r--r--   0        0        0     1499 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/oauth_token.py
--rw-r--r--   0        0        0      735 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      840 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3669 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      799 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      182 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/auth/user.py
--rw-r--r--   0        0        0     2958 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0      673 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8449 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     8885 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     6711 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/constants.py
--rw-r--r--   0        0        0    21493 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/plotly_chart.py
--rw-r--r--   0        0        0    10075 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/pubsub.py
--rw-r--r--   0        0        0     3046 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/security.py
--rw-r--r--   0        0        0     6843 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/sync_local_socket_connection.py
--rw-r--r--   0        0        0     5396 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0     6955 2023-04-09 16:17:25.970300 flet-0.6.0.dev1296/src/flet/utils.py
--rw-r--r--   0        0        0     1431 2023-04-09 16:17:59.419243 flet-0.6.0.dev1296/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-04-09 16:09:40.000000 flet-0.6.0.dev1296/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      455 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0   916508 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1645184 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     1028 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/favicon.png
--rw-r--r--   0        0        0    13910 2023-04-09 16:08:36.000000 flet-0.6.0.dev1296/src/flet/web/flutter.js
--rw-r--r--   0        0        0     7836 2023-04-09 16:09:40.000000 flet-0.6.0.dev1296/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     2971 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/index.html
--rw-r--r--   0        0        0  5302180 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-04-09 16:09:39.000000 flet-0.6.0.dev1296/src/flet/web/version.json
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1296/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/README.md
+-rw-r--r--   0        0        0     1066 2023-04-10 22:24:51.837691 flet-0.6.0.dev1298/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3636 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     6192 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/async_local_socket_connection.py
+-rw-r--r--   0        0        0     7183 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0     9083 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/group.py
+-rw-r--r--   0        0        0     1499 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/oauth_token.py
+-rw-r--r--   0        0        0      735 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      840 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3669 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      799 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      182 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/auth/user.py
+-rw-r--r--   0        0        0     2958 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0      673 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8449 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     8885 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     6711 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/constants.py
+-rw-r--r--   0        0        0    21493 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0    10239 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/pubsub.py
+-rw-r--r--   0        0        0     3046 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/security.py
+-rw-r--r--   0        0        0     6843 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     5396 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0     6955 2023-04-10 22:24:16.129252 flet-0.6.0.dev1298/src/flet/utils.py
+-rw-r--r--   0        0        0     1431 2023-04-10 22:24:51.617688 flet-0.6.0.dev1298/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-04-10 22:15:19.000000 flet-0.6.0.dev1298/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      455 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0   916508 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1645184 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     1028 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    13910 2023-04-10 22:14:05.000000 flet-0.6.0.dev1298/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     7836 2023-04-10 22:15:19.000000 flet-0.6.0.dev1298/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     2972 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/index.html
+-rw-r--r--   0        0        0  5302180 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-04-10 22:15:18.000000 flet-0.6.0.dev1298/src/flet/web/version.json
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.6.0.dev1298/PKG-INFO
```

### Comparing `flet-0.6.0.dev1296/README.md` & `flet-0.6.0.dev1298/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/pyproject.toml` & `flet-0.6.0.dev1298/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.6.0.dev1296"
+version = "0.6.0.dev1298"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.6.0.dev1296"
+flet-core = "0.6.0.dev1298"
 python = "^3.7"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 websocket-client = "^1.4.2"
 watchdog = "^2.2.1"
 oauthlib = "^3.2.2"
 websockets = "^10.4"
 httpx = "^0.23.3"
```

### Comparing `flet-0.6.0.dev1296/src/flet/__pyinstaller/macos_utils.py` & `flet-0.6.0.dev1298/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/__pyinstaller/utils.py` & `flet-0.6.0.dev1298/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/__pyinstaller/win_utils.py` & `flet-0.6.0.dev1298/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/async_local_socket_connection.py` & `flet-0.6.0.dev1298/src/flet/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/async_websocket_connection.py` & `flet-0.6.0.dev1298/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/authorization.py` & `flet-0.6.0.dev1298/src/flet/auth/authorization.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from typing import List, Optional, Tuple
 
 import httpx
 from flet.auth.oauth_provider import OAuthProvider
 from flet.auth.oauth_token import OAuthToken
 from flet.auth.user import User
 from flet.version import version
+from flet_core.locks import AsyncNopeLock, NopeLock
+from flet_core.utils import is_asyncio
 from oauthlib.oauth2 import WebApplicationClient
 from oauthlib.oauth2.rfc6749.tokens import OAuth2Token
 
 
 class Authorization:
     def __init__(
         self,
@@ -24,16 +26,16 @@
     ) -> None:
         self.fetch_user = fetch_user
         self.fetch_groups = fetch_groups
         self.scope = scope if scope is not None else []
         self.provider = provider
         self.__token: Optional[OAuthToken] = None
         self.user: Optional[User] = None
-        self.__lock = threading.Lock()
-        self.__async_lock = asyncio.Lock()
+        self.__lock = threading.Lock() if not is_asyncio() else NopeLock()
+        self.__async_lock = asyncio.Lock() if is_asyncio() else AsyncNopeLock()
 
         # fix scopes
         self.scope.extend(self.provider.scopes)
         if self.fetch_user:
             for s in self.provider.user_scopes:
                 if s not in self.scope:
                     self.scope.append(s)
```

### Comparing `flet-0.6.0.dev1296/src/flet/auth/oauth_provider.py` & `flet-0.6.0.dev1298/src/flet/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/oauth_token.py` & `flet-0.6.0.dev1298/src/flet/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/providers/auth0_oauth_provider.py` & `flet-0.6.0.dev1298/src/flet/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/providers/azure_oauth_provider.py` & `flet-0.6.0.dev1298/src/flet/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/providers/github_oauth_provider.py` & `flet-0.6.0.dev1298/src/flet/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/auth/providers/google_oauth_provider.py` & `flet-0.6.0.dev1298/src/flet/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/cli.py` & `flet-0.6.0.dev1298/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/commands/base.py` & `flet-0.6.0.dev1298/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/commands/options.py` & `flet-0.6.0.dev1298/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/commands/pack.py` & `flet-0.6.0.dev1298/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/commands/publish.py` & `flet-0.6.0.dev1298/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/cli/commands/run.py` & `flet-0.6.0.dev1298/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/flet.py` & `flet-0.6.0.dev1298/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/pubsub.py` & `flet-0.6.0.dev1298/src/flet/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 import logging
 import threading
 from typing import Any, Callable, Dict, Iterable
 
 import flet
+from flet_core.locks import AsyncNopeLock, NopeLock
+from flet_core.utils import is_asyncio
 
 logger = logging.getLogger(flet.__name__)
 
 
 class PubSubHub:
     def __init__(self):
-        self.__lock = threading.Lock()
-        self.__async_lock = asyncio.Lock()
+        self.__lock = threading.Lock() if not is_asyncio() else NopeLock()
+        self.__async_lock = asyncio.Lock() if is_asyncio() else AsyncNopeLock()
         self.__subscribers: Dict[str, Callable] = {}  # key: session_id, value: handler
         self.__topic_subscribers: Dict[
             str, Dict[str, Callable]
         ] = {}  # key: topic, value: dict[session_id, handler]
         self.__subscriber_topics: Dict[
             str, Dict[str, Callable]
         ] = {}  # key: session_id, value: dict[topic, handler]
```

### Comparing `flet-0.6.0.dev1296/src/flet/reconnecting_websocket.py` & `flet-0.6.0.dev1298/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/security.py` & `flet-0.6.0.dev1298/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/sync_local_socket_connection.py` & `flet-0.6.0.dev1298/src/flet/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/sync_websocket_connection.py` & `flet-0.6.0.dev1298/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/utils.py` & `flet-0.6.0.dev1298/src/flet/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/version.py` & `flet-0.6.0.dev1298/src/flet/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess as sp
 from pathlib import Path
 
 import flet
 from flet.utils import is_windows, which
 
 # this value will be replaced by CI
-version = "0.6.0.dev1296"
+version = "0.6.0.dev1298"
 
 
 def update_version():
     """Return the current version or default."""
     working = Path().absolute()
     os.chdir(Path(flet.__file__).absolute().parent)
     in_repo = which("git.exe" if is_windows() else "git") and sp.run(
```

### Comparing `flet-0.6.0.dev1296/src/flet/web/assets/NOTICES` & `flet-0.6.0.dev1298/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.6.0.dev1298/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/favicon.png` & `flet-0.6.0.dev1298/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/flutter.js` & `flet-0.6.0.dev1298/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/flutter_service_worker.js` & `flet-0.6.0.dev1298/src/flet/web/flutter_service_worker.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,16 +24,16 @@
     "icons/icon-512.png": "06b219f171b5a1af6dd8299ea1e116f2",
     "python.js": "9eee2c1773af78bc45ee89ca2ac5724f",
     "canvaskit/canvaskit.wasm": "3de12d898ec208a5f31362cc00f09b9e",
     "canvaskit/canvaskit.js": "97937cb4c2c2073c968525a3e08c86a3",
     "canvaskit/profiling/canvaskit.wasm": "371bc4e204443b0d5e774d64a046eb99",
     "canvaskit/profiling/canvaskit.js": "c21852696bc1cc82e8894d851c01921a",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "16056ddf28a864d6f0f63fccb58c1e93",
-    "/": "16056ddf28a864d6f0f63fccb58c1e93"
+    "index.html": "649f9e2132180f260cecebc5af0bd3dd",
+    "/": "649f9e2132180f260cecebc5af0bd3dd"
 };
 
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = [
     "main.dart.js",
     "index.html",
```

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.6.0.dev1298/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/icon-192.png` & `flet-0.6.0.dev1298/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/icon-512.png` & `flet-0.6.0.dev1298/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/icon-maskable-192.png` & `flet-0.6.0.dev1298/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/icon-maskable-512.png` & `flet-0.6.0.dev1298/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/icons/loading-animation.png` & `flet-0.6.0.dev1298/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/index.html` & `flet-0.6.0.dev1298/src/flet/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
   <!-- flutterWebRenderer -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = '227347627';
+    var serviceWorkerVersion = '1864934848';
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.6.0.dev1296/src/flet/web/main.dart.js` & `flet-0.6.0.dev1298/src/flet/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/manifest.json` & `flet-0.6.0.dev1298/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/python-worker.js` & `flet-0.6.0.dev1298/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/src/flet/web/python.js` & `flet-0.6.0.dev1298/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.6.0.dev1296/PKG-INFO` & `flet-0.6.0.dev1298/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.6.0.dev1296
+Version: 0.6.0.dev1298
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.6.0.dev1296)
+Requires-Dist: flet-core (==0.6.0.dev1298)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.2,<2.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
```

