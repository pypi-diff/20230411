# Comparing `tmp/bgmi-5.0.0a1.tar.gz` & `tmp/bgmi-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgmi-5.0.0a1.tar", max compression
+gzip compressed data, was "bgmi-5.0.0a2.tar", max compression
```

## Comparing `bgmi-5.0.0a1.tar` & `bgmi-5.0.0a2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1117 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/LICENSE
--rw-r--r--   0        0        0    14399 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/README.md
--rw-r--r--   0        0        0      176 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/__init__.py
--rw-r--r--   0        0        0       35 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/__main__.py
--rw-r--r--   0        0        0     6523 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/config.py
--rw-r--r--   0        0        0      240 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/downloader/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/downloader/aria2_rpc.py
--rw-r--r--   0        0        0     1558 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/downloader/deluge.py
--rw-r--r--   0        0        0     1752 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/downloader/qbittorrent.py
--rw-r--r--   0        0        0     1225 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/downloader/transmission.py
--rw-r--r--   0        0        0        0 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/__init__.py
--rw-r--r--   0        0        0     3230 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/admin.py
--rw-r--r--   0        0        0     2848 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/base.py
--rw-r--r--   0        0        0     2865 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/index.py
--rw-r--r--   0        0        0     3410 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/resources.py
--rw-r--r--   0        0        0     2272 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/server.py
--rw-r--r--   0        0        0      467 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/front/templates/download.xml
--rw-r--r--   0        0        0        0 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/__init__.py
--rw-r--r--   0        0        0      492 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/constants.py
--rw-r--r--   0        0        0    16873 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/controllers.py
--rw-r--r--   0        0        0     1867 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/download.py
--rw-r--r--   0        0        0      497 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/fetch.py
--rw-r--r--   0        0        0     9695 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/table.py
--rw-r--r--   0        0        0     1366 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/lib/update.py
--rw-r--r--   0        0        0    16986 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/main.py
--rw-r--r--   0        0        0       38 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/namespace.py
--rw-r--r--   0        0        0      163 2023-04-05 20:07:41.767620 bgmi-5.0.0a1/bgmi/others/cron.vbs
--rw-r--r--   0        0        0      922 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/others/crontab.sh
--rw-r--r--   0        0        0      543 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/others/me.ricterz.bgmi.plist
--rw-r--r--   0        0        0      499 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/others/nginx.conf
--rw-r--r--   0        0        0        0 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/plugin/__init__.py
--rw-r--r--   0        0        0      955 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/plugin/download.py
--rw-r--r--   0        0        0     7872 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/script.py
--rw-r--r--   0        0        0      875 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/session.py
--rw-r--r--   0        0        0     1430 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/setup.py
--rw-r--r--   0        0        0    10988 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/__init__.py
--rw-r--r--   0        0        0     8295 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/bangumi_moe.py
--rw-r--r--   0        0        0     6092 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/base.py
--rw-r--r--   0        0        0    13771 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/mikan.py
--rw-r--r--   0        0        0     1518 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/model.py
--rw-r--r--   0        0        0     9146 2023-04-05 20:07:41.771620 bgmi-5.0.0a1/bgmi/website/share_dmhy.py
--rw-r--r--   0        0        0     4556 2023-04-05 20:07:41.783620 bgmi-5.0.0a1/pyproject.toml
--rw-r--r--   0        0        0    16343 1970-01-01 00:00:00.000000 bgmi-5.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/LICENSE
+-rw-r--r--   0        0        0    14399 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/README.md
+-rw-r--r--   0        0        0      176 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/__init__.py
+-rw-r--r--   0        0        0       35 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/__main__.py
+-rw-r--r--   0        0        0     6523 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/config.py
+-rw-r--r--   0        0        0      240 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/aria2_rpc.py
+-rw-r--r--   0        0        0     1558 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/deluge.py
+-rw-r--r--   0        0        0     1752 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/qbittorrent.py
+-rw-r--r--   0        0        0     1225 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/downloader/transmission.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/__init__.py
+-rw-r--r--   0        0        0     3230 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/admin.py
+-rw-r--r--   0        0        0     2848 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/base.py
+-rw-r--r--   0        0        0     2865 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/index.py
+-rw-r--r--   0        0        0     3410 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/resources.py
+-rw-r--r--   0        0        0     2272 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/server.py
+-rw-r--r--   0        0        0      467 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/front/templates/download.xml
+-rw-r--r--   0        0        0        0 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/constants.py
+-rw-r--r--   0        0        0    16873 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/controllers.py
+-rw-r--r--   0        0        0     1867 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/download.py
+-rw-r--r--   0        0        0      497 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/fetch.py
+-rw-r--r--   0        0        0     9695 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/table.py
+-rw-r--r--   0        0        0     1366 2023-04-05 20:19:41.162937 bgmi-5.0.0a2/bgmi/lib/update.py
+-rw-r--r--   0        0        0    17010 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/main.py
+-rw-r--r--   0        0        0       38 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/namespace.py
+-rw-r--r--   0        0        0      163 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/cron.vbs
+-rw-r--r--   0        0        0      922 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/crontab.sh
+-rw-r--r--   0        0        0      543 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/me.ricterz.bgmi.plist
+-rw-r--r--   0        0        0      499 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/others/nginx.conf
+-rw-r--r--   0        0        0        0 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/plugin/__init__.py
+-rw-r--r--   0        0        0      955 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/plugin/download.py
+-rw-r--r--   0        0        0     7872 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/script.py
+-rw-r--r--   0        0        0      875 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/session.py
+-rw-r--r--   0        0        0     1430 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/setup.py
+-rw-r--r--   0        0        0    10988 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/__init__.py
+-rw-r--r--   0        0        0     8295 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/bangumi_moe.py
+-rw-r--r--   0        0        0     6092 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/base.py
+-rw-r--r--   0        0        0    13771 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/mikan.py
+-rw-r--r--   0        0        0     1518 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/model.py
+-rw-r--r--   0        0        0     9146 2023-04-05 20:19:41.166936 bgmi-5.0.0a2/bgmi/website/share_dmhy.py
+-rw-r--r--   0        0        0     4556 2023-04-05 20:19:41.178937 bgmi-5.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0    16343 1970-01-01 00:00:00.000000 bgmi-5.0.0a2/PKG-INFO
```

### Comparing `bgmi-5.0.0a1/LICENSE` & `bgmi-5.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/README.md` & `bgmi-5.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/config.py` & `bgmi-5.0.0a2/bgmi/config.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/downloader/aria2_rpc.py` & `bgmi-5.0.0a2/bgmi/downloader/aria2_rpc.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/downloader/deluge.py` & `bgmi-5.0.0a2/bgmi/downloader/deluge.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/downloader/qbittorrent.py` & `bgmi-5.0.0a2/bgmi/downloader/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/downloader/transmission.py` & `bgmi-5.0.0a2/bgmi/downloader/transmission.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/front/admin.py` & `bgmi-5.0.0a2/bgmi/front/admin.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/front/base.py` & `bgmi-5.0.0a2/bgmi/front/base.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/front/index.py` & `bgmi-5.0.0a2/bgmi/front/index.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/front/resources.py` & `bgmi-5.0.0a2/bgmi/front/resources.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/front/server.py` & `bgmi-5.0.0a2/bgmi/front/server.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/lib/controllers.py` & `bgmi-5.0.0a2/bgmi/lib/controllers.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/lib/download.py` & `bgmi-5.0.0a2/bgmi/lib/download.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/lib/table.py` & `bgmi-5.0.0a2/bgmi/lib/table.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/lib/update.py` & `bgmi-5.0.0a2/bgmi/lib/update.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/main.py` & `bgmi-5.0.0a2/bgmi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,30 +283,31 @@
         include=include,
         exclude=exclude,
         regex=regex,
     )
     if "data" not in result:
         globals()["print_{}".format(result["status"])](result["message"])
     else:
