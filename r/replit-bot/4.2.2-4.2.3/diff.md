# Comparing `tmp/replit-bot-4.2.2.tar.gz` & `tmp/replit-bot-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.2.tar", max compression
+gzip compressed data, was "replit-bot-4.2.3.tar", max compression
```

## Comparing `replit-bot-4.2.2.tar` & `replit-bot-4.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.2/LICENSE
--rw-r--r--   0        0        0      822 2023-04-09 17:39:50.797395 replit-bot-4.2.2/pyproject.toml
--rw-r--r--   0        0        0    34078 2023-04-09 17:39:58.889384 replit-bot-4.2.2/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50124 2023-04-01 19:33:20.331864 replit-bot-4.2.2/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.2/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.2/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-09 17:39:48.185398 replit-bot-4.2.2/replit_bot/__init__.py
--rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.2/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.2/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.2/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.2/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.2/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.2/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.2/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.2/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.2/replit_bot/queries.js
--rw-r--r--   0        0        0    66318 2023-04-09 17:33:34.445917 replit-bot-4.2.2/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.2/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.2/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.2/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.2/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.2/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.2/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      823 2023-04-09 17:40:02.253538 replit-bot-4.2.2/setup.py
--rw-r--r--   0        0        0      674 2023-04-09 17:40:02.253851 replit-bot-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.3/LICENSE
+-rw-r--r--   0        0        0      822 2023-04-11 18:24:41.452411 replit-bot-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0    35477 2023-04-11 18:25:13.346789 replit-bot-4.2.3/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50177 2023-04-11 18:25:00.917862 replit-bot-4.2.3/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.3/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.3/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-11 18:24:38.508192 replit-bot-4.2.3/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.3/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.3/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.3/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.3/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.3/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.3/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.3/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.3/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.3/replit_bot/queries.js
+-rw-r--r--   0        0        0    66318 2023-04-09 17:33:34.445917 replit-bot-4.2.3/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.3/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.3/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.3/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.3/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.3/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.3/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      823 2023-04-11 18:25:17.754156 replit-bot-4.2.3/setup.py
+-rw-r--r--   0        0        0      674 2023-04-11 18:25:17.754523 replit-bot-4.2.3/PKG-INFO
```

### Comparing `replit-bot-4.2.2/LICENSE` & `replit-bot-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/pyproject.toml` & `replit-bot-4.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.2"
+version = "4.2.3"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.6.1,<4.0.0"
 # replit db I think I can't remember lol
```

### Comparing `replit-bot-4.2.2/replit_bot/AsyncBot.py` & `replit-bot-4.2.3/replit_bot/AsyncBot.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 repls = x["currentUser"]["replFolderByPath"]["repls"]["items"]
                 cursor = x["currentUser"]["replFolderByPath"]["repls"]["pageInfo"][
                     "nextCursor"
                 ]
                 for i in repls:
                     repl = await self.gql("repl", {"id": i["id"]})
                     url = repl["repl"]["url"]
