# Comparing `tmp/nonebot_plugin_sdgpt-0.1.8.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.1.8.tar` & `nonebot_plugin_sdgpt-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.8/LICENSE
--rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     9983 2023-04-11 05:21:10.304226 nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     1004 2023-04-11 05:23:24.004991 nonebot_plugin_sdgpt-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.8/README.md
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3468 2023-04-11 09:43:15.736752 nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     9983 2023-04-11 05:21:10.304226 nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     1004 2023-04-11 09:44:51.579889 nonebot_plugin_sdgpt-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.9/README.md
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.1.8/LICENSE` & `nonebot_plugin_sdgpt-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .bot import info,error,warn,err
 from nonebot.plugin import on_command , on_message , on
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 from nonebot.adapters import Message
 from nonebot.plugin import PluginMetadata
 
-from nonebot.adapters.onebot.v11.event import GroupMessageEvent
+from nonebot.adapters.onebot.v11.event import GroupMessageEvent,PrivateMessageEvent
 from nonebot.params import CommandArg
 from nonebot.rule import to_me
 from .bot import Chat,Bing,text2image,startup,Chat_api,AIcheck
 
 from dotenv import dotenv_values, load_dotenv
 config =dotenv_values(".cfg")
 
@@ -37,63 +37,62 @@
     Presets = CFGdata['Presets']
     botList = CFGdata['botList']
     cfg = CFGdata['cfg']
     ChatUse = CFGdata['ChatUse']
 
     
 
-chat = on_command('chat')
+chat = on_command('chat', priority=1, block=True)
 @chat.handle()
-async def _(event:GuildMessageEvent|GroupMessageEvent,args: Message = CommandArg()):
+async def _(event:GuildMessageEvent | GroupMessageEvent | PrivateMessageEvent,args: Message = CommandArg()):
     global ChatUse
     message = args.extract_plain_text()
     if ChatUse == Bing:
         if await AIcheck(Chat_api):
             ChatUse = Chat_api
         elif await AIcheck(Chat):
             ChatUse = Chat
     if type(event) == GuildMessageEvent:await ChatUse(bing,message) # type: ignore
-    elif type(event) == GroupMessageEvent:await ChatUse(bing,message,0) # type: ignore
+    else: await ChatUse(bing,message,0) # type: ignore
 
-bing = on_command('bing')
+bing = on_command('bing', priority=1, block=True)
 @bing.handle()
-async def _(event:GuildMessageEvent|GroupMessageEvent,args: Message = CommandArg()):
+async def _(event:GuildMessageEvent|GroupMessageEvent|PrivateMessageEvent,args: Message = CommandArg()):
     message = args.extract_plain_text()
     if type(event) == GuildMessageEvent:await Bing(bing,message)
-    elif type(event) == GroupMessageEvent:await Bing(bing,message,0)
+    else:await Bing(bing,message,0)
         
 
-
-msg = on_message(rule=to_me())
+msg = on_message(rule=to_me(), priority=2, block=True)
 @msg.handle()
-async def _(event:GuildMessageEvent|GroupMessageEvent):
+async def _(event:GuildMessageEvent|GroupMessageEvent|PrivateMessageEvent):
     global ChatUse
     message = str(event.message)
     if type(event) == GuildMessageEvent:await ChatUse(msg,message) # type: ignore
-    elif type(event) == GroupMessageEvent:await ChatUse(msg,message,0) # type: ignore
+    else:await ChatUse(msg,message,0) # type: ignore
 
 
-tag = on_command('tag')
+tag = on_command('tag', priority=1, block=True)
 @tag.handle()
 async def _(args: Message = CommandArg()):
     message = args.extract_plain_text()
     global ChatUse
     await ChatUse(tag,Presets['PromptGenerator'] + message,0) # type: ignore
 
 
-ai = on_command('ai')
+ai = on_command('ai', priority=1, block=True)
 @ai.handle()
 async def _(args: Message = CommandArg()):
     message = args.extract_plain_text()
     global ChatUse
     text = await ChatUse(tag,Presets['PromptGenerator'] + message,2) # type: ignore
     img_bytes = await text2image(ai,text)
     await ai.reject(MessageSegment.image(file=img_bytes,cache=False))
 
-chatC = on_command('切换AI')
+chatC = on_command('切换AI', priority=1, block=True)
 @chatC.handle()
 async def _(args: Message = CommandArg()):
     All = {
         'ChatGPT' : Chat,
         'Bing' : Bing,
         'ChatGPT_api' : Chat_api,
     }
```

### Comparing `nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.1.9/nonebot_plugin_SDGPT/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.8/pyproject.toml` & `nonebot_plugin_sdgpt-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.1.8"
+version = "0.1.9"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
```

### Comparing `nonebot_plugin_sdgpt-0.1.8/README.md` & `nonebot_plugin_sdgpt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.8/PKG-INFO` & `nonebot_plugin_sdgpt-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.1.8
+Version: 0.1.9
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

