# Comparing `tmp/selenium_profiles-2.2.5.5.tar.gz` & `tmp/selenium_profiles-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_profiles-2.2.5.5.tar", last modified: Fri Mar 24 23:05:36 2023, max compression
+gzip compressed data, was "dist\selenium_profiles-2.2.6.tar", last modified: Tue Apr 11 09:43:09 2023, max compression
```

## Comparing `selenium_profiles-2.2.5.5.tar` & `selenium_profiles-2.2.6.tar`

### file list

```diff
@@ -1,58 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.5.5/LICENSE.md
--rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12105 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    10757 2023-03-24 22:13:31.000000 selenium_profiles-2.2.5.5/README.md
--rw-rw-rw-   0        0        0     1695 2022-11-30 14:03:19.000000 selenium_profiles-2.2.5.5/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.5.5/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/setup.cfg
--rw-rw-rw-   0        0        0     2340 2023-03-16 14:43:39.000000 selenium_profiles-2.2.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/
--rw-rw-rw-   0        0        0      111 2023-03-24 23:03:35.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/__init__.py
--rw-rw-rw-   0        0        0     8245 2023-03-18 06:50:56.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/driver.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/__init__.py
--rw-rw-rw-   0        0        0     3134 2023-03-24 22:44:33.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/get_navigator.js
--rw-rw-rw-   0        0        0      241 2022-12-02 20:56:33.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/run_box.js
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/undetected/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/undetected/__init.py
--rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/
--rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/__init__.py
--rw-rw-rw-   0        0        0     3121 2023-03-24 22:34:30.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/default.json
--rw-rw-rw-   0        0        0     2030 2023-01-17 08:04:46.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/example.json
--rw-rw-rw-   0        0        0      864 2022-12-16 08:26:17.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/__init__.py
--rw-rw-rw-   0        0        0     4250 2023-03-24 22:20:02.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/cdp_tools.py
--rw-rw-rw-   0        0        0     3419 2023-01-27 09:47:18.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    17203 2023-03-24 22:37:47.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/profiles.py
--rw-rw-rw-   0        0        0     1651 2023-03-18 10:36:31.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/proxy_extension.py
--rw-rw-rw-   0        0        0     1334 2023-01-27 09:48:51.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/touch_actions.py
--rw-rw-rw-   0        0        0     1435 2023-03-18 06:51:53.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/utils/
--rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/utils/colab_utils.py
--rw-rw-rw-   0        0        0      256 2023-03-16 14:12:17.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/utils/installer.py
--rw-rw-rw-   0        0        0     1268 2023-03-16 15:34:17.000000 selenium_profiles-2.2.5.5/src/selenium_profiles/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/
--rw-rw-rw-   0        0        0    12105 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1676 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-24 23:05:36.000000 selenium_profiles-2.2.5.5/tests/
--rw-rw-rw-   0        0        0     1767 2023-03-24 22:39:14.000000 selenium_profiles-2.2.5.5/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12069 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10723 2023-04-11 09:29:31.000000 selenium_profiles-2.2.6/README.md
+-rw-rw-rw-   0        0        0     1695 2022-11-30 14:03:19.000000 selenium_profiles-2.2.6/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2057 2023-04-11 08:18:26.000000 selenium_profiles-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/
+-rw-rw-rw-   0        0        0       23 2023-04-11 09:30:30.000000 selenium_profiles-2.2.6/src/selenium_profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/proxy_extension/
+-rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/tmp/proxy_extension/
+-rw-rw-rw-   0        0        0      629 2023-04-10 02:54:47.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/tmp/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-04-10 02:54:47.000000 selenium_profiles-2.2.6/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/undetected/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/undetected/__init.py
+-rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.6/src/selenium_profiles/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/
+-rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__pycache__/
+-rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1418 2023-04-09 11:28:56.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/default.json
+-rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/example.json
+-rw-rw-rw-   0        0        0      864 2022-12-16 08:26:17.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.6/src/selenium_profiles/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4254 2023-04-10 14:47:07.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/cdp_tools.py
+-rw-rw-rw-   0        0        0    10673 2023-04-10 13:49:26.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24992 2023-04-10 20:40:19.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/profiles.py
+-rw-rw-rw-   0        0        0     1651 2023-03-18 10:36:31.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/proxy_extension.py
+-rw-rw-rw-   0        0        0     2001 2023-04-10 19:21:04.000000 selenium_profiles-2.2.6/src/selenium_profiles/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.6/src/selenium_profiles/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.6/src/selenium_profiles/utils/colab_utils.py
+-rw-rw-rw-   0        0        0      256 2023-03-16 14:12:17.000000 selenium_profiles-2.2.6/src/selenium_profiles/utils/installer.py
+-rw-rw-rw-   0        0        0     1558 2023-04-10 02:18:50.000000 selenium_profiles-2.2.6/src/selenium_profiles/utils/utils.py
+-rw-rw-rw-   0        0        0     8495 2023-04-11 09:39:23.000000 selenium_profiles-2.2.6/src/selenium_profiles/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/
+-rw-rw-rw-   0        0        0    12069 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1963 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/src/selenium_profiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:43:09.000000 selenium_profiles-2.2.6/tests/
+-rw-rw-rw-   0        0        0     1651 2023-04-11 09:42:08.000000 selenium_profiles-2.2.6/tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.5.5/LICENSE.md` & `selenium_profiles-2.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/PKG-INFO` & `selenium_profiles-2.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_profiles
-Version: 2.2.5.5
+Version: 2.2.6
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -26,22 +26,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Selenium-Profiles
 
