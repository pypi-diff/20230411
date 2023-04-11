# Comparing `tmp/iLiaShahpy-3.8.5.tar.gz` & `tmp/iLiaShahpy-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iLiaShahpy-3.8.5.tar", last modified: Mon Mar 27 12:04:51 2023, max compression
+gzip compressed data, was "iLiaShahpy-3.8.6.tar", last modified: Tue Apr 11 07:47:18 2023, max compression
```

## Comparing `iLiaShahpy-3.8.5.tar` & `iLiaShahpy-3.8.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-27 12:04:51.015583 iLiaShahpy-3.8.5/
--rw-rw----   0 root         (0) everybody  (9997)     1084 2023-03-26 11:27:06.000000 iLiaShahpy-3.8.5/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     3038 2023-03-27 12:04:51.019583 iLiaShahpy-3.8.5/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-27 12:04:50.843583 iLiaShahpy-3.8.5/iLiaShahpy/
--rw-rw----   0 root         (0) everybody  (9997)      373 2023-02-12 11:47:26.000000 iLiaShahpy-3.8.5/iLiaShahpy/Clien.py
--rw-rw----   0 root         (0) everybody  (9997)     1733 2023-03-27 11:44:58.000000 iLiaShahpy-3.8.5/iLiaShahpy/Copyright.py
--rw-rw----   0 root         (0) everybody  (9997)      443 2023-02-12 18:39:14.000000 iLiaShahpy-3.8.5/iLiaShahpy/Device.py
--rw-rw----   0 root         (0) everybody  (9997)     1953 2023-02-12 18:39:23.000000 iLiaShahpy-3.8.5/iLiaShahpy/Encoder.py
--rw-rw----   0 root         (0) everybody  (9997)      155 2023-02-12 11:46:48.000000 iLiaShahpy-3.8.5/iLiaShahpy/Error.py
--rw-rw----   0 root         (0) everybody  (9997)     8700 2023-03-27 09:18:10.000000 iLiaShahpy-3.8.5/iLiaShahpy/Getheader.py
--rw-rw----   0 root         (0) everybody  (9997)     1124 2023-03-27 09:18:34.000000 iLiaShahpy-3.8.5/iLiaShahpy/GtM.py
--rw-rw----   0 root         (0) everybody  (9997)     2501 2023-03-27 09:22:12.000000 iLiaShahpy-3.8.5/iLiaShahpy/PostData.py
--rw-rw----   0 root         (0) everybody  (9997)      594 2023-02-12 18:39:48.000000 iLiaShahpy-3.8.5/iLiaShahpy/TypeText.py
--rw-rw----   0 root         (0) everybody  (9997)    10114 2023-03-27 09:23:30.000000 iLiaShahpy-3.8.5/iLiaShahpy/Zedcontent.py
--rw-rw----   0 root         (0) everybody  (9997)       29 2023-03-27 10:09:07.000000 iLiaShahpy-3.8.5/iLiaShahpy/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53662 2023-03-27 10:39:23.000000 iLiaShahpy-3.8.5/iLiaShahpy/iLia.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-03-27 12:04:50.999583 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     3038 2023-03-27 12:04:50.000000 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      457 2023-03-27 12:04:50.000000 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-03-27 12:04:50.000000 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       93 2023-03-27 12:04:50.000000 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-03-27 12:04:50.000000 iLiaShahpy-3.8.5/iLiaShahpy.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-03-27 12:04:51.031583 iLiaShahpy-3.8.5/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     3527 2023-03-27 11:45:23.000000 iLiaShahpy-3.8.5/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 07:47:18.762330 iLiaShahpy-3.8.6/
+-rw-rw----   0 root         (0) everybody  (9997)     1084 2023-03-26 11:27:06.000000 iLiaShahpy-3.8.6/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     3192 2023-04-11 07:47:18.762330 iLiaShahpy-3.8.6/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 07:47:18.566330 iLiaShahpy-3.8.6/iLiaShahpy/
+-rw-rw----   0 root         (0) everybody  (9997)      373 2023-04-07 18:50:09.000000 iLiaShahpy-3.8.6/iLiaShahpy/Clien.py
+-rw-rw----   0 root         (0) everybody  (9997)     1792 2023-04-08 11:41:35.000000 iLiaShahpy-3.8.6/iLiaShahpy/Copyright.py
+-rw-rw----   0 root         (0) everybody  (9997)      443 2023-02-12 18:39:14.000000 iLiaShahpy-3.8.6/iLiaShahpy/Device.py
+-rw-rw----   0 root         (0) everybody  (9997)     1953 2023-02-12 18:39:23.000000 iLiaShahpy-3.8.6/iLiaShahpy/Encoder.py
+-rw-rw----   0 root         (0) everybody  (9997)      155 2023-02-12 11:46:48.000000 iLiaShahpy-3.8.6/iLiaShahpy/Error.py
+-rw-rw----   0 root         (0) everybody  (9997)     8700 2023-03-27 09:18:10.000000 iLiaShahpy-3.8.6/iLiaShahpy/Getheader.py
+-rw-rw----   0 root         (0) everybody  (9997)     1124 2023-03-27 09:18:34.000000 iLiaShahpy-3.8.6/iLiaShahpy/GtM.py
+-rw-rw----   0 root         (0) everybody  (9997)     2501 2023-03-27 09:22:12.000000 iLiaShahpy-3.8.6/iLiaShahpy/PostData.py
+-rw-rw----   0 root         (0) everybody  (9997)      594 2023-04-08 11:18:49.000000 iLiaShahpy-3.8.6/iLiaShahpy/TrubText.py
+-rw-rw----   0 root         (0) everybody  (9997)    10112 2023-04-08 11:12:44.000000 iLiaShahpy-3.8.6/iLiaShahpy/ZedLink.py
+-rw-rw----   0 root         (0) everybody  (9997)       29 2023-03-27 10:09:07.000000 iLiaShahpy-3.8.6/iLiaShahpy/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53652 2023-04-08 11:28:22.000000 iLiaShahpy-3.8.6/iLiaShahpy/iLia.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 07:47:18.730330 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3192 2023-04-11 07:47:17.000000 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      454 2023-04-11 07:47:18.000000 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-11 07:47:17.000000 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       93 2023-04-11 07:47:17.000000 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-11 07:47:17.000000 iLiaShahpy-3.8.6/iLiaShahpy.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-11 07:47:18.770330 iLiaShahpy-3.8.6/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     3692 2023-04-08 11:52:45.000000 iLiaShahpy-3.8.6/setup.py
```

### Comparing `iLiaShahpy-3.8.5/LICENCE` & `iLiaShahpy-3.8.6/LICENCE`

 * *Files identical despite different names*

### Comparing `iLiaShahpy-3.8.5/PKG-INFO` & `iLiaShahpy-3.8.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iLiaShahpy
-Version: 3.8.5
+Version: 3.8.6
 Summary:  library Robot Rubika
 Home-page: 
 Author: iLiaShah
 Author-email: iLiaShahmanam@gmail.com
 License: MIT
