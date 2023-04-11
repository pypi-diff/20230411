# Comparing `tmp/tatarubot2-0.1.7.tar.gz` & `tmp/tatarubot2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tatarubot2-0.1.7.tar", max compression
+gzip compressed data, was "tatarubot2-0.1.8.tar", max compression
```

## Comparing `tatarubot2-0.1.7.tar` & `tatarubot2-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.7/LICENSE
--rw-r--r--   0        0        0     3600 2023-04-10 16:38:02.000000 tatarubot2-0.1.7/README_PIP.md
--rw-r--r--   0        0        0      420 2023-04-10 16:38:02.000000 tatarubot2-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.7/tatarubot2/__init__.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.7/tatarubot2/data/boss.json
--rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.7/tatarubot2/data/item_dict.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.7/tatarubot2/data/job.json
--rw-r--r--   0        0        0     1680 2023-04-10 15:34:49.000000 tatarubot2-0.1.7/tatarubot2/plugins/__init__.py
--rw-r--r--   0        0        0     1084 2023-04-10 15:35:48.501998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     1759 2023-04-10 15:35:49.525995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/bot_help.cpython-37.pyc
--rw-r--r--   0        0        0     1259 2023-04-10 15:42:09.704827 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/chat_ai.cpython-37.pyc
--rw-r--r--   0        0        0     1878 2023-04-10 15:35:48.501998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/ff_weibo.cpython-37.pyc
--rw-r--r--   0        0        0     4186 2023-04-10 15:35:48.565998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/house.cpython-37.pyc
--rw-r--r--   0        0        0    11706 2023-04-10 15:35:48.629998 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item.cpython-37.pyc
--rw-r--r--   0        0        0    11717 2023-04-10 15:35:48.697997 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item_new.cpython-37.pyc
--rw-r--r--   0        0        0     6049 2023-04-10 15:35:48.985997 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/logs_dps.cpython-37.pyc
--rw-r--r--   0        0        0     1298 2023-04-10 15:35:49.049996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/lottery.cpython-37.pyc
--rw-r--r--   0        0        0     6464 2023-04-10 15:35:49.113996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market.cpython-37.pyc
--rw-r--r--   0        0        0     6614 2023-04-10 15:35:49.177996 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market_new.cpython-37.pyc
--rw-r--r--   0        0        0     2737 2023-04-10 15:35:49.401995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/nuannuan.cpython-37.pyc
--rw-r--r--   0        0        0     1167 2023-04-10 15:35:49.465995 tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/precious.cpython-37.pyc
--rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.7/tatarubot2/plugins/auto_response.py
--rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/plugins/bot_help.py
--rw-r--r--   0        0        0     1249 2023-04-10 15:47:26.000000 tatarubot2-0.1.7/tatarubot2/plugins/chat_ai.py
--rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.7/tatarubot2/plugins/ff_weibo.py
--rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/house.py
--rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.7/tatarubot2/plugins/item.py
--rw-r--r--   0        0        0    17442 2023-04-10 14:32:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/item_new.py
--rw-r--r--   0        0        0     7150 2023-04-10 14:58:41.000000 tatarubot2-0.1.7/tatarubot2/plugins/logs_dps.py
--rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.7/tatarubot2/plugins/lottery.py
--rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.7/tatarubot2/plugins/market.py
--rw-r--r--   0        0        0     8327 2023-04-10 14:32:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/market_new.py
--rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.7/tatarubot2/plugins/nuannuan.py
--rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.7/tatarubot2/plugins/precious.py
--rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.7/tatarubot2/plugins/weather.py
--rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.7/tatarubot2/tools/__init__.py
--rw-r--r--   0        0        0      117 2023-04-10 15:35:49.585995 tatarubot2-0.1.7/tatarubot2/tools/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.7/tatarubot2/tools/data.json
--rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/tools/download_boss.py
--rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.7/tatarubot2/tools/download_item2id.py
--rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.7/tatarubot2/tools/new_boss.json
--rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.7/tatarubot2/tools/new_job.json
--rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.7/tatarubot2/tools/normal_data.py
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 tatarubot2-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-08-12 03:44:26.000000 tatarubot2-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3600 2023-04-10 16:38:02.000000 tatarubot2-0.1.8/README_PIP.md
+-rw-r--r--   0        0        0      449 2023-04-11 01:38:50.000000 tatarubot2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-10 10:03:09.000000 tatarubot2-0.1.8/tatarubot2/__init__.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.8/tatarubot2/data/boss.json
+-rw-r--r--   0        0        0  1218488 2023-01-30 01:23:59.000000 tatarubot2-0.1.8/tatarubot2/data/item_dict.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:14:52.000000 tatarubot2-0.1.8/tatarubot2/data/job.json
+-rw-r--r--   0        0        0     1680 2023-04-10 15:34:49.000000 tatarubot2-0.1.8/tatarubot2/plugins/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-10 15:35:48.501998 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     1759 2023-04-10 15:35:49.525995 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/bot_help.cpython-37.pyc
+-rw-r--r--   0        0        0     1259 2023-04-10 15:42:09.704827 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/chat_ai.cpython-37.pyc
+-rw-r--r--   0        0        0     1878 2023-04-10 15:35:48.501998 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/ff_weibo.cpython-37.pyc
+-rw-r--r--   0        0        0     4186 2023-04-10 15:35:48.565998 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/house.cpython-37.pyc
+-rw-r--r--   0        0        0    11706 2023-04-10 15:35:48.629998 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/item.cpython-37.pyc
+-rw-r--r--   0        0        0    11717 2023-04-10 15:35:48.697997 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/item_new.cpython-37.pyc
+-rw-r--r--   0        0        0     6049 2023-04-10 15:35:48.985997 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/logs_dps.cpython-37.pyc
+-rw-r--r--   0        0        0     1298 2023-04-10 15:35:49.049996 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/lottery.cpython-37.pyc
+-rw-r--r--   0        0        0     6464 2023-04-10 15:35:49.113996 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/market.cpython-37.pyc
+-rw-r--r--   0        0        0     6614 2023-04-10 15:35:49.177996 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/market_new.cpython-37.pyc
+-rw-r--r--   0        0        0     2737 2023-04-10 15:35:49.401995 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/nuannuan.cpython-37.pyc
+-rw-r--r--   0        0        0     1167 2023-04-10 15:35:49.465995 tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/precious.cpython-37.pyc
+-rw-r--r--   0        0        0      713 2022-11-15 08:07:47.000000 tatarubot2-0.1.8/tatarubot2/plugins/auto_response.py
+-rw-r--r--   0        0        0     1627 2023-04-07 06:02:20.000000 tatarubot2-0.1.8/tatarubot2/plugins/bot_help.py
+-rw-r--r--   0        0        0     1249 2023-04-10 15:47:26.000000 tatarubot2-0.1.8/tatarubot2/plugins/chat_ai.py
+-rw-r--r--   0        0        0     2262 2022-08-16 07:15:05.000000 tatarubot2-0.1.8/tatarubot2/plugins/ff_weibo.py
+-rw-r--r--   0        0        0     4409 2022-08-17 03:31:15.000000 tatarubot2-0.1.8/tatarubot2/plugins/house.py
+-rw-r--r--   0        0        0    17045 2023-01-29 07:09:23.000000 tatarubot2-0.1.8/tatarubot2/plugins/item.py
+-rw-r--r--   0        0        0    17442 2023-04-10 14:32:15.000000 tatarubot2-0.1.8/tatarubot2/plugins/item_new.py
+-rw-r--r--   0        0        0     7150 2023-04-10 14:58:41.000000 tatarubot2-0.1.8/tatarubot2/plugins/logs_dps.py
+-rw-r--r--   0        0        0     1230 2022-08-12 01:48:07.000000 tatarubot2-0.1.8/tatarubot2/plugins/lottery.py
+-rw-r--r--   0        0        0     7754 2022-08-15 08:28:24.000000 tatarubot2-0.1.8/tatarubot2/plugins/market.py
+-rw-r--r--   0        0        0     8327 2023-04-10 14:32:15.000000 tatarubot2-0.1.8/tatarubot2/plugins/market_new.py
+-rw-r--r--   0        0        0     3103 2022-09-24 04:17:17.000000 tatarubot2-0.1.8/tatarubot2/plugins/nuannuan.py
+-rw-r--r--   0        0        0      899 2022-08-12 01:48:15.000000 tatarubot2-0.1.8/tatarubot2/plugins/precious.py
+-rw-r--r--   0        0        0     1196 2022-06-23 07:26:19.000000 tatarubot2-0.1.8/tatarubot2/plugins/weather.py
+-rw-r--r--   0        0        0        0 2022-08-12 07:58:45.000000 tatarubot2-0.1.8/tatarubot2/tools/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 15:35:49.585995 tatarubot2-0.1.8/tatarubot2/tools/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0  1010264 2022-08-12 20:09:39.000000 tatarubot2-0.1.8/tatarubot2/tools/data.json
+-rw-r--r--   0        0        0     5058 2023-04-07 06:02:20.000000 tatarubot2-0.1.8/tatarubot2/tools/download_boss.py
+-rw-r--r--   0        0        0     1962 2023-01-30 01:23:02.000000 tatarubot2-0.1.8/tatarubot2/tools/download_item2id.py
+-rw-r--r--   0        0        0    82117 2023-01-12 06:12:13.000000 tatarubot2-0.1.8/tatarubot2/tools/new_boss.json
+-rw-r--r--   0        0        0     2422 2022-12-26 09:13:22.000000 tatarubot2-0.1.8/tatarubot2/tools/new_job.json
+-rw-r--r--   0        0        0     1725 2023-04-07 06:02:20.000000 tatarubot2-0.1.8/tatarubot2/tools/normal_data.py
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 tatarubot2-0.1.8/PKG-INFO
```

### Comparing `tatarubot2-0.1.7/LICENSE` & `tatarubot2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/README_PIP.md` & `tatarubot2-0.1.8/README_PIP.md`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/data/boss.json` & `tatarubot2-0.1.8/tatarubot2/data/boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/data/item_dict.json` & `tatarubot2-0.1.8/tatarubot2/data/item_dict.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/data/job.json` & `tatarubot2-0.1.8/tatarubot2/data/job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__init__.py` & `tatarubot2-0.1.8/tatarubot2/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/__init__.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/bot_help.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/bot_help.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/chat_ai.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/chat_ai.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/ff_weibo.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/ff_weibo.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/house.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/house.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/item.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/item_new.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/item_new.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/logs_dps.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/logs_dps.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/lottery.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/lottery.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/market.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/market_new.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/market_new.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/nuannuan.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/nuannuan.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/__pycache__/precious.cpython-37.pyc` & `tatarubot2-0.1.8/tatarubot2/plugins/__pycache__/precious.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/auto_response.py` & `tatarubot2-0.1.8/tatarubot2/plugins/auto_response.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/bot_help.py` & `tatarubot2-0.1.8/tatarubot2/plugins/bot_help.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/chat_ai.py` & `tatarubot2-0.1.8/tatarubot2/plugins/chat_ai.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/ff_weibo.py` & `tatarubot2-0.1.8/tatarubot2/plugins/ff_weibo.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/house.py` & `tatarubot2-0.1.8/tatarubot2/plugins/house.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/item.py` & `tatarubot2-0.1.8/tatarubot2/plugins/item.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/item_new.py` & `tatarubot2-0.1.8/tatarubot2/plugins/item_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/logs_dps.py` & `tatarubot2-0.1.8/tatarubot2/plugins/logs_dps.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/lottery.py` & `tatarubot2-0.1.8/tatarubot2/plugins/lottery.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/market.py` & `tatarubot2-0.1.8/tatarubot2/plugins/market.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/market_new.py` & `tatarubot2-0.1.8/tatarubot2/plugins/market_new.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/nuannuan.py` & `tatarubot2-0.1.8/tatarubot2/plugins/nuannuan.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/precious.py` & `tatarubot2-0.1.8/tatarubot2/plugins/precious.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/plugins/weather.py` & `tatarubot2-0.1.8/tatarubot2/plugins/weather.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/data.json` & `tatarubot2-0.1.8/tatarubot2/tools/data.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/download_boss.py` & `tatarubot2-0.1.8/tatarubot2/tools/download_boss.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/download_item2id.py` & `tatarubot2-0.1.8/tatarubot2/tools/download_item2id.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/new_boss.json` & `tatarubot2-0.1.8/tatarubot2/tools/new_boss.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/new_job.json` & `tatarubot2-0.1.8/tatarubot2/tools/new_job.json`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/tatarubot2/tools/normal_data.py` & `tatarubot2-0.1.8/tatarubot2/tools/normal_data.py`

 * *Files identical despite different names*

### Comparing `tatarubot2-0.1.7/PKG-INFO` & `tatarubot2-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tatarubot2
-Version: 0.1.7
+Version: 0.1.8
 Summary: FF14 bot Tataru
 Author: aaron-li
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # TataruBot2
 
 基于NoneBot2的FF14机器人塔塔露
```

