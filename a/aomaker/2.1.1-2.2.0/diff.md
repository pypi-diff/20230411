# Comparing `tmp/aomaker-2.1.1.tar.gz` & `tmp/aomaker-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.1.1.tar", last modified: Mon Mar 27 16:06:24 2023, max compression
+gzip compressed data, was "aomaker-2.2.0.tar", last modified: Tue Apr 11 14:14:48 2023, max compression
```

## Comparing `aomaker-2.1.1.tar` & `aomaker-2.2.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.925457 aomaker-2.1.1/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.1.1/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       37 2022-11-30 11:05:04.000000 aomaker-2.1.1/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-03-27 16:06:24.925311 aomaker-2.1.1/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.1.1/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.911973 aomaker-2.1.1/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-03-27 16:05:52.000000 aomaker-2.1.1/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      762 2023-03-23 05:16:42.000000 aomaker-2.1.1/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7361 2023-03-22 16:30:41.000000 aomaker-2.1.1/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.919200 aomaker-2.1.1/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4394 2023-02-21 07:52:13.000000 aomaker-2.1.1/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5839 2023-03-27 15:57:34.000000 aomaker-2.1.1/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.1.1/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.920473 aomaker-2.1.1/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.1.1/aomaker/database/base_db.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.1.1/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.920597 aomaker-2.1.1/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.920881 aomaker-2.1.1/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.1.1/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.921664 aomaker-2.1.1/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.1.1/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/extension/recording/recording.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3000 2023-03-23 05:16:42.000000 aomaker-2.1.1/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.1.1/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.922758 aomaker-2.1.1/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.1.1/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.1.1/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2022-12-22 09:57:22.000000 aomaker-2.1.1/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.1.1/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.1.1/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3002 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8774 2023-03-23 05:16:42.000000 aomaker-2.1.1/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8514 2023-03-27 15:57:34.000000 aomaker-2.1.1/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.923925 aomaker-2.1.1/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.924771 aomaker-2.1.1/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9343 2023-02-01 03:18:54.000000 aomaker-2.1.1/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.1.1/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.1.1/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-03-27 16:06:24.918097 aomaker-2.1.1/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1309 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-03-27 16:06:24.000000 aomaker-2.1.1/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-03-27 16:06:24.925539 aomaker-2.1.1/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-03-27 16:05:52.000000 aomaker-2.1.1/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.484575 aomaker-2.2.0/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.0/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       37 2022-11-30 11:05:04.000000 aomaker-2.2.0/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-11 14:14:48.484382 aomaker-2.2.0/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.0/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.478322 aomaker-2.2.0/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-04-09 15:54:39.000000 aomaker-2.2.0/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9297 2023-04-10 15:50:41.000000 aomaker-2.2.0/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.0/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.0/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.479573 aomaker-2.2.0/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.0/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.0/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.0/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480404 aomaker-2.2.0/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.0/aomaker/database/base_db.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.0/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480537 aomaker-2.2.0/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480846 aomaker-2.2.0/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.0/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.481401 aomaker-2.2.0/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.0/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/recording/recording.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3000 2023-03-23 05:16:42.000000 aomaker-2.2.0/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.0/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.482295 aomaker-2.2.0/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.0/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.0/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3002 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8814 2023-04-10 03:38:53.000000 aomaker-2.2.0/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.0/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.483012 aomaker-2.2.0/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.483874 aomaker-2.2.0/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9343 2023-02-01 03:18:54.000000 aomaker-2.2.0/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.0/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.479056 aomaker-2.2.0/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1329 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-04-11 14:14:48.484629 aomaker-2.2.0/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-04-09 15:54:39.000000 aomaker-2.2.0/setup.py
```

### Comparing `aomaker-2.1.1/LICENSE` & `aomaker-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/PKG-INFO` & `aomaker-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.1.1
+Version: 2.2.0
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.1.1/README.md` & `aomaker-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/__init__.py` & `aomaker-2.2.0/aomaker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.1.1/aomaker/_constants.py` & `aomaker-2.2.0/aomaker/_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     DB_NAME = "aomaker.db"
     CONFIG_TABLE = 'config'
     CACHE_TABLE = 'cache'
     SCHEMA_TABLE = 'schema'
     CACHE_VAR_NAME = 'var_name'
     CACHE_RESPONSE = 'response'
     CACHE_WORKER = 'worker'
+    CACHE_API_INFO = 'api_info'
     CONFIG_KEY = 'key'
     CONFIG_VALUE = 'value'
     SCHEMA_API_NAME = 'api_name'
     SCHEMA_SCHEMA = 'schema'
 
 
 # log
```

### Comparing `aomaker-2.1.1/aomaker/_log.py` & `aomaker-2.2.0/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/aomaker.py` & `aomaker-2.2.0/aomaker/_aomaker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # --coding:utf-8--
+import json
 import os
