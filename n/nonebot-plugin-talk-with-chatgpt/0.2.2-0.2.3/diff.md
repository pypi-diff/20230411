# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.2.2.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.3.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2.tar` & `nonebot_plugin_talk_with_chatgpt-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4257 2023-04-11 15:34:32.816134 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0     5861 2023-04-11 15:42:31.156223 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-11 15:42:53.816118 nonebot_plugin_talk_with_chatgpt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3869 2023-04-11 15:42:49.594832 nonebot_plugin_talk_with_chatgpt-0.2.2/README.md
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4257 2023-04-11 15:44:23.714962 nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0     5861 2023-04-11 15:42:31.156223 nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-11 15:44:53.030102 nonebot_plugin_talk_with_chatgpt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3869 2023-04-11 15:44:28.945983 nonebot_plugin_talk_with_chatgpt-0.2.3/README.md
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,22 @@
     # 获取用户id
     id = get_id(event)
     # 获取信息
     text = event.get_plaintext().strip()
     # 把命令前缀截掉
     if text[: len(start_cmd)] == start_cmd:
         text = text[len(start_cmd) :]
+    # 无内容
+    if not text:
+        await prompt.finish(
+            f"""插件命令如下
+{start_cmd} 【内容】 # 开始对话，群里@机器人也可以
+{clear_cmd}  # 重置对话（不会重置预设）
+{prompt_cmd}  # 设置预设（人格），设置后会重置对话"""
+        )
     # 根据配置是否发出提示
     if pc.talk_with_chatgpt_reply_notice:
         await talk.send("响应中...")
     result = await req_chatgpt(id, text)
     await talk.finish(result, at_sender=True)
 
 
@@ -116,22 +124,14 @@
     if not mp[0]:
         user_prompt = var.session_data[id][2] if var.session_data[id][2] else "<未设置>"
         await prompt.finish(
             f"{prompt_cmd} 重置  # 重置预设\n{prompt_cmd} 【预设信息】  # 设置预设\n当前预设：\n{user_prompt}",
             at_sender=True,
         )
     text = mp[0].strip()
-    # 无内容
-    if not text:
-        await prompt.finish(
-            f"""插件命令如下
-{start_cmd} 【内容】 # 开始对话，群里@机器人也可以
-{clear_cmd}  # 重置对话（不会重置预设）
-{prompt_cmd}  # 设置预设（人格），设置后会重置对话"""
-        )
     # 重置
     if text.strip() == "重置":
         var.session_data[id] = ["", "", ""]
         await prompt.finish("已重置预设", at_sender=True)
     # 设置
     var.session_data[id][2] = text
     await prompt.send("设置中，请稍后...", at_sender=True)
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.2.3/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.2.2"
+version = "0.2.3"
 description = "Nonebot2 基于accessToken登录的chatgpt聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/README.md` & `nonebot_plugin_talk_with_chatgpt-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,10 +85,10 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/11 \[v0.2.2]
+### 2023/4/11 \[v0.2.3]
 
 * 发布第一版较简陋的插件，并修复了些小问题，细节很重要
```

#### html2text {}

```diff
@@ -38,9 +38,9 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/11 \[v0.2.2] *
+4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.2/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Nonebot2 基于accessToken登录的chatgpt聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -108,11 +108,11 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/11 \[v0.2.2]
+### 2023/4/11 \[v0.2.3]
 
 * 发布第一版较简陋的插件，并修复了些小问题，细节很重要
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.2
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.3
 Summary: Nonebot2 åºäºaccessTokenç»å½çchatgptèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -53,9 +53,9 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/11 \[v0.2.2] *
+4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

