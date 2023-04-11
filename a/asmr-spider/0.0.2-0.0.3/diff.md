# Comparing `tmp/asmr_spider-0.0.2.tar.gz` & `tmp/asmr_spider-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.0.2.tar", max compression
+gzip compressed data, was "asmr_spider-0.0.3.tar", max compression
```

## Comparing `asmr_spider-0.0.2.tar` & `asmr_spider-0.0.3.tar`

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
+-rw-r--r--   0        0        0    35149 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/LICENSE
+-rw-r--r--   0        0        0      894 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/README.md
+-rw-r--r--   0        0        0      318 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1767 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/asmr_spider/config.py
+-rw-r--r--   0        0        0     5102 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/asmr_spider/spider.py
+-rw-r--r--   0        0        0      941 2023-04-11 11:47:21.951596 asmr_spider-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 asmr_spider-0.0.3/PKG-INFO
```

### Comparing `asmr_spider-0.0.2/LICENSE` & `asmr_spider-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/asmr_spider/config.py` & `asmr_spider-0.0.3/asmr_spider/config.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/asmr_spider/spider.py` & `asmr_spider-0.0.3/asmr_spider/spider.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.0.2/pyproject.toml` & `asmr_spider-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmr-spider"
-version = "0.0.2"
+version = "0.0.3"
 description = "asmr.one 音声下载器"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "asmr_spider" },
 ]
@@ -21,15 +21,15 @@
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

