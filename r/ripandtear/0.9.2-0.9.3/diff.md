# Comparing `tmp/ripandtear-0.9.2.tar.gz` & `tmp/ripandtear-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripandtear-0.9.2.tar", last modified: Thu Mar  2 23:15:46 2023, max compression
+gzip compressed data, was "ripandtear-0.9.3.tar", last modified: Tue Apr 11 15:17:30 2023, max compression
```

## Comparing `ripandtear-0.9.2.tar` & `ripandtear-0.9.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-03-02 23:15:46.048971 ripandtear-0.9.2/
--rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.2/LICENSE
--rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-03-02 23:15:46.048971 ripandtear-0.9.2/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)    16527 2023-02-28 03:34:50.000000 ripandtear-0.9.2/README.md
--rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.2/pyproject.toml
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-03-02 23:15:46.040971 ripandtear-0.9.2/ripandtear/
--rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/__main__.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-03-02 23:15:46.044971 ripandtear-0.9.2/ripandtear/extractors/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.2/ripandtear/extractors/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    13230 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/extractors/bunkr.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/extractors/common.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6444 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/extractors/coomer.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4997 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/extractors/cyberdrop.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2390 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/extractors/gfycat.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5239 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/extractors/gofile.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7920 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/extractors/imgur.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6544 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/extractors/jpg.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    18031 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/extractors/reddit.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6449 2023-02-27 19:38:52.000000 ripandtear-0.9.2/ripandtear/extractors/redgifs.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6004 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/extractors/tiktits.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-03-02 23:15:46.048971 ripandtear-0.9.2/ripandtear/utils/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.2/ripandtear/utils/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/utils/cli_arguments.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/utils/color.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6754 2023-02-28 02:57:32.000000 ripandtear-0.9.2/ripandtear/utils/conductor.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/utils/content_finder.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/utils/custom_types.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8858 2023-02-27 19:38:52.000000 ripandtear-0.9.2/ripandtear/utils/downloader.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.2/ripandtear/utils/file_hasher.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2361 2023-02-20 00:52:42.000000 ripandtear-0.9.2/ripandtear/utils/file_sorter.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/utils/logger.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/utils/progress.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.2/ripandtear/utils/rat_info.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.2/ripandtear/utils/rat_interaction.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4131 2023-03-02 23:14:20.000000 ripandtear-0.9.2/ripandtear/utils/tracker.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-03-02 23:15:46.044971 ripandtear-0.9.2/ripandtear.egg-info/
--rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/SOURCES.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/dependency_links.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/entry_points.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/requires.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-03-02 23:15:46.000000 ripandtear-0.9.2/ripandtear.egg-info/top_level.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-03-02 23:15:46.052971 ripandtear-0.9.2/setup.cfg
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.308816 ripandtear-0.9.3/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.3/LICENSE
+-rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-04-11 15:17:30.308816 ripandtear-0.9.3/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)    16527 2023-02-28 03:34:50.000000 ripandtear-0.9.3/README.md
+-rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.3/pyproject.toml
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.300816 ripandtear-0.9.3/ripandtear/
+-rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-03-09 22:35:04.000000 ripandtear-0.9.3/ripandtear/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/__main__.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.304816 ripandtear-0.9.3/ripandtear/extractors/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.3/ripandtear/extractors/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-02 21:19:42.000000 ripandtear-0.9.3/ripandtear/extractors/bunkr.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/extractors/common.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-03-20 18:38:53.000000 ripandtear-0.9.3/ripandtear/extractors/coomer.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-02 22:53:26.000000 ripandtear-0.9.3/ripandtear/extractors/cyberdrop.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-03-12 23:21:36.000000 ripandtear-0.9.3/ripandtear/extractors/gfycat.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-03-12 23:22:37.000000 ripandtear-0.9.3/ripandtear/extractors/gofile.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-03-12 23:23:07.000000 ripandtear-0.9.3/ripandtear/extractors/imgur.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-02 19:55:36.000000 ripandtear-0.9.3/ripandtear/extractors/jpg.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-03-31 03:36:45.000000 ripandtear-0.9.3/ripandtear/extractors/reddit.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6506 2023-03-12 16:08:32.000000 ripandtear-0.9.3/ripandtear/extractors/redgifs.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-03-12 23:25:25.000000 ripandtear-0.9.3/ripandtear/extractors/tiktits.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.308816 ripandtear-0.9.3/ripandtear/utils/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.3/ripandtear/utils/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.3/ripandtear/utils/cli_arguments.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/color.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-02 18:45:08.000000 ripandtear-0.9.3/ripandtear/utils/conductor.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-03-02 23:14:20.000000 ripandtear-0.9.3/ripandtear/utils/content_finder.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/custom_types.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-02 04:30:56.000000 ripandtear-0.9.3/ripandtear/utils/downloader.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.3/ripandtear/utils/file_hasher.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-03-12 15:20:35.000000 ripandtear-0.9.3/ripandtear/utils/file_sorter.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/logger.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/progress.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.3/ripandtear/utils/rat_info.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.3/ripandtear/utils/rat_interaction.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-02 05:10:23.000000 ripandtear-0.9.3/ripandtear/utils/tracker.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-11 15:17:30.300816 ripandtear-0.9.3/ripandtear.egg-info/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    16917 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/SOURCES.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/dependency_links.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/entry_points.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/requires.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-11 15:17:30.000000 ripandtear-0.9.3/ripandtear.egg-info/top_level.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-11 15:17:30.308816 ripandtear-0.9.3/setup.cfg
```

### Comparing `ripandtear-0.9.2/LICENSE` & `ripandtear-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/PKG-INFO` & `ripandtear-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.2
+Version: 0.9.3
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.2/README.md` & `ripandtear-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/__main__.py` & `ripandtear-0.9.3/ripandtear/__main__.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/extractors/bunkr.py` & `ripandtear-0.9.3/ripandtear/extractors/bunkr.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,25 @@
 re_bunkr_media_files = re.compile(
     r"((media-files[\w]+)|(media-files))")
 
 # 'https://bunkr.su/v/0h1vsyrrw8558lb5agtx4_source-gigzea10.mp4'
 re_bunkr_video_href = re.compile(
     r"(/|/[v|d]/)([\w\-_\(\)\.]+)\.(\w+)")
 
