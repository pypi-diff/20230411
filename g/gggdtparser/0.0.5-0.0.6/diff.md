# Comparing `tmp/gggdtparser-0.0.5.tar.gz` & `tmp/gggdtparser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.0.5.tar", last modified: Mon Apr 10 04:26:42 2023, max compression
+gzip compressed data, was "gggdtparser-0.0.6.tar", last modified: Tue Apr 11 07:58:51 2023, max compression
```

## Comparing `gggdtparser-0.0.5.tar` & `gggdtparser-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.677419 gggdtparser-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-04-10 04:26:42.678417 gggdtparser-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.672432 gggdtparser-0.0.5/gggdtparser/
--rw-rw-rw-   0        0        0      259 2023-03-28 10:39:47.000000 gggdtparser-0.0.5/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0    11660 2023-04-10 03:37:05.000000 gggdtparser-0.0.5/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    15931 2023-04-10 01:46:49.000000 gggdtparser-0.0.5/gggdtparser/dtparser.py
--rw-rw-rw-   0        0        0    40554 2023-04-07 06:00:15.000000 gggdtparser-0.0.5/gggdtparser/test.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:26:42.676422 gggdtparser-0.0.5/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 04:26:42.000000 gggdtparser-0.0.5/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-04-10 04:26:42.685483 gggdtparser-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.565783 gggdtparser-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-04-11 07:58:51.566780 gggdtparser-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.560796 gggdtparser-0.0.6/gggdtparser/
+-rw-rw-rw-   0        0        0      259 2023-03-28 10:39:47.000000 gggdtparser-0.0.6/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0    12567 2023-04-11 07:54:36.000000 gggdtparser-0.0.6/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    15812 2023-04-11 07:32:49.000000 gggdtparser-0.0.6/gggdtparser/dtparser.py
+-rw-rw-rw-   0        0        0    41227 2023-04-11 06:55:56.000000 gggdtparser-0.0.6/gggdtparser/test.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.564786 gggdtparser-0.0.6/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-04-11 07:58:51.570961 gggdtparser-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.6/setup.py
```

### Comparing `gggdtparser-0.0.5/LICENSE` & `gggdtparser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.5/PKG-INFO` & `gggdtparser-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.5
+Version: 0.0.6
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.5/README.md` & `gggdtparser-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.5/gggdtparser/dtconfigs.py` & `gggdtparser-0.0.6/gggdtparser/dtconfigs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 # date: 2023/3/24
 
 
 STRING_DATE_TIME_REGEX_LIST = [
     # 精准策略
     r"(?P<ts>\d{13})",
     r"(?P<ts>\d{10})",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[:分]\s*(?P<S>\d{2})\s*[秒]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[分]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{2})\s*[时]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[:分]\s*(?P<S>\d{2})\s*[秒]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[分]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{2})\s*[时]?",
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})\s*[\-\|/\.月]\s*(?P<d>\d{2})\s*[日]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[分]?",
-    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<ap>am|pm)?\s*(?P<H>\d{1,2})\s*[时]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[分]?",
+    r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?\s*[T，]?\s*(?P<apm>am|pm)?\s*(?P<H>\d{1,2})\s*[时]?",
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
 
 
     # before
-    r"(?P<bd>\d+)\s*天\s*前",
-    r"(?P<bM>\d+)\s*分钟\s*前",
-    r"(?P<bH>\d+)\s*小时\s*前",
-    r"(?P<bm>\d+)\s*(个)?月\s*前",
-    r"(?P<bY>\d+)\s*年\s*前",
-    r"(?P<bS>\d+)\s*秒\s*前",
-    r"(?P<ba>\d+)\s*周\s*前",
-    r"(?P<ba>\d+)\s*星期\s*前",
+    r"(?P<bd>\d+)\s*天\s*(前|ago)",
+    r"(?P<bM>\d+)\s*分钟\s*(前|ago)",
+    r"(?P<bH>\d+)\s*小时\s*(前|ago)",
+    r"(?P<bm>\d+)\s*(个)?月\s*(前|ago)",
+    r"(?P<bY>\d+)\s*年\s*(前|ago)",
+    r"(?P<bS>\d+)\s*秒\s*(前|ago)",
+    r"(?P<ba>\d+)\s*周\s*(前|ago)",
+    r"(?P<ba>\d+)\s*星期\s*(前|ago)",
     # in
     r"(?P<wd>\d+)\s*天内",
     r"(?P<wM>\d+)\s*分钟内",
     r"(?P<wH>\d+)\s*小时内",
     r"(?P<wm>\d+)\s*(个)?月内",
     r"(?P<wY>\d+)\s*年内",
     r"(?P<wS>\d+)\s*秒内",
