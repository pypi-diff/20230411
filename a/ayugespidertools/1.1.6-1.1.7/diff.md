# Comparing `tmp/ayugespidertools-1.1.6.tar.gz` & `tmp/ayugespidertools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayugespidertools-1.1.6.tar", max compression
+gzip compressed data, was "ayugespidertools-1.1.7.tar", max compression
```

## Comparing `ayugespidertools-1.1.6.tar` & `ayugespidertools-1.1.7.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/LICENSE
--rw-r--r--   0        0        0    12098 2023-04-03 01:21:20.000000 ayugespidertools-1.1.6/README.md
--rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/AyuRequest.py
--rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/AyugeCrawlSpider.py
--rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/AyugeSpider.py
--rw-r--r--   0        0        0     8185 2023-02-17 07:53:37.000000 ayugespidertools-1.1.6/ayugespidertools/DownloaderMiddlewares.py
--rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.6/ayugespidertools/FormatData.py
--rw-r--r--   0        0        0     9527 2023-03-30 01:53:24.000000 ayugespidertools-1.1.6/ayugespidertools/ImgOperation.py
--rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.6/ayugespidertools/Items.py
--rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.6/ayugespidertools/Middlewares.py
--rw-r--r--   0        0        0     8593 2023-02-24 01:40:43.000000 ayugespidertools-1.1.6/ayugespidertools/MongoClient.py
--rw-r--r--   0        0        0     1150 2023-04-04 01:32:28.000000 ayugespidertools-1.1.6/ayugespidertools/MysqlClient.py
--rw-r--r--   0        0        0     5480 2023-03-17 03:03:53.000000 ayugespidertools-1.1.6/ayugespidertools/Oss.py
--rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.6/ayugespidertools/Pipelines.py
--rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/ProcessManager.py
--rw-r--r--   0        0        0     2407 2023-04-04 07:13:29.000000 ayugespidertools-1.1.6/ayugespidertools/RPA.py
--rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/RunJs.py
--rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/VerificationCode.py
--rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.6/ayugespidertools/__init__.py
--rw-r--r--   0        0        0     7227 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/commands/__init__.py
--rw-r--r--   0        0        0     7109 2023-03-29 02:02:32.428686 ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
--rw-r--r--   0        0        0     2947 2023-03-29 02:02:32.473687 ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
--rw-r--r--   0        0        0     1158 2023-03-29 02:02:32.506687 ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
--rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.6/ayugespidertools/commands/crawl.py
--rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/commands/genspider.py
--rw-r--r--   0        0        0     4072 2023-03-28 09:33:33.000000 ayugespidertools-1.1.6/ayugespidertools/commands/startproject.py
--rw-r--r--   0        0        0      626 2023-03-28 09:33:33.000000 ayugespidertools-1.1.6/ayugespidertools/commands/version.py
--rw-r--r--   0        0        0     3095 2023-03-30 03:16:54.000000 ayugespidertools-1.1.6/ayugespidertools/common/Encryption.py
--rw-r--r--   0        0        0    15065 2023-04-04 07:06:21.000000 ayugespidertools-1.1.6/ayugespidertools/common/Expend.py
--rw-r--r--   0        0        0    13353 2023-04-04 03:20:52.000000 ayugespidertools-1.1.6/ayugespidertools/common/MultiPlexing.py
--rw-r--r--   0        0        0    32200 2023-04-04 01:43:29.000000 ayugespidertools-1.1.6/ayugespidertools/common/Params.py
--rw-r--r--   0        0        0     3695 2023-03-17 01:47:09.000000 ayugespidertools-1.1.6/ayugespidertools/common/SqlFormat.py
--rw-r--r--   0        0        0      959 2023-03-06 01:34:32.000000 ayugespidertools-1.1.6/ayugespidertools/common/TypeVars.py
--rw-r--r--   0        0        0    11663 2023-04-04 02:00:41.000000 ayugespidertools-1.1.6/ayugespidertools/common/Utils.py
--rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/common/YiDunGap.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/common/__init__.py
--rw-r--r--   0        0        0      455 2023-03-15 08:01:04.000000 ayugespidertools-1.1.6/ayugespidertools/config.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/__init__.py
--rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.6/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0     1810 2023-02-23 06:18:01.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0     4279 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/netlib/requestslib.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     4374 2023-04-04 01:43:29.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2934 2023-04-04 01:43:29.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0    11204 2023-04-04 01:43:29.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/private.py
--rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/download/image.py
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     4282 2023-04-04 02:43:34.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0     2331 2023-04-04 01:32:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0    14927 2023-04-04 01:32:33.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-04 01:32:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      338 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     2081 2023-04-04 01:32:33.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2597 2023-04-04 01:43:29.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     5227 2023-04-04 01:32:34.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     9594 2023-04-04 03:26:52.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0     5950 2023-04-04 07:28:59.092153 ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      777 2023-03-29 02:02:30.564685 ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
--rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
--rw-r--r--   0        0        0      450 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/.gitignore
--rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/README.md
--rw-r--r--   0        0        0      623 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
--rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     4604 2023-03-15 09:36:02.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.6/ayugespidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.6/ayugespidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.6/ayugespidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.6/ayugespidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.6/ayugespidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.6/ayugespidertools/utils/__init__.py
--rw-r--r--   0        0        0     5953 2023-02-10 19:57:28.000000 ayugespidertools-1.1.6/ayugespidertools/utils/cmdline.py
--rw-r--r--   0        0        0     3073 2023-04-04 07:46:51.000000 ayugespidertools-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    13832 1970-01-01 00:00:00.000000 ayugespidertools-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/LICENSE
+-rw-r--r--   0        0        0    12951 2023-04-10 09:42:27.000000 ayugespidertools-1.1.7/README.md
+-rw-r--r--   0        0        0      201 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyuRequest.py
+-rw-r--r--   0        0        0      108 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyugeCrawlSpider.py
+-rw-r--r--   0        0        0       92 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/AyugeSpider.py
+-rw-r--r--   0        0        0     8185 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/DownloaderMiddlewares.py
+-rw-r--r--   0        0        0     9990 2023-02-24 01:32:11.000000 ayugespidertools-1.1.7/ayugespidertools/FormatData.py
+-rw-r--r--   0        0        0     9527 2023-03-30 01:53:24.000000 ayugespidertools-1.1.7/ayugespidertools/ImgOperation.py
+-rw-r--r--   0        0        0     1934 2023-03-14 06:08:38.000000 ayugespidertools-1.1.7/ayugespidertools/Items.py
+-rw-r--r--   0        0        0      673 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/Middlewares.py
+-rw-r--r--   0        0        0     8545 2023-04-11 06:06:53.000000 ayugespidertools-1.1.7/ayugespidertools/MongoClient.py
+-rw-r--r--   0        0        0     1150 2023-04-04 01:32:28.000000 ayugespidertools-1.1.7/ayugespidertools/MysqlClient.py
+-rw-r--r--   0        0        0     5480 2023-03-17 03:03:53.000000 ayugespidertools-1.1.7/ayugespidertools/Oss.py
+-rw-r--r--   0        0        0      694 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/Pipelines.py
+-rw-r--r--   0        0        0       43 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/ProcessManager.py
+-rw-r--r--   0        0        0     2409 2023-04-06 07:08:21.000000 ayugespidertools-1.1.7/ayugespidertools/RPA.py
+-rw-r--r--   0        0        0      982 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/RunJs.py
+-rw-r--r--   0        0        0     6924 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/VerificationCode.py
+-rw-r--r--   0        0        0      474 2023-02-24 06:05:27.000000 ayugespidertools-1.1.7/ayugespidertools/__init__.py
+-rw-r--r--   0        0        0     7227 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/commands/__init__.py
+-rw-r--r--   0        0        0     7109 2023-03-29 02:02:32.428686 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      685 2023-03-29 02:02:32.466687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc
+-rw-r--r--   0        0        0     2947 2023-03-29 02:02:32.473687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc
+-rw-r--r--   0        0        0     1158 2023-03-29 02:02:32.506687 ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/version.cpython-38.pyc
+-rw-r--r--   0        0        0      250 2023-02-23 07:01:46.000000 ayugespidertools-1.1.7/ayugespidertools/commands/crawl.py
+-rw-r--r--   0        0        0      346 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/commands/genspider.py
+-rw-r--r--   0        0        0     4072 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/commands/startproject.py
+-rw-r--r--   0        0        0      626 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/commands/version.py
+-rw-r--r--   0        0        0     3095 2023-03-30 03:16:54.000000 ayugespidertools-1.1.7/ayugespidertools/common/Encryption.py
+-rw-r--r--   0        0        0     6458 2023-04-11 06:00:18.000000 ayugespidertools-1.1.7/ayugespidertools/common/Expend.py
+-rw-r--r--   0        0        0     3832 2023-04-11 07:28:36.000000 ayugespidertools-1.1.7/ayugespidertools/common/MongoDBPipe.py
+-rw-r--r--   0        0        0    11894 2023-04-11 06:29:34.000000 ayugespidertools-1.1.7/ayugespidertools/common/MultiPlexing.py
+-rw-r--r--   0        0        0    12983 2023-04-11 07:26:18.000000 ayugespidertools-1.1.7/ayugespidertools/common/MysqlErrorHandle.py
+-rw-r--r--   0        0        0    32543 2023-04-11 07:27:48.000000 ayugespidertools-1.1.7/ayugespidertools/common/Params.py
+-rw-r--r--   0        0        0     4264 2023-04-11 07:33:08.000000 ayugespidertools-1.1.7/ayugespidertools/common/SpiderDBConf.py
+-rw-r--r--   0        0        0     3726 2023-04-11 07:35:01.000000 ayugespidertools-1.1.7/ayugespidertools/common/SqlFormat.py
+-rw-r--r--   0        0        0     1421 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/common/TypeVars.py
+-rw-r--r--   0        0        0    11146 2023-04-11 07:54:51.000000 ayugespidertools-1.1.7/ayugespidertools/common/Utils.py
+-rw-r--r--   0        0        0     3693 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/common/YiDunGap.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/common/__init__.py
+-rw-r--r--   0        0        0      455 2023-03-15 08:01:04.000000 ayugespidertools-1.1.7/ayugespidertools/config.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      187 2023-02-17 07:53:37.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-29 02:02:28.613683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1439 2023-03-29 02:02:28.615683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8625 2023-03-29 02:02:28.620683 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0    10545 2023-03-01 02:44:36.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      970 2023-02-28 02:20:41.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0     1742 2023-04-11 07:50:13.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0     4275 2023-04-11 07:41:24.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/netlib/requestslib.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     4244 2023-04-11 07:45:40.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2869 2023-04-11 07:45:43.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0    11139 2023-04-11 07:45:49.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/private.py
+-rw-r--r--   0        0        0      963 2023-02-17 07:53:38.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0      820 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0      793 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/image.py
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     3022 2023-04-10 09:37:05.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0     1356 2023-04-10 09:37:46.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0    13257 2023-04-11 03:04:29.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     2823 2023-04-11 02:54:07.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      338 2023-04-11 08:02:51.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     2086 2023-04-10 07:23:47.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2840 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3899 2023-04-11 03:05:04.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     6737 2023-04-10 01:20:43.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     6119 2023-04-04 17:02:00.663859 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      777 2023-03-29 02:02:30.564685 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc
+-rw-r--r--   0        0        0     1213 2023-03-31 08:04:57.033997 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc
+-rw-r--r--   0        0        0      450 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0     2065 2023-03-28 09:33:33.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/.gitignore
+-rw-r--r--   0        0        0       36 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/README.md
+-rw-r--r--   0        0        0      630 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-02 09:20:59.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl
+-rw-r--r--   0        0        0      282 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       77 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     4604 2023-03-15 09:36:02.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2023-02-03 06:47:49.000000 ayugespidertools-1.1.7/ayugespidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0     1654 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     6423 2023-03-14 08:48:24.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1950 2023-02-03 02:54:13.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      567 2023-02-03 02:54:45.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0      559 2023-02-03 02:54:59.000000 ayugespidertools-1.1.7/ayugespidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2023-01-29 07:51:47.000000 ayugespidertools-1.1.7/ayugespidertools/utils/__init__.py
+-rw-r--r--   0        0        0     5953 2023-02-10 19:57:28.000000 ayugespidertools-1.1.7/ayugespidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     3073 2023-04-06 08:21:44.000000 ayugespidertools-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14673 1970-01-01 00:00:00.000000 ayugespidertools-1.1.7/PKG-INFO
```

### Comparing `ayugespidertools-1.1.6/LICENSE` & `ayugespidertools-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/README.md` & `ayugespidertools-1.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -94,14 +94,21 @@
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
 - 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
 + 12).demo_proxy_two: 测试快代理独享代理
+
++13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
++14).demo_crawl: 支持 scrapy CrawlSpider 的示例
+
+# 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
++15).demo_item_loader: 本库 ScrapyClassicItem 及原生 scrapy item 动态添加 item 字段及支持 Item Loaders 的示例
++16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
@@ -149,25 +156,25 @@
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
 
 比如你可能需要更新依赖库中 `pymongo` 为新版本 `x.x.x`，那只需 `poetry install` 安装现有依赖后，再 `poetry add pymongo@x.x.x` 安装目标版本（尽量不要使用 `poetry update pymongo`），确定测试正常了即可 `poetry build` 打包使用。
 
 ## TodoList
 
 - [x] `scrapy` 的扩展功能场景
-  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~ 
+  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [ ] `selenum`: 性能没有 `pyppeteer` 强
+    - [ ] ~~`selenium`: 性能没有 `pyppeteer` 强~~
     - [x] `pyppeteer`: `Gerapy-pyppeteer` 库已经实现此功能
     - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
-    - [ ] `splash`: 继承 `splash` 渲染 `js` 的功能
+    - [ ] ~~`splash`: 继承 `splash` 渲染 `js` 的功能~~
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
@@ -180,7 +187,12 @@
   - [x] `html` 格式转 `markdown` 格式
   - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等等等
   - [x] 添加常用的图片验证码中的处理方法
     - [x] 滑块缺口距离的识别方法（多种实现方式）
     - [x] 根据滑块距离生成轨迹数组的方法
     - [x] 识别点选验证码位置及点击顺序，识别结果不太好，待优化
     - [x] 图片乱序混淆的还原方法示例
+
+注：
+
+- 不再开发结合 `selenium` 扩展的功能，推荐使用 `scrapy-playwright`，`Gerapy-pyppeteer` 等其它库；
+- 不再开发结合 `splash` 的功能，如果使用 `splash http api` 的话，在 `scrapy` ，本库或自写脚本中都比较容易扩展。如果要使用 `lua` `api` 等复杂的功能那还是推荐 `scrapy-splash` 这类的扩展库。
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/DownloaderMiddlewares.py` & `ayugespidertools-1.1.7/ayugespidertools/DownloaderMiddlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/FormatData.py` & `ayugespidertools-1.1.7/ayugespidertools/FormatData.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/ImgOperation.py` & `ayugespidertools-1.1.7/ayugespidertools/ImgOperation.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/Items.py` & `ayugespidertools-1.1.7/ayugespidertools/Items.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/Middlewares.py` & `ayugespidertools-1.1.7/ayugespidertools/Middlewares.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/MongoClient.py` & `ayugespidertools-1.1.7/ayugespidertools/MongoClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,18 @@
             user: 用户名
             password: 用户对应的密码
             host: mongoDB 链接需要的 host
             port: mongoDB 链接需要的端口
             authsource: mongoDB 身份验证需要的数据库名称，默认为 admin
             database: mongoDB 链接需要的数据库
             connect_style: mongoDB 的链接方式，参数选择有：