-re_bunkr_video_extensions = re.compile(
-    r"(mkv|mp4|webm|mov|MOV)")
-
 re_bunkr_file_extensions = re.compile(
     r"(zip|rar|7z|txt)")
 
+re_bunkr_video_extensions = re.compile(
+    r"(mkv|mp4|webm|mov)")
+
+
 # 'https://bunkr.su/a/ouikRoFy'
 # 'https://stream.bunkr.ru/v/2022-04-23_Fake-Tan-01-Av9w6Za4.mp4'
 re_bunkr_album = re.compile(
-    r"(https?://)(bunkr.ru|bunkr.su|bunkr.is)/a/(\w+)")
+    r"(https?://)(bunkr.ru|bunkr.su|bunkr.is|bunkr.la)/a/(\w+)")
 
 # 'https://i.bunkr.ru/2316x3088_6f524042147f7b97c8c6e44ccab72374-jvBZFnON.jpg'
 # re_bunkr_single = re.compile(
 #     r"(https?://)([\w\-]+\.)?(bunkr\.(ru|la|su|is))(/|/[v|d]/)([\w\-_\(\)\.\%\’]+)\.(\w+)")
 re_bunkr_single = re.compile(
     r"(https?://)([\w\-]+\.)?(bunkr\.(ru|la|su|is))(/|/[v|d]/)(.*)\.(\w+)")
 
@@ -104,15 +105,15 @@
                     if url is None:
                         return
 
                     url_dictionary['url'] = str(url)
                     await self.url_dictionary_builder(url_dictionary.copy())
                     return
 
-            elif re_bunkr_video_extensions.match(re_bunkr_single.match(url_dictionary['url']).group(7)):
+            elif re_bunkr_video_extensions.match(re_bunkr_single.match(url_dictionary['url']).group(7).lower()):
 
                 log.debug("Video page found. Finding url")
                 async with sem:
                     await asyncio.sleep(random.randint(1, 4))
 
                     url = await self.bunkr_stream(url_dictionary)
 
@@ -151,14 +152,19 @@
                 return
 
         except AttributeError:
             log.exception(f"Unable to match {url_dictionary['url']}")
             await self.common_failed_attempt(url_dictionary)
             return
 
+        except TypeError:
+            log.exception(f"TypeError found for {url_dictionary['url']}")
+            await self.common_failed_attempt(url_dictionary)
+            return
+
     async def url_dictionary_builder(self, url_dictionary: UrlDictionary) -> None:
 
         try:
 
             log.debug("Sending request")
             async with httpx.AsyncClient() as client:
                 response = await client.head(f"{url_dictionary['url']}", timeout=None, follow_redirects=True)
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/common.py` & `ripandtear-0.9.3/ripandtear/extractors/common.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/extractors/coomer.py` & `ripandtear-0.9.3/ripandtear/extractors/coomer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 log = logging.getLogger(__name__)
 
 re_single_content = re.compile(
     r"(https?://)([\w]+\.)?((coomer)\.(party))(/(data))([\w\/]+)(/)([\w\-\_]+)\.(\w+)")
 
 re_content_page = re.compile(
-    r"(https?://)([\w]+\.)?((coomer)\.(party))(/(onlyfans)/)(user/)([\w\_\-]+)(/(post)/)([\w]+)")
+    r"(https?://)([\w]+\.)?((coomer)\.(party))(/(onlyfans)/)(user/)([\w\_\-\.]+)(/(post)/)([\w]+)")
 
 re_user_page = re.compile(
-    r"(https?://)([\w]+\.)?((coomer)\.(party))(/(onlyfans)/)(user/)([\w\_\-]+)(\?o=[\w]+)?")
+    r"(https?://)([\w]+\.)?((coomer)\.(party))(/(onlyfans)/)(user/)([\w\_\-\.]+)(\?o=[\w]+)?")
 
 
 class Coomer(Common):
 
     def __init__(self):
         self.tracker = Tracker.getInstance()
         self.prefix = 'coomer'
@@ -95,14 +95,15 @@
             url_dictionary['file_size'] = 0
 
         url_dictionary['extension'] = response.headers.get('content-type')
         url_dictionary['filename'] = self.common_filename_creator(
             url_dictionary.copy())
 
         # log.warn(url_dictionary)
+        log.debug("Url dictionary built. Sending to tracker")
         await self.tracker.add_url_dictionary(url_dictionary.copy())
         await self.common_advance_search_count(url_dictionary.copy())
 
     async def content_page_download(self, url_dictionary: UrlDictionary) -> None:
 
         if url_dictionary['url'] in self.already_downloaded:
             log.info(f"Already downloaded: {url_dictionary['url']}")
@@ -169,27 +170,32 @@
         except IndexError:
             count = 0
 
         username = re_user_page.match(url_dictionary['url']).group(9)
         while True:
 
             call_url = f"https://coomer.party/onlyfans/user/{username}?o={count}"
+            log.debug(f"Call Url: {call_url}")
 
             response = await self.call(call_url, url_dictionary.copy())
 
             if response is None:
                 log.error(f"Problem finding: {call_url}")
                 return
 
             html = BeautifulSoup(response.text, 'html.parser')
 
             posts = html.find_all('article', {'class': 'post-card'})
+            log.debug(f"Number of posts found: {len(posts)}")
 
             if len(posts) == 0:
+                log.info("No more posts found")
                 break
 
             for post in posts:
                 href = post.find('a')
                 url = f"https://coomer.party{href['href']}"
+                log.debug(url)
                 url_dictionary['url'] = url
+                log.debug(url_dictionary)
                 await self.run(url_dictionary.copy())
             count += 25
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/cyberdrop.py` & `ripandtear-0.9.3/ripandtear/extractors/cyberdrop.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 log = logging.getLogger(__name__)
 
 sem = asyncio.Semaphore(6)
 
 # 'https://cyberdrop.me/a/7ADTZ9dO'
 re_cyberdrop_album = re.compile(
-    r"(https?://)(www\.)?(cyberdrop\.(me))(/a/)(\w+)")
+    r"(https?://)(www\.)?(cyberdrop\.(cc|me|to))(/a/)(\w+)")
 
 re_cyberdrop_single = re.compile(
-    r"(https?://)([\w-]+\.)(cyberdrop\.(cc|to))/([\w\-_\(\)\%\+]+)\.(\w+)")
+    r"(https?://)([\w-]+\.)(cyberdrop\.(cc|me|to))/([\w\-_\(\)\%\+]+)\.(\w+)")
 
 
 class Cyberdrop(Common):
 
     def __init__(self):
 
         self.tracker = Tracker.getInstance()
