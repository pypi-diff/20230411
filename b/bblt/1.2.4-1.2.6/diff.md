# Comparing `tmp/bblt-1.2.4.tar.gz` & `tmp/bblt-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblt-1.2.4.tar", last modified: Mon Mar 27 08:56:50 2023, max compression
+gzip compressed data, was "bblt-1.2.6.tar", last modified: Tue Apr 11 08:42:33 2023, max compression
```

## Comparing `bblt-1.2.4.tar` & `bblt-1.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-03-27 08:56:50.082139 bblt-1.2.4/
--rw-r--r--   0 miaog001   (504) staff       (20)      224 2023-03-27 08:56:50.081484 bblt-1.2.4/PKG-INFO
-drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-03-27 08:56:50.075358 bblt-1.2.4/bblt/
--rw-r--r--   0 miaog001   (504) staff       (20)       35 2022-08-29 06:31:46.000000 bblt-1.2.4/bblt/__init__.py
--rw-r--r--   0 miaog001   (504) staff       (20)    12873 2023-03-27 08:42:49.000000 bblt-1.2.4/bblt/launchtime.py
--rw-r--r--   0 miaog001   (504) staff       (20)     6341 2022-08-31 08:14:19.000000 bblt-1.2.4/bblt/line.py
-drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-03-27 08:56:50.080766 bblt-1.2.4/bblt.egg-info/
--rw-r--r--   0 miaog001   (504) staff       (20)      224 2023-03-27 08:56:50.000000 bblt-1.2.4/bblt.egg-info/PKG-INFO
--rw-r--r--   0 miaog001   (504) staff       (20)      196 2023-03-27 08:56:50.000000 bblt-1.2.4/bblt.egg-info/SOURCES.txt
--rw-r--r--   0 miaog001   (504) staff       (20)        1 2023-03-27 08:56:50.000000 bblt-1.2.4/bblt.egg-info/dependency_links.txt
--rw-r--r--   0 miaog001   (504) staff       (20)      138 2023-03-27 08:56:50.000000 bblt-1.2.4/bblt.egg-info/requires.txt
--rw-r--r--   0 miaog001   (504) staff       (20)        5 2023-03-27 08:56:50.000000 bblt-1.2.4/bblt.egg-info/top_level.txt
--rw-r--r--   0 miaog001   (504) staff       (20)       38 2023-03-27 08:56:50.082394 bblt-1.2.4/setup.cfg
--rw-r--r--   0 miaog001   (504) staff       (20)      777 2023-03-27 08:56:17.000000 bblt-1.2.4/setup.py
+drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-04-11 08:42:33.921469 bblt-1.2.6/
+-rw-r--r--   0 miaog001   (504) staff       (20)      224 2023-04-11 08:42:33.921062 bblt-1.2.6/PKG-INFO
+drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-04-11 08:42:33.916628 bblt-1.2.6/bblt/
+-rw-r--r--   0 miaog001   (504) staff       (20)       35 2022-08-29 06:31:46.000000 bblt-1.2.6/bblt/__init__.py
+-rw-r--r--   0 miaog001   (504) staff       (20)    14586 2023-04-11 08:40:07.000000 bblt-1.2.6/bblt/launchtime.py
+-rw-r--r--   0 miaog001   (504) staff       (20)     6341 2022-08-31 08:14:19.000000 bblt-1.2.6/bblt/line.py
+drwxr-xr-x   0 miaog001   (504) staff       (20)        0 2023-04-11 08:42:33.920220 bblt-1.2.6/bblt.egg-info/
+-rw-r--r--   0 miaog001   (504) staff       (20)      224 2023-04-11 08:42:33.000000 bblt-1.2.6/bblt.egg-info/PKG-INFO
+-rw-r--r--   0 miaog001   (504) staff       (20)      196 2023-04-11 08:42:33.000000 bblt-1.2.6/bblt.egg-info/SOURCES.txt
+-rw-r--r--   0 miaog001   (504) staff       (20)        1 2023-04-11 08:42:33.000000 bblt-1.2.6/bblt.egg-info/dependency_links.txt
+-rw-r--r--   0 miaog001   (504) staff       (20)      138 2023-04-11 08:42:33.000000 bblt-1.2.6/bblt.egg-info/requires.txt
+-rw-r--r--   0 miaog001   (504) staff       (20)        5 2023-04-11 08:42:33.000000 bblt-1.2.6/bblt.egg-info/top_level.txt
+-rw-r--r--   0 miaog001   (504) staff       (20)       38 2023-04-11 08:42:33.921656 bblt-1.2.6/setup.cfg
+-rw-r--r--   0 miaog001   (504) staff       (20)      777 2023-04-11 08:07:17.000000 bblt-1.2.6/setup.py
```

### Comparing `bblt-1.2.4/bblt/launchtime.py` & `bblt-1.2.6/bblt/launchtime.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,45 @@
 import wda
 import time
 import uiautomator2 as u2
 import datetime
 import subprocess
 import argparse
 import pyautogui
