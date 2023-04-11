# Comparing `tmp/ScaleConvertion-0.3.tar.gz` & `tmp/ScaleConvertion-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ScaleConvertion-0.3.tar", last modified: Mon Apr 10 01:49:31 2023, max compression
+gzip compressed data, was "dist\ScaleConvertion-0.4.tar", last modified: Tue Apr 11 08:01:27 2023, max compression
```

## Comparing `ScaleConvertion-0.3.tar` & `ScaleConvertion-0.4.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/
--rw-rw-rw-   0        0        0     1189 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-09 16:11:33.000000 ScaleConvertion-0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/Model/
--rw-rw-rw-   0        0        0     7201 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/Efficientnet.py
--rw-rw-rw-   0        0        0    12126 2023-03-05 09:30:27.000000 ScaleConvertion-0.3/ScaleConvertion/Model/Restnet.py
--rw-rw-rw-   0        0        0     9277 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel.py
--rw-rw-rw-   0        0        0     9351 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel_2.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/Model/__init__.py
--rw-rw-rw-   0        0        0    26665 2023-04-09 06:38:21.000000 ScaleConvertion-0.3/ScaleConvertion/Model/restnet_transformer.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/
--rw-rw-rw-   0        0        0      556 2023-04-09 11:16:51.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/ConcatAnswer.py
--rw-rw-rw-   0        0        0     2962 2023-04-09 15:57:59.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/DataPredict.py
--rw-rw-rw-   0        0        0     9504 2023-04-09 14:53:26.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/Draw_Window.py
--rw-rw-rw-   0        0        0     2232 2023-04-09 12:04:26.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/MakeData.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/PicProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/
--rw-rw-rw-   0        0        0      853 2023-04-09 15:59:04.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/Info.py
--rw-rw-rw-   0        0        0     1172 2023-04-09 14:00:58.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/PictureInfo.py
--rw-rw-rw-   0        0        0     7930 2023-01-04 15:45:26.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/SED.py
--rw-rw-rw-   0        0        0      878 2023-04-09 12:12:21.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/SaveFile.py
--rw-rw-rw-   0        0        0     1308 2023-04-09 08:10:19.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/ScaleCompute.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/Utiles/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.3/ScaleConvertion/__init__.py
--rw-rw-rw-   0        0        0      993 2023-04-09 15:01:28.000000 ScaleConvertion-0.3/ScaleConvertion/main.py
-drwxrwxrwx   0        0        0        0 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      900 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/ScaleConvertion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 01:49:31.000000 ScaleConvertion-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1936 2023-04-10 01:47:32.000000 ScaleConvertion-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/
+-rw-rw-rw-   0        0        0     2355 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-04-11 08:00:40.000000 ScaleConvertion-0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion/
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion/Model/
+-rw-rw-rw-   0        0        0     7201 2023-04-09 06:38:21.000000 ScaleConvertion-0.4/ScaleConvertion/Model/Efficientnet.py
+-rw-rw-rw-   0        0        0    12126 2023-03-05 09:30:27.000000 ScaleConvertion-0.4/ScaleConvertion/Model/Restnet.py
+-rw-rw-rw-   0        0        0     9277 2023-04-09 06:38:21.000000 ScaleConvertion-0.4/ScaleConvertion/Model/SwimModel.py
+-rw-rw-rw-   0        0        0     9351 2023-04-09 06:38:21.000000 ScaleConvertion-0.4/ScaleConvertion/Model/SwimModel_2.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.4/ScaleConvertion/Model/__init__.py
+-rw-rw-rw-   0        0        0    26665 2023-04-09 06:38:21.000000 ScaleConvertion-0.4/ScaleConvertion/Model/restnet_transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/
+-rw-rw-rw-   0        0        0      556 2023-04-09 11:16:51.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/ConcatAnswer.py
+-rw-rw-rw-   0        0        0     4284 2023-04-11 07:37:02.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/DataPredict.py
+-rw-rw-rw-   0        0        0    11476 2023-04-11 07:45:28.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/Draw_Window.py
+-rw-rw-rw-   0        0        0     2232 2023-04-11 07:28:25.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/MakeData.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.4/ScaleConvertion/PicProcess/__init__.py
+-rw-rw-rw-   0        0        0     2505 2023-04-11 07:45:28.000000 ScaleConvertion-0.4/ScaleConvertion/SC.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/
+-rw-rw-rw-   0        0        0      853 2023-04-09 15:59:04.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/Info.py
+-rw-rw-rw-   0        0        0     2909 2023-04-11 03:17:55.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/PictureInfo.py
+-rw-rw-rw-   0        0        0     8102 2023-04-11 03:04:26.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/SED.py
+-rw-rw-rw-   0        0        0     2576 2023-04-11 07:51:49.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/SaveFile.py
+-rw-rw-rw-   0        0        0     1308 2023-04-09 08:10:19.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/ScaleCompute.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.4/ScaleConvertion/Utiles/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-09 06:31:29.000000 ScaleConvertion-0.4/ScaleConvertion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion/test/
+-rw-rw-rw-   0        0        0      127 2023-04-11 08:01:21.000000 ScaleConvertion-0.4/ScaleConvertion/test/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-04-11 07:20:49.000000 ScaleConvertion-0.4/ScaleConvertion/test/test.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 07:50:52.000000 ScaleConvertion-0.4/ScaleConvertion/test/testuav.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/
+-rw-rw-rw-   0        0        0     2355 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/ScaleConvertion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:01:27.000000 ScaleConvertion-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-04-11 07:55:21.000000 ScaleConvertion-0.4/setup.py
```

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Model/Efficientnet.py` & `ScaleConvertion-0.4/ScaleConvertion/Model/Efficientnet.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Model/Restnet.py` & `ScaleConvertion-0.4/ScaleConvertion/Model/Restnet.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel.py` & `ScaleConvertion-0.4/ScaleConvertion/Model/SwimModel.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Model/SwimModel_2.py` & `ScaleConvertion-0.4/ScaleConvertion/Model/SwimModel_2.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Model/restnet_transformer.py` & `ScaleConvertion-0.4/ScaleConvertion/Model/restnet_transformer.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/PicProcess/ConcatAnswer.py` & `ScaleConvertion-0.4/ScaleConvertion/PicProcess/ConcatAnswer.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/PicProcess/Draw_Window.py` & `ScaleConvertion-0.4/ScaleConvertion/PicProcess/Draw_Window.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/9 15:07
 # @Author  : qxcnwu
 # @FileName: Draw_Window.py
 # @Software: PyCharm
 import os.path
 import tkinter as tk
+from math import tan, pi
 from tkinter import filedialog
 from typing import Any, List
 
 import cv2
 import numpy as np
 
 from .DataPredict import predict
 from .ConcatAnswer import concate
 from .MakeData import DataMaker
 from ..Utiles.Info import Sensors_IFOV, UAV_IFOV
-from ..Utiles.PictureInfo import read_pic, copy_image
+from ..Utiles.PictureInfo import read_pic, copy_image, get_ref, get_true, read_tiff
 from ..Utiles.SED import SED
-from ..Utiles.SaveFile import save_csv
+from ..Utiles.SaveFile import save_csv_png, save_csv_tif
 from ..Utiles.ScaleCompute import compute_sensors_rad, compute_pixel_rad
 
 
 class struct_getPoint:
     def __init__(self, image: Any, name: str, sensors_rad: List[int], pixel_rad: List[int], img_h: int, img_w: int):
         """
         get point and pixel rad
@@ -160,39 +161,89 @@
     :param pixel:
     :param sensors_altitude:    :param img_path:
     :param sensors_IFOV:
     :param uav_IFOV:
     :return:
     """
     # read dataset init
-    if img_path == None:
-        img_path = filedialog.askopenfilename(title='chose uav picture')
+    print("start get picture process step 1/6")
     img_path = copy_image(img_path, os.path.join(os.path.dirname(__file__), "tmp"))
     altitude, img_h, img_w, img_c = read_pic(img_path)
     sen_alt = [compute_sensors_rad(img_h, img_w, altitude, i, sensors_IFOV, uav_IFOV) for i in sensors_altitude]
     pixel_rad = [compute_pixel_rad(img_h, img_w, altitude, uav_IFOV, i) for i in pixel]
+    print("start get points step 2/6")
     img = cv2.imdecode(np.fromfile(img_path, dtype=np.uint8), cv2.IMREAD_UNCHANGED)
     tmp = struct_getPoint(img, os.path.basename(img_path), sen_alt, pixel_rad, img_h, img_w)
     tmp.getPoint()
     while True:
         # wait to exit
         flag = cv2.waitKey(1)
         if flag == ord('s'):
             cv2.destroyAllWindows()
             break
     # data process
+    print("start make dataset step 3/6")
     dm = DataMaker(img_path, tmp.point[:-1], sen_alt, tmp.point[-1], tmp.true_pixel)
     # data pridict
+    print("start predict dataset step 4/6")
     ans = predict(dm.small_path, dm.big_path)
     # save answer
+    print("start concate answer step 5/6")
     out = concate(seds, ans)
     # end
-    save_csv(out, pixel[0:len(tmp.true_pixel)], save_dir)
-    return out
+    print("start concate save answer step 6/6")
+    save_csv_png(out, pixel[0:len(tmp.true_pixel)], save_dir, seds)
+    return out, ans, dm
 
 
-if __name__ == '__main__':
-    root = tk.Tk()
-    root.withdraw()
-    ans = read_(r"..\pic\31日-样区2-裸土-上东下西-H971m-77m（全）-5.JPG",
-                sensors_altitude=[1, 1, 1, 1, 1, 1, 1, 1],
-                pixel=[2, 4, 8, 10, 20, 30])
+def read_tif(img_path: str = None, tiff_path: str = None, save_dir: str = "",
+             sensors_IFOV: float = Sensors_IFOV.SEI_RS800,
+             scale_tiff: float = 0.065,
+             sen_alt: List[float] = None, pixel: List[float] = None):
+    """
+    read img and draw img
+    :param seds:
+    :param pixel:
+    :param sensors_altitude:    :param img_path:
+    :param sensors_IFOV:
+    :param uav_IFOV:
+    :return:
+    """
+    # read dataset init
+    print("start get picture process step 1/7")
+    img_path = copy_image(img_path, os.path.join(os.path.dirname(__file__), "tmp"))
+    imgs = read_tiff(tiff_path)
+    img_h, img_w, _ = imgs.shape
+
+    sen_alt = [int(tan(sensors_IFOV / 2 / 180 * pi) *
+                   altitude_sensors / 0.065) for altitude_sensors in sen_alt]
+    pixel_rad = [int(i / scale_tiff) for i in pixel]
+
+    print("start get points step 2/7")
+    img = cv2.imdecode(np.fromfile(img_path, dtype=np.uint8), cv2.IMREAD_UNCHANGED)
+    tmp = struct_getPoint(img, os.path.basename(img_path), sen_alt, pixel_rad, img_h, img_w)
+    tmp.getPoint()
+    while True:
+        # wait to exit
+        flag = cv2.waitKey(1)
+        if flag == ord('s'):
+            cv2.destroyAllWindows()
+            break
+
+    # get ref
+    print("start get refs step 3/7")
+    seds = get_ref(imgs, tmp.point[:-1], sen_alt)
+    seds_true = get_true(imgs, tmp.point[-1], tmp.true_pixel)
+
+    # data process
+    print("start make dataset step 4/7")
+    dm = DataMaker(img_path, tmp.point[:-1], sen_alt, tmp.point[-1], tmp.true_pixel)
+    # data pridict
+    print("start predict dataset step 5/7")
+    ans = predict(dm.small_path, dm.big_path)
+    # save answer
+    print("start concate answer step 6/7")
+    out = concate(seds, ans)
+    # end
+    print("start concate save answer step 7/7")
+    save_csv_tif(out, pixel[0:len(tmp.true_pixel)], save_dir, seds_true[0:len(tmp.true_pixel)], seds)
+    return out, ans, dm
```