@@ -52,15 +52,17 @@
     r"(?P<sd>前天)",
     r"(?P<so>刚刚)",
 ]
 
 STRING_DATE_TIME_REGEX_LIST_FUZZY = [  # 模糊时间
     # 2010 7月19日
     r"(?P<Y>\d{4})\s*[\-\|/\.年]?\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
-    # 14 March 2023
+    # 10 апреля 2023, 18:57
+    r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})\s*[,]?\s*(?P<H>\d{2})\s*[:时h]\s*(?P<M>\d{2})\s*[分]?",
+    # # 14 March 2023
     r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})",
     # 2023/0329
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{2})(?P<d>\d{2})",
     # 2012.9
     r"(?P<Y>\d{4})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})",
     r"(?P<m>\d{1,2})\s*[\-\|/\.月]?\s*(?P<d>\d{1,2})\s*[\-\|/\.日]?\s*?(?P<Y>\d{4})\s*[\-\|/\.年]?",
     # 11/1/2018
@@ -84,33 +86,39 @@
     # Feb 5
     r"(?P<m>\d{1,2})\s*[月]\s*(?P<d>\d{1,2})",
     # 2022年
     r"(?P<Y>\d{4})\s*年",
     # 02月
     r"(?P<m>\d{1,2})\s*[月]",
 
+    r"(?P<bH>\d+)\s*hr\s*",
+    r"(?P<bH>\d+)\s*h\s*",
+    r"(?P<bd>\d+)\s*d\s*",
+    r"(?P<ba>\d+)\s*w\s*",
+    r"(?P<bm>\d+)\s*m\s*",
+    r"(?P<bY>\d+)\s*y\s*",
 
 ]
 
 OTHER_STRING_DATE_TIME_REGEX_LIST = {
     'EN': [
         # Thu February 02 02:02:02 2022
         r"(?P<m>\d{1,2})\s*[\-\|/\.月]?\s*(?P<d>\d{1,2})\s*[\-\|/\.日]?\s*(?P<H>\d{1,2})\s*[:时h]\s*(?P<M>\d{1,2})\s*[:分]\s*(?P<S>\d{1,2})\s*[秒]?\s*(?P<Y>\d{4})\s*[\-\|/\.年]?",
         # 04:28, 13 Feb 2023
         r"(?P<H>\d{1,2})[:](?P<M>\d{1,2})\s*[,]?\s*(?P<d>\d{1,2})\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})",
         # Mar 23 02:28:00 2023
         r"(?P<m>\d{1,2})\s*[月]\s*(?P<d>\d{1,2})\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})[:](?P<S>\d{1,2})\s*(?P<Y>\d{4})",
         # Feb 02, 2022 08:35 pm
-        r"(?P<m>\d{1,2})\s*[月]?\s*(?P<d>\d{1,2})\s*,\s*(?P<Y>\d{4})\s*[-]?\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})\s*(?P<ap>am|pm)",
+        r"(?P<m>\d{1,2})\s*[月]?\s*(?P<d>\d{1,2})\s*,\s*(?P<Y>\d{4})\s*[-]?\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})\s*(?P<apm>am|pm)",
         # Feb 02, 2022 08:35
         r"(?P<m>\d{1,2})\s*[月]?\s*(?P<d>\d{1,2})\s*,\s*(?P<Y>\d{4})\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})",
         # Feb 02, 2022
         r"(?P<m>\d{1,2})\s*[月]?\s*(?P<d>\d{1,2})\s*,\s*(?P<Y>\d{4})",
         # 10 25, 2021| Jan 01, 2000
-        r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})\s*[|]?\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})\s*(?P<ap>am|pm)",
+        r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})\s*[|]?\s*(?P<H>\d{1,2})[:](?P<M>\d{1,2})\s*(?P<apm>am|pm)",
         # Wed 29 Mar 2023 at 3:04pm
         r"(?P<d>\d{1,2})[\.]?\s*(?P<m>\d{1,2})\s*[月]\s*(?P<Y>\d{4})\s*(?P<H>\d{1,2})[:h](?P<M>\d{1,2})",
         # Wed 29 Mar 2023 at 3:04
 
         r"(?P<d>\d{1,2})\s*(?P<m>\d{1,2})\s*(?P<Y>\d{4})",  # 25 10 2021
         r"(?P<m>\d{1,2})\s*(?P<Y>\d{4})",  # 10 2021
         #