-                            1). uri: uri 方式；
-                            2). key: 关键字变量方式；
-                            3). auth: authenticate 或 admin 认证方式;
-                            默认为 uri 方式，但其实对外使用还是只传 user, password ... connect_style 的形式
+                1). uri: uri 方式；
+                2). key: 关键字变量方式；
+                3). auth: authenticate 或 admin 认证方式;
+                默认为 uri 方式，但其实对外使用还是只传 user, password ... connect_style 的形式
         """
         # uri 方式，默认使用此方式连接
         if any([not connect_style, connect_style in {"uri", "U"}]):
             uri = f"mongodb://{user}:{password}@{host}:{port}/?authSource={authsource}&authMechanism=SCRAM-SHA-1"
             self.conn = MongoClient(uri)
 
         elif connect_style in {"key", "K"}:
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/MysqlClient.py` & `ayugespidertools-1.1.7/ayugespidertools/MysqlClient.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/Oss.py` & `ayugespidertools-1.1.7/ayugespidertools/Oss.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/Pipelines.py` & `ayugespidertools-1.1.7/ayugespidertools/Pipelines.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/RPA.py` & `ayugespidertools-1.1.7/ayugespidertools/RPA.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         # 当运行成功时
         if not read_log[0]:
             log_res = "".join(read_log[1])
 
             block_times = cls.get_crawl_debug(content=log_res)
             # 当连续输出 scrapy 的统计信息 3 次时，则卡住
             if block_times >= 3:
-                print("quit process success")
-                # cls.quit_process(
-                #     process_name="curr_process", sudo_pwd="自行替换 sudo root 的密码"
-                # )
+                # logger.info("quit process success")
+                cls.quit_process(
+                    process_name="curr_process", sudo_pwd="自行替换 sudo root 的密码"
+                )
 
             # 当最新四行日志中未出现 scrapy 统计，则为正常状态，并清空日志
             elif block_times == 0:
                 clean_log = subprocess.getstatusoutput(f"> {fn}")
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/RunJs.py` & `ayugespidertools-1.1.7/ayugespidertools/RunJs.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/VerificationCode.py` & `ayugespidertools-1.1.7/ayugespidertools/VerificationCode.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/genspider.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/startproject.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/__pycache__/version.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/commands/__pycache__/version.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/startproject.py` & `ayugespidertools-1.1.7/ayugespidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/commands/version.py` & `ayugespidertools-1.1.7/ayugespidertools/commands/version.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/Encryption.py` & `ayugespidertools-1.1.7/ayugespidertools/common/Encryption.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/MultiPlexing.py` & `ayugespidertools-1.1.7/ayugespidertools/common/MultiPlexing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,414 +1,377 @@
-import asyncio
-import copy
-import json
-import os
-import random
-import re
-from typing import Any, Optional, Union
-
-import cv2
-import numpy as np
-import pymysql
-from twisted.internet.defer import Deferred
-
-from ayugespidertools.config import logger
-
-__all__ = [
-    "ReuseOperation",
-]
-
-
-class ReuseOperation(object):
-    """
-    用于存放经常复用的一些操作
-    """
-
-    @staticmethod
-    def as_deferred(f):
-        """
-        transform a Twisted Deferred to an Asyncio Future
-        Args:
-            f: async function
-
-        Returns:
-            1).Deferred
-        """
-        return Deferred.fromFuture(asyncio.ensure_future(f))
-
-    @staticmethod
-    def is_namedtuple_instance(x: Any) -> bool:
-        """
-        判断 x 是否为 namedtuple 类型
-        Args:
-            x: 需要判断的参数
-
-        Returns:
-            1). 是否符合 namedtuple 类型
-        """
-        return isinstance(x, tuple) and hasattr(x, "_fields")
-
-    @staticmethod
-    def judge_file_style(
-        media_file_or_url: str,
-        strict: bool = False,
-        media_type: Optional[str] = None,
-    ) -> str:
-        """
-        判断新增图片的格式类型（此方法是为了防止图片地址格式不统一，造成图片格式提取错误）
-        Args:
-            media_file_or_url: 需要判断格式类型的文件或文件链接
-            strict: media 是否为严格模式，严格模式下也需要仔细判断
-            media_type: media 文件的类型，image，vedio，voice 等
-
-        Returns:
-            1): 文件的格式信息
-        """
-        if any([media_file_or_url.startswith("http"), strict]):
-            image_style = [
-                ".svg",
-                ".png",
-                ".jpg",
-                ".jpeg",
-                ".bmp",
-                ".wav",
-                ".mp3",
-                ".ogg",
-                ".flv",
-            ]
-            for image_format in image_style:
-                if image_format in media_file_or_url:
-                    return image_format[1:]
-
-        # 否则就是文件，则返回文件后缀即可
-        return media_file_or_url.split(".")[-1]
-
-    @staticmethod
-    def get_file_name_by_url(file_url: str) -> str:
-        """
-        根据文件链接取出文件的名称
-        Args:
-            file_url: 文件链接
-
-        Returns:
-            1). 文件名称
-        """
-        pattern = re.compile(r""".*/(.*?)\..*?""")
-        if file_name_list := pattern.findall(file_url):
-            return file_name_list[0]
-        return ""
-
-    # TODO: 优化此方法，修改方法名称等
-    @staticmethod
-    def get_voice_files(path: str) -> list:
-        """
-        获取 path 文件夹下的所有文件
-        Args:
-            path: 需要判断的文件夹路径
-
-        Returns:
-            file_list: path 文件夹下的文件列表
-        """
-        # 得到文件夹下的所有文件名称
-        files = os.listdir(path)
-        return [file for file in files if not os.path.isdir(path + "\\" + file)]
-
-    @staticmethod
-    def get_bytes_by_file(file_path: str) -> bytes:
-        """
-        获取媒体文件的 bytes 内容
-        Args:
-            file_path: 对应文件的路径
-
-        Returns:
-            file_bytes: file_path 对应文件的 bytes 内容
-        """
-        with open(file_path, "rb") as f:
-            file_bytes = f.read()
-        return file_bytes
-
-    @staticmethod
-    def read_image_data(bg: Union[bytes, str], tp: Union[bytes, str]):
-        """
-        用 opencv 读取图片数据
-        Args:
-            bg: 背景图片信息
-            tp: 滑块图
-
-        Returns:
-            bg_cv: opencv 读取背景图片的数据
-            tp_cv: opencv 读取滑块图片的数据
-        """
-        assert type(bg) in [str, bytes], "带缺口的背景图参数需要是全路径图片或 bytes 数据"
-        assert type(tp) in [str, bytes], "滑块图参数需要是全路径图片或 bytes 数据"
-
-        if isinstance(bg, bytes):
-            bg_buf = np.frombuffer(bg, np.uint8)
-            bg_cv = cv2.imdecode(bg_buf, cv2.IMREAD_ANYCOLOR)
-        else:
-            # 读取图片，读进来直接是 BGR 格式数据格式在 0~255
-            bg_cv = cv2.imread(bg)
-
-        if isinstance(tp, bytes):
-            tp_buf = np.frombuffer(tp, np.uint8)
-            tp_cv = cv2.imdecode(tp_buf, cv2.IMREAD_ANYCOLOR)
-        else:
-            # 0 表示采用黑白的方式读取图片
-            tp_cv = cv2.imread(tp, 0)
-
-        return bg_cv, tp_cv
-
-    @staticmethod
-    def random_weight(weight_data: list):
-        """
-        带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
-        Args:
-            weight_data: 带权重的列表信息，示例：
-                [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
-
-        Returns:
-            ret: 返回当前权重列表 account_arr 中的一个值
-        """
-        total = sum(item["weight"] for item in weight_data)
-        # 在 0 与权重和之间获取一个随机数
-        ra = random.uniform(0, total)
-        curr_sum = 0
-        ret = None
-        for data in weight_data:
-            # 在遍历中，累加当前权重值
-            curr_sum += data["weight"]
-            # 当随机数 <= 当前权重和时，返回权重 key
-            if ra <= curr_sum:
-                ret = data
-                break
-        return ret
-
-    @classmethod
-    def is_dict_meet_min_limit(cls, dict_conf: dict, key_list: list) -> bool:
-        """
-        判断 dict_conf 是否满足 key_list 中的 key 值限定
-        Args:
-            dict_conf: 需要判断的参数
-            key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
-
-        Returns:
-            1). 是否满足 key 值限制
-        """
-        if any([not dict_conf, not isinstance(dict_conf, dict)]):
-            return False
-
-        return all(key in dict_conf for key in key_list)
-
-    @classmethod
-    def get_items_by_keys(cls, dict_conf: dict, key_list: list) -> Union[dict, bool]:
-        """
-        获取 dict_conf 中的含有 key_list 的 key 的字段
-        Args:
-            dict_conf: 需要处理的参数
-            key_list: 需要取的 key 值列表
-
-        Returns:
-            1). 取值后的 dict，或不满足请求的 False 值
-        """
-        # 参数先要满足最小限定，然后再取出限定的参数值；否则直接返回 False
-        return (
-            {k: dict_conf[k] for k in key_list}
-            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=key_list)
-            else False
-        )
-
-    @classmethod
-    def get_items_except_keys(cls, dict_conf, key_list: list) -> dict:
-        """
-        获取 dict_conf 中的不含有 key_list 的 key 的字段
-        Args:
-            dict_conf: 需要处理的参数
-            key_list: 需要排除的 key 值列表
-
-        Returns:
-            1). dict_conf 排除 key_list 中的键值后的值
-        """
-        return {k: dict_conf[k] for k in dict_conf if k not in key_list}
-
-    @classmethod
-    def create_database(cls, pymysql_dict_conf: dict):
-        """
-        创建数据库
-        由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
-        Args:
-            pymysql_dict_conf: pymysql 的数据库连接配置 dict
-
-        Returns:
-            None
-        """
-        # 判断 pymysql_dict_conf 是否满足最少的 key 值
-        judge_pymysql_dict_conf = cls.is_dict_meet_min_limit(
-            dict_conf=pymysql_dict_conf,
-            key_list=["host", "port", "user", "password", "charset"],
-        )
-        assert (
-            judge_pymysql_dict_conf
-        ), "创建数据库时的 pymysql 连接参数不满足条件，可能多了 database 参数，或者少了某些参数！"
-
-        pymysql_dict_conf_tmp = copy.deepcopy(pymysql_dict_conf)
-        if "database" in pymysql_dict_conf_tmp:
-            del pymysql_dict_conf_tmp["database"]
-        conn = pymysql.connect(**pymysql_dict_conf_tmp)
-        cursor = conn.cursor()
-        cursor.execute(
-            f"""CREATE DATABASE `{pymysql_dict_conf["database"]}` character set {pymysql_dict_conf["charset"]};"""
-        )
-        conn.close()
-        logger.info(
-            f"""创建数据库 {pymysql_dict_conf["database"]} 成功，其 charset 类型是：{pymysql_dict_conf["charset"]}!"""
-        )
-
-    @classmethod
-    def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
-        """
-        将 dict 中 str 类型的 key 值变成小写
-        Args:
-            deal_dict: 需要处理的 dict
-
-        Returns:
-            1).处理后的 dict 值
-        """
-        str_key_to_lower_dict = {
-            k.lower(): v for k, v in deal_dict.items() if isinstance(k, str)
-        }
-        not_str_key_dict = {
-            k: v for k, v in deal_dict.items() if not isinstance(k, str)
-        }
-        # python 3.9+ 可优化为：str_key_to_lower_dict |= not_str_key_dict
-        str_key_to_lower_dict.update(not_str_key_dict)
-        return str_key_to_lower_dict
-
-    @classmethod
-    def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
-        """
-        将 dict 中 str 类型的 key 值变成大写
-        Args:
-            deal_dict: 需要处理的 dict
-
-        Returns:
-            1).处理后的 dict 值
-        """
-        # 找出 str 类型的 key 字段数据，并将其大写
-        str_key_to_upper_dict = {
-            k.upper(): v for k, v in deal_dict.items() if isinstance(k, str)
-        }
-        # 找出非 str 类型的数据
-        not_str_key_dict = {
-            k: v for k, v in deal_dict.items() if not isinstance(k, str)
-        }
-        # 将大写处理的字典加上非 str 类型的 key 字段数据
-        str_key_to_upper_dict.update(not_str_key_dict)
-        return str_key_to_upper_dict
-
-    @classmethod
-    def get_consul_conf(cls, settings: dict) -> dict:
-        """
-        获取项目中的 consul 配置，且要根据项目整体情况来取出满足最少要求的 consul 配置
-        Args:
-            settings: scrapy 的 settings 信息
-
-        Returns:
-            consul_conf_dict_min: 满足要求的最少要求的 consul 配置
-        """
-        consul_conf_dict = settings.get("CONSUL_CONFIG", {})
-        consul_conf_dict_lowered = cls.dict_keys_to_lower(consul_conf_dict)
-        # 取最少需要配置的值，consul 一般情况下最少需要 token, url 两个值，format 默认为 json
-        consul_conf_dict_min = cls.get_items_by_keys(
-            dict_conf=consul_conf_dict_lowered, key_list=["token", "url", "format"]
-        )
-        assert consul_conf_dict_min, f"consul 配置：{consul_conf_dict} 不满足最小参数配置要求！"
-        return consul_conf_dict_min
-
-    @classmethod
-    def judge_str_is_json(cls, judge_str: str) -> bool:
-        """
-        判断字符串是否为 json 格式
-        Args:
-            judge_str: 需要判断的字符串
-
-        Returns:
-            1）.是否为 json 格式
-        """
-        if not isinstance(judge_str, str):
-            return False
-
-        try:
-            json.loads(judge_str)
-        except Exception as e:
-            return False
-        else:
-            return True
-
-    @staticmethod
-    def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
-        """
-        从 headers 中的 ck str 格式转化为 dict 格式
-        Args:
-            headers_ck_str: request headers ck 的 str 格式
-
-        Returns:
-            1). 转化 dict 格式后的 ck
-        """
-        # 也可以这样写，但不推荐
-        # dict(line.split("=", 1) for line in headers_ck_str.split("; "))
-        return {
-            x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
-            for x in headers_ck_str.split(";")
-        }
-
-    @staticmethod
-    def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
-        """
-        将 scrapy 请求中的 body 对象转为 dict 格式
-        Args:
-            req_body_data_str: scrapy 中的 body 参数
-
-        Returns:
-            1). 转化 dict 格式后的 body
-        """
-        return {
-            x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
-        }
-
-    @staticmethod
-    def get_array_dimension(array: list) -> int:
-        """
-        获取 array 的维度
-        Args:
-            array: 数组
-
-        Returns:
-            1).层级数
-        """
-        # 其实直接返回 len(array) 即可
-        return len(np.array(array).shape)
-
-    @classmethod
-    def get_array_depth(cls, array: list) -> int:
-        """
-        获取 array 的最大层级，深度
-        Args:
-            array: 数组
-
-        Returns:
-            1).最大层级，深度
-        """
-
-        """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
-        # 先判断是否为数组类型的元素
-        judge_array = isinstance(
-            array,
-            (
-                frozenset,
-                list,
-                set,
-                tuple,
-            ),
-        )
-        return (
-            int(judge_array) and len(array) and 1 + max(map(cls.get_array_depth, array))
-        )
+import asyncio
+import json
+import os
+import random
+import re
+from typing import Any, List, Union
+
+import cv2
+import numpy as np
+import pymysql
+from scrapy.settings import Settings
+from twisted.internet.defer import Deferred
+
+from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.config import logger
+
+__all__ = [
+    "ReuseOperation",
+]
+
+
+class ReuseOperation(object):
+    """
+    用于存放经常复用的一些操作
+    """
+
+    @staticmethod
+    def as_deferred(f):
+        """
+        transform a Twisted Deferred to an Asyncio Future
+        Args:
+            f: async function
+
+        Returns:
+            1).Deferred
+        """
+        return Deferred.fromFuture(asyncio.ensure_future(f))
+
+    @staticmethod
+    def is_namedtuple_instance(x: Any) -> bool:
+        """
+        判断 x 是否为 namedtuple 类型
+        Args:
+            x: 需要判断的参数
+
+        Returns:
+            1). 是否符合 namedtuple 类型
+        """
+        return isinstance(x, tuple) and hasattr(x, "_fields")
+
+    @staticmethod
+    def get_file_name_by_url(file_url: str) -> str:
+        """
+        根据文件链接取出文件的名称
+        Args:
+            file_url: 文件链接
+
+        Returns:
+            1). 文件名称
+        """
+        pattern = re.compile(r""".*/(.*?)\..*?""")
+        if file_name_list := pattern.findall(file_url):
+            return file_name_list[0]
+        return ""
+
+    @staticmethod
+    def get_files_from_path(path: str) -> list:
+        """
+        获取 path 文件夹下的所有文件
+        Args:
+            path: 需要判断的文件夹路径
+
+        Returns:
+            file_list: path 文件夹下的文件列表
+        """
+        # 得到文件夹下的所有文件名称
+        files = os.listdir(path)
+        return [file for file in files if not os.path.isdir(path + "\\" + file)]
+
+    @staticmethod
+    def get_bytes_by_file(file_path: str) -> bytes:
+        """
+        获取媒体文件的 bytes 内容
+        Args:
+            file_path: 对应文件的路径
+
+        Returns:
+            file_bytes: file_path 对应文件的 bytes 内容
+        """
+        with open(file_path, "rb") as f:
+            file_bytes = f.read()
+        return file_bytes
+
+    @staticmethod
+    def read_image_data(
+        bg: Union[bytes, str],
+        tp: Union[bytes, str],
+    ) -> (np.ndarray, np.ndarray):
+        """
+        用 opencv 读取图片数据
+        Args:
+            bg: 背景图片信息
+            tp: 滑块图
+
+        Returns:
+            bg_cv: opencv 读取背景图片的数据
+            tp_cv: opencv 读取滑块图片的数据
+        """
+        assert type(bg) in [str, bytes], "带缺口的背景图参数需要是全路径图片或 bytes 数据"
+        assert type(tp) in [str, bytes], "滑块图参数需要是全路径图片或 bytes 数据"
+
+        if isinstance(bg, bytes):
+            bg_buf = np.frombuffer(bg, np.uint8)
+            bg_cv = cv2.imdecode(bg_buf, cv2.IMREAD_ANYCOLOR)
+        else:
+            # 读取图片，读进来直接是 BGR 格式数据格式在 0~255
+            bg_cv = cv2.imread(bg)
+
+        if isinstance(tp, bytes):
+            tp_buf = np.frombuffer(tp, np.uint8)
+            tp_cv = cv2.imdecode(tp_buf, cv2.IMREAD_ANYCOLOR)
+        else:
+            # 0 表示采用黑白的方式读取图片
+            tp_cv = cv2.imread(tp, 0)
+
+        return bg_cv, tp_cv
+
+    @staticmethod
+    def random_weight(weight_data: list):
+        """
+        带权重的随机取值，即在带权重的列表数据中根据权重随机取一个值
+        Args:
+            weight_data: 带权重的列表信息，示例：
+                [{'username': 'xxxx', 'password': '******', 'weight': 8}, ...]
+
+        Returns:
+            ret: 返回当前权重列表 account_arr 中的一个值
+        """
+        total = sum(item["weight"] for item in weight_data)
+        # 在 0 与权重和之间获取一个随机数
+        ra = random.uniform(0, total)
+        curr_sum = 0
+        ret = None
+        for data in weight_data:
+            # 在遍历中，累加当前权重值
+            curr_sum += data["weight"]
+            # 当随机数 <= 当前权重和时，返回权重 key
+            if ra <= curr_sum:
+                ret = data
+                break
+        return ret
+
+    @classmethod
+    def is_dict_meet_min_limit(cls, dict_conf: dict, key_list: List[str]) -> bool:
+        """
+        判断 dict_conf 是否满足 key_list 中的 key 值限定
+        Args:
+            dict_conf: 需要判断的参数
+            key_list: dict_conf 中需要包含的 key 值列表，示例为：['proxy', 'username', 'password']
+
+        Returns:
+            1). 是否满足 key 值限制
+        """
+        if any([not dict_conf, not isinstance(dict_conf, dict)]):
+            return False
+
+        return all(key in dict_conf for key in key_list)
+
+    @classmethod
+    def get_items_by_keys(
+        cls,
+        dict_conf: dict,
+        key_list: List[str],
+    ) -> Union[dict, bool]:
+        """
+        获取 dict_conf 中的含有 key_list 的 key 的字段
+        Args:
+            dict_conf: 需要处理的参数
+            key_list: 需要取的 key 值列表
+
+        Returns:
+            1). 取值后的 dict，或不满足请求的 False 值
+        """
+        # 参数先要满足最小限定，然后再取出限定的参数值；否则直接返回 False
+        return (
+            {k: dict_conf[k] for k in key_list}
+            if cls.is_dict_meet_min_limit(dict_conf=dict_conf, key_list=key_list)
+            else False
+        )
+
+    @classmethod
+    def get_items_except_keys(cls, dict_conf, key_list: List[str]) -> dict:
+        """
+        获取 dict_conf 中的不含有 key_list 的 key 的字段
+        Args:
+            dict_conf: 需要处理的参数
+            key_list: 需要排除的 key 值列表
+
+        Returns:
+            1). dict_conf 排除 key_list 中的键值后的值
+        """
+        return {k: dict_conf[k] for k in dict_conf if k not in key_list}
+
+    @classmethod
+    def create_database(cls, mysql_conf: MysqlConfig) -> None:
+        """
+        创建数据库
+        由于这是在连接数据库，报数据库不存在错误时的场景，则需要新建(不指定数据库)连接创建好所需数据库即可
+        Args:
+            mysql_conf: pymysql 的数据库连接配置
+
+        Returns:
+            None
+        """
+        conn = pymysql.connect(
+            user=mysql_conf.user,
+            password=mysql_conf.password,
+            host=mysql_conf.host,
+            port=mysql_conf.port,
+            charset=mysql_conf.charset,
+        )
+        cursor = conn.cursor()
+        cursor.execute(
+            f"CREATE DATABASE `{mysql_conf.database}` character set {mysql_conf.charset};"
+        )
+        conn.close()
+        logger.info(
+            f"创建数据库 {mysql_conf.database} 成功，其 charset 类型是：{mysql_conf.charset}!"
+        )
+
+    @classmethod
+    def dict_keys_to_lower(cls, deal_dict: dict) -> dict:
+        """
+        将 dict 中 str 类型的 key 值变成小写
+        Args:
+            deal_dict: 需要处理的 dict
+
+        Returns:
+            1).处理后的 dict 值
+        """
+        str_key_to_lower_dict = {
+            k.lower(): v for k, v in deal_dict.items() if isinstance(k, str)
+        }
+        not_str_key_dict = {
+            k: v for k, v in deal_dict.items() if not isinstance(k, str)
+        }
+        # python 3.9+ 可优化为：str_key_to_lower_dict |= not_str_key_dict
+        str_key_to_lower_dict.update(not_str_key_dict)
+        return str_key_to_lower_dict
+
+    @classmethod
+    def dict_keys_to_upper(cls, deal_dict: dict) -> dict:
+        """
+        将 dict 中 str 类型的 key 值变成大写
+        Args:
+            deal_dict: 需要处理的 dict
+
+        Returns:
+            1).处理后的 dict 值
+        """
+        # 找出 str 类型的 key 字段数据，并将其大写
+        str_key_to_upper_dict = {
+            k.upper(): v for k, v in deal_dict.items() if isinstance(k, str)
+        }
+        # 找出非 str 类型的数据
+        not_str_key_dict = {
+            k: v for k, v in deal_dict.items() if not isinstance(k, str)
+        }
+        # 将大写处理的字典加上非 str 类型的 key 字段数据
+        str_key_to_upper_dict.update(not_str_key_dict)
+        return str_key_to_upper_dict
+
+    @classmethod
+    def get_consul_conf(cls, settings: Settings) -> dict:
+        """
+        获取项目中的 consul 配置，且要根据项目整体情况来取出满足最少要求的 consul 配置
+        Args:
+            settings: scrapy 的 settings 信息
+
+        Returns:
+            consul_conf_dict_min: 满足要求的最少要求的 consul 配置
+        """
+        consul_conf_dict = settings.get("CONSUL_CONFIG", {})
+        consul_conf_dict_lowered = cls.dict_keys_to_lower(consul_conf_dict)
+        return cls.get_items_by_keys(
+            dict_conf=consul_conf_dict_lowered, key_list=["token", "url", "format"]
+        )
+
+    @classmethod
+    def judge_str_is_json(cls, judge_str: str) -> bool:
+        """
+        判断字符串是否为 json 格式
+        Args:
+            judge_str: 需要判断的字符串
+
+        Returns:
+            1）.是否为 json 格式
+        """
+        if not isinstance(judge_str, str):
+            return False
+
+        try:
+            json.loads(judge_str)
+        except Exception as e:
+            return False
+        else:
+            return True
+
+    @staticmethod
+    def get_ck_dict_from_headers(headers_ck_str: str) -> dict:
+        """
+        从 headers 中的 ck str 格式转化为 dict 格式
+        Args:
+            headers_ck_str: request headers ck 的 str 格式
+
+        Returns:
+            1). 转化 dict 格式后的 ck
+        """
+        # 也可以这样写，但不推荐
+        # dict(line.split("=", 1) for line in headers_ck_str.split("; "))
+        return {
+            x.split("=", 1)[0].strip(): x.split("=", 1)[1].strip()
+            for x in headers_ck_str.split(";")
+        }
+
+    @staticmethod
+    def get_req_dict_from_scrapy(req_body_data_str: str) -> dict:
+        """
+        将 scrapy 请求中的 body 对象转为 dict 格式
+        Args:
+            req_body_data_str: scrapy 中的 body 参数
+
+        Returns:
+            1). 转化 dict 格式后的 body
+        """
+        return {
+            x.split("=", 1)[0]: x.split("=", 1)[1] for x in req_body_data_str.split("&")
+        }
+
+    @staticmethod
+    def get_array_dimension(array: list) -> int:
+        """
+        获取 array 的维度
+        Args:
+            array: 数组
+
+        Returns:
+            1).层级数
+        """
+        # 其实直接返回 len(array) 即可
+        return len(np.array(array).shape)
+
+    @classmethod
+    def get_array_depth(cls, array: list) -> int:
+        """
+        获取 array 的最大层级，深度
+        Args:
+            array: 数组
+
+        Returns:
+            1).最大层级，深度
+        """
+
+        """1 + max(map(depthCount,x)) if x and isinstance(x,list) else 0"""
+        # 先判断是否为数组类型的元素
+        judge_array = isinstance(
+            array,
+            (
+                frozenset,
+                list,
+                set,
+                tuple,
+            ),
+        )
+        return (
+            int(judge_array) and len(array) and 1 + max(map(cls.get_array_depth, array))
+        )
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/Params.py` & `ayugespidertools-1.1.7/ayugespidertools/common/Params.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
     NoneType = type(None)
     # 用于参数的描述
     I_Str = TypeVar("I_Str", int, str)
     B_Str = TypeVar("B_Str", bytes, str)
     I_Str_N = TypeVar("I_Str_N", int, str, NoneType)
     Str_Lstr = TypeVar("Str_Lstr", str, List[str])