### Comparing `ScaleConvertion-0.3/ScaleConvertion/PicProcess/MakeData.py` & `ScaleConvertion-0.4/ScaleConvertion/PicProcess/MakeData.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Utiles/Info.py` & `ScaleConvertion-0.4/ScaleConvertion/Utiles/Info.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Utiles/SED.py` & `ScaleConvertion-0.4/ScaleConvertion/Utiles/SED.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/7/11 15:40
 # @Author  : qxcnwu
 # @FileName: SED.py
 # @Software: PyCharm
 import math
 import os
+import tkinter
 from datetime import datetime
+from tkinter import filedialog
 from typing import List
 
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 import json
 from tqdm import tqdm
@@ -232,17 +234,25 @@
     ans = []
     for file in os.listdir(base_path):
         if not file.endswith("sed"):
             continue
         ans.append(SED(os.path.join(base_path, file)))
     return ans
 
+def getSeds():
+    root = tkinter.Tk()
+    root.withdraw()
+    fnstr = filedialog.askopenfilenames(filetypes=[("sed file", "*.sed"), ("all", "*.*")])
+    seds = []
+    alts = []
+    for name in fnstr:
+        sed = SED(name)
+        seds.append(sed.ref[:, -1])
+        try:
+            alts.append(float(sed.USER_FIELD1[1].replace('m', '')))
+        except:
+            alts.append(1.2)
+    root.destroy()
+    return seds, alts
 
 if __name__ == '__main__':