+[![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
+
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
 * **Undetected** by Google, Cloudflare, creep-js ..
-* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor)
+* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
 * [Touch Actions](#Touch_actions)
 * [proxies with authentication](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4704385)
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.requests.fetch(url, options)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
+* apply profile on allready running driver with `driver.profiles.apply(profiles.Android())`
+* use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
 
 ### Feel free to test my code!
 
 ## Getting Started
 
@@ -54,73 +58,75 @@
 
 * Install [Google-Chrome](https://www.google.de/chrome/) (or another chromium-based browser)
 * ```pip install selenium-profiles```
 
 ### Start Driver
 
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By  # locate elements
+from selenium.webdriver import ChromeOptions
+
 
-mydriver = mydriver()
 profile = profiles.Windows()
-# profile["options"]["browser"]["headless"] = True
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+options = ChromeOptions()
+mydriver = Chrome(profile, options=options, uc_driver=False)
+# mydriver.options.add_argument("--headless=new")
+
+driver = mydriver.start()  # or .Android
 
 # get url
-driver.get('https://browserleaks.com/client-hints')  # test client hints
+driver.get('https://abrahamjuliot.github.io/creepjs/')  # test client hints
 
 input("Press ENTER to exit: ")
 driver.quit()  # Execute on the End!
 ```
 
 Don't forget to execute
 ```driver.quit()```
 in the End. Else-wise your temporary folder will get flooded!
 
 #### Run with Google-Colab
-[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: google-colab/selenium_profiles.ipynb)
+__[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: master@google-colab/selenium_profiles.ipynb)__
+
+[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/dev/google-colab/selenium_profiles.ipynb) (file: dev@google-colab/selenium_profiles.ipynb)
 
 ## Profiles
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
-    "browser": {
       "sandbox": True,
       "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
+      "touch": True,
       "app": False,
-      "touch": True, # 
       "gpu": False,
-      "proxy": "example-proxy.com:9000", # note: auth not supported
-      "proxy_method": "http://" # optional, default: "socks5://"
-    },
-      "extensions": {
-          "extension_paths": ["path/to/extension_1"], # directory, .crx or .zip
-          "auth_proxy": {"host":"host","port":9000,"username":"user", "password":"password", "temp_dir": "C:/Downloads/proxy_extension"}
-        },
-      "option_args": ["--my-arg1", "..."],
-      "capabilities": [],
-      "adb": False,
+      "proxy": "http://example-proxy.com:9000", # note: auth not supported,
+      "extension_paths": ["path/to/extension_1", ...], # directory, .crx or .zip
+      "auth_proxy": {
+            "host":"host", "port":9000,
+            "username":"user", "password":"password", 
+            "temp_dir": "C:/Downloads/proxy_extension"
+                },
+      "args": ["--my-arg1", ...],
+      "capabilities": {"cap_1":"val_1", "cap_2":"val_2"},
+      "experimental_options":{"option1":"value1", "option2":"value2"},
+      "adb": False, # run on harware device over ADB
       "adb_package": "com.android.chrome",
       "use_running_app": True
   },
   "cdp": {
-    "browser": {
-      "pointer_as_touch": False,
-      "darkmode": False,
-      "mobile": True
-    },
     "touch": True,
+    "darkmode":None,
     "maxtouchpoints": 5,
     "cores":8,
     "cdp_args": [],
     "emulation": {"mobile":True,"width": 384, "height": 700, "deviceScaleFactor": 10,
         "screenOrientation": {"type": "portrait-primary", "angle": 0}},
     "patch_version": True, # to patch automatically, or use "111.0.5563.111"
     "useragent": {
@@ -143,69 +149,72 @@
                     "wow64": False}
     }
   }
 }
 ```
 
 ### Modify-headers
-```python
 
-from selenium_interceptor.interceptor import cdp_listener
-
-from selenium_profiles import driver as mydriver
+using selenium-wire
+```python
+from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
 
-mydriver = mydriver()
-profile = profiles.Windows()
+profile = profiles.Android()
 
-driver = mydriver.start(profile)
+mydriver = webdriver.Chrome(profile, uc_driver=False, seleniumwire_options=True) # or pass seleniumwire-options
+driver = mydriver.start()
 
-cdp_listener = cdp_listener(driver=driver)
-cdp_listener.specify_headers({"sec-ch-ua-platform":"Android"})
-thread = cdp_listener.start_threaded(listener={"listener": cdp_listener.requests, "at_event": cdp_listener.modify_headers})
+def interceptor(request):
+    request.headers['New-Header'] = 'Some Value'
+driver.request_interceptor = interceptor
 
-driver.get("https://modheader.com/headers?product=ModHeader")
+# checkout headers
+driver.get("https://httpbin.org/headers")
+
+input("Press ENTER to quit..")
+driver.quit()
+exit()
 ```
-Don't forget to execute
-`cdp_listener.terminate_all()`
 
 ### Touch_actions
 
 Example demonstration script
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome, ChromeOptions
 from selenium_profiles.profiles import profiles
-
-from selenium_profiles.scripts.driver_utils import actions
-
 from selenium.webdriver.common.by import By
 
+from selenium_profiles.scripts.driver_utils import TouchActionChain
+
 
 # Start Driver
-mydriver = mydriver()
+options = ChromeOptions()
 profile = profiles.Android()
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+mydriver = Chrome(profile, uc_driver=False, options=ChromeOptions)
+driver = mydriver.start()  # or .Android
 
 # initialise touch_actions
-actions = actions(driver)
+chain = TouchActionChain(driver)
 
 driver.get("https://cps-check.com/de/multi-touch-test")
 
 touch_box = driver.find_element(By.XPATH,'//*[@id="box"]') # Get element
-location = actions.mid_location(touch_box) # get element middle location
 
-# setup actions
-action = actions.touch_action_chain()
-action.pointer_action.move_to_location(location['x'],location['y'])
-action.pointer_action.pointer_down()
+
+
+chain.touch_and_hold(touch_box)
+chain.pause(10)
+chain.release(touch_box)
 
 # perform actions
-action.perform()
+chain.perform()
 
-# now you should see a touch indication point on the Website
+# now you should see a touch indication
+# point on the Website for 10 seconds
 
 # quit driver
 input('Press ENTER to quit Driver\n')
 driver.quit()
 ```
 
 ### To export a profile:
@@ -218,29 +227,22 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] installer.py script
-  - [ ] bump to [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-  - [ ] [Chrome-Browser](https://www.google.de/chrome/) (silent install)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
-  - [ ] does not match worker scope (Emulation)
+  - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
-  - [x] with wrong version (is:111, emulate:107) fixed with "patch_version"
-      - v107 failed CSS features by 2 versions
-      - v107 failed v109 Window features
-      - v107 failed v109 CSS features
-- [x] Mobile emulation
-  - [ ] click_as touch makes code hung
+    - `navigator.hardwareConcurrency`
+- [ ] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -251,27 +253,24 @@
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
 - [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [ ] support for 
+- [X] support for 
   - [x] Windows
   - [x] Jupyter Notebook (Google-Colab)
   - [x] Linux
-- [ ] add error handling for [invalid keys](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4699462) in profile
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
-* [Selenium-Wire](https://github.com/wkeeling/selenium-wire) (proxy, no https)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
-* [Modheader-Selenium](https://github.com/modheader/modheader_selenium) (Changing headers now possible without)
 
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_profiles-2.2.5.5/README.md` & `selenium_profiles-2.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Selenium-Profiles
 
+[![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
+
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
 * **Undetected** by Google, Cloudflare, creep-js ..
-* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor)
+* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
 * [Touch Actions](#Touch_actions)
 * [proxies with authentication](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4704385)
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.requests.fetch(url, options)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
+* apply profile on allready running driver with `driver.profiles.apply(profiles.Android())`
+* use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
 
 ### Feel free to test my code!
 
 ## Getting Started
 
@@ -24,73 +28,75 @@
 
 * Install [Google-Chrome](https://www.google.de/chrome/) (or another chromium-based browser)
 * ```pip install selenium-profiles```
 
 ### Start Driver
 
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By  # locate elements
+from selenium.webdriver import ChromeOptions
+
 
-mydriver = mydriver()
 profile = profiles.Windows()
-# profile["options"]["browser"]["headless"] = True
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+options = ChromeOptions()
+mydriver = Chrome(profile, options=options, uc_driver=False)
+# mydriver.options.add_argument("--headless=new")
+
+driver = mydriver.start()  # or .Android
 
 # get url
-driver.get('https://browserleaks.com/client-hints')  # test client hints
+driver.get('https://abrahamjuliot.github.io/creepjs/')  # test client hints
 
 input("Press ENTER to exit: ")
 driver.quit()  # Execute on the End!
 ```
 
 Don't forget to execute
 ```driver.quit()```
 in the End. Else-wise your temporary folder will get flooded!
 
 #### Run with Google-Colab
-[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: google-colab/selenium_profiles.ipynb)
+__[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: master@google-colab/selenium_profiles.ipynb)__
+
+[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/dev/google-colab/selenium_profiles.ipynb) (file: dev@google-colab/selenium_profiles.ipynb)
 
 ## Profiles
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
-    "browser": {
       "sandbox": True,
       "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
+      "touch": True,
       "app": False,
-      "touch": True, # 
       "gpu": False,
-      "proxy": "example-proxy.com:9000", # note: auth not supported
-      "proxy_method": "http://" # optional, default: "socks5://"
-    },
-      "extensions": {
-          "extension_paths": ["path/to/extension_1"], # directory, .crx or .zip
-          "auth_proxy": {"host":"host","port":9000,"username":"user", "password":"password", "temp_dir": "C:/Downloads/proxy_extension"}
-        },
-      "option_args": ["--my-arg1", "..."],
-      "capabilities": [],
-      "adb": False,
+      "proxy": "http://example-proxy.com:9000", # note: auth not supported,
+      "extension_paths": ["path/to/extension_1", ...], # directory, .crx or .zip
+      "auth_proxy": {
+            "host":"host", "port":9000,
+            "username":"user", "password":"password", 
+            "temp_dir": "C:/Downloads/proxy_extension"
+                },
+      "args": ["--my-arg1", ...],
+      "capabilities": {"cap_1":"val_1", "cap_2":"val_2"},
+      "experimental_options":{"option1":"value1", "option2":"value2"},
+      "adb": False, # run on harware device over ADB
       "adb_package": "com.android.chrome",
       "use_running_app": True
   },
   "cdp": {
-    "browser": {
-      "pointer_as_touch": False,
-      "darkmode": False,
-      "mobile": True
-    },
     "touch": True,
+    "darkmode":None,
     "maxtouchpoints": 5,
     "cores":8,
     "cdp_args": [],
     "emulation": {"mobile":True,"width": 384, "height": 700, "deviceScaleFactor": 10,
         "screenOrientation": {"type": "portrait-primary", "angle": 0}},
     "patch_version": True, # to patch automatically, or use "111.0.5563.111"
     "useragent": {
@@ -113,69 +119,72 @@
                     "wow64": False}
     }
   }
 }
 ```
 
 ### Modify-headers
-```python
 
-from selenium_interceptor.interceptor import cdp_listener
-
-from selenium_profiles import driver as mydriver
+using selenium-wire
+```python
+from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
 
-mydriver = mydriver()
-profile = profiles.Windows()
+profile = profiles.Android()
 
-driver = mydriver.start(profile)
+mydriver = webdriver.Chrome(profile, uc_driver=False, seleniumwire_options=True) # or pass seleniumwire-options
+driver = mydriver.start()
 
-cdp_listener = cdp_listener(driver=driver)
-cdp_listener.specify_headers({"sec-ch-ua-platform":"Android"})
-thread = cdp_listener.start_threaded(listener={"listener": cdp_listener.requests, "at_event": cdp_listener.modify_headers})
+def interceptor(request):
+    request.headers['New-Header'] = 'Some Value'
+driver.request_interceptor = interceptor
 
-driver.get("https://modheader.com/headers?product=ModHeader")
+# checkout headers
+driver.get("https://httpbin.org/headers")
+
+input("Press ENTER to quit..")
+driver.quit()
+exit()
 ```
-Don't forget to execute
-`cdp_listener.terminate_all()`
 
 ### Touch_actions
 
 Example demonstration script
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome, ChromeOptions
 from selenium_profiles.profiles import profiles
-
-from selenium_profiles.scripts.driver_utils import actions
-
 from selenium.webdriver.common.by import By
 
+from selenium_profiles.scripts.driver_utils import TouchActionChain
+
 
 # Start Driver
-mydriver = mydriver()
+options = ChromeOptions()
 profile = profiles.Android()
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+mydriver = Chrome(profile, uc_driver=False, options=ChromeOptions)
+driver = mydriver.start()  # or .Android
 
 # initialise touch_actions
-actions = actions(driver)
+chain = TouchActionChain(driver)
 
 driver.get("https://cps-check.com/de/multi-touch-test")
 
 touch_box = driver.find_element(By.XPATH,'//*[@id="box"]') # Get element
-location = actions.mid_location(touch_box) # get element middle location
 
-# setup actions
-action = actions.touch_action_chain()
-action.pointer_action.move_to_location(location['x'],location['y'])
-action.pointer_action.pointer_down()
+
+
+chain.touch_and_hold(touch_box)
+chain.pause(10)
+chain.release(touch_box)
 
 # perform actions
-action.perform()
+chain.perform()
 
-# now you should see a touch indication point on the Website
+# now you should see a touch indication
+# point on the Website for 10 seconds
 
 # quit driver
 input('Press ENTER to quit Driver\n')
 driver.quit()
 ```
 
 ### To export a profile:
@@ -188,29 +197,22 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] installer.py script
-  - [ ] bump to [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-  - [ ] [Chrome-Browser](https://www.google.de/chrome/) (silent install)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
-  - [ ] does not match worker scope (Emulation)
+  - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
-  - [x] with wrong version (is:111, emulate:107) fixed with "patch_version"
-      - v107 failed CSS features by 2 versions
-      - v107 failed v109 Window features
-      - v107 failed v109 CSS features
-- [x] Mobile emulation
-  - [ ] click_as touch makes code hung
+    - `navigator.hardwareConcurrency`
+- [ ] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -221,27 +223,24 @@
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
 - [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [ ] support for 
+- [X] support for 
   - [x] Windows
   - [x] Jupyter Notebook (Google-Colab)
   - [x] Linux
-- [ ] add error handling for [invalid keys](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4699462) in profile
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
-* [Selenium-Wire](https://github.com/wkeeling/selenium-wire) (proxy, no https)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
-* [Modheader-Selenium](https://github.com/modheader/modheader_selenium) (Changing headers now possible without)
 
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_profiles-2.2.5.5/build_upload.md` & `selenium_profiles-2.2.6/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/setup.py` & `selenium_profiles-2.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 import setuptools
+import sys
 
 
-# noinspection SpellCheckingInspection
-def is_collab():
-    import sys
-    # noinspection PyBroadException
-    try:
-        # noinspection PyPackageRequirements
-        import google.colab
-        cimport = True
-    except:
-        cimport = False
-    if ('google.colab' in sys.modules) and cimport:
-        return True
-    else:
-        return False
+requirements = ['selenium', 'requests', 'selenium-interceptor', "undetected-chromedriver", "selenium-wire", "webdriver-manager"]
 
-
-requirements = ['selenium', 'requests', 'selenium-interceptor', "undetected-chromedriver"]
-
-if is_collab():
-    requirements.extend(['PyVirtualDisplay', "webdriver-manager", "google-colab-shell"])
+if 'google.colab' in sys.modules: # we're on google-colab
+    requirements.extend(['PyVirtualDisplay', "google-colab-shell"])
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_profiles',
     author='Aurin Aegerter',
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/driver.py` & `selenium_profiles-2.2.6/src/selenium_profiles/webdriver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,218 @@
-import time  # for time.sleep()
-import traceback  # print exception
+# noinspection PyUnresolvedReferences
+from selenium.webdriver import ChromeOptions
 import warnings
-from collections import defaultdict
 
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service as ChromeService
 
-from selenium_profiles.scripts import profiles
-from selenium_profiles.utils.colab_utils import is_colab
-from selenium_profiles.scripts.cdp_tools import cdp_tools
-from selenium_profiles.scripts.driver_utils import sendkeys
-from selenium_profiles.scripts import undetected
-from selenium_profiles.scripts.driver_utils import requests, actions
+#
+class Chrome:
+    # noinspection PyDefaultArgument
+    def __init__(self, profile: dict = None, chrome_binary:str=None, executable_path:str = None,
+                 options = None,dublicate_policy: str = "warn-add", safe_dublicates: list = ["--add-extension"],
+                 uc_driver: bool or None = None, seleniumwire_options:dict or bool or None = None):
+        from collections import defaultdict
+        from selenium.webdriver.chrome.service import Service as ChromeService
+        from selenium_profiles.utils.colab_utils import is_colab
+        from selenium_profiles.scripts.cdp_tools import cdp_tools
+        from selenium_profiles.scripts.profiles import options as options_handler
+        from selenium_profiles.utils.utils import valid_key
 
-from selenium_profiles.utils.utils import sel_profiles_path  # read txt files
 
-
-# noinspection PyPep8Naming,GrazieInspection
-class driver(object):
-    def __init__(self):
         # initial attributes
-        # noinspection SpellCheckingInspection
-        self.returnnavigator = None
-        self.profile = None
-        self.driver = None
-        self.cdp_tools = None
-        self.options = None
-
-        self.profiles = profiles.profiles()
+        self.cdp = None
+        self._started = None
+        self.kwargs = {}
+
+        self.uc_driver = uc_driver
+        self.seleniumwire_options = seleniumwire_options
+        self.executable_path = executable_path
+        self.cdp_tools = cdp_tools
+        self.chrome_binary = chrome_binary
 
-    # noinspection PyUnresolvedReferences
-    def start(self, profile: dict, uc_driver: bool = False, executable_path:str = None, chrome_binary:str=None):
+        valid_key(profile.keys(), ["cdp", "options"], "profile (selenium-profiles)")
         self.profile = defaultdict(lambda: None)
         self.profile.update(profile)
 
-        if is_colab():  # google-colab doesn't support sandbox!
+        # sandbox handling for google-colab
+        if is_colab():
             # todo: nested default-dict with Lambda: None
-            if "options" in self.profile.keys():
-                if "browser" in self.profile["options"].keys():
-                    if "sandbox" in self.profile["options"]["browser"].keys():
-                        if self.profile["options"]["browser"]["sandbox"] is True:
-                            warnings.warn('Google-colab doesn\'t work with sandbox enabled yet, disabling..')
-                    else:
-                        self.profile["options"]["browser"].update({"sandbox":False})
+            if self.profile["options"]:
+                # noinspection PyUnresolvedReferences
+                if 'sandbox' in self.profile["options"].keys():
+                    # noinspection PyUnresolvedReferences
+                    if self.profile["options"]["sandbox"] is True:
+                        import warnings
+                        warnings.warn('Google-colab doesn\'t work with sandbox enabled yet, disabling sandbox')
                 else:
-                    self.profile["options"].update({"browser":{"sandbox":False}})
+                     # noinspection PyUnresolvedReferences
+                     self.profile["options"].update({"sandbox": False})
             else:
                 # noinspection PyTypeChecker
-                self.profile.update({"options":{"browser":{"sandbox":False}}})
+                self.profile.update({"options": {"sandbox": False}})
 
-        if uc_driver:
-            import undetected_chromedriver as uc  # undetected chromedriver
-            self.options = uc.ChromeOptions()  # selenium.webdriver options, https://peter.sh/experiments/chromium-command-line-switches/
+        # import webdriver
+        if self.uc_driver:
+            if self.seleniumwire_options:
+                import seleniumwire.undetected_chromedriver as webdriver
+            else:
+                import undetected_chromedriver as webdriver
         else:
-            self.options = webdriver.ChromeOptions()
+            if self.seleniumwire_options:
+                from seleniumwire import webdriver
+            else:
+                from selenium import webdriver
 
-        # options-manager
-        self.options = self.profiles.options.set(options=self.options, options_profile=self.profile["options"])
+        if type(self.seleniumwire_options) is dict:
+            self.kwargs.update({"seleniumwire_options":self.seleniumwire_options})
 
-        if executable_path is None: # chromedriver path
-            if uc_driver:
-                executable_path = None
-            else:
-                from selenium.webdriver.chrome.service import DEFAULT_EXECUTABLE_PATH
-                executable_path = DEFAULT_EXECUTABLE_PATH
+        self.driver = webdriver.Chrome
+        if not options:
+            options = webdriver.ChromeOptions()
 
-        service = ChromeService(executable_path=executable_path)
 
 
-        if not (chrome_binary is None):
-            self.options.binary_location = chrome_binary
+        # options-manager
+        self.options = options_handler(options, self.profile["options"], dublicate_policy=dublicate_policy, safe_dublicates=safe_dublicates)
+
+        # chrome executable path
+        if not self.chrome_binary :
+            self.options.Options.binary_location = chrome_binary
 
-        # ACTUAL START
+        # process kwargs
 
         if uc_driver:
-            # noinspection PyUnboundLocalVariable
-            self.driver = uc.Chrome(use_subprocess=True, options=self.options, keep_alive=True, driver_executable_path=executable_path)  # start undetected_chromedriver
+            if self.executable_path:
+                self.kwargs.update({"driver_executable_path":self.executable_path})
         else:
+            # detectability options
+            from selenium_profiles.scripts import undetected
+
+            # is adb used ?
             try:
                 # noinspection PyUnresolvedReferences
                 adb = self.profile["options"]["adb"]
             except TypeError:
                 adb = None
             except KeyError:
                 adb = None
 
-            self.options = undetected.config_options(self.options, adb=adb)
+            self.options.Options = undetected.config_options(self.options.Options, adb=adb)
 
-            # Actual start of chrome
-            self.driver = webdriver.Chrome(options=self.options, service=service)  # start selenium webdriver
+            # chromedriver path
+            if self.executable_path:
+                self.kwargs.update({"service": ChromeService(executable_path=self.executable_path)})
 
-        self.driver.get("http://lumtest.com/myip.json")  # wait browser to start
+        # add options to kwargs
+        self.kwargs.update({"options": self.options.Options})
+
+    def start(self):
+
+        if self._started:
+            raise TypeError("webdriver.Chrome() object can't be re-used")
+
+        # Actual start of chrome
+        self.driver = self.driver(**self.kwargs)
+        self._started = True
 
-        self.cdp_tools = cdp_tools(self.driver)
+
+        # cdp tools
+
+        self.driver.get("http://lumtest.com/myip.json")  # wait browser to start
+        self.cdp_tools = self.cdp_tools(self.driver)
 
         self.cdp_tools.evaluate_on_document_identifiers.update({1: # we know that it is there:)
                 """(function () {window.cdc_adoQpoasnfa76pfcZLmcfl_Array = window.Array;
                 window.cdc_adoQpoasnfa76pfcZLmcfl_Object = window.Object;
                 window.cdc_adoQpoasnfa76pfcZLmcfl_Promise = window.Promise;
                 window.cdc_adoQpoasnfa76pfcZLmcfl_Proxy = window.Proxy;
                 window.cdc_adoQpoasnfa76pfcZLmcfl_Symbol = window.Symbol;
                 }) ();"""})
 
-        self.cdp_tools.delete_all_cookies()  # delete website cookies
-
-        # execute cdp based on profile
-        self.profiles.cdp.set(driver=self.driver, cdp_profile=self.profile["cdp"])
+        from selenium_profiles.scripts.profiles import cdp as cdp_handler
+        self.cdp = cdp_handler(self.driver, self.cdp_tools)
+        self.cdp.apply(cdp_profile=self.profile["cdp"])
 
-        profiles.exec_js_evaluators(self.profile, self.driver, self.cdp_tools)
-
-        if not uc_driver:
+        if not self.uc_driver:
+            from selenium_profiles.scripts import undetected
             undetected.exec_cdp(self.driver, self.cdp_tools)
 
-        self.driver.profile = self.profile
-        self.driver.options = self.options
         self.add_funcs_to_driver()
 
         # Return actual driver
         return self.driver
 
     def add_funcs_to_driver(self):
 
-        self.driver.cdp_tools = self.cdp_tools
+        # add selenium-profiles utils to driver
+        class utils(object):
+            pass
+            def apply(self, profile:dict):
+                """
+                apply options after driver allready started
+                :param profile: selenium-profiles options
+                """
+                from selenium_profiles.utils.utils import valid_key
+                valid_key(profile.keys(),["cdp", "options"], "profile (selenium-profiles)")
+                if "options" in profile.keys():
+                    warnings.warn('profile["options"] can\'t be applied when driver allready started')
+                if "cdp" in profile.keys():
+                    # noinspection PyUnresolvedReferences
+                    self.cdp.apply(profile["cdp"])
+
+        utils = utils()
+
+        # our profile
+        utils.__setattr__("profile",self.profile)
 
         # add selenium-interceptor
         from selenium_interceptor.interceptor import cdp_listener
-        self.driver.cdp_listener = cdp_listener(driver=self.driver)
+        utils.__setattr__("cdp_listener", cdp_listener(driver=self.driver))
 
-        # add my functions to driver$
+        # add my functions
+        utils.__setattr__("get_profile", self.get_profile)
+        utils.__setattr__("export_profile", self.export_profile)
+        utils.__setattr__("get_profile", self.get_profile)
+        utils.__setattr__("cdp", self.cdp)
 
-        self.driver.send_keys = sendkeys # DEPRECATED!
+        from selenium_profiles.scripts.driver_utils import requests, actions, TouchActionChain
 
-        self.driver.get_profile = self.get_profile
-        self.driver.requests = requests(self.driver)
-        self.driver.actions = actions(self.driver)
+        # requests.fetch
+        requests = requests(self.driver)
+        utils.__setattr__("fetch", requests.fetch)
 
-        # Captcha
-        self.driver.solve_captcha = self.solve_captcha
+        actions = actions(self.driver)
+        actions.__setattr__("TouchActionChain", TouchActionChain)
+        utils.__setattr__("actions", actions)
 
-        # patch cookie functions
+        self.driver.profiles = utils
+
+        # patch driver functions
         self.driver.get_cookies = self.cdp_tools.get_cookies
         self.driver.add_cookie = self.cdp_tools.add_cookie
         self.driver.get_cookie = self.cdp_tools.get_cookie
         self.driver.delete_cookie = self.cdp_tools.delete_cookie
         self.driver.delete_all_cookies = self.cdp_tools.delete_all_cookies
 
-    def export_profile(self, to_path=sel_profiles_path() + "files/user_dir"):
+    def export_profile(self, to_path=None):
         import shutil
+        self.ensure_started()
+
+        if not to_path: # default path
+            from selenium_profiles.utils.utils import sel_profiles_path
+            to_path = sel_profiles_path() + "files/user_dir"
+
+
+        # noinspection PyUnresolvedReferences
         shutil.copytree(self.driver.user_data_dir, to_path)
 
     def get_profile(self):
         from selenium_profiles.utils.utils import read
-        js = read('js/get_navigator.js')
-        # noinspection PyBroadException
-        self.driver.execute_script(js)
-        time.sleep(1)
-        return self.driver.execute_script('return window.useragent')
-
-    def solve_captcha(self):
-        from selenium.webdriver.common.by import By  # locate elements
-        from selenium.webdriver.support import expected_conditions as EC
-        from selenium.webdriver.support.ui import WebDriverWait
-
-        # noinspection PyBroadException
-        try:
-            wait = WebDriverWait(self.driver, 5)  # driver 5s timeout
-            #  click on captcha
-            wait.until(EC.frame_to_be_available_and_switch_to_it(
-                (By.CSS_SELECTOR, "iframe[name^='a-'][src^='https://www.google.com/recaptcha/api2/anchor?']")))
-            wait.until(EC.element_to_be_clickable((By.XPATH, "//span[@id='recaptcha-anchor']"))).click()
-            self.driver.switch_to.default_content()
-            # click on audio
-            WebDriverWait(self.driver, 4).until(EC.frame_to_be_available_and_switch_to_it(
-                (By.CSS_SELECTOR, "iframe[name^='c-'][src^='https://www.google.com/recaptcha/api2/bframe?']")))
-            time.sleep(2)
-            self.driver.find_element(By.XPATH, '//*[@id="recaptcha-audio-button"]').click()
-            self.driver.switch_to.default_content()
-        except:
-            # check "try again later"
-            WebDriverWait(self.driver, 4).until(EC.frame_to_be_available_and_switch_to_it(
-                (By.CSS_SELECTOR, "iframe[name^='c-'][src^='https://www.google.com/recaptcha/api2/bframe?']")))
-            self.driver.find_element(By.CSS_SELECTOR,
-                                     "a[href='https://developers.google.com/recaptcha/docs/faq#my-computer-or-network-may-be-sending-automated-queries']")
-            traceback.print_exc()
-            warnings.warn("Captcha could not be solved!")
-            self.driver.switch_to.default_content()
+        self.ensure_started()
+
+        js = read('js/export_profile.js', sel_root=True)
+
+        # noinspection PyArgumentList
+        return self.driver.execute_async_script(js)
+
+    def ensure_started(self):
+        if not self._started:
+            raise TypeError("driver needs to be started first :)")
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/files/proxy_extension/background.js` & `selenium_profiles-2.2.6/src/selenium_profiles/files/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/js/get_navigator.js` & `selenium_profiles-2.2.6/src/selenium_profiles/js/export_profile.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,48 @@
+try {
+    var done = arguments[0]
+} catch {
+    var done = undefined
+} // we're executing with selenium
+
 function roundHalf(num) { // round to half int
     if (typeof num === 'number') {
         return Math.round(num * 2) / 2
     } else {
         return null
     }
 };
 
 function copyToClipboard(text) {
     window.prompt("Copy to clipboard: Ctrl+C, Enter", text);
 };
 
+function is_done(value) {
+    if (done) {
+        done(value)
+    } else {
+        copyToClipboard(JSON.stringify(value))
+    }
+}
+
 function a(elem, replace = null) { // replace non_existing variables with null
     try {
         elem = eval(elem)
     } catch {
         elem = replace
     };
     //if_exist, else null
     if (typeof elem !== 'undefined') {
         return elem
     } else {
         return replace
     };
 };
 
-function build_navigator() {
+function build_navigator(useragent) {
     wow64 = a(navigator.userAgent.indexOf('WOW64') > -1);
 
     maxtouchpoints = a('window.navigator.maxTouchPoints');
     if (maxtouchpoints > 16 || maxtouchpoints < 1) {
         maxtouchpoints = 10
     }
 
@@ -60,42 +74,38 @@
             "emulation": my_screen,
             "cores": a("navigator.hardwareConcurrency"),
             "useragent": {
                 "platform": a('navigator.platform'),
                 "acceptLanguage": a('navigator.language') || a('navigator.userLanguage'),
                 "userAgent": a('navigator.userAgent'),
                 "userAgentMetadata": {
-                    "brands": window.useragent["brands"],
-                    "fullVersionList": window.useragent["fullVersionList"],
-                    "fullVersion": window.useragent["uaFullVersion"],
-                    "platform": window.useragent["platform"],
-                    "platformVersion": window.useragent["platformVersion"],
-                    "architecture": window.useragent["architecture"],
-                    "model": window.useragent["model"],
-                    "mobile": window.useragent["mobile"],
-                    "bitness": window.useragent["bitness"],
+                    "brands": useragent["brands"],
+                    "fullVersionList": useragent["fullVersionList"],
+                    "fullVersion": useragent["uaFullVersion"],
+                    "platform": useragent["platform"],
+                    "platformVersion": useragent["platformVersion"],
+                    "architecture": useragent["architecture"],
+                    "model": useragent["model"],
+                    "mobile": useragent["mobile"],
+                    "bitness": useragent["bitness"],
                     "wow64": window.wow64
                 }
             }
         }
     }
     return my_navigator
 }
 
 console.log('Getting Profile..')
-window.useragent_set = false;
 navigator.userAgentData.getHighEntropyValues( // get useragent
         ["architecture",
             "model",
             "platformVersion",
             "bitness",
             "uaFullVersion",
             "fullVersionList"
         ])
     .then((values) => {
-        window.useragent = values;
-        console.log(values);
-        window.useragent = build_navigator();
-        window.useragent_set = true
-        return window.useragent;
-        //copyToClipboard(JSON.stringify(window.navigator()));
+        my_profile = build_navigator(values);
+        console.log(my_profile)
+        is_done(my_profile)
     });
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/default.json` & `selenium_profiles-2.2.6/src/selenium_profiles/profiles/default.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9479166666666666%*

 * *Differences: {"'Android'": "{'options': {replace: OrderedDict([('gpu', False), ('window_size', "*

 * *              "OrderedDict([('x', 384), ('y', 700)]))])}, 'cdp': {'maxtouchpoints': 10}}",*

 * * "'Windows'": "{'options': {replace: OrderedDict([('gpu', False), ('window_size', "*

 * *              "OrderedDict([('x', 1024), ('y', 648)]))])}}"}*

```diff
@@ -8,15 +8,15 @@
                 "mobile": true,
                 "screenOrientation": {
                     "angle": 0,
                     "type": "portraitPrimary"
                 },
                 "width": 384
             },
-            "maxtouchpoints": 1,
+            "maxtouchpoints": 10,
             "patch_version": true,
             "touch": true,
             "useragent": {
                 "acceptLanguage": "en-US",
                 "platform": "Linux aarch64",
                 "userAgent": "Mozilla/5.0 (Linux; Android 11; HD1913) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Mobile Safari/537.36",
                 "userAgentMetadata": {
@@ -56,20 +56,18 @@
                     "platform": "Android",
                     "platformVersion": "11.0.0",
                     "wow64": false
                 }
             }
         },
         "options": {
-            "browser": {
-                "gpu": false,
-                "window_size": {
-                    "x": 384,
-                    "y": 700
-                }
+            "gpu": false,
+            "window_size": {
+                "x": 384,
+                "y": 700
             }
         }
     },
     "IOS": {},
     "Linux": {},
     "Tablet": {},
     "Windows": {
@@ -129,17 +127,15 @@
                     "platform": "Windows",
                     "platformVersion": "10.0.0",
                     "wow64": false
                 }
             }
         },
         "options": {
-            "browser": {
-                "gpu": false,
-                "window_size": {
-                    "x": 1024,
-                    "y": 648
-                }
+            "gpu": false,
+            "window_size": {
+                "x": 1024,
+                "y": 648
             }
         }
     }
 }
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/example.json` & `selenium_profiles-2.2.6/src/selenium_profiles/profiles/example.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6843520220588235%*

 * *Differences: {"'cdp'": "{'cdp_args': {replace: OrderedDict()}, 'emulation': {'screenOrientation': {'type': "*

 * *          "'portraitPrimary'}}, 'pointer_as_touch': False, 'darkmode': False, delete: ['browser']}",*

 * * "'options'": "{'sandbox': True, 'window_size': OrderedDict([('x', 1024), ('y', 648)]), "*

 * *              "'headless': False, 'load_images': True, 'incognito': True, 'app': False, 'gpu': "*

 * *              "False, 'proxy': None, 'extension_paths': [], 'auth_proxy': OrderedDict([('host', "*

 * *              "'host'), ('port […]*

```diff
@@ -1,26 +1,23 @@
 {
     "cdp": {
-        "browser": {
-            "darkmode": false,
-            "mobile": true,
-            "pointer_as_touch": false
-        },
-        "cdp_args": [],
+        "cdp_args": {},
+        "darkmode": false,
         "emulation": {
             "deviceScaleFactor": 10,
             "height": 700,
             "mobile": true,
             "screenOrientation": {
                 "angle": 0,
-                "type": "portrait-primary"
+                "type": "portraitPrimary"
             },
             "width": 384
         },
         "maxtouchpoints": 5,
+        "pointer_as_touch": false,
         "touch": true,
         "useragent": {
             "acceptLanguage": "en-US",
             "platform": "Linux aarch64",
             "userAgent": "Mozilla/5.0 (Linux; Android 11; HD1913) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Mobile Safari/537.36",
             "userAgentMetadata": {
                 "architecture": "",
@@ -61,34 +58,29 @@
                 "wow64": false
             }
         }
     },
     "options": {
         "adb": false,
         "adb_package": "com.android.chrome",
-        "browser": {
-            "app": false,
-            "gpu": false,
-            "headless": false,
-            "incognito": true,
-            "load_images": true,
-            "proxy": null,
-            "proxy_method": null,
-            "sandbox": true,
-            "window_size": {
-                "x": 1024,
-                "y": 648
-            }
+        "app": false,
+        "args": [],
+        "auth_proxy": {
+            "host": "host",
+            "password": "password",
+            "port": 9000,
+            "username": "user"
         },
         "capabilities": [],
-        "extensions": {
-            "auth_proxy": {
-                "host": "host",
-                "password": "password",
-                "port": 9000,
-                "username": "user"
-            },
-            "extension_paths": []
-        },
-        "option_args": []
+        "extension_paths": [],
+        "gpu": false,
+        "headless": false,
+        "incognito": true,
+        "load_images": true,
+        "proxy": null,
+        "sandbox": true,
+        "window_size": {
+            "x": 1024,
+            "y": 648
+        }
     }
 }
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/profiles.py` & `selenium_profiles-2.2.6/src/selenium_profiles/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/profiles/scratch.json` & `selenium_profiles-2.2.6/src/selenium_profiles/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/cdp_tools.py` & `selenium_profiles-2.2.6/src/selenium_profiles/scripts/cdp_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,97 +1,95 @@
 from typing import Dict, List  # define types in functions
 import warnings
 import json
-import traceback
-
 
 # noinspection PyPep8Naming
-class cdp_tools(object):
+class cdp_tools:
     def __init__(self, driver):
-        self.driver = driver
+        self._driver = driver
 
         # initial property
         self.evaluate_on_document_identifiers = {}
 
     # EMULATION
 
     def set_emulation(self, emulation:bool or None) -> (Dict[str, int or Dict[str, str or int or float]]):
         if emulation:
-            return self.driver.execute_cdp_cmd('Emulation.setDeviceMetricsOverride', emulation)
+            return self._driver.execute_cdp_cmd('Emulation.setDeviceMetricsOverride', emulation)
 
     def clear_emulation(self, enabled:bool or None):
         if enabled or (enabled is None):
-            self.driver.execute_cdp_cmd("Emulation.clearDeviceMetricsOverride", {})
+            self._driver.execute_cdp_cmd("Emulation.clearDeviceMetricsOverride", {})
 
     def set_useragent(self, useragent) -> Dict[str, str or Dict[str, str or bool or List[Dict[str, str]]]] or None:
         if useragent:
-            return self.driver.execute_cdp_cmd('Emulation.setUserAgentOverride', useragent)
+            return self._driver.execute_cdp_cmd('Emulation.setUserAgentOverride', useragent)
 
     def set_cores(self, cores_count:int or None=8):
         if cores_count:
-            return self.driver.execute_cdp_cmd("Emulation.setHardwareConcurrencyOverride", {"hardwareConcurrency":cores_count})
+            return self._driver.execute_cdp_cmd("Emulation.setHardwareConcurrencyOverride", {"hardwareConcurrency":cores_count})
 
     # BROWSER
 
     def set_darkmode(self, enabled=True, mobile=True) -> (bool, bool):
         if not (mobile or mobile is None) and enabled:
             warnings.warn('darkmode might look weird without mobile_view!')
         if enabled:
-            return self.driver.execute_cdp_cmd('Emulation.setAutoDarkModeOverride',
-                                           {'enabled': enabled})
+            return self._driver.execute_cdp_cmd('Emulation.setAutoDarkModeOverride',
+                                                {'enabled': enabled})
 
     # TOUCH
 
     def set_touchpoints(self, enabled:bool or None=True, maxpoints:int or None=10):  # set touch options
         if maxpoints is None:
             maxpoints = 10
-        return self.driver.execute_cdp_cmd('Emulation.setTouchEmulationEnabled',
-                                           {'enabled': enabled, 'maxTouchPoints': maxpoints})  # already set in options
+        return self._driver.execute_cdp_cmd('Emulation.setTouchEmulationEnabled',
+                                            {'enabled': enabled, 'maxTouchPoints': maxpoints})  # already set in options
 
     def pointer_as_touch(self, mobile:bool or None, enabled:bool or None=True):  # (makes code hung)
         if mobile or mobile is None:
             config = 'mobile'
         else:
             config = 'desktop'
         if enabled:
             warnings.warn('Actions execute, but then take long when "EmitTouchEventsForMouse"!')
-            return self.driver.execute_cdp_cmd('Emulation.setEmitTouchEventsForMouse', {'enabled': enabled,
+            return self._driver.execute_cdp_cmd('Emulation.setEmitTouchEventsForMouse', {'enabled': enabled,
                                                                                     'configuration': config})  # executes, but then takes long [maybe check if success?]
 
     # OVERRIDE JAVASCRIPT
 
     def evaluate_on_new_document(self, js: str):  # evaluate js on every new page
         identifier = int(
-            self.driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {"source": js})["identifier"])
+            self._driver.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument", {"source": js})["identifier"])
         self.evaluate_on_document_identifiers.update({identifier: js})
         return identifier
 
     # remove js evaluation  on every new page for specific script
     def remove_evaluate_on_document(self, identifier: int):
         del self.evaluate_on_document_identifiers[identifier]
-        return self.driver.execute_cdp_cmd("Page.removeScriptToEvaluateOnNewDocument", {"identifier": str(identifier)})
+        return self._driver.execute_cdp_cmd("Page.removeScriptToEvaluateOnNewDocument", {"identifier": str(identifier)})
 
     # define var.property for javascript
     def define_prop_on_new_document(self, var, prop, val, func='get: ()') -> (str, str, any, str):
         self.evaluate_on_new_document(
             "Object.defineProperty(" + var + ", " + json.dumps(prop) + ", {" + func + " => " + json.dumps(val) + "})")
 
     # COOKIES
 
     def get_cookies(self):
-        return self.driver.execute_cdp_cmd("Network.getAllCookies", {})
+        return self._driver.execute_cdp_cmd("Network.getAllCookies", {})['cookies']
 
     def get_cookie(self, urls: list = None):
         if urls:
             arg = {"urls": urls}
         else:
             arg = {}
-        return self.driver.execute_cdp_cmd("Network.getCookies", arg)
+        return self._driver.execute_cdp_cmd("Network.getCookies", arg)
 
     def add_cookie(self, cookie_dict):
-        return self.driver.execute_cdp_cmd("Network.setCookie", cookie_dict)
+        return self._driver.execute_cdp_cmd("Network.setCookie", cookie_dict)
 
     def delete_cookie(self, name: str):
-        return self.driver.execute_cdp_cmd("Network.deleteCookies", {"name": name})
+        return self._driver.execute_cdp_cmd("Network.deleteCookies", {"name": name})
 
     def delete_all_cookies(self):
-        return self.driver.execute_cdp_cmd("Network.clearBrowserCookies", {})
+        return self._driver.execute_cdp_cmd("Network.clearBrowserCookies", {})
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/proxy_extension.py` & `selenium_profiles-2.2.6/src/selenium_profiles/scripts/proxy_extension.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/scripts/undetected.py` & `selenium_profiles-2.2.6/src/selenium_profiles/scripts/undetected.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,24 +16,31 @@
     x = driver.execute_cdp_cmd('Emulation.setIdleOverride', {'isUserActive': True, 'isScreenUnlocked': True})
 
     def get_cdc_props():  # if true ==> detectable
         return driver.execute_script(read('js/undetected/get_cdc_props.js'))
 
     if get_cdc_props():
         # remove cdc-props:)
+
         # cdp_tools.evaluate_on_new_document(read('js/undetected/remove_cdc_props.js'))
         cdp_tools.remove_evaluate_on_document(1)
 
         if do_return:
             return cdp_tools.evaluate_on_document_identifiers
 
 
-def config_options(options, adb=False):
-    options.add_experimental_option("excludeSwitches", ["enable-automation"])
+def config_options(options, adb=False, dublicate_policy="warn-replace"):
+    from selenium_profiles.scripts.profiles import options as option_manager
+    manager = option_manager(options)
+    if "excludeSwitches" in options.experimental_options.keys():
+        if "enable-automation" not in options.experimental_options["excludeSwitches"]:
+            manager.Options.experimental_options["excludeSwitches"].append("enable-automation")
+    else:
+        manager.update_experimental_options({"excludeSwitches": ["enable-automation"]}, dublicate_policy=dublicate_policy)
     if not adb or adb is None:
-        options.add_experimental_option('useAutomationExtension', False)
-    options.arguments.extend(["--disable-blink-features=AutomationControlled", "--disable-blink-features"])
+        manager.update_experimental_options({'useAutomationExtension': False}, dublicate_policy=dublicate_policy)
+    manager.extend_arguments(["--disable-blink-features=AutomationControlled", "--disable-blink-features"], dublicate_policy="warn-add")
 
     # suppress welcome
-    options.arguments.extend(["--no-default-browser-check", "--no-first-run"])
+    manager.extend_arguments(["--no-default-browser-check", "--no-first-run"], dublicate_policy="warn-add")
 
-    return options
+    return manager.Options
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/utils/colab_utils.py` & `selenium_profiles-2.2.6/src/selenium_profiles/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles/utils/utils.py` & `selenium_profiles-2.2.6/src/selenium_profiles/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-import warnings
 import os
+
 import selenium_profiles
 
 
 def sel_profiles_path():
     return os.path.dirname(selenium_profiles.__file__) + "/"
 
 
@@ -25,18 +25,27 @@
         return f.write(content)
 
 def read_json(filename: str = 'example.json', encoding: str = "utf-8",sel_root=True):
     if sel_root:
         path = sel_profiles_path() + filename
     else:
         path = filename
-    with open(sel_profiles_path() + filename, 'r', encoding=encoding) as f:
+    with open(path, 'r', encoding=encoding) as f:
         return json.load(f)
 
 
 def write_json(obj: dict or list, filename: str = "out.json", encoding: str = "utf-8",sel_root=True):
     if sel_root:
         path = sel_profiles_path() + filename
     else:
         path = filename
     with open(path, "w", encoding=encoding) as outfile:
         outfile.write(json.dumps(obj))
+
+def check_cmd(value, values):
+    if value not in values:
+        raise ValueError("got " + str(value) + " , but expected " + str(values))
+
+def valid_key(got:list or set, valid:list, obj_name:str):
+    for key in got:
+        if key not in valid:
+            raise ValueError(f"'{key}' isn't a valid key for {obj_name}")
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/PKG-INFO` & `selenium_profiles-2.2.6/src/selenium_profiles.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-profiles
-Version: 2.2.5.5
+Version: 2.2.6
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -26,22 +26,26 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
 
 # Selenium-Profiles
 
+[![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
+
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
 * **Undetected** by Google, Cloudflare, creep-js ..
-* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor)
+* [Modifying headers](#Modify-headers) supported using [Selenium-Interceptor](https://github.com/kaliiiiiiiiii/Selenium-Interceptor) or seleniumwire
 * [Touch Actions](#Touch_actions)
 * [proxies with authentication](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4704385)
 * making single [POST](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/11#discussioncomment-4797109), GET or other requests using `driver.requests.fetch(url, options)`  ([syntax](https://developer.mozilla.org/en-US/docs/Web/API/fetch#syntax))
 * headless unofficially supported
+* apply profile on allready running driver with `driver.profiles.apply(profiles.Android())`
+* use of [seleniumwire](https://github.com/wkeeling/selenium-wire)
 
 for the latest features, have a look at the `dev` branch
 
 ### Feel free to test my code!
 
 ## Getting Started
 
@@ -54,73 +58,75 @@
 
 * Install [Google-Chrome](https://www.google.de/chrome/) (or another chromium-based browser)
 * ```pip install selenium-profiles```
 
 ### Start Driver
 
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By  # locate elements
+from selenium.webdriver import ChromeOptions
+
 
-mydriver = mydriver()
 profile = profiles.Windows()
-# profile["options"]["browser"]["headless"] = True
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+options = ChromeOptions()
+mydriver = Chrome(profile, options=options, uc_driver=False)
+# mydriver.options.add_argument("--headless=new")
+
+driver = mydriver.start()  # or .Android
 
 # get url
-driver.get('https://browserleaks.com/client-hints')  # test client hints
+driver.get('https://abrahamjuliot.github.io/creepjs/')  # test client hints
 
 input("Press ENTER to exit: ")
 driver.quit()  # Execute on the End!
 ```
 
 Don't forget to execute
 ```driver.quit()```
 in the End. Else-wise your temporary folder will get flooded!
 
 #### Run with Google-Colab
-[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: google-colab/selenium_profiles.ipynb)
+__[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/master/google-colab/selenium_profiles.ipynb) (file: master@google-colab/selenium_profiles.ipynb)__
+
+[Google-Colab](https://colab.research.google.com/github/kaliiiiiiiiii/Selenium-Profiles/blob/dev/google-colab/selenium_profiles.ipynb) (file: dev@google-colab/selenium_profiles.ipynb)
 
 ## Profiles
 
 Example Profile: 
 ```python
 profile = \
 {
   "options": {
-    "browser": {
       "sandbox": True,
       "window_size": {"x":1024,"y":648},
       "headless": False,
       "load_images": True,
       "incognito": True,
+      "touch": True,
       "app": False,
-      "touch": True, # 
       "gpu": False,
-      "proxy": "example-proxy.com:9000", # note: auth not supported
-      "proxy_method": "http://" # optional, default: "socks5://"
-    },
-      "extensions": {
-          "extension_paths": ["path/to/extension_1"], # directory, .crx or .zip
-          "auth_proxy": {"host":"host","port":9000,"username":"user", "password":"password", "temp_dir": "C:/Downloads/proxy_extension"}
-        },
-      "option_args": ["--my-arg1", "..."],
-      "capabilities": [],
-      "adb": False,
+      "proxy": "http://example-proxy.com:9000", # note: auth not supported,
+      "extension_paths": ["path/to/extension_1", ...], # directory, .crx or .zip
+      "auth_proxy": {
+            "host":"host", "port":9000,
+            "username":"user", "password":"password", 
+            "temp_dir": "C:/Downloads/proxy_extension"
+                },
+      "args": ["--my-arg1", ...],
+      "capabilities": {"cap_1":"val_1", "cap_2":"val_2"},
+      "experimental_options":{"option1":"value1", "option2":"value2"},
+      "adb": False, # run on harware device over ADB
       "adb_package": "com.android.chrome",
       "use_running_app": True
   },
   "cdp": {
-    "browser": {
-      "pointer_as_touch": False,
-      "darkmode": False,
-      "mobile": True
-    },
     "touch": True,
+    "darkmode":None,
     "maxtouchpoints": 5,
     "cores":8,
     "cdp_args": [],
     "emulation": {"mobile":True,"width": 384, "height": 700, "deviceScaleFactor": 10,
         "screenOrientation": {"type": "portrait-primary", "angle": 0}},
     "patch_version": True, # to patch automatically, or use "111.0.5563.111"
     "useragent": {
@@ -143,69 +149,72 @@
                     "wow64": False}
     }
   }
 }
 ```
 
 ### Modify-headers
-```python
 
-from selenium_interceptor.interceptor import cdp_listener
-
-from selenium_profiles import driver as mydriver
+using selenium-wire
+```python
+from selenium_profiles import webdriver
 from selenium_profiles.profiles import profiles
 
-mydriver = mydriver()
-profile = profiles.Windows()
+profile = profiles.Android()
 
-driver = mydriver.start(profile)
+mydriver = webdriver.Chrome(profile, uc_driver=False, seleniumwire_options=True) # or pass seleniumwire-options
+driver = mydriver.start()
 
-cdp_listener = cdp_listener(driver=driver)
-cdp_listener.specify_headers({"sec-ch-ua-platform":"Android"})
-thread = cdp_listener.start_threaded(listener={"listener": cdp_listener.requests, "at_event": cdp_listener.modify_headers})
+def interceptor(request):
+    request.headers['New-Header'] = 'Some Value'
+driver.request_interceptor = interceptor
 
-driver.get("https://modheader.com/headers?product=ModHeader")
+# checkout headers
+driver.get("https://httpbin.org/headers")
+
+input("Press ENTER to quit..")
+driver.quit()
+exit()
 ```
-Don't forget to execute
-`cdp_listener.terminate_all()`
 
 ### Touch_actions
 
 Example demonstration script
 ```python
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome, ChromeOptions
 from selenium_profiles.profiles import profiles
-
-from selenium_profiles.scripts.driver_utils import actions
-
 from selenium.webdriver.common.by import By
 
+from selenium_profiles.scripts.driver_utils import TouchActionChain
+
 
 # Start Driver
-mydriver = mydriver()
+options = ChromeOptions()
 profile = profiles.Android()
-driver = mydriver.start(profile, uc_driver=False)  # or .Android
+mydriver = Chrome(profile, uc_driver=False, options=ChromeOptions)
+driver = mydriver.start()  # or .Android
 
 # initialise touch_actions
-actions = actions(driver)
+chain = TouchActionChain(driver)
 
 driver.get("https://cps-check.com/de/multi-touch-test")
 
 touch_box = driver.find_element(By.XPATH,'//*[@id="box"]') # Get element
-location = actions.mid_location(touch_box) # get element middle location
 
-# setup actions
-action = actions.touch_action_chain()
-action.pointer_action.move_to_location(location['x'],location['y'])
-action.pointer_action.pointer_down()
+
+
+chain.touch_and_hold(touch_box)
+chain.pause(10)
+chain.release(touch_box)
 
 # perform actions
-action.perform()
+chain.perform()
 
-# now you should see a touch indication point on the Website
+# now you should see a touch indication
+# point on the Website for 10 seconds
 
 # quit driver
 input('Press ENTER to quit Driver\n')
 driver.quit()
 ```
 
 ### To export a profile:
@@ -218,29 +227,22 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] installer.py script
-  - [ ] bump to [webdriver-manager](https://pypi.org/project/webdriver-manager/)
-  - [ ] [Chrome-Browser](https://www.google.de/chrome/) (silent install)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
-  - [ ] does not match worker scope (Emulation)
+  - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
-  - [x] with wrong version (is:111, emulate:107) fixed with "patch_version"
-      - v107 failed CSS features by 2 versions
-      - v107 failed v109 Window features
-      - v107 failed v109 CSS features
-- [x] Mobile emulation
-  - [ ] click_as touch makes code hung
+    - `navigator.hardwareConcurrency`
+- [ ] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -251,27 +253,24 @@
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
 - [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [ ] support for 
+- [X] support for 
   - [x] Windows
   - [x] Jupyter Notebook (Google-Colab)
   - [x] Linux
-- [ ] add error handling for [invalid keys](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/6#discussioncomment-4699462) in profile
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
-* [Selenium-Wire](https://github.com/wkeeling/selenium-wire) (proxy, no https)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
-* [Modheader-Selenium](https://github.com/modheader/modheader_selenium) (Changing headers now possible without)
 
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
 ## License
```

### Comparing `selenium_profiles-2.2.5.5/src/selenium_profiles.egg-info/SOURCES.txt` & `selenium_profiles-2.2.6/src/selenium_profiles.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 MANIFEST.in
 README.md
 build_upload.md
 pyproject.toml
 setup.cfg
 setup.py
 src/selenium_profiles/__init__.py
-src/selenium_profiles/driver.py
+src/selenium_profiles/webdriver.py
 src/selenium_profiles.egg-info/PKG-INFO
 src/selenium_profiles.egg-info/SOURCES.txt
 src/selenium_profiles.egg-info/dependency_links.txt
 src/selenium_profiles.egg-info/requires.txt
 src/selenium_profiles.egg-info/top_level.txt
 src/selenium_profiles/files/__init__.py
 src/selenium_profiles/files/proxy_extension/background.js
 src/selenium_profiles/files/proxy_extension/manifest.json
 src/selenium_profiles/files/tmp/__init__.py
+src/selenium_profiles/files/tmp/proxy_extension/background.js
 src/selenium_profiles/files/tmp/proxy_extension/manifest.json
 src/selenium_profiles/js/__init__.py
-src/selenium_profiles/js/get_navigator.js
-src/selenium_profiles/js/run_box.js
+src/selenium_profiles/js/export_profile.js
+src/selenium_profiles/js/fetch.js
 src/selenium_profiles/js/undetected/__init.py
 src/selenium_profiles/js/undetected/get_cdc_props.js
 src/selenium_profiles/js/undetected/navigator_webdriver.js
 src/selenium_profiles/js/undetected/remove_cdc_props.js
 src/selenium_profiles/profiles/__init__.py
 src/selenium_profiles/profiles/default.json
 src/selenium_profiles/profiles/example.json
 src/selenium_profiles/profiles/profiles.py
 src/selenium_profiles/profiles/scratch.json
+src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
 src/selenium_profiles/scripts/__init__.py
 src/selenium_profiles/scripts/cdp_tools.py
 src/selenium_profiles/scripts/driver_utils.py
 src/selenium_profiles/scripts/profiles.py
 src/selenium_profiles/scripts/proxy_extension.py
-src/selenium_profiles/scripts/touch_actions.py
 src/selenium_profiles/scripts/undetected.py
 src/selenium_profiles/utils/__init__.py
 src/selenium_profiles/utils/colab_utils.py
 src/selenium_profiles/utils/installer.py
 src/selenium_profiles/utils/utils.py
 tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.5.5/tests/test_driver.py` & `selenium_profiles-2.2.6/tests/test_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import unittest
 
 from selenium_profiles.utils.utils import read_json
-from selenium_profiles.driver import driver as mydriver
+from selenium_profiles.webdriver import Chrome
 from selenium.webdriver.common.by import By  # locate elements
 
-mydriver = mydriver()
 
 
 def test_driver(choose: str, headless: bool = True, uc_driver=False):
-    import json
     profile = read_json(filename='profiles\\default.json')
-    # noinspection PyGlobalUndefined
-    global mydriver
     testprofile = profile[choose]
     testprofile["cdp"]["patch_version"] = None # don't change version :)
-    testprofile["options"]["browser"]["headless"] = headless
-    driver = mydriver.start(testprofile, uc_driver=uc_driver)
+    testprofile["options"]["headless"] = headless
+    my_driver = Chrome(profile=testprofile, uc_driver=uc_driver)
+    driver = my_driver.start()
     driver.get('https://browserleaks.com/client-hints')
     useragent = driver.find_element(By.XPATH, '//*[@id="content"]/table[1]/tbody/tr/td[2]').accessible_name
-    exported_profile = driver.get_profile()
+    exported_profile = driver.profiles.get_profile()
     driver.quit()
 
     print(choose+'\n'+useragent+'\n')
-    return {"profile": driver.profile, "exported_profile": exported_profile, "useragent":useragent}
+    return {"profile": driver.profiles.profile, "exported_profile": exported_profile, "useragent":useragent}
 
 
 class Driver(unittest.TestCase):
     # noinspection PyGlobalUndefined
     # Hello World!
     def test_windows(self):
-        global mydriver
         output = test_driver('Windows', headless=True)
         self.assertEqual(output["exported_profile"]["cdp"]["useragent"],
                          output["profile"]["cdp"]["useragent"])  # add assertion here
 
     # noinspection PyGlobalUndefined
     def test_android(self):
-        global mydriver
         output = test_driver('Android', headless=False)
         self.assertEqual(output["exported_profile"]["cdp"]["useragent"],
                          output["profile"]["cdp"]["useragent"])  # add assertion here
 
 
 if __name__ == '__main__':
     unittest.main()
```

