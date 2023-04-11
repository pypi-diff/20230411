# Comparing `tmp/wbtest_utils-0.0.1.tar.gz` & `tmp/wbtest_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wbtest_utils-0.0.1.tar", last modified: Mon Apr 10 08:22:10 2023, max compression
+gzip compressed data, was "dist/wbtest_utils-0.0.2.tar", last modified: Tue Apr 11 03:27:42 2023, max compression
```

## Comparing `wbtest_utils-0.0.1.tar` & `wbtest_utils-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.700899 wbtest_utils-0.0.1/
--rw-r--r--   0 zhihui18   (501) staff       (20)       99 2023-04-10 03:31:16.000000 wbtest_utils-0.0.1/MANIFEST.in
--rw-r--r--   0 zhihui18   (501) staff       (20)      273 2023-04-10 08:22:10.698050 wbtest_utils-0.0.1/PKG-INFO
--rw-r--r--   0 zhihui18   (501) staff       (20)     1853 2023-04-06 09:00:27.000000 wbtest_utils-0.0.1/README.md
--rw-r--r--   0 zhihui18   (501) staff       (20)       38 2023-04-10 08:22:10.701068 wbtest_utils-0.0.1/setup.cfg
--rw-r--r--   0 zhihui18   (501) staff       (20)      708 2023-04-10 03:31:27.000000 wbtest_utils-0.0.1/setup.py
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.613650 wbtest_utils-0.0.1/src/
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.623806 wbtest_utils-0.0.1/src/wbtest_utils/
--rw-r--r--   0 zhihui18   (501) staff       (20)       68 2023-04-10 02:59:48.000000 wbtest_utils-0.0.1/src/wbtest_utils/__init__.py
--rw-r--r--   0 zhihui18   (501) staff       (20)    13898 2023-04-10 06:27:06.000000 wbtest_utils-0.0.1/src/wbtest_utils/android_utils.py
--rw-r--r--   0 zhihui18   (501) staff       (20)     3075 2023-04-10 06:25:02.000000 wbtest_utils-0.0.1/src/wbtest_utils/common_utils.py
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.648232 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/
--rwxr-xr-x   0 zhihui18   (501) staff       (20)      161 2023-03-31 07:14:16.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/abl.strings
--rwxr-xr-x   0 zhihui18   (501) staff       (20)      153 2023-04-10 06:25:28.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/awl.strings
--rw-r--r--   0 zhihui18   (501) staff       (20)    85664 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/fastbot-thirdpart.jar
--rwxr-xr-x   0 zhihui18   (501) staff       (20)  1149240 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/framework.jar
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.616501 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.650081 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/arm64-v8a/
--rwxr-xr-x   0 zhihui18   (501) staff       (20)  1996056 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/arm64-v8a/libfastbot_native.so
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.659173 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/armeabi-v7a/
--rwxr-xr-x   0 zhihui18   (501) staff       (20)  1592144 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/armeabi-v7a/libfastbot_native.so
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.670410 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86/
--rwxr-xr-x   0 zhihui18   (501) staff       (20)  2037928 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86/libfastbot_native.so
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.679360 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86_64/
--rwxr-xr-x   0 zhihui18   (501) staff       (20)  2114816 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86_64/libfastbot_native.so
--rwxr-xr-x   0 zhihui18   (501) staff       (20)       56 2023-03-31 06:47:48.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/max.config
--rwxr-xr-x   0 zhihui18   (501) staff       (20)       43 2023-04-10 06:25:18.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/max.schema
--rwxr-xr-x   0 zhihui18   (501) staff       (20)      418 2023-04-10 02:59:48.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/max.widget.black
--rwxr-xr-x   0 zhihui18   (501) staff       (20)      583 2023-03-31 08:24:03.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/max.xpath.actions
--rw-r--r--   0 zhihui18   (501) staff       (20)    77245 2023-03-22 11:44:46.000000 wbtest_utils-0.0.1/src/wbtest_utils/fastbot/monkeyq.jar
--rw-r--r--   0 zhihui18   (501) staff       (20)    12999 2023-04-10 02:59:48.000000 wbtest_utils-0.0.1/src/wbtest_utils/ios_utils.py
-drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-10 08:22:10.626818 wbtest_utils-0.0.1/src/wbtest_utils.egg-info/
--rw-r--r--   0 zhihui18   (501) staff       (20)      273 2023-04-10 08:22:10.000000 wbtest_utils-0.0.1/src/wbtest_utils.egg-info/PKG-INFO
--rw-r--r--   0 zhihui18   (501) staff       (20)      907 2023-04-10 08:22:10.000000 wbtest_utils-0.0.1/src/wbtest_utils.egg-info/SOURCES.txt
--rw-r--r--   0 zhihui18   (501) staff       (20)        1 2023-04-10 08:22:10.000000 wbtest_utils-0.0.1/src/wbtest_utils.egg-info/dependency_links.txt
--rw-r--r--   0 zhihui18   (501) staff       (20)       13 2023-04-10 08:22:10.000000 wbtest_utils-0.0.1/src/wbtest_utils.egg-info/top_level.txt
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.288713 wbtest_utils-0.0.2/
+-rw-r--r--   0 zhihui18   (501) staff       (20)       99 2023-04-10 03:31:16.000000 wbtest_utils-0.0.2/MANIFEST.in
+-rw-r--r--   0 zhihui18   (501) staff       (20)      273 2023-04-11 03:27:42.288415 wbtest_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 zhihui18   (501) staff       (20)     1853 2023-04-06 09:00:27.000000 wbtest_utils-0.0.2/README.md
+-rw-r--r--   0 zhihui18   (501) staff       (20)       38 2023-04-11 03:27:42.288801 wbtest_utils-0.0.2/setup.cfg
+-rw-r--r--   0 zhihui18   (501) staff       (20)      708 2023-04-11 03:27:36.000000 wbtest_utils-0.0.2/setup.py
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.222301 wbtest_utils-0.0.2/src/
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.226798 wbtest_utils-0.0.2/src/wbtest_utils/
+-rw-r--r--   0 zhihui18   (501) staff       (20)       68 2023-04-10 02:59:48.000000 wbtest_utils-0.0.2/src/wbtest_utils/__init__.py
+-rw-r--r--   0 zhihui18   (501) staff       (20)    14258 2023-04-11 03:21:52.000000 wbtest_utils-0.0.2/src/wbtest_utils/android_utils.py
+-rw-r--r--   0 zhihui18   (501) staff       (20)     5726 2023-04-11 03:24:58.000000 wbtest_utils-0.0.2/src/wbtest_utils/common_utils.py
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.245122 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)      161 2023-03-31 07:14:16.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/abl.strings
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)      153 2023-04-10 06:25:28.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/awl.strings
+-rw-r--r--   0 zhihui18   (501) staff       (20)    85664 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/fastbot-thirdpart.jar
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)  1149240 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/framework.jar
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.223075 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.246805 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/arm64-v8a/
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)  1996056 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/arm64-v8a/libfastbot_native.so
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.256240 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/armeabi-v7a/
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)  1592144 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/armeabi-v7a/libfastbot_native.so
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.266512 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86/
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)  2037928 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86/libfastbot_native.so
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.279270 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86_64/
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)  2114816 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86_64/libfastbot_native.so
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)       56 2023-03-31 06:47:48.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/max.config
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)       43 2023-04-10 06:25:18.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/max.schema
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)      418 2023-04-10 02:59:48.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/max.widget.black
+-rwxr-xr-x   0 zhihui18   (501) staff       (20)      583 2023-03-31 08:24:03.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/max.xpath.actions
+-rw-r--r--   0 zhihui18   (501) staff       (20)    77245 2023-03-22 11:44:46.000000 wbtest_utils-0.0.2/src/wbtest_utils/fastbot/monkeyq.jar
+-rw-r--r--   0 zhihui18   (501) staff       (20)    14125 2023-04-11 03:06:18.000000 wbtest_utils-0.0.2/src/wbtest_utils/ios_utils.py
+drwxr-xr-x   0 zhihui18   (501) staff       (20)        0 2023-04-11 03:27:42.228940 wbtest_utils-0.0.2/src/wbtest_utils.egg-info/
+-rw-r--r--   0 zhihui18   (501) staff       (20)      273 2023-04-11 03:27:42.000000 wbtest_utils-0.0.2/src/wbtest_utils.egg-info/PKG-INFO
+-rw-r--r--   0 zhihui18   (501) staff       (20)      907 2023-04-11 03:27:42.000000 wbtest_utils-0.0.2/src/wbtest_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 zhihui18   (501) staff       (20)        1 2023-04-11 03:27:42.000000 wbtest_utils-0.0.2/src/wbtest_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 zhihui18   (501) staff       (20)       13 2023-04-11 03:27:42.000000 wbtest_utils-0.0.2/src/wbtest_utils.egg-info/top_level.txt
```

### Comparing `wbtest_utils-0.0.1/README.md` & `wbtest_utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/setup.py` & `wbtest_utils-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 解压压缩包，python setup.py install  安装自己的包，就可以引用了
 
 
 from setuptools import find_packages
 from distutils.core import setup
 
 setup(name='wbtest_utils',  # 包名
-      version='0.0.1',  # 版本号
+      version='0.0.2',  # 版本号
       description='微博自动化测试工具',
       long_description='',
       author='zhihui18',
       author_email='zhihui18@staff.weibo.com',
       url='https://gitlab.weibo.cn/andarchitecture/Android_AutoTest',
       license='',
       install_requires=[],
```

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/android_utils.py` & `wbtest_utils-0.0.2/src/wbtest_utils/android_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,31 @@
         return True
 
     except Exception as e:
         print(e)
         return False
 
 
+def clean_mock_dir():
+    f"""
+    删除手机上{mock_path}下的文件
+    :return: 
+    """
+    if isinstance(G.DEVICE, Android):
+        android = Android()
+    else:
+        return False
+    try:
+        android.adb.shell(f"rm -rf {mock_path}")
+        return True
+    except Exception as e:
+        print(e)
+        return False
+
+
 def clean_wlog_dir():
     f"""
     清空 {pc_wlog_capture_path} 目录, 以及手机上存储的wlog日志文件
     :return: 
     """
     if isinstance(G.DEVICE, Android):
         android = Android()
@@ -348,15 +365,16 @@
             android.adb.push(f"{PROJECT_DIR}/fastbot/max.schema", "/sdcard")
         else:
             print("appid cannot be null")
             return False
         sleep(10)
         android.adb.shell(f"ls {fastbot_adb_path}")
         # 设置fastbot白名单文件
-        origin_list = ["com.sina.weibo.SplashActivity\n", "com.sina.weibo.NewProjectModeActivity\n", "com.sina.weibo.wboxsdk.page.acts.WBXPageActivity\n"]
+        origin_list = ["com.sina.weibo.SplashActivity\n", "com.sina.weibo.NewProjectModeActivity\n",
+                       "com.sina.weibo.wboxsdk.page.acts.WBXPageActivity\n"]
         f_w = open(f"{PROJECT_DIR}/fastbot/awl.strings", "w")
         f_w.writelines(origin_list)
         f_w.close()
         if len(activity_list) > 0:
             f = open(f"{PROJECT_DIR}/fastbot/awl.strings", "a")
             f.writelines(activity_list)
             f.close()
@@ -386,15 +404,14 @@
         # android.adb.pull("/storage/emulated/0/crash-dump.log", PROJECT_DIR)
         # android.adb.pull("/storage/emulated/0/oom-traces.log", PROJECT_DIR)
         return True
     except Exception as e:
         print(e)
         return False
 
-
 # json_test = get_customer_file_last("actlog_14980")
 
 # print(json_test)
 
 # request_body = get_json_dic_from_string(json_test.get("requestBody"))
 
 # print(request_body['extJson'])
```

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/fastbot-thirdpart.jar` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/fastbot-thirdpart.jar`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/framework.jar` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/framework.jar`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/arm64-v8a/libfastbot_native.so` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/arm64-v8a/libfastbot_native.so`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/armeabi-v7a/libfastbot_native.so` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/armeabi-v7a/libfastbot_native.so`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86/libfastbot_native.so` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86/libfastbot_native.so`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/libs/x86_64/libfastbot_native.so` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/libs/x86_64/libfastbot_native.so`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/max.xpath.actions` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/max.xpath.actions`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/fastbot/monkeyq.jar` & `wbtest_utils-0.0.2/src/wbtest_utils/fastbot/monkeyq.jar`

 * *Files identical despite different names*

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils/ios_utils.py` & `wbtest_utils-0.0.2/src/wbtest_utils/ios_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,60 +2,61 @@
 import shutil
 import subprocess
 
 from airtest.core.api import *
 from airtest.core.helper import *
 from airtest.core.ios.ios import *
 
-auto_setup(__file__)
+AUTOTEST_MOCK_AB_DIR = "Autotest/Mock/AB/"
+AUTOTEST_MOCK_DATA_DIR = "Autotest/Mock/Data/"
+AUTOTEST_MOCK_LOG_DIR = "Autotest/Logs/"
 
 
 class apputils(object):
     def __init__(self, udid: str = None, bundle_id: str = None, parent_dir=os.environ["HOME"]):
         """初始化
         
         Keyword arguments:
-        udid -- 设备的udid，此处是用的是 airtest 的 udid 格式为 http://ip 或者 http+usbmux://udid，
-        如果是前者默认使用usb连接的第一个设备，如果是后者解析 udid
+        udid -- 设备的udid, 此处是用的是 airtest 的 udid 格式为 http://ip 或者 http+usbmux://udid, 
+        如果是前者默认使用usb连接的第一个设备, 如果是后者解析 udid
         
-        bundle_id -- 应用的唯一标识，如果没有，从环境变量取，再没有默认为 com.sina.weibo.inhouse
+        bundle_id -- 应用的唯一标识, 如果没有, 从环境变量取, 再没有默认为 com.sina.weibo.inhouse
         
         parent_dir -- abspath for parent_dir
         """
-        # 
         o = urlparse(udid)
         if o.scheme == "http+usbmux":
-            parse_udid = o.hostname
+            # hostname 会改变大小写，所以用netloc代替
+            parse_udid = o.netloc
         else:
             parse_udid = self.__first_connect_usb_device_udid()
             log("使用第一个usb链接的udid", desc="[ios_utils] udid 解析")
 
         if not parse_udid:
-            raise ValueError("invalid udid value")
+            raise ValueError("invalid udid value %s" % parse_udid)
         if not bundle_id:
             try:
                 bundle_id = os.environ["bundle_id"]
             except KeyError as e:
                 bundle_id = "com.sina.weibo.inhouse"
                 log(e, desc="[ios_utils] bundle_id 解析")
 
         self.__client = wda.USBClient(udid=parse_udid)
+        self.__udid = parse_udid
         self.__logData = {}
         self.__bundle_id = bundle_id
         self.__is_mounted_documents = False
         self.__is_mounted_container = False
-        self.__auto_test_mock_dir = "Autotest/Mock/"
-        self.__auto_test_log_dir = "Autotest/Logs/"
 
         # mount point path
         self.__root_dir = os.path.expanduser(parent_dir)
 
         # /mount_parent_dir/uuid_bundleId_documents
-        self.__mount_documents_path = os.path.join(self.__root_dir, udid + bundle_id + "documents")
-        self.__mount_container_path = os.path.join(self.__root_dir, udid + bundle_id + "container")
+        self.__mount_documents_path = os.path.join(self.__root_dir, self.__udid + self.__bundle_id + "documents")
+        self.__mount_container_path = os.path.join(self.__root_dir, self.__udid + self.__bundle_id + "container")
 
     # def mounted_dir(self, documents=True):
     #     if documents and self.__is_mounted_documents:
     #         return self.__mount_documents_path
     #     elif not documents and self.__is_mounted_container:
     #         return self.__mount_container_path
     #     else:
@@ -65,35 +66,41 @@
     # def exist_mount_point(self, mount_point) -> bool:
     #     p1 = subprocess.Popen('mount', stdout=subprocess.PIPE)
     #     p2 = subprocess.Popen(['grep', mount_point], stdin=p1.stdout, stdout=subprocess.PIPE)
     #     p1.stdout.close()
     #     p2.communicate()
 
     #     return True if p2.returncode == 0 else False
+    @property
+    def log_dict(self) -> dict:
+        return self.__logData
 
     def mount_documents(self) -> bool:
         return self.__mount()
 
     def mount_container(self) -> bool:
         return self.__mount(False)
 
     def __mount(self, documents=True) -> bool:
 
         mounted = self.__is_mounted_documents if documents else self.__is_mounted_container
         if mounted:
             return
 
         mount_dir = self.__mount_documents_path if documents else self.__mount_container_path
-        mound_arg = '--documents' if documents else '--container'
-
         result = True
         if not os.path.ismount(mount_dir):
-            self.__creat_empty_dir_force(mount_dir)
-            code = subprocess.call(['ifuse', mount_dir, '-u', self.__uuid, mound_arg, self.__bundle_id])
-            result = code == 0
+            try:
+                self.__creat_empty_dir_force(mount_dir)
+                mound_arg = '--documents' if documents else '--container'
+                code = subprocess.call(['ifuse', mount_dir, '-u', self.__udid, mound_arg, self.__bundle_id])
+                result = code == 0
+            except Exception as e:
+                result = False
+                log(e, timestamp=time.time(), desc="挂载 app documents 目录失败")
 
         if documents:
             self.__is_mounted_documents = result
         else:
             self.__is_mounted_container = result
         return result
 
@@ -127,38 +134,50 @@
         for line in lines[1:]:
             sl = line.rstrip("\n")
             o = re.split(r"  +", sl, 5)
             if o[-1] == "usb":
                 return o[0]
         return None
 
-    def __push_file_to_device(self, local_file, parent_dir, file_name=None) -> bool:
+    def __push_file_to_device(self, local_paths, parent_dir, file_name=None) -> bool:
         """Copy local file to App documents
         
         Keyword arguments:
-        local_file -- local file path, abspath
+        local_paths -- local file path/dir, abspath
         parent_dir -- the parent directory in documents, not include mount point prefix 
         file_name -- under the parent_dir
         """
-        print("__push_file_to_device")
-        s = os.path.expanduser(local_file)
+        if len(local_paths) == 0:
+            return False
+
+        if len(local_paths) > 1 and file_name:
+            log("移动文件超过1个, file_name 将被弃用", desc="移动本地文件到app 沙盒 documents")
+            file_name = None
+
+        expand_paths = []
+        for path in local_paths:
+            s = os.path.expanduser(path)
+            expand_paths.append(s)
 
-        if not os.path.exists(s):
-            raise FileNotFoundError(f"{local_file} does not exist")
         if not self.__is_mounted_documents:
             self.__mount()
         if parent_dir.startswith("/"):
             parent_dir = parent_dir[1:]
         dest = os.path.join(self.__mount_documents_path, parent_dir)
         if not os.path.exists(dest):
             os.makedirs(dest)
         if file_name:
             dest = os.path.join(dest, file_name)
 
-        r = subprocess.call('cp' + ' -Rf ' + s + ' ' + dest, shell=True)
+        cmd = "cp -rf"
+        for arg in expand_paths:
+            cmd += f" {arg}"
+        cmd += f" {dest}"
+
+        r = subprocess.call(cmd, shell=True)
         return r == 0
 
     # def __pull_file_from_device(self, dest: str = "", app_documents_file: str = "") -> bool:
     #     """Copy App file in documents to local
 
     #     Keyword arguments:
     #     dest -- description
@@ -185,32 +204,32 @@
         arguments = {"bundleId": self.__bundle_id, "value": data}
 
         if method.upper == "POST":
             return self.__client.http.post(path, arguments)
         elif method.upper == "GET":
             return self.__client.http.get(path, arguments)
         else:
-            print("__app_send_request unsurport")
+            log("Unsurport requeset method: %s" % method)
             return None
 
     def __app_mock_data_json_file(self, data: dict = {}):
         """Mock app request with k/v pairs 
         
         Keyword arguments:
         data -- dict, { "path" : "filename"}
 
         """
         return self.__app_send_request('/wda/app/mock/data/file', "POST", data)
 
     # Public
-    def push_preset_mock_ab_to_device(self, src: str):
-        print("push_preset_mock_file_to_device")
-        # /Documents/Autotest/Mock/AB/config.json
-        parent_dir = os.path.join(self.__auto_test_mock_dir, "AB")
-        self.__push_file_to_device(src, parent_dir, "config.json")
+    def push_preset_mock_ab_file_to_device(self, src: str):
+        # /APP_Documents/Autotest/Mock/AB/config.json
+        if not os.path.exists(src):
+            raise FileExistsError("%s does not exist" % src)
+        self.__push_file_to_device(src, AUTOTEST_MOCK_AB_DIR, "config.json")
 
     # Public
     def mock_ab(self, data: dict = {}):
         """Mock app abtest with k/v pairs {feature_name:value}
         
         Keyword arguments:
         data -- dict, {feature_name1:val , feature_name2: value}
@@ -223,148 +242,148 @@
         
         Keyword arguments:
         data -- dict, {key:val , key: value}
         """
         return self.__app_send_request('/wda/app/unmock/ab', "POST", data)
 
     # Public
-    def push_preset_mock_file_to_device(self, src):
-        print("push_preset_mock_file_to_device")
+    def push_preset_mock_data_file_to_device(self, src: str):
+        if not os.path.exists(src):
+            raise FileExistsError("File does not exist: %s " % src)
         # /Autotest/Mock/Data/config.json
-        parent_dir = os.path.join(self.__auto_test_mock_dir, "Data")
-        self.__push_file_to_device(src, parent_dir, "config.json")
+        self.__push_file_to_device([src], AUTOTEST_MOCK_DATA_DIR, "config.json")
 
     # Public 
-    def push_mock_file_to_device(self, src):
-        print("push file to device")
+    def push_mock_file_to_device(self, paths: list = [str]):
         # /Autotest/Mock/Data/
-        parent_dir = os.path.join(self.__auto_test_mock_dir, "Data")
-        self.__push_file_to_device(src, parent_dir)
+        self.__push_file_to_device(paths, AUTOTEST_MOCK_DATA_DIR)
 
     # Public
     def push_mock_interface(self, url_path: str = None, file_path: str = None):
         """Mock app request with url path、local file abspath end with .json
 
         url_path -- request url path
 
         file_path -- local json file path, must end with .json
         """
 
         if not url_path or not file_path:
             raise ValueError("push_mock_interface arguments not None")
 
-        print("push_mock_interface")
-
         # cp local file to /Autotest/Mock/Data/
-        self.__push_file_to_device(file_path, "Autotest/Mock/Data/")
+        self.__push_file_to_device([file_path], "Autotest/Mock/Data/")
 
         # set mock map
         file_name = os.path.basename(file_path)
         self.__app_mock_data_json_file({url_path: file_name})
 
     # Public
     def clean_mock_interface(self, data: dict = {}):
-        """Unmock app request with k/v pairs 
+        """取消数据mock, 如果为空, 会clean 所有 mock, 并且删除 mock 文件 
         
         Keyword arguments:
         data -- dict, {"path1":"file_name.json" , "path2": "file_name.json"} 
         path eg: /2/xxx/aaa
 
         """
-        print("clean_mock_interface")
         self.__app_mock_data_json_file(data)
 
-        # def app_mock_data_json_data(self, data):
-
-    #     """Mock app abtest with json responce
-
-    #     Keyword arguments:
-    #     data -- dict, {key:val , key: value}
-
-    #     """
-    #     return self.__app_send_request('/wda/app/mock/data/json', "POST", data)
-
-    # def app_ummock_data(self, data):
-    #     """Unmock url paths, k/v pairs , Remove all if data is empty
-
-    #     Keyword arguments:
-    #     data -- dict, {key:val , key: value}
-
-    #     """
-    #     return self.__app_send_request('/wda/app/unmock/data', "POST", data)
-
-    # Public
-    # def pull_log_file_from_device(self):
-    #     print("pull_log_file_from_device")
-    #     #App: /Documents/Autotest/Logs/
-    #     # locol dir:
-
-    #     local_dir = os.environ["HOME"] + 
-    #     self.__pull_file_from_device("Autotest/Logs/")
-
-    #     r = subprocess.call('cp' + ' -Rf ' + s + ' ' + dest, shell=True)
-    #     return r == 0
-
-    # Public
-    def get_last_log_file_content(self, act_code: str = ""):
-        print("get_last_log_file_content")
-        # 
-        if len(self.__logData) > 0:
-            return {}
-
-        if not self.__is_mounted_documents:
-            self.__mount()
+        # Public
 
-        log_dir = os.path.join(self.__mount_documents_path, self.__auto_test_log_dir)
+    def pull_log_file_from_device(self):
+        """读取日志文件到当前类的 logdata
+        {
+            action1:{
+                subtype1:[
+                    {},
+                    {}
+                ],
+                subtype2:[
+                    {},
+                    {}
+                ]
+            }
+            ... 依次类推
+        }
+        """
+        self.__mount()
+        log_dir = os.path.join(self.__mount_documents_path, AUTOTEST_MOCK_LOG_DIR)
         if not os.path.exists(log_dir):
             return None
 
         subfiles = os.listdir(log_dir)
         log_file = os.path.join(log_dir, subfiles[-1])
 
         # Parse log file
-        with open(log_file, mode="r", encoding='utf-8') as f:
-            # format:    timestamp:xx|action:xx|subtype:xx|content:xxx\n
-            for line in f:
-                real_line = line[:-1]
-                if len(real_line) == 0:
-                    continue
-                args = real_line.split('|')
-                if len(args) != 4:
-                    continue
-                timestamp = args[0].split(':')[1]
-                action = args[1].split(':')[1]
-                subtype = args[2].split(':')[1]
-                content = args[3][len("content:"):]
-                log = {"ts": timestamp, "value": json.loads(content)}
-                if action in self.__logData:
-                    subtypes = self.__logData[action]
-                    if subtype in subtypes:
-                        subtypes[subtype].append(log)
+        try:
+            with open(log_file, mode="r", encoding='utf-8') as f:
+                # format:    timestamp:xx|action:xx|subtype:xx|content:xxx\n
+                for line in f:
+                    real_line = line[:-1]
+                    if len(real_line) == 0:
+                        continue
+                    args = real_line.split('|')
+                    if len(args) != 4:
+                        continue
+                    timestamp = args[0].split(':')[1]
+                    action = args[1].split(':')[1]
+                    subtype = args[2].split(':')[1]
+                    content = args[3][len("content:"):]
+                    log_content = {"ts": timestamp, "value": json.loads(content)}
+                    if action in self.__logData:
+                        subtypes = self.__logData[action]
+                        if subtype in subtypes:
+                            subtypes[subtype].append(log_content)
+                        else:
+                            subtypes[subtype] = [log_content]
                     else:
-                        subtypes[subtype] = [log]
-                else:
-                    subtype_obj = {subtype: [log]}
-                    self.__logData[action] = subtype_obj
+                        subtype_obj = {subtype: [log_content]}
+                        self.__logData[action] = subtype_obj
+        except Exception as e:
+            log(e, timestamp=time.time(), desc="日志文件读取失败")
+
+        return len(self.__logData) > 0
+
+    # Public
+    def get_last_log_file_content(self, act: str, act_code: str = ""):
+        if len(self.__logData) == 0:
+            return {}
+        if not act or not act_code:
+            return {}
+        try:
+            act_code_log_list = self.__logData[act][act_code]
+            return act_code_log_list[-1]
+        except Exception as e:
+            log(e, timestamp=time.time(), desc=f"获取指定类型的日志失败act:{act} act_code:{act_code}")
+            return {}
 
     # Public
     def clean_log_file(self):
-        print("clean log file")
+        self.__mount()
+        log_dir = os.path.join(self.__mount_documents_path, AUTOTEST_MOCK_LOG_DIR)
+        if os.path.exists(log_dir):
+            shutil.rmtree(log_dir)
+        self.__logData = {}
+        return True
 
     # Public
-    def clean_all(self):
-        """ !!!! Will Remove all in directory Autotest, eg: preset data、ab、log、mock ab、mock data
+    def clean_all(self, mock_data: bool = True, mock_ab: bool = True):
+        """ !!!! Will Remove all in directory Autotest, eg: preset data、preset ab、log、mock ab、mock data
         
         """
-        print("clean all")
-
         if not self.__is_mounted_documents:
             self.__mount()
 
-        autotest_dir = os.path.join(self.__mount_documents_path, "Autotest")
-        subprocess.call("rm" + " -rf " + autotest_dir)
         self.unmock_ab()
         self.clean_mock_interface()
+        # 删除 Autotest 目录
+        autotest_dir = os.path.join(self.__mount_documents_path, "Autotest")
+        subprocess.call("rm" + " -rf " + autotest_dir)
+
         self.unmount()
 
-    def start_app(self):
-        self.__client.app_start(self.__bundle_id)
+    def wb_start_app(self, bundle_id, arguments=[], environment={}, wait_for_quiescence=False, force=False):
+        if force:
+            stop_app(bundle_id)
+        self.__client.app_start(bundle_id, arguments=arguments, environment=environment,
+                                wait_for_quiescence=wait_for_quiescence)
+        start_app(bundle_id)
```

### Comparing `wbtest_utils-0.0.1/src/wbtest_utils.egg-info/SOURCES.txt` & `wbtest_utils-0.0.2/src/wbtest_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

