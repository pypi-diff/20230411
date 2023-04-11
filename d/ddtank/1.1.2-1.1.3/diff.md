# Comparing `tmp/ddtank-1.1.2.tar.gz` & `tmp/ddtank-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddtank-1.1.2.tar", last modified: Mon Mar  6 01:55:44 2023, max compression
+gzip compressed data, was "ddtank-1.1.3.tar", last modified: Tue Apr 11 06:43:06 2023, max compression
```

## Comparing `ddtank-1.1.2.tar` & `ddtank-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 01:55:44.149917 ddtank-1.1.2/
--rw-rw-rw-   0        0        0     1091 2022-12-26 11:39:15.000000 ddtank-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     9457 2023-03-06 01:55:44.149241 ddtank-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9065 2023-03-06 01:32:13.000000 ddtank-1.1.2/README.md
--rw-rw-rw-   0        0        0      592 2023-03-06 01:55:37.000000 ddtank-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-06 01:55:44.150075 ddtank-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-06 01:55:44.120204 ddtank-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-06 01:55:44.134452 ddtank-1.1.2/src/ddtank/
--rw-rw-rw-   0        0        0      145 2023-03-06 01:38:34.000000 ddtank-1.1.2/src/ddtank/__init__.py
--rw-rw-rw-   0        0        0     4634 2023-03-06 01:17:45.000000 ddtank-1.1.2/src/ddtank/ddtanker.py
--rw-rw-rw-   0        0        0    17232 2023-03-06 01:12:51.000000 ddtank-1.1.2/src/ddtank/status.py
-drwxrwxrwx   0        0        0        0 2023-03-06 01:55:44.148047 ddtank-1.1.2/src/ddtank/utils/
--rw-rw-rw-   0        0        0        0 2023-03-05 13:16:40.000000 ddtank-1.1.2/src/ddtank/utils/__init__.py
--rw-rw-rw-   0        0        0     2119 2023-03-06 01:17:05.000000 ddtank-1.1.2/src/ddtank/utils/get_capture.py
--rw-rw-rw-   0        0        0     1493 2023-03-01 01:11:37.000000 ddtank-1.1.2/src/ddtank/utils/get_game.py
--rw-rw-rw-   0        0        0      716 2023-03-06 01:12:51.000000 ddtank-1.1.2/src/ddtank/utils/get_map.py
--rw-rw-rw-   0        0        0     1775 2023-03-06 01:55:01.000000 ddtank-1.1.2/src/ddtank/utils/get_script.py
--rw-rw-rw-   0        0        0      793 2023-03-02 00:31:25.000000 ddtank-1.1.2/src/ddtank/utils/stop_thread.py
-drwxrwxrwx   0        0        0        0 2023-03-06 01:55:44.140067 ddtank-1.1.2/src/ddtank.egg-info/
--rw-rw-rw-   0        0        0     9457 2023-03-06 01:55:44.000000 ddtank-1.1.2/src/ddtank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-03-06 01:55:44.000000 ddtank-1.1.2/src/ddtank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 01:55:44.000000 ddtank-1.1.2/src/ddtank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-03-06 01:55:44.000000 ddtank-1.1.2/src/ddtank.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-06 01:55:44.000000 ddtank-1.1.2/src/ddtank.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 06:43:06.680157 ddtank-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2022-12-26 11:39:15.000000 ddtank-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     9457 2023-04-11 06:43:06.680157 ddtank-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9065 2023-03-06 01:32:13.000000 ddtank-1.1.3/README.md
+-rw-rw-rw-   0        0        0      592 2023-04-11 06:42:55.000000 ddtank-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 06:43:06.680157 ddtank-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 06:43:06.629953 ddtank-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:43:06.649998 ddtank-1.1.3/src/ddtank/
+-rw-rw-rw-   0        0        0      107 2023-04-09 00:26:48.000000 ddtank-1.1.3/src/ddtank/__init__.py
+-rw-rw-rw-   0        0        0     4837 2023-03-06 14:41:34.000000 ddtank-1.1.3/src/ddtank/ddtanker.py
+-rw-rw-rw-   0        0        0    15855 2023-03-28 00:59:26.000000 ddtank-1.1.3/src/ddtank/status.py
+-rw-rw-rw-   0        0        0     2948 2023-03-06 11:23:42.000000 ddtank-1.1.3/src/ddtank/team.py
+-rw-rw-rw-   0        0        0     1624 2023-03-13 03:12:52.000000 ddtank-1.1.3/src/ddtank/team2.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:43:06.680157 ddtank-1.1.3/src/ddtank/utils/
+-rw-rw-rw-   0        0        0        4 2023-03-06 07:23:38.000000 ddtank-1.1.3/src/ddtank/utils/__init__.py
+-rw-rw-rw-   0        0        0     1825 2023-03-13 02:22:04.000000 ddtank-1.1.3/src/ddtank/utils/aim.py
+-rw-rw-rw-   0        0        0     2119 2023-03-06 01:17:05.000000 ddtank-1.1.3/src/ddtank/utils/get_capture.py
+-rw-rw-rw-   0        0        0     1180 2023-03-13 02:09:51.000000 ddtank-1.1.3/src/ddtank/utils/get_game.py
+-rw-rw-rw-   0        0        0      716 2023-03-06 01:12:51.000000 ddtank-1.1.3/src/ddtank/utils/get_map.py
+-rw-rw-rw-   0        0        0     1773 2023-03-06 07:24:58.000000 ddtank-1.1.3/src/ddtank/utils/get_script.py
+-rw-rw-rw-   0        0        0      793 2023-03-02 00:31:25.000000 ddtank-1.1.3/src/ddtank/utils/stop_thread.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:43:06.659759 ddtank-1.1.3/src/ddtank.egg-info/
+-rw-rw-rw-   0        0        0     9457 2023-04-11 06:43:06.000000 ddtank-1.1.3/src/ddtank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-11 06:43:06.000000 ddtank-1.1.3/src/ddtank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:43:06.000000 ddtank-1.1.3/src/ddtank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-04-11 06:43:06.000000 ddtank-1.1.3/src/ddtank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 06:43:06.000000 ddtank-1.1.3/src/ddtank.egg-info/top_level.txt
```

### Comparing `ddtank-1.1.2/LICENSE` & `ddtank-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddtank-1.1.2/PKG-INFO` & `ddtank-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ddtank
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package used for writing ddtank game scripts.
 Author-email: zx <jugking6688@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DDTank
 
 A package used for writing ddtank game scripts.