+    PymongoDataBase = TypeVar("PymongoDataBase", bound="pymongo.database.Database")
+    PymysqlConnect = TypeVar("PymysqlConnect", bound="pymysql.connections.Connection")
+    PymysqlCursor = TypeVar("PymysqlCursor", bound="pymysql.cursors.Cursor")
+    PymysqlDictCursor = TypeVar("PymysqlDictCursor", bound="pymysql.cursors.DictCursor")
     # 此框架中 Item 的类型种类
     ScrapyItems = TypeVar(
         "ScrapyItems", MysqlDataItem, MongoDataItem, ScrapyClassicItem
     )
 
     # 基本的请求头
     base_headers = {
@@ -124,15 +128,15 @@
             "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/31.0.1623.0 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/30.0.1599.17 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.62 Safari/537.36",
             "Mozilla/5.0 (X11; CrOS i686 4319.74.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.57 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/29.0.1547.2 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1468.0 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1467.0 Safari/537.36",
-            "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1464.0 Safari/537.36",
+            "Mozilla/a/5.0 (Windows NT 6.2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/28.0.1464.0 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1500.55 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
             "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/SqlFormat.py` & `ayugespidertools-1.1.7/ayugespidertools/common/SqlFormat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional, Union
+from typing import Any, Dict, Literal, Optional, Union
 
 __all__ = [
     "AboutSql",
 ]
 
 SqlModeStr = Literal["and", "or"]
 
@@ -14,15 +14,15 @@
     或 pymilk 等第三方类似功能库的实现方法，以后会再优化此场景
     """
 
     @staticmethod
     def select_generate(
         db_table: str,
         key: list,
-        rule: dict,
+        rule: Dict[str, Any],
         base: SqlModeStr = "and",
         order_by: Optional[str] = None,
         limit: Union[bool, int] = False,
     ) -> (str, tuple):
         """
         根据一些参数来生成供 pymysql 之类的库中使用的 sql 查询语句（适用于简单情况）
         Args:
@@ -69,15 +69,15 @@
         keys = ", ".join(f"`{k}`" for k in data)
         values = ", ".join(["%s"] * len(data))
         sql = f"""insert into `{db_table}` ({keys}) values ({values})"""
         return sql, tuple(data.values())
 
     @staticmethod
     def update_generate(
-        db_table: str, data: dict, rule: dict, base: SqlModeStr = "and"
+        db_table: str, data: dict, rule: Dict[str, Any], base: SqlModeStr = "and"
     ) -> (str, tuple):
         """
         根据一些参数来生成供 pymysql 之类的库中使用的 sql 更新语句
         Args:
             db_table: 需要插入的表名称
             data: 需要更新的 key 和 value 值
             rule: 更新需要的规则
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/Utils.py` & `ayugespidertools-1.1.7/ayugespidertools/common/Utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,306 @@
-import copy
-import dataclasses
-import json
-import xml.etree.ElementTree as ET
-from typing import List, Literal, Optional, Union
-from urllib.parse import urlparse
-
-import hcl2
-import pandas
-import requests
-import yaml
-from itemadapter import ItemAdapter
-
-import ayugespidertools.Items
-from ayugespidertools.common.Encryption import EncryptOperation
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.config import logger
-from ayugespidertools.FormatData import DataHandle
-
-__all__ = [
-    "ToolsForAyu",
-]
-
-ConsulFormatStr = Literal["JSON", "HCL", "YAML", "XML"]
-ConsulConfNameStr = Literal["MONGODB", "MYSQL"]
-
-
-class ToolsForAyu(object):
-    """
-    这里用于存放框架所依赖的方法
-    """
-
-    @classmethod
-    def consul_get_all_group(cls, host: str, port: int, token: str) -> list:
-        """
-        获取 consul 的所有 group 信息
-        Args:
-            host: host
-            port: port
-            token: 请求 consul 所需要的 token 值
-
-        Returns:
-            1). consul 的所有 group 信息
-        """
-        curr_consul_headers = copy.deepcopy(Param.consul_headers)
-        curr_consul_headers["X-Consul-Token"] = token
-        r = requests.get(
-            url=f"http://{host}:{port}/v1/kv/?keys&dc=dc1&separator=%2F",
-            headers=curr_consul_headers,
-            verify=False,
-        )
-        return r.json()
-
-    @classmethod
-    def get_kvs_detail_by_consul(
-        cls,
-        url: str,
-        token: Optional[str] = None,
-    ) -> str:
-        """
-        获取 consul 的 key_values 的详细信息
-        Args:
-            token: consul token，最好只要有只读权限的 token 即可，如果未配置，则默认为 None。
-            url: 当前 consul 所需配置的 url
-
-        Returns:
-            conf_value: consul 的 group 下 key_values 的详细信息
-        """
-        url_params = urlparse(url).query
-
-        curr_consul_headers = copy.deepcopy(Param.consul_headers)
-        curr_consul_headers["X-Consul-Token"] = token
-        r = requests.get(url, headers=curr_consul_headers, verify=False)
-        # 判断是否返回的 raw 原始数据
-        if "raw" in url_params:
-            return r.text
-        return EncryptOperation.base64_decode(decode_data=r.json()[0]["Value"])
-
-    @classmethod
-    def get_conf_by_consul(
-        cls,
-        conf_name: ConsulConfNameStr,
-        url: str,
-        format: ConsulFormatStr = "json",
-        token: Optional[str] = None,
-    ):
-        """
-        获取 consul 中的 mysql 配置信息
-        Args:
-            conf_name: 需要获取的配置，本选项只有 "MYSQL" 和 "MONGODB"。
-            token: consul token，最好只要有只读权限的 token 即可，如果未配置，则默认为 None。
-            format: consul 中的配置格式，默认为 json 格式
-            url: 当前 consul 所需配置的 url
-
-        Returns:
-            1). consul 应用配置中心中的 Mysql 配置信息（key 值为小写）
-        """
-        conf_value = cls.get_kvs_detail_by_consul(url, token)
-        if format == "json":
-            conf_data = json.loads(conf_value)
-        elif format == "hcl":
-            conf_data = hcl2.loads(conf_value)
-        elif format == "yaml":
-            conf_data = yaml.safe_load(conf_value)
-        elif format == "xml":
-            root = ET.fromstring(conf_value)
-            # 将 XML 数据转换成 Python 字典
-            conf_data = {}
-            for child in root:
-                conf_data[child.tag] = {}
-                for sub_child in child:
-                    conf_data[child.tag][sub_child.tag] = sub_child.text
-        else:
-            raise ValueError("consul 暂不支持该格式的配置")
-
-        _conf = conf_data.get(conf_name, {})
-        if not _conf:
-            logger.info(f"consul 中未设置 {conf_name} 的配置信息")
-        return ReuseOperation.dict_keys_to_lower(_conf)
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_css(
-        cls, response, query: str, get_all: bool = False, return_selector: bool = False
-    ):
-        """
-        使用 scrapy 的 css 提取信息
-        Args:
-            response: scrapy response 或者是 selector 对象
-            query: css 提取的规则
-            get_all: 提取模式，默认：False, 提取符合中的一个
-            return_selector: 是否返回选择器对象
-
-        Returns:
-            1).提取的内容
-        """
-        if return_selector:
-            return response.css(query)
-        if get_all:
-            return response.css(query).getall()
-        else:
-            return response.css(query).get(default="").strip()
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_xpath(
-        cls, response, query: str, get_all: bool = False, return_selector: bool = False
-    ):
-        """
-        使用 scrapy 的 xpath 提取信息
-        Args:
-            response: scrapy response 或者是 selector 对象
-            query: css 提取的规则
-            get_all: 提取模式，默认：False, 提取符合中的一个
-            return_selector: 是否返回选择器对象
-
-        Returns:
-            1).提取的内容
-        """
-        if return_selector:
-            return response.xpath(query)
-        if get_all:
-            return response.xpath(query).getall()
-        else:
-            return response.xpath(query).get(default="").strip()
-
-    @classmethod
-    @DataHandle.simple_deal_for_extract
-    def extract_with_json(cls, json_data: dict, query: Union[str, List[str]]):
-        """
-        scrapy 中提取 json 数据遇到的情况
-        Args:
-            json_data: scrapy response 响应内容中的 json 格式数据
-            query: json 提取的规则
-
-        Returns:
-            1).提取的内容
-        """
-        # 如果输入的提取规则参数的格式为字符；或者参数格式是个列表，但是只含有一个元素的情况时
-        if any(
-            [isinstance(query, str), all([isinstance(query, list), len(query) == 1])]
-        ):
-            if isinstance(query, str):
-                return json_data.get(query, "")
-            return json_data.get(query[0], "")
-
-        # 循环取值时的处理
-        for curr_q in query:
-            # 这里循环时不对 json_data 的类型做判断，如果此时 json_data 类型无 get 方法，不处理
-            json_data = json_data.get(curr_q, "")
-            if not json_data:
-                return json_data
-        return json_data
-
-    @classmethod
-    def extract_with_json_rules(
-        cls, json_data: dict, query_rules: List[Param.Str_Lstr]
-    ):
-        """
-        当提取 json 某个数据时，可以在某些字段中取值，只要返回其中任意一个含有数据的值即可
-        Args:
-            json_data: scrapy response 响应内容中的 json 格式数据
-            query_rules: json 提取的规则列表
-
-        Returns:
-            1).提取的内容
-        """
-        # 先判断层级，最多为 2 层
-        depth_num = ReuseOperation.get_array_depth(query_rules)
-        assert depth_num <= 2, "query_rules 参数错误，请输入深度最多为 2 的参数！"
-
-        for query in query_rules:
-            if extract_res := cls.extract_with_json(json_data=json_data, query=query):
-                return extract_res
-        return ""
-
-    @staticmethod
-    def get_collate_by_charset(mysql_conf: dict) -> str:
-        """
-        根据 mysql 的 charset 获取对应默认的 collate
-        Args:
-            mysql_conf: mysql 连接配置
-
-        Returns:
-            collate: 排序规则
-        """
-        charset_collate_map = {
-            # utf8mb4_unicode_ci 也是经常使用的
-            "utf8mb4": "utf8mb4_general_ci",
-            "utf8": "utf8_general_ci",
-            "gbk": "gbk_chinese_ci",
-            "latin1": "latin1_swedish_ci",
-            "utf16": "utf16_general_ci",
-            "utf16le": "utf16le_general_ci",
-            "cp1251": "cp1251_general_ci",
-            "euckr": "euckr_korean_ci",
-            "greek": "greek_general_ci",
-        }
-        collate = charset_collate_map.get(mysql_conf["charset"])
-        assert (
-            collate is not None
-        ), f"数据库配置出现未知 charset：{mysql_conf['charset']}，若抛错请查看或手动创建所需数据表！"
-        return collate
-
-    @staticmethod
-    def convert_item_to_dict(item) -> dict:
-        """
-        将 item 结构数据转为 dict 格式（这种转换方法太过啰嗦，已放弃，请使用下面的 convert_items_to_dict 方法）
-        Args:
-            item: 需要转换的参数
-
-        Returns:
-            1). 转换为 dict 格式的结果
-        """
-        # MongoDataItem 等其它的场景不再转换为 dict，直接使用 dataclass 即可
-        if isinstance(item, ayugespidertools.Items.MysqlDataItem):
-            return dataclasses.asdict(item)
-
-        elif isinstance(item, dict):
-            return item
-
-        elif isinstance(item, ayugespidertools.Items.ScrapyClassicItem):
-            return dict(item)
-
-        else:
-            logger.warning(f"出现未知 item 格式，item: {item}")
-            return dict(item)
-
-    @staticmethod
-    def convert_items_to_dict(item) -> ItemAdapter:
-        """
-        数据容器对象的包装器，提供了一个通用接口以统一的方式处理不同类型的对象，而不管它们的底层实现如何。
-        目前支持的类型有：
-            1. scrapy.item.Item
-            2. dict
-            3. dataclass 基础类
-            4. attrs 基础类
-            5. pydantic 基础类
-        Args:
-            item: 需要转换的项目，请查看支持类型
-
-        Returns:
-            1). 转换的 ItemAdapter 结果，可以通过  obj["params"] 或 obj.get("params") 来取值
-        """
-        return ItemAdapter(item)
-
-    @staticmethod
-    def get_dict_form_scrapy_req_headers(scrapy_headers) -> dict:
-        """
-        根据 scrapy request 中的 headers 信息转化为正常的 dict 格式
-        Args:
-            scrapy_headers: scrapy 的 request headers 内容
-
-        Returns:
-            req_headers: 转化 dict 后的 headers 内容
-        """
-        return {
-            str(b_key, encoding="utf-8"): str(b_value_list[0], encoding="utf-8")
-            for b_key, b_value_list in dict(scrapy_headers).items()
-        }
-
-    @staticmethod
-    def filter_data_before_yield(
-        sql: str,
-        mysql_engine,
-        item: Param.ScrapyItems,
-    ) -> Param.ScrapyItems:
-        """
-        数据入库前查询是否已存在，已存在则跳过
-        Args:
-            sql: 判断的 sql
-            mysql_engine: sqlalchemy 的 create_engine 句柄
-            item: 当前 scrapy item
-
-        Returns:
-            item: 当前 scrapy item
-        """
-        # 数据入库逻辑
-        try:
-            df = pandas.read_sql(sql, mysql_engine)
-            # 如果为空，说明此数据不存在于数据库，则新增
-            if df.empty:
-                return item
-
-        except Exception as e:
-            # 若数据库或数据表不存在时，直接返回 item 即可，会自动创建所依赖的数据库数据表及字段注释（前提是用户有对应权限，否则还是会报错）
-            if any(["1146" in str(e), "1054" in str(e), "doesn't exist" in str(e)]):
-                return item
-            else:
-                raise ValueError(f"请查看网络是否通畅，或 sql 是否正确！Error: {e}") from e
+import copy
+import json
+import xml.etree.ElementTree as ET
+from typing import List, Literal, Optional, Union
+from urllib.parse import urlparse
+
+import hcl2
+import pandas
+import requests
+import yaml
+from itemadapter import ItemAdapter
+
+from ayugespidertools.common.Encryption import EncryptOperation
+from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.Params import Param
+from ayugespidertools.common.TypeVars import MysqlConfig
+from ayugespidertools.config import logger
+from ayugespidertools.FormatData import DataHandle
+
+__all__ = [
+    "ToolsForAyu",
+]
+
+ConsulFormatStr = Literal["JSON", "HCL", "YAML", "XML"]
+ConsulConfNameStr = Literal["MONGODB", "MYSQL"]
+
+
+class ToolsForAyu(object):
+    """
+    这里用于存放框架所依赖的方法
+    """
+
+    @classmethod
+    def consul_get_all_group(cls, host: str, port: int, token: str) -> list:
+        """
+        获取 consul 的所有 group 信息
+        Args:
+            host: host
+            port: port
+            token: 请求 consul 所需要的 token 值
+
+        Returns:
+            1). consul 的所有 group 信息
+        """
+        curr_consul_headers = copy.deepcopy(Param.consul_headers)
+        curr_consul_headers["X-Consul-Token"] = token
+        r = requests.get(
+            url=f"http://{host}:{port}/v1/kv/?keys&dc=dc1&separator=%2F",
+            headers=curr_consul_headers,
+            verify=False,
+        )
+        return r.json()
+
+    @classmethod
+    def get_kvs_detail_by_consul(
+        cls,
+        url: str,
+        token: Optional[str] = None,
+    ) -> str:
+        """
+        获取 consul 的 key_values 的详细信息
+        Args:
+            token: consul token，最好只要有只读权限的 token 即可，如果未配置，则默认为 None。
+            url: 当前 consul 所需配置的 url
+
+        Returns:
+            conf_value: consul 的 group 下 key_values 的详细信息
+        """
+        url_params = urlparse(url).query
+
+        curr_consul_headers = copy.deepcopy(Param.consul_headers)
+        curr_consul_headers["X-Consul-Token"] = token
+        r = requests.get(url, headers=curr_consul_headers, verify=False)
+        # 判断是否返回的 raw 原始数据
+        if "raw" in url_params:
+            return r.text
+        return EncryptOperation.base64_decode(decode_data=r.json()[0]["Value"])
+
+    @classmethod
+    def get_conf_by_consul(
+        cls,
+        conf_name: ConsulConfNameStr,
+        url: str,
+        format: ConsulFormatStr = "json",
+        token: Optional[str] = None,
+    ) -> dict:
+        """
+        获取 consul 中的 mysql 配置信息
+        Args:
+            conf_name: 需要获取的配置，本选项只有 "MYSQL" 和 "MONGODB"。
+            token: consul token，最好只要有只读权限的 token 即可，如果未配置，则默认为 None。
+            format: consul 中的配置格式，默认为 json 格式
+            url: 当前 consul 所需配置的 url
+
+        Returns:
+            1). consul 应用配置中心中的 Mysql 配置信息（key 值为小写）
+        """
+        conf_value = cls.get_kvs_detail_by_consul(url, token)
+        if format == "json":
+            conf_data = json.loads(conf_value)
+        elif format == "hcl":
+            conf_data = hcl2.loads(conf_value)
+        elif format == "yaml":
+            conf_data = yaml.safe_load(conf_value)
+        elif format == "xml":
+            root = ET.fromstring(conf_value)
+            # 将 XML 数据转换成 Python 字典
+            conf_data = {}
+            for child in root:
+                conf_data[child.tag] = {}
+                for sub_child in child:
+                    conf_data[child.tag][sub_child.tag] = sub_child.text
+        else:
+            raise ValueError("consul 暂不支持该格式的配置")
+
+        _conf = conf_data.get(conf_name, {})
+        if not _conf:
+            logger.info(f"consul 中未设置 {conf_name} 的配置信息")
+        return ReuseOperation.dict_keys_to_lower(_conf)
+
+    @classmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_css(
+        cls, response, query: str, get_all: bool = False, return_selector: bool = False
+    ):
+        """
+        使用 scrapy 的 css 提取信息
+        Args:
+            response: scrapy response 或者是 selector 对象
+            query: css 提取的规则
+            get_all: 提取模式，默认：False, 提取符合中的一个
+            return_selector: 是否返回选择器对象
+
+        Returns:
+            1).提取的内容
+        """
+        if return_selector:
+            return response.css(query)
+        if get_all:
+            return response.css(query).getall()
+        else:
+            return response.css(query).get(default="").strip()
+
+    @classmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_xpath(
+        cls, response, query: str, get_all: bool = False, return_selector: bool = False
+    ):
+        """
+        使用 scrapy 的 xpath 提取信息
+        Args:
+            response: scrapy response 或者是 selector 对象
+            query: css 提取的规则
+            get_all: 提取模式，默认：False, 提取符合中的一个
+            return_selector: 是否返回选择器对象
+
+        Returns:
+            1).提取的内容
+        """
+        if return_selector:
+            return response.xpath(query)
+        if get_all:
+            return response.xpath(query).getall()
+        else:
+            return response.xpath(query).get(default="").strip()
+
+    @classmethod
+    @DataHandle.simple_deal_for_extract
+    def extract_with_json(cls, json_data: dict, query: Union[str, List[str]]):
+        """
+        scrapy 中提取 json 数据遇到的情况
+        Args:
+            json_data: scrapy response 响应内容中的 json 格式数据
+            query: json 提取的规则
+
+        Returns:
+            1).提取的内容
+        """
+        # 如果输入的提取规则参数的格式为字符；或者参数格式是个列表，但是只含有一个元素的情况时
+        if any(
+            [isinstance(query, str), all([isinstance(query, list), len(query) == 1])]
+        ):
+            if isinstance(query, str):
+                return json_data.get(query, "")
+            return json_data.get(query[0], "")
+
+        # 循环取值时的处理
+        for curr_q in query:
+            # 这里循环时不对 json_data 的类型做判断，如果此时 json_data 类型无 get 方法，不处理
+            json_data = json_data.get(curr_q, "")
+            if not json_data:
+                return json_data
+        return json_data
+
+    @classmethod
+    def extract_with_json_rules(
+        cls, json_data: dict, query_rules: List[Param.Str_Lstr]
+    ):
+        """
+        当提取 json 某个数据时，可以在某些字段中取值，只要返回其中任意一个含有数据的值即可
+        Args:
+            json_data: scrapy response 响应内容中的 json 格式数据
+            query_rules: json 提取的规则列表
+
+        Returns:
+            1).提取的内容
+        """
+        # 先判断层级，最多为 2 层
+        depth_num = ReuseOperation.get_array_depth(query_rules)
+        assert depth_num <= 2, "query_rules 参数错误，请输入深度最多为 2 的参数！"
+
+        for query in query_rules:
+            if extract_res := cls.extract_with_json(json_data=json_data, query=query):
+                return extract_res
+        return ""
+
+    @staticmethod
+    def get_collate_by_charset(mysql_conf: MysqlConfig) -> str:
+        """
+        根据 mysql 的 charset 获取对应默认的 collate
+        Args:
+            mysql_conf: mysql 连接配置
+
+        Returns:
+            collate: 排序规则
+        """
+        charset_collate_map = {
+            # utf8mb4_unicode_ci 也是经常使用的
+            "utf8mb4": "utf8mb4_general_ci",
+            "utf8": "utf8_general_ci",
+            "gbk": "gbk_chinese_ci",
+            "latin1": "latin1_swedish_ci",
+            "utf16": "utf16_general_ci",
+            "utf16le": "utf16le_general_ci",
+            "cp1251": "cp1251_general_ci",
+            "euckr": "euckr_korean_ci",
+            "greek": "greek_general_ci",
+        }
+        collate = charset_collate_map.get(mysql_conf.charset)
+        assert (
+            collate is not None
+        ), f"数据库配置出现未知 charset：{mysql_conf.charset}，若抛错请查看或手动创建所需数据表！"
+        return collate
+
+    @staticmethod
+    def convert_items_to_dict(item) -> ItemAdapter:
+        """
+        数据容器对象的包装器，提供了一个通用接口以统一的方式处理不同类型的对象，而不管它们的底层实现如何。
+        目前支持的类型有：
+            1. scrapy.item.Item
+            2. dict
+            3. dataclass 基础类
+            4. attrs 基础类
+            5. pydantic 基础类
+        Args:
+            item: 需要转换的项目，请查看支持类型
+
+        Returns:
+            1). 转换的 ItemAdapter 结果，可以通过  obj["params"] 或 obj.get("params") 来取值
+        """
+        return ItemAdapter(item)
+
+    @staticmethod
+    def get_dict_form_scrapy_req_headers(scrapy_headers) -> dict:
+        """
+        根据 scrapy request 中的 headers 信息转化为正常的 dict 格式
+        Args:
+            scrapy_headers: scrapy 的 request headers 内容
+
+        Returns:
+            req_headers: 转化 dict 后的 headers 内容
+        """
+        return {
+            str(b_key, encoding="utf-8"): str(b_value_list[0], encoding="utf-8")
+            for b_key, b_value_list in dict(scrapy_headers).items()
+        }
+
+    @staticmethod
+    def filter_data_before_yield(
+        sql: str,
+        mysql_engine,
+        item: Param.ScrapyItems,
+    ) -> Param.ScrapyItems:
+        """
+        数据入库前查询是否已存在，已存在则跳过
+        Args:
+            sql: 判断的 sql
+            mysql_engine: sqlalchemy 的 create_engine 句柄
+            item: 当前 scrapy item
+
+        Returns:
+            item: 当前 scrapy item
+        """
+        # 数据入库逻辑
+        try:
+            df = pandas.read_sql(sql, mysql_engine)
+            # 如果为空，说明此数据不存在于数据库，则新增
+            if df.empty:
+                return item
+
+        except Exception as e:
+            # 若数据库或数据表不存在时，直接返回 item 即可，会自动创建所依赖的数据库数据表及字段注释（前提是用户有对应权限，否则还是会报错）
+            if any(["1146" in str(e), "1054" in str(e), "doesn't exist" in str(e)]):
+                return item
+            else:
+                raise ValueError(f"请查看网络是否通畅，或 sql 是否正确！Error: {e}") from e
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/common/YiDunGap.py` & `ayugespidertools-1.1.7/ayugespidertools/common/YiDunGap.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/http/request/form.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/headers/ua.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/headers/ua.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,24 +15,22 @@
     """
 
     def __init__(self):
         self.explorer_types = None
         self.explorer_weights = None
 
     def get_random_ua_by_weight(self) -> str:
-        """根据权重来获取随机请求头 ua 信息"""
         # 先按权重取出所需浏览器类型
         explorer_types = random.choices(
             self.explorer_types, weights=self.explorer_weights
         )
         return random.choice(Param.fake_useragent_dict[explorer_types[0]])
 
     @classmethod
     def from_crawler(cls, crawler):
-        # This method is used by Scrapy to create your spiders.
         s = cls()
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def spider_opened(self, spider):
         # 带权重的 ua 列表，将比较常用的 ua 标识的权重设置高一点。这里是根据 fake_useragent 库中的打印信息来规划权重的。
         ua_arr = [
@@ -43,9 +41,10 @@
             {"explorer": "chrome", "weight": 772},
         ]
         self.explorer_types = [x["explorer"] for x in ua_arr]
         self.explorer_weights = [x["weight"] for x in ua_arr]
         spider.slog.info(f"随机请求头中间件 RandomRequestUaMiddleware 已开启，生效脚本为: {spider.name}")
 
     def process_request(self, request, spider):
+        # 根据权重来获取随机请求头 ua 信息
         if curr_ua := self.get_random_ua_by_weight():
             request.headers.setdefault(b"User-Agent", curr_ua)
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/netlib/requestslib.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/netlib/requestslib.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 status=r_response.status_code,
                 body=r_response.text,
                 request=request,
                 encoding="utf-8",
             )
 
         except Exception as e:
-            """这里比较重要，还是推荐捕获所有错误；不建议只抛错 requests.exceptions.ConnectTimeout:"""
+            # 这里比较重要，还是推荐捕获所有错误；不建议只抛错 requests.exceptions.ConnectTimeout:
             return HtmlResponse(
                 url=request.url,
                 status=202,
                 body=f"requests 请求出现错误：{e}",
                 request=request,
                 encoding="utf-8",
             )
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/dynamic.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
         self.proxy_url = dynamic_proxy_conf["PROXY_URL"]
         self.username = dynamic_proxy_conf["USERNAME"]
         self.password = dynamic_proxy_conf["PASSWORD"]
 
     @classmethod
     def from_crawler(cls, crawler):
-        # This method is used by Scrapy to create your spiders.
         s = cls(crawler.settings)
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def process_request(self, request, spider):
         # TODO: 根据权重来随机获取一个账号 DYNAMIC_PROXY_CONFIG
         # account = ReuseOperation.random_weight(self.account_arr)
@@ -82,15 +81,14 @@
 
         self.proxy_url = dynamic_proxy_conf["PROXY_URL"]
         self.username = dynamic_proxy_conf["USERNAME"]
         self.password = dynamic_proxy_conf["PASSWORD"]
 
     @classmethod
     def from_crawler(cls, crawler):
