# Comparing `tmp/nonebot_plugin_bilichat-1.2.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.2.0.tar", last modified: Mon Apr 10 16:24:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.2.1.tar", last modified: Tue Apr 11 04:49:32 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.2.0.tar` & `nonebot_plugin_bilichat-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-10 16:24:50.045187 nonebot_plugin_bilichat-1.2.0/LICENSE
--rw-r--r--   0        0        0     6703 2023-04-10 16:24:50.045187 nonebot_plugin_bilichat-1.2.0/README.md
--rw-r--r--   0        0        0     7031 2023-04-10 16:24:50.049187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4394 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4408 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      289 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3678 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0      406 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     3544 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2457 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1311 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-10 16:24:50.053187 nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1344 2023-04-10 16:24:58.421182 nonebot_plugin_bilichat-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7992 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-11 04:49:17.757088 nonebot_plugin_bilichat-1.2.1/LICENSE
+-rw-r--r--   0        0        0     6750 2023-04-11 04:49:17.757088 nonebot_plugin_bilichat-1.2.1/README.md
+-rw-r--r--   0        0        0     7031 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4394 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-11 04:49:17.761088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0      406 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4016 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2457 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1311 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-11 04:49:17.765088 nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1344 2023-04-11 04:49:32.445170 nonebot_plugin_bilichat-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.2.0/LICENSE` & `nonebot_plugin_bilichat-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/README.md` & `nonebot_plugin_bilichat-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,27 +113,29 @@
 | bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
 | bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
-| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
+| bilichat_newbing_token_limit | int       | 0                    | newbing请求的文本量上限, 0为无上限 |
+| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
-| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE))
-| bilichat_newbing_token_limit | int       | 0                    | 请求的文本量上限, 0为无上限 |
+
 
 注:
 
 1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
-2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `chatgpt` 进行总结
+2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `openai` 进行总结
 3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
-4. 由于 newbing 限制较大，也不如 chatgpt 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+4. 由于 newbing 限制较大，也不如 openai 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -36,33 +36,34 @@
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
-bilichat_openai_token | str | None | openaiçapikey,
-è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
-è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
-gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
-bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
-è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | |
 bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
 (è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) | bilichat_newbing_token_limit
-| int | 0 | è¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | æ³¨: 1.
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
+è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
+newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_openai_token | str
+| None | openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | |
+bilichat_openai_proxy | str | None |
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
+è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 ~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
 2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
-`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `chatgpt` è¿è¡æ»ç» 3.
+`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
 token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 4. ç±äº newbing