-from typing import List, Dict, Callable, Text
+import importlib
+from typing import List, Dict, Callable, Text, Tuple
 from functools import wraps
 
 import yaml
 import click
 from jsonpath import jsonpath
 from genson import SchemaBuilder
 
-from aomaker.cache import Cache
+from aomaker.cache import cache
 from aomaker.log import logger
 from aomaker.path import BASEDIR
 from aomaker.exceptions import FileNotFound, YamlKeyError
 from aomaker.hook_manager import _cli_hook, _session_hook
 
 
 def dependence(dependent_api: Callable or str, var_name: Text, imp_module=None, *out_args, **out_kwargs):
@@ -29,47 +31,19 @@
     :return:
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             api_name = func.__name__
-            cache = Cache()
-            # 1.先判断是否调用过依赖
             if not cache.get(var_name):
-
-                # 2.调用依赖
-                if isinstance(dependent_api, str):
-                    # 同一个类下的接口
-                    class_, method_ = _parse_dependent_api(dependent_api)
-                    try:
-                        exec(f'from {imp_module} import {class_}')
-                    except ModuleNotFoundError as mne:
-                        logger.error(f"导入模块{imp_module}未找到，请确保imp_module传入参数正确")
-                        raise mne
-                    except ImportError as ie:
-                        logger.error(f"导入ao对象错误：{class_}，请确保dependence传入参数正确")
-                        raise ie
-                    except SyntaxError as se:
-                        logger.error(f"dependence传入imp_module参数错误，imp_module={imp_module} ")
-                        raise se
-                    depend_api_name = eval(f"{class_}.{method_}.__name__")
-                    logger.info(f"==========<{api_name}>前置依赖<{depend_api_name}>执行==========")
-                    try:
-                        res = eval(f'{class_}.{method_}(*{out_args},**{out_kwargs})')
-                    except TypeError as te:
-                        logger.error(f"dependence参数传递错误，错误参数：{dependent_api}")
-                        raise te
-                else:
-                    # 不同类下的接口
-                    depend_api_name = dependent_api.__name__
-                    logger.info(f"==========<{api_name}>前置依赖<{depend_api_name}>执行==========")
-                    res = dependent_api(*out_args, **out_kwargs)
-                # 3.存储响应结果
-                cache.set(var_name, res)
+                dependence_res, depend_api_info = _call_dependence(dependent_api, api_name, imp_module=imp_module,
+                                                                   *out_args, **out_kwargs)
+                depend_api_name = depend_api_info.get("name")
+                cache.set(var_name, dependence_res, api_info=depend_api_info)
 
                 logger.info(f"==========存储全局变量{var_name}完成==========")
                 logger.info(f"==========<{api_name}>前置依赖<{depend_api_name}>结束==========")
             else:
                 logger.info(
                     f"==========<{api_name}>前置依赖已被调用过，本次不再调用,依赖参数{var_name}直接从cache表中读取==========")
             r = func(*args, **kwargs)
@@ -110,14 +84,33 @@
             return r
 
         return wrapper
 
     return decorator
 
 
+def update(var_name: Text, *out_args, **out_kwargs):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            resp = func(*args, **kwargs)
+            api_name = func.__name__
+            if cache.get(var_name):
+                logger.info(f"==========cache变量<{var_name}>开始更新==========")
+                api_info = cache.get(var_name, select_field="api_info")
+                dependence_res = _call_dependence_for_update(json.loads(api_info), *out_args, **out_kwargs)
+                cache.update(var_name, dependence_res)
+                logger.info(f"==========<{api_name}>cache更新<{api_info.get('name')}>结束==========")
+            return resp
+
+        return wrapper
+
+    return decorator
+
+
 def command(name, **out_kwargs):
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             from aomaker.cli import main, OptionHandler
             cmd = main.get_command(None, 'run')
             option_handler = OptionHandler()