-        # This method is used by Scrapy to create your spiders.
         s = cls(crawler.settings)
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def spider_opened(self, spider):
         spider.slog.info(
             f"阿布云动态隧道代理中间件: AbuDynamicProxyDownloaderMiddleware 已开启，生效脚本为: {spider.name}"
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/exclusive.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self.proxy_url = exclusive_proxy_conf["PROXY_URL"]
         self.username = exclusive_proxy_conf["USERNAME"]
         self.password = exclusive_proxy_conf["PASSWORD"]
         self.proxy_index = exclusive_proxy_conf["PROXY_INDEX"]
 
     @classmethod
     def from_crawler(cls, crawler):
-        # This method is used by Scrapy to create your spiders.
         s = cls(
             exclusive_proxy_conf=crawler.settings.get("EXCLUSIVE_PROXY_CONFIG", None)
         )
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         return s
 
     def get_proxy_ip(self):
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/middlewares/proxy/private.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/middlewares/proxy/private.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         self.settings = Settings()
         super(PrivateProxyDownloaderMiddleware, self).__init__(self.settings)
         self.important_error = False
         self.WWX = WWXRobot(key=wwx_robot_key)
 
     @classmethod
     def from_crawler(cls, crawler):
-        # This method is used by Scrapy to create your spiders.
         s = cls(wwx_robot_key=crawler.settings.get("WWXRobot_key", None))
         crawler.signals.connect(s.spider_opened, signal=signals.spider_opened)
         crawler.signals.connect(s.spider_closed, signal=signals.spider_closed)
         return s
 
     @retry(stop_max_attempt_number=Param.retry_num)
     def get_proxy_ip(self, size, isdict: Optional[bool] = None):
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/download/file.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/download/image.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/download/image.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,371 +1,336 @@
-import datetime
-import warnings
-from typing import Optional, Type
-
-import pymysql
-from retrying import retry
-
-from ayugespidertools.common.Expend import MysqlErrorHandlingMixin
-from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Params import Param
-from ayugespidertools.common.TypeVars import TableEnumTypeVar
-from ayugespidertools.common.Utils import ToolsForAyu
-
-# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
-warnings.filterwarnings(
-    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
-)
-
-__all__ = [
-    "AyuMysqlPipeline",
-]
-
-
-class AyuMysqlPipeline(MysqlErrorHandlingMixin):
-    """
-    Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
-    """
-
-    def __init__(
-        self,
-        table_prefix: str,
-        table_enum: Type[TableEnumTypeVar],
-        env: str,
-        record_log_to_mysql: Optional[bool] = False,
-    ) -> None:
-        """
-        初始化 Mysql 链接所需要的信息
-        Args:
-            table_prefix: 数据库表前缀
-            table_enum: 数据表的枚举信息
-            env: 当前程序部署环境名
-            record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
-        """
-        self.table_prefix = table_prefix
-        self.table_enum = table_enum
-        self.env = env
-        self.record_log_to_mysql = record_log_to_mysql
-        # 排序规则，用于创建数据库时使用
-        self.collate = None
-        self.mysql_conf = None
-        self.conn = None
-        self.slog = None
-        self.cursor = None
-        self.crawl_time = datetime.date.today()
-
-    @classmethod
-    def from_crawler(cls, crawler):
-        return cls(
-            # 数据库表前缀
-            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
-            # 数据库表枚举是否开启
-            table_enum=crawler.settings.get("DATA_ENUM"),
-            # 获取部署的环境
-            env=crawler.settings.get("ENV"),
-            # 当 record_log_to_mysql 为 True 时，会记录运行情况
-            record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
-        )
-
-    def open_spider(self, spider):
-        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
-
-        self.slog = spider.slog
-        self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
-        self.conn = self._connect(self.mysql_conf)
-        self.cursor = self.conn.cursor()
-
-    def get_table_name(self, table: str) -> str:
-        """
-        组合完整的数据库表
-        Args:
-            table: 数据表的后缀
-
-        Returns:
-            1). 拼接成完整的数据表的值
-        """
-        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
-        full_table_name = f"{self.table_prefix}{table}"
-
-        # 最终的数据表名不能含有空格
-        assert (
-            " " not in full_table_name
-        ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
-        return full_table_name
-
-    def get_new_item(self, item):
-        """
-        重新整合 item
-        Args:
-            item: scrapy yield 的 item 信息
-
-        Returns:
-            1). 整合后的 item
-        """
-        new_item = {}
-        notes_dic = {}
-        # 如果是 ayugespidertools.Items 中的各个自封装类型时
-        # alldata 可以认为是关键字，需要判断其是否存在，且是否为 dict。
-        # 若其存在且为 dict，则默认其为 Items 中的 alldata 数据类型而非单一字段值
-        insert_data = item.get("alldata")
-        if all([insert_data, isinstance(insert_data, dict)]):
-            judge_item = next(iter(insert_data.values()))
-            # 是 namedtuple 类型
-            if ReuseOperation.is_namedtuple_instance(judge_item):
-                for key, value in insert_data.items():
-                    new_item[key] = value.key_value
-                    notes_dic[key] = value.notes
-            # 是双层 dict 格式
-            elif isinstance(judge_item, dict):
-                for key, value in insert_data.items():
-                    new_item[key] = value.get("key_value", "")
-                    notes_dic[key] = value["notes"]
-            # 其它默认为单层 dict 格式
-            else:
-                for key, value in insert_data.items():
-                    new_item[key] = value
-                    notes_dic[key] = key
-
-        # 兼容旧写法，直接 dict 格式的 item 即可
-        else:
-            # 将存入表的无关字段给去掉
-            save_data_item = ReuseOperation.get_items_except_keys(
-                dict_conf=item, key_list=["table", "item_mode"]
-            )
-            for key, value in save_data_item.items():
-                new_item[key] = value
-                notes_dic[key] = key
-
-        return {"new_item": new_item, "notes_dic": notes_dic}
-
-    def process_item(self, item, spider):
-        item_dict = ToolsForAyu.convert_items_to_dict(item)
-        # 先查看存储场景是否匹配
-        if item_dict["item_mode"] == "Mysql":
-            self.insert_item(
-                self.get_new_item(item_dict), self.get_table_name(item_dict["table"])
-            )
-        return item
-
-    def insert_item(self, item_o, table):
-        """
-        通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
-        Args:
-            item_o: item
-            table: 数据库表名
-
-        Returns:
-            None
-        """
-        if not (new_item := item_o.get("new_item")):
-            return
-
-        note_dic = item_o.get("notes_dic")
-        keys = f"""`{"`, `".join(new_item.keys())}`"""
-        values = ", ".join(["%s"] * len(new_item))
-        update = ",".join([f" `{key}` = %s" for key in new_item])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-
-        try:
-            if self.cursor.execute(sql, tuple(new_item.values()) * 2):
-                self.conn.commit()
-
-        except Exception as e:
-            self.slog.warning(f":{e}")
-            self.slog.warning(f"Item:{new_item}  Table: {table}")
-            self.conn.rollback()
-            err_msg = str(e)
-            if "1054" in err_msg:
-                self.deal_1054_error(
-                    err_msg=err_msg,
-                    conn=self.conn,
-                    cursor=self.cursor,
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.insert_item(item_o, table)
-
-            elif "1146" in err_msg:
-                self.deal_1146_error(
-                    err_msg=err_msg,
-                    table_prefix=self.table_prefix,
-                    cursor=self.cursor,
-                    charset=self.mysql_conf["charset"],
-                    collate=self.collate,
-                    table_enum=self.table_enum,
-                )
-                return self.insert_item(item_o, table)
-
-            elif "1406" in err_msg:
-                self.deal_1406_error(
-                    err_msg=err_msg,
-                    conn=self.conn,
-                    cursor=self.cursor,
-                    database=self.mysql_conf["database"],
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.insert_item(item_o, table)
-
-            elif "1265" in err_msg:
-                self.deal_1265_error(
-                    err_msg=err_msg,
-                    conn=self.conn,
-                    cursor=self.cursor,
-                    database=self.mysql_conf["database"],
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.insert_item(item_o, table)
-
-            else:
-                # 碰到其他的异常才打印错误日志，已处理的异常不打印
-                self.slog.error(f"ERROR:{e}")
-
-    def close_spider(self, spider):
-        # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
-        if self.record_log_to_mysql:
-            log_info = self._get_log_by_spider(
-                spider=spider, crawl_time=self.crawl_time
-            )
-
-            # 运行脚本统计信息
-            self.insert_script_statistics(log_info)
-            self.table_collection_statistics(
-                spider_name=spider.name,
-                database=spider.mysql_conf["database"],
-                crawl_time=self.crawl_time,
-            )
-
-        if self.conn:
-            self.conn.close()
-
-    def table_collection_statistics(
-        self, spider_name: str, database: str, crawl_time: datetime.date
-    ):
-        """
-        统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
-        Args:
-            spider_name: 爬虫脚本名称
-            database: 数据库，保存程序采集记录保存的数据库
-            crawl_time: 采集时间，程序运行时间
-
-        Returns:
-            None
-        """
-        sql = f"""
-        select concat(
-            'select "',
-            TABLE_NAME,
-            '", count(id) as num , crawl_time from ',
-            TABLE_SCHEMA,
-            '.',
-            TABLE_NAME,
-                ' where crawl_time = "{crawl_time}"'
-        ) from information_schema.tables
-        where TABLE_SCHEMA='{database}' and TABLE_NAME in (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
-        """
-        self.cursor.execute(sql)
-        results = self.cursor.fetchall()
-        if sql_list := [row[0] for row in results]:
-            sql_all = " union all ".join(sql_list)
-            self.cursor.execute(sql_all)
-            results = self.cursor.fetchall()
-
-            for row in results:
-                table_statistics = {
-                    "spider_name": spider_name,
-                    "database": database,
-                    "table_name": row[0],
-                    "number": row[1],
-                    "crawl_time": str((row[2] or crawl_time)),
-                }
-                self.insert_table_statistics(table_statistics)
-
-    def insert_table_statistics(
-        self, data: dict, table: str = "table_collection_statistics"
-    ):
-        """
-        插入统计数据到表中
-        Args:
-            data: 需要统计的入库信息
-            table: 存储表的名称
-
-        Returns:
-            None
-        """
-        self.cursor.execute(
-            f"""
-            CREATE TABLE IF NOT EXISTS `{table}` (
-            `id` int(11) NOT NULL AUTO_INCREMENT,
-            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',            
-            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
-            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',            
-            PRIMARY KEY (`id`) USING BTREE
-            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
-            """
-        )
-
-        keys = f"""`{"`, `".join(data.keys())}`"""
-        values = ", ".join(["%s"] * len(data))
-        update = ",".join([f" `{key}` = %s" for key in data])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-        try:
-            if self.cursor.execute(sql, tuple(data.values()) * 2):
-                self.conn.commit()
-        except Exception as e:
-            self.conn.rollback()
-            self.slog.warning(f":{e}")
-
-    @retry(
-        stop_max_attempt_number=Param.retry_num,
-        wait_random_min=Param.retry_time_min,
-        wait_random_max=Param.retry_time_max,
-    )
-    def insert_script_statistics(
-        self, data: dict, table: str = "script_collection_statistics"
-    ):
-        """
-        存储运行脚本的统计信息
-        Args:
-            data: 需要插入的 log 信息
-            table: 存储表的名称
-
-        Returns:
-            None
-        """
-        self.cursor.execute(
-            f"""
-            CREATE TABLE IF NOT EXISTS `{table}` (
-            `id` int(11) NOT NULL AUTO_INCREMENT,
-            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
-            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
-            `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
-            `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
-            `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
-            `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
-            `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
-            `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
-            `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
-            `start_time` datetime NOT NULL COMMENT '开始时间',
-            `finish_time` datetime NOT NULL COMMENT '结束时间',
-            `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
-            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
-            `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
-            PRIMARY KEY (`id`) USING BTREE
-            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
-            """
-        )
-
-        keys = f"""`{"`, `".join(data.keys())}`"""
-        values = ", ".join(["%s"] * len(data))
-        update = ",".join([f" `{key}` = %s" for key in data])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
-        try:
-            if self.cursor.execute(sql, tuple(data.values()) * 2):
-                self.conn.commit()
-        except Exception as e:
-            self.conn.rollback()
-            self.slog.warning(f":{e}")
+import datetime
+import warnings
+from typing import Optional, Type
+
+import pymysql
+from retrying import retry
+
+from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
+from ayugespidertools.common.MultiPlexing import ReuseOperation
+from ayugespidertools.common.MysqlErrorHandle import Synchronize, deal_mysql_err
+from ayugespidertools.common.Params import Param
+from ayugespidertools.common.TypeVars import MysqlConfig, TableEnumTypeVar
+from ayugespidertools.common.Utils import ToolsForAyu
+
+# 将 pymysql 中 Data truncated for column 警告类型置为 Error，其他警告忽略
+warnings.filterwarnings(
+    "error", category=pymysql.Warning, message=".*Data truncated for column.*"
+)
+
+__all__ = [
+    "AyuMysqlPipeline",
+]
+
+
+class AyuMysqlPipeline(MysqlPipeEnhanceMixin):
+    """
+    Mysql 存储场景的 scrapy pipeline 扩展的主要功能示例
+    """
+
+    def __init__(
+        self,
+        table_prefix: str,
+        table_enum: Type[TableEnumTypeVar],
+        env: str,
+        record_log_to_mysql: Optional[bool] = False,
+    ) -> None:
+        """
+        初始化 Mysql 链接所需要的信息
+        Args:
+            table_prefix: 数据库表前缀
+            table_enum: 数据表的枚举信息
+            env: 当前程序部署环境名
+            record_log_to_mysql: 是否需要记录程序采集的基本信息到 Mysql 中
+        """
+        self.table_prefix = table_prefix
+        self.table_enum = table_enum
+        self.env = env
+        self.record_log_to_mysql = record_log_to_mysql
+        # 排序规则，用于创建数据库时使用
+        self.collate = None
+        self.mysql_conf: Optional[MysqlConfig] = None
+        self.conn = None
+        self.slog = None
+        self.cursor = None
+        self.crawl_time = datetime.date.today()
+
+    @classmethod
+    def from_crawler(cls, crawler):
+        return cls(
+            # 数据库表前缀
+            table_prefix=crawler.settings.get("MYSQL_TABLE_PREFIX", ""),
+            # 数据库表枚举是否开启
+            table_enum=crawler.settings.get("DATA_ENUM"),
+            # 获取部署的环境
+            env=crawler.settings.get("ENV"),
+            # 当 record_log_to_mysql 为 True 时，会记录运行情况
+            record_log_to_mysql=crawler.settings.get("RECORD_LOG_TO_MYSQL", False),
+        )
+
+    def open_spider(self, spider):
+        assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
+
+        self.slog = spider.slog
+        self.mysql_conf = spider.mysql_conf
+        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
+        self.conn = self._connect(self.mysql_conf)
+        self.cursor = self.conn.cursor()
+
+    def get_table_name(self, table: str) -> str:
+        """
+        组合完整的数据库表
+        Args:
+            table: 数据表的后缀
+
+        Returns:
+            1). 拼接成完整的数据表的值
+        """
+        assert isinstance(table, str), "item 中 table 字段不是 str，或未传入 table 参数"
+        full_table_name = f"{self.table_prefix}{table}"
+
+        # 最终的数据表名不能含有空格
+        assert (
+            " " not in full_table_name
+        ), "数据表名不能含空格，请检查 MYSQL_TABLE_PREFIX 参数和 item 中的 table 参数"
+        return full_table_name
+
+    def get_new_item(self, item):
+        """
+        重新整合 item
+        Args:
+            item: scrapy yield 的 item 信息
+
+        Returns:
+            1). 整合后的 item
+        """
+        new_item = {}
+        notes_dic = {}
+        # 如果是 ayugespidertools.Items 中的各个自封装类型时
+        # alldata 可以认为是关键字，需要判断其是否存在，且是否为 dict。
+        # 若其存在且为 dict，则默认其为 Items 中的 alldata 数据类型而非单一字段值
+        insert_data = item.get("alldata")
+        if all([insert_data, isinstance(insert_data, dict)]):
+            judge_item = next(iter(insert_data.values()))
+            # 是 namedtuple 类型
+            if ReuseOperation.is_namedtuple_instance(judge_item):
+                for key, value in insert_data.items():
+                    new_item[key] = value.key_value
+                    notes_dic[key] = value.notes
+            # 是双层 dict 格式
+            elif isinstance(judge_item, dict):
+                for key, value in insert_data.items():
+                    new_item[key] = value.get("key_value", "")
+                    notes_dic[key] = value["notes"]
+            # 其它默认为单层 dict 格式
+            else:
+                for key, value in insert_data.items():
+                    new_item[key] = value
+                    notes_dic[key] = key
+
+        # 兼容旧写法，直接 dict 格式的 item 即可
+        else:
+            # 将存入表的无关字段给去掉
+            save_data_item = ReuseOperation.get_items_except_keys(
+                dict_conf=item, key_list=["table", "item_mode"]
+            )
+            for key, value in save_data_item.items():
+                new_item[key] = value
+                notes_dic[key] = key
+
+        return {"new_item": new_item, "notes_dic": notes_dic}
+
+    def process_item(self, item, spider):
+        item_dict = ToolsForAyu.convert_items_to_dict(item)
+        # 先查看存储场景是否匹配
+        if item_dict["item_mode"] == "Mysql":
+            self.insert_item(
+                self.get_new_item(item_dict), self.get_table_name(item_dict["table"])
+            )
+        return item
+
+    def insert_item(self, item_o, table):
+        """
+        通用插入数据，将 item 数据存入 Mysql 中，item 中的 key 需要跟 Mysql 数据中的字段名称一致
+        Args:
+            item_o: item
+            table: 数据库表名
+
+        Returns:
+            None
+        """
+        if not (new_item := item_o.get("new_item")):
+            return
+
+        note_dic = item_o.get("notes_dic")
+        sql = self._get_sql_by_item(table=table, item=new_item)
+
+        try:
+            if self.cursor.execute(sql, tuple(new_item.values()) * 2):
+                self.conn.commit()
+
+        except Exception as e:
+            self.slog.warning(f":{e}")
+            self.slog.warning(f"Item:{new_item}  Table: {table}")
+            self.conn.rollback()
+            deal_mysql_err(
+                Synchronize(),
+                err_msg=str(e),
+                conn=self.conn,
+                cursor=self.cursor,
+                charset=self.mysql_conf.charset,
+                collate=self.collate,
+                database=self.mysql_conf.database,
+                table=table,
+                table_prefix=self.table_prefix,
+                table_enum=self.table_enum,
+                note_dic=note_dic,
+            )
+            return self.insert_item(item_o, table)
+
+    def close_spider(self, spider):
+        # 是否记录程序采集的基本信息到 Mysql 中，只有打开 record_log_to_mysql 配置才会收集和存储相关的统计信息
+        if self.record_log_to_mysql:
+            log_info = self._get_log_by_spider(
+                spider=spider, crawl_time=self.crawl_time
+            )
+
+            # 运行脚本统计信息
+            self.insert_script_statistics(log_info)
+            self.table_collection_statistics(
+                spider_name=spider.name,
+                database=spider.mysql_conf.database,
+                crawl_time=self.crawl_time,
+            )
+
+        if self.conn:
+            self.conn.close()
+
+    def table_collection_statistics(
+        self, spider_name: str, database: str, crawl_time: datetime.date
+    ):
+        """
+        统计数据库入库数据，获取当前数据库中所有包含 crawl_time 字段的数据表的简要信息
+        Args:
+            spider_name: 爬虫脚本名称
+            database: 数据库，保存程序采集记录保存的数据库
+            crawl_time: 采集时间，程序运行时间
+
+        Returns:
+            None
+        """
+        sql = f"""
+        select concat(
+            'select "',
+            TABLE_NAME,
+            '", count(id) as num , crawl_time from ',
+            TABLE_SCHEMA,
+            '.',
+            TABLE_NAME,
+                ' where crawl_time = "{crawl_time}"'
+        ) from information_schema.tables
+        where TABLE_SCHEMA='{database}' and TABLE_NAME in (SELECT TABLE_NAME FROM information_schema.columns WHERE COLUMN_NAME='crawl_time');
+        """
+        self.cursor.execute(sql)
+        results = self.cursor.fetchall()
+        if sql_list := [row[0] for row in results]:
+            sql_all = " union all ".join(sql_list)
+            self.cursor.execute(sql_all)
+            results = self.cursor.fetchall()
+
+            for row in results:
+                table_statistics = {
+                    "spider_name": spider_name,
+                    "database": database,
+                    "table_name": row[0],
+                    "number": row[1],
+                    "crawl_time": str((row[2] or crawl_time)),
+                }
+                self.insert_table_statistics(table_statistics)
+
+    def insert_table_statistics(
+        self, data: dict, table: str = "table_collection_statistics"
+    ):
+        """
+        插入统计数据到表中
+        Args:
+            data: 需要统计的入库信息
+            table: 存储表的名称
+
+        Returns:
+            None
+        """
+        self.cursor.execute(
+            f"""
+            CREATE TABLE IF NOT EXISTS `{table}` (
+            `id` int(11) NOT NULL AUTO_INCREMENT,
+            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',            
+            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+            `table_name` varchar(255) NOT NULL COMMENT '此项目所在库（一般某个项目放在单独的数据库中）的当前表名',
+            `number` varchar(255) NOT NULL COMMENT '当前表的当前 crawl_time 的采集个数',            
+            PRIMARY KEY (`id`) USING BTREE
+            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目对应库中各表采集统计表';
+            """
+        )
+
+        keys = f"""`{"`, `".join(data.keys())}`"""
+        values = ", ".join(["%s"] * len(data))
+        update = ",".join([f" `{key}` = %s" for key in data])
+        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
+        try:
+            if self.cursor.execute(sql, tuple(data.values()) * 2):
+                self.conn.commit()
+        except Exception as e:
+            self.conn.rollback()
+            self.slog.warning(f":{e}")
+
+    @retry(
+        stop_max_attempt_number=Param.retry_num,
+        wait_random_min=Param.retry_time_min,
+        wait_random_max=Param.retry_time_max,
+    )
+    def insert_script_statistics(
+        self, data: dict, table: str = "script_collection_statistics"
+    ):
+        """
+        存储运行脚本的统计信息
+        Args:
+            data: 需要插入的 log 信息
+            table: 存储表的名称
+
+        Returns:
+            None
+        """
+        self.cursor.execute(
+            f"""
+            CREATE TABLE IF NOT EXISTS `{table}` (
+            `id` int(11) NOT NULL AUTO_INCREMENT,
+            `database` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集程序和记录信息存储的数据库名',
+            `spider_name` varchar(255) NOT NULL DEFAULT '-' COMMENT '脚本名称',
+            `uid` varchar(255) NOT NULL DEFAULT '-' COMMENT 'uid',
+            `request_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '请求次数统计',
+            `received_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '接收次数统计',
+            `item_counts` varchar(255) NOT NULL DEFAULT '-' COMMENT '采集数据量',
+            `info_count` varchar(255) NOT NULL DEFAULT '-' COMMENT 'info 数据统计',
+            `warning_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '警告数据统计',
+            `error_count` varchar(255) NOT NULL DEFAULT '-' COMMENT '错误数据统计',
+            `start_time` datetime NOT NULL COMMENT '开始时间',
+            `finish_time` datetime NOT NULL COMMENT '结束时间',
+            `spend_minutes` varchar(255) NOT NULL DEFAULT '-' COMMENT '花费时间',
+            `crawl_time` datetime NOT NULL COMMENT '程序运行/数据采集时间',
+            `log_count_ERROR` varchar(255) DEFAULT NULL COMMENT '错误原因',
+            PRIMARY KEY (`id`) USING BTREE
+            ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 ROW_FORMAT=DYNAMIC COMMENT='项目运行脚本统计信息表';
+            """
+        )
+
+        keys = f"""`{"`, `".join(data.keys())}`"""
+        values = ", ".join(["%s"] * len(data))
+        update = ",".join([f" `{key}` = %s" for key in data])
+        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
+        try:
+            if self.cursor.execute(sql, tuple(data.values()) * 2):
+                self.conn.commit()
+        except Exception as e:
+            self.conn.rollback()
+            self.slog.warning(f":{e}")
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/asynced.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/asynced.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 
 class AsyncMysqlPipeline(AyuMysqlPipeline):
     def open_spider(self, spider):
         assert hasattr(spider, "mysql_conf"), "未配置 Mysql 连接信息！"
 
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
-        self.collate = ToolsForAyu.get_collate_by_charset(
-            mysql_conf=self.mysql_conf
-        )
+        self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=spider.mysql_conf)
         return ReuseOperation.as_deferred(self._open_spider(spider))
 
     async def _open_spider(self, spider):
-        # 将 mysql_conf 改为 aiomysql 所需要的配置
-        self.mysql_conf["db"] = self.mysql_conf.pop("database")
-        self.mysql_conf["cursorclass"] = aiomysql.DictCursor
-        self.pool = await aiomysql.create_pool(**self.mysql_conf)
+        # aiomysql 所需要的配置
+        self.pool = await aiomysql.create_pool(
+            user=spider.mysql_conf.user,
+            password=spider.mysql_conf.password,
+            host=spider.mysql_conf.host,
+            port=spider.mysql_conf.port,
+            db=spider.mysql_conf.database,
+            charset=spider.mysql_conf.charset,
+        )
         # 创建列表以存储任务
         self.tasks = []
 
     def process_item(self, item, spider):
         # 创建任务以运行协程
         task = asyncio.create_task(self.insert_item(item, spider))
         # 将任务添加到列表
@@ -41,15 +44,14 @@
             async with aiomysql_conn.cursor() as aiomysql_cursor:
                 item_dict = ToolsForAyu.convert_items_to_dict(item)
                 item_o = super(AsyncMysqlPipeline, self).get_new_item(item_dict)
                 table = super(AsyncMysqlPipeline, self).get_table_name(
                     item_dict["table"]
                 )
                 new_item = item_o.get("new_item")
-                # note_dic = item_o.get("notes_dic")
                 keys = f"""`{"`, `".join(new_item.keys())}`"""
                 values = ", ".join(["%s"] * len(new_item))
                 update = ",".join([f" `{key}` = %s" for key in new_item])
                 sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
 
                 await aiomysql_cursor.execute(sql, tuple(new_item.values()) * 2)
                 await aiomysql_conn.commit()
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/stats.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import dataclasses
 import datetime
 
-from ayugespidertools.common.Expend import MysqlErrorHandlingMixin
+from ayugespidertools.common.Expend import MysqlPipeEnhanceMixin
 from ayugespidertools.common.Utils import ToolsForAyu
 
-__all__ = ["AyuStatisticsMysqlPipeline"]
+__all__ = [
+    "AyuStatisticsMysqlPipeline",
+]
 
 
-class AyuStatisticsMysqlPipeline(MysqlErrorHandlingMixin):
+class AyuStatisticsMysqlPipeline(MysqlPipeEnhanceMixin):
     """
     Mysql 存储且记录脚本运行状态的简单示例
     """
 
     # TODO: 此方法暂用于测试
     def __init__(self, env):
         self.env = env
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/turbo.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/turbo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pymysql
 from dbutils.pooled_db import PooledDB
 
 from ayugespidertools.common.Utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
-__all__ = ["AyuTurboMysqlPipeline"]
+__all__ = [
+    "AyuTurboMysqlPipeline",
+]
 
 
 class AyuTurboMysqlPipeline(AyuMysqlPipeline):
     """
     Mysql 存储场景的 scrapy pipeline 扩展，使用 dbutils.pooled_db 实现
     """
 
@@ -46,13 +48,21 @@
                 # 连接数达到最大时，新连接是否可阻塞。默认False，即达到最大连接数时，再取新连接将会报错
                 "blocking": True,
             }
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
 
         # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。这个并不需要此连接对象，直接关闭即可
-        self._connect(pymysql_dict_conf=self.mysql_conf).close()
+        self._connect(spider.mysql_conf).close()
 
         # 添加 PooledDB 的配置
-        self.mysql_conf.update(self.pool_db_conf)
-        self.conn = PooledDB(creator=pymysql, **self.mysql_conf).connection()
+        self.conn = PooledDB(
+            creator=pymysql,
+            user=self.mysql_conf.user,
+            password=self.mysql_conf.password,
+            host=self.mysql_conf.host,
+            port=self.mysql_conf.port,
+            database=self.mysql_conf.database,
+            charset=self.mysql_conf.charset,
+            **self.pool_db_conf
+        ).connection()
         self.cursor = self.conn.cursor()
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/pipelines/mysql/twisted.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/pipelines/mysql/twisted.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pymysql import cursors
 from twisted.enterprise import adbapi
 
+from ayugespidertools.common.MysqlErrorHandle import TwistedAsynchronous, deal_mysql_err
 from ayugespidertools.common.Utils import ToolsForAyu
 from ayugespidertools.scraper.pipelines.mysql import AyuMysqlPipeline
 
-__all__ = ["AyuTwistedMysqlPipeline"]
+__all__ = [
+    "AyuTwistedMysqlPipeline",
+]
 
 
 class AyuTwistedMysqlPipeline(AyuMysqlPipeline):
     """
     使用 twisted 的 adbapi 实现 Mysql 存储场景下的异步操作
     注意：
         1. 推荐先用 AyuFtyMysqlPipeline 使用稳定后，再迁移至此管道
@@ -22,23 +25,29 @@
         self.slog = spider.slog
         self.mysql_conf = spider.mysql_conf
         self.collate = ToolsForAyu.get_collate_by_charset(mysql_conf=self.mysql_conf)
 
         # 判断目标数据库是否连接正常。若连接目标数据库错误时，创建缺失的目标数据库。
         # 记录日志时需要此连接对象，否则直接关闭
         if self.record_log_to_mysql:
-            self.conn = self._connect(pymysql_dict_conf=self.mysql_conf)
+            self.conn = self._connect(self.mysql_conf)
             self.cursor = self.conn.cursor()
         else:
-            self._connect(pymysql_dict_conf=self.mysql_conf).close()
+            self._connect(self.mysql_conf).close()
 
-        self.mysql_conf["cursorclass"] = cursors.DictCursor
-        self.dbpool = adbapi.ConnectionPool(
-            "pymysql", cp_reconnect=True, **self.mysql_conf
-        )
+        _mysql_conf = {
+            "user": spider.mysql_conf.user,
+            "password": spider.mysql_conf.password,
+            "host": spider.mysql_conf.host,
+            "port": spider.mysql_conf.port,
+            "db": spider.mysql_conf.database,
+            "charset": spider.mysql_conf.charset,
+            "cursorclass": cursors.DictCursor,
+        }
+        self.dbpool = adbapi.ConnectionPool("pymysql", cp_reconnect=True, **_mysql_conf)
         query = self.dbpool.runInteraction(self.db_create)
         query.addErrback(self.db_create_err)
 
     def db_create(self, cursor):
         pass
 
     def db_create_err(self, failure):
@@ -52,81 +61,41 @@
             query.addErrback(self.handle_error, item)
         return item
 
     def db_insert(self, cursor, item):
         item_o = super(AyuTwistedMysqlPipeline, self).get_new_item(item)
         table = super(AyuTwistedMysqlPipeline, self).get_table_name(item["table"])
 
-        # 以下逻辑直接 copy 父类的 insert_item 方法，只是剔除了 commit 方法和修改 cursor 而已
-        new_item = item_o.get("new_item")
+        if not (new_item := item_o.get("new_item")):
+            return
+
         note_dic = item_o.get("notes_dic")
-        keys = f"""`{"`, `".join(new_item.keys())}`"""
-        values = ", ".join(["%s"] * len(new_item))
-        update = ",".join([f" `{key}` = %s" for key in new_item])
-        sql = f"INSERT INTO `{table}` ({keys}) values ({values}) ON DUPLICATE KEY UPDATE {update}"
+        sql = self._get_sql_by_item(table=table, item=new_item)
 
         try:
             cursor.execute(sql, tuple(new_item.values()) * 2)
 
         except Exception as e:
             self.slog.warning(f":{e}")
             self.slog.warning(f"Item:{new_item}  Table: {table}")
-            err_msg = str(e)
-            if "1054" in err_msg:
-                self.deal_1054_error(
-                    err_msg=err_msg,
-                    conn=None,
-                    cursor=cursor,
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.db_insert(cursor, item)
-
-            elif "1146" in err_msg:
-                self.deal_1146_error(
-                    err_msg=err_msg,
-                    table_prefix=self.table_prefix,
-                    cursor=cursor,
-                    charset=self.mysql_conf["charset"],
-                    collate=self.collate,
-                    table_enum=self.table_enum,
-                )
-                return self.db_insert(cursor, item)
-
-            elif "1406" in err_msg:
-                self.deal_1406_error(
-                    err_msg=err_msg,
-                    conn=None,
-                    cursor=cursor,
-                    database=self.mysql_conf["database"],
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.db_insert(cursor, item)
-
-            elif "1265" in err_msg:
-                self.deal_1265_error(
-                    err_msg=err_msg,
-                    conn=None,
-                    cursor=cursor,
-                    database=self.mysql_conf["database"],
-                    table=table,
-                    note_dic=note_dic,
-                )
-                return self.db_insert(cursor, item)
-
-            else:
-                # 碰到其他的异常才打印错误日志，已处理的异常不打印
-                self.slog.error(f"ERROR:{e}")
+            deal_mysql_err(
+                TwistedAsynchronous(),
+                err_msg=str(e),
+                cursor=cursor,
+                charset=self.mysql_conf.charset,
+                collate=self.collate,
+                database=self.mysql_conf.database,
+                table=table,
+                table_prefix=self.table_prefix,
+                table_enum=self.table_enum,
+                note_dic=note_dic,
+            )
+            return self.db_insert(cursor, item)
 
         return item
 
     def handle_error(self, failure, item):
         self.slog.error(f"插入数据失败:{failure}, item: {item}")
 
     def close_spider(self, spider):
-        # 不删除 cursorclass 其实也不影响
-        if "cursorclass" in self.mysql_conf.keys():
-            del self.mysql_conf["cursorclass"]
-
         # 这里新建数据库链接，是为了正常继承父类的脚本运行统计的方法（需要 self 的 mysql 连接对象存在）
         super(AyuTwistedMysqlPipeline, self).close_spider(spider)
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__init__.py` & `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import threading
 import time
-from typing import Union
 
 from scrapy.spiders import Spider
 from sqlalchemy import create_engine
 
 from ayugespidertools.common.MultiPlexing import ReuseOperation
-from ayugespidertools.common.Utils import ToolsForAyu
+from ayugespidertools.common.SpiderDBConf import (
+    MongoDBConfCreator,
+    MysqlConfCreator,
+    get_spider_db_conf,
+)
 from ayugespidertools.config import logger
 
 __all__ = [
     "AyuSpider",
 ]
 
 
@@ -103,16 +106,19 @@
     def __init__(self, *args, **kwargs):
         super(AyuSpider, self).__init__(*args, **kwargs)
         self.mysql_engine = None
 
     @property
     def slog(self):
         """
-        本库的日志管理模块，使用 loguru 来管理日志；
-        本配置可与 Scrapy 的 spider.log 同时管理，根据场景可以自行配置。
+        本库的日志管理模块，使用 loguru 来管理日志
+        注：
+            1. 本库不是通过适配器模式或 mixin 等方法对 scrapy logger 重写或扩展，而是
+        新增一个 slog 的日志管理方法，目前感觉这样最适合；
+            2. 本配置可与 Scrapy 的 spider.log 同时管理，根据场景可以自行配置。
         """
         # 设置 loguru 日志配置
         loguru_conf_tmp = self.crawler.settings.get("LOGURU_CONFIG")
         # 是否开启 loguru 日志记录
         loguru_enabled = self.crawler.settings.get("LOGURU_ENABLED", True)
         assert isinstance(loguru_enabled, bool), "loguru_enabled 参数格式需要为 bool"
 
@@ -133,119 +139,46 @@
         # 根据 settings_type 参数取出对应的 inner_settings 配置
         inner_settings = getattr(cls, f"custom_{settings_type}_settings", {})
 
         if custom_table_enum:
             inner_settings["DATA_ENUM"] = custom_table_enum
 
         # 内置配置 inner_settings 优先级介于 project 和 spider 之间
-        # 即优先级顺序：settings.py < inner_settings < custom_settings
+        # 即优先级顺序：settings < inner_settings < custom_settings
         settings.setdict(inner_settings, priority="project")
         settings.setdict(cls.custom_settings or {}, priority="spider")
 
     @classmethod
-    def get_mysql_conf(
-        cls,
-        settings,
-    ) -> Union[dict, None]:
-        """
-        根据环境获取相应的 Mysql 数据库配置，获取其他自定义配置
-        Args:
-            settings: crawler settings 配置信息
-
-        Returns:
-            1). Mysql 数据库链接配置
-        """
-        # 自定义 mysql 链接配置
-        local_mysql_conf = settings.get("LOCAL_MYSQL_CONFIG", {})
-        # 是否开启应用配置管理
-        app_conf_manage = settings.get("APP_CONF_MANAGE", False)
-        if all([not local_mysql_conf.get("DATABASE"), not app_conf_manage]):
-            return None
-
-        # 1). 如果开启应用管理，从 consul 中获取应用配置
-        if app_conf_manage:
-            consul_conf = ReuseOperation.get_consul_conf(settings=settings)
-            return ToolsForAyu.get_conf_by_consul(conf_name="MYSQL", **consul_conf)
-
-        # 2). 从本地 local_mysql_config 的参数中取值
-        if ReuseOperation.is_dict_meet_min_limit(
-            dict_conf=local_mysql_conf,
-            key_list=["HOST", "PORT", "USER", "PASSWORD", "CHARSET", "DATABASE"],
-        ):
-            return {
-                "host": local_mysql_conf.get("HOST"),
-                "port": local_mysql_conf.get("PORT"),
-                "user": local_mysql_conf.get("USER"),
-                "password": local_mysql_conf.get("PASSWORD"),
-                "database": local_mysql_conf.get("DATABASE"),
-                "charset": local_mysql_conf.get("CHARSET") or "utf8mb4",
-            }
-
-    @classmethod
-    def get_mongodb_conf(
-        cls,
-        settings,
-    ) -> Union[dict, None]:
-        """
-        根据环境获取相应的 mongoDB 数据库配置，获取其他自定义配置
-        Args:
-            settings: crawler settings 配置信息
-
-        Returns:
-            1). MongoDB 数据库链接配置
-        """
-        # 自定义 mysql 链接配置
-        local_mongodb_conf = settings.get("LOCAL_MONGODB_CONFIG", {})
-        # 是否开启应用配置管理
-        app_conf_manage = settings.get("APP_CONF_MANAGE", False)
-        if all([not local_mongodb_conf.get("DATABASE"), not app_conf_manage]):
-            return None
-
-        # 1). 如果开启应用管理，从 consul 中获取应用配置
-        if app_conf_manage:
-            consul_conf = ReuseOperation.get_consul_conf(settings=settings)
-            return ToolsForAyu.get_conf_by_consul(conf_name="MONGODB", **consul_conf)
-
-        # 2). 从本地 local_mongo_conf 的参数中取值
-        if ReuseOperation.is_dict_meet_min_limit(
-            dict_conf=local_mongodb_conf,
-            key_list=["HOST", "PORT", "USER", "PASSWORD", "DATABASE"],
-        ):
-            return {
-                "host": local_mongodb_conf.get("HOST"),
-                "port": local_mongodb_conf.get("PORT"),
-                "user": local_mongodb_conf.get("USER"),
-                "password": local_mongodb_conf.get("PASSWORD"),
-                "authsource": local_mongodb_conf.get("AUTHSOURCE"),
-                "database": local_mongodb_conf.get("DATABASE"),
-            }
-
-    @classmethod
     def from_crawler(cls, crawler, *args, **kwargs):
         spider = super(AyuSpider, cls).from_crawler(crawler, *args, **kwargs)
         spider.stats = crawler.stats
 
         # 先输出下相关日志，用于调试时查看
         spider.slog.debug(f"settings_type 配置: {cls.settings_type}")
-        spider.slog.debug(f"scrapy 当前配置为: {dict(crawler.settings)}")
 
+        _consul_conf = ReuseOperation.get_consul_conf(settings=crawler.settings)
         # 1).先配置 Mysql 的相关信息，如果存在 Mysql 配置，则把 mysql_conf 添加到 spider 上
-        if mysql_conf := cls.get_mysql_conf(settings=crawler.settings):
+        if mysql_conf := get_spider_db_conf(
+            MysqlConfCreator().create_product(
+                settings=crawler.settings, consul_conf=_consul_conf
+            )
+        ):
             spider.slog.info("项目中配置了 mysql_conf 信息")
             spider.mysql_conf = mysql_conf
-
-            # 如果打开了 mysql_engine_enabled 参数(用于 spiders 中数据入库前去重查询)
             if cls.mysql_engine_enabled:
                 mysql_url = (
-                    f'mysql+pymysql://{mysql_conf.get("user")}'
-                    f':{mysql_conf.get("password")}@{mysql_conf.get("host")}'
-                    f':{mysql_conf.get("port")}/{mysql_conf.get("database")}'
-                    f'?charset={mysql_conf.get("charset")}'
+                    f"mysql+pymysql://{mysql_conf.user}"
+                    f":{mysql_conf.password}@{mysql_conf.host}"
+                    f":{mysql_conf.port}/{mysql_conf.database}"
+                    f"?charset={mysql_conf.charset}"
                 )
                 spider.mysql_engine = MySqlEngineClass(engine_url=mysql_url).engine
 
         # 2).配置 MongoDB 的相关信息，如果存在 MongoDB 配置，则把 mongodb_conf 添加到 spider 上
-        if mongodb_conf := cls.get_mongodb_conf(settings=crawler.settings):
+        if mongodb_conf := get_spider_db_conf(
+            MongoDBConfCreator().create_product(
+                settings=crawler.settings, consul_conf=_consul_conf
+            )
+        ):
             spider.slog.info("项目中配置了 mongodb_conf 信息")
             spider.mongodb_conf = mongodb_conf
-
         return spider
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  4 03:26:52 2023 UTC, .py size: 9594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,372 +1,383 @@
-00000000: 550d 0d0a 0000 0000 fc98 2b64 7a25 0000  U.........+dz%..
+00000000: 550d 0d0a 0000 0000 eb57 2c64 1a26 0000  U........W,d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
-00000080: 6d0d 5a0d 0100 6408 6701 5a0e 4700 6409  m.Z...d.g.Z.G.d.
-00000090: 640a 8400 640a 8302 5a0f 4700 640b 6408  d...d...Z.G.d.d.
-000000a0: 8400 6408 6505 8303 5a10 6401 5300 290c  ..d.e...Z.d.S.).
-000000b0: e900 0000 004e 2901 da05 556e 696f 6e29  .....N)...Union)
-000000c0: 01da 0653 7069 6465 7229 01da 0d63 7265  ...Spider)...cre
-000000d0: 6174 655f 656e 6769 6e65 2901 da0e 5265  ate_engine)...Re
-000000e0: 7573 654f 7065 7261 7469 6f6e 2901 da0b  useOperation)...
-000000f0: 546f 6f6c 7346 6f72 4179 7529 01da 066c  ToolsForAyu)...l
-00000100: 6f67 6765 72da 0941 7975 5370 6964 6572  ogger..AyuSpider
-00000110: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000120: 0002 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
-00000130: 5a01 6400 5a02 6401 5a03 6504 a005 a100  Z.d.Z.d.Z.e.....
-00000140: 5a06 6402 6403 8400 5a07 6404 6405 8400  Z.d.d...Z.d.d...
-00000150: 5a08 6406 5300 2907 da10 4d79 5371 6c45  Z.d.S.)...MySqlE
-00000160: 6e67 696e 6543 6c61 7373 7528 0000 000a  ngineClassu(....
-00000170: 2020 2020 6d79 7371 6c20 e993 bee6 8ea5      mysql ......
-00000180: e58f a5e6 9f84 e58d 95e4 be8b e6a8 a1e5  ................
-00000190: bc8f 0a20 2020 2063 0200 0000 0000 0000  ...    c........
-000001a0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-000001b0: 7314 0000 0074 007c 0164 0164 0264 038d  s....t.|.d.d.d..
-000001c0: 037c 005f 0164 0053 0029 044e 5469 7062  .|._.d.S.).NTipb
-000001d0: 0000 2902 5a0d 706f 6f6c 5f70 7265 5f70  ..).Z.pool_pre_p
-000001e0: 696e 675a 0c70 6f6f 6c5f 7265 6379 636c  ingZ.pool_recycl
-000001f0: 6529 0272 0400 0000 da06 656e 6769 6e65  e).r......engine
-00000200: 2902 da04 7365 6c66 da0a 656e 6769 6e65  )...self..engine
-00000210: 5f75 726c a900 720d 0000 00fa 4a2f 726f  _url..r.....J/ro
-00000220: 6f74 2f6d 7970 726f 6a2f 4179 7567 6553  ot/myproj/AyugeS
-00000230: 7069 6465 7254 6f6f 6c73 2f61 7975 6765  piderTools/ayuge
-00000240: 7370 6964 6572 746f 6f6c 732f 7363 7261  spidertools/scra
-00000250: 7065 722f 7370 6964 6572 732f 5f5f 696e  per/spiders/__in
-00000260: 6974 5f5f 2e70 79da 085f 5f69 6e69 745f  it__.py..__init_
-00000270: 5f18 0000 0073 0a00 0000 0001 0201 0200  _....s..........
-00000280: 0200 02ff 7a19 4d79 5371 6c45 6e67 696e  ....z.MySqlEngin
-00000290: 6543 6c61 7373 2e5f 5f69 6e69 745f 5f63  eClass.__init__c
-000002a0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000002b0: 0900 0000 4f00 0000 7338 0000 0074 0074  ....O...s8...t.t
-000002c0: 0164 0183 0273 327c 006a 028f 1c01 0074  .d...s2|.j.....t
-000002d0: 0074 0164 0183 0273 2874 03a0 047c 00a1  .t.d...s(t...|..
-000002e0: 0174 015f 0557 0035 0051 0052 0058 0074  .t._.W.5.Q.R.X.t
-000002f0: 016a 0553 0029 024e da09 5f69 6e73 7461  .j.S.).N.._insta
-00000300: 6e63 6529 06da 0768 6173 6174 7472 7209  nce)...hasattrr.
-00000310: 0000 00da 0e5f 696e 7374 616e 6365 5f6c  ....._instance_l
-00000320: 6f63 6bda 066f 626a 6563 74da 075f 5f6e  ock..object..__n
-00000330: 6577 5f5f 7210 0000 0029 03da 0363 6c73  ew__r....)...cls
-00000340: da04 6172 6773 da06 6b77 6172 6773 720d  ..args..kwargsr.
-00000350: 0000 0072 0d00 0000 720e 0000 0072 1400  ...r....r....r..
-00000360: 0000 1d00 0000 730a 0000 0000 010a 0108  ......s.........
-00000370: 010a 0116 027a 184d 7953 716c 456e 6769  .....z.MySqlEngi
-00000380: 6e65 436c 6173 732e 5f5f 6e65 775f 5f4e  neClass.__new__N
-00000390: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000003a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000003b0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-000003c0: 0974 6872 6561 6469 6e67 da04 4c6f 636b  .threading..Lock
-000003d0: 7212 0000 0072 0f00 0000 7214 0000 0072  r....r....r....r
-000003e0: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-000003f0: 0000 0072 0900 0000 1100 0000 7308 0000  ...r........s...
-00000400: 0008 0104 0408 0208 0572 0900 0000 6300  .........r....c.
-00000410: 0000 0000 0000 0000 0000 0000 0000 000a  ................
-00000420: 0000 0000 0000 0073 ec00 0000 6500 5a01  .......s....e.Z.
-00000430: 6400 5a02 6401 5a03 6402 6402 6403 6404  d.Z.d.Z.d.d.d.d.
-00000440: 6405 6406 9c05 5a04 6407 6402 6408 6403  d.d...Z.d.d.d.d.
-00000450: 6402 6404 6409 640a 6402 640b 9c09 5a05  d.d.d.d.d.d...Z.
-00000460: 640c 6402 6408 6403 6402 6404 640d 640a  d.d.d.d.d.d.d.d.
-00000470: 6402 640b 9c09 5a06 6507 a008 640e 6507  d.d...Z.e...d.e.
-00000480: a009 a100 a102 5a0a 640f 5a0b 6410 5a0c  ......Z.d.Z.d.Z.
-00000490: 640a 5a0d 6402 5a0e 8700 6601 6411 6412  d.Z.d.Z...f.d.d.
-000004a0: 8408 5a0f 8700 6601 6413 6414 8408 5a10  ..Z...f.d.d...Z.
-000004b0: 6511 8700 6601 6415 6416 8408 8301 5a12  e...f.d.d.....Z.
-000004c0: 6513 6417 6418 8400 8301 5a14 6513 6515  e.d.d.....Z.e.e.
-000004d0: 6516 640a 6602 1900 6419 9c01 641a 641b  e.d.f...d...d.d.
-000004e0: 8404 8301 5a17 6513 6515 6516 640a 6602  ....Z.e.e.e.d.f.
-000004f0: 1900 6419 9c01 641c 641d 8404 8301 5a18  ..d...d.d.....Z.
-00000500: 6513 8700 6601 641e 641f 8408 8301 5a19  e...f.d.d.....Z.
-00000510: 8700 0400 5a1a 5300 2920 7208 0000 0075  ....Z.S.) r....u
-00000520: 5600 0000 0a20 2020 20e7 94a8 e4ba 8ee5  V....    .......
-00000530: 889d e5a7 8be9 858d e7bd ae20 7363 7261  ........... scra
-00000540: 7079 20e7 9a84 e590 84e7 a78d 2073 6574  py ......... set
-00000550: 7469 6e67 20e7 9a84 e580 bce5 8f8a 2073  ting ......... s
-00000560: 7069 6465 7220 e585 a8e5 b180 e58f 98e9  pider ..........
-00000570: 878f e7ad 890a 2020 2020 46e9 0300 0000  ......    F.....
-00000580: e9ff ffff ffda 0364 6576 2905 da0e 524f  .......dev)...RO
-00000590: 424f 5453 5458 545f 4f42 4559 5a15 5445  BOTSTXT_OBEYZ.TE
-000005a0: 4c4e 4554 434f 4e53 4f4c 455f 454e 4142  LNETCONSOLE_ENAB
-000005b0: 4c45 44da 0b52 4554 5259 5f54 494d 4553  LED..RETRY_TIMES
-000005c0: da0e 4445 5054 485f 5052 494f 5249 5459  ..DEPTH_PRIORITY
-000005d0: da03 454e 56da 0544 4542 5547 e914 0000  ..ENV..DEBUG....
-000005e0: 00da 0474 6573 744e 2909 5a09 4c4f 475f  ...testN).Z.LOG_
-000005f0: 4c45 5645 4c72 2100 0000 5a10 444f 574e  LEVELr!...Z.DOWN
-00000600: 4c4f 4144 5f54 494d 454f 5554 7222 0000  LOAD_TIMEOUTr"..
-00000610: 005a 1052 4544 4952 4543 545f 454e 4142  .Z.REDIRECT_ENAB
-00000620: 4c45 4472 2300 0000 7224 0000 00da 0944  LEDr#...r$.....D
-00000630: 4154 415f 454e 554d 5a13 5245 434f 5244  ATA_ENUMZ.RECORD
-00000640: 5f4c 4f47 5f54 4f5f 4d59 5351 4cda 0545  _LOG_TO_MYSQL..E
-00000650: 5252 4f52 da04 7072 6f64 7a08 2559 2d25  RROR..prodz.%Y-%
-00000660: 6d2d 2564 da06 636f 6d6d 6f6e da00 6302  m-%d..common..c.
-00000670: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000680: 0000 000b 0000 0073 1800 0000 7400 7401  .......s....t.t.
-00000690: 7c00 8302 6a02 7c01 6601 7c02 8e01 0100  |...j.|.f.|.....
-000006a0: 6401 5300 2902 753d 0000 000a 2020 2020  d.S.).u=....    
-000006b0: 2020 2020 e5ae 9ee7 8eb0 e689 80e7 bba7      ............
-000006c0: e689 bfe7 b1bb e79a 8420 6162 7374 7261  ......... abstra
-000006d0: 6374 20e6 96b9 e6b3 9520 7061 7273 650a  ct ...... parse.
-000006e0: 2020 2020 2020 2020 4e29 03da 0573 7570          N)...sup
-000006f0: 6572 7208 0000 00da 0570 6172 7365 2903  err......parse).
-00000700: 720b 0000 00da 0872 6573 706f 6e73 6572  r......responser
-00000710: 1700 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
-00000720: 5f72 0d00 0000 720e 0000 0072 2e00 0000  _r....r....r....
-00000730: 6100 0000 7302 0000 0000 047a 0f41 7975  a...s......z.Ayu
-00000740: 5370 6964 6572 2e70 6172 7365 6301 0000  Spider.parsec...
-00000750: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000760: 000f 0000 0073 1c00 0000 7400 7401 7c00  .....s....t.t.|.
-00000770: 8302 6a02 7c01 7c02 8e01 0100 6400 7c00  ..j.|.|.....d.|.
-00000780: 5f03 6400 5300 2901 4e29 0472 2d00 0000  _.d.S.).N).r-...
-00000790: 7208 0000 0072 0f00 0000 da0c 6d79 7371  r....r......mysq
-000007a0: 6c5f 656e 6769 6e65 2903 720b 0000 0072  l_engine).r....r
-000007b0: 1600 0000 7217 0000 0072 3000 0000 720d  ....r....r0...r.
-000007c0: 0000 0072 0e00 0000 720f 0000 0067 0000  ...r....r....g..
-000007d0: 0073 0400 0000 0001 1201 7a12 4179 7553  .s........z.AyuS
-000007e0: 7069 6465 722e 5f5f 696e 6974 5f5f 6301  pider.__init__c.
-000007f0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000800: 0000 0003 0000 0073 4c00 0000 7c00 6a00  .......sL...|.j.
-00000810: 6a01 a002 6401 a101 7d01 7c00 6a00 6a01  j...d...}.|.j.j.
-00000820: a002 6402 6403 a102 7d02 7403 7c02 7404  ..d.d...}.t.|.t.
-00000830: 8302 7330 7405 6404 8301 8201 7c02 723c  ..s0t.d.....|.r<
-00000840: 7c01 703a 7406 5300 7407 7408 7c00 8302  |.p:t.S.t.t.|...
-00000850: 6a06 5300 6405 5300 2906 75af 0000 000a  j.S.d.S.).u.....
-00000860: 2020 2020 2020 2020 e69c ace5 ba93 e79a          ........
-00000870: 84e6 97a5 e5bf 97e7 aea1 e790 86e6 a8a1  ................
-00000880: e59d 97ef bc8c e4bd bfe7 94a8 206c 6f67  ............ log
-00000890: 7572 7520 e69d a5e7 aea1 e790 86e6 97a5  uru ............
-000008a0: e5bf 97ef bc9b 0a20 2020 2020 2020 20e6  .......        .
-000008b0: 9cac e985 8de7 bdae e58f afe4 b88e 2053  .............. S
-000008c0: 6372 6170 7920 e79a 8420 7370 6964 6572  crapy ... spider
-000008d0: 2e6c 6f67 20e5 908c e697 b6e7 aea1 e790  .log ...........
-000008e0: 86ef bc8c e6a0 b9e6 8dae e59c bae6 99af  ................
-000008f0: e58f afe4 bba5 e887 aae8 a18c e985 8de7  ................
-00000900: bdae e380 820a 2020 2020 2020 2020 5a0d  ......        Z.
-00000910: 4c4f 4755 5255 5f43 4f4e 4649 475a 0e4c  LOGURU_CONFIGZ.L
-00000920: 4f47 5552 555f 454e 4142 4c45 4454 7529  OGURU_ENABLEDTu)
-00000930: 0000 006c 6f67 7572 755f 656e 6162 6c65  ...loguru_enable
-00000940: 6420 e58f 82e6 95b0 e6a0 bce5 bc8f e99c  d ..............
-00000950: 80e8 a681 e4b8 ba20 626f 6f6c 4e29 09da  ....... boolN)..
-00000960: 0763 7261 776c 6572 da08 7365 7474 696e  .crawler..settin
-00000970: 6773 da03 6765 74da 0a69 7369 6e73 7461  gs..get..isinsta
-00000980: 6e63 65da 0462 6f6f 6cda 0e41 7373 6572  nce..bool..Asser
-00000990: 7469 6f6e 4572 726f 7272 0700 0000 722d  tionErrorr....r-
-000009a0: 0000 0072 0800 0000 2903 720b 0000 005a  ...r....).r....Z
-000009b0: 0f6c 6f67 7572 755f 636f 6e66 5f74 6d70  .loguru_conf_tmp
-000009c0: 5a0e 6c6f 6775 7275 5f65 6e61 626c 6564  Z.loguru_enabled
-000009d0: 7230 0000 0072 0d00 0000 720e 0000 00da  r0...r....r.....
-000009e0: 0473 6c6f 676b 0000 0073 0c00 0000 0007  .slogk...s......
-000009f0: 0e02 1001 1203 0402 0804 7a0e 4179 7553  ..........z.AyuS
-00000a00: 7069 6465 722e 736c 6f67 6302 0000 0000  pider.slogc.....
-00000a10: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-00000a20: 0000 0073 5e00 0000 7400 7c00 6401 6400  ...s^...t.|.d.d.
-00000a30: 8303 7d02 7400 7c00 6402 6403 8303 7d03  ..}.t.|.d.d...}.
-00000a40: 7400 7c00 6404 7c03 9b00 6405 9d03 6900  t.|.d.|...d...i.
-00000a50: 8303 7d04 7c02 7238 7c02 7c04 6406 3c00  ..}.|.r8|.|.d.<.
-00000a60: 7c01 6a01 7c04 6407 6408 8d02 0100 7c01  |.j.|.d.d.....|.
-00000a70: 6a01 7c00 6a02 7052 6900 6409 6408 8d02  j.|.j.pRi.d.d...
-00000a80: 0100 6400 5300 290a 4eda 1163 7573 746f  ..d.S.).N..custo
-00000a90: 6d5f 7461 626c 655f 656e 756d da0d 7365  m_table_enum..se
-00000aa0: 7474 696e 6773 5f74 7970 6572 2b00 0000  ttings_typer+...
-00000ab0: 5a07 6375 7374 6f6d 5fda 095f 7365 7474  Z.custom_.._sett
-00000ac0: 696e 6773 7228 0000 005a 0770 726f 6a65  ingsr(...Z.proje
-00000ad0: 6374 2901 da08 7072 696f 7269 7479 da06  ct)...priority..
-00000ae0: 7370 6964 6572 2903 da07 6765 7461 7474  spider)...getatt
-00000af0: 72da 0773 6574 6469 6374 da0f 6375 7374  r..setdict..cust
-00000b00: 6f6d 5f73 6574 7469 6e67 7329 0572 1500  om_settings).r..
-00000b10: 0000 7234 0000 0072 3a00 0000 723b 0000  ..r4...r:...r;..
-00000b20: 005a 0e69 6e6e 6572 5f73 6574 7469 6e67  .Z.inner_setting
-00000b30: 7372 0d00 0000 720d 0000 0072 0e00 0000  sr....r....r....
-00000b40: da0f 7570 6461 7465 5f73 6574 7469 6e67  ..update_setting
-00000b50: 7380 0000 0073 0e00 0000 0002 0c02 0c02  s....s..........
-00000b60: 1402 0401 0804 0e01 7a19 4179 7553 7069  ........z.AyuSpi
-00000b70: 6465 722e 7570 6461 7465 5f73 6574 7469  der.update_setti
-00000b80: 6e67 7329 01da 0672 6574 7572 6e63 0200  ngs)...returnc..
-00000b90: 0000 0000 0000 0000 0000 0500 0000 0800  ................
-00000ba0: 0000 4300 0000 73ae 0000 007c 01a0 0064  ..C...s....|...d
-00000bb0: 0169 00a1 027d 027c 01a0 0064 0264 03a1  .i...}.|...d.d..
-00000bc0: 027d 0374 017c 02a0 0064 04a1 010c 007c  .}.t.|...d.....|
-00000bd0: 030c 0067 0283 0172 3264 0553 007c 0372  ...g...r2d.S.|.r
-00000be0: 5674 026a 037c 0164 068d 017d 0474 046a  Vt.j.|.d...}.t.j
-00000bf0: 0566 0064 0764 0869 017c 0497 028e 0153  .f.d.d.i.|.....S
-00000c00: 0074 026a 067c 0264 0964 0a64 0b64 0c64  .t.j.|.d.d.d.d.d
-00000c10: 0d64 0467 0664 0e8d 0272 aa7c 02a0 0064  .d.g.d...r.|...d
-00000c20: 09a1 017c 02a0 0064 0aa1 017c 02a0 0064  ...|...d...|...d
-00000c30: 0ba1 017c 02a0 0064 0ca1 017c 02a0 0064  ...|...d...|...d
-00000c40: 04a1 017c 02a0 0064 0da1 0170 a464 0f64  ...|...d...p.d.d
-00000c50: 109c 0653 0064 0553 0029 1175 e100 0000  ...S.d.S.).u....
-00000c60: 0a20 2020 2020 2020 20e6 a0b9 e68d aee7  .        .......
-00000c70: 8eaf e5a2 83e8 8eb7 e58f 96e7 9bb8 e5ba  ................
-00000c80: 94e7 9a84 204d 7973 716c 20e6 95b0 e68d  .... Mysql .....
-00000c90: aee5 ba93 e985 8de7 bdae efbc 8ce8 8eb7  ................
-00000ca0: e58f 96e5 85b6 e4bb 96e8 87aa e5ae 9ae4  ................
-00000cb0: b989 e985 8de7 bdae 0a20 2020 2020 2020  .........       
-00000cc0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00000cd0: 2020 2073 6574 7469 6e67 733a 2063 7261     settings: cra
-00000ce0: 776c 6572 2073 6574 7469 6e67 7320 e985  wler settings ..
-00000cf0: 8de7 bdae e4bf a1e6 81af 0a0a 2020 2020  ............    
-00000d00: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00000d10: 2020 2020 2020 2020 2031 292e 204d 7973           1). Mys
-00000d20: 716c 20e6 95b0 e68d aee5 ba93 e993 bee6  ql .............
-00000d30: 8ea5 e985 8de7 bdae 0a20 2020 2020 2020  .........       
-00000d40: 205a 124c 4f43 414c 5f4d 5953 514c 5f43   Z.LOCAL_MYSQL_C
-00000d50: 4f4e 4649 47da 0f41 5050 5f43 4f4e 465f  ONFIG..APP_CONF_
-00000d60: 4d41 4e41 4745 46da 0844 4154 4142 4153  MANAGEF..DATABAS
-00000d70: 454e a901 7234 0000 00da 0963 6f6e 665f  EN..r4.....conf_
-00000d80: 6e61 6d65 5a05 4d59 5351 4cda 0448 4f53  nameZ.MYSQL..HOS
-00000d90: 54da 0450 4f52 54da 0455 5345 52da 0850  T..PORT..USER..P
-00000da0: 4153 5357 4f52 44da 0743 4841 5253 4554  ASSWORD..CHARSET
-00000db0: a902 5a09 6469 6374 5f63 6f6e 665a 086b  ..Z.dict_confZ.k
-00000dc0: 6579 5f6c 6973 74da 0775 7466 386d 6234  ey_list..utf8mb4
-00000dd0: 2906 da04 686f 7374 da04 706f 7274 da04  )...host..port..
-00000de0: 7573 6572 da08 7061 7373 776f 7264 da08  user..password..
-00000df0: 6461 7461 6261 7365 da07 6368 6172 7365  database..charse
-00000e00: 74a9 0772 3500 0000 da03 616c 6c72 0500  t..r5.....allr..
-00000e10: 0000 5a0f 6765 745f 636f 6e73 756c 5f63  ..Z.get_consul_c
-00000e20: 6f6e 6672 0600 0000 5a12 6765 745f 636f  onfr....Z.get_co
-00000e30: 6e66 5f62 795f 636f 6e73 756c 5a16 6973  nf_by_consulZ.is
-00000e40: 5f64 6963 745f 6d65 6574 5f6d 696e 5f6c  _dict_meet_min_l
-00000e50: 696d 6974 2905 7215 0000 0072 3400 0000  imit).r....r4...
-00000e60: 5a10 6c6f 6361 6c5f 6d79 7371 6c5f 636f  Z.local_mysql_co
-00000e70: 6e66 da0f 6170 705f 636f 6e66 5f6d 616e  nf..app_conf_man
-00000e80: 6167 65da 0b63 6f6e 7375 6c5f 636f 6e66  age..consul_conf
-00000e90: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-00000ea0: 0e67 6574 5f6d 7973 716c 5f63 6f6e 6690  .get_mysql_conf.
-00000eb0: 0000 0073 2400 0000 000e 0c02 0c01 1601  ...s$...........
-00000ec0: 0403 0401 0c01 1403 0401 0201 0efe 0605  ................
-00000ed0: 0801 0801 0801 0801 0801 0cfa 7a18 4179  ............z.Ay
-00000ee0: 7553 7069 6465 722e 6765 745f 6d79 7371  uSpider.get_mysq
-00000ef0: 6c5f 636f 6e66 6302 0000 0000 0000 0000  l_confc.........
-00000f00: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00000f10: a800 0000 7c01 a000 6401 6900 a102 7d02  ....|...d.i...}.
-00000f20: 7c01 a000 6402 6403 a102 7d03 7401 7c02  |...d.d...}.t.|.
-00000f30: a000 6404 a101 0c00 7c03 0c00 6702 8301  ..d.....|...g...
-00000f40: 7232 6405 5300 7c03 7256 7402 6a03 7c01  r2d.S.|.rVt.j.|.
-00000f50: 6406 8d01 7d04 7404 6a05 6600 6407 6408  d...}.t.j.f.d.d.
-00000f60: 6901 7c04 9702 8e01 5300 7402 6a06 7c02  i.|.....S.t.j.|.
-00000f70: 6409 640a 640b 640c 6404 6705 640d 8d02  d.d.d.d.d.g.d...
-00000f80: 72a4 7c02 a000 6409 a101 7c02 a000 640a  r.|...d...|...d.
-00000f90: a101 7c02 a000 640b a101 7c02 a000 640c  ..|...d...|...d.
-00000fa0: a101 7c02 a000 640e a101 7c02 a000 6404  ..|...d...|...d.
-00000fb0: a101 640f 9c06 5300 6405 5300 2910 75e5  ..d...S.d.S.).u.
-00000fc0: 0000 000a 2020 2020 2020 2020 e6a0 b9e6  ....        ....
-00000fd0: 8dae e78e afe5 a283 e88e b7e5 8f96 e79b  ................
-00000fe0: b8e5 ba94 e79a 8420 6d6f 6e67 6f44 4220  ....... mongoDB 
-00000ff0: e695 b0e6 8dae e5ba 93e9 858d e7bd aeef  ................
-00001000: bc8c e88e b7e5 8f96 e585 b6e4 bb96 e887  ................
-00001010: aae5 ae9a e4b9 89e9 858d e7bd ae0a 2020  ..............  
-00001020: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00001030: 2020 2020 2020 2020 7365 7474 696e 6773          settings
-00001040: 3a20 6372 6177 6c65 7220 7365 7474 696e  : crawler settin
-00001050: 6773 20e9 858d e7bd aee4 bfa1 e681 af0a  gs .............
-00001060: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00001070: 3a0a 2020 2020 2020 2020 2020 2020 3129  :.            1)
-00001080: 2e20 4d6f 6e67 6f44 4220 e695 b0e6 8dae  . MongoDB ......
-00001090: e5ba 93e9 93be e68e a5e9 858d e7bd ae0a  ................
-000010a0: 2020 2020 2020 2020 5a14 4c4f 4341 4c5f          Z.LOCAL_
-000010b0: 4d4f 4e47 4f44 425f 434f 4e46 4947 7244  MONGODB_CONFIGrD
-000010c0: 0000 0046 7245 0000 004e 7246 0000 0072  ...FrE...NrF...r
-000010d0: 4700 0000 5a07 4d4f 4e47 4f44 4272 4800  G...Z.MONGODBrH.
-000010e0: 0000 7249 0000 0072 4a00 0000 724b 0000  ..rI...rJ...rK..
-000010f0: 0072 4d00 0000 5a0a 4155 5448 534f 5552  .rM...Z.AUTHSOUR
-00001100: 4345 2906 724f 0000 0072 5000 0000 7251  CE).rO...rP...rQ
-00001110: 0000 0072 5200 0000 da0a 6175 7468 736f  ...rR.....authso
-00001120: 7572 6365 7253 0000 0072 5500 0000 2905  urcerS...rU...).
-00001130: 7215 0000 0072 3400 0000 5a12 6c6f 6361  r....r4...Z.loca
-00001140: 6c5f 6d6f 6e67 6f64 625f 636f 6e66 7257  l_mongodb_confrW
-00001150: 0000 0072 5800 0000 720d 0000 0072 0d00  ...rX...r....r..
-00001160: 0000 720e 0000 00da 1067 6574 5f6d 6f6e  ..r......get_mon
-00001170: 676f 6462 5f63 6f6e 66b7 0000 0073 2400  godb_conf....s$.
-00001180: 0000 000e 0c02 0c01 1601 0403 0401 0c01  ................
-00001190: 1403 0401 0201 0cfe 0605 0801 0801 0801  ................
-000011a0: 0801 0801 08fa 7a1a 4179 7553 7069 6465  ......z.AyuSpide
-000011b0: 722e 6765 745f 6d6f 6e67 6f64 625f 636f  r.get_mongodb_co
-000011c0: 6e66 6302 0000 0000 0000 0000 0000 0008  nfc.............
-000011d0: 0000 000e 0000 000f 0000 0073 f800 0000  ...........s....
-000011e0: 7400 7401 7c00 8302 6a02 7c01 6601 7c02  t.t.|...j.|.f.|.
-000011f0: 9e02 7c03 8e01 7d04 7c01 6a03 7c04 5f03  ..|...}.|.j.|._.
-00001200: 7c04 6a04 a005 6401 7c00 6a06 9b00 9d02  |.j...d.|.j.....
-00001210: a101 0100 7c04 6a04 a005 6402 7407 7c01  ....|.j...d.t.|.
-00001220: 6a08 8301 9b00 9d02 a101 0100 7c00 6a09  j...........|.j.
-00001230: 7c01 6a08 6403 8d01 0400 7d05 72d0 7c04  |.j.d.....}.r.|.
-00001240: 6a04 a00a 6404 a101 0100 7c05 7c04 5f0b  j...d.....|.|._.
-00001250: 7c00 6a0c 72d0 6405 7c05 a00d 6406 a101  |.j.r.d.|...d...
-00001260: 9b00 6407 7c05 a00d 6408 a101 9b00 6409  ..d.|...d.....d.
-00001270: 7c05 a00d 640a a101 9b00 6407 7c05 a00d  |...d.....d.|...
-00001280: 640b a101 9b00 640c 7c05 a00d 640d a101  d.....d.|...d...
-00001290: 9b00 640e 7c05 a00d 640f a101 9b00 9d0c  ..d.|...d.......
-000012a0: 7d06 740e 7c06 6410 8d01 6a0f 7c04 5f10  }.t.|.d...j.|._.
-000012b0: 7c00 6a11 7c01 6a08 6403 8d01 0400 7d07  |.j.|.j.d.....}.
-000012c0: 72f4 7c04 6a04 a00a 6411 a101 0100 7c07  r.|.j...d.....|.
-000012d0: 7c04 5f12 7c04 5300 2912 4e75 1600 0000  |._.|.S.).Nu....
-000012e0: 7365 7474 696e 6773 5f74 7970 6520 e985  settings_type ..
-000012f0: 8de7 bdae 3a20 7518 0000 0073 6372 6170  ....: u....scrap
-00001300: 7920 e5bd 93e5 898d e985 8de7 bdae e4b8  y ..............
-00001310: ba3a 2072 4600 0000 7524 0000 00e9 a1b9  .: rF...u$......
-00001320: e79b aee4 b8ad e985 8de7 bdae e4ba 8620  ............... 
-00001330: 6d79 7371 6c5f 636f 6e66 20e4 bfa1 e681  mysql_conf .....
-00001340: af7a 106d 7973 716c 2b70 796d 7973 716c  .z.mysql+pymysql
-00001350: 3a2f 2f72 5100 0000 fa01 3a72 5200 0000  ://rQ.....:rR...
-00001360: fa01 4072 4f00 0000 7250 0000 00fa 012f  ..@rO...rP...../
-00001370: 7253 0000 007a 093f 6368 6172 7365 743d  rS...z.?charset=
-00001380: 7254 0000 0029 0172 0c00 0000 7526 0000  rT...).r....u&..
-00001390: 00e9 a1b9 e79b aee4 b8ad e985 8de7 bdae  ................
-000013a0: e4ba 8620 6d6f 6e67 6f64 625f 636f 6e66  ... mongodb_conf
-000013b0: 20e4 bfa1 e681 af29 1372 2d00 0000 7208   ......).r-...r.
-000013c0: 0000 00da 0c66 726f 6d5f 6372 6177 6c65  .....from_crawle
-000013d0: 72da 0573 7461 7473 7239 0000 00da 0564  r..statsr9.....d
-000013e0: 6562 7567 723b 0000 00da 0464 6963 7472  ebugr;.....dictr
-000013f0: 3400 0000 7259 0000 00da 0469 6e66 6fda  4...rY.....info.
-00001400: 0a6d 7973 716c 5f63 6f6e 66da 146d 7973  .mysql_conf..mys
-00001410: 716c 5f65 6e67 696e 655f 656e 6162 6c65  ql_engine_enable
-00001420: 6472 3500 0000 7209 0000 0072 0a00 0000  dr5...r....r....
-00001430: 7232 0000 0072 5b00 0000 da0c 6d6f 6e67  r2...r[.....mong
-00001440: 6f64 625f 636f 6e66 2908 7215 0000 0072  odb_conf).r....r
-00001450: 3300 0000 7216 0000 0072 1700 0000 723e  3...r....r....r>
-00001460: 0000 0072 6400 0000 5a09 6d79 7371 6c5f  ...rd...Z.mysql_
-00001470: 7572 6c72 6600 0000 7230 0000 0072 0d00  urlrf...r0...r..
-00001480: 0000 720e 0000 0072 5f00 0000 de00 0000  ..r....r_.......
-00001490: 731e 0000 0000 0218 0108 0314 0118 0312  s...............
-000014a0: 010c 0106 0306 024a ff02 060e 0312 010c  .......J........
-000014b0: 0106 027a 1641 7975 5370 6964 6572 2e66  ...z.AyuSpider.f
-000014c0: 726f 6d5f 6372 6177 6c65 7229 1b72 1800  rom_crawler).r..
-000014d0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000014e0: 005a 1663 7573 746f 6d5f 636f 6d6d 6f6e  .Z.custom_common
-000014f0: 5f73 6574 7469 6e67 735a 1563 7573 746f  _settingsZ.custo
-00001500: 6d5f 6465 6275 675f 7365 7474 696e 6773  m_debug_settings
-00001510: 5a17 6375 7374 6f6d 5f70 726f 6475 6374  Z.custom_product
-00001520: 5f73 6574 7469 6e67 73da 0474 696d 65da  _settings..time.
-00001530: 0873 7472 6674 696d 65da 096c 6f63 616c  .strftime..local
-00001540: 7469 6d65 5a0b 5350 4944 4552 5f54 494d  timeZ.SPIDER_TIM
-00001550: 4572 3b00 0000 5a0f 7072 6f6a 6563 745f  Er;...Z.project_
-00001560: 636f 6e74 656e 7472 3a00 0000 7265 0000  contentr:...re..
-00001570: 0072 2e00 0000 720f 0000 00da 0870 726f  .r....r......pro
-00001580: 7065 7274 7972 3900 0000 da0b 636c 6173  pertyr9.....clas
-00001590: 736d 6574 686f 6472 4200 0000 7202 0000  smethodrB...r...
-000015a0: 0072 6200 0000 7259 0000 0072 5b00 0000  .rb...rY...r[...
-000015b0: 725f 0000 00da 0d5f 5f63 6c61 7373 6365  r_.....__classce
-000015c0: 6c6c 5f5f 720d 0000 0072 0d00 0000 7230  ll__r....r....r0
-000015d0: 0000 0072 0e00 0000 7208 0000 0026 0000  ...r....r....&..
-000015e0: 0073 5c00 0000 0801 0406 0201 0201 0201  .s\.............
-000015f0: 0201 02fb 060b 0201 0202 0202 0202 0202  ................
-00001600: 0202 0202 0202 02ef 0616 0201 0201 0201  ................
-00001610: 0201 0201 0201 0201 0201 02f7 060d 1002  ................
-00001620: 0402 0402 0402 0402 0c06 0c04 0201 0e14  ................
-00001630: 0201 0a0f 0204 0afd 0e26 0204 0afd 0e26  .........&.....&
-00001640: 0201 2911 721c 0000 0072 6700 0000 da06  ..).r....rg.....
-00001650: 7479 7069 6e67 7202 0000 00da 0e73 6372  typingr......scr
-00001660: 6170 792e 7370 6964 6572 7372 0300 0000  apy.spidersr....
-00001670: 5a0a 7371 6c61 6c63 6865 6d79 7204 0000  Z.sqlalchemyr...
-00001680: 005a 2461 7975 6765 7370 6964 6572 746f  .Z$ayugespiderto
-00001690: 6f6c 732e 636f 6d6d 6f6e 2e4d 756c 7469  ols.common.Multi
-000016a0: 506c 6578 696e 6772 0500 0000 5a1d 6179  Plexingr....Z.ay
-000016b0: 7567 6573 7069 6465 7274 6f6f 6c73 2e63  ugespidertools.c
-000016c0: 6f6d 6d6f 6e2e 5574 696c 7372 0600 0000  ommon.Utilsr....
-000016d0: 5a17 6179 7567 6573 7069 6465 7274 6f6f  Z.ayugespidertoo
-000016e0: 6c73 2e63 6f6e 6669 6772 0700 0000 da07  ls.configr......
-000016f0: 5f5f 616c 6c5f 5f72 0900 0000 7208 0000  __all__r....r...
-00001700: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00001710: 720e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001720: 0000 0073 1600 0000 0801 0801 0c02 0c01  ...s............
-00001730: 0c02 0c01 0c01 0c03 02ff 0405 0e15       ..............
+00000070: 6406 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
+00000080: 0100 6400 6407 6c0e 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6408 6c10 6d11 5a11 0100 6409 6701 5a12  d.l.m.Z...d.g.Z.
+000000a0: 4700 640a 640b 8400 640b 8302 5a13 4700  G.d.d...d...Z.G.
+000000b0: 640c 6409 8400 6409 6505 8303 5a14 6401  d.d...d.e...Z.d.
+000000c0: 5300 290d e900 0000 004e 2901 da05 556e  S.)......N)...Un
+000000d0: 696f 6e29 01da 0653 7069 6465 7229 01da  ion)...Spider)..
+000000e0: 0d63 7265 6174 655f 656e 6769 6e65 2901  .create_engine).
+000000f0: da0e 5265 7573 654f 7065 7261 7469 6f6e  ..ReuseOperation
+00000100: 2903 da0f 6765 745f 7370 6964 6572 5f63  )...get_spider_c
+00000110: 6f6e 66da 104d 7973 716c 436f 6e66 4372  onf..MysqlConfCr
+00000120: 6561 746f 72da 124d 6f6e 676f 4442 436f  eator..MongoDBCo
+00000130: 6e66 4372 6561 746f 7229 01da 0b54 6f6f  nfCreator)...Too
+00000140: 6c73 466f 7241 7975 2901 da06 6c6f 6767  lsForAyu)...logg
+00000150: 6572 da09 4179 7553 7069 6465 7263 0000  er..AyuSpiderc..
+00000160: 0000 0000 0000 0000 0000 0000 0000 0200  ................
+00000170: 0000 4000 0000 7328 0000 0065 005a 0164  ..@...s(...e.Z.d
+00000180: 005a 0264 015a 0365 04a0 05a1 005a 0664  .Z.d.Z.e.....Z.d
+00000190: 0264 0384 005a 0764 0464 0584 005a 0864  .d...Z.d.d...Z.d
+000001a0: 0653 0029 07da 104d 7953 716c 456e 6769  .S.)...MySqlEngi
+000001b0: 6e65 436c 6173 7375 2800 0000 0a20 2020  neClassu(....   
+000001c0: 206d 7973 716c 20e9 93be e68e a5e5 8fa5   mysql .........
+000001d0: e69f 84e5 8d95 e4be 8be6 a8a1 e5bc 8f0a  ................
+000001e0: 2020 2020 6302 0000 0000 0000 0000 0000      c...........
+000001f0: 0002 0000 0005 0000 0043 0000 0073 1400  .........C...s..
+00000200: 0000 7400 7c01 6401 6402 6403 8d03 7c00  ..t.|.d.d.d...|.
+00000210: 5f01 6400 5300 2904 4e54 6970 6200 0029  _.d.S.).NTipb..)
+00000220: 025a 0d70 6f6f 6c5f 7072 655f 7069 6e67  .Z.pool_pre_ping
+00000230: 5a0c 706f 6f6c 5f72 6563 7963 6c65 2902  Z.pool_recycle).
+00000240: 7204 0000 00da 0665 6e67 696e 6529 02da  r......engine)..
+00000250: 0473 656c 66da 0a65 6e67 696e 655f 7572  .self..engine_ur
+00000260: 6ca9 0072 1000 0000 fa4a 2f72 6f6f 742f  l..r.....J/root/
+00000270: 6d79 7072 6f6a 2f41 7975 6765 5370 6964  myproj/AyugeSpid
+00000280: 6572 546f 6f6c 732f 6179 7567 6573 7069  erTools/ayugespi
+00000290: 6465 7274 6f6f 6c73 2f73 6372 6170 6572  dertools/scraper
+000002a0: 2f73 7069 6465 7273 2f5f 5f69 6e69 745f  /spiders/__init_
+000002b0: 5f2e 7079 da08 5f5f 696e 6974 5f5f 1900  _.py..__init__..
+000002c0: 0000 730a 0000 0000 0102 0102 0002 0002  ..s.............
+000002d0: ff7a 194d 7953 716c 456e 6769 6e65 436c  .z.MySqlEngineCl
+000002e0: 6173 732e 5f5f 696e 6974 5f5f 6301 0000  ass.__init__c...
+000002f0: 0000 0000 0000 0000 0003 0000 0009 0000  ................
+00000300: 004f 0000 0073 3800 0000 7400 7401 6401  .O...s8...t.t.d.
+00000310: 8302 7332 7c00 6a02 8f1c 0100 7400 7401  ..s2|.j.....t.t.
+00000320: 6401 8302 7328 7403 a004 7c00 a101 7401  d...s(t...|...t.
+00000330: 5f05 5700 3500 5100 5200 5800 7401 6a05  _.W.5.Q.R.X.t.j.
+00000340: 5300 2902 4eda 095f 696e 7374 616e 6365  S.).N.._instance
+00000350: 2906 da07 6861 7361 7474 7272 0c00 0000  )...hasattrr....
+00000360: da0e 5f69 6e73 7461 6e63 655f 6c6f 636b  .._instance_lock
+00000370: da06 6f62 6a65 6374 da07 5f5f 6e65 775f  ..object..__new_
+00000380: 5f72 1300 0000 2903 da03 636c 73da 0461  _r....)...cls..a
+00000390: 7267 73da 066b 7761 7267 7372 1000 0000  rgs..kwargsr....
+000003a0: 7210 0000 0072 1100 0000 7217 0000 001e  r....r....r.....
+000003b0: 0000 0073 0a00 0000 0001 0a01 0801 0a01  ...s............
+000003c0: 1602 7a18 4d79 5371 6c45 6e67 696e 6543  ..z.MySqlEngineC
+000003d0: 6c61 7373 2e5f 5f6e 6577 5f5f 4e29 09da  lass.__new__N)..
+000003e0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000003f0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000400: 655f 5fda 075f 5f64 6f63 5f5f da09 7468  e__..__doc__..th
+00000410: 7265 6164 696e 67da 044c 6f63 6b72 1500  reading..Lockr..
+00000420: 0000 7212 0000 0072 1700 0000 7210 0000  ..r....r....r...
+00000430: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000440: 720c 0000 0012 0000 0073 0800 0000 0801  r........s......
+00000450: 0404 0802 0805 720c 0000 0063 0000 0000  ......r....c....
+00000460: 0000 0000 0000 0000 0000 0000 0a00 0000  ................
+00000470: 0000 0000 73ec 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000480: 0264 015a 0364 0264 0264 0364 0464 0564  .d.Z.d.d.d.d.d.d
+00000490: 069c 055a 0464 0764 0264 0864 0364 0264  ...Z.d.d.d.d.d.d
+000004a0: 0464 0964 0a64 0264 0b9c 095a 0564 0c64  .d.d.d.d...Z.d.d
+000004b0: 0264 0864 0364 0264 0464 0d64 0a64 0264  .d.d.d.d.d.d.d.d
+000004c0: 0b9c 095a 0665 07a0 0864 0e65 07a0 09a1  ...Z.e...d.e....
+000004d0: 00a1 025a 0a64 0f5a 0b64 105a 0c64 0a5a  ...Z.d.Z.d.Z.d.Z
+000004e0: 0d64 025a 0e87 0066 0164 1164 1284 085a  .d.Z...f.d.d...Z
+000004f0: 0f87 0066 0164 1364 1484 085a 1065 1187  ...f.d.d...Z.e..
+00000500: 0066 0164 1564 1684 0883 015a 1265 1364  .f.d.d.....Z.e.d
+00000510: 1764 1884 0083 015a 1465 1365 1565 1664  .d.....Z.e.e.e.d
+00000520: 0a66 0219 0064 199c 0164 1a64 1b84 0483  .f...d...d.d....
+00000530: 015a 1765 1365 1565 1664 0a66 0219 0064  .Z.e.e.e.d.f...d
+00000540: 199c 0164 1c64 1d84 0483 015a 1865 1387  ...d.d.....Z.e..
+00000550: 0066 0164 1e64 1f84 0883 015a 1987 0004  .f.d.d.....Z....
+00000560: 005a 1a53 0029 2072 0b00 0000 7556 0000  .Z.S.) r....uV..
+00000570: 000a 2020 2020 e794 a8e4 ba8e e588 9de5  ..    ..........
+00000580: a78b e985 8de7 bdae 2073 6372 6170 7920  ........ scrapy 
+00000590: e79a 84e5 9084 e7a7 8d20 7365 7474 696e  ......... settin
+000005a0: 6720 e79a 84e5 80bc e58f 8a20 7370 6964  g ......... spid
+000005b0: 6572 20e5 85a8 e5b1 80e5 8f98 e987 8fe7  er .............
+000005c0: ad89 0a20 2020 2046 e903 0000 00e9 ffff  ...    F........
+000005d0: ffff da03 6465 7629 05da 0e52 4f42 4f54  ....dev)...ROBOT
+000005e0: 5354 5854 5f4f 4245 59da 1554 454c 4e45  STXT_OBEY..TELNE
+000005f0: 5443 4f4e 534f 4c45 5f45 4e41 424c 4544  TCONSOLE_ENABLED
+00000600: da0b 5245 5452 595f 5449 4d45 53da 0e44  ..RETRY_TIMES..D
+00000610: 4550 5448 5f50 5249 4f52 4954 59da 0345  EPTH_PRIORITY..E
+00000620: 4e56 da05 4445 4255 47e9 1400 0000 da04  NV..DEBUG.......
+00000630: 7465 7374 4e29 09da 094c 4f47 5f4c 4556  testN)...LOG_LEV
+00000640: 454c 7224 0000 00da 1044 4f57 4e4c 4f41  ELr$.....DOWNLOA
+00000650: 445f 5449 4d45 4f55 5472 2600 0000 da10  D_TIMEOUTr&.....
+00000660: 5245 4449 5245 4354 5f45 4e41 424c 4544  REDIRECT_ENABLED
+00000670: 7227 0000 0072 2800 0000 da09 4441 5441  r'...r(.....DATA
+00000680: 5f45 4e55 4d5a 1352 4543 4f52 445f 4c4f  _ENUMZ.RECORD_LO
+00000690: 475f 544f 5f4d 5953 514c da05 4552 524f  G_TO_MYSQL..ERRO
+000006a0: 52da 0470 726f 647a 0825 592d 256d 2d25  R..prodz.%Y-%m-%
+000006b0: 64da 0663 6f6d 6d6f 6eda 0063 0200 0000  d..common..c....
+000006c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000006d0: 0b00 0000 7318 0000 0074 0074 017c 0083  ....s....t.t.|..
+000006e0: 026a 027c 0166 017c 028e 0101 0064 0153  .j.|.f.|.....d.S
+000006f0: 0029 0275 3d00 0000 0a20 2020 2020 2020  .).u=....       
+00000700: 20e5 ae9e e78e b0e6 8980 e7bb a7e6 89bf   ...............
+00000710: e7b1 bbe7 9a84 2061 6273 7472 6163 7420  ...... abstract 
+00000720: e696 b9e6 b395 2070 6172 7365 0a20 2020  ...... parse.   
+00000730: 2020 2020 204e 2903 da05 7375 7065 7272       N)...superr
+00000740: 0b00 0000 da05 7061 7273 6529 0372 0e00  ......parse).r..
+00000750: 0000 da08 7265 7370 6f6e 7365 721a 0000  ....responser...
+00000760: 00a9 01da 095f 5f63 6c61 7373 5f5f 7210  .....__class__r.
+00000770: 0000 0072 1100 0000 7235 0000 0062 0000  ...r....r5...b..
+00000780: 0073 0200 0000 0004 7a0f 4179 7553 7069  .s......z.AyuSpi
+00000790: 6465 722e 7061 7273 6563 0100 0000 0000  der.parsec......
+000007a0: 0000 0000 0000 0300 0000 0300 0000 0f00  ................
+000007b0: 0000 731c 0000 0074 0074 017c 0083 026a  ..s....t.t.|...j
+000007c0: 027c 017c 028e 0101 0064 007c 005f 0364  .|.|.....d.|._.d
+000007d0: 0053 0029 014e 2904 7234 0000 0072 0b00  .S.).N).r4...r..
+000007e0: 0000 7212 0000 00da 0c6d 7973 716c 5f65  ..r......mysql_e
+000007f0: 6e67 696e 6529 0372 0e00 0000 7219 0000  ngine).r....r...
+00000800: 0072 1a00 0000 7237 0000 0072 1000 0000  .r....r7...r....
+00000810: 7211 0000 0072 1200 0000 6800 0000 7304  r....r....h...s.
+00000820: 0000 0000 0112 017a 1241 7975 5370 6964  .......z.AyuSpid
+00000830: 6572 2e5f 5f69 6e69 745f 5f63 0100 0000  er.__init__c....
+00000840: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00000850: 0300 0000 734c 0000 007c 006a 006a 01a0  ....sL...|.j.j..
+00000860: 0264 01a1 017d 017c 006a 006a 01a0 0264  .d...}.|.j.j...d
+00000870: 0264 03a1 027d 0274 037c 0274 0483 0273  .d...}.t.|.t...s
+00000880: 3074 0564 0483 0182 017c 0272 3c7c 0170  0t.d.....|.r<|.p
+00000890: 3a74 0653 0074 0774 087c 0083 026a 0653  :t.S.t.t.|...j.S
+000008a0: 0064 0553 0029 0675 af00 0000 0a20 2020  .d.S.).u.....   
+000008b0: 2020 2020 20e6 9cac e5ba 93e7 9a84 e697       ...........
+000008c0: a5e5 bf97 e7ae a1e7 9086 e6a8 a1e5 9d97  ................
+000008d0: efbc 8ce4 bdbf e794 a820 6c6f 6775 7275  ......... loguru
+000008e0: 20e6 9da5 e7ae a1e7 9086 e697 a5e5 bf97   ...............
+000008f0: efbc 9b0a 2020 2020 2020 2020 e69c ace9  ....        ....
+00000900: 858d e7bd aee5 8faf e4b8 8e20 5363 7261  ........... Scra
+00000910: 7079 20e7 9a84 2073 7069 6465 722e 6c6f  py ... spider.lo
+00000920: 6720 e590 8ce6 97b6 e7ae a1e7 9086 efbc  g ..............
+00000930: 8ce6 a0b9 e68d aee5 9cba e699 afe5 8faf  ................
+00000940: e4bb a5e8 87aa e8a1 8ce9 858d e7bd aee3  ................
+00000950: 8082 0a20 2020 2020 2020 205a 0d4c 4f47  ...        Z.LOG
+00000960: 5552 555f 434f 4e46 4947 5a0e 4c4f 4755  URU_CONFIGZ.LOGU
+00000970: 5255 5f45 4e41 424c 4544 5475 2900 0000  RU_ENABLEDTu)...
+00000980: 6c6f 6775 7275 5f65 6e61 626c 6564 20e5  loguru_enabled .
+00000990: 8f82 e695 b0e6 a0bc e5bc 8fe9 9c80 e8a6  ................
+000009a0: 81e4 b8ba 2062 6f6f 6c4e 2909 da07 6372  .... boolN)...cr
+000009b0: 6177 6c65 72da 0873 6574 7469 6e67 73da  awler..settings.
+000009c0: 0367 6574 da0a 6973 696e 7374 616e 6365  .get..isinstance
+000009d0: da04 626f 6f6c da0e 4173 7365 7274 696f  ..bool..Assertio
+000009e0: 6e45 7272 6f72 720a 0000 0072 3400 0000  nErrorr....r4...
+000009f0: 720b 0000 0029 0372 0e00 0000 5a0f 6c6f  r....).r....Z.lo
+00000a00: 6775 7275 5f63 6f6e 665f 746d 705a 0e6c  guru_conf_tmpZ.l
+00000a10: 6f67 7572 755f 656e 6162 6c65 6472 3700  oguru_enabledr7.
+00000a20: 0000 7210 0000 0072 1100 0000 da04 736c  ..r....r......sl
+00000a30: 6f67 6c00 0000 730c 0000 0000 070e 0210  ogl...s.........
+00000a40: 0112 0304 0208 047a 0e41 7975 5370 6964  .......z.AyuSpid
+00000a50: 6572 2e73 6c6f 6763 0200 0000 0000 0000  er.slogc........
+00000a60: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
+00000a70: 735e 0000 0074 007c 0064 0164 0083 037d  s^...t.|.d.d...}
+00000a80: 0274 007c 0064 0264 0383 037d 0374 007c  .t.|.d.d...}.t.|
+00000a90: 0064 047c 039b 0064 059d 0369 0083 037d  .d.|...d...i...}
+00000aa0: 047c 0272 387c 027c 0464 063c 007c 016a  .|.r8|.|.d.<.|.j
+00000ab0: 017c 0464 0764 088d 0201 007c 016a 017c  .|.d.d.....|.j.|
+00000ac0: 006a 0270 5269 0064 0964 088d 0201 0064  .j.pRi.d.d.....d
+00000ad0: 0053 0029 0a4e da11 6375 7374 6f6d 5f74  .S.).N..custom_t
+00000ae0: 6162 6c65 5f65 6e75 6dda 0d73 6574 7469  able_enum..setti
+00000af0: 6e67 735f 7479 7065 7232 0000 005a 0763  ngs_typer2...Z.c
+00000b00: 7573 746f 6d5f da09 5f73 6574 7469 6e67  ustom_.._setting
+00000b10: 7372 2f00 0000 da07 7072 6f6a 6563 7429  sr/.....project)
+00000b20: 01da 0870 7269 6f72 6974 79da 0673 7069  ...priority..spi
+00000b30: 6465 7229 03da 0767 6574 6174 7472 da07  der)...getattr..
+00000b40: 7365 7464 6963 74da 0f63 7573 746f 6d5f  setdict..custom_
+00000b50: 7365 7474 696e 6773 2905 7218 0000 0072  settings).r....r
+00000b60: 3b00 0000 7241 0000 0072 4200 0000 5a0e  ;...rA...rB...Z.
+00000b70: 696e 6e65 725f 7365 7474 696e 6773 7210  inner_settingsr.
+00000b80: 0000 0072 1000 0000 7211 0000 00da 0f75  ...r....r......u
+00000b90: 7064 6174 655f 7365 7474 696e 6773 8100  pdate_settings..
+00000ba0: 0000 730e 0000 0000 020c 020c 0214 0204  ..s.............
+00000bb0: 0108 040e 017a 1941 7975 5370 6964 6572  .....z.AyuSpider
+00000bc0: 2e75 7064 6174 655f 7365 7474 696e 6773  .update_settings
+00000bd0: 2901 da06 7265 7475 726e 6302 0000 0000  )...returnc.....
+00000be0: 0000 0000 0000 0005 0000 0008 0000 0043  ...............C
+00000bf0: 0000 0073 ae00 0000 7c01 a000 6401 6900  ...s....|...d.i.
+00000c00: a102 7d02 7c01 a000 6402 6403 a102 7d03  ..}.|...d.d...}.
+00000c10: 7401 7c02 a000 6404 a101 0c00 7c03 0c00  t.|...d.....|...
+00000c20: 6702 8301 7232 6405 5300 7c03 7256 7402  g...r2d.S.|.rVt.
+00000c30: 6a03 7c01 6406 8d01 7d04 7404 6a05 6600  j.|.d...}.t.j.f.
+00000c40: 6407 6408 6901 7c04 9702 8e01 5300 7402  d.d.i.|.....S.t.
+00000c50: 6a06 7c02 6409 640a 640b 640c 640d 6404  j.|.d.d.d.d.d.d.
+00000c60: 6706 640e 8d02 72aa 7c02 a000 6409 a101  g.d...r.|...d...
+00000c70: 7c02 a000 640a a101 7c02 a000 640b a101  |...d...|...d...
+00000c80: 7c02 a000 640c a101 7c02 a000 6404 a101  |...d...|...d...
+00000c90: 7c02 a000 640d a101 70a4 640f 6410 9c06  |...d...p.d.d...
+00000ca0: 5300 6405 5300 2911 75e1 0000 000a 2020  S.d.S.).u.....  
+00000cb0: 2020 2020 2020 e6a0 b9e6 8dae e78e afe5        ..........
+00000cc0: a283 e88e b7e5 8f96 e79b b8e5 ba94 e79a  ................
+00000cd0: 8420 4d79 7371 6c20 e695 b0e6 8dae e5ba  . Mysql ........
+00000ce0: 93e9 858d e7bd aeef bc8c e88e b7e5 8f96  ................
+00000cf0: e585 b6e4 bb96 e887 aae5 ae9a e4b9 89e9  ................
+00000d00: 858d e7bd ae0a 2020 2020 2020 2020 4172  ......        Ar
+00000d10: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00000d20: 7365 7474 696e 6773 3a20 6372 6177 6c65  settings: crawle
+00000d30: 7220 7365 7474 696e 6773 20e9 858d e7bd  r settings .....
+00000d40: aee4 bfa1 e681 af0a 0a20 2020 2020 2020  .........       
+00000d50: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00000d60: 2020 2020 2020 3129 2e20 4d79 7371 6c20        1). Mysql 
+00000d70: e695 b0e6 8dae e5ba 93e9 93be e68e a5e9  ................
+00000d80: 858d e7bd ae0a 2020 2020 2020 2020 da12  ......        ..
+00000d90: 4c4f 4341 4c5f 4d59 5351 4c5f 434f 4e46  LOCAL_MYSQL_CONF
+00000da0: 4947 da0f 4150 505f 434f 4e46 5f4d 414e  IG..APP_CONF_MAN
+00000db0: 4147 4546 da08 4441 5441 4241 5345 4ea9  AGEF..DATABASEN.
+00000dc0: 0172 3b00 0000 da09 636f 6e66 5f6e 616d  .r;.....conf_nam
+00000dd0: 655a 054d 5953 514c da04 484f 5354 da04  eZ.MYSQL..HOST..
+00000de0: 504f 5254 da04 5553 4552 da08 5041 5353  PORT..USER..PASS
+00000df0: 574f 5244 da07 4348 4152 5345 54a9 025a  WORD..CHARSET..Z
+00000e00: 0964 6963 745f 636f 6e66 da08 6b65 795f  .dict_conf..key_
+00000e10: 6c69 7374 da07 7574 6638 6d62 3429 06da  list..utf8mb4)..
+00000e20: 0468 6f73 74da 0470 6f72 74da 0475 7365  .host..port..use
+00000e30: 72da 0870 6173 7377 6f72 64da 0864 6174  r..password..dat
+00000e40: 6162 6173 65da 0763 6861 7273 6574 a907  abase..charset..
+00000e50: 723c 0000 00da 0361 6c6c 7205 0000 00da  r<.....allr.....
+00000e60: 0f67 6574 5f63 6f6e 7375 6c5f 636f 6e66  .get_consul_conf
+00000e70: 7209 0000 005a 1267 6574 5f63 6f6e 665f  r....Z.get_conf_
+00000e80: 6279 5f63 6f6e 7375 6c5a 1669 735f 6469  by_consulZ.is_di
+00000e90: 6374 5f6d 6565 745f 6d69 6e5f 6c69 6d69  ct_meet_min_limi
+00000ea0: 7429 0572 1800 0000 723b 0000 00da 106c  t).r....r;.....l
+00000eb0: 6f63 616c 5f6d 7973 716c 5f63 6f6e 66da  ocal_mysql_conf.
+00000ec0: 0f61 7070 5f63 6f6e 665f 6d61 6e61 6765  .app_conf_manage
+00000ed0: da0b 636f 6e73 756c 5f63 6f6e 6672 1000  ..consul_confr..
+00000ee0: 0000 7210 0000 0072 1100 0000 da0e 6765  ..r....r......ge
+00000ef0: 745f 6d79 7371 6c5f 636f 6e66 9100 0000  t_mysql_conf....
+00000f00: 7324 0000 0000 0e0c 020c 0116 0104 0304  s$..............
+00000f10: 010c 0114 0304 0102 010e fe06 0508 0108  ................
+00000f20: 0108 0108 0108 010c fa7a 1841 7975 5370  .........z.AyuSp
+00000f30: 6964 6572 2e67 6574 5f6d 7973 716c 5f63  ider.get_mysql_c
+00000f40: 6f6e 6663 0200 0000 0000 0000 0000 0000  onfc............
+00000f50: 0500 0000 0800 0000 4300 0000 73a8 0000  ........C...s...
+00000f60: 007c 01a0 0064 0169 00a1 027d 027c 01a0  .|...d.i...}.|..
+00000f70: 0064 0264 03a1 027d 0374 017c 02a0 0064  .d.d...}.t.|...d
+00000f80: 04a1 010c 007c 030c 0067 0283 0172 3264  .....|...g...r2d
+00000f90: 0553 007c 0372 5674 026a 037c 0164 068d  .S.|.rVt.j.|.d..
+00000fa0: 017d 0474 046a 0566 0064 0764 0869 017c  .}.t.j.f.d.d.i.|
+00000fb0: 0497 028e 0153 0074 026a 067c 0264 0964  .....S.t.j.|.d.d
+00000fc0: 0a64 0b64 0c64 0467 0564 0d8d 0272 a47c  .d.d.d.g.d...r.|
+00000fd0: 02a0 0064 09a1 017c 02a0 0064 0aa1 017c  ...d...|...d...|
+00000fe0: 02a0 0064 0ba1 017c 02a0 0064 0ca1 017c  ...d...|...d...|
+00000ff0: 02a0 0064 0ea1 017c 02a0 0064 04a1 0164  ...d...|...d...d
+00001000: 0f9c 0653 0064 0553 0029 1075 e500 0000  ...S.d.S.).u....
+00001010: 0a20 2020 2020 2020 20e6 a0b9 e68d aee7  .        .......
+00001020: 8eaf e5a2 83e8 8eb7 e58f 96e7 9bb8 e5ba  ................
+00001030: 94e7 9a84 206d 6f6e 676f 4442 20e6 95b0  .... mongoDB ...
+00001040: e68d aee5 ba93 e985 8de7 bdae efbc 8ce8  ................
+00001050: 8eb7 e58f 96e5 85b6 e4bb 96e8 87aa e5ae  ................
+00001060: 9ae4 b989 e985 8de7 bdae 0a20 2020 2020  ...........     
+00001070: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00001080: 2020 2020 2073 6574 7469 6e67 733a 2063       settings: c
+00001090: 7261 776c 6572 2073 6574 7469 6e67 7320  rawler settings 
+000010a0: e985 8de7 bdae e4bf a1e6 81af 0a0a 2020  ..............  
+000010b0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+000010c0: 2020 2020 2020 2020 2020 2031 292e 204d             1). M
+000010d0: 6f6e 676f 4442 20e6 95b0 e68d aee5 ba93  ongoDB .........
+000010e0: e993 bee6 8ea5 e985 8de7 bdae 0a20 2020  .............   
+000010f0: 2020 2020 20da 144c 4f43 414c 5f4d 4f4e       ..LOCAL_MON
+00001100: 474f 4442 5f43 4f4e 4649 4772 4d00 0000  GODB_CONFIGrM...
+00001110: 4672 4e00 0000 4e72 4f00 0000 7250 0000  FrN...NrO...rP..
+00001120: 005a 074d 4f4e 474f 4442 7251 0000 0072  .Z.MONGODBrQ...r
+00001130: 5200 0000 7253 0000 0072 5400 0000 7256  R...rS...rT...rV
+00001140: 0000 00da 0a41 5554 4853 4f55 5243 4529  .....AUTHSOURCE)
+00001150: 0672 5900 0000 725a 0000 0072 5b00 0000  .rY...rZ...r[...
+00001160: 725c 0000 00da 0a61 7574 6873 6f75 7263  r\.....authsourc
+00001170: 6572 5d00 0000 725f 0000 0029 0572 1800  er]...r_...).r..
+00001180: 0000 723b 0000 00da 126c 6f63 616c 5f6d  ..r;.....local_m
+00001190: 6f6e 676f 6462 5f63 6f6e 6672 6300 0000  ongodb_confrc...
+000011a0: 7264 0000 0072 1000 0000 7210 0000 0072  rd...r....r....r
+000011b0: 1100 0000 da10 6765 745f 6d6f 6e67 6f64  ......get_mongod
+000011c0: 625f 636f 6e66 b800 0000 7324 0000 0000  b_conf....s$....
+000011d0: 0e0c 020c 0116 0104 0304 010c 0114 0304  ................
+000011e0: 0102 010c fe06 0508 0108 0108 0108 0108  ................
+000011f0: 0108 fa7a 1a41 7975 5370 6964 6572 2e67  ...z.AyuSpider.g
+00001200: 6574 5f6d 6f6e 676f 6462 5f63 6f6e 6663  et_mongodb_confc
+00001210: 0200 0000 0000 0000 0000 0000 0900 0000  ................
+00001220: 0e00 0000 0f00 0000 73fe 0000 0074 0074  ........s....t.t
+00001230: 017c 0083 026a 027c 0166 017c 029e 027c  .|...j.|.f.|...|
+00001240: 038e 017d 047c 016a 037c 045f 037c 046a  ...}.|.j.|._.|.j
+00001250: 04a0 0564 017c 006a 069b 009d 02a1 0101  ...d.|.j........
+00001260: 0074 076a 087c 016a 0964 028d 017d 0574  .t.j.|.j.d...}.t
+00001270: 0a74 0b83 006a 0c7c 016a 097c 0564 038d  .t...j.|.j.|.d..
+00001280: 0283 0104 007d 0672 ce7c 046a 04a0 0d64  .....}.r.|.j...d
+00001290: 04a1 0101 007c 067c 045f 0e7c 006a 0f72  .....|.|._.|.j.r
+000012a0: ce64 057c 06a0 1064 06a1 019b 0064 077c  .d.|...d.....d.|
+000012b0: 06a0 1064 08a1 019b 0064 097c 06a0 1064  ...d.....d.|...d
+000012c0: 0aa1 019b 0064 077c 06a0 1064 0ba1 019b  .....d.|...d....
+000012d0: 0064 0c7c 06a0 1064 0da1 019b 0064 0e7c  .d.|...d.....d.|
+000012e0: 06a0 1064 0fa1 019b 009d 0c7d 0774 117c  ...d.......}.t.|
+000012f0: 0764 108d 016a 127c 045f 1374 0a74 1483  .d...j.|._.t.t..
+00001300: 006a 0c7c 016a 097c 0564 038d 0283 0104  .j.|.j.|.d......
+00001310: 007d 0872 fa7c 046a 04a0 0d64 11a1 0101  .}.r.|.j...d....
+00001320: 007c 087c 045f 157c 0453 0029 124e 7516  .|.|._.|.S.).Nu.
+00001330: 0000 0073 6574 7469 6e67 735f 7479 7065  ...settings_type
+00001340: 20e9 858d e7bd ae3a 2072 4f00 0000 2902   ......: rO...).
+00001350: 723b 0000 0072 6400 0000 7524 0000 00e9  r;...rd...u$....
+00001360: a1b9 e79b aee4 b8ad e985 8de7 bdae e4ba  ................
+00001370: 8620 6d79 7371 6c5f 636f 6e66 20e4 bfa1  . mysql_conf ...
+00001380: e681 af7a 106d 7973 716c 2b70 796d 7973  ...z.mysql+pymys
+00001390: 716c 3a2f 2f72 5b00 0000 fa01 3a72 5c00  ql://r[.....:r\.
+000013a0: 0000 fa01 4072 5900 0000 725a 0000 00fa  ....@rY...rZ....
+000013b0: 012f 725d 0000 007a 093f 6368 6172 7365  ./r]...z.?charse
+000013c0: 743d 725e 0000 0029 0172 0f00 0000 7526  t=r^...).r....u&
+000013d0: 0000 00e9 a1b9 e79b aee4 b8ad e985 8de7  ................
+000013e0: bdae e4ba 8620 6d6f 6e67 6f64 625f 636f  ..... mongodb_co
+000013f0: 6e66 20e4 bfa1 e681 af29 1672 3400 0000  nf ......).r4...
+00001400: 720b 0000 00da 0c66 726f 6d5f 6372 6177  r......from_craw
+00001410: 6c65 72da 0573 7461 7473 7240 0000 00da  ler..statsr@....
+00001420: 0564 6562 7567 7242 0000 0072 0500 0000  .debugrB...r....
+00001430: 7261 0000 0072 3b00 0000 7206 0000 0072  ra...r;...r....r
+00001440: 0700 0000 5a0e 6372 6561 7465 5f70 726f  ....Z.create_pro
+00001450: 6475 6374 da04 696e 666f da0a 6d79 7371  duct..info..mysq
+00001460: 6c5f 636f 6e66 da14 6d79 7371 6c5f 656e  l_conf..mysql_en
+00001470: 6769 6e65 5f65 6e61 626c 6564 723c 0000  gine_enabledr<..
+00001480: 0072 0c00 0000 720d 0000 0072 3900 0000  .r....r....r9...
+00001490: 7208 0000 00da 0c6d 6f6e 676f 6462 5f63  r......mongodb_c
+000014a0: 6f6e 6629 0972 1800 0000 723a 0000 0072  onf).r....r:...r
+000014b0: 1900 0000 721a 0000 0072 4600 0000 5a0c  ....r....rF...Z.
+000014c0: 5f63 6f6e 7375 6c5f 636f 6e66 7272 0000  _consul_confrr..
+000014d0: 005a 096d 7973 716c 5f75 726c 7274 0000  .Z.mysql_urlrt..
+000014e0: 0072 3700 0000 7210 0000 0072 1100 0000  .r7...r....r....
+000014f0: 726e 0000 00df 0000 0073 2600 0000 0002  rn.......s&.....
+00001500: 1801 0803 1402 0e02 0201 10ff 0803 0c01  ................
+00001510: 0601 0602 4aff 0206 0e03 0201 10ff 0803  ....J...........
+00001520: 0c01 0601 7a16 4179 7553 7069 6465 722e  ....z.AyuSpider.
+00001530: 6672 6f6d 5f63 7261 776c 6572 291b 721b  from_crawler).r.
+00001540: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00001550: 0000 5a16 6375 7374 6f6d 5f63 6f6d 6d6f  ..Z.custom_commo
+00001560: 6e5f 7365 7474 696e 6773 5a15 6375 7374  n_settingsZ.cust
+00001570: 6f6d 5f64 6562 7567 5f73 6574 7469 6e67  om_debug_setting
+00001580: 735a 1763 7573 746f 6d5f 7072 6f64 7563  sZ.custom_produc
+00001590: 745f 7365 7474 696e 6773 da04 7469 6d65  t_settings..time
+000015a0: da08 7374 7266 7469 6d65 da09 6c6f 6361  ..strftime..loca
+000015b0: 6c74 696d 655a 0b53 5049 4445 525f 5449  ltimeZ.SPIDER_TI
+000015c0: 4d45 7242 0000 005a 0f70 726f 6a65 6374  MErB...Z.project
+000015d0: 5f63 6f6e 7465 6e74 7241 0000 0072 7300  _contentrA...rs.
+000015e0: 0000 7235 0000 0072 1200 0000 da08 7072  ..r5...r......pr
+000015f0: 6f70 6572 7479 7240 0000 00da 0b63 6c61  opertyr@.....cla
+00001600: 7373 6d65 7468 6f64 724a 0000 0072 0200  ssmethodrJ...r..
+00001610: 0000 da04 6469 6374 7265 0000 0072 6a00  ....dictre...rj.
+00001620: 0000 726e 0000 00da 0d5f 5f63 6c61 7373  ..rn.....__class
+00001630: 6365 6c6c 5f5f 7210 0000 0072 1000 0000  cell__r....r....
+00001640: 7237 0000 0072 1100 0000 720b 0000 0027  r7...r....r....'
+00001650: 0000 0073 5c00 0000 0801 0406 0201 0201  ...s\...........
+00001660: 0201 0201 02fb 060b 0201 0202 0202 0202  ................
+00001670: 0202 0202 0202 0202 02ef 0616 0201 0201  ................
+00001680: 0201 0201 0201 0201 0201 0201 02f7 060d  ................
+00001690: 1002 0402 0402 0402 0402 0c06 0c04 0201  ................
+000016a0: 0e14 0201 0a0f 0204 0afd 0e26 0204 0afd  ...........&....
+000016b0: 0e26 0201 2915 721f 0000 0072 7500 0000  .&..).r....ru...
+000016c0: da06 7479 7069 6e67 7202 0000 00da 0e73  ..typingr......s
+000016d0: 6372 6170 792e 7370 6964 6572 7372 0300  crapy.spidersr..
+000016e0: 0000 5a0a 7371 6c61 6c63 6865 6d79 7204  ..Z.sqlalchemyr.
+000016f0: 0000 00da 2461 7975 6765 7370 6964 6572  ....$ayugespider
+00001700: 746f 6f6c 732e 636f 6d6d 6f6e 2e4d 756c  tools.common.Mul
+00001710: 7469 506c 6578 696e 6772 0500 0000 5a24  tiPlexingr....Z$
+00001720: 6179 7567 6573 7069 6465 7274 6f6f 6c73  ayugespidertools
+00001730: 2e63 6f6d 6d6f 6e2e 5370 6964 6572 4442  .common.SpiderDB
+00001740: 436f 6e66 7206 0000 0072 0700 0000 7208  Confr....r....r.
+00001750: 0000 005a 1d61 7975 6765 7370 6964 6572  ...Z.ayugespider
+00001760: 746f 6f6c 732e 636f 6d6d 6f6e 2e55 7469  tools.common.Uti
+00001770: 6c73 7209 0000 005a 1761 7975 6765 7370  lsr....Z.ayugesp
+00001780: 6964 6572 746f 6f6c 732e 636f 6e66 6967  idertools.config
+00001790: 720a 0000 00da 075f 5f61 6c6c 5f5f 720c  r......__all__r.
+000017a0: 0000 0072 0b00 0000 7210 0000 0072 1000  ...r....r....r..
+000017b0: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+000017c0: 6f64 756c 653e 0100 0000 7318 0000 0008  odule>....s.....
+000017d0: 0108 010c 020c 010c 020c 0114 010c 010c  ................
+000017e0: 0302 ff04 050e 15                        .......
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/crawl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc` & `ayugespidertools-1.1.7/ayugespidertools/scraper/spiders/__pycache__/init.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/project/.gitignore` & `ayugespidertools-1.1.7/ayugespidertools/templates/project/.gitignore`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/project/module/VIT/.conf` & `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/VIT/.conf`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 00000040: 2a2a 0d0a 4348 4152 5345 543d 7574 6638  **..CHARSET=utf8
 00000050: 6d62 340d 0a0d 0a5b 4d4f 4e47 4f44 425d  mb4....[MONGODB]
 00000060: 0d0a 484f 5354 3d2a 2a2a 0d0a 504f 5254  ..HOST=***..PORT
 00000070: 3d32 3730 3137 0d0a 4441 5441 4241 5345  =27017..DATABASE
 00000080: 3d2a 2a2a 0d0a 4155 5448 534f 5552 4345  =***..AUTHSOURCE
 00000090: 3d2a 2a2a 0d0a 5553 4552 3d2a 2a2a 0d0a  =***..USER=***..
 000000a0: 5041 5353 574f 5244 3d2a 2a2a 0d0a 0d0a  PASSWORD=***....
-000000b0: 5b43 4f4e 5355 4c5d 0d0a 484f 5354 3d2a  [CONSUL]..HOST=*
-000000c0: 2a2a 0d0a 504f 5254 3d38 3530 300d 0a54  **..PORT=8500..T
-000000d0: 4f4b 454e 3d2a 2a2a 0d0a 4b45 595f 5641  OKEN=***..KEY_VA
-000000e0: 4c55 4553 3d2a 2a2a 0d0a 4752 4f55 503d  LUES=***..GROUP=
-000000f0: 0d0a 0d0a 5b4b 444c 5f44 594e 414d 4943  ....[KDL_DYNAMIC
-00000100: 5f50 524f 5859 5d0d 0a50 524f 5859 5f55  _PROXY]..PROXY_U
-00000110: 524c 3d6f 3636 382e 6b64 6c74 7073 2e63  RL=o668.kdltps.c
-00000120: 6f6d 3a31 3538 3138 0d0a 5553 4552 4e41  om:15818..USERNA
-00000130: 4d45 3d2a 2a2a 0d0a 5041 5353 574f 5244  ME=***..PASSWORD
-00000140: 3d2a 2a2a 0d0a 0d0a 5b4b 444c 5f45 5843  =***....[KDL_EXC
-00000150: 4c55 5349 5645 5f50 524f 5859 5d0d 0a50  LUSIVE_PROXY]..P
-00000160: 524f 5859 5f55 524c 3d68 7474 703a 2f2f  ROXY_URL=http://
-00000170: 6b70 732e 6b64 6c61 7069 2e63 6f6d 2f61  kps.kdlapi.com/a
-00000180: 7069 2f67 6574 6b70 733f 6f72 6465 7269  pi/getkps?orderi
-00000190: 643d 2a2a 2a26 6e75 6d3d 3130 3026 666f  d=***&num=100&fo
-000001a0: 726d 6174 3d6a 736f 6e0d 0a55 5345 524e  rmat=json..USERN
-000001b0: 414d 453d 2a2a 2a0d 0a50 4153 5357 4f52  AME=***..PASSWOR
-000001c0: 443d 2a2a 2a0d 0a50 524f 5859 5f49 4e44  D=***..PROXY_IND
-000001d0: 4558 3d31 0d0a 0d0a 5b41 4c49 5f4f 5353  EX=1....[ALI_OSS
-000001e0: 5d0d 0a4f 7373 4163 6365 7373 4b65 7949  ]..OssAccessKeyI
-000001f0: 643d 4c54 412a 2a2a 2a2a 2a0d 0a4f 7373  d=LTA******..Oss
-00000200: 4163 6365 7373 4b65 7953 6563 7265 743d  AccessKeySecret=
-00000210: 2a2a 2a2a 2a2a 0d0a 456e 6470 6f69 6e74  ******..Endpoint
-00000220: 3d68 7474 7073 3a2f 2f6f 7373 2d63 6e2d  =https://oss-cn-
-00000230: 2a2a 2a2a 2a2a 2e61 6c69 7975 6e63 732e  ******.aliyuncs.
-00000240: 636f 6d0d 0a45 7861 6d70 6c65 6275 636b  com..Examplebuck
-00000250: 6574 3d2a 2a2a 2a2a 2a0d 0a4f 7065 7261  et=******..Opera
-00000260: 7465 446f 633d 2a2a 2a2a 2a2a 2a0d 0a    teDoc=*******..
+000000b0: 5b43 4f4e 5355 4c5d 0d0a 544f 4b45 4e3d  [CONSUL]..TOKEN=
+000000c0: 2a2a 2a0d 0a55 524c 3d68 7474 703a 2f2f  ***..URL=http://
+000000d0: 686f 7374 3a70 6f72 742f 7631 2f6b 762f  host:port/v1/kv/
+000000e0: 2e2e 2e3f 6463 3d64 6331 0d0a 464f 524d  ...?dc=dc1..FORM
+000000f0: 4154 3d6a 736f 6e0d 0a0d 0a5b 4b44 4c5f  AT=json....[KDL_
+00000100: 4459 4e41 4d49 435f 5052 4f58 595d 0d0a  DYNAMIC_PROXY]..
+00000110: 5052 4f58 595f 5552 4c3d 6f36 3638 2e6b  PROXY_URL=o668.k
+00000120: 646c 7470 732e 636f 6d3a 3135 3831 380d  dltps.com:15818.
+00000130: 0a55 5345 524e 414d 453d 2a2a 2a0d 0a50  .USERNAME=***..P
+00000140: 4153 5357 4f52 443d 2a2a 2a0d 0a0d 0a5b  ASSWORD=***....[
+00000150: 4b44 4c5f 4558 434c 5553 4956 455f 5052  KDL_EXCLUSIVE_PR
+00000160: 4f58 595d 0d0a 5052 4f58 595f 5552 4c3d  OXY]..PROXY_URL=
+00000170: 6874 7470 3a2f 2f6b 7073 2e6b 646c 6170  http://kps.kdlap
+00000180: 692e 636f 6d2f 6170 692f 6765 746b 7073  i.com/api/getkps
+00000190: 3f6f 7264 6572 6964 3d2a 2a2a 266e 756d  ?orderid=***&num
+000001a0: 3d31 3030 2666 6f72 6d61 743d 6a73 6f6e  =100&format=json
+000001b0: 0d0a 5553 4552 4e41 4d45 3d2a 2a2a 0d0a  ..USERNAME=***..
+000001c0: 5041 5353 574f 5244 3d2a 2a2a 0d0a 5052  PASSWORD=***..PR
+000001d0: 4f58 595f 494e 4445 583d 310d 0a0d 0a5b  OXY_INDEX=1....[
+000001e0: 414c 495f 4f53 535d 0d0a 4f73 7341 6363  ALI_OSS]..OssAcc
+000001f0: 6573 734b 6579 4964 3d4c 5441 2a2a 2a2a  essKeyId=LTA****
+00000200: 2a2a 0d0a 4f73 7341 6363 6573 734b 6579  **..OssAccessKey
+00000210: 5365 6372 6574 3d2a 2a2a 2a2a 2a0d 0a45  Secret=******..E
+00000220: 6e64 706f 696e 743d 6874 7470 733a 2f2f  ndpoint=https://
+00000230: 6f73 732d 636e 2d2a 2a2a 2a2a 2a2e 616c  oss-cn-******.al
+00000240: 6979 756e 6373 2e63 6f6d 0d0a 4578 616d  iyuncs.com..Exam
+00000250: 706c 6562 7563 6b65 743d 2a2a 2a2a 2a2a  plebucket=******
+00000260: 0d0a 4f70 6572 6174 6544 6f63 3d2a 2a2a  ..OperateDoc=***
+00000270: 2a2a 2a2a 0d0a                           ****..
```

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/common/DataEnum.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/project/module/middlewares.py.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/project/module/settings.py.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/spiders/async.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/spiders/basic.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/spiders/crawl.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/spiders/csvfeed.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/templates/spiders/xmlfeed.tmpl` & `ayugespidertools-1.1.7/ayugespidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/ayugespidertools/utils/cmdline.py` & `ayugespidertools-1.1.7/ayugespidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `ayugespidertools-1.1.6/pyproject.toml` & `ayugespidertools-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AyugeSpiderTools"
-version = "1.1.6"
+version = "1.1.7"
 description = "scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。"
 authors = ["ayuge <ayugesheng@gmail.com>"]
 maintainers = ["ayuge <ayugesheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ayugespidertools"}]
 repository = "https://github.com/shengchenyang/AyugeSpiderTools"
 documentation = "https://ayugespidertools.readthedocs.io/en/latest/"
```

### Comparing `ayugespidertools-1.1.6/PKG-INFO` & `ayugespidertools-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayugespidertools
-Version: 1.1.6
+Version: 1.1.7
 Summary: scrapy 扩展库：用于扩展 Scrapy 功能来解放双手，还内置一些爬虫开发中的通用方法。
 Home-page: https://www.ayuge.top/mkdocs-material/
 Keywords: crawler,scraping,twisted,aiohttp,asyncio,scrapy,aiomysql,mmh3
 Author: ayuge
 Author-email: ayugesheng@gmail.com
 Maintainer: ayuge
 Maintainer-email: ayugesheng@gmail.com
@@ -139,14 +139,21 @@
 + 8).demo_eight: 同时存入 Mysql 和 MongoDB 的场景
 
 - 9).demo_aiohttp_example: scrapy Request 替换为 aiohttp 请求的场景，提供了各种请求场景示例（GET,POST）
 + 10).demo_aiohttp_test: scrapy aiohttp 在具体项目中的使用方法示例
 
 + 11).demo_proxy_one: 快代理动态隧道代理示例
 + 12).demo_proxy_two: 测试快代理独享代理
+
++13).demo_AyuTurboMysqlPipeline: mysql 同步连接池的示例
++14).demo_crawl: 支持 scrapy CrawlSpider 的示例
+
+# 本库中给出支持 Item Loaders 特性的示例(文档地址：https://ayugespidertools.readthedocs.io/en/latest/topics/loaders.html)
++15).demo_item_loader: 本库 ScrapyClassicItem 及原生 scrapy item 动态添加 item 字段及支持 Item Loaders 的示例
++16).demo_item_loader_two: 展示本库使用 itemLoader 特性的示例
 ```
 
 注：具体内容及时效性请以 [DemoSpider](https://github.com/shengchenyang/DemoSpider) 项目中描述为准。
 
 ### 2.2. 开发场景
 
 > 这里不再一一列举所有功能，大概介绍下包含的大致功能。
@@ -194,25 +201,25 @@
 据 [3.2](#3.2.-你可能在意的事) 可知，你可以 `clone` 源码后，修改任意方法（比如你的项目场景下可能需要其它的日志配置默认值，或添加其它的项目结构模板等），修改完成后 `poetry  build` 或 `make build` 即可打包使用。
 
 比如你可能需要更新依赖库中 `pymongo` 为新版本 `x.x.x`，那只需 `poetry install` 安装现有依赖后，再 `poetry add pymongo@x.x.x` 安装目标版本（尽量不要使用 `poetry update pymongo`），确定测试正常了即可 `poetry build` 打包使用。
 
 ## TodoList
 
 - [x] `scrapy` 的扩展功能场景
-  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~ 
+  - [ ] ~~`scrapy` 结合 `crawlab` 的日志统计功能~~
   - [x] `scrapy` 脚本运行信息统计和项目依赖表采集量统计，可用于日志记录和预警
   - [x] 自定义模板，在 `ayugespidertools startproject <projname>` 和 `ayugespidertools genspider <spidername>` 时生成适合本库的模板文件
   - [x] ~~增加根据 `nacos` 来获取配置的功能~~ -> 改为增加根据 `consul` 来获取配置的功能
   - [x] 代理中间件（独享代理、动态隧道代理）
   - [x] 随机请求头 `UA` 中间件，根据 `fake_useragent` 中的权重来随机
   - [x] 使用以下工具来替换 `scrapy` 的 `Request` 来发送请求
-    - [ ] `selenum`: 性能没有 `pyppeteer` 强
+    - [ ] ~~`selenium`: 性能没有 `pyppeteer` 强~~
     - [x] `pyppeteer`: `Gerapy-pyppeteer` 库已经实现此功能
     - [x] `requests`: 这个不推荐使用，`requests` 同步库会降低 `scrapy` 运行效率
-    - [ ] `splash`: 继承 `splash` 渲染 `js` 的功能
+    - [ ] ~~`splash`: 继承 `splash` 渲染 `js` 的功能~~
     - [x] `aiohttp`: 集成将 `scrapy Request` 替换为 `aiohttp` 的协程方式
   - [x] `Mysql` 存储的场景下适配
     - [x] 自动创建 `Mysql` 用户场景下需要的数据库和数据表及字段格式，还有字段注释
   - [x] `MongoDB` 存储的场景下适配，编写风格与 `Mysql` 存储等场景下一致
   - [x] `asyncio` 语法支持与 `async` 第三方库支持示例
     - [x] `spider` 中使用 `asyncio` 的 `aiohttp` 示例
     - [x] `pipeline` 中使用 `asyncio` 的 `aioMysql` 示例
@@ -226,7 +233,12 @@
   - [x] `html` 数据处理，去除标签，不可见字符，特殊字符改成正常显示等等等
   - [x] 添加常用的图片验证码中的处理方法
     - [x] 滑块缺口距离的识别方法（多种实现方式）
     - [x] 根据滑块距离生成轨迹数组的方法
     - [x] 识别点选验证码位置及点击顺序，识别结果不太好，待优化
     - [x] 图片乱序混淆的还原方法示例
 
+注：
+
+- 不再开发结合 `selenium` 扩展的功能，推荐使用 `scrapy-playwright`，`Gerapy-pyppeteer` 等其它库；
+- 不再开发结合 `splash` 的功能，如果使用 `splash http api` 的话，在 `scrapy` ，本库或自写脚本中都比较容易扩展。如果要使用 `lua` `api` 等复杂的功能那还是推荐 `scrapy-splash` 这类的扩展库。
+
```