```

### Comparing `ddtank-1.1.2/README.md` & `ddtank-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ddtank-1.1.2/pyproject.toml` & `ddtank-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ddtank"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="zx", email="jugking6688@gmail.com" },
 ]
 description = "A package used for writing ddtank game scripts."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pywin32==227",
```

### Comparing `ddtank-1.1.2/src/ddtank/ddtanker.py` & `ddtank-1.1.3/src/ddtank/ddtanker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import PySimpleGUI as sg
 
 from ddtank.utils.get_game import get_game
 from ddtank.utils.get_script import get_script_name, start_script, stop_script
 from ddtank.utils.get_capture import get_point, get_image
 from ddtank.utils.get_map import get_map
 
-menu_def = [['游戏', ['窗口识别']],
-            ['辅助功能', ['截图取色', '截图取图', '地图识别']]
-            ]
-layout = [[sg.Menu(menu_def, tearoff=False, pad=(20, 1))],
-          [sg.Text('选择游戏窗口'), sg.Combo(values=get_game(True)[1], default_value='请选择游戏窗口', size=(20, 1), key='窗口列表')],
-          [sg.Text('选择游戏窗口所执行的脚本内容')],
-          [sg.Listbox(values=get_script_name(), size=(32, 12), key='脚本列表')],
-          [sg.Button('执行', key='执行', size=(8, 1)), sg.Button('结束', key='结束', size=(8, 1)), sg.Button('退出', key='退出', size=(8, 1))],
-          [sg.StatusBar('欢迎使用ddtank', size=(32, 1), relief=sg.RELIEF_SOLID, key='状态栏')]
-          ]
-
 
 class DDTanker:
     def __init__(self):
