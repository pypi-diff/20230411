# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.6.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.61.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.6.tar` & `nonebot_plugin_blive_danmaku-0.1.61.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.6/LICENSE
--rw-r--r--   0        0        0      127 2023-04-11 07:21:06.066890 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       99 2023-04-10 07:39:11.035690 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/live/__init__.py
--rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/live/live_off.py
--rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/live/live_on.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1421 2023-04-09 17:51:35.475589 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0      980 2023-04-09 17:52:09.092145 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2661 2023-04-11 07:21:12.888303 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     2813 2023-04-11 07:21:06.068901 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      950 2023-04-11 07:21:22.179422 nonebot_plugin_blive_danmaku-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2745 2023-04-11 07:21:06.065885 nonebot_plugin_blive_danmaku-0.1.6/README.md
--rw-r--r--   0        0        0     3781 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.61/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-11 12:02:27.067229 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       99 2023-04-11 12:02:27.068736 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_off.py
+-rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_on.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1409 2023-04-11 12:03:03.764913 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0      980 2023-04-11 12:02:27.070244 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2838 2023-04-11 12:14:08.615605 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     2813 2023-04-11 12:07:23.972087 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      951 2023-04-11 12:14:24.249514 nonebot_plugin_blive_danmaku-0.1.61/pyproject.toml
+-rw-r--r--   0        0        0     2745 2023-04-11 12:02:27.048184 nonebot_plugin_blive_danmaku-0.1.61/README.md
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.61/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/live/live_off.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/live/live_on.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,12 +21,12 @@
     except ResponseCodeError as ex:
         if ex.code == -400 or ex.code == -404:
             await sub_add.finish(f"UID {uid}不存在，请检查后重试")
         elif ex.code == -412:
             await sub_add.finish(f"操作过于频繁，请半小时后再试")
         else:
             await sub_add.finish("发送未知错误")
-    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, live=False, bot_id=event.self_id)
+    res = await db.add_sub(uid=uid, type=event.message_type, type_id=type_id, street_lamp=True, bot_id=event.self_id)
     name = user["name"]
     if res:
         await sub_add.finish(f"添加订阅 {name}({uid}) 成功")
     await sub_add.finish(f"{name}({uid}) 已经订阅")
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,33 +39,36 @@
         if live_status == status:
             continue
         live_uids[uid] = live_status
 
         name = info["uname"]
         room_id = info["short_id"] if info["short_id"] else info["room_id"]
         room_info = await get_room_info_by_id(room_id, reqtype="web")
-        start_timespan = get_timespan(room_info["live_time"])
         if live_status:
             logger.info(f"{name} 开播了")
             url = f"https://live.bilibili.com/{room_id}"
             cover = (
                 info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
             )
             title = info["title"]
             msg = f"{name} 正在直播：\n{title}\n{MessageSegment.image(cover)}\n{url}"
 
+            start_timespan = get_timespan(room_info["live_time"])
             room = db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
             if not room:
                 await db.add_room(room_id=room_id, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0)
         else:
             logger.info(f"{name} 下播了")
             cover = (
                 info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
             )
             msg = f"{name} 下播了\n{MessageSegment.image(cover)}"
 
             now = int(time.time())
-            await db.update_room("end_time", now, room_id=room_id, uid=uid, start_time=start_timespan)
+            room_list = await db.get_rooms(room_id=room_id, uid=uid)
+            room_list.sort(key=lambda x:x.start_time, reverse=True)
+            room = room_list[0]
+            await db.update_room("end_time", now, room_id=room_id, uid=uid, start_time=room.start_time)
         sub_list = await db.get_subs(uid=uid)
         for sub in sub_list:
             await send_msg(bot_id=sub.bot_id, send_type=sub.type, type_id=sub.type_id, message=msg)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.61/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.6"
+version = "0.1.61"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/README.md` & `nonebot_plugin_blive_danmaku-0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.6/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.1.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.1.6
+Version: 0.1.61
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.6
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.61
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

