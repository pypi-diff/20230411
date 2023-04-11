# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.2.1.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.2.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1.tar` & `nonebot_plugin_talk_with_chatgpt-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4257 2023-04-11 15:34:32.816134 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0     5858 2023-04-11 09:11:46.010773 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-11 15:38:01.871761 nonebot_plugin_talk_with_chatgpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3869 2023-04-11 15:37:48.275409 nonebot_plugin_talk_with_chatgpt-0.2.1/README.md
--rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4257 2023-04-11 15:34:32.816134 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0     5861 2023-04-11 15:42:31.156223 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-11 15:42:53.816118 nonebot_plugin_talk_with_chatgpt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3869 2023-04-11 15:42:49.594832 nonebot_plugin_talk_with_chatgpt-0.2.2/README.md
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 class Config(BaseModel, extra=Extra.ignore):
     # access_token
     talk_with_chatgpt_accesstoken: str = ""
     # http代理
     talk_with_chatgpt_http_proxy: Optional[str] = None
 
     # 触发对话的命令前缀，群聊直接艾特也可以触发
-    talk_with_chatgpt_start_cmd: str = "talk"
+    talk_with_chatgpt_start_cmd: str = "/talk"
     # 重置对话，就是清空聊天记录
-    talk_with_chatgpt_clear_cmd: str = "clear"
+    talk_with_chatgpt_clear_cmd: str = "/clear"
     # 设置预设
-    talk_with_chatgpt_prompt_cmd: str = "prompt"
+    talk_with_chatgpt_prompt_cmd: str = "/prompt"
     # 处理消息时是否提示
     talk_with_chatgpt_reply_notice: bool = True
     # 群聊是否共享会话
     talk_with_chatgpt_group_share: bool = False
 
     # 请求超时时间
     talk_with_chatgpt_timeout: int = 60
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.2.2/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.2.1"
+version = "0.2.2"
 description = "Nonebot2 基于accessToken登录的chatgpt聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/README.md` & `nonebot_plugin_talk_with_chatgpt-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -85,10 +85,10 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/11 \[v0.2.1]
+### 2023/4/11 \[v0.2.2]
 
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
-4/11 \[v0.2.1] *
+4/11 \[v0.2.2] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.1/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.2.1
+Version: 0.2.2
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
-### 2023/4/11 \[v0.2.1]
+### 2023/4/11 \[v0.2.2]
 
 * 发布第一版较简陋的插件，并修复了些小问题，细节很重要
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.1
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.2
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
-4/11 \[v0.2.1] *
+4/11 \[v0.2.2] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

