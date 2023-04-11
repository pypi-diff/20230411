# Comparing `tmp/CrawlersTools-1.4.64.tar.gz` & `tmp/CrawlersTools-1.4.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrawlersTools-1.4.64.tar", last modified: Tue Apr 11 03:51:49 2023, max compression
+gzip compressed data, was "CrawlersTools-1.4.65.tar", last modified: Tue Apr 11 09:01:48 2023, max compression
```

## Comparing `CrawlersTools-1.4.64.tar` & `CrawlersTools-1.4.65.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.727151 CrawlersTools-1.4.64/CrawlersTools/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/attachment_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/content_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/list_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/extractors/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/schemas/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/time_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/title_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/extractors/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/js_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/js_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/js_crawler/font_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/js_crawler/transfer_js.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/pipelines/mongo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/pipelines/mysql_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/pipelines/redis_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.731151 CrawlersTools-1.4.64/CrawlersTools/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/preprocess/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/preprocess/time_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/CrawlersTools/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/projects/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/projects/upload_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/CrawlersTools/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/requests/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/requests/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/requests/random_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/CrawlersTools/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/CrawlersTools/schedules/auto_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:51:49.727151 CrawlersTools-1.4.64/CrawlersTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-11 03:51:49.000000 CrawlersTools-1.4.64/CrawlersTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-11 03:51:49.000000 CrawlersTools-1.4.64/CrawlersTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:51:49.000000 CrawlersTools-1.4.64/CrawlersTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 03:51:49.000000 CrawlersTools-1.4.64/CrawlersTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 03:51:49.000000 CrawlersTools-1.4.64/CrawlersTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 03:51:49.735151 CrawlersTools-1.4.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-11 03:51:40.000000 CrawlersTools-1.4.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.227987 CrawlersTools-1.4.65/CrawlersTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.227987 CrawlersTools-1.4.65/CrawlersTools/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/attachment_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/content_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/list_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.227987 CrawlersTools-1.4.65/CrawlersTools/extractors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/schemas/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/time_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/title_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.231987 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/extractors/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.231987 CrawlersTools-1.4.65/CrawlersTools/js_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/js_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/js_crawler/font_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/js_crawler/transfer_js.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.231987 CrawlersTools-1.4.65/CrawlersTools/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/CrawlersTools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/pipelines/mysql_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/pipelines/redis_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/CrawlersTools/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/preprocess/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/preprocess/time_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/CrawlersTools/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/projects/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/projects/upload_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/CrawlersTools/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/requests/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/requests/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/requests/random_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/CrawlersTools/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/CrawlersTools/schedules/auto_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:01:48.227987 CrawlersTools-1.4.65/CrawlersTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-11 09:01:48.000000 CrawlersTools-1.4.65/CrawlersTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-11 09:01:48.000000 CrawlersTools-1.4.65/CrawlersTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:01:48.000000 CrawlersTools-1.4.65/CrawlersTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-11 09:01:48.000000 CrawlersTools-1.4.65/CrawlersTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 09:01:48.000000 CrawlersTools-1.4.65/CrawlersTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:01:48.235987 CrawlersTools-1.4.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-11 09:01:32.000000 CrawlersTools-1.4.65/setup.py
```

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/__init__.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/attachment_extractor.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/attachment_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/base.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/base.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/content_extractor.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/content_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/list_extractor.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/list_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/schemas/element.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/schemas/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/time_extractor.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/time_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/title_extractor.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/title_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/utils/cluster.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/utils/element.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/utils/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/utils/preprocess.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/utils/settings.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/utils/settings.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/extractors/utils/similarity.py` & `CrawlersTools-1.4.65/CrawlersTools/extractors/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/js_crawler/font_decrypt.py` & `CrawlersTools-1.4.65/CrawlersTools/js_crawler/font_decrypt.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/js_crawler/transfer_js.py` & `CrawlersTools-1.4.65/CrawlersTools/js_crawler/transfer_js.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/logs/log.py` & `CrawlersTools-1.4.65/CrawlersTools/logs/log.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/pipelines/mongo_pipeline.py` & `CrawlersTools-1.4.65/CrawlersTools/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/pipelines/mysql_pipeline.py` & `CrawlersTools-1.4.65/CrawlersTools/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/pipelines/redis_pipeline.py` & `CrawlersTools-1.4.65/CrawlersTools/pipelines/redis_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/preprocess/bloom_filter.py` & `CrawlersTools-1.4.65/CrawlersTools/preprocess/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/preprocess/time_process.py` & `CrawlersTools-1.4.65/CrawlersTools/preprocess/time_process.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/projects/filters.py` & `CrawlersTools-1.4.65/CrawlersTools/projects/filters.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/projects/upload_oss.py` & `CrawlersTools-1.4.65/CrawlersTools/projects/upload_oss.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/requests/base_requests.py` & `CrawlersTools-1.4.65/CrawlersTools/requests/base_requests.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/requests/proxy.py` & `CrawlersTools-1.4.65/CrawlersTools/requests/proxy.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/requests/random_ua.py` & `CrawlersTools-1.4.65/CrawlersTools/requests/random_ua.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/CrawlersTools/schedules/auto_thread.py` & `CrawlersTools-1.4.65/CrawlersTools/schedules/auto_thread.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # -*- coding: utf-8 -*-
 # @Project : CrawlersTools
 # @Time    : 2022/6/21 17:19
 # @Author  : MuggleK
 # @File    : auto_thread.py
 
 import time
+import random
 from inspect import isgenerator
 from threading import Thread, active_count, Lock
 from traceback import format_exc
 
-import vthread as vthread
 from loguru import logger
 
-
 thread_lock = Lock()
 
 
 class ExcThread(Thread):
     """
     主动捕获子线程异常
     """
 
-    def __init__(self, target, args=None, kwargs=None):
+    def __init__(self, target, args=(), kwargs=None):
         super(ExcThread, self).__init__()
         self._target = target
-        self._args = tuple() if args is None else (args, )
-        self._kwargs = kwargs or dict()
+        self._args = args
+        self._kwargs = kwargs if kwargs else {}
 
     def run(self):
         try:
             if self._target:
                 self._target(*self._args, **self._kwargs)
         except:
-            logger.error(f'target：{self._target} args：{self._args} kwargs：{self._kwargs}，{format_exc()}')
+            logger.error(f'args：{self._args} kwargs：{self._kwargs}，{format_exc()}')
 
 
 class AutoThread(object):
     """
     动态线程调度, 传入任务队列可为列表（初始化转换成生成器），也可为生成器
     usage:
         a_thread = AutoThread(20, fun, arg_list)
         a_thread.main_thread()
 
-    ps: 支持三种并发方式：1.并发函数 2.并发传参 3.函数和参数按顺序组合
+    ps: 支持两种并发方式：1.并发函数 2.并发传参
     """
 
     def __init__(self, thread_num: int, fun, arg_list=None):
         self.thread_num = thread_num
+        self.arg = arg_list  # 并发函数需要入参
         self.fun = (f for f in fun) if isinstance(fun, list) else fun
-        self.args = (a for a in arg_list) if isinstance(arg_list, list) else arg_list
+        self.args = (arg for arg in arg_list) if isinstance(arg_list, list) else arg_list
+        self.flag = True if isgenerator(self.fun) else False  # True 并发函数 False并发参数
         self.os_threads = active_count()
 
     def wait(self):
         while active_count() > self.os_threads:
             time.sleep(.25)
 
     @staticmethod
@@ -61,23 +62,32 @@
             task_arg = next(task)
         except StopIteration:
             task_arg = None
 
         return task_arg
 
     def main_thread(self):
-        while True:
-            with thread_lock:
-                active_thread = active_count()
-                if active_thread >= self.thread_num:
-                    time.sleep(.5)
-                    continue
-
-            fun = self.next_task(self.fun) if isgenerator(self.fun) else self.fun
-            if fun is None:
-                break
-            args = self.next_task(self.args) if isgenerator(self.args) else self.args
-            if args is None:
-                break
+        loop_flag = True
+        while loop_flag:
+            active_thread = active_count()
+            if active_count() >= self.thread_num:
+                time.sleep(random.uniform(0, 1))
+                continue
+            for _ in range(self.thread_num - active_thread + self.os_threads):
+                thread_lock.acquire()
+                if self.flag:
+                    task_fun = self.next_task(self.fun)
+                    thread_lock.release()
+                    if task_fun is None:
+                        loop_flag = False
+                        break
+                    child_thread = ExcThread(target=task_fun) if self.arg is None else ExcThread(target=task_fun, args=(
+                        self.arg,))
+                else:
+                    task_arg = self.next_task(self.args)
+                    thread_lock.release()
+                    if task_arg is None:
+                        loop_flag = False
+                        break
+                    child_thread = ExcThread(target=self.fun, args=(task_arg,))
 
-            t = ExcThread(target=fun, args=args)
-            t.start()
+                child_thread.start()
```

### Comparing `CrawlersTools-1.4.64/CrawlersTools.egg-info/PKG-INFO` & `CrawlersTools-1.4.65/CrawlersTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.64
+Version: 1.4.65
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.64/CrawlersTools.egg-info/SOURCES.txt` & `CrawlersTools-1.4.65/CrawlersTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/LICENSE` & `CrawlersTools-1.4.65/LICENSE`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/PKG-INFO` & `CrawlersTools-1.4.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.64
+Version: 1.4.65
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.64/README.md` & `CrawlersTools-1.4.65/README.md`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.64/setup.py` & `CrawlersTools-1.4.65/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CrawlersTools',  # 包名
-    version='1.4.64',  # 版本号
+    version='1.4.65',  # 版本号
     description='Tools for Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MuggleK',
     author_email='peichangchuan@gmail.com',
     url='https://github.com/MuggleK/CrawlersTools',
     install_requires=[
```

