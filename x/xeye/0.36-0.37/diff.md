# Comparing `tmp/xeye-0.36.tar.gz` & `tmp/xeye-0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeye-0.36.tar", last modified: Sat Jan 28 14:21:14 2023, max compression
+gzip compressed data, was "xeye-0.37.tar", last modified: Tue Apr 11 10:16:36 2023, max compression
```

## Comparing `xeye-0.36.tar` & `xeye-0.37.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-01-28 14:21:14.096564 xeye-0.36/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.36/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-01-28 14:21:14.095396 xeye-0.36/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13348 2023-01-19 23:29:40.000000 xeye-0.36/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-01-28 14:18:34.000000 xeye-0.36/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-01-28 14:21:14.096734 xeye-0.36/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-01-28 14:21:14.087660 xeye-0.36/src/
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-01-28 14:21:14.092500 xeye-0.36/src/xeye/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3538 2023-01-28 14:04:32.000000 xeye-0.36/src/xeye/__build_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13687 2023-01-28 13:50:01.000000 xeye-0.36/src/xeye/__dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13129 2023-01-28 13:49:58.000000 xeye-0.36/src/xeye/__fast_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      187 2023-01-28 14:18:29.000000 xeye-0.36/src/xeye/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5357 2023-01-28 14:18:10.000000 xeye-0.36/src/xeye/__manual_dataset.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-01-28 14:21:14.094659 xeye-0.36/src/xeye.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-01-28 14:21:14.000000 xeye-0.36/src/xeye.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      318 2023-01-28 14:21:14.000000 xeye-0.36/src/xeye.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-01-28 14:21:14.000000 xeye-0.36/src/xeye.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-01-28 14:21:14.000000 xeye-0.36/src/xeye.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-01-28 14:21:14.000000 xeye-0.36/src/xeye.egg-info/top_level.txt
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.272905 xeye-0.37/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.37/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-04-11 10:16:36.272273 xeye-0.37/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13348 2023-01-19 23:29:40.000000 xeye-0.37/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-11 07:40:11.000000 xeye-0.37/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-11 10:16:36.273087 xeye-0.37/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.265690 xeye-0.37/src/
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.269623 xeye-0.37/src/xeye/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-11 07:39:23.000000 xeye-0.37/src/xeye/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.37/src/xeye/build_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14924 2023-04-11 08:53:43.000000 xeye-0.37/src/xeye/dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.37/src/xeye/fast_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.37/src/xeye/manual_dataset.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.271649 xeye-0.37/src/xeye.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      310 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/top_level.txt
```

### Comparing `xeye-0.36/LICENSE` & `xeye-0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `xeye-0.36/PKG-INFO` & `xeye-0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.36
+Version: 0.37
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `xeye-0.36/README.md` & `xeye-0.37/README.md`

 * *Files identical despite different names*

### Comparing `xeye-0.36/pyproject.toml` & `xeye-0.37/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xeye"
-version = "0.36"
+version = "0.37"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Create datasets for computer vision applications"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `xeye-0.36/src/xeye/__dataset.py` & `xeye-0.37/src/xeye/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,32 +2,58 @@
 import os
 from sklearn.model_selection import train_test_split
 import numpy as np
 import time
 
 
 class Dataset:
+    """
+    A class for collecting a dataset of images using OpenCV.
+
+    Attributes:
+        index (int): The index of the camera to be used for creating the dataset.
+        label (list): The list of names of the different types of images to be collected.
+        num (int): The number of frames to shoot for every image type.
+        height (int): The height of the individual frames.
+        width (int): The width of the individual frames.
+        standby_time (float): The number of seconds to wait between every frame.
+        perc (int): The percentage of data to use for training (the remaining will be used for validation).
+        name (str): The name of the dataset.
+
+    Examples:
+        >>> import xeye
+        >>> data = xeye.Dataset()
+        >>> data.setup()
+        >>> data.var_control()
+        >>> data.preview()
+        >>> data.rgb() # or data.gray()
+        >>> data.compress_train_test()
+        >>> data.compress_all()
+        >>> data.just.compress()
+    """
     index = 0
     label = []
     num = 0
     height = 0
     width = 0
-    class_dict = {}
-    tensor = {}
+    _class_dict = {}
+    _tensor = {}
     standby_time = 0
-    statusGray = 0
-    statusRGB = 0
+    _statusGray = 0
+    _statusRGB = 0
     perc = 0
     name = "dataset_raw"