-    import os
-    for file in os.listdir("site_data/sn1335"):
-        if not file.endswith("sed"):
-            continue
-        path = os.path.join("site_data/sn1335", file)
-        sed = SED(path)
-        sed.draw_line([2], False, save_path=os.path.join(
-            "site_data/sn1335/ans", file.replace("sed", "jpg")))
+    pass
```

### Comparing `ScaleConvertion-0.3/ScaleConvertion/Utiles/ScaleCompute.py` & `ScaleConvertion-0.4/ScaleConvertion/Utiles/ScaleCompute.py`

 * *Files identical despite different names*

### Comparing `ScaleConvertion-0.3/ScaleConvertion.egg-info/SOURCES.txt` & `ScaleConvertion-0.4/ScaleConvertion.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 README.rst
 setup.py
+ScaleConvertion/SC.py
 ScaleConvertion/__init__.py
-ScaleConvertion/main.py
 ScaleConvertion.egg-info/PKG-INFO
 ScaleConvertion.egg-info/SOURCES.txt
 ScaleConvertion.egg-info/dependency_links.txt
 ScaleConvertion.egg-info/requires.txt
 ScaleConvertion.egg-info/top_level.txt
 ScaleConvertion/Model/Efficientnet.py
 ScaleConvertion/Model/Restnet.py
