# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.4.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.4.tar` & `nonebot_plugin_blive_danmaku-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.4/LICENSE
--rw-r--r--   0        0        0      127 2023-04-07 18:53:54.995600 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       99 2023-04-10 07:39:11.035690 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/__init__.py
--rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_off.py
--rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_on.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1421 2023-04-09 17:51:35.475589 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0      980 2023-04-09 17:52:09.092145 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2645 2023-04-10 15:15:45.271259 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     2830 2023-04-10 15:01:41.440478 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      950 2023-04-09 16:52:22.392021 nonebot_plugin_blive_danmaku-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2835 2023-04-10 17:47:03.111172 nonebot_plugin_blive_danmaku-0.1.4/README.md
--rw-r--r--   0        0        0     3869 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.5/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-11 03:52:55.075348 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       99 2023-04-10 07:39:11.035690 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/live/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/live/live_off.py
+-rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1421 2023-04-09 17:51:35.475589 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0      980 2023-04-09 17:52:09.092145 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2645 2023-04-10 15:15:45.271259 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     2813 2023-04-11 03:53:05.223905 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      950 2023-04-11 04:02:27.264133 nonebot_plugin_blive_danmaku-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2745 2023-04-11 03:52:55.074335 nonebot_plugin_blive_danmaku-0.1.5/README.md
+-rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_off.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/live/live_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/live/live_on.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/live/live_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Db:
     @classmethod
     async def init(cls):
         config={
             "connections":{"danmaku_bot":f"sqlite://{get_path('danmakuBot.sqlite3')}"},
             "apps":{
                 "danmaku_bot_app":{
-                    "models":["nonebot_plugin_blive_danmaku.database.model", "aerich.models"],
+                    "models":["nonebot_plugin_blive_danmaku.database.model"],
                     "default_connection":"danmaku_bot"
                 }
             }
         }
         await Tortoise.init(config=config)
         await Tortoise.generate_schemas()
         await cls.update_sub_list()
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.5/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.4"
+version = "0.1.5"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/README.md` & `nonebot_plugin_blive_danmaku-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [![pypi](https://img.shields.io/pypi/v/nonebot-plugin-blive-danmaku.svg)](https://pypi.org/project/nonebot-plugin-blive-danmaku/)  ![python](https://img.shields.io/pypi/pyversions/nonebot-plugin-blive-danmaku)  [![license](https://img.shields.io/github/license/zangxx66/nonebot_plugin_blive_danmaku.svg)](https://raw.githubusercontent.com/zangxx66/nonebot_plugin_blive_danmaku/main/LICENSE)  
 
 </div>  
 
 ## 简介  
 - 基于[nonebot2](https://v2.nonebot.dev/)开发的B站直播间弹幕监听插件，参考了Haruka和blivechat的部分代码。  
-- 起源于[哈鹿hallu](https://space.bilibili.com/3493118494116797)的一条动态，苦于做视频时没有人做路灯，翻录播的时候头都大了，说要花钱请个全职路灯，我寻思与其把钱送给别人，不如交给Bot去做路灯。
+- 起源于[哈鹿hallu](https://space.bilibili.com/3493118494116797)的一条动态，苦于做视频时没有人做路灯，翻录播的时候头都大了，说要花钱请个全职路灯，我寻思与其把钱送给别人，不如交给Bot去做路灯。  
 ![](/doc/screenshot1.png)
 - 路灯：指把直播过程中有趣的点记录下来，给剪辑根据记录的时间点和内容做出对应的视频。
 
 ## 功能
 
 - 用弹幕的形式记录直播高能点
 - 弹幕指令为`#路灯`加上记录的内容
@@ -45,16 +45,14 @@
 
 |指令|说明|
 |------|------|
 |/添加订阅 UID|UID为B站用户的uid，不是直播间id，以下同理|
 |/取消订阅 UID|删除订阅|
 |/开启路灯 UID|开启直播间弹幕监听|
 |/关闭路灯 UID|关闭直播间弹幕监听|
-|/开启直播推送 UID|开启开播提醒|
-|/关闭直播推送 UID|关闭开播提醒|
 |/订阅列表|| 
 
 ## 效果预览 
 
 ![](/doc/screenshot.png)
 
 ## 更新日志
```

#### html2text {}

```diff
@@ -18,18 +18,16 @@
 ä»å¨å¼æ­æ¶å¼¹å¹æä»¤æä¼çæ ## ä¾èµ - Python >= 3.10 - OneBot V11
 ## å®è£ - æ¹å¼ä¸ï¼ä½¿ç¨`nb-cli`å®è£æä»¶ ``` nb plugin install
 nonebot-plugin-blive-danmaku ``` - æ¹å¼äºï¼ä½¿ç¨`pip`å®è£ ``` python -
 m pip install nonebot-plugin-blive-danmaku ``` ## æä»¤ |æä»¤|è¯´æ| |-----
 -|------| |/æ·»å è®¢é
 UID|UIDä¸ºBç«ç¨æ·çuidï¼ä¸æ¯ç´æ­é´idï¼ä»¥ä¸åç| |/åæ¶è®¢é
 UID|å é¤è®¢é| |/å¼å¯è·¯ç¯ UID|å¼å¯ç´æ­é´å¼¹å¹çå¬| |/
-å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/å¼å¯ç´æ­æ¨é
-UID|å¼å¯å¼æ­æé| |/å³é­ç´æ­æ¨é UID|å³é­å¼æ­æé| |/
-è®¢éåè¡¨|| ## ææé¢è§ ![](/doc/screenshot.png) ## æ´æ°æ¥å¿ -
-v0.1.4 -
+å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| ## ææé¢è§
+![](/doc/screenshot.png) ## æ´æ°æ¥å¿ - v0.1.4 -
 æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3) -
 è°æ´æ¥å¿çº§å« [#5](https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku/issues/5) - v0.1.3 -
 botæéå¨æ¶é´åé¢å ä¸ç´æ­æ¶é¿æ¾ç¤ºï¼é¿åç´æ­ç»é¢æ²¡æå½åæ¶é´çåºæ¯
 - v0.1.2 - fixå±é¨åéæ æ³æ­£å¸¸æ´æ°çbug - v0.1.0 -
 åºäºnonebot2ï¼å®ç°åæ­¥è·¯ç¯å¼¹å¹å°qqç¾¤ ## æè°¢ - [HarukaBot]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.4/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.1.4
+Version: 0.1.5
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
@@ -39,15 +39,15 @@
 
 [![pypi](https://img.shields.io/pypi/v/nonebot-plugin-blive-danmaku.svg)](https://pypi.org/project/nonebot-plugin-blive-danmaku/)  ![python](https://img.shields.io/pypi/pyversions/nonebot-plugin-blive-danmaku)  [![license](https://img.shields.io/github/license/zangxx66/nonebot_plugin_blive_danmaku.svg)](https://raw.githubusercontent.com/zangxx66/nonebot_plugin_blive_danmaku/main/LICENSE)  
 
 </div>  
 
 ## 简介  
 - 基于[nonebot2](https://v2.nonebot.dev/)开发的B站直播间弹幕监听插件，参考了Haruka和blivechat的部分代码。  
-- 起源于[哈鹿hallu](https://space.bilibili.com/3493118494116797)的一条动态，苦于做视频时没有人做路灯，翻录播的时候头都大了，说要花钱请个全职路灯，我寻思与其把钱送给别人，不如交给Bot去做路灯。
+- 起源于[哈鹿hallu](https://space.bilibili.com/3493118494116797)的一条动态，苦于做视频时没有人做路灯，翻录播的时候头都大了，说要花钱请个全职路灯，我寻思与其把钱送给别人，不如交给Bot去做路灯。  
 ![](/doc/screenshot1.png)
 - 路灯：指把直播过程中有趣的点记录下来，给剪辑根据记录的时间点和内容做出对应的视频。
 
 ## 功能
 
 - 用弹幕的形式记录直播高能点
 - 弹幕指令为`#路灯`加上记录的内容
@@ -72,16 +72,14 @@
 
 |指令|说明|
 |------|------|
 |/添加订阅 UID|UID为B站用户的uid，不是直播间id，以下同理|
 |/取消订阅 UID|删除订阅|
 |/开启路灯 UID|开启直播间弹幕监听|
 |/关闭路灯 UID|关闭直播间弹幕监听|
-|/开启直播推送 UID|开启开播提醒|
-|/关闭直播推送 UID|关闭开播提醒|
 |/订阅列表|| 
 
 ## 效果预览 
 
 ![](/doc/screenshot.png)
 
 ## 更新日志
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.5
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -34,18 +34,16 @@
 ä»å¨å¼æ­æ¶å¼¹å¹æä»¤æä¼çæ ## ä¾èµ - Python >= 3.10 - OneBot V11
 ## å®è£ - æ¹å¼ä¸ï¼ä½¿ç¨`nb-cli`å®è£æä»¶ ``` nb plugin install
 nonebot-plugin-blive-danmaku ``` - æ¹å¼äºï¼ä½¿ç¨`pip`å®è£ ``` python -
 m pip install nonebot-plugin-blive-danmaku ``` ## æä»¤ |æä»¤|è¯´æ| |-----
 -|------| |/æ·»å è®¢é
 UID|UIDä¸ºBç«ç¨æ·çuidï¼ä¸æ¯ç´æ­é´idï¼ä»¥ä¸åç| |/åæ¶è®¢é
 UID|å é¤è®¢é| |/å¼å¯è·¯ç¯ UID|å¼å¯ç´æ­é´å¼¹å¹çå¬| |/
-å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/å¼å¯ç´æ­æ¨é
-UID|å¼å¯å¼æ­æé| |/å³é­ç´æ­æ¨é UID|å³é­å¼æ­æé| |/
-è®¢éåè¡¨|| ## ææé¢è§ ![](/doc/screenshot.png) ## æ´æ°æ¥å¿ -
-v0.1.4 -
+å³é­è·¯ç¯ UID|å³é­ç´æ­é´å¼¹å¹çå¬| |/è®¢éåè¡¨|| ## ææé¢è§
+![](/doc/screenshot.png) ## æ´æ°æ¥å¿ - v0.1.4 -
 æ·»å å¼æ­æéï¼`.env`æ°å¢å¨å±éç½®é¡¹`danmaku_group_notice`å¼å³
 [#3](https://github.com/zangxx66/nonebot_plugin_blive_danmaku/issues/3) -
 è°æ´æ¥å¿çº§å« [#5](https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku/issues/5) - v0.1.3 -
 botæéå¨æ¶é´åé¢å ä¸ç´æ­æ¶é¿æ¾ç¤ºï¼é¿åç´æ­ç»é¢æ²¡æå½åæ¶é´çåºæ¯
 - v0.1.2 - fixå±é¨åéæ æ³æ­£å¸¸æ´æ°çbug - v0.1.0 -
 åºäºnonebot2ï¼å®ç°åæ­¥è·¯ç¯å¼¹å¹å°qqç¾¤ ## æè°¢ - [HarukaBot]
```

