# Comparing `tmp/kameleo.local_api_client-2.6.0.tar.gz` & `tmp/kameleo.local_api_client-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kameleo.local_api_client-2.6.0.tar", last modified: Fri Feb 18 09:11:30 2022, max compression
+gzip compressed data, was "kameleo.local_api_client-2.9.0.tar", last modified: Fri Aug 19 09:54:29 2022, max compression
```

## Comparing `kameleo.local_api_client-2.6.0.tar` & `kameleo.local_api_client-2.9.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2022-02-18 09:11:30.547014 kameleo.local_api_client-2.6.0/
--rw-rw-rw-   0        0        0     1100 2021-07-21 14:14:28.000000 kameleo.local_api_client-2.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0     9536 2022-02-18 09:11:30.546011 kameleo.local_api_client-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     8970 2022-02-18 08:05:38.000000 kameleo.local_api_client-2.6.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-18 09:11:30.356013 kameleo.local_api_client-2.6.0/kameleo/
--rw-rw-rw-   0        0        0       57 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-18 09:11:30.376015 kameleo.local_api_client-2.6.0/kameleo/local_api_client/
--rw-rw-rw-   0        0        0      479 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/__init__.py
--rw-rw-rw-   0        0        0    12916 2022-02-18 05:27:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/builder_for_create_profile.py
--rw-rw-rw-   0        0        0    48266 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/kameleo_local_api_client.py
-drwxrwxrwx   0        0        0        0 2022-02-18 09:11:30.543012 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/
--rw-rw-rw-   0        0        0     6325 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/__init__.py
--rw-rw-rw-   0        0        0     3065 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile.py
--rw-rw-rw-   0        0        0     2048 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_preview.py
--rw-rw-rw-   0        0        0     2004 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_preview_py3.py
--rw-rw-rw-   0        0        0     2988 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_py3.py
--rw-rw-rw-   0        0        0     2125 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_search_parameters.py
--rw-rw-rw-   0        0        0     2112 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_search_parameters_py3.py
--rw-rw-rw-   0        0        0     1383 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser.py
--rw-rw-rw-   0        0        0     5149 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_cookie.py
--rw-rw-rw-   0        0        0     5118 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_cookie_py3.py
--rw-rw-rw-   0        0        0     1374 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_py3.py
--rw-rw-rw-   0        0        0     4298 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/cookie_request.py
--rw-rw-rw-   0        0        0     4287 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/cookie_request_py3.py
--rw-rw-rw-   0        0        0     5865 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/create_profile_request.py
--rw-rw-rw-   0        0        0     5757 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/create_profile_request_py3.py
--rw-rw-rw-   0        0        0     1092 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/device.py
--rw-rw-rw-   0        0        0     1090 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/device_py3.py
--rw-rw-rw-   0        0        0     1168 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice.py
--rw-rw-rw-   0        0        0     1158 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1231 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_options.py
--rw-rw-rw-   0        0        0     1237 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1333 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1323 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      932 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/load_profile_request.py
--rw-rw-rw-   0        0        0      934 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/load_profile_request_py3.py
--rw-rw-rw-   0        0        0     1513 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/os.py
--rw-rw-rw-   0        0        0     1506 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/os_py3.py
--rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice.py
--rw-rw-rw-   0        0        0     1170 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1192 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/preference.py
--rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/preference_py3.py
--rw-rw-rw-   0        0        0     1303 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/problem_response.py
--rw-rw-rw-   0        0        0     1302 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/problem_response_py3.py
--rw-rw-rw-   0        0        0     2958 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_preview.py
--rw-rw-rw-   0        0        0     2904 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_preview_py3.py
--rw-rw-rw-   0        0        0     7042 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_response.py
--rw-rw-rw-   0        0        0     6882 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_response_py3.py
--rw-rw-rw-   0        0        0     1215 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice.py
--rw-rw-rw-   0        0        0     1205 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      921 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/save_profile_request.py
--rw-rw-rw-   0        0        0      923 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/save_profile_request_py3.py
--rw-rw-rw-   0        0        0     1252 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py
--rw-rw-rw-   0        0        0     1247 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1852 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/server.py
--rw-rw-rw-   0        0        0     1837 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/server_py3.py
--rw-rw-rw-   0        0        0     1844 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/status_response.py
--rw-rw-rw-   0        0        0     1871 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/status_response_py3.py
--rw-rw-rw-   0        0        0     1188 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_request.py
--rw-rw-rw-   0        0        0     1173 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_request_py3.py
--rw-rw-rw-   0        0        0     1670 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_response.py
--rw-rw-rw-   0        0        0     1677 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_response_py3.py
--rw-rw-rw-   0        0        0     1302 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice.py
--rw-rw-rw-   0        0        0     1297 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     5691 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/update_profile_request.py
--rw-rw-rw-   0        0        0     5576 2022-02-15 10:59:26.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/update_profile_request_py3.py
--rw-rw-rw-   0        0        0     2067 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/user_info_response.py
--rw-rw-rw-   0        0        0     2057 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/user_info_response_py3.py
--rw-rw-rw-   0        0        0     1831 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_driver_settings.py
--rw-rw-rw-   0        0        0     1841 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_driver_settings_py3.py
--rw-rw-rw-   0        0        0     1327 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_options.py
--rw-rw-rw-   0        0        0     1331 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1293 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1283 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1013 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_options.py
--rw-rw-rw-   0        0        0     1022 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1265 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1255 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      343 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.6.0/kameleo/local_api_client/version.py
-drwxrwxrwx   0        0        0        0 2022-02-18 09:11:30.365014 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/
--rw-rw-rw-   0        0        0     9536 2022-02-18 09:11:29.000000 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4746 2022-02-18 09:11:29.000000 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-18 09:11:29.000000 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-02-18 09:11:29.000000 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-02-18 09:11:29.000000 kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-18 09:11:30.548022 kameleo.local_api_client-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1016 2022-01-27 14:44:09.000000 kameleo.local_api_client-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.583867 kameleo.local_api_client-2.9.0/
+-rw-rw-rw-   0        0        0     1100 2021-07-21 14:14:28.000000 kameleo.local_api_client-2.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9589 2022-08-19 09:54:29.582892 kameleo.local_api_client-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9023 2022-08-19 09:48:42.000000 kameleo.local_api_client-2.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.428869 kameleo.local_api_client-2.9.0/kameleo/
+-rw-rw-rw-   0        0        0       57 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.443895 kameleo.local_api_client-2.9.0/kameleo/local_api_client/
+-rw-rw-rw-   0        0        0      479 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/__init__.py
+-rw-rw-rw-   0        0        0    12918 2022-08-19 09:33:39.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/builder_for_create_profile.py
+-rw-rw-rw-   0        0        0    48266 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/kameleo_local_api_client.py
+drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.580873 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/
+-rw-rw-rw-   0        0        0     6325 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/__init__.py
+-rw-rw-rw-   0        0        0     3065 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile.py
+-rw-rw-rw-   0        0        0     2048 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview.py
+-rw-rw-rw-   0        0        0     2004 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview_py3.py
+-rw-rw-rw-   0        0        0     2988 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_py3.py
+-rw-rw-rw-   0        0        0     2125 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters.py
+-rw-rw-rw-   0        0        0     2112 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters_py3.py
+-rw-rw-rw-   0        0        0     1383 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser.py
+-rw-rw-rw-   0        0        0     5149 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie.py
+-rw-rw-rw-   0        0        0     5118 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie_py3.py
+-rw-rw-rw-   0        0        0     1374 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_py3.py
+-rw-rw-rw-   0        0        0     4298 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request.py
+-rw-rw-rw-   0        0        0     4287 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request_py3.py
+-rw-rw-rw-   0        0        0     5865 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request.py
+-rw-rw-rw-   0        0        0     5757 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request_py3.py
+-rw-rw-rw-   0        0        0     1092 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device.py
+-rw-rw-rw-   0        0        0     1090 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device_py3.py
+-rw-rw-rw-   0        0        0     1168 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1158 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0     1231 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options.py
+-rw-rw-rw-   0        0        0     1237 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options_py3.py
+-rw-rw-rw-   0        0        0     1333 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1323 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0      932 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request.py
+-rw-rw-rw-   0        0        0      934 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request_py3.py
+-rw-rw-rw-   0        0        0     1513 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os.py
+-rw-rw-rw-   0        0        0     1506 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os_py3.py
+-rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1170 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0     1192 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference.py
+-rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference_py3.py
+-rw-rw-rw-   0        0        0     1303 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response.py
+-rw-rw-rw-   0        0        0     1302 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response_py3.py
+-rw-rw-rw-   0        0        0     2958 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview.py
+-rw-rw-rw-   0        0        0     2904 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview_py3.py
+-rw-rw-rw-   0        0        0     7042 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response.py
+-rw-rw-rw-   0        0        0     6882 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response_py3.py
+-rw-rw-rw-   0        0        0     1215 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1205 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0      921 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request.py
+-rw-rw-rw-   0        0        0      923 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request_py3.py
+-rw-rw-rw-   0        0        0     1252 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1247 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0     1852 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server.py
+-rw-rw-rw-   0        0        0     1837 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server_py3.py
+-rw-rw-rw-   0        0        0     1844 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response.py
+-rw-rw-rw-   0        0        0     1871 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response_py3.py
+-rw-rw-rw-   0        0        0     1188 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request.py
+-rw-rw-rw-   0        0        0     1173 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request_py3.py
+-rw-rw-rw-   0        0        0     1670 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response.py
+-rw-rw-rw-   0        0        0     1677 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response_py3.py
+-rw-rw-rw-   0        0        0     1302 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1297 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0     5691 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request.py
+-rw-rw-rw-   0        0        0     5576 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request_py3.py
+-rw-rw-rw-   0        0        0     2067 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response.py
+-rw-rw-rw-   0        0        0     2057 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response_py3.py
+-rw-rw-rw-   0        0        0     1831 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings.py
+-rw-rw-rw-   0        0        0     1841 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings_py3.py
+-rw-rw-rw-   0        0        0     1327 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options.py
+-rw-rw-rw-   0        0        0     1331 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options_py3.py
+-rw-rw-rw-   0        0        0     1293 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1283 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0     1013 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options.py
+-rw-rw-rw-   0        0        0     1022 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options_py3.py
+-rw-rw-rw-   0        0        0     1265 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice.py
+-rw-rw-rw-   0        0        0     1255 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3.py
+-rw-rw-rw-   0        0        0      343 2022-08-19 09:53:43.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/version.py
+drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.436894 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/
+-rw-rw-rw-   0        0        0     9589 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4746 2022-08-19 09:54:29.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-19 09:54:29.584880 kameleo.local_api_client-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/setup.py
```

### Comparing `kameleo.local_api_client-2.6.0/LICENSE.txt` & `kameleo.local_api_client-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/PKG-INFO` & `kameleo.local_api_client-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kameleo.local_api_client
-Version: 2.6.0
+Version: 2.9.0
 Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
 Home-page: https://github.com/kameleo-io/local-api-client-python
 Author: Kameleo Team
 Author-email: support@kameleo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/kameleo-io/local-api-client-python/HEAD/docs/kameleo-logo.png" width="150" align="right" />
 
 # Kameleo Local API Client
