# Comparing `tmp/tg-botting-1.5.6.tar.gz` & `tmp/tg-botting-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.5.6.tar", last modified: Sat Feb  4 20:34:57 2023, max compression
+gzip compressed data, was "tg-botting-1.5.7.tar", last modified: Tue Apr 11 17:08:24 2023, max compression
```

## Comparing `tg-botting-1.5.6.tar` & `tg-botting-1.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 20:34:57.306353 tg-botting-1.5.6/
--rw-rw-rw-   0        0        0      918 2023-02-04 20:34:57.306353 tg-botting-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-04 20:34:57.307351 tg-botting-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-02-04 20:34:21.000000 tg-botting-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-04 20:34:57.300370 tg-botting-1.5.6/tg_botting/
--rw-rw-rw-   0        0        0    27688 2023-02-04 20:34:21.000000 tg-botting-1.5.6/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.5.6/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.5.6/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15253 2023-02-01 14:37:15.000000 tg-botting-1.5.6/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.5.6/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-04 20:34:57.305356 tg-botting-1.5.6/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      918 2023-02-04 20:34:57.000000 tg-botting-1.5.6/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-02-04 20:34:57.000000 tg-botting-1.5.6/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 20:34:57.000000 tg-botting-1.5.6/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-04 20:34:57.000000 tg-botting-1.5.6/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-04 20:34:57.000000 tg-botting-1.5.6/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.521845 tg-botting-1.5.7/
+-rw-rw-rw-   0        0        0      918 2023-04-11 17:08:24.521845 tg-botting-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 17:08:24.522842 tg-botting-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-04-11 17:07:52.000000 tg-botting-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.517856 tg-botting-1.5.7/tg_botting/
+-rw-rw-rw-   0        0        0    27942 2023-04-11 17:05:02.000000 tg-botting-1.5.7/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.5.7/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.5.7/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15548 2023-04-11 17:03:57.000000 tg-botting-1.5.7/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.5.7/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:08:24.520848 tg-botting-1.5.7/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 17:08:24.000000 tg-botting-1.5.7/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.5.6/PKG-INFO` & `tg-botting-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.5.6
+Version: 1.5.7
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.5.6/README.md` & `tg-botting-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.6/setup.py` & `tg-botting-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.6'
+VERSION = '1.5.7'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.5.6/tg_botting/bot.py` & `tg-botting-1.5.7/tg_botting/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         self.bot = self
         self.prefix = prefixs
         self.__cogs = {}
         self.group_photos = []
         self.actions_from_cog = {}
         self.command_roles = {}
         self.ignore_listener_filter = []
+        self.trigger_on_forward_message = True
         self.message_handlers = {}
         self.listeners_handle = {}
         self.aliases = {}
         self.chat_filter = []
         self.ignore_filter = []
         self.all_commands = {}
         self._skip_check = lambda x, y: x == y
@@ -421,14 +422,17 @@
 
     async def handleMessage(self, obj):
         if len(obj) >= 1:
             self.offset = obj.get('update_id') + 1
             if 'message' in obj:
                 message = Message(self, obj.get('message'))
                 if await self.check_date(message):
+                    if not self.trigger_on_forward_message:
+                        if message.forward_from is not None or message.forward_date is not None:
+                            return
                     return await self.dispatch(message)
             elif 'callback_query' in obj:
                 query = CallbackQuery(self, obj.get('callback_query'))
                 try:
                     return await self.dispacth_query(query)
                 except Exception:
                     traceback.print_exc()
@@ -665,15 +669,15 @@
         while True:
             lp = self.loop.create_task(self.longpoll())
             if updates is not None:
                 for update in updates:
                     await self.handleMessage(update)
             updates = await lp
 
-    async def general_request(self, url, post=False, **params):
+    async def general_request(self, url, post=False, file=None, **params):
         params = generals.convert_params(params)
         for tries in range(5):
             try:
                 req = self.session.post(url, data=params) if post else self.session.get(url, params=params)
                 async with req as r:
                     if r.content_type == 'application/json':
                         return await r.json()
```

### Comparing `tg-botting-1.5.6/tg_botting/cog.py` & `tg-botting-1.5.7/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.6/tg_botting/generals.py` & `tg-botting-1.5.7/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.5.6/tg_botting/objects.py` & `tg-botting-1.5.7/tg_botting/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,16 @@
             payload.get('new_chat_participant')) if 'new_chat_participant' in payload else None
         self.left_chat_participant = User(
             payload.get('left_chat_participant')) if 'left_chat_participant' in payload else None
         self.left_chat_member = User(payload.get('left_chat_member')) if 'left_chat_member' in payload else None
         self.media_group_id = payload.get('media_group_id') if 'media_group_id' in payload else -1
         self.successful_payment = SuccessfulPayment(
             payload.get('successful_payment')) if 'successful_payment' in payload else None
+        self.forward_from = User(payload.get('forward_from')) if 'forward_from' in payload else None
+        self.forward_date = payload.get('forward_date') if 'forward_date' in payload else None
         try:
             if 'entities' in payload:
                 self.entities = [Entity(p) for p in payload.get('entities')]
             else:
                 self.entities = []
         except Exception:
             self.entities = []
@@ -260,26 +262,27 @@
             return Message(self.bot, rs.get('result'))
 
     async def reply(self, text, reply_markup=None, photo=None, parse_mode=None, **kwargs):
         data = {
             'chat_id': self.chat.id or kwargs['chat_id'],
             'reply_to_message_id': self.message_id
         }
+        if len(text) > 4096:
+            data['text'] = text[0:4096]
+            rs = await self.bot.tg_request('sendMessage', True, **data)
+        data['text'] = text[4096:len(text)]
         if parse_mode:
             data['parse_mode'] = parse_mode
         if reply_markup:
             data['reply_markup'] = json.dumps(reply_markup.to_dict())
         if photo:
             data['caption'] = text
             data.pop('chat_id')
             return await self.send_photo(photo, **data)
-
         data['text'] = text
-        if self.chat.id != self.message_id:
-            del data["reply_to_message_id"]
         rs = await self.bot.tg_request('sendMessage', True, **data)
         return rs.get('ok')
 
 
 class PreCheckOutQuery:
     def __init__(self, payload):
         self.id = payload.get('id')
```

### Comparing `tg-botting-1.5.6/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.5.7/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.5.6
+Version: 1.5.7
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