-    # --------------------
-    # init image parameters
-    # --------------------
-    def init(self)->None:
+
+
+    def setup(self) -> None:
         """
-        The init function starts the terminal interface for setting up the parameters of the dataset.
+        Starts the terminal interface for setting up the parameters of the dataset.
+
+        Returns:
+            None
         """
         # clear terminal 
         if(os.name == 'posix'): #unix
             os.system('clear')
         else: #windows
             os.system('cls')
         # camera setting control 
@@ -66,21 +92,21 @@
             raise ValueError('Frame WIDTH must be greather than 0')
 
         # Waiting time in shooting loop
         self.standby_time = float(input('num. of waiting time (in sec.) between every frame: '))
         if self.standby_time < 0:
             raise ValueError('waiting time must be grater than 0...')
 
-
-    # --------------------
-    # preview 
-    # --------------------    
-    def preview(self)->None:
+  
+    def preview(self) -> None:
         """
-        Open the camera stream on a window. Helpful for checking the framing of the image.
+        Opens the camera stream on a window for checking the framing of the image.
+
+        Returns: 
+            None
         """
         print('\n')
         print('--- PREVIEW ---')
         camera = cv2.VideoCapture(self.index)
         while(True):
             status, frame = camera.read()
             if not status:
@@ -95,20 +121,20 @@
                 print('preview closed')
                 camera.release()
                 cv2.destroyAllWindows()
                 cv2.waitKey(1)
                 break
 
 
-    # ---------------
-    # grayscale images 
-    #----------------
-    def gray(self)->None:
+    def gray(self) -> None:
         """
-        Method for shooting images in grayscale. 
+        Method for shooting images in grayscale.
+
+        Returns:
+            None 
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
         camera = cv2.VideoCapture(self.index)
         # Index for files name 
         i = 0
         for folder in self.label:
@@ -132,24 +158,24 @@
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # set status
-        self.statusGray = 1
-        self.statusRGB = 0
+        self._statusGray = 1
+        self._statusRGB = 0
 
-    
-    # -----------
-    # rgb imges
-    # -----------
-    def rgb(self)->None:
+
+    def rgb(self) -> None:
         """
-        Method for shooting images in RGB. 
+        Method for shooting images in RGB.
+
+        Returns:
+            None
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
         camera = cv2.VideoCapture(self.index)
         # Index for files name 
         i = 0
         for folder in self.label:
@@ -173,125 +199,135 @@
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # Set status 
-        self.statusGray = 0
-        self.statusRGB = 1
+        self._statusGray = 0
+        self._statusRGB = 1
     
 
-    # -----------
-    # compressTrainTest
-    # -----------
-    def compress_train_test(self)->None:
+    def compress_train_test(self) -> None:
         """
-        Save the images shot in datasets divided by train and test like the mnist dataset.
+        Saves the images shot in datasets divided by train and test like the mnist dataset.
+    
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+            ValueError: If the percentage value for images in the test set is less than or equal to 0.
+    
+        Returns:
+            None
         """
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         print('\n')
         print('--- DATASET SETTING ---')
         self.perc = float(input('percentage of images in the test set (0,1): '))
         if self.perc <= 0:
             raise ValueError('percentage value must be greater than 0...')
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # y 
-        self.tensor['y'] = np.empty((0))
+        self._tensor['y'] = np.empty((0))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format  
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors 
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
-            self.tensor['y'] = np.append(self.tensor['y'], np.repeat(i, self.num, axis = 0))
+            # unique final _tensors 
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
+            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        self.tensor['y'] = self.tensor['y'].astype('uint8')
-        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.tensor['X'], self.tensor['y'], test_size=self.perc, random_state=123)
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        self._tensor['y'] = self._tensor['y'].astype('uint8')
+        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self._tensor['X'], self._tensor['y'], test_size=self.perc, random_state=123)
         np.savez('dataset.npz', X_train=self.X_train, X_test=self.X_test, y_train=self.y_train, y_test=self.y_test)
 
 