@@ -169,14 +162,60 @@
     """
     builder = SchemaBuilder()
     builder.add_object(data)
     to_schema = builder.to_schema()
     return to_schema
 
 
+def _call_dependence(dependent_api: Callable or Text, api_name: Text, imp_module, *out_args,
+                     **out_kwargs) -> Tuple:
+    if isinstance(dependent_api, str):
+        # 同一个类下的接口
+        class_, method_ = _parse_dependent_api(dependent_api)
+        try:
+            exec(f'from {imp_module} import {class_}')
+        except ModuleNotFoundError as mne:
+            logger.error(f"导入模块{imp_module}未找到，请确保imp_module传入参数正确")
+            raise mne
+        except ImportError as ie:
+            logger.error(f"导入ao对象错误：{class_}，请确保dependence传入参数正确")
+            raise ie
+        except SyntaxError as se:
+            logger.error(f"dependence传入imp_module参数错误，imp_module={imp_module} ")
+            raise se
+        depend_api_name = eval(f"{class_}.{method_}.__name__")
+        logger.info(f"==========<{api_name}>前置依赖<{depend_api_name}>执行==========")
+        try:
+            res = eval(f'{class_}.{method_}(*{out_args},**{out_kwargs})')
+        except TypeError as te:
+            logger.error(f"dependence参数传递错误，错误参数：{dependent_api}")
+            raise te
+        depend_api_info = {"name": method_, "module": imp_module, "ao": class_.lower()}
+    else:
+        # 不同类下的接口
+        depend_api_name = dependent_api.__name__
+        logger.info(f"==========<{api_name}>前置依赖<{depend_api_name}>执行==========")
+        res = dependent_api(*out_args, **out_kwargs)
+        depend_api_info = {"name": depend_api_name, "module": _get_module_name_by_method_obj(dependent_api),
+                           "ao": type(dependent_api.__self__).__name__.lower()}
+    return res, depend_api_info
+
+
+def _call_dependence_for_update(api_info: Dict, *out_args, **out_kwargs) -> Dict:
+    api_name = api_info.get("name")
+    api_module = api_info.get("module")
+    module = importlib.import_module(api_module)
+    try:
+        ao = getattr(module, api_info.get("ao"))
+    except AttributeError as e:
+        logger.error(f"在{api_module}中未找到ao对象<{api_info.get('ao')}>！")
+        raise e
+    res = getattr(ao, api_name)(*out_args, **out_kwargs)
+    return res
+
 
 def _extract_by_jsonpath(source: Text, jsonpath_expr: Text, index: int):
     target = jsonpath(source, jsonpath_expr)[index]
     return target
 
 
 def _parse_dependent_api(dependent_api):
@@ -191,10 +230,22 @@
 
 def _load_yaml(yaml_file):
     with open(yaml_file, encoding='utf-8') as f:
         yaml_testcase = yaml.safe_load(f)
     return yaml_testcase
 
 
+def _get_module_name_by_method_obj(method_obj) -> Text:
+    """
+    return: x.y.z
+    """
+    module_name = method_obj.__module__
+    module_path = importlib.import_module(module_name).__file__
+    cur_dir = os.path.abspath('.')
+    rel_path = os.path.relpath(module_path, cur_dir)
+    module_name = os.path.splitext(rel_path)[0].replace(os.path.sep, '.')
+    return module_name
+
+
 if __name__ == '__main__':
     x = data_maker('aomaker/data/api_data/job.yaml', 'job', 'submit_job')
     print(x)
```

### Comparing `aomaker-2.1.1/aomaker/base/base_api.py` & `aomaker-2.2.0/aomaker/base/base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import allure
 import requests
 from json.decoder import JSONDecodeError
 
 from aomaker.log import logger
 from aomaker.cache import Config, Cache, Schema
-from aomaker.aomaker import genson
+from aomaker._aomaker import genson
 from aomaker.exceptions import HttpRequestError
 
 
 def request(func):
     def wrapper(*args, **kwargs):
         conf = Config()
         cache = Cache()
```

### Comparing `aomaker-2.1.1/aomaker/base/base_testcase.py` & `aomaker-2.2.0/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/cache.py` & `aomaker-2.2.0/aomaker/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,39 +109,43 @@
 
 
 class Cache(SQLiteDB):
     def __init__(self):
         super(Cache, self).__init__()
         self.table = DataBase.CACHE_TABLE
 
-    def set(self, key: str, value):
+    def set(self, key: str, value, api_info=None):
         sql = f"""insert into {self.table} (var_name,response,worker) values (:key,:value,:worker)"""
         worker = _get_worker()
         if self.get(key) is not None:
             logger.debug(f"缓存插入重复数据, key:{key}，worker:{worker}，已被忽略！")
             return
         try:
-            self.execute_sql(sql, (key, json.dumps(value), worker))
+            if api_info:
+                sql = f"""insert into {self.table} (var_name,response,worker,api_info) values (:key,:value,:worker,:api_info)"""
+                self.execute_sql(sql, (key, json.dumps(value), worker, json.dumps(api_info)))
+            else:
+                self.execute_sql(sql, (key, json.dumps(value), worker))
         except sqlite3.IntegrityError as e:
             raise e
 
     def update(self, key, value):
         key_value = {"response": json.dumps(value)}
         worker = _get_worker()
         condition = {"worker": worker, "var_name": key}
         self.update_data(self.table, key_value, where=condition)
-        logger.info(f"缓存数据更新完成, 表：{self.table}, var_name: {key}, response: {value}, worker: {worker}")
+        logger.info(f"缓存数据更新完成, 表：{self.table},\n var_name: {key},\n response: {value},\n worker: {worker}")
 
-    def get(self, key: str):
+    def get(self, key: str, select_field="response"):
         worker = _get_worker()
         if key == "headers":
-            sql = f"""select response from {self.table} where var_name=:key"""
+            sql = f"""select {select_field} from {self.table} where var_name=:key"""
             query_res = self.query_sql(sql, (key,))
         else:
-            sql = f"""select response from {self.table} where var_name=:key and worker=:worker"""
+            sql = f"""select {select_field} from {self.table} where var_name=:key and worker=:worker"""
             query_res = self.query_sql(sql, (key, worker))
         try:
             res = query_res[0][0]
         except IndexError:
             return None
         res = json.loads(res)
```

### Comparing `aomaker-2.1.1/aomaker/cli.py` & `aomaker-2.2.0/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/database/base_db.py` & `aomaker-2.2.0/aomaker/database/base_db.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/database/mysql.py` & `aomaker-2.2.0/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/database/sqlite.py` & `aomaker-2.2.0/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/exceptions.py` & `aomaker-2.2.0/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/extension/har_parse/__init__.py` & `aomaker-2.2.0/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.2.0/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/extension/recording/__init__.py` & `aomaker-2.2.0/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/extension/recording/recording.py` & `aomaker-2.2.0/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/field.py` & `aomaker-2.2.0/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/fixture.py` & `aomaker-2.2.0/aomaker/fixture.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/hook_manager.py` & `aomaker-2.2.0/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/html/heading.html` & `aomaker-2.2.0/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/html/report.html` & `aomaker-2.2.0/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/html/template.html` & `aomaker-2.2.0/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/log.py` & `aomaker-2.2.0/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/make.py` & `aomaker-2.2.0/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/make_api.py` & `aomaker-2.2.0/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/make_testcase.py` & `aomaker-2.2.0/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/models.py` & `aomaker-2.2.0/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/path.py` & `aomaker-2.2.0/aomaker/path.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/report.py` & `aomaker-2.2.0/aomaker/report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/runner.py` & `aomaker-2.2.0/aomaker/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         # 前置
         logger.info(emojize(
             '******************************:puzzle_piece: 开始初始化环境 :puzzle_piece:******************************'))
         method_of_class_name = func.__qualname__.split('.')[0]
         config.set("run_mode", RUN_MODE[method_of_class_name])
         SetUpSession(login).set_session_vars()
         shutil.rmtree(allure_json_dir, ignore_errors=True)
-        _cli_hook.run()
+        if _cli_hook.custom_kwargs:
+            _cli_hook.run()
         _session_hook.run()
         logger.info(emojize(
             '*****************:beer_mug: 环境初始化完成，所有全局配置已加载到config表 :beer_mug:*****************'))
         r = func(*args, **kwargs)
         TearDownSession().clear_env()
         return r
```

### Comparing `aomaker-2.1.1/aomaker/scaffold.py` & `aomaker-2.2.0/aomaker/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         logger.info(msg)
 
     def create_table(db_object, table_name: str):
         table_attr = get_table_attribute(table_name)
         key = table_attr.get('key')
         value = table_attr.get('value')
         worker = table_attr.get('worker')
+        api_info = table_attr.get('api_info')
         if worker is not None:
-            sql = f"""create table {table_name}({key} text,{value} text,{worker} text);"""
+            sql = f"""create table {table_name}({key} text,{value} text,{worker} text,{api_info} text);"""
         else:
             sql = f"""create table {table_name}({key} text,{value} text);"""
         db_object.execute_sql(sql)
         if table_name != "cache":
             sql2 = f"""create unique index {table_name}_{key}_uindex on {table_name} ({key});"""
             db_object.execute_sql(sql2)
         msg = f"创建数据表：{table_name}"
```

### Comparing `aomaker-2.1.1/aomaker/send_msg/wechat.py` & `aomaker-2.2.0/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/swagger2yaml.py` & `aomaker-2.2.0/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/template.py` & `aomaker-2.2.0/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/utils/gen_allure_report.py` & `aomaker-2.2.0/aomaker/utils/gen_allure_report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/utils/utils.py` & `aomaker-2.2.0/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker/yaml2case.py` & `aomaker-2.2.0/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.1.1/aomaker.egg-info/PKG-INFO` & `aomaker-2.2.0/aomaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.1.1
+Version: 2.2.0
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.1.1/aomaker.egg-info/SOURCES.txt` & `aomaker-2.2.0/aomaker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 aomaker/__init__.py
+aomaker/_aomaker.py
 aomaker/_constants.py
 aomaker/_log.py
 aomaker/aomaker.py
 aomaker/cache.py
 aomaker/cli.py
 aomaker/exceptions.py
 aomaker/field.py
```

### Comparing `aomaker-2.1.1/setup.py` & `aomaker-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.1.1",
+    version="2.2.0",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
```