-Keywords: iLia,iLiaShahpy,iLiashahpy,iLiaShohpy,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
+Keywords: iLiarub,iLiaShahpy,RoboRubika,iLiashahpy,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -27,70 +27,71 @@
 
 
 ## iLiaShahpy
 
 > Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
 
 <p align="center">
-    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="500">
+    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="580">
     <br>
-    <b>library iLiaShah</b>
+    <b>library iLiaShahpy</b>
     <br>
 </p>
 
-###  iLiaShah library documents soon...
+###  iLiaShahpy library documents soon...
 
 
 ### How to import the Rubik's library
 
 ``` bash
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
 Or
 
 from iLiaShahpy import RoboRubika
 ```
 
 ### How to import the anti-advertising class
 
 ``` bash
-from iLiaShahpy.Zedcontent import Antiadvertisement
+from iLiaShahpy.ZedLink import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install iLiaShahpy==3.8.3
+pip install iLiaShahpy==3.8.6
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Sourse_py
+@iLiaShahpy
 ```
 ## An example:
 ``` python
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
-bot = Messenger("Your Auth Account")
+bot = iLiarub("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 
 ## And Or:
 ``` python
 from iLiaShahpy import RoboRubika
 
 bot = RoboRubika("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 Made by iLiaShah
 
 
 
 ### Key Features
 
@@ -105,23 +106,33 @@
 ### Our channel in messengers
 
 ``` bash
 Our channel in Ita
 
 https://eitaa.com/Sourse_py
 
+https://eitaa.com/iLiaShahpy
+
 Our channel in Soroush Plus
 
 https://splus.ir/Sourse_py
 
+https://splus.ir/iLiaShahpy
+
 Our channel in Rubika
 
 https://rubika.ir/Sourse_py
 
-Our channel in the Gap
-
-https://gap.im/Sourse_py
+https://rubika.ir/iLiaShahpy
 
 Our channel on Telegram
 
 https://t.me/Sourse_py
+
+https://t.me/iLiaShahpy
+
+Our channel in Bale
+
+https://bale.ai/Sourse_py
+
+https://bale.ai/iLiaShahpy
 ```
```

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/Copyright.py` & `iLiaShahpy-3.8.6/iLiaShahpy/Copyright.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,21 @@
         	magenta = '\033[95m'
         	cyan = '\033[96m'
         	white = '\033[97m'
         	bold = '\033[1m'
         	underline = '\033[4m'
         	black='\033[30m'
         	ir = pytz.timezone("Asia/Tehran")
-        	time = f"{datetime.now(ir).strftime(f'{yellow}[{magenta}%H:%M:%S{yellow}]')}"
+        	time = f"{datetime.now(ir).strftime(f'{yellow}[{cyan}{bold}%H{magenta}{bold}:{cyan}{bold}%M{magenta}{bold}:{cyan}{bold}%S{yellow}]')}"
         	CopyRight = print(f"""{bold}
-{white} 〔༄〕- {cyan} 𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵𝗽𝘆 {magenta} 𝗩𝗲𝗿𝘀𝗶𝗼𝗻  {yellow}3.8.5    
+{white} 〔༄〕- {cyan} 𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵𝗽𝘆 {magenta} 𝗩𝗲𝗿𝘀𝗶𝗼𝗻  {yellow}3.8.6    
 
-{white} 〔༄〕- {cyan} 𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵𝗽𝘆 {magenta} 𝙲𝚘𝚙𝚢𝚁𝚒𝚐𝚑𝚝 (𝙲) {yellow} 2023 {red} 𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵   
+{white} 〔༄〕- {cyan} 𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵𝗽𝘆{magenta} 𝙲𝚘𝚙𝚢𝚁𝚒𝚐𝚑𝚝 (𝙲){yellow} 2023 {red}𝗶𝗟𝗶𝗮𝗦𝗵𝗮𝗵   
 
-{white} 〔༄〕- {cyan} 𝗥𝘂𝗯𝗶𝗸𝗮{magenta} 𝗖𝗵𝗮𝗻𝗲𝗹𝗹  {yellow} @𝚂𝚘𝚞𝚛𝚜𝚎_𝚙𝚢
+{white} 〔༄〕- {cyan} 𝗥𝘂𝗯𝗶𝗸𝗮{magenta} 𝗖𝗵𝗮𝗻𝗲𝗹𝗹 {yellow}@𝚒𝙻𝚒𝚊𝚂𝚑𝚊𝚑𝚙𝚢
 
 {white} 〔༄〕- {cyan} 𝗧𝗶𝗺𝗲 {magenta}{time}
 
 {white}⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁⌁
 """)
         	for x in range(3):
               	  for i in ("⢿", "⣻", "⣽", "⣾", "⣷", "⣯", "⣟", "⡿"):
```

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/Encoder.py` & `iLiaShahpy-3.8.6/iLiaShahpy/Encoder.py`

 * *Files identical despite different names*

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/Getheader.py` & `iLiaShahpy-3.8.6/iLiaShahpy/Getheader.py`

 * *Files identical despite different names*

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/GtM.py` & `iLiaShahpy-3.8.6/iLiaShahpy/GtM.py`

 * *Files identical despite different names*

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/PostData.py` & `iLiaShahpy-3.8.6/iLiaShahpy/PostData.py`

 * *Files identical despite different names*

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/TypeText.py` & `iLiaShahpy-3.8.6/iLiaShahpy/TrubText.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-def TypeText(Type:str = None,text:str = None,guid:str = None):
-	if Type == "MentionText":
+def TrubText(Trub:str = None,text:str = None,guid:str = None):
+	if Trub == "MentionText":
 		if guid and text != None:
 			return [{"type":"MentionText","mention_text_object_guid":guid,"from_index":0,"length":len(text),"mention_text_object_type":"User"}]
-	if Type == "Mono":
+	if Trub == "Mono":
 		if text != None:
 			return [{"from_index": 0, "length": len(text), "type": "Mono"}]
-	elif Type == "Bold":
+	elif Trub == "Bold":
 		if text != None:
 			return [{"from_index": 0, "length": len(text), "type": "Bold"}]
-	elif Type == "Italic":
+	elif Trub == "Italic":
 		if text != None:
 			return [{"from_index": 0, "length": len(text), "type": "Italic"}]
```

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/Zedcontent.py` & `iLiaShahpy-3.8.6/iLiaShahpy/ZedLink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from iLiaShahpy.iLia import Messenger
+from iLiaShahpy.iLia import iLiarub
 from re import findall
 from iLiaShahpy.Error import AuthError,TypeAnti
 from iLiaShahpy.Copyright import copyright
 from iLiaShahpy.PostData import method_Rubika
 
 
 class Antiadvertisement:
```

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy/iLia.py` & `iLiaShahpy-3.8.6/iLiaShahpy/iLia.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-from iLiaShahpy.Copyright import copyright
+from iLiaShahpy.Copyright import copyright
```

### Comparing `iLiaShahpy-3.8.5/iLiaShahpy.egg-info/PKG-INFO` & `iLiaShahpy-3.8.6/iLiaShahpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iLiaShahpy
-Version: 3.8.5
+Version: 3.8.6
 Summary:  library Robot Rubika
 Home-page: 
 Author: iLiaShah
 Author-email: iLiaShahmanam@gmail.com
 License: MIT
-Keywords: iLia,iLiaShahpy,iLiashahpy,iLiaShohpy,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
+Keywords: iLiarub,iLiaShahpy,RoboRubika,iLiashahpy,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
@@ -27,70 +27,71 @@
 
 
 ## iLiaShahpy
 
 > Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
 
 <p align="center">
-    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="500">
+    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="580">
     <br>
-    <b>library iLiaShah</b>
+    <b>library iLiaShahpy</b>
     <br>
 </p>
 
-###  iLiaShah library documents soon...
+###  iLiaShahpy library documents soon...
 
 
 ### How to import the Rubik's library
 
 ``` bash
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
 Or
 
 from iLiaShahpy import RoboRubika
 ```
 
 ### How to import the anti-advertising class
 
 ``` bash
-from iLiaShahpy.Zedcontent import Antiadvertisement
+from iLiaShahpy.ZedLink import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install iLiaShahpy==3.8.3
+pip install iLiaShahpy==3.8.6
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Sourse_py
+@iLiaShahpy
 ```
 ## An example:
 ``` python
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
-bot = Messenger("Your Auth Account")
+bot = iLiarub("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 
 ## And Or:
 ``` python
 from iLiaShahpy import RoboRubika
 
 bot = RoboRubika("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 Made by iLiaShah
 
 
 
 ### Key Features
 
@@ -105,23 +106,33 @@
 ### Our channel in messengers
 
 ``` bash
 Our channel in Ita
 
 https://eitaa.com/Sourse_py
 
+https://eitaa.com/iLiaShahpy
+
 Our channel in Soroush Plus
 
 https://splus.ir/Sourse_py
 
+https://splus.ir/iLiaShahpy
+
 Our channel in Rubika
 
 https://rubika.ir/Sourse_py
 
-Our channel in the Gap
-
-https://gap.im/Sourse_py
+https://rubika.ir/iLiaShahpy
 
 Our channel on Telegram
 
 https://t.me/Sourse_py
+
+https://t.me/iLiaShahpy
+
+Our channel in Bale
+
+https://bale.ai/Sourse_py
+
+https://bale.ai/iLiaShahpy
 ```
```

### Comparing `iLiaShahpy-3.8.5/setup.py` & `iLiaShahpy-3.8.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,70 +7,71 @@
 _long_description = """
 
 ## iLiaShahpy
 
 > Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
 
 <p align="center">
-    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="500">
+    <img src="https://s2.uupload.ir/files/img_20230325_150407_843_hcgc_thumb.jpg" alt="iLiaShah" width="580">
     <br>
-    <b>library iLiaShah</b>
+    <b>library iLiaShahpy</b>
     <br>
 </p>
 
-###  iLiaShah library documents soon...
+###  iLiaShahpy library documents soon...
 
 
 ### How to import the Rubik's library
 
 ``` bash
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
 Or
 
 from iLiaShahpy import RoboRubika
 ```
 
 ### How to import the anti-advertising class
 
 ``` bash
-from iLiaShahpy.Zedcontent import Antiadvertisement
+from iLiaShahpy.ZedLink import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install iLiaShahpy==3.8.3
+pip install iLiaShahpy==3.8.6
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Sourse_py
+@iLiaShahpy
 ```
 ## An example:
 ``` python
-from iLiaShahpy import Messenger
+from iLiaShahpy import iLiarub
 
-bot = Messenger("Your Auth Account")
+bot = iLiarub("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 
 ## And Or:
 ``` python
 from iLiaShahpy import RoboRubika
 
 bot = RoboRubika("Your Auth Account")
 
 gap = "your guid or gap or pv or channel"
 
-bot.sendMessage(gap,"libraryiLiaShah")
+bot.sendMessage(gap,"libraryiLiaShahpy")
 ```
 Made by iLiaShah
 
 
 
 ### Key Features
 
@@ -85,40 +86,50 @@
 ### Our channel in messengers
 
 ``` bash
 Our channel in Ita
 
 https://eitaa.com/Sourse_py
 
+https://eitaa.com/iLiaShahpy
+
 Our channel in Soroush Plus
 
 https://splus.ir/Sourse_py
 
+https://splus.ir/iLiaShahpy
+
 Our channel in Rubika
 
 https://rubika.ir/Sourse_py
 
-Our channel in the Gap
-
-https://gap.im/Sourse_py
+https://rubika.ir/iLiaShahpy
 
 Our channel on Telegram
 
 https://t.me/Sourse_py
+
+https://t.me/iLiaShahpy
+
+Our channel in Bale
+
+https://bale.ai/Sourse_py
+
+https://bale.ai/iLiaShahpy
 ```
 """
 
 setup(
     name = "iLiaShahpy",
-    version = "3.8.5",
+    version = "3.8.6",
     author = "iLiaShah",
     author_email = "iLiaShahmanam@gmail.com",
     description = (" library Robot Rubika"),
     license = "MIT",
-    keywords = ["iLia","iLiaShahpy","iLiashahpy","iLiaShohpy","bot","Bot","BOT","Robot","ROBOT","robot","self","api","API","Api","rubika","Rubika","RUBIKA","Python","python","aiohttp","asyncio"],
+    keywords = ["iLiarub","iLiaShahpy","RoboRubika","iLiashahpy","bot","Bot","BOT","Robot","ROBOT","robot","self","api","API","Api","rubika","Rubika","RUBIKA","Python","python","aiohttp","asyncio"],
     url = "",
     packages = ['iLiaShahpy'],
     long_description=_long_description,
     long_description_content_type = 'text/markdown',
     install_requires=requires,
     classifiers=[
     'Development Status :: 3 - Alpha',
```