@@ -19,8 +19,11 @@
 ScaleConvertion/PicProcess/MakeData.py
 ScaleConvertion/PicProcess/__init__.py
 ScaleConvertion/Utiles/Info.py
 ScaleConvertion/Utiles/PictureInfo.py
 ScaleConvertion/Utiles/SED.py
 ScaleConvertion/Utiles/SaveFile.py
 ScaleConvertion/Utiles/ScaleCompute.py
-ScaleConvertion/Utiles/__init__.py
+ScaleConvertion/Utiles/__init__.py
+ScaleConvertion/test/__init__.py
+ScaleConvertion/test/test.py
+ScaleConvertion/test/testuav.py
```

### Comparing `ScaleConvertion-0.3/setup.py` & `ScaleConvertion-0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-'''
-Author: qxcnwu 2081896628@qq.com
-Date: 2023-04-09 21:34:20
-LastEditors: qxcnwu 2081896628@qq.com
-LastEditTime: 2023-04-10 00:18:40
-FilePath: \package\setup.py
-Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-'''
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/9 21:34
 # @Author  : qxcnwu
 # @FileName: setup.py
 # @Software: PyCharm
 from setuptools import setup, find_packages
 
 setup(
     name='ScaleConvertion',  # 包名
-    version='0.3',  # 版本
+    version='0.4',  # 版本
     description="Helps achieve surface reflectance scale conversion",  # 包简介
     long_description=open('README.rst').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='qxcnwu',  # 作者
     author_email='qxcnwu@gmail.com',  # 作者邮件
     maintainer='qxcnwu',  # 维护者
     maintainer_email='qxcnwu@gmail.com',  # 维护者邮件
@@ -32,14 +24,14 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',  # 设置编写时的python版本
     ],
     python_requires='>=3.4',  # 设置python版本要求
     install_requires=['tqdm', 'numpy', 'pandas', 'torch', 'timm', 'exifread', 'qt5_applications', 'matplotlib',
-                      'torchvision', 'requests', 'colour', 'opencv-python'],  # 安装所需要的库
+                      'torchvision', 'requests', 'colour', 'opencv-python','gdal'],  # 安装所需要的库
     # entry_points={
     #     'console_scripts': [
     #         ''],
     # },  # 设置命令行工具(可不使用就可以注释掉)
 
 )
```

