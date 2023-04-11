# Comparing `tmp/nonebot_plugin_sdgpt-0.1.7.tar.gz` & `tmp/nonebot_plugin_sdgpt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sdgpt-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_sdgpt-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_sdgpt-0.1.7.tar` & `nonebot_plugin_sdgpt-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.7/LICENSE
--rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/__init__.py
--rw-r--r--   0        0        0     9983 2023-04-10 17:22:24.976760 nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/bot.py
--rw-r--r--   0        0        0     1004 2023-04-10 17:47:44.163226 nonebot_plugin_sdgpt-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.7/README.md
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot_plugin_sdgpt-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3339 2023-04-10 14:07:48.620257 nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/__init__.py
+-rw-r--r--   0        0        0     9983 2023-04-11 05:21:10.304226 nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/bot.py
+-rw-r--r--   0        0        0     1004 2023-04-11 05:23:24.004991 nonebot_plugin_sdgpt-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1034 2023-04-09 01:25:35.547383 nonebot_plugin_sdgpt-0.1.8/README.md
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 nonebot_plugin_sdgpt-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_sdgpt-0.1.7/LICENSE` & `nonebot_plugin_sdgpt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/__init__.py` & `nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.7/nonebot_plugin_SDGPT/bot.py` & `nonebot_plugin_sdgpt-0.1.8/nonebot_plugin_SDGPT/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if len(out_text) < len(text) or mode == 0:
         outText = text.replace(out_text,'')
         success('ChatGPT', outText)
         await func.send(outText)
     
 async def Chat_api(func,message:str,mode=1):
     if not message or len(message)<1:return
-    Rtime = cfg['Chat_stream_waitTime']
+    Rtime = int(cfg['Chat_stream_waitTime'])
     endStr = ast.literal_eval(cfg['Chat_stream_endStr'])
     text = ''
     info('ChatGPT api','开始询问 api')
     for data in chatbot_api.ask_stream(message):
         text += data 
         try: not now # type: ignore
         except: now = time.time()
@@ -151,15 +151,14 @@
         'Bing' : Bing,
         'ChatGPT_api' : Chat_api,
     }
 async def text2image(func,prompt):
     ip = cfg['text2img_proxy'].split(':')
     info('Stable-Diffusion','开始询问 api'+cfg['text2img_proxy'])
     api = webuiapi.WebUIApi(host=ip[0], port=ip[1]) # type: ignore
-    
     result1 = api.txt2img(
         prompt=prompt,
         negative_prompt=cfg['text2img_negative_prompt'],
         steps=cfg['text2img_step'],
     )
     image = result1.image
     success('Stable-Diffusion','返回图片')
```

### Comparing `nonebot_plugin_sdgpt-0.1.7/pyproject.toml` & `nonebot_plugin_sdgpt-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-SDGPT"
-version = "0.1.7"
+version = "0.1.8"
 description = "ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像"
 license = "MIT"
 authors = ["F_thx <thx1140093097@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/thx114/SDGPT"
 repository = "https://github.com/thx114/SDGPT"
 documentation = "https://github.com/thx114/SDGPTreadme"
```

### Comparing `nonebot_plugin_sdgpt-0.1.7/README.md` & `nonebot_plugin_sdgpt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sdgpt-0.1.7/PKG-INFO` & `nonebot_plugin_sdgpt-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sdgpt
-Version: 0.1.7
+Version: 0.1.8
 Summary: ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion : ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像
 Home-page: https://github.com/thx114/SDGPT
 License: MIT
 Keywords: nonebot,nonebot2,chatgpt,new bing,Stable-Diffusion
 Author: F_thx
 Author-email: thx1140093097@gmail.com
 Requires-Python: >=3.8,<4.0
```