+import shutil
 file_dir = str(__file__).replace(str(__file__).split("/")[-1], "")
 
 
 class launchtest:
 
-    def __init__(self):
-        pass
+    # def __init__(self):
+    #     pass
 
-    def __init__(self, package, video_screen=1, run_times=10, ios="http://localhost:8100"):
-        print("12345")
+    def __init__(self, package="",
+                 video_screen=1,
+                 run_times=10,
+                 device_name="",
+                 size="",
+                 different_allow=15,
+                 ios="http://localhost:8100"):
+        print("Init parameters....")
         self.screen = video_screen
         self.times = run_times
         self.ios_host = ios
         self.package_name = package
+        self.device_name = device_name
+        self.size = size
+        self.different_allow = different_allow
+
+    # def __init__(self, package="", video_screen=1, run_times=10, ios="http://localhost:8100"):
+    #     print("12345")
+    #     self.screen = video_screen
+    #     self.times = run_times
+    #     self.ios_host = ios
+    #     self.package_name = package
 
     def start_video(self, video_path):
         global process
         command_linux = f"ffmpeg -f avfoundation  -video_device_index {self.screen} -i ':' {video_path}"
         print(command_linux)
         process = subprocess.Popen(command_linux, shell=True)
 
@@ -49,32 +66,36 @@
 
     def convert_video_to_screenshot(self, video_file, dir):
         screenshot_path = dir + "/%04d.jpg"
         command = "ffmpeg -i " + video_file + "  -vf fps=5 " + screenshot_path
         process_temp = subprocess.Popen(command, shell=True)
         process_temp.communicate()
 
-    def cut_video(self, device_name, size, different_allow):
+    def cut_video(self, device_name):
         video_path = file_dir + "/recorded_videos/" + device_name + "/video/"
         screen_path = file_dir + "/recorded_videos/" + device_name + "/screenshot/"
         video_list = []
+        try:
+            os.rmdir(video_path)
+        except:
+            pass
         print("Video Path: " + video_path)
         for (dirpath, dirnames, filenames) in walk(video_path):
             video_list.extend(filenames)
             break
         try:
             video_list.remove(".DS_Store")
         except:
             pass
         for video in video_list:
             self.mk_folder(screen_path + video.replace(".mkv", ""))
             self.mk_folder(screen_path + video.replace(".mkv", "") + "/converted/")
             self.convert_video_to_screenshot(video_path + video, screen_path + video.replace(".mkv", ""))
-            self.crop_image(screen_path + video.replace(".mkv", ""), size)
-        self.show(device_name=device_name, different_allow=different_allow)
+            self.crop_image(screen_path + video.replace(".mkv", ""), self.size)
+        self.show(device_name=device_name, different_allow=self.different_allow)
 
     def crop_image(self, dir, size):
         f = []
         for (dirpath, dirnames, filenames) in walk(dir):
             f.extend(filenames)
             break
         for file in f:
@@ -137,19 +158,21 @@
             total_time += launch_time
 
         for diff in differences:
             for i in range(0, len(differences[diff])):
                 xarray.append(0.2 * i)
             break
         df = pd.DataFrame(data, index=xarray)
+        df.cumsum()
         df.plot()
         plt.title("App Launch time in " + device_name + ": " + str(round(total_time/len(differences), 2)))
         plt.xlabel("App bblt image actions change")
         plt.ylabel("Launch time")
-        plt.show()
+        file_location = file_dir + "/recorded_videos/"+device_name + '.png'
+        plt.savefig(file_location)
         plt.close()
 
     def mend_list(self, li):
         len_list = []
         for item in li:
             len_list.append(len(li[item]))
         max_len = max(len_list)
@@ -159,14 +182,22 @@
         return li
 
     def android_launch_test(self):
         d = u2.connect()
         device_name = d.info['productName']
         print(device_name)
         file_dir = str(__file__).replace(str(__file__).split("/")[-1], "")
+        try:
+            shutil.rmtree(path=file_dir + f"/recorded_videos/{device_name}/video")
+        except:
+            pass
+        try:
+            shutil.rmtree(path=file_dir + f"/recorded_videos/{device_name}/screenshot")
+        except:
+            pass
         self.mk_folder(dir=file_dir + f"/recorded_videos/{device_name}/video")
         self.mk_folder(dir=file_dir + f"/recorded_videos/{device_name}/screenshot")
         print(f'\n\n=======Android Device {device_name} Launch Time Test Started ========\n')
         for x in range(0, self.times):
             start_time = str(datetime.datetime.now()).replace(" ", "_")
             video_path = file_dir + f"/recorded_videos/{device_name}/video/video_{start_time}.mkv"
             d.app_stop_all()
