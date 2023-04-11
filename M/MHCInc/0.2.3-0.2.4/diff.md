# Comparing `tmp/MHCInc-0.2.3.tar.gz` & `tmp/MHCInc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MHCInc-0.2.3.tar", last modified: Sat Dec 24 11:28:38 2022, max compression
+gzip compressed data, was "MHCInc-0.2.4.tar", last modified: Tue Apr 11 21:59:27 2023, max compression
```

## Comparing `MHCInc-0.2.3.tar` & `MHCInc-0.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2022-12-24 11:28:38.852975 MHCInc-0.2.3/
--rw-r--r--   0 mhcteam    (501) staff       (20)     1073 2022-07-24 07:55:00.000000 MHCInc-0.2.3/LICENSE.txt
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2022-12-24 11:28:38.848407 MHCInc-0.2.3/MHCInc/
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2022-12-24 11:28:38.852028 MHCInc-0.2.3/MHCInc/MHCInc/
--rw-r--r--   0 mhcteam    (501) staff       (20)     5891 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/GuessGame.py
--rw-r--r--   0 mhcteam    (501) staff       (20)    15461 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/GuessGameEasy.py
--rw-r--r--   0 mhcteam    (501) staff       (20)    11622 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/GuessGameSecondary.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/MITLicense.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3734 2022-11-26 10:54:40.000000 MHCInc-0.2.3/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      808 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/Python3学习示例.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4084 2022-11-26 10:31:10.000000 MHCInc-0.2.3/MHCInc/MHCInc/__init__.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1028 2022-09-24 03:12:38.000000 MHCInc-0.2.3/MHCInc/MHCInc/animal_guess.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4058 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/caterpillar.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     2891 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/caterpillar2.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1148 2022-11-13 00:34:45.000000 MHCInc-0.2.3/MHCInc/MHCInc/copyright.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3274 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/egg_catcher.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3578 2022-11-26 10:54:22.000000 MHCInc-0.2.3/MHCInc/MHCInc/egg_catcher_perfect.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1936 2022-11-26 10:54:32.000000 MHCInc-0.2.3/MHCInc/MHCInc/matchmaker.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     2917 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/random.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      846 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/rectangle.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-11-12 23:06:17.000000 MHCInc-0.2.3/MHCInc/MHCInc/robot_builder.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4608 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/screen_pet.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4285 2022-12-24 11:27:44.000000 MHCInc-0.2.3/MHCInc/MHCInc/swift.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     1570 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/加密消息.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     4373 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/单词九连猜.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      413 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/圆筒万花筒.py
--rw-r--r--   0 mhcteam    (501) staff       (20)     3245 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/快照抓拍.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      805 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/星光夜空.py
--rw-r--r--   0 mhcteam    (501) staff       (20)      576 2022-07-24 07:55:00.000000 MHCInc-0.2.3/MHCInc/MHCInc/螺旋万花筒.py
-drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2022-12-24 11:28:38.852610 MHCInc-0.2.3/MHCInc/MHCInc.egg-info/
--rw-r--r--   0 mhcteam    (501) staff       (20)     2825 2022-12-24 11:28:38.000000 MHCInc-0.2.3/MHCInc/MHCInc.egg-info/PKG-INFO
--rw-r--r--   0 mhcteam    (501) staff       (20)      954 2022-12-24 11:28:38.000000 MHCInc-0.2.3/MHCInc/MHCInc.egg-info/SOURCES.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)        1 2022-12-24 11:28:38.000000 MHCInc-0.2.3/MHCInc/MHCInc.egg-info/dependency_links.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)        7 2022-12-24 11:28:38.000000 MHCInc-0.2.3/MHCInc/MHCInc.egg-info/top_level.txt
--rw-r--r--   0 mhcteam    (501) staff       (20)     2825 2022-12-24 11:28:38.852832 MHCInc-0.2.3/PKG-INFO
--rw-r--r--   0 mhcteam    (501) staff       (20)     2310 2022-11-26 10:34:41.000000 MHCInc-0.2.3/README.rst
--rw-r--r--   0 mhcteam    (501) staff       (20)       87 2022-11-13 01:29:47.000000 MHCInc-0.2.3/pyproject.toml
--rw-r--r--   0 mhcteam    (501) staff       (20)       38 2022-12-24 11:28:38.853016 MHCInc-0.2.3/setup.cfg
--rw-r--r--   0 mhcteam    (501) staff       (20)      819 2022-12-24 11:28:07.000000 MHCInc-0.2.3/setup.py
+drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.770766 MHCInc-0.2.4/
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1073 2022-07-24 07:55:00.000000 MHCInc-0.2.4/LICENSE.txt
+drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.766049 MHCInc-0.2.4/MHCInc/
+drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.769962 MHCInc-0.2.4/MHCInc/MHCInc/
+-rw-r--r--   0 mhcteam    (501) staff       (20)     5891 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGame.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)    15461 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGameEasy.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)    11622 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/GuessGameSecondary.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/MITLicense.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     3734 2022-11-26 10:54:40.000000 MHCInc-0.2.4/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)      808 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/Python3学习示例.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     6222 2023-04-11 21:56:32.000000 MHCInc-0.2.4/MHCInc/MHCInc/__init__.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1028 2022-09-24 03:12:38.000000 MHCInc-0.2.4/MHCInc/MHCInc/animal_guess.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     4058 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/caterpillar.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     2891 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/caterpillar2.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1148 2022-11-13 00:34:45.000000 MHCInc-0.2.4/MHCInc/MHCInc/copyright.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     3274 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     3578 2022-11-26 10:54:22.000000 MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher_perfect.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1936 2022-11-26 10:54:32.000000 MHCInc-0.2.4/MHCInc/MHCInc/matchmaker.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     2917 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/random.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)      846 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/rectangle.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1211 2022-11-12 23:06:17.000000 MHCInc-0.2.4/MHCInc/MHCInc/robot_builder.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     4608 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/screen_pet.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     4285 2022-12-24 11:27:44.000000 MHCInc-0.2.4/MHCInc/MHCInc/swift.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     1570 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/加密消息.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     4373 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/单词九连猜.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)      413 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/圆筒万花筒.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)     3245 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/快照抓拍.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)      805 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/星光夜空.py
+-rw-r--r--   0 mhcteam    (501) staff       (20)      576 2022-07-24 07:55:00.000000 MHCInc-0.2.4/MHCInc/MHCInc/螺旋万花筒.py
+drwxr-xr-x   0 mhcteam    (501) staff       (20)        0 2023-04-11 21:59:27.770457 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/
+-rw-r--r--   0 mhcteam    (501) staff       (20)     2864 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/PKG-INFO
+-rw-r--r--   0 mhcteam    (501) staff       (20)      954 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/SOURCES.txt
+-rw-r--r--   0 mhcteam    (501) staff       (20)        1 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/dependency_links.txt
+-rw-r--r--   0 mhcteam    (501) staff       (20)        7 2023-04-11 21:59:27.000000 MHCInc-0.2.4/MHCInc/MHCInc.egg-info/top_level.txt
+-rw-r--r--   0 mhcteam    (501) staff       (20)     2864 2023-04-11 21:59:27.770633 MHCInc-0.2.4/PKG-INFO
+-rw-r--r--   0 mhcteam    (501) staff       (20)     2310 2022-11-26 10:34:41.000000 MHCInc-0.2.4/README.rst
+-rw-r--r--   0 mhcteam    (501) staff       (20)       87 2022-11-13 01:29:47.000000 MHCInc-0.2.4/pyproject.toml
+-rw-r--r--   0 mhcteam    (501) staff       (20)       38 2023-04-11 21:59:27.770805 MHCInc-0.2.4/setup.cfg
+-rw-r--r--   0 mhcteam    (501) staff       (20)      858 2023-04-11 21:59:21.000000 MHCInc-0.2.4/setup.py
```

### Comparing `MHCInc-0.2.3/LICENSE.txt` & `MHCInc-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/GuessGame.py` & `MHCInc-0.2.4/MHCInc/MHCInc/GuessGame.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/GuessGameEasy.py` & `MHCInc-0.2.4/MHCInc/MHCInc/GuessGameEasy.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/GuessGameSecondary.py` & `MHCInc-0.2.4/MHCInc/MHCInc/GuessGameSecondary.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/MITLicense.py` & `MHCInc-0.2.4/MHCInc/MHCInc/MITLicense.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py` & `MHCInc-0.2.4/MHCInc/MHCInc/PHYSICAL_CONDITION_APPLET.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/Python3学习示例.py` & `MHCInc-0.2.4/MHCInc/MHCInc/Python3学习示例.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/animal_guess.py` & `MHCInc-0.2.4/MHCInc/MHCInc/animal_guess.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/caterpillar.py` & `MHCInc-0.2.4/MHCInc/MHCInc/caterpillar.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/caterpillar2.py` & `MHCInc-0.2.4/MHCInc/MHCInc/caterpillar2.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/copyright.py` & `MHCInc-0.2.4/MHCInc/MHCInc/copyright.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/egg_catcher.py` & `MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/egg_catcher_perfect.py` & `MHCInc-0.2.4/MHCInc/MHCInc/egg_catcher_perfect.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/matchmaker.py` & `MHCInc-0.2.4/MHCInc/MHCInc/matchmaker.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/random.py` & `MHCInc-0.2.4/MHCInc/MHCInc/random.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/rectangle.py` & `MHCInc-0.2.4/MHCInc/MHCInc/rectangle.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/robot_builder.py` & `MHCInc-0.2.4/MHCInc/MHCInc/robot_builder.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/screen_pet.py` & `MHCInc-0.2.4/MHCInc/MHCInc/screen_pet.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/swift.py` & `MHCInc-0.2.4/MHCInc/MHCInc/swift.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/加密消息.py` & `MHCInc-0.2.4/MHCInc/MHCInc/加密消息.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/单词九连猜.py` & `MHCInc-0.2.4/MHCInc/MHCInc/单词九连猜.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/快照抓拍.py` & `MHCInc-0.2.4/MHCInc/MHCInc/快照抓拍.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/星光夜空.py` & `MHCInc-0.2.4/MHCInc/MHCInc/星光夜空.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc/螺旋万花筒.py` & `MHCInc-0.2.4/MHCInc/MHCInc/螺旋万花筒.py`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc.egg-info/PKG-INFO` & `MHCInc-0.2.4/MHCInc/MHCInc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MHCInc
-Version: 0.2.3
-Summary: 改进漏洞：将使用模块功能时找不到文件优化
+Version: 0.2.4
+Summary: 改进漏洞：重复模块引用时无法配置删除的环境，使用MHCInc.module.setup()即可
 Home-page: https://pypi.org/project/MHCInc/
 Author: Mhc-inc
 Author-email: Wf6350177@163.com
 Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MHCInc-0.2.3/MHCInc/MHCInc.egg-info/SOURCES.txt` & `MHCInc-0.2.4/MHCInc/MHCInc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MHCInc-0.2.3/PKG-INFO` & `MHCInc-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MHCInc
-Version: 0.2.3
-Summary: 改进漏洞：将使用模块功能时找不到文件优化
+Version: 0.2.4
+Summary: 改进漏洞：重复模块引用时无法配置删除的环境，使用MHCInc.module.setup()即可
 Home-page: https://pypi.org/project/MHCInc/
 Author: Mhc-inc
 Author-email: Wf6350177@163.com
 Project-URL: Bug Tracker, https://github.com/Mhc-inc/MHCInc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MHCInc-0.2.3/README.rst` & `MHCInc-0.2.4/README.rst`

 * *Files identical despite different names*