@@ -126,15 +134,15 @@
 
 
     ],
     'ZH_TW': [
         r"民国\s*(?P<mgY>\d+)[\-\|/\.年]\s*(?P<m>\d+)[\-\|/\.月]\s*(?P<d>\d+)[日]?",
         r"民国\s*(?P<mgY>\d+)[\-\|/\.年]\s*(?P<m>\d+)[\-\|/\.月]?",
         r"民国(?P<mgY>\d+)[年]?",
-
+        r"(?P<mgY>\d{3})\s*[\-\|/\.年]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<d>\d{1,2})\s*[日]?",
         r"(?P<bH>\d+)\s*时间前",
     ],
     'FRA': [
         # 31/03/23 à 12h03
         r"(?P<d>\d{1,2})\s*[\-\|/\.日]\s*(?P<m>\d{1,2})\s*[\-\|/\.月]\s*(?P<Y>\d{2,4})\s*[,]?\s*(?P<H>\d{1,2})\s*[:时h\.]\s*(?P<M>\d{1,2})\s*[:分]?",
 
         # before
@@ -155,24 +163,27 @@
     "IR": [
         r"(?P<bS>\d+)\s*секунда?\s*",
         r"(?P<bM>\d+)\s*минута?\s*",
         r"(?P<bH>\d+)\s*час?\s*",
     ],
     "MAR": [
         r"(?P<bM>\d+)\s*तासांपूर्वी",
+    ],
+    "VIE": [
+        "(?P<d>\d{1,2})\s*[\-\|/\.月]\s*(?P<m>\d{1,2})\s*[\-\|/\.年]\s*(?P<Y>\d{2,4})"  # 29 tháng 3 năm 2023
     ]
 }
 
 # 替换翻译
 SUB_TRANSLATE = {
     'EN': [
         (r"January|JANUARY|Jan\.|Jan", "1月"),
         (r"February|FEBRUARY|Feb\.", "2月"),
         (r"March|MARCH|Mar\.|Mar|Mai", "3月"),
-        (r"April|APRIL|Apr\.|Apr|Abr", "4月"),
+        (r"April|APRIL|Apr\.|Apr", "4月"),
         (r"May\.|May|MAY", "5月"),
         (r"June|JUNE|Jun\.|Jun", "6月"),
         (r"July|JULY|Jul\.|Jul", "7月"),
         (r"August|AUGUST|Aug\.|Aug", "8月"),
         (r"September|SEPTEMBER|Sept\.|Sept|Sep\.|Sep", "9月"),
         (r"October|OCTOBER|Oct\.|Oct", "10月"),
         (r"November|NOVEMBER|Nov\.|Nov", "11月"),
@@ -221,23 +232,26 @@
         (r'鐘', '钟'),
     ],
     'DE': [
         (r"Januar|Jan", "1月"),
         (r"Februar|Feb\.", "2月"),
         (r"März|Mär", "3月"),
         (r"April|Apr", "4月"),
+        (r"Abriil|Abr", "4月"),
         (r"Mai|mai", "5月"),
         (r"Juni|Jun", "6月"),
         (r"Juli|Jnl", "7月"),
         (r"August|Aug", "8月"),
         (r"September|Sep\.", "9月"),
         (r"Oktober|Okt", "10月"),
         (r"November|Nov", "11月"),
         (r"Dezember|Dez", "12月"),
         (r"Uhr", "am"),
+        (r"une heure", "1 heure"),
+        (r"il y a heure", "il y a 1 heure"),
     ],
     'FRA': [
         (r"janvier|jan\.", "1月"),
         (r"février|fev\.", "2月"),
         (r"mars\.|mars", "3月"),
         (r"avril|avr\.", "4月"),
         (r"mai\.|mai", "5月"),
@@ -246,20 +260,23 @@
         (r"aout\.|août", "8月"),
         (r"septembre|sept\.", "9月"),
         (r"octobre|oct\.", "10月"),
         (r"novembre|nov\.", "11月"),
         (r"décembre|dec\.", "12月"),
         (r"aujourd’hui à", ""),
         (r"à l’instant", "刚刚"),
+        (r"hier à", "昨天"),
         (r"à", ""),
     ],
     'VIE': [
         (r"phút", "分钟"),
         (r"trước", "前"),
         (r"giờ", "小时"),
+        (r"tháng", "月"),
+        (r"năm", "年"),
     ],
     'KAB': [
         (r"Fev", "2月"),
     ],
     'KOR': [
         (r"(de)?\s*enero\s*(de)?", "1月"),
         (r"(de)?\s*febrero\s*(de)?", "2月"),
@@ -274,23 +291,24 @@
         (r"(de)?\s*noviembre\s*(de)?", "11月"),
         (r"(de)?\s*diciembre\s*(de)?", "12月"),
     ],
     'IR': [
         (r"январь", "1月"),
         (r"февраль", "2月"),
         (r"март", "3月"),
-        (r"апрель", "4月"),
+        (r"апрель|апреля|апрел", "4月"),
         (r"май", "5月"),
         (r"июнь", "6月"),
         (r"июль", "7月"),
         (r"август", "8月"),
         (r"сентябрь", "9月"),
         (r"октябрь", "10月"),
         (r"ноябрь", "11月"),
         (r"декабрь", "12月"),
+        (r"сегодня  в|сегодня", "今天"),
     ],
     'SWE': [
         (r"janeiro", "1月"),
         (r"fevereiro", "2月"),
         (r"março", "3月"),
         (r"abril", "4月"),
         (r"maio", "5月"),
```

### Comparing `gggdtparser-0.0.5/gggdtparser/dtparser.py` & `gggdtparser-0.0.6/gggdtparser/dtparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,39 +96,36 @@
             if not match_obj:
                 continue
             group_dict = match_obj.groupdict()
             if group_dict:
                 try:
                     result = cls._parse_group_dict(
                         group_dict, accurately, max_datetime)
-                    print(regex)
+                    # print(regex)
                     return result
                 except Exception:
                     continue
 
     @classmethod
     def _parse_group_dict(cls, group_dict, accurately, max_datetime):
         un_accurately = not accurately
         now = datetime.datetime.now()
         timestamp = int(group_dict.get('ts') or 0)
         if timestamp:
             if len(str(timestamp)) == 13:
                 timestamp = int(timestamp) // 1000
             return datetime.datetime.fromtimestamp(timestamp)
-        year = group_dict.get('Y') or 0  # or now.year
+        year = group_dict.get('Y')  # or now.year
         if year and isinstance(year, str) and len(year) == 2:
             year = '20' + year
-        year = int(year)
-        # if year < 1970:
-        #     raise ValueError
-        month = int(group_dict.get('m') or 0)
-        day = int(group_dict.get('d') or 0)
-        hour = int(group_dict.get('H') or 0)
-        minute = int(group_dict.get('M') or 0)
-        second = int(group_dict.get('S') or 0)
+        month = group_dict.get('m')
+        day = group_dict.get('d')
+        hour = group_dict.get('H')
+        minute = group_dict.get('M')
+        second = group_dict.get('S')
         # 常见异常组合
         use_now_config = dict()
         use_now_config['year'] = use_now_config['month'] = False
         use_now_config['day'] = use_now_config['hour'] = False
         use_now_config['minute'] = use_now_config['second'] = False
         cls._update_use_now_config_by_has_parse(
             use_now_config, year, month, day, hour, minute, second)
@@ -247,18 +244,14 @@
                     second=un_accurately)
         if special_other:
             if special_other == '刚刚':
                 change_second += 5
                 cls._update_use_now_config(
                     use_now_config, year=True, month=True,
                     day=True, hour=True, minute=True, second=True)
-        # 上下午
-        ap = group_dict.get('ap')
-        if ap == 'pm':
-            hour += 12 if hour and hour < 12 else hour
         # 民国时间
         mg_year = group_dict.get('mgY')
         if mg_year:
             year = 1911 + int(mg_year)
             month = month if month else 1
         # 计算时间
         change_timedelta = datetime.timedelta(
@@ -274,14 +267,18 @@
             accurately, use_now_config['hour'], now.hour, hour)
         minute = cls._get_default_or_now(
             accurately, use_now_config['minute'], now.minute, minute)
         second = cls._get_default_or_now(
             accurately, use_now_config['second'], now.second, second)
         month = 1 if not month else month
         day = 1 if not day else day
+        # 上下午
+        apm = group_dict.get('apm')
+        if apm == 'pm':
+            hour += 12 if hour and hour < 12 else hour
         parse_datetime = datetime.datetime(
             year=year, month=month,
             day=day, hour=hour,
             minute=minute, second=second) - change_timedelta
         if max_datetime and parse_datetime > max_datetime:
             raise Exception('解析时间超出最大时间')
         return parse_datetime
@@ -296,16 +293,16 @@
         use_now_config['hour'] = hour
         use_now_config['minute'] = minute
         use_now_config['second'] = second
 
     @classmethod
     def _get_default_or_now(cls, accurately, use_now_enabled,
                             now_value, default_value):
-        return now_value if not default_value and (
-                use_now_enabled or not accurately) else default_value
+        return int((now_value if default_value is None and (
+                use_now_enabled or not accurately) else default_value) or 0)
 
     @classmethod
     def _update_use_now_config_by_has_parse(
             cls, use_now_config, year, month, day, hour, minute, second):
         parse_flag = '%s%s%s%s%s%s' % (
             int(bool(year)), int(bool(month)), int(bool(day)),
             int(bool(hour)), int(bool(minute)), int(bool(second))
```

### Comparing `gggdtparser-0.0.5/gggdtparser/test.py` & `gggdtparser-0.0.6/gggdtparser/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,21 @@
             if mode == 'accurately':
                 pass
             elif mode == 'un_accurately':
                 accurately = False
             else:
                 continue
             result = parse(string_datetime, accurately=accurately,
-                           max_datetime=datetime.datetime(year=2030,month=1,
+                           max_datetime=datetime.datetime(year=2030, month=1,
                                                           day=1))
             check_result = check(result, check_dt)
             if not check_result:
                 print('字符串时间：%s | 解析结果：%s | 严格模式：%s | 预期效果：%s | 验证结果：%s' % (
-                    string_datetime, result, accurately, check_dt, check_result))
+                    string_datetime, result, accurately, check_dt,
+                    check_result))
 
 
 now = datetime.datetime.now()
 HAS_TEST_STRING_DATETIME = {
     '1643738522': {
         'accurately': datetime.datetime(year=2022, month=2, day=2,
                                         hour=2, minute=2, second=2),
@@ -60,21 +61,21 @@
             year=2022, month=2, day=2,
             hour=2, minute=2),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2, second=now.second),
     },
     '2022年2月02日，上午02:02': {
-            'accurately': datetime.datetime(
-                year=2022, month=2, day=2, hour=2,
-                minute=2, second=0),
-            'un_accurately': datetime.datetime(
-                year=2022, month=2, day=2, hour=2,
-                minute=2, second=now.second)
-        },
+        'accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=2,
+            minute=2, second=0),
+        'un_accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=2,
+            minute=2, second=now.second)
+    },
     '2022-02-02 02:02': {
         'accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=2, minute=2, second=now.second),
@@ -354,16 +355,16 @@
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute, second=now.second) - datetime.timedelta(
             seconds=5),
     },
     '2年前': {
         'accurately': datetime.datetime(
             year=now.year - 2, month=1, day=1),
-        'un_accurately': (now-datetime.timedelta(days=365*3),
-                          now-datetime.timedelta(days=365*2)),
+        'un_accurately': (now - datetime.timedelta(days=365 * 3),
+                          now - datetime.timedelta(days=365 * 2)),
     },
     '2月前': {
         'accurately': datetime.datetime(
             year=now.year, month=now.month, day=now.day) -
                       datetime.timedelta(days=30 * 2),
         'un_accurately': (datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
@@ -448,16 +449,16 @@
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute, second=now.second) -
                           datetime.timedelta(seconds=2)),
     },
     '2年内': {
         'accurately': datetime.datetime(
             year=now.year - 2, month=1, day=1),
-        'un_accurately': (now-datetime.timedelta(days=365*2),
-                          now-datetime.timedelta(days=365*1)),
+        'un_accurately': (now - datetime.timedelta(days=365 * 2),
+                          now - datetime.timedelta(days=365 * 1)),
     },
     '2月内': {
         'accurately': datetime.datetime(
             year=now.year, month=now.month, day=now.day) -
                       datetime.timedelta(days=30 * 2),
         'un_accurately': (datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
@@ -548,14 +549,22 @@
         'accurately': datetime.datetime(
             year=2022, month=2, day=2, hour=0,
             minute=0, second=0),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2, hour=now.hour,
             minute=now.minute, second=now.second)
     },
