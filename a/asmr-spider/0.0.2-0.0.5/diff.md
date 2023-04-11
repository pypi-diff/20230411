# Comparing `tmp/asmr_spider-0.0.2.tar.gz` & `tmp/asmr_spider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.0.2.tar", max compression
+gzip compressed data, was "asmr_spider-0.0.5.tar", max compression
```

## Comparing `asmr_spider-0.0.2.tar` & `asmr_spider-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/LICENSE
--rw-r--r--   0        0        0      552 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/__init__.py
--rw-r--r--   0        0        0      601 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/__main__.py
--rw-r--r--   0        0        0     1767 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/config.py
--rw-r--r--   0        0        0     5102 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/asmr_spider/spider.py
--rw-r--r--   0        0        0      942 2023-04-10 04:39:40.064361 asmr_spider-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 asmr_spider-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/LICENSE
+-rw-r--r--   0        0        0      894 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/README.md
+-rw-r--r--   0        0        0      318 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1767 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/config.py
+-rw-r--r--   0        0        0     5102 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/asmr_spider/spider.py
+-rw-r--r--   0        0        0      940 2023-04-11 12:05:38.207458 asmr_spider-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 asmr_spider-0.0.5/PKG-INFO
```

### Comparing `asmr_spider-0.0.2/LICENSE` & `asmr_spider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/asmr_spider/config.py` & `asmr_spider-0.0.5/asmr_spider/config.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/asmr_spider/spider.py` & `asmr_spider-0.0.5/asmr_spider/spider.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/pyproject.toml` & `asmr_spider-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmr-spider"
-version = "0.0.2"
+version = "0.0.5"
 description = "asmr.one 音声下载器"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "asmr_spider" },
 ]
@@ -13,23 +13,23 @@
 keywords = ["ASMR", "ASMR Downloader"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = ">=6.0"
 httpx = ">=0.23.0"
 loguru = ">=0.6.0"
-pydantic = ">=1.10.5"
+pydantic = "^1.10.5"
 rich = ">=13.0.0"
 
 [tool.poetry.dev-dependencies]
 python = "^3.9"
 PyYAML = ">=6.0"
 httpx = ">=0.23.0"
 loguru = ">=0.6.0"
-pydantic = ">=1.10.5"
+pydantic = "^1.10.5"
 rich = ">=13.0.0"
 ujson = ">=5.2.0"
 
 [tool.poetry.scripts]
 asmr = "asmr_spider.__main__:main"
 
 [tool.mypy]
```

### Comparing `asmr_spider-0.0.2/PKG-INFO` & `asmr_spider-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: asmr-spider
-Version: 0.0.2
+Version: 0.0.5
 Summary: asmr.one 音声下载器
 Home-page: https://github.com/tkgs0/asmr-spider
 License: GPL-3.0
 Keywords: ASMR,ASMR Downloader
 Author: 月ヶ瀬
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: pydantic (>=1.10.5)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: rich (>=13.0.0)
 Project-URL: Repository, https://github.com/tkgs0/asmr-spider
 Description-Content-Type: text/markdown
 
 # ASMR-Spider
 
 本项目改编自 [DiheChen/go-asmr-spider](https://github.com/DiheChen/go-asmr-spider/tree/python)
@@ -39,12 +39,29 @@
 **Run**:
 
 ```bash
 asmr RJ373001 RJ385913
 # `asmr` 后面接RJ号, 可输入多个, 使用空格隔开
 ```
 
+配置文件 `asmr_spider.yml` 和 音频目录 `Voice` 保存在命令执行时所在的路径
+
+<details>
+  <summary>Import</summary>
+
+```python3
+from asmr_spider import dload
+
+async def demo():
+    args = ['RJ373001', 'RJ385913']
+    await dload(args)
+```
+
+`asmr_spider.yml` 和 `Voice` 将保存在你自己的项目根路径
+
+</details>
+
 ## 致谢
 
 - 感谢 [地河酱](https://github.com/DiheChen), 地河酱yyds🤗
 - 感谢 <https://asmr.one>, 现在每天都有不同的女孩子陪我睡觉。
```