-    # -----------
-    # compressAll
-    # -----------
-    def compress_all(self)->None:
+    def compress_all(self) -> None:
         """
-        Save the images shot in a unique dataset.
+        Saves the images shot in a unique dataset.
+    
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+        
+        Returns:
+            None
         """
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # y 
-        self.tensor['y'] = np.empty((0))
+        self._tensor['y'] = np.empty((0))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save 
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors 
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
-            self.tensor['y'] = np.append(self.tensor['y'], np.repeat(i, self.num, axis = 0))
+            # unique final _tensors 
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
+            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        self.tensor['y'] = self.tensor['y'].astype('uint8')
-        np.savez('datasetall.npz', x = self.tensor['X'], y = self.tensor['y'])
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        self._tensor['y'] = self._tensor['y'].astype('uint8')
+        np.savez('datasetall.npz', x = self._tensor['X'], y = self._tensor['y'])
 
 
-    # -----------
-    # justCompress
-    # -----------
-    def just_compress(self)->None:
+    def just_compress(self) -> None:
         """
-        Save the images shot in a unique dataset without saving the y variable containing the type of the single image.
+        Saves the images shot in a unique dataset without saving the y variable containing the type of the single image.
+    
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+        
+        Returns:
+            None
         """
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # insert name for the compress file 
         print('\n')
         print('--- DATASET SETTING ---')
         name = input('Select a name for the compressed file: ')
         # check the name for the dataset 
         if len(name) == 0:
@@ -299,54 +335,51 @@
         if name == "0":
             pass
         else:
             self.name = name 
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
+            # unique final _tensors
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        np.savez(f'{self.name}.npz', x = self.tensor['X'])
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        np.savez(f'{self.name}.npz', x = self._tensor['X'])
 
 
-    # ------------------
-    # control function 
-    # ------------------
-    def var_control(self)->None:
+    def var_control(self) -> None:
         """
-        Print the parameters specified in the init method about the dataset to create.
+        Print the parameters specified in the setup method about the dataset to create.
         """
         print('\n')
         print('--- PARAMETERS CONTROL ---')
-        print(f'camera index: {self.index}')
-        print(f'labels of images types: {self.label}')
-        print(f'num. of images for types: {self.num}')
-        print(f'single frame HEIGHT: {self.height}')
-        print(f'single frame WIDTH: {self.width}')
-        print(f'waiting time between frames: {self.standby_time}')
-        print(f'percentage of images in train dataset: {self.perc}')
-        print(f'statusGray: {self.statusGray}')
-        print(f'statusRGB: {self.statusRGB}')
+        print(f'Camera index: {self.index}')
+        print(f'Labels of images types: {self.label}')
+        print(f'Num. of images for types: {self.num}')
+        print(f'Single frame HEIGHT: {self.height}')
+        print(f'Single frame WIDTH: {self.width}')
+        print(f'Waiting time between frames: {self.standby_time}')
+        print(f'Percentage of images in train dataset: {self.perc}')
+        print(f'StatusGray: {self._statusGray}')
+        print(f'StatusRGB: {self._statusRGB}')
```

### Comparing `xeye-0.36/src/xeye/__fast_dataset.py` & `xeye-0.37/src/xeye/fast_dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,70 @@
 import cv2 
 import os
 from sklearn.model_selection import train_test_split
 import numpy as np
 import time
+from typing import List
 
 
 class FastDataset:
+    """
+    A class for shooting and saving images in grayscale or RGB using OpenCV.
+
+    Attributes:
+        index (int): the index of the camera to use.
+        img_types (int): the number of types of images to collect.
+        label (List[str]): a list of strings that represent the name of the directories where the images will be saved.
+        num (int): the number of frames to capture for each image type.
+        height (int): the height of the frames to capture.
+        width (int): the width of the frames to capture.
+        standby_time (float): the time to wait before capturing each frame. 
     
-    def __init__(self, index: int, img_types: int, label: list[str], num: int, height: int, width: int, stand_by_time: float) -> None:
-    # inizialized variable
+    Examples: 
+        >>> import xeye
+        >>> # define parameters values
+        >>> index = 0
+        >>> img_types = 2
+        >>> label = ['keyboard', 'mouse']
+        >>> num = 20
+        >>> height = 100
+        >>> width = 100
+        >>> standby_time = 0
+        >>> data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
+        >>> data.preview()
+        >>> data.rgb() # or data.gray()
+        >>> data.compress_train_test(perc=0.2)
+        >>> data.compress_all()
+        >>> data.just_compress(name="batch_test")
+    """
+    def __init__(self, index: int, img_types: int, label: List[str], num: int, height: int, width: int, stand_by_time: float) -> None:
         self.index = index
         self.img_types = img_types
         self.label = label
         self.num = num
         self.height = height
         self.width = width
-        self.class_dict = {}
-        self.tensor = {}
+        self._class_dict = {}
+        self._tensor = {}
         self.standby_time = stand_by_time
