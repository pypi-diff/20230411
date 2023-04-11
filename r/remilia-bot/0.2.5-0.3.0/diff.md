# Comparing `tmp/remilia_bot-0.2.5.tar.gz` & `tmp/remilia_bot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remilia_bot-0.2.5.tar", max compression
+gzip compressed data, was "remilia_bot-0.3.0.tar", max compression
```

## Comparing `remilia_bot-0.2.5.tar` & `remilia_bot-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/LICENSE
--rw-r--r--   0        0        0     2276 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/README.md
--rw-r--r--   0        0        0      840 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/__init__.py
--rw-r--r--   0        0        0       66 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/__main__.py
--rw-r--r--   0        0        0     1866 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/config.py
--rw-r--r--   0        0        0      961 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/log.py
--rw-r--r--   0        0        0      984 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/__init__.py
--rw-r--r--   0        0        0     2230 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/Gua64/Gua64.py
--rw-r--r--   0        0        0     1414 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/Gua64/__init__.py
--rw-r--r--   0        0        0     4995 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/block/__init__.py
--rw-r--r--   0        0        0     3721 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/chat/__init__.py
--rw-r--r--   0        0        0     2958 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/chat/looklike.py
--rw-r--r--   0        0        0    81630 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/chat/resource/data.json
--rw-r--r--   0        0        0     3579 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/chat/utils.py
--rw-r--r--   0        0        0     1326 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/cmd/__init__.py
--rw-r--r--   0        0        0     2086 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/cmd/sys_cmd.py
--rw-r--r--   0        0        0     1016 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/code_runner/__init__.py
--rw-r--r--   0        0        0     2857 2023-03-25 02:56:04.165810 remilia_bot-0.2.5/remilia/src/plugins/code_runner/data_source.py
--rw-r--r--   0        0        0     2666 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/setu/__init__.py
--rw-r--r--   0        0        0     3979 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/setu/acggov.py
--rw-r--r--   0        0        0     1776 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/setu/download.py
--rw-r--r--   0        0        0     2359 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/setu/lolicon.py
--rw-r--r--   0        0        0     1099 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/start/__init__.py
--rw-r--r--   0        0        0     1015 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/status/__init__.py
--rw-r--r--   0        0        0     2841 2023-03-25 02:56:04.169810 remilia_bot-0.2.5/remilia/src/plugins/status/data_source.py
--rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 remilia_bot-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2266 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/README.md
+-rw-r--r--   0        0        0      896 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      970 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/__main__.py
+-rw-r--r--   0        0        0     1866 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/config.py
+-rw-r--r--   0        0        0      961 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/log.py
+-rw-r--r--   0        0        0     2230 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/Gua64/Gua64.py
+-rw-r--r--   0        0        0     1414 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/Gua64/__init__.py
+-rw-r--r--   0        0        0     4995 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/block/__init__.py
+-rw-r--r--   0        0        0     3721 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/chat/__init__.py
+-rw-r--r--   0        0        0     2958 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/chat/looklike.py
+-rw-r--r--   0        0        0    81630 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/chat/resource/data.json
+-rw-r--r--   0        0        0     3565 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/chat/utils.py
+-rw-r--r--   0        0        0     1326 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/cmd/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/cmd/sys_cmd.py
+-rw-r--r--   0        0        0     1016 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/code_runner/__init__.py
+-rw-r--r--   0        0        0     2857 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/code_runner/data_source.py
+-rw-r--r--   0        0        0     2666 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/setu/__init__.py
+-rw-r--r--   0        0        0     3979 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/setu/acggov.py
+-rw-r--r--   0        0        0     1776 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/setu/download.py
+-rw-r--r--   0        0        0     2359 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/setu/lolicon.py
+-rw-r--r--   0        0        0     1099 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/start/__init__.py
+-rw-r--r--   0        0        0     1011 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/status/__init__.py
+-rw-r--r--   0        0        0     2841 2023-04-11 09:22:31.673952 remilia_bot-0.3.0/remilia/plugins/status/data_source.py
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 remilia_bot-0.3.0/PKG-INFO
```

### Comparing `remilia_bot-0.2.5/LICENSE` & `remilia_bot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/README.md` & `remilia_bot-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 1. 安装Python3并配置好环境变量
 2. 创建一个空文件夹, 在命令行cd到该文件夹下
 3. 输入以下命令安装并运行
 
 ```sh
 pip install remilia-bot   # 从 PyPI 安装 Bot
-python -m remilia   # 运行 Bot
+remilia   # 运行 Bot
 ```
 
 ### 功能表
 
 - [x] **/start**  
   查看当前会话ID, 通常私聊的会话ID会与用户ID相同
```

### Comparing `remilia_bot-0.2.5/pyproject.toml` & `remilia_bot-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "remilia-bot"
-version = "0.2.5"
+version = "0.3.0"
 description = "女生自用(?)电报机器人"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "remilia" },
 ]
 homepage = "https://github.com/tkgs0/RemiliaBot"
 repository = "https://github.com/tkgs0/RemiliaBot"
 keywords = ["RemiliaBot", "Telegram Bot", "Telegram"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-telegram-bot = ">=20.0"
-pydantic = ">=1.10.0,!=1.10.3"
+pydantic = "^1.10.0,!=1.10.3"
 pyyaml = ">=6.0"
 loguru = ">=0.6.0"
 apscheduler = ">=3.9.1.post1"
 psutil = ">=5.9.0"
 ujson = ">=5.2.0"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.scripts]