@@ -58,14 +58,15 @@
             url_dictionary['file_size'] = int(
                 response.headers['Content-Length'])
             url_dictionary['filename'] = self.common_filename_creator(
                 url_dictionary.copy())
 
             # print(url_dictionary)
             # await self.common_file_downloader(url_dictionary.copy())
+            log.debug("Url dictionary built. Sending to tracker")
             await self.tracker.add_url_dictionary(url_dictionary.copy())
 
             url_dictionary['progress']['search_object'].advance(
                 url_dictionary['progress']['search_id'], 1)
 
     async def album_downloader(self, url_dictionary: UrlDictionary) -> None:
 
@@ -87,14 +88,15 @@
             await self.common_failed_attempt(url_dictionary)
             return
 
         if response.status_code >= 300:
             url_dictionary['response'] = response
 
             url_dictionary['fail'] = True
+            log.debug("Bulding dictionary failed. Sending to tracker")
             await self.tracker.add_url_dictionary(url_dictionary.copy())
 
             url_dictionary['progress']['search_object'].advance(
                 url_dictionary['progress']['search_id'], 1)
             return
 
         log.debug("Got response. Parsing for individual file urls")
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/gfycat.py` & `ripandtear-0.9.3/ripandtear/extractors/gfycat.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,9 +66,10 @@
         url_dictionary['date'] = data['gfyItem']['createDate']
         url_dictionary['file_size'] = data['gfyItem']['mp4Size']
         url_dictionary['extension'] = 'mp4'
         url_dictionary['filename'] = self.common_filename_creator(
             url_dictionary.copy())
 
         # await self.common_file_downloader(url_dictionary.copy())
+        log.info("Url dictionary built. Sending to tracker")
         await self.tracker.add_url_dictionary(url_dictionary.copy())
         await self.common_advance_search_count(url_dictionary.copy())
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/gofile.py` & `ripandtear-0.9.3/ripandtear/extractors/gofile.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     async def get_content(self, contentId: str, url_dictionary: UrlDictionary, password: Optional[str] = None) -> None:
 
         already_downloaded_urls: list[str] = rat_info.get_downloaded_urls()
 
         if already_downloaded_urls:
             if url_dictionary['url'] in already_downloaded_urls:
                 url_dictionary['completed'] = True
+                log.info("Already found. Sending to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
                 return
 
         params = {"contentId": contentId,
                   "token": self.token,
                   "websiteToken": self.website_token}
@@ -124,14 +125,15 @@
                 url_dictionary['url_to_download'] = item['link']
                 url_dictionary['cookies'] = {'accountToken': str(self.token)}
                 url_dictionary['file_size'] = item['size']
                 url_dictionary['extension'] = item['mimetype']
                 url_dictionary['filename'] = self.common_filename_creator(
                     url_dictionary.copy())
 
+                log.info("Url dictionary built. Sending to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
 
             elif item['type'] == 'folder':
                 url = f"https://gofile.io/d/{id}"
                 url_dictionary['url'] = url
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/imgur.py` & `ripandtear-0.9.3/ripandtear/extractors/imgur.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,15 @@
             url_dictionary['name'] = data['data']['id']
             url_dictionary['date'] = data['data']['datetime']
             url_dictionary['url_to_download'] = url_to_download
             url_dictionary['file_size'] = file_size
             url_dictionary['filename'] = self.common_filename_creator(
                 url_dictionary.copy())
 
-            log.info("Sending url_dictionary to tracker")
-
+            log.info("Url dictionary built. Sending to tracker")
             await self.tracker.add_url_dictionary(url_dictionary.copy())
             await self.common_advance_search_count(url_dictionary.copy())
 
         except KeyError:
             log.warn(f"Url missing keyword. Possibly deleted: {image_hash}")
 
             await self.common_failed_attempt(url_dictionary)
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/jpg.py` & `ripandtear-0.9.3/ripandtear/extractors/jpg.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 log = logging.getLogger(__name__)
 
 sem = asyncio.Semaphore(6)
 
 # 'https://simp4.jpg.church/1206x2208_bb3d16221cfbf54df75b3d2b6618b5e7.jpg'
 re_direct_image_link = re.compile(
-    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li))(/|/images/)([\w\/]+/)?([\w\-_\(\)\.]+)\.(\w+)")
+    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li|fishing))(/|/images/)([\w\/]+/)?([\w\-_\(\)\.]+)\.(\w+)")
 
 # 'https://jpg.fish/img/1206x2208-bb3d16221cfbf54df75b3d2b6618b5e7.TmmoSd'
 re_image_page = re.compile(
-    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li))(/(img|image)/)([\w\-_\(\)\.]+)\.(\w+)")
+    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li|fishing))(/(img|image)/)([\w\-_\(\)\.]+)\.(\w+)")
 
 # 'https://jpg.fish/a/finn.Hu6qp'
 re_album_page = re.compile(
-    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li))(/(a|album)/)([\w\-_\(\)\.]+)")
+    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li|fishing))(/(a|album)/)([\w\-_\(\)\.]+)")
 
 
 class Jpg(Common):
 
     def __init__(self):
         self.tracker = Tracker.getInstance()
 
@@ -83,26 +83,29 @@
             url_dictionary['url'] = url_dictionary['url'].replace(".md", "")
 
             response = await self.call(url_dictionary['url'])
 
             try:
                 # print(response.headers)
                 log.debug("Got response. Building dictionary")
