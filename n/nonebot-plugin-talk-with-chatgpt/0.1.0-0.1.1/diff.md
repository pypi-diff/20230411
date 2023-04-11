# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.1.0.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0.tar` & `nonebot_plugin_talk_with_chatgpt-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3928 2023-04-11 09:09:16.637865 nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0     5858 2023-04-11 09:11:46.010773 nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      955 2023-04-11 08:52:44.422881 nonebot_plugin_talk_with_chatgpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3808 2023-04-11 09:15:14.803512 nonebot_plugin_talk_with_chatgpt-0.1.0/README.md
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3928 2023-04-11 09:09:16.637865 nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0     5858 2023-04-11 09:11:46.010773 nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     3049 2023-04-11 08:32:58.238282 nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-11 09:22:02.448737 nonebot_plugin_talk_with_chatgpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3810 2023-04-11 09:21:24.029070 nonebot_plugin_talk_with_chatgpt-0.1.1/README.md
+-rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.1.1/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.1.0"
+version = "0.1.1"
 description = "Nonebot2 基于accessToken登录的chatgpt聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
@@ -16,11 +16,12 @@
 default = true
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 nonebot2 = ">=2.0.0rc1"
 nonebot-adapter-onebot = ">=2.0.0"
 httpx = ">=0.22.0"
+ujson = ">=5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/README.md` & `nonebot_plugin_talk_with_chatgpt-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 ## 简介
 发现商店里没有基于accessToken登录的chatgpt插件，也没看到喜欢的插件，就花一天时间自己写了一个。参考了[chatgpt web](https://github.com/Chanzhaoyu/chatgpt-web)这个开源项目，使用了社区上的反代，如果要使用其他反代可以参考这个项目里的。  
-<img width="500" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
+<img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
 
 插件功能相对其他的来说比较简单，因此也比较易用，获取accessToken并配置代理即可使用，[accessToken获取方式](https://chat.openai.com/api/auth/session)，accessToken字段的值就是了。如果有其他想法或建议欢迎提出，欢迎pr。
 
 ## 安装
 
 使用nb-cli安装
 ```bash
@@ -85,10 +85,10 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | talk | 开始对话，群里@机器人也可以 |
 | clear | 重置对话（不会重置预设） |
 | prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/1 \[v0.1.0]
+### 2023/4/11 \[v0.1.1]
 
 * 发布第一版较简陋的插件
```

#### html2text {}

```diff
@@ -38,8 +38,8 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | talk |
 å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/1 \[v0.1.0] * åå¸ç¬¬ä¸çè¾ç®éçæä»¶
+4/11 \[v0.1.1] * åå¸ç¬¬ä¸çè¾ç®éçæä»¶
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.1.0/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nonebot2 基于accessToken登录的chatgpt聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1)
+Requires-Dist: ujson (>=5.0.0)
 Project-URL: Documentation, https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt#README.md
 Project-URL: Repository, https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/store">
   <img src="https://user-images.githubusercontent.com/44545625/209862575-acdc9feb-3c76-471d-ad89-cc78927e5875.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -40,15 +41,15 @@
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 ## 简介
 发现商店里没有基于accessToken登录的chatgpt插件，也没看到喜欢的插件，就花一天时间自己写了一个。参考了[chatgpt web](https://github.com/Chanzhaoyu/chatgpt-web)这个开源项目，使用了社区上的反代，如果要使用其他反代可以参考这个项目里的。  
-<img width="500" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
+<img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_chatgpt/readme_img/1.jpg"/>  
 
 插件功能相对其他的来说比较简单，因此也比较易用，获取accessToken并配置代理即可使用，[accessToken获取方式](https://chat.openai.com/api/auth/session)，accessToken字段的值就是了。如果有其他想法或建议欢迎提出，欢迎pr。
 
 ## 安装
 
 使用nb-cli安装
 ```bash
@@ -107,11 +108,11 @@
 | 指令 | 说明 |
 |:-----:|:----:|
 | talk | 开始对话，群里@机器人也可以 |
 | clear | 重置对话（不会重置预设） |
 | prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/1 \[v0.1.0]
+### 2023/4/11 \[v0.1.1]
 
 * 发布第一版较简陋的插件
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.1.0
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.1.1
 Summary: Nonebot2 åºäºaccessTokenç»å½çchatgptèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.22.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0) Requires-Dist: nonebot2
-(>=2.0.0rc1) Project-URL: Documentation, https://github.com/nikissXI/
-nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt#README.md Project-
-URL: Repository, https://github.com/nikissXI/nonebot_plugins/tree/main/
-nonebot_plugin_talk_with_chatgpt Description-Content-Type: text/markdown
+(>=2.0.0rc1) Requires-Dist: ujson (>=5.0.0) Project-URL: Documentation, https:/
+/github.com/nikissXI/nonebot_plugins/tree/main/
+nonebot_plugin_talk_with_chatgpt#README.md Project-URL: Repository, https://
+github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
+Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                # nonebot_plugin_talk_with_chatgpt _â¨ Nonebot2
                     ä¸ä¸ªç®åæç¨çchatgptæä»¶ â¨_
                          [license] [nonebot2] [python]
 ## ç®ä»
 åç°ååºéæ²¡æåºäºaccessTokenç»å½çchatgptæä»¶ï¼ä¹æ²¡çå°åæ¬¢çæä»¶ï¼å°±è±ä¸å¤©æ¶é´èªå·±åäºä¸ä¸ªãåèäº
 [chatgpt web](https://github.com/Chanzhaoyu/chatgpt-
@@ -52,8 +53,8 @@
 talk_with_chatgpt_bot_qqnum_list = [1234, 5678, 6666] #
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | talk |
 å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/1 \[v0.1.0] * åå¸ç¬¬ä¸çè¾ç®éçæä»¶
+4/11 \[v0.1.1] * åå¸ç¬¬ä¸çè¾ç®éçæä»¶
```

