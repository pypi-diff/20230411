# Comparing `tmp/roboweb_server-0.1.36.tar.gz` & `tmp/roboweb_server-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboweb_server-0.1.36.tar", last modified: Tue Apr 11 07:51:00 2023, max compression
+gzip compressed data, was "roboweb_server-0.1.37.tar", last modified: Tue Apr 11 07:59:30 2023, max compression
```

## Comparing `roboweb_server-0.1.36.tar` & `roboweb_server-0.1.37.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.423483 roboweb_server-0.1.36/
--rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-11 07:51:00.423302 roboweb_server-0.1.36/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.403941 roboweb_server-0.1.36/roboweb_server/
--rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/ext.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.408492 roboweb_server-0.1.36/roboweb_server/static/
--rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/.last_build_id
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.409037 roboweb_server-0.1.36/roboweb_server/static/assets/
--rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/assets/AssetManifest.bin
--rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/assets/AssetManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/assets/FontManifest.json
--rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/assets/NOTICES
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.410236 roboweb_server-0.1.36/roboweb_server/static/assets/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.410677 roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/
--rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/firebase.webp
--rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/gcloud.png
--rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/github.png
--rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/assets/assets/jupyter.jpg
--rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/assets/assets/oauth2redirect.html
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.410808 roboweb_server-0.1.36/roboweb_server/static/assets/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)     9392 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.402191 roboweb_server-0.1.36/roboweb_server/static/assets/packages/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.401892 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.401946 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.411225 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.411647 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.412070 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
--rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
--rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
--rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
--rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.402251 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.402310 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.412626 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
--rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
--rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.412931 roboweb_server-0.1.36/roboweb_server/static/assets/shaders/
--rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/assets/shaders/ink_sparkle.frag
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.420007 roboweb_server-0.1.36/roboweb_server/static/canvaskit/
--rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-10 00:21:14.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  6756915 2023-04-10 00:21:10.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/canvaskit.wasm
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.420345 roboweb_server-0.1.36/roboweb_server/static/canvaskit/chromium/
--rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-10 00:21:12.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/chromium/canvaskit.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  5357911 2023-04-10 00:21:08.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
--rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-10 00:22:12.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.js
--rwxr-xr-x   0 hamel      (501) staff       (20)  4447359 2023-04-10 00:22:08.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.wasm
--rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-10 00:22:12.000000 roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.worker.js
--rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/roboweb_server/static/favicon.ico
--rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/flutter.js
--rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/flutter_service_worker.js
--rw-r--r--   0 hamel      (501) staff       (20)     3292 2023-04-11 07:50:59.000000 roboweb_server-0.1.36/roboweb_server/static/index.html
--rw-r--r--   0 hamel      (501) staff       (20)  3921210 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server/static/main.dart.js
--rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-11 07:50:58.000000 roboweb_server-0.1.36/roboweb_server/static/version.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:51:00.405468 roboweb_server-0.1.36/roboweb_server.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:23:46.000000 roboweb_server-0.1.36/roboweb_server.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/roboweb_server.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-11 07:51:00.000000 roboweb_server-0.1.36/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-11 07:51:00.423524 roboweb_server-0.1.36/setup.cfg
--rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 22:21:06.000000 roboweb_server-0.1.36/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.704057 roboweb_server-0.1.37/
+-rw-r--r--   0 hamel      (501) staff       (20)      115 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-11 07:59:30.703849 roboweb_server-0.1.37/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      322 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.683063 roboweb_server-0.1.37/roboweb_server/
+-rw-r--r--   0 hamel      (501) staff       (20)       49 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1031 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/ext.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.687883 roboweb_server-0.1.37/roboweb_server/static/
+-rw-r--r--   0 hamel      (501) staff       (20)       32 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server/static/.last_build_id
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.688597 roboweb_server-0.1.37/roboweb_server/static/assets/
+-rw-r--r--   0 hamel      (501) staff       (20)     1487 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/assets/AssetManifest.bin
+-rw-r--r--   0 hamel      (501) staff       (20)     2245 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/assets/AssetManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)      544 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/assets/FontManifest.json
+-rw-r--r--   0 hamel      (501) staff       (20)  1793816 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/assets/NOTICES
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.690009 roboweb_server-0.1.37/roboweb_server/static/assets/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.690492 roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/
+-rw-r--r--   0 hamel      (501) staff       (20)     4722 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/firebase.webp
+-rw-r--r--   0 hamel      (501) staff       (20)    16313 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/gcloud.png
+-rw-r--r--   0 hamel      (501) staff       (20)     7966 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/github.png
+-rw-r--r--   0 hamel      (501) staff       (20)    21222 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/assets/assets/jupyter.jpg
+-rw-r--r--   0 hamel      (501) staff       (20)     1600 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/assets/assets/oauth2redirect.html
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.690642 roboweb_server-0.1.37/roboweb_server/static/assets/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)     9392 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.681460 roboweb_server-0.1.37/roboweb_server/static/assets/packages/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.681170 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.681223 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.691277 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.691764 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     1387 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1696 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     1515 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.692264 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/
+-rw-r--r--   0 hamel      (501) staff       (20)     2059 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2503 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)     2224 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png
+-rw-r--r--   0 hamel      (501) staff       (20)      745 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png
+-rw-r--r--   0 hamel      (501) staff       (20)      888 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png
+-rw-r--r--   0 hamel      (501) staff       (20)      807 2023-04-05 04:39:17.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.681515 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.681569 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.692895 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/
+-rw-r--r--   0 hamel      (501) staff       (20)   169440 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)    48796 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf
+-rw-r--r--   0 hamel      (501) staff       (20)   357436 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.693268 roboweb_server-0.1.37/roboweb_server/static/assets/shaders/
+-rw-r--r--   0 hamel      (501) staff       (20)     9242 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/assets/shaders/ink_sparkle.frag
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.700243 roboweb_server-0.1.37/roboweb_server/static/canvaskit/
+-rw-r--r--   0 hamel      (501) staff       (20)    95983 2023-04-10 00:21:14.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  6756915 2023-04-10 00:21:10.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/canvaskit.wasm
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.700672 roboweb_server-0.1.37/roboweb_server/static/canvaskit/chromium/
+-rw-r--r--   0 hamel      (501) staff       (20)    95628 2023-04-10 00:21:12.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/chromium/canvaskit.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  5357911 2023-04-10 00:21:08.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/chromium/canvaskit.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)    60828 2023-04-10 00:22:12.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.js
+-rwxr-xr-x   0 hamel      (501) staff       (20)  4447359 2023-04-10 00:22:08.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.wasm
+-rw-r--r--   0 hamel      (501) staff       (20)     2744 2023-04-10 00:22:12.000000 roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)    15406 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/roboweb_server/static/favicon.ico
+-rw-r--r--   0 hamel      (501) staff       (20)    14233 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server/static/flutter.js
+-rw-r--r--   0 hamel      (501) staff       (20)     9022 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/flutter_service_worker.js
+-rw-r--r--   0 hamel      (501) staff       (20)     3292 2023-04-11 07:59:29.000000 roboweb_server-0.1.37/roboweb_server/static/index.html
+-rw-r--r--   0 hamel      (501) staff       (20)  3921205 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server/static/main.dart.js
+-rw-r--r--   0 hamel      (501) staff       (20)       84 2023-04-11 07:59:28.000000 roboweb_server-0.1.37/roboweb_server/static/version.json
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-11 07:59:30.684578 roboweb_server-0.1.37/roboweb_server.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1067 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2565 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 22:23:46.000000 roboweb_server-0.1.37/roboweb_server.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/roboweb_server.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      430 2023-04-11 07:59:30.000000 roboweb_server-0.1.37/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-11 07:59:30.704101 roboweb_server-0.1.37/setup.cfg
+-rw-r--r--   0 hamel      (501) staff       (20)     2803 2023-04-09 22:21:06.000000 roboweb_server-0.1.37/setup.py
```

### Comparing `roboweb_server-0.1.36/PKG-INFO` & `roboweb_server-0.1.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb_server
-Version: 0.1.36
+Version: 0.1.37
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.36/roboweb_server/ext.py` & `roboweb_server-0.1.37/roboweb_server/ext.py`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/AssetManifest.bin` & `roboweb_server-0.1.37/roboweb_server/static/assets/AssetManifest.bin`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/AssetManifest.json` & `roboweb_server-0.1.37/roboweb_server/static/assets/AssetManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/FontManifest.json` & `roboweb_server-0.1.37/roboweb_server/static/assets/FontManifest.json`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/NOTICES` & `roboweb_server-0.1.37/roboweb_server/static/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/firebase.webp` & `roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/firebase.webp`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/gcloud.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/gcloud.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/assets/apps/github.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/assets/apps/github.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/assets/jupyter.jpg` & `roboweb_server-0.1.37/roboweb_server/static/assets/assets/jupyter.jpg`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/assets/oauth2redirect.html` & `roboweb_server-0.1.37/roboweb_server/static/assets/assets/oauth2redirect.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf` & `roboweb_server-0.1.37/roboweb_server/static/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/2.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/3.0x/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/facebook_new.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_dark.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/flutter_signin_button/assets/logos/google_light.png`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf` & `roboweb_server-0.1.37/roboweb_server/static/assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/assets/shaders/ink_sparkle.frag` & `roboweb_server-0.1.37/roboweb_server/static/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/canvaskit.js` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/canvaskit.wasm` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/chromium/canvaskit.js` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/chromium/canvaskit.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/chromium/canvaskit.wasm` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/chromium/canvaskit.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.js` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.wasm` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.wasm`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/canvaskit/skwasm.worker.js` & `roboweb_server-0.1.37/roboweb_server/static/canvaskit/skwasm.worker.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/favicon.ico` & `roboweb_server-0.1.37/roboweb_server/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/flutter.js` & `roboweb_server-0.1.37/roboweb_server/static/flutter.js`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/flutter_service_worker.js` & `roboweb_server-0.1.37/roboweb_server/static/flutter_service_worker.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
 const CACHE_NAME = 'flutter-app-cache';
 
 const RESOURCES = {
     "version.json": "558d4558c36159f1d7c7fa8b43dce5ab",
     "favicon.ico": "ae3f664c1893363bef172d7fe3913cf5",
     "index.html": "0404a71390237214f7e03caff13fc334",
     "/": "0404a71390237214f7e03caff13fc334",
-    "main.dart.js": "e644f06c19ba1e345ed56850a0ccd3a9",
+    "main.dart.js": "6bbb009274f3f6081faeb91b6f17bad0",
     "flutter.js": "6fef97aeca90b426343ba6c5c9dc5d4a",
     "assets/AssetManifest.json": "e2b510a90489a717ddddbc5c9d3ca7b8",
     "assets/NOTICES": "f5673ea70f78ee6578c580299fc5e3eb",
     "assets/FontManifest.json": "3ddd9b2ab1c2ae162d46e3cc7b78ba88",
     "assets/packages/font_awesome_flutter/lib/fonts/fa-solid-900.ttf": "efc6c90b58d765987f922c95c2031dd2",
     "assets/packages/font_awesome_flutter/lib/fonts/fa-regular-400.ttf": "01bb14ae3f14c73ee03eed84f480ded9",
     "assets/packages/font_awesome_flutter/lib/fonts/fa-brands-400.ttf": "0db203e8632f03baae0184700f3bda48",
```

### Comparing `roboweb_server-0.1.36/roboweb_server/static/index.html` & `roboweb_server-0.1.37/roboweb_server/static/index.html`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/roboweb_server/static/main.dart.js` & `roboweb_server-0.1.37/roboweb_server/static/main.dart.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -172018,15 +172018,15 @@
         s($, "b7V", "aNb", () => new A.Qn(A.aG("/", !0, !1, !1), A.aG("[^/]$", !0, !1, !1), A.aG("^/", !0, !1, !1)))
         s($, "b7X", "a24", () => new A.TA(A.aG("[/\\\\]", !0, !1, !1), A.aG("[^/\\\\]$", !0, !1, !1), A.aG("^(\\\\\\\\[^\\\\]+\\\\[^\\\\/]+|[a-zA-Z]:[/\\\\])", !0, !1, !1), A.aG("^[/\\\\](?![/\\\\])", !0, !1, !1)))
         s($, "b7W", "Jz", () => new A.Tl(A.aG("/", !0, !1, !1), A.aG("(^[a-zA-Z][-+.a-zA-Z\\d]*://|[^/])$", !0, !1, !1), A.aG("[a-zA-Z][-+.a-zA-Z\\d]*://[^/]*", !0, !1, !1), A.aG("^/", !0, !1, !1)))
         s($, "b7U", "aDJ", () => A.aZo())
         s($, "b7k", "co", () => A.il())
         s($, "b9z", "aOa", () => !t.Cm.b(A.b([], t.Z)))
         s($, "b8B", "aND", () => A.aWj(null, A.a9("ux")))
-        s($, "b5x", "az5", () => A.kG("https://roboweb.app/docs/faq/", 0, null))
+        s($, "b5x", "az5", () => A.kG("https://roboweb.app/faq/", 0, null))
         s($, "b7M", "aDI", () => new A.G())
         r($, "aZ_", "aDH", () => {
             var q = new A.aew()
             q.xo($.aDI())
             return q
         })
         s($, "b8f", "aDM", () => new A.G())
```

### Comparing `roboweb_server-0.1.36/roboweb_server.egg-info/PKG-INFO` & `roboweb_server-0.1.37/roboweb_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboweb-server
-Version: 0.1.36
+Version: 0.1.37
 Summary: ChatGPT plugin for Jupyter Server
 Home-page: https://github.com/jlewi/roboweb
 Author: Jeremy Lewi
 Author-email: jeremy@lewi.us
 License: Apache Software License 2.0
 Keywords: gpt jupyter-server llm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `roboweb_server-0.1.36/roboweb_server.egg-info/SOURCES.txt` & `roboweb_server-0.1.37/roboweb_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboweb_server-0.1.36/setup.py` & `roboweb_server-0.1.37/setup.py`

 * *Files identical despite different names*