-                url_dictionary['name'] = re_direct_image_link.match(
-                    url_dictionary['url']).group(8)
+
+                if url_dictionary.get('name') is None:
+                    url_dictionary['name'] = re_direct_image_link.match(
+                        url_dictionary['url']).group(8)
+
                 url_dictionary['extension'] = response.headers.get(
                     'content-type')
                 url_dictionary['url_to_download'] = url_dictionary['url']
                 url_dictionary['file_size'] = response.headers.get(
                     'content-length')
                 url_dictionary['filename'] = self.common_filename_creator(
                     url_dictionary)
 
                 # print(url_dictionary)
-                log.debug("Building Dictionary")
+                log.info("Url dictionary built. Sending to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
 
             except AttributeError:
                 log.debug("No response. Possible 404")
                 await self.common_failed_attempt(url_dictionary.copy())
                 return
@@ -112,17 +115,21 @@
         response = await self.call(url_dictionary['url'])
 
         try:
             soup = BeautifulSoup(response.text, 'html.parser')
             image_container = soup.find(
                 'div', {'id': 'image-viewer-container'})
             image_link = image_container.find('img')
+            name = soup.find(
+                'h1', {'class': 'phone-float-none'}).find('a').text
+            url_dictionary['name'] = name
+            log.debug(name)
 
         except AttributeError:
-            log.debug("AttributeError: url_dictionary['url']")
+            log.exception("AttributeError: url_dictionary['url']")
             await self.common_failed_attempt(url_dictionary.copy())
             return
 
         url = image_link['src']
         url = url.replace(".md", "")
         url_dictionary['url'] = url
 
@@ -135,60 +142,82 @@
 
         if url[-1] == '/':
             url = url[:-1]
 
         page = 1
         album_url = f"{url}/?sort=date_desc&page={page}"
 
-        saved_links = []
+        saved_links_url_dictionaries = []
         while True:
 
             log.info(f"Starting pass number {page}")
-            log.info(f"Number of links found: {len(saved_links)}")
+            log.info(
+                f"Number of links found: {len(saved_links_url_dictionaries)}")
 
             response = await self.call(album_url)
 
             soup = BeautifulSoup(response.text, 'html.parser')
             table = soup.find_all('div', {"class": "list-item"})
 
             if len(table) == 1:
                 for link in table:
-                    saved_links.append(link.find('img')['src'])
+
+                    url_dictionary['url'] = link.find('img')['src']
+                    url_dictionary['name'] = link.find(
+                        'div', {'class': "list-item-desc"}).find('a').text
+                    saved_links_url_dictionaries.append(url_dictionary.copy())
+
                 log.info("Found page with only 1 image. Breaking loop")
                 break
 
             for link in table:
-                # print(link)
-                saved_links.append(link.find('img')['src'])
+                # print(link.find('img')['src'])
+                url_dictionary['url'] = link.find('img')['src']
+                url_dictionary['name'] = link.find(
+                    'div', {'class': "list-item-desc"}).find('a').text
+                saved_links_url_dictionaries.append(url_dictionary.copy())
+
+            # There may be cases where the last image on the page has an error and doesn't contain
+            # a last-modified date in the header. If this occurs instead of looking at the last image
+            # the second to last image will be used. This variable is used to go back to the second
+            # to last image if needed be decrementing the variable
+
+            last_image_count = -1
+
+            last_image_dictionary = saved_links_url_dictionaries[last_image_count]
+            last_image_response = await self.call(last_image_dictionary['url'])
+
+            if last_image_response.headers.get('last-modified') is None:
+                last_image_count -= 1
+                last_image_response = await self.call(last_image_dictionary['url'])
 
             ids = [id['data-id'] for id in table]
             if len(ids) >= 1:
-                last_image_id = ids[-1]
+                last_image_id = ids[last_image_count]
 
             else:
                 break
 
-            last_image_response = await self.call(saved_links[-1])
             seek_date = await self.seek_date(last_image_response)
 
             page += 1
             album_url = f"{url}/?sort=date_desc&page={page}&seek={seek_date}.{last_image_id}"
 
-        saved_links = set(saved_links)
+        # saved_links_url_dictionaries = set(saved_links_url_dictionaries)
 
-        log.debug(f"Total number of links found: {len(saved_links)}")
+        log.debug(
+            f"Total number of links found: {len(saved_links_url_dictionaries)}")
 
         tasks = []
         already_downloaded_urls = rat_info.get_downloaded_urls()
         log.debug("Attempting download of untracked links")
-        for url in saved_links:
-            url = url.replace(".md", "")
+        for url_dictionary in saved_links_url_dictionaries:
+            url_dictionary['url'] = url_dictionary['url'].replace(".md", "")
 
-            if url in already_downloaded_urls and url_dictionary['download'] is True:
+            if url_dictionary['url'] in already_downloaded_urls and url_dictionary['download'] is True:
                 continue
 
             else:
-                url_dictionary['url'] = url
                 tasks.append(asyncio.create_task(
                     self.run(url_dictionary.copy())))
 
         await asyncio.gather(*tasks)
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/reddit.py` & `ripandtear-0.9.3/ripandtear/extractors/reddit.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,16 @@
                     url_dictionary['file_size'] = int(
                         data['Content-Length'])
 
                 url_dictionary['extension'] = data['content-type']
                 url_dictionary['filename'] = self.common_filename_creator(
                     url_dictionary)
 
-                log.debug("url_dictionary sent to downloader")
-
                 # await self.common_file_downloader(url_dictionary.copy())
+                log.info("Url dictionary built. Sending to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
 
             except Exception:
                 log.exception(
                     f"Problem downloading file. Saving for later: {url_dictionary['url_to_download']}")
                 await self.common_failed_attempt(url_dictionary.copy())
@@ -246,14 +245,15 @@
                 url_dictionary['extension'] = 'mp4'
 
                 url_dictionary['filename'] = self.common_filename_creator(
                     url_dictionary.copy())
 
                 # print(url_dictionary)
                 # await self.common_file_downloader(url_dictionary.copy())
+                log.info("Url dictionary built. Sending to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
                 return
 
             await self.reddit_post(url_dictionary.copy())
 
     async def reddit_post(self, url_dictionary: UrlDictionary) -> None:
@@ -374,14 +374,16 @@
                     elif post['data']['url'] not in already_downloaded_urls and url_dictionary['download'] is True:
                         url_dictionary['reddit_uniq_id'] = post['data']['id']
                         tasks.append(asyncio.create_task(
                             self.reddit_post(url_dictionary.copy())))
 
                     elif url_dictionary['download'] is False:
                         url_dictionary['url_to_download'] = post['data']['url']
+
+                        log.info("Url dictionary built. Sending to tracker")
                         await self.tracker.add_url_dictionary(url_dictionary.copy())
                         continue
 
                 if data['data']['after']:
                     params['after'] = data['data']['after']
 
                 else:
@@ -399,51 +401,56 @@
         log.debug("gallery found")
         image_order = []
         for entry in post['gallery_data']['items']:
             id = entry['media_id']
             image_order.append(id)
 
         count = 0
-        for id in image_order:
+        try:
+            for id in image_order:
 
-            count += 1
+                count += 1
 
-            image_link = post['media_metadata'][id]['p'][0]['u']
+                image_link = post['media_metadata'][id]['p'][0]['u']
 
-            url_dictionary['name'] = re_reddit_gallery_link.match(
-                image_link).group(4)
+                url_dictionary['name'] = re_reddit_gallery_link.match(
+                    image_link).group(4)
 
-            url_dictionary['extension'] = re_reddit_gallery_link.match(
-                image_link).group(5)
+                url_dictionary['extension'] = re_reddit_gallery_link.match(
+                    image_link).group(5)
 
-            image_url = f"https://i.redd.it/{url_dictionary['name']}.{url_dictionary['extension']}"
+                image_url = f"https://i.redd.it/{url_dictionary['name']}.{url_dictionary['extension']}"
 
-            async with httpx.AsyncClient() as client:
-                response = await client.head(
-                    image_url, headers=self.headers, timeout=None)
+                async with httpx.AsyncClient() as client:
+                    response = await client.head(
+                        image_url, headers=self.headers, timeout=None)
+
+                temp = json.dumps(dict(response.headers))
+                data = json.loads(temp)
 
-            temp = json.dumps(dict(response.headers))
-            data = json.loads(temp)
+                url_dictionary['prefix'] = self.prefix
+                url_dictionary['date'] = post['created_utc']
 
-            url_dictionary['prefix'] = self.prefix
-            url_dictionary['date'] = post['created_utc']
+                url_dictionary['album_name'] = url_dictionary['reddit_uniq_id']
+                url_dictionary['count'] = count
+                url_dictionary['description'] = str(post['title'])
 
-            url_dictionary['album_name'] = url_dictionary['reddit_uniq_id']
-            url_dictionary['count'] = count
-            url_dictionary['description'] = str(post['title'])
+                if data.get('content-length'):
+                    url_dictionary['file_size'] = int(data['content-length'])
 
-            if data.get('content-length'):
-                url_dictionary['file_size'] = int(data['content-length'])
+                url_dictionary['url_to_download'] = image_url
+                url_dictionary['filename'] = self.common_filename_creator(
+                    url_dictionary.copy())
 
-            url_dictionary['url_to_download'] = image_url
-            url_dictionary['filename'] = self.common_filename_creator(
-                url_dictionary.copy())
+                log.info("Url dictionary built. Sending to tracker")
+                await self.tracker.add_url_dictionary(url_dictionary.copy())
+                await self.common_advance_search_count(url_dictionary.copy())
 
-            await self.tracker.add_url_dictionary(url_dictionary.copy())
-            await self.common_advance_search_count(url_dictionary.copy())
+        except IndexError:
+            pass
 
     async def reddit_video_download(self, post, url_dictionary):
 
         log.info(f"Reddit video found: {post['url']}")
 
         url_dictionary['ytdlp_required'] = True
         url_dictionary['prefix'] = self.prefix
@@ -452,9 +459,10 @@
         url_dictionary['description'] = post['title']
         url_dictionary['url_to_download'] = str(post['url'])
         url_dictionary['extension'] = "mp4"
         url_dictionary['filename'] = self.common_filename_creator(
             url_dictionary.copy())
 
         # await self.common_file_downloader(url_dictionary.copy())
+        log.info("Url dictionary built. Sending to tracker")
         await self.tracker.add_url_dictionary(url_dictionary.copy())
         await self.common_advance_search_count(url_dictionary.copy())
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/redgifs.py` & `ripandtear-0.9.3/ripandtear/extractors/redgifs.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 sem = asyncio.Semaphore(6)
 
 
 class Redgifs(Common):
 
     def __init__(self):
-        self .tracker = Tracker.getInstance()
+        self.tracker = Tracker.getInstance()
 
     async def get_token(self) -> None:
 
         log.debug("Requesting auth token")
         headers = {'token': ''}
 
         async with httpx.AsyncClient() as client:
@@ -107,14 +107,15 @@
                 url_dictionary['extension'] = re_extension.match(
                     url_dictionary['url_to_download']).group(6)
 
                 url_dictionary['filename'] = self.common_filename_creator(
                     url_dictionary)
 
                 # await self.common_file_downloader(url_dictionary.copy())
+                log.info("Sending dictionary to tracker")
                 await self.tracker.add_url_dictionary(url_dictionary.copy())
                 await self.common_advance_search_count(url_dictionary.copy())
 
     async def user_download_v3(self, username: str, url_dictionary: UrlDictionary) -> None:
 
         log.info(f"Redgifs user Found: {username}")
```

### Comparing `ripandtear-0.9.2/ripandtear/extractors/tiktits.py` & `ripandtear-0.9.3/ripandtear/extractors/tiktits.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,9 +177,10 @@
         url_dictionary['extension'] = response.headers.get('content-type')
 
         url_dictionary['filename'] = self.common_filename_creator(
             url_dictionary.copy())
 
         # print(url_dictionary)
         # await self.common_file_downloader(url_dictionary.copy())
+        log.info("Url dictionary built. Sending to tracker")
         await self.tracker.add_url_dictionary(url_dictionary.copy())
         await self.common_advance_search_count(url_dictionary.copy())
```

### Comparing `ripandtear-0.9.2/ripandtear/utils/cli_arguments.py` & `ripandtear-0.9.3/ripandtear/utils/cli_arguments.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/color.py` & `ripandtear-0.9.3/ripandtear/utils/color.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/conductor.py` & `ripandtear-0.9.3/ripandtear/utils/conductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 gofile_re = re.compile(r"(https?://)(gofile\.io)")
 
 gfycat_re = re.compile(r"(https?://)(gfycat\.com(/))")
 
 imgur_re = re.compile(r"(https?://)?(www\.|[im]\.)?imgur\.(?:com|io)")
 
 # both jpg and pixl
-jpg_re = re.compile(r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li))")
+jpg_re = re.compile(
+    r"(https?://)(\w+\.)?((jpg|pixl)\.(church|fish|li|fishing))")
 
 reddit_re = re.compile(r"(https?://)([iv]\.|www\.)?(reddit|redd\.it)")
 
 redgifs_re = re.compile(r"(https?://)(v3\.|www\.|i.)?(redgifs.com)")
 
 tiktits_re = re.compile(r"(https?://)(tiktits\.(com))")
```

### Comparing `ripandtear-0.9.2/ripandtear/utils/content_finder.py` & `ripandtear-0.9.3/ripandtear/utils/content_finder.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/custom_types.py` & `ripandtear-0.9.3/ripandtear/utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/downloader.py` & `ripandtear-0.9.3/ripandtear/utils/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import json
 import httpx
 import logging
 import os
 
 import yt_dlp
 from pathlib import Path
@@ -12,186 +11,160 @@
 from ripandtear.utils.progress import file_progress, file_category_progress
 
 log = logging.getLogger(__name__)
 
 
 async def download_file(url_dictionary: UrlDictionary, asyncio_semphore) -> None:
 
-    log.debug("Inside downloader")
-
-    url_to_download = str(url_dictionary['url_to_download'])
-    url_dictionary['url_to_download'] = url_to_download
-
-    if url_dictionary.get('url_to_record'):
-
-        url_to_record = str(url_dictionary['url_to_record'])
-        url_dictionary['url_to_record'] = url_to_record
-
-    if url_dictionary.get("file_size"):
-        file_size = int(url_dictionary['file_size'])
-
-    else:
-        file_size = 0
-
-    log.debug("Checking if url has already been downloaded")
-    if url_dictionary.get('url_to_record'):
-
-        if rat_info.check_existence(category_1='urls_downloaded', entry=url_dictionary['url_to_record']):
-
-            log.info(
-                f"Url already recorded: {url_dictionary['url_to_record']}")
-            file_category_progress.advance(
-                url_dictionary['progress']['completed_id'], 1)
-            return
+    async with asyncio_semphore:
+        log.debug("Inside downloader")
 
-    if url_dictionary.get('url_to_download'):
+        if url_dictionary.get("file_size"):
+            file_size = int(url_dictionary['file_size'])
 
-        if rat_info.check_existence(category_1='urls_downloaded', entry=url_dictionary['url_to_download']):
+        else:
+            file_size = 0
 
-            log.info(f"Url already recorded: {url_to_download}")
-            file_category_progress.advance(
-                url_dictionary['progress']['completed_id'], 1)
+        if url_dictionary.get('ytdlp_required'):
+            ytdlp_download(url_dictionary)
             return
 
-    log.debug("url has not been downloaded yet")
+        # is_file_local returns a tuple that says if the file exists in the
+        # first position and many bytes have been downloaded in the second
+        # Ex: (True, 8473)
 
-    if url_dictionary.get('ytdlp_required'):
-        ytdlp_download(url_dictionary)
-        return
+        log.debug("Checking if file exists locally")
 
-    # is_file_local returns a tuple that says if the file exists in the
-    # first position and many bytes have been downloaded in the second
-    # Ex: (True, 8473)
+        if url_dictionary.get('filename'):
+            filename = url_dictionary['filename']
 
-    log.debug("Checking if file exists locally")
+        else:
+            filename = url_dictionary['url_to_download'].split('/')[-1]
 
-    if url_dictionary.get('filename'):
-        filename = url_dictionary['filename']
+        is_file_local = local_file_exists(filename, file_size)
 
-    else:
-        filename = url_dictionary['url_to_download'].split('/')[-1]
-
-    is_file_local = local_file_exists(filename, file_size)
+        try:
+            if is_file_local[0] == "True":
 
-    try:
-        if is_file_local[0] == "True":
+                if is_file_local[1] == "done":
 
-            if is_file_local[1] == "done":
+                    file_category_progress.advance(
+                        url_dictionary['progress']['completed_id'], 1)
+                    return
 
-                file_category_progress.advance(
-                    url_dictionary['progress']['completed_id'], 1)
-                return
+                else:
 
+                    mode = 'ab'
+                    initial_position = is_file_local[1]
             else:
 
-                mode = 'ab'
-                initial_position = is_file_local[1]
-        else:
+                mode = 'wb'
+                initial_position = 0
 
-            mode = 'wb'
-            initial_position = 0
+        except TypeError:
+            log.error("Filename too long. Skipping")
 
-    except TypeError:
-        log.error("Filename too long. Skipping")
+            rat_info.add_entry(category_1='urls_downloaded',
+                               entry=str(url_dictionary['url']))
 
-        rat_info.add_entry(category_1='urls_downloaded',
-                           entry=str(url_dictionary['url']))
+            file_category_progress.advance(
+                url_dictionary['progress']['failed_id'], 1)
 
-        file_category_progress.advance(
-            url_dictionary['progress']['failed_id'], 1)
+            return
 
-        return
+        headers = {'Range': f'bytes={initial_position}-'}
 
-    headers = {'Range': f'bytes={initial_position}-'}
+        if url_dictionary.get('headers'):
 
-    if url_dictionary.get('headers'):
+            for key, value in url_dictionary['headers'].items():
+                headers[key] = value
 
-        for key, value in url_dictionary['headers'].items():
-            headers[key] = value
+        if len(filename) > 60:
+            name = filename[:57] + "..."
 
-    async with asyncio_semphore:
+        else:
+            name = filename
+
+        file_progress_id = file_progress.add_task(
+            f"{name}", completed=initial_position, total=file_size)
 
         try:
             cookies = None
             if url_dictionary.get('cookies'):
                 cookies = url_dictionary['cookies']
 
             async with httpx.AsyncClient() as client:
                 async with client.stream('GET',
-                                         url_to_download,
+                                         url_dictionary['url_to_download'],
                                          headers=headers,
                                          timeout=None,
                                          cookies=cookies,
                                          follow_redirects=True) as response:
 
                     if response.status_code >= 300:
 
                         url_dictionary['status_code'] = int(
                             response.status_code)
 
-                        await errors(url_dictionary.copy())
+                        await errors(url_dictionary.copy(), file_progress_id)
                         return
 
                     temp = json.dumps(dict(response.headers))
                     data = json.loads(temp)
 
-                    try:
-                        if isinstance(int(data.get('content-length')), int):
-                            file_size = int(data.get('content-length'))
-
-                    except TypeError:
-                        pass
-
-                    except KeyError:
-                        pass
+                    if file_size == 0:
+                        try:
+                            if isinstance(int(data.get('content-length')), int):
+                                file_size = int(data.get('content-length'))
+                                file_progress.update(
+                                    file_progress_id, total=file_size)
 
-                    if len(filename) > 60:
-                        name = filename[:57] + "..."
+                        except TypeError:
+                            pass
 
-                    else:
-                        name = filename
-
-                    file_progress_id = file_progress.add_task(
-                        f"{name}", completed=initial_position, total=file_size)
+                        except KeyError:
+                            pass
 
                     file = open(filename, mode)
                     async for chunk in response.aiter_bytes(8192):
                         size = file.write(chunk)
                         file_progress.update(file_progress_id, advance=size)
 
                     file_progress.update(file_progress_id, visible=False)
                     file_category_progress.advance(
                         url_dictionary['progress']['downloaded_id'], 1)
 
         except FileNotFoundError:
 
+            file_progress.update(file_progress_id, visible=False)
             file_category_progress.advance(
                 url_dictionary['progress']['failed_id'], 1)
             return
 
         except Exception:
             log.exception(
                 f"Unable to download: {url_dictionary['url_to_download']}")
             rat_info.add_error_dictionary(url_dictionary.copy())
+            file_progress.update(file_progress_id, visible=False)
             file_category_progress.advance(
                 url_dictionary['progress']['failed_id'], 1)
             return
 
-    try:
-        if url_dictionary.get('url_to_record'):
+        try:
+            if url_dictionary.get('url_to_record'):
 
-            rat_info.add_entry(category_1='urls_downloaded',
-                               entry=url_dictionary['url_to_record'])
+                rat_info.add_entry(category_1='urls_downloaded',
+                                   entry=url_dictionary['url_to_record'])
 
-        else:
-            rat_info.add_entry(category_1='urls_downloaded',
-                               entry=url_dictionary['url_to_download'])
+            else:
+                rat_info.add_entry(category_1='urls_downloaded',
+                                   entry=url_dictionary['url_to_download'])
 
-    except ValueError as identifier:
-        log.info(identifier)
+        except ValueError as identifier:
+            log.info(identifier)
 
 
 def local_file_exists(filename, online_file_size):
 
     try:
         if Path(filename).exists():
 
@@ -212,49 +185,53 @@
         else:
             return ("False")
 
     except OSError:
         return
 
 
-async def errors(url_dictionary):
+async def errors(url_dictionary, file_progress_id):
 
     log.error("Finding bad status code")
 
     if url_dictionary['status_code'] == 403:
 
         log.error(f"Authorization Error - {url_dictionary['url']}")
 
         rat_info.add_error_dictionary(url_dictionary.copy())
+        file_progress.update(file_progress_id, visible=False)
         file_category_progress.advance(
             url_dictionary['progress']['failed_id'], 1)
 
     elif url_dictionary['status_code'] == 404:
 
         log.error(
             f"Content was deleted or did not exist: {url_dictionary['status_code']} - {url_dictionary['url']}")
 
         rat_info.add_error_dictionary(url_dictionary.copy())
+        file_progress.update(file_progress_id, visible=False)
         file_category_progress.advance(
             url_dictionary['progress']['failed_id'], 1)
 
     elif url_dictionary['status_code'] == 429:
 
         log.error(f"{url_dictionary['status_code']}: Too Many Requests")
 
         rat_info.add_error_dictionary(url_dictionary.copy())
+        file_progress.update(file_progress_id, visible=False)
         file_category_progress.advance(
             url_dictionary['progress']['failed_id'], 1)
 
     elif 500 <= url_dictionary['status_code'] < 600:
 
         log.error(
             f"500 error. Saving the url to be attempted later: {url_dictionary['status_code']} - {url_dictionary['url_to_download']}")
 
         rat_info.add_error_dictionary(url_dictionary.copy())
+        file_progress.update(file_progress_id, visible=False)
         file_category_progress.advance(
             url_dictionary['progress']['failed_id'], 1)
 
     else:
         log.error(
             f"Unable to download {url_dictionary['status_code']}: {url_dictionary['url']}")
 
@@ -279,8 +256,7 @@
     except yt_dlp.utils.DownloadError:
         log.info(
             f"Problem downloading url. Saving for later: {url_dictionary['url_to_download']}")
         rat_info.add_error_dictionary(url_dictionary)
         file_category_progress.advance(
             url_dictionary['progress']['failed_id'], 1)
         return
-
```

### Comparing `ripandtear-0.9.2/ripandtear/utils/file_hasher.py` & `ripandtear-0.9.3/ripandtear/utils/file_hasher.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/file_sorter.py` & `ripandtear-0.9.3/ripandtear/utils/file_sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 
 async def sort():
 
     files = [file for file in Path().cwd().iterdir() if file.is_file()]
 
     log.info("Sorting files...")
-    try:
-        for file in files:
+    for file in files:
 
+        try:
             source = Path(file).name
 
             if image_suffix.match(Path(file).suffix).group(1):
 
                 destination = (f"pics/{Path(file).name}")
                 dir = 'pics'
                 await move_file(source, destination, dir)
@@ -49,16 +49,16 @@
 
             elif text_suffix.match(Path(file).suffix).group(1):
 
                 destination = (f"text/{Path(file).name}")
                 dir = 'text'
                 await move_file(source, destination, dir)
 
-    except AttributeError:
-        log.info(f"Did not find mattching pattern for: {Path(file).name}")
+        except AttributeError:
+            log.info(f"Did not find mattching pattern for: {Path(file).name}")
 
 
 async def file_size(source_file, destination_file):
 
     source_file_bytes = Path(source_file).stat().st_size
 
     destination_file_bytes = Path(destination_file).stat().st_size
```

### Comparing `ripandtear-0.9.2/ripandtear/utils/progress.py` & `ripandtear-0.9.3/ripandtear/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/rat_info.py` & `ripandtear-0.9.3/ripandtear/utils/rat_info.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/rat_interaction.py` & `ripandtear-0.9.3/ripandtear/utils/rat_interaction.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/ripandtear/utils/tracker.py` & `ripandtear-0.9.3/ripandtear/utils/tracker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import logging
 
+
 from ripandtear.utils.progress import file_category_progress
 from ripandtear.utils import rat_info
 
 from ripandtear.utils import downloader
 
 log = logging.getLogger(__name__)
 
@@ -18,14 +19,15 @@
         if Tracker.__instance is None:
             Tracker()
         return Tracker.__instance
 
     def __init__(self):
         Tracker.__instance = self
         self.url_dictionaries = []
+        self.fast_dictionaries = []
         self.medium_dictionaries = []
         self.slow_dictionaries = []
 
     async def add_url_dictionary(self, url_dictionary):
         log.debug("Adding url_dictionary")
         self.url_dictionaries.append(url_dictionary)
 
@@ -49,66 +51,82 @@
         downloaded_id = file_category_progress.add_task(
             "Downloaded", total=self.total_url_dictionaries())
 
         fast_semaphore = asyncio.Semaphore(6)
         medium_semaphore = asyncio.Semaphore(4)
         slow_semaphore = asyncio.Semaphore(2)
 
-        tasks = []
         already_downloaded_urls = rat_info.get_downloaded_urls()
+
         for url_dictionary in self.url_dictionaries:
 
             url_dictionary['progress'] = {}
             url_dictionary['progress']['failed_id'] = failed_id
             url_dictionary['progress']['completed_id'] = completed_id
             url_dictionary['progress']['downloaded_id'] = downloaded_id
 
             # This is to handle cases where an error dictionary might not
             # have set the url_to_download before encountering an error,
             # but set the correct url to ['url']
 
             if url_dictionary.get('url_to_download') is None:
                 url_dictionary['url_to_download'] = url_dictionary['url']
+                continue
 
             if url_dictionary.get('fail'):
                 rat_info.add_error_dictionary(url_dictionary.copy())
                 file_category_progress.advance(
                     url_dictionary['progress']['failed_id'], 1)
                 continue
 
-            elif url_dictionary.get('completed'):
+            if url_dictionary.get('completed'):
                 file_category_progress.advance(
                     url_dictionary['progress']['completed_id'], 1)
                 continue
 
-            elif url_dictionary.get('url_to_record'):
+            log.debug("Checking if url has already been downloaded")
+            if url_dictionary.get('url_to_record'):
                 if url_dictionary['url_to_record'] in already_downloaded_urls:
+                    log.info(
+                        f"Url already recorded: {url_dictionary['url_to_record']}")
                     file_category_progress.advance(
                         url_dictionary['progress']['completed_id'], 1)
                     continue
 
-            elif url_dictionary['url_to_download'] in already_downloaded_urls:
+            if url_dictionary['url_to_download'] in already_downloaded_urls:
+                log.info(
+                    f"Url already recorded: {url_dictionary['url_to_download']}")
                 file_category_progress.advance(
                     url_dictionary['progress']['completed_id'], 1)
                 continue
 
+            log.debug("url has not been downloaded yet")
+
             if 'media-files' in url_dictionary['url_to_download']:
                 self.slow_dictionaries.append(asyncio.create_task(
                     downloader.download_file(url_dictionary.copy(), slow_semaphore)))
                 continue
 
             if 'coomer' in url_dictionary['url_to_download']:
                 self.slow_dictionaries.append(asyncio.create_task(
                     downloader.download_file(url_dictionary.copy(), slow_semaphore)))
                 continue
 
-            tasks.append(asyncio.create_task(
-                downloader.download_file(url_dictionary.copy(), fast_semaphore)))
-
-        log.info("Starting Fast Downloads")
-        await asyncio.gather(*tasks)
+            if 'cyberdrop' in url_dictionary['url_to_download']:
+                self.medium_dictionaries.append(asyncio.create_task(
+                    downloader.download_file(url_dictionary.copy(), medium_semaphore)))
+                continue
 
-        log.info("Starting Medium Downloads")
-        await asyncio.gather(*self.medium_dictionaries)
+            self.fast_dictionaries.append(asyncio.create_task(
+                downloader.download_file(url_dictionary.copy(), fast_semaphore)))
 
-        log.info("Starting Slow Downloads")
-        await asyncio.gather(*self.slow_dictionaries)
+        if len(self.fast_dictionaries) >= 1:
+            log.info("Starting Fast Downloads")
+            await asyncio.gather(*self.fast_dictionaries)
+
+        if len(self.medium_dictionaries) >= 1:
+            log.info("Starting Medium Downloads")
+            await asyncio.gather(*self.medium_dictionaries)
+
+        if len(self.slow_dictionaries) >= 1:
+            log.info("Starting Slow Downloads")
+            await asyncio.gather(*self.slow_dictionaries)
```

### Comparing `ripandtear-0.9.2/ripandtear.egg-info/PKG-INFO` & `ripandtear-0.9.3/ripandtear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.2
+Version: 0.9.3
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.2/ripandtear.egg-info/SOURCES.txt` & `ripandtear-0.9.3/ripandtear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.2/setup.cfg` & `ripandtear-0.9.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	rfc3986==1.5.0
 	rich==13.3.1
 	sniffio==1.3.0
 	soupsieve==2.3.2.post1
 	typing_extensions==4.4.0
 	urllib3==1.26.12
 	websockets==10.1
-	yt-dlp==2023.1.6
+	yt-dlp==2023.3.4
 
 [options.entry_points]
 console_scripts = 
 	ripandtear = ripandtear.__main__:launch
 
 [egg_info]
 tag_build =
```