+remilia = "remilia.__main__:main"
+
 [tool.mypy]
 python_version = "3.9"
 ignore_missing_imports = true
 implicit_reexport = true
 pretty = true
 show_error_codes = true
 strict = true
```

### Comparing `remilia_bot-0.2.5/remilia/config.py` & `remilia_bot-0.3.0/remilia/config.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/log.py` & `remilia_bot-0.3.0/remilia/log.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/__init__.py` & `remilia_bot-0.3.0/remilia/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from telegram.ext import ApplicationBuilder
 
-from remilia.log import (
+from .log import (
     logging,
     logger,
     LoguruHandler,
     default_format
 )
-from remilia.config import LOG_LEVEL, TOKEN
+from .config import LOG_LEVEL, TOKEN
 
 
 logging.basicConfig(handlers=[LoguruHandler()], level=logging.DEBUG)
 
 logger.remove()
 logger.add(sys.stdout, level=LOG_LEVEL, diagnose=False, format=default_format)
```

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/Gua64/Gua64.py` & `remilia_bot-0.3.0/remilia/plugins/Gua64/Gua64.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/Gua64/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/Gua64/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/block/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/block/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/chat/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/chat/looklike.py` & `remilia_bot-0.3.0/remilia/plugins/chat/looklike.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/chat/resource/data.json` & `remilia_bot-0.3.0/remilia/plugins/chat/resource/data.json`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/chat/utils.py` & `remilia_bot-0.3.0/remilia/plugins/chat/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 )
 
 # hello之类的回复
 hello__reply = [
     'ʕ  •ᴥ•ʔ ?',
 ]
 
+
 # 从字典里返还消息, 借鉴(抄)的zhenxun-bot
-async def get_chat_result(text: str):
+async def get_chat_result(text: str) -> str | None:
     if len(text) < 7:
-        keys = AnimeThesaurus.keys()
-        for key in keys:
-            if text.find(key) != -1:
+        for key in AnimeThesaurus.keys():
+            if key in text:
                 return random.choice(AnimeThesaurus[key])
 
 
 # 从思知api拿到消息
 async def xiaosi(msg: str, NICKNAME: str) -> str:
 
     # 将半角标点和空白符号换成全角空格
```

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/cmd/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/cmd/sys_cmd.py` & `remilia_bot-0.3.0/remilia/plugins/cmd/sys_cmd.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/code_runner/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/code_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/code_runner/data_source.py` & `remilia_bot-0.3.0/remilia/plugins/code_runner/data_source.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/setu/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/setu/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/setu/acggov.py` & `remilia_bot-0.3.0/remilia/plugins/setu/acggov.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/setu/download.py` & `remilia_bot-0.3.0/remilia/plugins/setu/download.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/setu/lolicon.py` & `remilia_bot-0.3.0/remilia/plugins/setu/lolicon.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/start/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/start/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/status/__init__.py` & `remilia_bot-0.3.0/remilia/plugins/status/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from telegram import Update
 from telegram.ext import (
     ContextTypes,
     CommandHandler,
     filters
 )
 
-from remilia.src import scheduler
+from remilia import scheduler
 from remilia.log import logger
 from remilia.config import SUPERUSERS
 from .data_source import get_status
 
 
 def run(application):
     status_handler = CommandHandler(
```

### Comparing `remilia_bot-0.2.5/remilia/src/plugins/status/data_source.py` & `remilia_bot-0.3.0/remilia/plugins/status/data_source.py`

 * *Files identical despite different names*

### Comparing `remilia_bot-0.2.5/PKG-INFO` & `remilia_bot-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: remilia-bot
-Version: 0.2.5
+Version: 0.3.0
 Summary: 女生自用(?)电报机器人
 Home-page: https://github.com/tkgs0/RemiliaBot
 License: GPL-3.0
 Keywords: RemiliaBot,Telegram Bot,Telegram
 Author: 月ヶ瀬
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apscheduler (>=3.9.1.post1)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: psutil (>=5.9.0)
-Requires-Dist: pydantic (>=1.10.0,!=1.10.3)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0,!=1.10.3)
 Requires-Dist: python-telegram-bot (>=20.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: ujson (>=5.2.0)
 Project-URL: Repository, https://github.com/tkgs0/RemiliaBot
 Description-Content-Type: text/markdown
 
 # RemiliaBot
@@ -29,15 +29,15 @@
 
 1. 安装Python3并配置好环境变量
 2. 创建一个空文件夹, 在命令行cd到该文件夹下
 3. 输入以下命令安装并运行
 
 ```sh
 pip install remilia-bot   # 从 PyPI 安装 Bot
-python -m remilia   # 运行 Bot
+remilia   # 运行 Bot
 ```
 
 ### 功能表
 
 - [x] **/start**  
   查看当前会话ID, 通常私聊的会话ID会与用户ID相同
```