-        print_info("Usable subtitle group: {}".format(", ".join(result["data"]["subtitle_group"])))
+        print("Usable subtitle group: {}".format(", ".join(result["data"]["subtitle_group"])))
+        print()
         filter_obj = Followed.get(Followed.bangumi_name == result["data"]["name"])
         print_filter(filter_obj)
 
 
 def print_filter(followed_filter_obj: Followed) -> None:
     print(
         "Followed subtitle group: {}".format(
-            ", ".join(x.name for x in Subtitle.get_subtitle_by_id(followed_filter_obj.subtitle))
+            [x.name for x in Subtitle.get_subtitle_by_id(followed_filter_obj.subtitle)]
             if followed_filter_obj.subtitle
-            else "None"
+            else None
         )
     )
-    print(f"Include keywords: {followed_filter_obj.include}")
-    print(f"Exclude keywords: {followed_filter_obj.exclude}")
-    print(f"Regular expression: {followed_filter_obj.regex}")
+    print(f"Include keywords: {followed_filter_obj.include or None}")
+    print(f"Exclude keywords: {followed_filter_obj.exclude or None}")
+    print(f"Regular expression: {followed_filter_obj.regex or None}")
 
 
 @cli.command("cal")
 @click.option(
     "-f",
     "--force-update",
     "force_update",
```

### Comparing `bgmi-5.0.0a1/bgmi/others/crontab.sh` & `bgmi-5.0.0a2/bgmi/others/crontab.sh`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/others/me.ricterz.bgmi.plist` & `bgmi-5.0.0a2/bgmi/others/me.ricterz.bgmi.plist`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/plugin/download.py` & `bgmi-5.0.0a2/bgmi/plugin/download.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/script.py` & `bgmi-5.0.0a2/bgmi/script.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/session.py` & `bgmi-5.0.0a2/bgmi/session.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/setup.py` & `bgmi-5.0.0a2/bgmi/setup.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/utils/__init__.py` & `bgmi-5.0.0a2/bgmi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/website/bangumi_moe.py` & `bgmi-5.0.0a2/bgmi/website/bangumi_moe.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/website/base.py` & `bgmi-5.0.0a2/bgmi/website/base.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/website/mikan.py` & `bgmi-5.0.0a2/bgmi/website/mikan.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/website/model.py` & `bgmi-5.0.0a2/bgmi/website/model.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/bgmi/website/share_dmhy.py` & `bgmi-5.0.0a2/bgmi/website/share_dmhy.py`

 * *Files identical despite different names*

### Comparing `bgmi-5.0.0a1/pyproject.toml` & `bgmi-5.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bgmi"
-version = "5.0.0-alpha.1"
+version = "5.0.0-alpha.2"
 description = 'BGmi is a cli tool for subscribed bangumi.'
 authors = ["RicterZ <ricterzheng@gmail.com>"]
 readme = 'README.md'
 license = 'MIT'
 maintainers = ["Trim21 <i@trim21.me>"]
 homepage = 'https://github.com/BGmi/BGmi'
 repository = 'https://github.com/BGmi/BGmi'
```

### Comparing `bgmi-5.0.0a1/PKG-INFO` & `bgmi-5.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgmi
-Version: 5.0.0a1
+Version: 5.0.0a2
 Summary: BGmi is a cli tool for subscribed bangumi.
 Home-page: https://github.com/BGmi/BGmi
 License: MIT
 Keywords: bangumi,bgmi,feed
 Author: RicterZ
 Author-email: ricterzheng@gmail.com
 Maintainer: Trim21
```