+        self.menu_def = [['游戏', ['窗口识别']],
+                         ['辅助功能', ['截图取色', '截图取图', '地图识别']]
+                         ]
+        self.layout = [[sg.Menu(self.menu_def, tearoff=False, pad=(20, 1))],
+                       [sg.Text('选择游戏窗口'), sg.Combo(values=get_game(True)[1], default_value='请选择游戏窗口', size=(20, 1), key='窗口列表')],
+                       [sg.Text('选择游戏窗口所执行的脚本内容')],
+                       [sg.Listbox(values=get_script_name(), size=(32, 12), key='脚本列表')],
+                       [sg.Button('执行', key='执行', size=(8, 1)), sg.Button('结束', key='结束', size=(8, 1)), sg.Button('退出', key='退出', size=(8, 1))],
+                       [sg.StatusBar('欢迎使用ddtank', size=(32, 1), relief=sg.RELIEF_SOLID, key='状态栏')]
+                       ]
         self.handle_list, self.title_list = get_game(True)
         self.thread_list = [None] * len(self.handle_list)
-        self.window = sg.Window('ddtank脚本执行器', layout)
+        self.window = sg.Window('ddtank脚本执行器', self.layout)
 
         while True:
             self.event, self.values = self.window.read()
             if self.event in (None, '退出'):
                 break
             elif self.event == '窗口识别':
                 self.update_windows()
@@ -69,14 +68,15 @@
 
     def update_windows(self):
         for thread in self.thread_list:
             if thread is not None:
                 self.window['状态栏'].update('当前有游戏窗口脚本运行中，请先结束')
         else:
             self.handle_list, self.title_list = get_game(True)
+            self.thread_list = [None] * len(self.handle_list)
             self.window['窗口列表'].update('请选择游戏窗口', values=self.title_list)
             self.window['状态栏'].update('重新识别窗口成功')
 
     def get_handle(self):
         if self.window['窗口列表'].get() not in self.window['窗口列表'].Values:
             self.window['状态栏'].update('当前没有选择游戏窗口')
         else:
@@ -85,8 +85,8 @@
             return handle
 
     def get_focus_script(self):
         script = self.values['脚本列表']
         if len(script) > 0:
             return script[0]
         else:
-            self.window['状态栏'].update('当前没有选择要执行的脚本')
+            self.window['状态栏'].update('当前没有选择要执行的脚本')
```

### Comparing `ddtank-1.1.2/src/ddtank/status.py` & `ddtank-1.1.3/src/ddtank/status.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import win32ui
 import cv2
 import numpy as np
 import string
 import time
 import ddtcv
 
-from typing import Union
+from typing import Union, Literal, Callable, Optional
 from threading import Thread
 from ctypes import windll
 from ddtank.utils.stop_thread import stop_thread