@@ -181,14 +212,22 @@
         print('\n\n=======Android Launch Time Test Stopped ========\n')
         return device_name
 
     def ios_launch_test(self):
         c = wda.Client(self.ios_host)
         device_name = c.info['name'].replace(" ", "")
         file_dir = str(__file__).replace(str(__file__).split("/")[-1], "")
+        try:
+            shutil.rmtree(path=file_dir + f"/recorded_videos/{device_name}/video")
+        except:
+            pass
+        try:
+            shutil.rmtree(path=file_dir + f"/recorded_videos/{device_name}/screenshot")
+        except:
+            pass
         self.mk_folder(file_dir + f"/recorded_videos/{device_name}/video")
         self.mk_folder(file_dir + f"/recorded_videos/{device_name}/screenshot")
         element = c(label=u"餐饮")
         # element = c(label=u"Park Info & Entry")
         print(c.info)
         print(f'\n\n======= IOS Device {device_name} Launch Time Test Started =======\n')
         for x in range(0, self.times):
@@ -205,20 +244,20 @@
             #     element.click()
             time.sleep(5)
             self.pause_video_recording()
             c.close()
         print('\n\n======= IOS Launch Time Test Stopped ========\n')
         return device_name
 
-    def launch_curve(self, device, cut_size="", different_allow=10):
-        if "ios" in device:
+    def launch_curve(self):
+        if "ios" in self.device_name:
             device_name = self.ios_launch_test()
         else:
             device_name = self.android_launch_test()
-        self.cut_video(device_name, cut_size, different_allow)
+        self.cut_video(device_name)
 
     def test_location(self, size):
         pyautogui.screenshot('t.png')
         # point = pyautogui.position()
         # print(point)
         # size = f"{point.x}x{point.y}+780+30"
         convert_str = f"convert 't.png' -crop {size} 'tt.png'"
@@ -257,18 +296,27 @@
 
 
 if __name__ == '__main__':
     # launchtest("").test_location("380x780+1450+150")
     # launchtest("").test_location("750x1600+2700+380")
     # launchtest("").show("sdk_gphone_x86", 10)
     # launchtest("com.disney.shanghaidisneyland_goo", video_screen=3, run_times=1).help()
-    launchtest("com.disney.shanghaidisneyland_goo", video_screen=3, run_times=1).launch_curve("android", "384x792+20+100", different_allow=15)
-    # launchtest("com.disney.shanghaidisneyland.dev", video_screen=3, run_times=10).cut_video("iPhone", "450x950+20+80", 15)
-    # launchtest("com.disney.shanghaidisneyland.dev", video_screen=3, run_times=10).launch_curve("ios", "450x950+20+80", different_allow=15)
+    # launchtest("com.disney.shanghaidisneyland_goo", video_screen=3, run_times=10).launch_curve("android", "384x792+20+100", different_allow=15)
+    # launchtest("com.disney.shanghaidisneyland_goo", video_screen=3, run_times=10).cut_video("oppo",  "384x792+20+100", different_allow=15)
+    # launchtest("com.disney.shanghaidisneyland", video_screen=3, run_times=1).launch_curve("ios", "450x950+20+80", different_allow=15)
+    launchtest(package="com.disney.shanghaidisneyland",
+               device_name="ios",
+               video_screen=3,
+               run_times=1,
+               size="450x950+20+80",
+               different_allow=10).launch_curve()
+    # launchtest("com.disney.shanghaidisneyland", video_screen=3, run_times=10).cut_video("iPhone", "450x950+20+80", different_allow=15)
+
     # launchtest("com.disney.shanghaidisneyland_goo", video_screen=3, run_times=10).launch_curve("android", "393x829+20+80", different_allow=15)
+    # launchtest("com.disney.shanghaidisneyland.dev", video_screen=3, run_times=10).cut_video("iPhone", "450x950+20+80", 15)
     # parser = argparse.ArgumentParser()
     # parser.add_argument("-os", "--operation_system", default=1, type=int,
     #                     help="Device OS Type, Only Support [1]: IOS & [2]: Android."
     #                          "[0]: Display available screens",
     #                     choices=[0, 1, 2])
     # parser.add_argument("-p", "--package_name", help="APP Package ID")
     #
```

### Comparing `bblt-1.2.4/bblt/line.py` & `bblt-1.2.6/bblt/line.py`

 * *Files identical despite different names*

### Comparing `bblt-1.2.4/setup.py` & `bblt-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: bb(bobby.miao)
 # Description: APP Launch Test
 
 from setuptools import setup, find_packages
 
 setup(
     name='bblt',
-    version='1.2.4',
+    version='1.2.6',
     keywords='launchtest',
     description='APP Launch Test',
     license='MIT License',
     url='https://github.com/xiaoyaoamiao/lt.git',
     author='bob',
     author_email='miao2005du@163.com',
     packages=find_packages(),
```

