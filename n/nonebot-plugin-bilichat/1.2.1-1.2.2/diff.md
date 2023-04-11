# Comparing `tmp/nonebot_plugin_bilichat-1.2.1.tar.gz` & `tmp/nonebot_plugin_bilichat-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.2.1.tar", last modified: Tue Apr 11 04:49:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.2.2.tar", last modified: Tue Apr 11 16:35:58 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.2.1.tar` & `nonebot_plugin_bilichat-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-11 04:49:17.757088 nonebot_plugin_bilichat-1.2.1/LICENSE
--rw-r--r--   0        0        0     6750 2023-04-11 04:49:17.757088 nonebot_plugin_bilichat-1.2.1/README.md
--rw-r--r--   0        0        0     7031 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4394 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0      406 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4016 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2457 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1311 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1344 2023-04-11 04:49:32.445170 nonebot_plugin_bilichat-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-11 16:35:48.299359 nonebot_plugin_bilichat-1.2.2/LICENSE
+-rw-r--r--   0        0        0     6750 2023-04-11 16:35:48.299359 nonebot_plugin_bilichat-1.2.2/README.md
+-rw-r--r--   0        0        0     7031 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4394 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-11 16:35:48.307359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4067 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2342 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-11 16:35:48.311359 nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1344 2023-04-11 16:35:58.791988 nonebot_plugin_bilichat-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.2.1/LICENSE` & `nonebot_plugin_bilichat-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/README.md` & `nonebot_plugin_bilichat-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 from pathlib import Path
 from typing import List
 
 from EdgeGPT import Chatbot, ConversationStyle
 from nonebot.log import logger
 
 from ..config import plugin_config
+from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
-from ..lib.store import BING_APOLOGY
 
 cookies = json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 logger.info("Try init bing chatbot")
 for count in range(5):
     try:
         bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
         logger.success("Bing chatbot init success")
         break
     except Exception:
         logger.error(f"Bing chatbot init failed, retrying {count+1}/5")
 
 
-
 def get_small_size_transcripts(title: str, text_data: List[str]):
-    prompt = f"请为视频“{title}”总结文案,开头简述要点(大于40字符),\
+    prompt = f"请为视频“{title}”总结文案,开头用一整段文字简述视频的要点(大于40字符),\
 随后总结2-6条视频的Bulletpoint(每条大于15字符),\
 然后使用以下格式输出总结内容 ## 总结 \n ## 要点 \n - [Emoji] Bulletpoint\n\n,\
 如果你无法找到相关的信息可以尝试自己总结,\
 但请一定不要输出任何其他内容。视频文案的内容如下: "
     unique_texts = list(OrderedDict.fromkeys(text_data))
     if plugin_config.bilichat_newbing_token_limit > 0:
         while len(",".join(unique_texts)) + len(prompt) > plugin_config.bilichat_newbing_token_limit:
@@ -49,47 +48,47 @@
     )
     await bot.reset()
     logger.debug(ans)
     bing_resp = ans["item"]["messages"][1]
     return None if bing_resp["contentOrigin"] == "Apology" else bing_resp["text"]
 
 
-
 async def newbing_summarization(cache: Cache, cid: str = "0"):
+    meaning = False
     try:
-        logger.info(f"Generation summary of Video(Column) {cache.id}")
-        if not cache.episodes[cid] or not cache.episodes[cid].content:
-            return "视频无有效字幕"
-        elif not cache.episodes[cid].newbing:
+        if not cache.episodes[cid].newbing:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await newbing_req(get_small_size_transcripts(cache.title, cache.episodes[cid].content))
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await newbing_req(
                     get_small_size_transcripts(cache.title, re.split(r"[，。；,.;\n]+", cache.episodes[cid].content[0]))
                 )
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
-
             # 如果为空则是拒绝回答
             if ai_summary is None:
-                return BING_APOLOGY.read_bytes()
+                return BING_APOLOGY.read_bytes(), False
             # 大于 100 认为有意义
             elif len(ai_summary) > 100:
                 cache.episodes[cid].newbing = ai_summary
                 cache.save()
+                meaning = True
             # 小于 100 认为无意义
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure")
                 cache.episodes[cid].newbing = f"视频(专栏) {cache.id} 总结失败: {ai_summary}"
+        else:
+            meaning = True
+            logger.info("Using cached newbing summarization")
 
-        if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结"):
-            return img
+        if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结", "new Bing(testing)"):
+            return img, meaning
         else:
-            return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].newbing}"
+            return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].newbing}", meaning
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
-        return f"视频(专栏) {cache.id} 总结中止: {e}"
+        return f"视频(专栏) {cache.id} 总结中止: {e}", False
     except Exception as e:
         capture_exception()
         logger.exception(f"Video(Column) {cache.id} summary failed: {e}")
-        return f"视频(专栏) {cache.id} 总结失败: {e}"
+        return f"视频(专栏) {cache.id} 总结失败: {e}", False
```

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from loguru import logger
 
 from .openai import get_small_size_transcripts, get_user_prompt, openai_req
 from .text_to_image import rich_text2image
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
+from ..config import plugin_config
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
     small_size_transcripts = get_small_size_transcripts(sub)
     prompt = get_user_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
@@ -23,32 +24,29 @@
     prompt = get_user_prompt(cv_title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
 async def openai_summarization(cache: Cache, cid: str = "0"):
     try:
-        logger.info(f"Generation summary of Video(Column) {cache.id}")
-        if not cache.episodes[cid] or not cache.episodes[cid].content:
-            return "视频无有效字幕"
-        elif not cache.episodes[cid].openai:
+        if not cache.episodes[cid].openai:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await subtitle_summarise(cache.title, cache.episodes[cid].content)
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await column_summarise(cache.title, cache.episodes[cid].content[0])
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
             if ai_summary.summary:
                 cache.episodes[cid].openai = ai_summary.summary
                 cache.save()
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
                 return f"视频(专栏) {cache.id} 总结失败: {ai_summary.raw}"
-        if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结"):
+        if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结", plugin_config.bilichat_openai_model):
             return img
         else:
             return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].openai}"
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
     except Exception as e:
```

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
 
 cache = cache_dir.joinpath("text2image")
 cache.mkdir(0o755, parents=True, exist_ok=True)
 cache = str(cache.absolute())
 
 
-async def rich_text2image(data: str):
+async def rich_text2image(data: str, src: str):
     config = ConfigInit(
         data_path=cache,
         font_path={
             "text": str(await get_font("HarmonyOS_Sans_SC_Medium.ttf")),
             "extra_text": str(await get_font("sarasa-mono-sc-bold.ttf")),
             "emoji": str(await get_font("nte.ttf")),
         },
     )
+    data = f"AI Summarization, Powered by A60 & Well404 \nNLP Model: {src}\n==========================================={data}"
     if config.dyn_color and config.dyn_font and config.dy_size:
         render = DynTextRender(config.static_path, config.dyn_color, config.dyn_font, config.dy_size)
         image = await render.run(
             Text(
                 text=data,
                 topic=None,
                 rich_text_nodes=[
```

### Comparing `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.2.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.1/pyproject.toml` & `nonebot_plugin_bilichat-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.2.1"
+version = "1.2.2"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.2.1/PKG-INFO` & `nonebot_plugin_bilichat-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.2.1
+Version: 1.2.2
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.2 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
```