+from ddtank.utils.get_game import get_game
 
 VkKeyScanA = windll.user32.VkKeyScanA
 
 keycode_dict = {
     "back": 0x08,
     "tab": 0x09,
     "enter": 0x0D,
@@ -88,45 +89,57 @@
     elif key in keycode_dict.keys():
         return keycode_dict[key]
     else:
         return -1
 
 
 class Status:
-    def __init__(self, hwnd: int, title: str = None):
-        self.handle = hwnd
-        self.dc = win32gui.GetWindowDC(self.handle)
-        if title:
-            self.name = title
+    def __init__(self, info: Union[int, str]):
+        games = get_game()
+        if isinstance(info, str):
+            for title in games.keys():
+                if info in title:
+                    self.handle = games[title]
+                    self.name = info
+                    break
+            else:
+                raise RuntimeError(f'找不到标题中存在{info}的游戏窗口')
+        elif isinstance(info, int):
+            self.handle = info
+            self.name = f'玩家{info}'
         else:
-            self.name = f'{hwnd}'
+            raise TypeError('info类型有误')
 
+        self.dc = win32gui.GetWindowDC(self.handle)
         self.thread = None
 
         self.capture_result = None
         self.image_path = './image'
+        self.repeat_find_period = 1000
 
         self.wind = None
         self.angle = None
         self.map_pos = None
         self.box_pos = None
         self.box_width = None
         self.blues = None
         self.cur_pos = None
         self.reds = None
         self.circle = None
 
+        self.team_task = []
+
     def __repr__(self) -> str:
         return self.name
 
     def task(self):
         pass
 
-    def start(self):
-        self.thread = Thread(target=self.task)
+    def start(self, task_func: Callable = None):
+        self.thread = Thread(target=self.task) if task_func is None else Thread(target=task_func)
         self.thread.setDaemon(True)
         self.thread.start()
         return self.thread.ident
 
     def stop(self):
         stop_thread(self.thread)
         self.thread = None
@@ -149,22 +162,15 @@
     def __press(self, key: str, period: int = None):
         keycode = get_keycode(key)
         win32api.SendMessage(self.handle, win32con.WM_KEYDOWN, keycode, 0)
         if period:
             self.__delay(period)
         win32api.SendMessage(self.handle, win32con.WM_KEYUP, keycode, 0)
 
-    def capture(self, position: tuple = (0, 0, 1000, 600), r: bool = False):
-        """
-        对角色游戏窗口执行截图操作，默认将截图存储在self.capture_result而不是返回一个图片，如果需要返回值，请设置r = True
-        注意，对于某些浏览器或登陆器，此方法可能无法正确获取截图(表现为全黑色截图)
-        因此，您需要自己来选择合适的登陆器以正确运行脚本
-        :param position: 指明截图位置的元组，分别为左上角x坐标、左上角y坐标、宽度、高度，默认为(0, 0, 1000, 600)即整个窗口
-        :param r: 是否返回图片，默认为False
-        """
+    def capture(self, position: tuple = (0, 0, 1000, 600), return_img: bool = False):
         x, y, w, h = position
         hwnd_dc = win32gui.GetWindowDC(self.handle)
         mfc_dc = win32ui.CreateDCFromHandle(hwnd_dc)
         save_dc = mfc_dc.CreateCompatibleDC()
         save_bit_map = win32ui.CreateBitmap()
         save_bit_map.CreateCompatibleBitmap(mfc_dc, w, h)
         save_dc.SelectObject(save_bit_map)
@@ -172,288 +178,231 @@
         signed_ints_array = save_bit_map.GetBitmapBits(True)
         img = np.frombuffer(signed_ints_array, dtype="uint8")
         img.shape = (h, w, 4)
         win32gui.DeleteObject(save_bit_map.GetHandle())
         mfc_dc.DeleteDC()
         save_dc.DeleteDC()
         img = cv2.cvtColor(img, cv2.COLOR_RGBA2RGB)
-        if r:
-            return img
         self.capture_result = img
+        return img if return_img else None
 
     def activate(self, period: int = 0):
         win32api.PostMessage(self.handle, win32con.WM_SETFOCUS, 0, 0)
         self.__sleep(period)
 
     def sleep(self, period: int):
         self.__sleep(period)
 
-    def find(self, method: str = 'find', **kwargs) -> Union[tuple, str, None]:
+    def find(self, method: Literal['find', 'rfind', 'mfind', 'find_image', 'rfind_image'] = 'find', **kwargs) -> Union[tuple, str, bool]:
         self.activate()
         if method in ('find', 'f'):
-            pos = kwargs['pos']
+            pos, rgb = kwargs['pos'], kwargs.get('rgb', None)
             pixel = win32gui.GetPixel(self.dc, *pos)
-            red = pixel & 0xff
-            green = (pixel >> 8) & 0xff
-            blue = (pixel >> 16) & 0xff
-            return red, green, blue
+            pixel = pixel & 0xff, (pixel >> 8) & 0xff, (pixel >> 16) & 0xff
+            if rgb is None:
+                return pixel
+            else:
+                # print(f'pixel: {pixel}')
+                # print(f'rgb: {rgb}')
+                return True if pixel == rgb else False
         elif method in ('rfind', 'rf', 'r'):
-            pos = kwargs['pos']
-            while True:
-                self.activate()
-                if self.find('find', pos=pos) == kwargs['rgb']:
-                    break
-                else:
-                    if 'el' in kwargs.keys():
-                        kwargs['el']()
-                    if 'period' in kwargs.keys():
-                        self.__sleep(kwargs['period'])
-                    else:
-                        self.__sleep(100)
+            pos, rgb = kwargs['pos'], kwargs['rgb']
+            while not (self.find('find', pos=pos) == rgb):
+                kwargs['el']() if 'el' in kwargs else self.activate()
+                self.__sleep(kwargs['period'] if 'period' in kwargs else self.repeat_find_period)
         elif method in ('mfind', 'mf', 'm'):
-            for condition in kwargs.keys():
-                pos: tuple = kwargs[condition][0]
-                rgb: tuple = kwargs[condition][1]
+            for condition, (pos, rgb) in kwargs.items():
                 if self.find('find', pos=pos) == rgb:
                     return condition
         elif method in ('find_image', 'fi', 'image', 'i'):
-            if 'part' in kwargs.keys():
-                part = kwargs['part']
-            else:
-                part = (0, 0, 1000, 600)
-            img = kwargs['img']
+            part, img = kwargs.get('part', (0, 0, 1000, 600)), kwargs['img']
             self.capture()
-            template_image = cv2.imread(self.image_path + '/' + img + '.png', 0)
+            if isinstance(img, np.ndarray) and len(img.shape) == 3 and img.shape[2] in [3, 4]:
+                template_image = img
+            elif isinstance(img, str):
+                if '.' in img:
+                    template_image = cv2.imread(img)
+                else:
+                    template_image = cv2.imread(self.image_path + '/' + img + '.png', 0)
+            else:
+                raise RuntimeError('找不到所要识别的图片')
+
             x, y, w, h = part
             image = cv2.cvtColor(self.capture_result, cv2.COLOR_BGR2GRAY)
-            res = cv2.matchTemplate(image[y:y+h, x:x+w], template_image, cv2.TM_CCOEFF_NORMED)
+            res = cv2.matchTemplate(image[y:y + h, x:x + w], template_image, cv2.TM_CCOEFF_NORMED)
             min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
             if max_val >= 0.9:
                 w, h = template_image.shape[::-1]
                 return int(max_loc[0] + w / 2), int(max_loc[1] + h / 2)
-            else:
-                return None
 
-    def click(self, method: str = 'normal', **kwargs):
+    def click(self, method: Literal['normal', 'find', 'rfind', 'find_image', 'rfind_image'] = 'normal', **kwargs):
+        self.activate()
         if method in ('normal', 'n', 'click'):
             pos = kwargs['pos']
             self.__click(pos=pos)
         elif method in ('find', 'f'):
             pos = kwargs['pos']
             if self.find('find', pos=pos) == kwargs['rgb']:
                 self.__click(pos=pos)
+                return True
+            return False
         elif method in ('rfind', 'rf', 'r'):
-            pos = kwargs['pos']
-            while True:
-                if self.find('find', pos=pos) == kwargs['rgb']:
-                    self.__click(pos=pos)
-                    break
-                else:
-                    if 'el' in kwargs.keys():
-                        kwargs['el']()
-                    if 'period' in kwargs.keys():
-                        self.__sleep(kwargs['period'])
-                    else:
-                        self.__sleep(100)
+            pos, rgb = kwargs['pos'], kwargs['rgb']
+            while not (self.find('find', pos=pos) == rgb):
+                kwargs['el']() if 'el' in kwargs else self.activate()
+                self.__sleep(kwargs['period'] if 'period' in kwargs else self.repeat_find_period)
+            self.__click(pos=pos)
         elif method in ('find_image', 'fi', 'i'):
-            img = kwargs['img']
-            if 'part' in kwargs.keys():
-                part = kwargs['part']
-            else:
-                part = (0, 0, 1000, 600)
-            pos = self.find('image', img=img, part=part)
-            if pos:
+            img, part = kwargs['img'], kwargs.get('part', (0, 0, 1000, 600))
+            if pos := self.find('find_image', img=img, part=part):
                 self.__click(pos)
+                return True
+            return False
         elif method in ('rfind_image', 'rfi', 'ri'):
-            img = kwargs['img']
-            if 'part' in kwargs.keys():
-                part = kwargs['part']
+            img, part = kwargs['img'], kwargs.get('part', (0, 0, 1000, 600))
+            while not (pos := self.find('find_image', img=img, part=part)):
+                kwargs['el']() if 'el' in kwargs else self.activate()
+                self.__sleep(kwargs['period'] if 'period' in kwargs else self.repeat_find_period)
+            self.__click(pos)
+
+    def press(self, key_series: Union[tuple, str, int]):
+        if isinstance(key_series, str):
+            self.__press(key_series)
+            return
+
+        elements = []
+        for elem in key_series:
+            if isinstance(elem, str):
+                elements.append(('press', elem))
+            elif isinstance(elem, int):
+                elements.append(('sleep', elem))
+            elif isinstance(elem, tuple):
+                elements.append(('press', *elem))
+
+        for action, arg in elements:
+            # getattr(self, f"__{action}")(arg)
+            if action == 'press':
+                self.__press(arg)
             else:
-                part = (0, 0, 1000, 600)
-            while True:
-                pos = self.find('image', img=img, part=part)
-                if pos:
-                    self.__click(pos)
-                    break
-                else:
-                    if 'el' in kwargs.keys():
-                        kwargs['el']()
-                    if 'period' in kwargs.keys():
-                        self.__sleep(kwargs['period'])
-                    else:
-                        self.__sleep(100)
-
-    def press(self, key_series):
-        for key in key_series:
-            if type(key) == str:
-                self.__press(key)
-            elif type(key) == int:
-                self.__sleep(key)
-            elif type(key) == tuple:
-                self.__press(*key)
+                self.__press(arg)
+
+    def input(self, content: str):
+        input_char = [ord(c) for c in content]
+        for char in input_char:
+            win32api.PostMessage(self.handle, win32con.WM_CHAR, char, 0)
 
     def read(self, is_circle: bool = False):
-        def cal_time(func):
-            def wrapper(*args, **kwargs):
-                start = time.perf_counter()
-                result = func(*args, **kwargs)
-                # print(f'{func.__name__} running time: {time.perf_counter() - start}')
-                return result
-            return wrapper
 
-        @cal_time
         def read_wind():
             image = self.capture_result
             b, g, r = image.item(21, 468, 0), image.item(21, 468, 1), image.item(21, 468, 2)
             if b == 252 and g == r and g > 240 and r > 240:
                 face = 1
             else:
                 face = -1
             return ddtcv.Wind(self.capture_result) * face
 
-        @cal_time
         def read_angle():
             return ddtcv.Angle(self.capture_result)
 
-        @cal_time
         def read_small_map():
             return np.argwhere(np.all(self.capture_result[1, 750:] == [160, 160, 160], axis=-1))[0, 0] + 742
 
-        @cal_time
         def read_white_box():
             img = np.where(np.any(self.capture_result[24:120, self.map_pos:998] != [153, 153, 153], axis=-1), 0, 255).astype('uint8')
             contours, hierarchy = cv2.findContours(img, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             for cnt in contours:
                 x, y, w, h = cv2.boundingRect(cnt)
                 if w > 30:
                     white_box_pos = (x, y)
                     white_box_width = w / 10
                     return white_box_pos, white_box_width
             return None
 
-        @cal_time
         def read_blue():
             blue_list = []
             blue_triangle = None
             img = np.where(np.any(self.capture_result[24:120, self.map_pos:998] != [204, 51, 0], axis=-1), 0, 255).astype('uint8')
             contours, hierarchy = cv2.findContours(img, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             for cnt in contours:
                 x, y, w, h = cv2.boundingRect(cnt)
                 if h > 3:
                     blue = (int(x + w / 2), int(y + h / 2))
                     blue_list.append(blue)
                 elif 2 <= h <= 4 and 4 <= w <= 6:
                     blue_triangle = (int(x + w / 2), int(y + h / 2))
             return blue_list, blue_triangle
 
-        @cal_time
         def read_red():
             red_list = []
             img = np.where(np.any(self.capture_result[24:120, self.map_pos:998] != [0, 0, 255], axis=-1), 0, 255).astype('uint8')
             contours, hierarchy = cv2.findContours(img, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             for cnt in contours:
                 x, y, w, h = cv2.boundingRect(cnt)
                 if h > 3:
                     red = (int(x + w / 2), int(y + h / 2))
                     red_list.append(red)
             return red_list
 
-        @cal_time
         def read_circle():
             def get_circle():
                 self.activate()
-                capture_1 = self.capture(position=(self.map_pos, 24, 998 - self.map_pos, 120 - 24), r=True)
+                capture_1 = self.capture(position=(self.map_pos, 24, 998 - self.map_pos, 120 - 24), return_img=True)
                 capture_1 = cv2.cvtColor(capture_1, cv2.COLOR_BGR2GRAY)
                 self.__sleep(30)
-                capture_2 = self.capture(position=(self.map_pos, 24, 998 - self.map_pos, 120 - 24), r=True)
+                capture_2 = self.capture(position=(self.map_pos, 24, 998 - self.map_pos, 120 - 24), return_img=True)
                 capture_2 = cv2.cvtColor(capture_2, cv2.COLOR_BGR2GRAY)
                 image = np.where(capture_1 == capture_2, 255, 0).astype('uint8')
                 contours, _ = cv2.findContours(image, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
                 for cnt in contours:
                     x, y, w, h = cv2.boundingRect(cnt)
                     if 15 < w < 25 or 15 < h < 25 and w == h:
                         self_x = int(x + w / 2)
                         self_y = int(y + h / 2)
                         return self_x, self_y
             while True:
                 circle_pos = get_circle()
                 if circle_pos:
                     return circle_pos
-                else:
-                    if is_circle:
-                        return None
-                    self.__sleep(100)
+                elif is_circle:
+                    return None
+                self.__sleep(100)
 
         self.capture()
         self.wind = read_wind()
         self.angle = read_angle()
         self.map_pos = read_small_map()
         self.box_pos, self.box_width = read_white_box()
         self.blues, self.cur_pos = read_blue()
         self.reds = read_red()
         self.circle = read_circle()
 
-    def shot(self, shot_angle, shot_strength: int, shot_item: tuple = None):
-        """
-        综合模拟发射炮弹操作
-        注意，使用此方法前需要先执行self.read方法，否则信息得不到及时更新
-        :param shot_angle: 发射的角度，若传递一个元组则执行变角操作
-        :param shot_strength: 发射的力度
-        :param shot_item: 使用的道具按键，多个道具之间用','分隔
-        :return: 无返回值
-        """
+    def shot(self, shot_angle: Union[int, tuple, None], shot_strength: int, shot_item: tuple = None, wait: bool = False):
         def change_angle(current_angle: int, target_angle: int):
-            """
-            调整角度至指定角度
-            :param current_angle: 当前角度
-            :param target_angle: 目标角度
-            :return: 无返回值
-            """
-            if current_angle == target_angle:
-                return
-            elif current_angle < target_angle:
-                for i in range(target_angle - current_angle):
-                    self.__press('W')
-            elif current_angle > target_angle:
-                for i in range(current_angle - target_angle):
-                    self.__press('S')
+            diff = target_angle - current_angle
+            direction = 'W' if diff > 0 else 'S'
+            for i in range(abs(diff)):
+                self.__press(direction)
 
         def press_shot(strength: int):
-            """
-            高精度模拟力度操作
-            :param strength: 模拟的力度数值，为0-100之间的整数
-            :return: 无返回值
-            """
-            if strength == 0:
-                self.__press('space', period=0)
-            x_pos, y_pos = 149 + int(strength * 5), 590
-            if (x_pos + 1) % 5 == 0:
-                x_pos += 1
-            if strength == 100:
-                x_pos = 647
-
-            win32api.PostMessage(self.handle, win32con.WM_KEYDOWN, 32, 0)
-            self.__delay(100)
-            pixel: tuple = self.capture_result[y_pos, x_pos]
-            while True:
-                if (self.capture_result[y_pos, x_pos] != pixel).any():
-                    win32api.PostMessage(self.handle, win32con.WM_KEYUP, 32, 0)
-                    break
+            self.__press('space', period=(strength + 1) * 40)
 
-        if shot_item:
-            self.press(shot_item)
-        if type(shot_angle) == int:
+        self.find('rfind', pos=(495, 163), rgb=(255, 255, 224)) if wait else None
+        self.press(shot_item) if shot_item else None
+        if isinstance(shot_angle, int):
             change_angle(self.angle, shot_angle)
             press_shot(shot_strength)
-        elif type(shot_angle) == tuple or list:
+        elif isinstance(shot_angle, (list, tuple)):
             change_angle(self.angle, shot_angle[0])
             press_shot(shot_strength)
             for i in range(1, len(shot_angle)):
-                self.__delay(800)
+                self.__sleep(800)
                 change_angle(shot_angle[i-1], shot_angle[i])
+        else:
+            press_shot(shot_strength)
 
     def move(self, move_face: str, move_period: int, reverse_face: bool = False):
         """
         角色移动
         :param move_face: 移动朝向
         :param move_period: 移动时间(毫秒)
         :param reverse_face: 移动完后是否逆转朝向
```

### Comparing `ddtank-1.1.2/src/ddtank/utils/get_capture.py` & `ddtank-1.1.3/src/ddtank/utils/get_capture.py`

 * *Files identical despite different names*

### Comparing `ddtank-1.1.2/src/ddtank/utils/get_map.py` & `ddtank-1.1.3/src/ddtank/utils/get_map.py`

 * *Files identical despite different names*

### Comparing `ddtank-1.1.2/src/ddtank/utils/get_script.py` & `ddtank-1.1.3/src/ddtank/utils/get_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import importlib.util
 import ctypes
 import inspect
 
-
 # 指定目录路径
 directory = './script'
 
 def get_script_name():
     if not os.path.exists(directory):
         os.mkdir(directory)
     script_name_list = []
```

### Comparing `ddtank-1.1.2/src/ddtank/utils/stop_thread.py` & `ddtank-1.1.3/src/ddtank/utils/stop_thread.py`

 * *Files identical despite different names*

### Comparing `ddtank-1.1.2/src/ddtank.egg-info/PKG-INFO` & `ddtank-1.1.3/src/ddtank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ddtank
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package used for writing ddtank game scripts.
 Author-email: zx <jugking6688@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DDTank
 
 A package used for writing ddtank game scripts.
```