-                    res = await self.gql("getReplAnnotations", {"url": url})
+                    res = await self.gql("getReplAnnotations", {"id": i["id"]})
                     repl_annotations = res["repl"]
                     if repl_annotations is None:
                         return
                     anchor = list(
                         filter(
                             lambda x: x["isGeneral"],
                             repl_annotations["annotationAnchors"],
@@ -479,25 +479,29 @@
             links.docs = None
 
         @self.on("notification")
         async def _run(notif_id, notif) -> None:
             """main runner code"""
             # MentionedInPost, MentionedInComment, RepliedToComment, RepliedToPost, AnswerAccepted, MultiplayerJoinedEmail, MultiplayerJoinedLink, MultiplayerInvited, MultiplayerOverlimit, Warning, TeamInvite, TeamOrganizationInvite, Basic, TeamTemplateSubmitted, TeamTemplateReviewedStatus, Annotation, EditRequestCreated, EditRequestAccepted, ReplCommentCreated, ReplCommentReplyCreated, ReplCommentMention, Thread, NewFollower
             await self.gql("markOneAsRead", {"id": notif_id})
-
             __typename = getattr(notif, "__typename")
             if __typename == "WarningNotification":
                 logger.critical(
                     f"{red}[FILE] BOT.py{end}\n{red}[INFO]{end} bot has been warned"
                 )
             elif __typename == "NewFollowerNotification":
                 await self._call_when_followed(self, notif.creator)
             elif (
-                __typename == "MentionedInComment" or __typename == "MentionedInPost"
+                __typename == "ReplCommentMentionNotification"
+                or __typename == "MentionedInPost"
             ) and getattr(notif, "comment", False):
+                if notif.comment.parentComment is not None:
+                    notif.comment.thread = notif.comment.parentComment.comments
+                else:
+                    notif.comment.thread = notif.comment.comments
                 notif.comment.notif_type = __typename
                 notif.comment.author = notif.comment.user
                 notif.comment.author.mention = "@" + notif.comment.author.username
                 notif.comment.Image = lambda url, caption="": f"![{caption}]({url})"
                 notif.comment.Link = lambda text, url: f"[{text}]({url})"
                 for i in dir(self):
                     if not i.startswith("__") and not i.endswith("__"):
@@ -620,14 +624,15 @@
                 await self.gql(
                     "markMessageAsSeen",
                     {"replId": repl_annotations["id"], "anchorId": anchor["id"]},
                 )
 
                 class CurrentCtx:
                     def __init__(self):
+                        self.thread = messages
                         self.notif_type = "AnnotationNotification"
                         self.repl_id = repl_annotations["id"]
                         self.anchor_id = anchor["id"]
 
                     async def reply(self, body) -> None:
                         return await self.gql(
                             "createChatMessage",
@@ -721,32 +726,59 @@
                         await self._not_all_required_params_specified(ctx)
                 elif "command" in parsed_json and valid_first:
                     logger.info(
                         f"{green}[FILE] BOT.py{end}\n{green}[INFO]{end} logging command\n\t{blue}[SUMMARY]{end} unsuccessful: {red}Invalid command{end}.\n\t{purple}[EXTRA]{end} Requested command: {parsed_json['command']}"
                     )
                     await self._default(ctx)
             elif __typename == "MultiplayerInvitedNotification":
+                super_self = self
                 url = notif.__dict__["url"]
                 res = await self.gql("getReplAnnotations", {"url": url})
                 repl_annotations = res["repl"]
                 if repl_annotations is None:
                     return
                 anchor = list(
                     filter(
                         lambda x: x["isGeneral"], repl_annotations["annotationAnchors"]
                     )
                 )
                 if len(anchor) > 0:
                     anchor = anchor[0]
                 else:
                     anchor = {"id": None}
+
+                class CurrentThread:
+                    def __init__(self, data) -> None:
+                        self.id = data["id"]
+                        self.anchor_id = data["anchor"]["id"]
+                        self.seen = data["seen"]
+                        self.user = None
+
+                        async def __temp_wrapper():
+                            self.user = await super_self.users.fetch(
+                                data["user"]["username"]
+                            )
+
+                        loop = asyncio.get_event_loop()
+                        loop.create_task(__temp_wrapper())
+                        self.body = data["content"]["text"]
+
+                messages = list(map(lambda x: CurrentThread(x), anchor["messages"]))
+                message = list(
+                    filter(
+                        lambda x: x.body.startswith("@" + self.user.username)
+                        and not x.seen,
+                        messages,
+                    )
+                )
                 super_self = self
 
                 class CurrentCtx:
                     def __init__(self):
+                        self.thread = messages
                         self.notif_type = "MultiplayerInvitedNotification"
                         self.repl_url = url
                         self.repl_id = repl_annotations["id"]
                         self.anchor_id = anchor["id"]
                         self.super_self = super_self
 
                     async def reply(self, body) -> None:
```

### Comparing `replit-bot-4.2.2/replit_bot/AsyncClient.py` & `replit-bot-4.2.3/replit_bot/AsyncClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,14 +892,17 @@
             },
         )
         if res["setBlocking"]:
             return False
         await self.update(res["setBlocking"])
         return self.isBlockedBycurrentUser
 
+    def __str__(self):
+        return self.username
+
 
 class CurrentUser(User):
     def __init__(self, client):
         super()
         super().__init__(client)
         self.c = client
         self.repls = ReplManager(self.c, self)
```

### Comparing `replit-bot-4.2.2/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.3/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/LICENSE` & `replit-bot-4.2.3/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/bot.py` & `replit-bot-4.2.3/replit_bot/bot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/client.py` & `replit-bot-4.2.3/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/html_default_templates.py` & `replit-bot-4.2.3/replit_bot/html_default_templates.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/param.py` & `replit-bot-4.2.3/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/post_ql.py` & `replit-bot-4.2.3/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/queries.js` & `replit-bot-4.2.3/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/queries.py` & `replit-bot-4.2.3/replit_bot/queries.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.3/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/replit_bot/utils/lines.py` & `replit-bot-4.2.3/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.2/setup.py` & `replit-bot-4.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'pyee>=9.0.4,<10.0.0',
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.2',
+    'version': '4.2.3',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.2/PKG-INFO` & `replit-bot-4.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.2
+Version: 4.2.3
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

