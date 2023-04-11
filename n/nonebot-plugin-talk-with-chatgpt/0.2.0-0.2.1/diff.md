# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.2.0.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0.tar` & `nonebot_plugin_talk_with_chatgpt-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4257 2023-04-11 15:34:32.816134 nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0     5858 2023-04-11 09:11:46.010773 nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-11 15:36:08.029900 nonebot_plugin_talk_with_chatgpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3866 2023-04-11 15:36:16.653769 nonebot_plugin_talk_with_chatgpt-0.2.0/README.md
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4257 2023-04-11 15:34:32.816134 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0     5858 2023-04-11 09:11:46.010773 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-11 15:38:01.871761 nonebot_plugin_talk_with_chatgpt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3869 2023-04-11 15:37:48.275409 nonebot_plugin_talk_with_chatgpt-0.2.1/README.md
+-rw-r--r--   0        0        0     4826 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.2.1/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.2.0"
+version = "0.2.1"
 description = "Nonebot2 基于accessToken登录的chatgpt聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/README.md` & `nonebot_plugin_talk_with_chatgpt-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 ```
 
 #### 大概率用得上的选填项
 ```bash
 # 触发对话的命令前缀，群聊直接艾特也可以触发
 talk_with_chatgpt_start_cmd = /talk
 # 重置对话的命令，就是清空聊天记录
-talk_with_chatgpt_clear_cmd = /talk
+talk_with_chatgpt_clear_cmd = /clear
 # 设置预设的命令前缀
-talk_with_chatgpt_prompt_cmd = /talk
+talk_with_chatgpt_prompt_cmd = /prompt
 # 处理消息时是否提示，默认开
 talk_with_chatgpt_reply_notice = true
 # 群聊是否共享会话，默认关
 talk_with_chatgpt_group_share = false
 ```
 
 #### 可能用得上的选填项
@@ -85,10 +85,10 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/11 \[v0.2.0]
+### 2023/4/11 \[v0.2.1]
 
 * 发布第一版较简陋的插件，并修复了些小问题，细节很重要
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 ## éç½® å¨botå¯¹åºç.envæä»¶ä¿®æ¹ #### å¿å¡«é¡¹ ```bash #
 å¡«ä¸é¢è·åå°çaccessToken talk_with_chatgpt_accesstoken = xxxxxxxxxxx #
 httpä»£çï¼ä¸æ¯æsocksä»£çï¼é»è®¤ç©ºå¼ talk_with_chatgpt_http_proxy =
 http://127.0.0.1:7890 ``` #### å¤§æ¦çç¨å¾ä¸çéå¡«é¡¹ ```bash #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
 talk_with_chatgpt_start_cmd = /talk #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_clear_cmd =
-/talk # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /talk #
+/clear # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt #
 å¤çæ¶æ¯æ¶æ¯å¦æç¤ºï¼é»è®¤å¼ talk_with_chatgpt_reply_notice = true #
 ç¾¤èæ¯å¦å±äº«ä¼è¯ï¼é»è®¤å³ talk_with_chatgpt_group_share = false ```
 #### å¯è½ç¨å¾ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptåä»£å°åï¼é»è®¤ https://
 bypass.churchless.tech/api/conversation talk_with_chatgpt_api_addr = https://
 bypass.churchless.tech/api/conversation # chatgptæ¨¡åï¼é»è®¤ text-davinci-
@@ -38,9 +38,9 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/11 \[v0.2.0] *
+4/11 \[v0.2.1] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.2.0/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.2.0
+Version: 0.2.1
 Summary: Nonebot2 基于accessToken登录的chatgpt聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -71,17 +71,17 @@
 ```
 
 #### 大概率用得上的选填项
 ```bash
 # 触发对话的命令前缀，群聊直接艾特也可以触发
 talk_with_chatgpt_start_cmd = /talk
 # 重置对话的命令，就是清空聊天记录
-talk_with_chatgpt_clear_cmd = /talk
+talk_with_chatgpt_clear_cmd = /clear
 # 设置预设的命令前缀
-talk_with_chatgpt_prompt_cmd = /talk
+talk_with_chatgpt_prompt_cmd = /prompt
 # 处理消息时是否提示，默认开
 talk_with_chatgpt_reply_notice = true
 # 群聊是否共享会话，默认关
 talk_with_chatgpt_group_share = false
 ```
 
 #### 可能用得上的选填项
@@ -108,11 +108,11 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/11 \[v0.2.0]
+### 2023/4/11 \[v0.2.1]
 
 * 发布第一版较简陋的插件，并修复了些小问题，细节很重要
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.0
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.2.1
 Summary: Nonebot2 åºäºaccessTokenç»å½çchatgptèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -32,15 +32,15 @@
 ## éç½® å¨botå¯¹åºç.envæä»¶ä¿®æ¹ #### å¿å¡«é¡¹ ```bash #
 å¡«ä¸é¢è·åå°çaccessToken talk_with_chatgpt_accesstoken = xxxxxxxxxxx #
 httpä»£çï¼ä¸æ¯æsocksä»£çï¼é»è®¤ç©ºå¼ talk_with_chatgpt_http_proxy =
 http://127.0.0.1:7890 ``` #### å¤§æ¦çç¨å¾ä¸çéå¡«é¡¹ ```bash #
 è§¦åå¯¹è¯çå½ä»¤åç¼ï¼ç¾¤èç´æ¥è¾ç¹ä¹å¯ä»¥è§¦å
 talk_with_chatgpt_start_cmd = /talk #
 éç½®å¯¹è¯çå½ä»¤ï¼å°±æ¯æ¸ç©ºèå¤©è®°å½ talk_with_chatgpt_clear_cmd =
-/talk # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /talk #
+/clear # è®¾ç½®é¢è®¾çå½ä»¤åç¼ talk_with_chatgpt_prompt_cmd = /prompt #
 å¤çæ¶æ¯æ¶æ¯å¦æç¤ºï¼é»è®¤å¼ talk_with_chatgpt_reply_notice = true #
 ç¾¤èæ¯å¦å±äº«ä¼è¯ï¼é»è®¤å³ talk_with_chatgpt_group_share = false ```
 #### å¯è½ç¨å¾ä¸çéå¡«é¡¹ ```bash #
 è¯·æ±è¶æ¶æ¶é´ï¼åç­çæçæ¶é´ä¹è¦ç®å¨è¿éé¢çï¼æä»¥ä¸è½å¤ªç­ï¼é»è®¤60ç§
 talk_with_chatgpt_timeout = 60 # chatgptåä»£å°åï¼é»è®¤ https://
 bypass.churchless.tech/api/conversation talk_with_chatgpt_api_addr = https://
 bypass.churchless.tech/api/conversation # chatgptæ¨¡åï¼é»è®¤ text-davinci-
@@ -53,9 +53,9 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/11 \[v0.2.0] *
+4/11 \[v0.2.1] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