-With [Kameleo](https://kameleo.io), you can easily crate multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
+With [Kameleo](https://kameleo.io), you can easily create multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
 
 
 # Features
 - Stay completely undetected, so websites wonâ€™t be able to detect that you are using automation tools
 - Start unlimited number of profiles with different natural browser fingerprints
 - Use authenticated HTTP/SOCKS/SSH proxies in browsers
 - Create isolated browsing environments simultaneously
@@ -154,21 +154,23 @@
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
-    browser = playwright.firefox.launch(
-        # The Playwright framework is not designed to connect to already running 
-        # browsers. To overcome this limitation, a tool bundled with Kameleo, named 
-        # pw-bridge.exe will bridge the communication gap between the running Firefox 
+    browser = playwright.firefox.launch_persistent_context(
+        '',
+        # The Playwright framework is not designed to connect to already running
+        # browsers. To overcome this limitation, a tool bundled with Kameleo, named
+        # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>>\\pw-bridge.exe',
-        args=[f'-target {browser_ws_endpoint}'])
+        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        args=[f'-target {browser_ws_endpoint}'],
+        viewport=None)
     
     # Kameleo will open the a new page in the default browser context.
     # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
```

### Comparing `kameleo.local_api_client-2.6.0/README.md` & `kameleo.local_api_client-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <img src="https://raw.githubusercontent.com/kameleo-io/local-api-client-python/HEAD/docs/kameleo-logo.png" width="150" align="right" />
 
 # Kameleo Local API Client
-With [Kameleo](https://kameleo.io), you can easily crate multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
+With [Kameleo](https://kameleo.io), you can easily create multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
 
 
 # Features
 - Stay completely undetected, so websites won’t be able to detect that you are using automation tools
 - Start unlimited number of profiles with different natural browser fingerprints
 - Use authenticated HTTP/SOCKS/SSH proxies in browsers
 - Create isolated browsing environments simultaneously
@@ -139,21 +139,23 @@
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
-    browser = playwright.firefox.launch(
-        # The Playwright framework is not designed to connect to already running 
-        # browsers. To overcome this limitation, a tool bundled with Kameleo, named 
-        # pw-bridge.exe will bridge the communication gap between the running Firefox 
+    browser = playwright.firefox.launch_persistent_context(
+        '',
+        # The Playwright framework is not designed to connect to already running
+        # browsers. To overcome this limitation, a tool bundled with Kameleo, named
+        # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>>\\pw-bridge.exe',
-        args=[f'-target {browser_ws_endpoint}'])
+        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        args=[f'-target {browser_ws_endpoint}'],
+        viewport=None)
     
     # Kameleo will open the a new page in the default browser context.
     # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
```

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/builder_for_create_profile.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/builder_for_create_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,17 @@
         """
         self.profile_request.launcher = browser_launcher
         return self
 
     def set_recommended_defaults(self):
         """This sets all the profile options to the defaults recommended by Kameleo Team. Please consider providing Proxy settings to your profile.
         """
-        self.profile_request.canvas = "noise"
-        self.profile_request.webgl.value = "noise"
-        self.profile_request.audio = "noise"
+        self.profile_request.canvas = "intelligent"
+        self.profile_request.webgl.value = "off"
+        self.profile_request.audio = "off"
         self.profile_request.timezone.value = "automatic"
         self.profile_request.geolocation.value = "automatic"
         self.profile_request.web_rtc.value = "automatic"
         self.profile_request.fonts.value = "enabled"
         self.profile_request.plugins.value = "enabled"
         self.profile_request.screen.value = "automatic"
         self.profile_request.launcher = "automatic"
```

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/kameleo_local_api_client.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/kameleo_local_api_client.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/__init__.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_preview.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_preview_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_search_parameters.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/base_profile_search_parameters_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_cookie.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_cookie_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/browser_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/cookie_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/cookie_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/create_profile_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/create_profile_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/device.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/device_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_options.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_options_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/load_profile_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/load_profile_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/os.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/os_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/preference.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/preference_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/problem_response.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/problem_response_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_preview.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_preview_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_response.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/profile_response_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/save_profile_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/save_profile_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/server.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/server_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/status_response.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/status_response_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_response.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/test_proxy_response_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/update_profile_request.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/update_profile_request_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/user_info_response.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/user_info_response_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_driver_settings.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_driver_settings_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_options.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_options_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_options.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_options_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3.py` & `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3.py`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/PKG-INFO` & `kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kameleo.local-api-client
-Version: 2.6.0
+Version: 2.9.0
 Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
 Home-page: https://github.com/kameleo-io/local-api-client-python
 Author: Kameleo Team
 Author-email: support@kameleo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <img src="https://raw.githubusercontent.com/kameleo-io/local-api-client-python/HEAD/docs/kameleo-logo.png" width="150" align="right" />
 
 # Kameleo Local API Client
-With [Kameleo](https://kameleo.io), you can easily crate multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
+With [Kameleo](https://kameleo.io), you can easily create multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
 
 
 # Features
 - Stay completely undetected, so websites wonâ€™t be able to detect that you are using automation tools
 - Start unlimited number of profiles with different natural browser fingerprints
 - Use authenticated HTTP/SOCKS/SSH proxies in browsers
 - Create isolated browsing environments simultaneously
@@ -154,21 +154,23 @@
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
-    browser = playwright.firefox.launch(
-        # The Playwright framework is not designed to connect to already running 
-        # browsers. To overcome this limitation, a tool bundled with Kameleo, named 
-        # pw-bridge.exe will bridge the communication gap between the running Firefox 
+    browser = playwright.firefox.launch_persistent_context(
+        '',
+        # The Playwright framework is not designed to connect to already running
+        # browsers. To overcome this limitation, a tool bundled with Kameleo, named
+        # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>>\\pw-bridge.exe',
-        args=[f'-target {browser_ws_endpoint}'])
+        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        args=[f'-target {browser_ws_endpoint}'],
+        viewport=None)
     
     # Kameleo will open the a new page in the default browser context.
     # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
```

### Comparing `kameleo.local_api_client-2.6.0/kameleo.local_api_client.egg-info/SOURCES.txt` & `kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.6.0/setup.py` & `kameleo.local_api_client-2.9.0/setup.py`

 * *Files identical despite different names*

