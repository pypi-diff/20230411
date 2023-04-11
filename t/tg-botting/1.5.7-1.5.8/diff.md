# Comparing `tmp/tg-botting-1.5.7.tar.gz` & `tmp/tg-botting-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.5.7.tar", last modified: Tue Apr 11 17:08:24 2023, max compression
+gzip compressed data, was "tg-botting-1.5.8.tar", last modified: Tue Apr 11 17:42:37 2023, max compression
```

## Comparing `tg-botting-1.5.7.tar` & `tg-botting-1.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.521845 tg-botting-1.5.7/
--rw-rw-rw-   0        0        0      918 2023-04-11 17:08:24.521845 tg-botting-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 17:08:24.522842 tg-botting-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-04-11 17:07:52.000000 tg-botting-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.517856 tg-botting-1.5.7/tg_botting/
--rw-rw-rw-   0        0        0    27942 2023-04-11 17:05:02.000000 tg-botting-1.5.7/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.5.7/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.5.7/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15548 2023-04-11 17:03:57.000000 tg-botting-1.5.7/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.5.7/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.520848 tg-botting-1.5.7/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      918 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 17:42:37.981238 tg-botting-1.5.8/
+-rw-rw-rw-   0        0        0      918 2023-04-11 17:42:37.981238 tg-botting-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 17:42:37.981238 tg-botting-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-04-11 17:42:06.000000 tg-botting-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:42:37.975190 tg-botting-1.5.8/tg_botting/
+-rw-rw-rw-   0        0        0    27942 2023-04-11 17:05:02.000000 tg-botting-1.5.8/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.5.8/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.5.8/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15519 2023-04-11 17:42:06.000000 tg-botting-1.5.8/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.5.8/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:42:37.980209 tg-botting-1.5.8/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-04-11 17:42:37.000000 tg-botting-1.5.8/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-11 17:42:37.000000 tg-botting-1.5.8/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 17:42:37.000000 tg-botting-1.5.8/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-11 17:42:37.000000 tg-botting-1.5.8/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 17:42:37.000000 tg-botting-1.5.8/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.5.7/PKG-INFO` & `tg-botting-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.5.7
+Version: 1.5.8
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.5.7/README.md` & `tg-botting-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.7/setup.py` & `tg-botting-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.7'
+VERSION = '1.5.8'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.5.7/tg_botting/bot.py` & `tg-botting-1.5.8/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.7/tg_botting/cog.py` & `tg-botting-1.5.8/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.7/tg_botting/generals.py` & `tg-botting-1.5.8/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.7/tg_botting/objects.py` & `tg-botting-1.5.8/tg_botting/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,27 +262,26 @@
             return Message(self.bot, rs.get('result'))
 
     async def reply(self, text, reply_markup=None, photo=None, parse_mode=None, **kwargs):
         data = {
             'chat_id': self.chat.id or kwargs['chat_id'],
             'reply_to_message_id': self.message_id
         }
-        if len(text) > 4096:
-            data['text'] = text[0:4096]
-            rs = await self.bot.tg_request('sendMessage', True, **data)
-        data['text'] = text[4096:len(text)]
         if parse_mode:
             data['parse_mode'] = parse_mode
         if reply_markup:
             data['reply_markup'] = json.dumps(reply_markup.to_dict())
+        if len(text) > 4096:
+            data['text'] = text[0:4096]
+            rs = await self.bot.tg_request('sendMessage', True, **data)
         if photo:
             data['caption'] = text
             data.pop('chat_id')
             return await self.send_photo(photo, **data)
-        data['text'] = text
+        data['text'] = text[4096:len(text)]
         rs = await self.bot.tg_request('sendMessage', True, **data)
         return rs.get('ok')
 
 
 class PreCheckOutQuery:
     def __init__(self, payload):
         self.id = payload.get('id')
```

### Comparing `tg-botting-1.5.7/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.5.8/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.5.7
+Version: 1.5.8
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