+    '111-02-02': {
+        'accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=0,
+            minute=0, second=0),
+        'un_accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=now.hour,
+            minute=now.minute, second=now.second)
+    },
     '2小時前': {
         'accurately': datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour) -
                       datetime.timedelta(hours=2),
         'un_accurately': (datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute, second=now.second) -
@@ -659,16 +668,16 @@
         'un_accurately': datetime.datetime(year=now.year, month=2, day=2,
                                            hour=now.hour, minute=now.minute,
                                            second=now.second),
     },
     '2 years ago': {
         'accurately': datetime.datetime(
             year=now.year - 2, month=1, day=1),
-        'un_accurately': (now-datetime.timedelta(days=365*3),
-                          now-datetime.timedelta(days=365*2)),
+        'un_accurately': (now - datetime.timedelta(days=365 * 3),
+                          now - datetime.timedelta(days=365 * 2)),
     },
     '2 month ago': {
         'accurately': datetime.datetime(
             year=now.year, month=now.month, day=now.day) -
                       datetime.timedelta(days=30 * 2),
         'un_accurately': (datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
@@ -865,24 +874,36 @@
     '02. Februar 2022': {
         'accurately': datetime.datetime(
             year=2022, month=2, day=2, ),
         'un_accurately': datetime.datetime(
             year=2022, month=2, day=2,
             hour=now.hour, minute=now.minute, second=now.second),
     },
-    # 越南语
+
+}
+
+# 越南语
+HAS_TEST_STRING_DATETIME_VIE = {
     '2 phút trước': {
         'accurately': datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute) -
                       datetime.timedelta(minutes=2),
         'un_accurately': (datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute, second=now.second) -
                           datetime.timedelta(minutes=3), datetime.datetime(
             year=now.year, month=now.month, day=now.day, hour=now.hour,
             minute=now.minute, second=now.second) -
                           datetime.timedelta(minutes=2)),
     },
+    '02 tháng 2 năm 2022': {
+        'accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=0,
+            minute=0, second=0),
+        'un_accurately': datetime.datetime(
+            year=2022, month=2, day=2, hour=now.hour,
+            minute=now.minute, second=now.second)
+    },
 }
 if __name__ == '__main__':
     pass
```

### Comparing `gggdtparser-0.0.5/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.0.6/gggdtparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.5
+Version: 0.0.6
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.5/setup.cfg` & `gggdtparser-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