-        self.statusGray = 0
-        self.statusRGB = 0
+        self._statusGray = 0
+        self._statusRGB = 0
         # clear terminal 
-        if(os.name == 'posix'): #unix
+        if(os.name == 'posix'): # unix
             os.system('clear')
-        else: #windows
+        else: # windows
             os.system('cls')
         # camera setting
         if self.index == -1:
             raise ValueError('(index) Insert valid camera index...')
         camera = cv2.VideoCapture(self.index)
         if camera.isOpened() == False:
             raise ValueError('(index) Insert valid camera index...')
         # set how many type of images do you want to collect
-        if self.img_types == 0: # informarsi sul raise error 
+        if self.img_types == 0: 
             raise ValueError('(img_types) Number of images types must be greather than 0')
         if type(self.img_types) != int:
             raise TypeError('(img_types) passed a string, not an integer')
         # folder building
         if self.label == []:
             raise ValueError('(label) Not valid names for images types...')
         if len(self.label) != self.img_types:
@@ -53,20 +81,20 @@
         if self.width == 0 or self.width < 0:
             raise ValueError('(width) Frame WIDTH must be greather than 0')
         # Waiting time in shooting loop
         if self.standby_time < 0:
             raise ValueError('(standby_time) waiting time must be grater than 0...')
 
 
-    # --------------------
-    # preview 
-    # --------------------      
-    def preview(self)->None:
+    def preview(self) -> None:
         """
-        Open the camera stream on a window. Helpful for checking the framing of the image.
+        Opens the camera stream on a window for checking the framing of the image.
+
+        Returns: 
+            None
         """
         print('\n')
         print('--- PREVIEW ---')
         camera = cv2.VideoCapture(self.index)
         while(True):
             status, frame = camera.read()
             if not status:
@@ -81,20 +109,20 @@
                 print('preview closed')
                 camera.release()
                 cv2.destroyAllWindows()
                 cv2.waitKey(1)
                 break
 
 
-    # ---------------
-    # grayscale images 
-    #----------------
-    def gray(self)->None:
+    def gray(self) -> None:
         """
-        Method for shooting images in grayscale. 
+        Method for shooting images in grayscale.
+
+        Returns:
+            None 
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
         camera = cv2.VideoCapture(self.index)
         # Index for files name 
         i = 0
         for folder in self.label:
@@ -118,24 +146,24 @@
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # set status
-        self.statusGray = 1
-        self.statusRGB = 0
+        self._statusGray = 1
+        self._statusRGB = 0
 
 
-    # -----------
-    # rgb imges
-    # -----------
-    def rgb(self)->None:
+    def rgb(self) -> None:
         """
-        Method for shooting images in RGB. 
+        Method for shooting images in RGB.
+
+        Returns:
+            None
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
         camera = cv2.VideoCapture(self.index)
         # Index for files name 
         i = 0
         for folder in self.label:
@@ -159,170 +187,183 @@
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # Set status 
-        self.statusGray = 0
-        self.statusRGB = 1
+        self._statusGray = 0
+        self._statusRGB = 1
 
 
-    # -----------
-    # compressTrainTest
-    # -----------
-    def compress_train_test(self, perc: float = 0.1)->None:
+    def compress_train_test(self, perc: float = 0.1) -> None:
         """
-        Save the images shot in datasets divided by train and test like the mnist dataset.
+        Saves the images shot in datasets divided by train and test like the mnist dataset.
+    
+        Args:
+            perc (float): The percentage of images to assign to the test dataset.
+
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+            ValueError: If the percentage value for images in the test set is less than or equal to 0.
+    
+        Returns:
+            None
         """
         # percentage control 
         if perc <= 0:
             raise ValueError('(perc) Percentage value must be greater than 0...')
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # y 
-        self.tensor['y'] = np.empty((0))
+        self._tensor['y'] = np.empty((0))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format  
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save in _tensor class 
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors 
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
-            self.tensor['y'] = np.append(self.tensor['y'], np.repeat(i, self.num, axis = 0))
+            # unique final _tensors 
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
+            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        self.tensor['y'] = self.tensor['y'].astype('uint8')
-        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self.tensor['X'], self.tensor['y'], test_size=perc, random_state=123)
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        self._tensor['y'] = self._tensor['y'].astype('uint8')
+        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self._tensor['X'], self._tensor['y'], test_size=perc, random_state=123)
         np.savez('dataset.npz', X_train=self.X_train, X_test=self.X_test, y_train=self.y_train, y_test=self.y_test)
 
 