-éå¶è¾å¤§ï¼ä¹ä¸å¦ chatgpt
+éå¶è¾å¤§ï¼ä¹ä¸å¦ openai
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
 (ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
 æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ | æä»¤ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æä»¤1 | ä¸»äºº |
 å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å | æ¯ | ç¾¤è | æä»¤è¯´æ
 | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
```

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,20 @@
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
 
     # AI Summary
+    bilichat_newbing_cookie: Optional[str]
+    bilichat_newbing_token_limit: int = 0
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
     bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
-    bilichat_newbing_cookie: Optional[str]
-    bilichat_newbing_token_limit: int = 0
 
     @validator("nickname")
     def check_nickname(cls, v):
         return list(v) or ["awesome-nonebot"]
 
     @validator("bilichat_openai_proxy")
     def check_openai_proxy(cls, v, values):
```

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,26 @@
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
+from ..lib.store import BING_APOLOGY
 
 cookies = json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
-bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
+logger.info("Try init bing chatbot")
+for count in range(5):
+    try:
+        bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
+        logger.success("Bing chatbot init success")
+        break
+    except Exception:
+        logger.error(f"Bing chatbot init failed, retrying {count+1}/5")
+
 
 
 def get_small_size_transcripts(title: str, text_data: List[str]):
     prompt = f"请为视频“{title}”总结文案,开头简述要点(大于40字符),\
 随后总结2-6条视频的Bulletpoint(每条大于15字符),\
 然后使用以下格式输出总结内容 ## 总结 \n ## 要点 \n - [Emoji] Bulletpoint\n\n,\
 如果你无法找到相关的信息可以尝试自己总结,\
@@ -36,15 +45,17 @@
     ans = await bot.ask(
         prompt=prompt,
         conversation_style=ConversationStyle.creative,
         wss_link="wss://sydney.bing.com/sydney/ChatHub",
     )
     await bot.reset()
     logger.debug(ans)
-    return None if ans["item"]["messages"][1]["contentOrigin"] == "Apology" else ans["item"]["messages"][1]["text"]
+    bing_resp = ans["item"]["messages"][1]
+    return None if bing_resp["contentOrigin"] == "Apology" else bing_resp["text"]
+
 
 
 async def newbing_summarization(cache: Cache, cid: str = "0"):
     try:
         logger.info(f"Generation summary of Video(Column) {cache.id}")
         if not cache.episodes[cid] or not cache.episodes[cid].content:
             return "视频无有效字幕"
@@ -54,20 +65,27 @@
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await newbing_req(
                     get_small_size_transcripts(cache.title, re.split(r"[，。；,.;\n]+", cache.episodes[cid].content[0]))
                 )
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
-            if ai_summary and len(ai_summary) > 100:
+
+            # 如果为空则是拒绝回答
+            if ai_summary is None:
+                return BING_APOLOGY.read_bytes()
+            # 大于 100 认为有意义
+            elif len(ai_summary) > 100:
                 cache.episodes[cid].newbing = ai_summary
                 cache.save()
+            # 小于 100 认为无意义
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure")
-                return f"视频(专栏) {cache.id} 总结失败: 可能是视频无意义或包含冒犯性信息"
+                cache.episodes[cid].newbing = f"视频(专栏) {cache.id} 总结失败: {ai_summary}"
+
         if img := await rich_text2image(cache.episodes[cid].newbing or "视频无法总结"):
             return img
         else:
             return f"总结图片生成失败, 直接发送原文:\n{cache.episodes[cid].newbing}"
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
```

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.2.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.2.0/pyproject.toml` & `nonebot_plugin_bilichat-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.2.0"
+version = "1.2.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.2.0/PKG-INFO` & `nonebot_plugin_bilichat-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -146,27 +146,29 @@
 | bilichat_enable_unkown_src   | bool      | False                | 是否允许响应未知来源的消息 |
 | bilichat_whitelist           | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist           | list[str] | []                   | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font        | str       | None                 | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time             | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_use_bcut_asr        | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
 | bilichat_word_cloud          | bool      | True                 | 是否开启词云功能 |
-| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) , 若留空则禁用newbing总结 |
+| bilichat_newbing_token_limit | int       | 0                    | newbing请求的文本量上限, 0为无上限 |
+| bilichat_openai_token        | str       | None                 | openai的apikey, 若留空则禁用openai总结 |
 | bilichat_openai_proxy        | str       | None                 | 访问openai或newbing使用的代理地址 |
 | bilichat_openai_model        | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
 | bilichat_openai_token_limit  | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
-| bilichat_newbing_cookie      | str       | None                 | newbing的cookie文件路径(获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE))
-| bilichat_newbing_token_limit | int       | 0                    | 请求的文本量上限, 0为无上限 |
+
 
 注:
 
 1. ~~合并转发由于极易受风控影响，因此不推荐使用~~已经把合并转发砍了，没精力适配这玩意了
-2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `chatgpt` 进行总结
+2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `openai` 进行总结
 3. 经测试，目前 newbing 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
-4. 由于 newbing 限制较大，也不如 chatgpt 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+4. 由于 newbing 限制较大，也不如 openai 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
+
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.2.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -54,33 +54,34 @@
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
-bilichat_openai_token | str | None | openaiçapikey,
-è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
-è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
-gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
-bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
-è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | |
 bilichat_newbing_cookie | str | None | newbingçcookieæä»¶è·¯å¾
 (è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) | bilichat_newbing_token_limit
-| int | 0 | è¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | æ³¨: 1.
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)) ,
+è¥çç©ºåç¦ç¨newbingæ»ç» | | bilichat_newbing_token_limit | int | 0 |
+newbingè¯·æ±çææ¬éä¸é, 0ä¸ºæ ä¸é | | bilichat_openai_token | str
+| None | openaiçapikey, è¥çç©ºåç¦ç¨openaiæ»ç» | |
+bilichat_openai_proxy | str | None |
+è®¿é®openaiænewbingä½¿ç¨çä»£çå°å | | bilichat_openai_model | str |
+gpt-3.5-turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | |
+bilichat_openai_token_limit | int | 3500 | è¯·æ±çææ¬éä¸é,
+è®¡ç®æ¹å¼å¯åè[tiktoken](https://github.com/openai/tiktoken) | æ³¨: 1.
 ~~åå¹¶è½¬åç±äºææåé£æ§å½±åï¼å æ­¤ä¸æ¨èä½¿ç¨~~å·²ç»æåå¹¶è½¬åç äºï¼æ²¡ç²¾åééè¿ç©æäº
 2. å¦æåæ¶å¡«åäº `bilichat_openai_token` å
-`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `chatgpt` è¿è¡æ»ç» 3.
+`bilichat_newbing_cookie`ï¼åä¼ä½¿ç¨ `openai` è¿è¡æ»ç» 3.
 ç»æµè¯ï¼ç®å newbing è³å°è½æ»ç» 12000 å­ç¬¦ä»¥ä¸çææ¬ï¼æ¨æµ
 token ä¸éåºä¸º `gpt-4-32k-0314` ç `32200`
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 4. ç±äº newbing
-éå¶è¾å¤§ï¼ä¹ä¸å¦ chatgpt
+éå¶è¾å¤§ï¼ä¹ä¸å¦ openai
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ ## ð ä½¿ç¨ ç´æ¥åéè§é¢
 (ä¸æ )é¾æ¥å³å¯ ### æä»¤è¡¨ >
 æ­£å¨å¼åæä»¤ç¸å³ï¼è¯·æ è§è¿éçæ¨¡æ¿ | æä»¤ | æé | éè¦@
 | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | æä»¤1 | ä¸»äºº |
 å¦ | ç§è | æä»¤è¯´æ | | æä»¤2 | ç¾¤å | æ¯ | ç¾¤è | æä»¤è¯´æ
 | ## ð æè°¢ å¨æ­¤æè°¢ä»¥ä¸å¼åè
```