-    # -----------
-    # compressAll
-    # -----------
-    def compress_all(self)->None:
+    def compress_all(self) -> None:
         """
-        Save the images shot in a unique dataset.
+        Saves the images shot in a unique dataset.
+    
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+        
+        Returns:
+            None
         """
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # y 
-        self.tensor['y'] = np.empty((0))
+        self._tensor['y'] = np.empty((0))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save in _tensor class 
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors 
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
-            self.tensor['y'] = np.append(self.tensor['y'], np.repeat(i, self.num, axis = 0))
+            # unique final _tensors 
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
+            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        self.tensor['y'] = self.tensor['y'].astype('uint8')
-        np.savez('datasetall.npz', x = self.tensor['X'], y = self.tensor['y'])
-
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        self._tensor['y'] = self._tensor['y'].astype('uint8')
+        np.savez('datasetall.npz', x = self._tensor['X'], y = self._tensor['y'])
 
 
-    # -----------
-    # justCompress
-    # -----------
-    def just_compress(self, name: str = "dataset_raw")->None:
+    def just_compress(self, name: str = "dataset_raw") -> None:
         """
-        Save the images shot in a unique dataset without saving the y variable containing the type of the single image.
+        Saves the images shot in a unique dataset without saving the y variable containing the type of the single image.
+
+        Args:
+            name (str): The name of the dataset (npz) to be saved.
+    
+        Raises:
+            ValueError: If both rgb and gray functions have not been called before compressing a dataset.
+        
+        Returns:
+            None
         """
         # data control
-        if self.statusRGB == 0 and self.statusGray == 0:
+        if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # check the name for the dataset 
         if len(str(name)) == 0:
             raise ValueError("name: Insert a valide name for the compressed file...")
         # index for image type 
         i = 0
         # X
-        if self.statusGray == 1:
-            self.tensor['X'] = np.empty((0,self.height,self.width))
+        if self._statusGray == 1:
+            self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
-            self.tensor['X'] = np.empty((0,self.height,self.width,3))
+            self._tensor['X'] = np.empty((0,self.height,self.width,3))
         # (append) loop 
         for lab in self.label:
             j = 0
-            if self.statusGray == 1:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if self._statusGray == 1:
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
             else:
-                self.class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self.statusGray == 1:
+                if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in tensor class 
-                self.class_dict['t'+str(i)][j] = img
+                # save in _tensor class 
+                self._class_dict['t'+str(i)][j] = img
                 j += 1
-            # unique final tensors
-            self.tensor['X'] = np.append(self.tensor['X'], self.class_dict['t'+str(i)], axis = 0)
+            # unique final _tensors
+            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
             i += 1
         # create dataset (mnist style)
-        self.tensor['X'] = self.tensor['X'].astype('uint8')
-        np.savez(f'{name}.npz', x = self.tensor['X'])
-
+        self._tensor['X'] = self._tensor['X'].astype('uint8')
+        np.savez(f'{name}.npz', x = self._tensor['X'])
 
 
-    def var_control(self)->None:
+    def var_control(self) -> None:
         """
         Print the parameters specified in the init method about the dataset to create.
         """
         print('\n')
         print('--- PARAMETERS CONTROL ---')
-        print(f'camera index: {self.index}')
-        print(f'num. of images types: {self.img_types}')
-        print(f'labels of images types: {self.label}')
-        print(f'num. of images for types: {self.num}')
-        print(f'single frame HEIGHT: {self.height}')
-        print(f'single frame WIDTH: {self.width}')
-        print(f'waiting time between frames: {self.standby_time}')
-        print(f'percentage of images in train dataset: {self.perc}')
-        print(f'statusGray: {self.statusGray}')
-        print(f'statusRGB: {self.statusRGB}')
+        print(f'Camera index: {self.index}')
+        print(f'Num. of images types: {self.img_types}')
+        print(f'Labels of images types: {self.label}')
+        print(f'Num. of images for type: {self.num}')
+        print(f'Single frame HEIGHT: {self.height}')
+        print(f'Single frame WIDTH: {self.width}')
+        print(f'Waiting time between frames: {self.standby_time}')
+        print(f'StatusGray: {self._statusGray}')
+        print(f'StatusRGB: {self._statusRGB}')
```

### Comparing `xeye-0.36/src/xeye.egg-info/PKG-INFO` & `xeye-0.37/src/xeye.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.36
+Version: 0.37
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

