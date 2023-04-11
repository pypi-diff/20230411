# Comparing `tmp/xeye-0.37.tar.gz` & `tmp/xeye-0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeye-0.37.tar", last modified: Tue Apr 11 10:16:36 2023, max compression
+gzip compressed data, was "xeye-0.38.tar", last modified: Tue Apr 11 15:32:27 2023, max compression
```

## Comparing `xeye-0.37.tar` & `xeye-0.38.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.272905 xeye-0.37/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.37/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-04-11 10:16:36.272273 xeye-0.37/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13348 2023-01-19 23:29:40.000000 xeye-0.37/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-11 07:40:11.000000 xeye-0.37/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-11 10:16:36.273087 xeye-0.37/setup.cfg
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.265690 xeye-0.37/src/
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.269623 xeye-0.37/src/xeye/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-11 07:39:23.000000 xeye-0.37/src/xeye/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.37/src/xeye/build_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14924 2023-04-11 08:53:43.000000 xeye-0.37/src/xeye/dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.37/src/xeye/fast_dataset.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.37/src/xeye/manual_dataset.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 10:16:36.271649 xeye-0.37/src/xeye.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15103 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      310 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-11 10:16:36.000000 xeye-0.37/src/xeye.egg-info/top_level.txt
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.281905 xeye-0.38/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-06-27 20:24:07.000000 xeye-0.38/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15112 2023-04-11 15:32:27.281387 xeye-0.38/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13357 2023-04-11 13:22:43.000000 xeye-0.38/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      704 2023-04-11 15:16:08.000000 xeye-0.38/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-11 15:32:27.282001 xeye-0.38/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.274474 xeye-0.38/src/
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.278746 xeye-0.38/src/xeye/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      268 2023-04-11 15:16:12.000000 xeye-0.38/src/xeye/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5924 2023-04-11 10:09:31.000000 xeye-0.38/src/xeye/build_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14287 2023-04-11 15:29:52.000000 xeye-0.38/src/xeye/dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    14881 2023-04-11 09:14:50.000000 xeye-0.38/src/xeye/fast_dataset.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4518 2023-04-11 09:52:09.000000 xeye-0.38/src/xeye/manual_dataset.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-11 15:32:27.280760 xeye-0.38/src/xeye.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    15112 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      310 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       33 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        5 2023-04-11 15:32:27.000000 xeye-0.38/src/xeye.egg-info/top_level.txt
```

### Comparing `xeye-0.37/LICENSE` & `xeye-0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `xeye-0.37/PKG-INFO` & `xeye-0.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.37
+Version: 0.38
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -76,15 +76,15 @@
 
 ```python
 data = xeye.Dataset()
 ```
 set the parameters related to the images with the **init** function
 
 ```python
-data.init()
+data.setup()
 
 ```
 the execution of this function causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
@@ -157,15 +157,15 @@
 * Train set:
   * **X_train**: matrices/tensors of every single image in the train dataset;
   * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
   * **X_test**: matrices/tensors of every single image in the test dataset;
   * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
   
-(matrices for grayscale images: [Height$\times$Width$\times$1], tensors for RGB images:[Height$\times$Width$\times$3]).
+(matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
 An alternative approach is represented by the use of the function **compress_all**
 
 ```python
 data.compress_all()
 ```
```

### Comparing `xeye-0.37/README.md` & `xeye-0.38/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 ```python
 data = xeye.Dataset()
 ```
 set the parameters related to the images with the **init** function
 
 ```python
-data.init()
+data.setup()
 
 ```
 the execution of this function causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
@@ -124,15 +124,15 @@
 * Train set:
   * **X_train**: matrices/tensors of every single image in the train dataset;
   * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
   * **X_test**: matrices/tensors of every single image in the test dataset;
   * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
   
-(matrices for grayscale images: [Height$\times$Width$\times$1], tensors for RGB images:[Height$\times$Width$\times$3]).
+(matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
 An alternative approach is represented by the use of the function **compress_all**
 
 ```python
 data.compress_all()
 ```
```

### Comparing `xeye-0.37/pyproject.toml` & `xeye-0.38/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xeye"
-version = "0.37"
+version = "0.38"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Create datasets for computer vision applications"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `xeye-0.37/src/xeye/build_dataset.py` & `xeye-0.38/src/xeye/build_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.37/src/xeye/dataset.py` & `xeye-0.38/src/xeye/fast_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,106 +1,94 @@
 import cv2 
 import os
 from sklearn.model_selection import train_test_split
 import numpy as np
 import time
+from typing import List
 
 
-class Dataset:
+class FastDataset:
     """
-    A class for collecting a dataset of images using OpenCV.
+    A class for shooting and saving images in grayscale or RGB using OpenCV.
 
     Attributes:
-        index (int): The index of the camera to be used for creating the dataset.
-        label (list): The list of names of the different types of images to be collected.
-        num (int): The number of frames to shoot for every image type.
-        height (int): The height of the individual frames.
-        width (int): The width of the individual frames.
-        standby_time (float): The number of seconds to wait between every frame.
-        perc (int): The percentage of data to use for training (the remaining will be used for validation).
-        name (str): The name of the dataset.
-
-    Examples:
+        index (int): the index of the camera to use.
+        img_types (int): the number of types of images to collect.
+        label (List[str]): a list of strings that represent the name of the directories where the images will be saved.
+        num (int): the number of frames to capture for each image type.
+        height (int): the height of the frames to capture.
+        width (int): the width of the frames to capture.
+        standby_time (float): the time to wait before capturing each frame. 
+    
+    Examples: 
         >>> import xeye
-        >>> data = xeye.Dataset()
-        >>> data.setup()
-        >>> data.var_control()
+        >>> # define parameters values
+        >>> index = 0
+        >>> img_types = 2
+        >>> label = ['keyboard', 'mouse']
+        >>> num = 20
+        >>> height = 100
+        >>> width = 100
+        >>> standby_time = 0
+        >>> data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
         >>> data.preview()
         >>> data.rgb() # or data.gray()
-        >>> data.compress_train_test()
+        >>> data.compress_train_test(perc=0.2)
         >>> data.compress_all()
-        >>> data.just.compress()
+        >>> data.just_compress(name="batch_test")
     """
-    index = 0
-    label = []
-    num = 0
-    height = 0
-    width = 0
-    _class_dict = {}
-    _tensor = {}
-    standby_time = 0
-    _statusGray = 0
-    _statusRGB = 0
-    perc = 0
-    name = "dataset_raw"
-
-
-    def setup(self) -> None:
-        """
-        Starts the terminal interface for setting up the parameters of the dataset.
-
-        Returns:
-            None
-        """
+    def __init__(self, index: int, img_types: int, label: List[str], num: int, height: int, width: int, stand_by_time: float) -> None:
+        self.index = index
+        self.img_types = img_types
+        self.label = label
+        self.num = num
+        self.height = height
+        self.width = width
+        self._class_dict = {}
+        self._tensor = {}
+        self.standby_time = stand_by_time
+        self._statusGray = 0
+        self._statusRGB = 0
         # clear terminal 
-        if(os.name == 'posix'): #unix
+        if(os.name == 'posix'): # unix
             os.system('clear')
-        else: #windows
+        else: # windows
             os.system('cls')
-        # camera setting control 
-        print('--- CAMERA SETTING ---')
-        self.index = int(input('Select the index of the camera that you want to use for creating the dataset: '))
+        # camera setting
         if self.index == -1:
-            raise ValueError('Insert valid camera index...')
+            raise ValueError('(index) Insert valid camera index...')
         camera = cv2.VideoCapture(self.index)
         if camera.isOpened() == False:
-            raise ValueError('Insert valid camera index...')
-        camera.release()
+            raise ValueError('(index) Insert valid camera index...')
         # set how many type of images do you want to collect
-        self.label = []
-        print('\n')
-        print('--- IMAGE SETTINGS ---')
-        img_types = int(input('Num. of types of images to scan: '))
-        if img_types == 0: 
-            raise ValueError('Number of images types must be greather than 0')
-        for i in range(0,img_types):
-            l = str(input(f"Name of image type ({i+1}): "))
-            self.label.append(l)
+        if self.img_types == 0: 
+            raise ValueError('(img_types) Number of images types must be greather than 0')
+        if type(self.img_types) != int:
+            raise TypeError('(img_types) passed a string, not an integer')
         # folder building
+        if self.label == []:
+            raise ValueError('(label) Not valid names for images types...')
+        if len(self.label) != self.img_types:
+            raise ValueError("(label) You must have a number of labels equal to the number of images types selected...")
         for lab in self.label:
             if not os.path.exists(lab):
                 os.mkdir(lab)
         # number of frames 
-        self.num = int(input('Num. of frames to shoot for every image type: '))
         if self.num == 0 or self.num < 0:
-            raise ValueError('You cant inizialize frames number equal or below zero...')
+            raise ValueError('(num) You cant inizialize frames number equal or below zero...')
         # Image shaping phase
-        self.height = int(input('Single frame HEIGHT: '))
         if self.height == 0 or self.height < 0:
-            raise ValueError('Frame HEIGHT must be greather than 0')
-        self.width = int(input('Single frame WIDTH: '))
+            raise ValueError('(height) Frame HEIGHT must be greather than 0')
         if self.width == 0 or self.width < 0:
-            raise ValueError('Frame WIDTH must be greather than 0')
-
+            raise ValueError('(width) Frame WIDTH must be greather than 0')
         # Waiting time in shooting loop
-        self.standby_time = float(input('num. of waiting time (in sec.) between every frame: '))
         if self.standby_time < 0:
-            raise ValueError('waiting time must be grater than 0...')
+            raise ValueError('(standby_time) waiting time must be grater than 0...')
+
 
-  
     def preview(self) -> None:
         """
         Opens the camera stream on a window for checking the framing of the image.
 
         Returns: 
             None
         """
@@ -146,15 +134,15 @@
             while count < self.num:
                 status, frame = camera.read()
                 if not status:
                     print("frame doesn't been captured")
                     break
                 gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
                 cv2.startWindowThread()
-                cv2.imshow(f"Camera View for image type [{folder}]", gray)
+                cv2.imshow(f"Camera View for image type [{folder}]",gray)
                 gray = cv2.resize(gray, (self.width, self.height))
                 cv2.imwrite(folder+'/'+ str(self.label[i]) + str(count) + '.png', gray)
                 count=count+1
                 time.sleep(self.standby_time)
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
@@ -201,35 +189,36 @@
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # Set status 
         self._statusGray = 0
         self._statusRGB = 1
-    
 
-    def compress_train_test(self) -> None:
+
+    def compress_train_test(self, perc: float = 0.1) -> None:
         """
         Saves the images shot in datasets divided by train and test like the mnist dataset.
     
+        Args:
+            perc (float): The percentage of images to assign to the test dataset.
+
         Raises:
             ValueError: If both rgb and gray functions have not been called before compressing a dataset.
             ValueError: If the percentage value for images in the test set is less than or equal to 0.
     
         Returns:
             None
         """
+        # percentage control 
+        if perc <= 0:
+            raise ValueError('(perc) Percentage value must be greater than 0...')
         # data control
         if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
-        print('\n')
-        print('--- DATASET SETTING ---')
-        self.perc = float(input('percentage of images in the test set (0,1): '))
-        if self.perc <= 0:
-            raise ValueError('percentage value must be greater than 0...')
         # index for image type 
         i = 0
         # X
         if self._statusGray == 1:
             self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
             self._tensor['X'] = np.empty((0,self.height,self.width,3))
@@ -245,25 +234,25 @@
             # loop for convert image format  
             for file in os.listdir(lab):
                 if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save
+                # save in _tensor class 
                 self._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors 
             self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
             self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
         self._tensor['X'] = self._tensor['X'].astype('uint8')
         self._tensor['y'] = self._tensor['y'].astype('uint8')
-        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self._tensor['X'], self._tensor['y'], test_size=self.perc, random_state=123)
+        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self._tensor['X'], self._tensor['y'], test_size=perc, random_state=123)
         np.savez('dataset.npz', X_train=self.X_train, X_test=self.X_test, y_train=self.y_train, y_test=self.y_test)
 
 
     def compress_all(self) -> None:
         """
         Saves the images shot in a unique dataset.
     
@@ -295,51 +284,46 @@
             # loop for convert image format
             for file in os.listdir(lab):
                 if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save 
+                # save in _tensor class 
                 self._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors 
             self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
             self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
             i += 1
         # create dataset (mnist style)
         self._tensor['X'] = self._tensor['X'].astype('uint8')
         self._tensor['y'] = self._tensor['y'].astype('uint8')
         np.savez('datasetall.npz', x = self._tensor['X'], y = self._tensor['y'])
 
 
-    def just_compress(self) -> None:
+    def just_compress(self, name: str = "dataset_raw") -> None:
         """
         Saves the images shot in a unique dataset without saving the y variable containing the type of the single image.
+
+        Args:
+            name (str): The name of the dataset (npz) to be saved.
     
         Raises:
             ValueError: If both rgb and gray functions have not been called before compressing a dataset.
         
         Returns:
             None
         """
         # data control
         if self._statusRGB == 0 and self._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
-        # insert name for the compress file 
-        print('\n')
-        print('--- DATASET SETTING ---')
-        name = input('Select a name for the compressed file: ')
         # check the name for the dataset 
-        if len(name) == 0:
-            raise ValueError("Insert a valide name for the compress file...")
-        if name == "0":
-            pass
-        else:
-            self.name = name 
+        if len(str(name)) == 0:
+            raise ValueError("name: Insert a valide name for the compressed file...")
         # index for image type 
         i = 0
         # X
         if self._statusGray == 1:
             self._tensor['X'] = np.empty((0,self.height,self.width))
         else:
             self._tensor['X'] = np.empty((0,self.height,self.width,3))
@@ -353,33 +337,33 @@
             # loop for convert image format
             for file in os.listdir(lab):
                 if self._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save
+                # save in _tensor class 
                 self._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors
             self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
             i += 1
         # create dataset (mnist style)
         self._tensor['X'] = self._tensor['X'].astype('uint8')
-        np.savez(f'{self.name}.npz', x = self._tensor['X'])
+        np.savez(f'{name}.npz', x = self._tensor['X'])
 
 
     def var_control(self) -> None:
         """
-        Print the parameters specified in the setup method about the dataset to create.
+        Print the parameters specified in the init method about the dataset to create.
         """
         print('\n')
         print('--- PARAMETERS CONTROL ---')
         print(f'Camera index: {self.index}')
+        print(f'Num. of images types: {self.img_types}')
         print(f'Labels of images types: {self.label}')
-        print(f'Num. of images for types: {self.num}')
+        print(f'Num. of images for type: {self.num}')
         print(f'Single frame HEIGHT: {self.height}')
         print(f'Single frame WIDTH: {self.width}')
         print(f'Waiting time between frames: {self.standby_time}')
-        print(f'Percentage of images in train dataset: {self.perc}')
         print(f'StatusGray: {self._statusGray}')
         print(f'StatusRGB: {self._statusRGB}')
```

### Comparing `xeye-0.37/src/xeye/fast_dataset.py` & `xeye-0.38/src/xeye/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,108 @@
 import cv2 
 import os
 from sklearn.model_selection import train_test_split
 import numpy as np
 import time
-from typing import List
 
 
-class FastDataset:
+class Dataset:
     """
-    A class for shooting and saving images in grayscale or RGB using OpenCV.
+    A class for collecting a dataset of images using OpenCV.
 
-    Attributes:
-        index (int): the index of the camera to use.
-        img_types (int): the number of types of images to collect.
-        label (List[str]): a list of strings that represent the name of the directories where the images will be saved.
-        num (int): the number of frames to capture for each image type.
-        height (int): the height of the frames to capture.
-        width (int): the width of the frames to capture.
-        standby_time (float): the time to wait before capturing each frame. 
-    
-    Examples: 
+    Examples:
         >>> import xeye
-        >>> # define parameters values
-        >>> index = 0
-        >>> img_types = 2
-        >>> label = ['keyboard', 'mouse']
-        >>> num = 20
-        >>> height = 100
-        >>> width = 100
-        >>> standby_time = 0
-        >>> data = xeye.FastDataset(index = index, img_types = img_types, label = label, num = num, height = height, width = width, stand_by_time = standby_time)
+        >>> data = xeye.Dataset()
+        >>> data.setup()
+        >>> data.var_control()
         >>> data.preview()
         >>> data.rgb() # or data.gray()
-        >>> data.compress_train_test(perc=0.2)
+        >>> data.compress_train_test()
         >>> data.compress_all()
-        >>> data.just_compress(name="batch_test")
+        >>> data.just.compress()
     """
-    def __init__(self, index: int, img_types: int, label: List[str], num: int, height: int, width: int, stand_by_time: float) -> None:
-        self.index = index
-        self.img_types = img_types
-        self.label = label
-        self.num = num
-        self.height = height
-        self.width = width
-        self._class_dict = {}
-        self._tensor = {}
-        self.standby_time = stand_by_time
-        self._statusGray = 0
-        self._statusRGB = 0
+    index = 0
+    label = []
+    num = 0
+    height = 0
+    width = 0
+    _class_dict = {}
+    _tensor = {}
+    standby_time = 0
+    _statusGray = 0
+    _statusRGB = 0
+    perc = 0
+    name = "dataset_raw"
+
+
+    @classmethod
+    def setup(cls) -> None:
+        """
+        Starts the terminal interface for setting up the parameters of the dataset.
+
+        Returns:
+            None
+        """
         # clear terminal 
-        if(os.name == 'posix'): # unix
+        if(os.name == 'posix'): #unix
             os.system('clear')
-        else: # windows
+        else: #windows
             os.system('cls')
-        # camera setting
-        if self.index == -1:
-            raise ValueError('(index) Insert valid camera index...')
-        camera = cv2.VideoCapture(self.index)
+        # camera setting control 
+        print('--- CAMERA SETTING ---')
+        cls.index = int(input('Select the index of the camera that you want to use for creating the dataset: '))
+        if cls.index == -1:
+            raise ValueError('Insert valid camera index...')
+        camera = cv2.VideoCapture(cls.index)
         if camera.isOpened() == False:
-            raise ValueError('(index) Insert valid camera index...')
+            raise ValueError('Insert valid camera index...')
+        camera.release()
         # set how many type of images do you want to collect
-        if self.img_types == 0: 
-            raise ValueError('(img_types) Number of images types must be greather than 0')
-        if type(self.img_types) != int:
-            raise TypeError('(img_types) passed a string, not an integer')
+        cls.label = []
+        print('\n')
+        print('--- IMAGE SETTINGS ---')
+        img_types = int(input('Num. of types of images to scan: '))
+        if img_types == 0: 
+            raise ValueError('Number of images types must be greather than 0')
+        for i in range(0,img_types):
+            l = str(input(f"Name of image type ({i+1}): "))
+            cls.label.append(l)
         # folder building
-        if self.label == []:
-            raise ValueError('(label) Not valid names for images types...')
-        if len(self.label) != self.img_types:
-            raise ValueError("(label) You must have a number of labels equal to the number of images types selected...")
-        for lab in self.label:
+        for lab in cls.label:
             if not os.path.exists(lab):
                 os.mkdir(lab)
         # number of frames 
-        if self.num == 0 or self.num < 0:
-            raise ValueError('(num) You cant inizialize frames number equal or below zero...')
+        cls.num = int(input('Num. of frames to shoot for every image type: '))
+        if cls.num == 0 or cls.num < 0:
+            raise ValueError('You cant inizialize frames number equal or below zero...')
         # Image shaping phase
-        if self.height == 0 or self.height < 0:
-            raise ValueError('(height) Frame HEIGHT must be greather than 0')
-        if self.width == 0 or self.width < 0:
-            raise ValueError('(width) Frame WIDTH must be greather than 0')
+        cls.height = int(input('Single frame HEIGHT: '))
+        if cls.height == 0 or cls.height < 0:
+            raise ValueError('Frame HEIGHT must be greather than 0')
+        cls.width = int(input('Single frame WIDTH: '))
+        if cls.width == 0 or cls.width < 0:
+            raise ValueError('Frame WIDTH must be greather than 0')
+
         # Waiting time in shooting loop
-        if self.standby_time < 0:
-            raise ValueError('(standby_time) waiting time must be grater than 0...')
+        cls.standby_time = float(input('num. of waiting time (in sec.) between every frame: '))
+        if cls.standby_time < 0:
+            raise ValueError('waiting time must be grater than 0...')
 
 
-    def preview(self) -> None:
+    @classmethod
+    def preview(cls) -> None:
         """
         Opens the camera stream on a window for checking the framing of the image.
 
         Returns: 
             None
         """
         print('\n')
         print('--- PREVIEW ---')
-        camera = cv2.VideoCapture(self.index)
+        camera = cv2.VideoCapture(cls.index)
         while(True):
             status, frame = camera.read()
             if not status:
                 print("frame doesn't been captured")
                 break
             font = cv2.FONT_HERSHEY_COMPLEX
             text = 'click on the image window and then press [q] on the keyboard to quit preview'
@@ -109,261 +113,271 @@
                 print('preview closed')
                 camera.release()
                 cv2.destroyAllWindows()
                 cv2.waitKey(1)
                 break
 
 
-    def gray(self) -> None:
+    @classmethod
+    def gray(cls) -> None:
         """
         Method for shooting images in grayscale.
 
         Returns:
             None 
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
-        camera = cv2.VideoCapture(self.index)
+        camera = cv2.VideoCapture(cls.index)
         # Index for files name 
         i = 0
-        for folder in self.label:
+        for folder in cls.label:
             count = 0
             print(f'Press [b] on the keyboard to start data collection of image type: [{folder}]')
             userinput = input()
             if userinput != 'b':
                 print("Wrong Input...press 'b'")
-            while count < self.num:
+            while count < cls.num:
                 status, frame = camera.read()
                 if not status:
                     print("frame doesn't been captured")
                     break
                 gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
                 cv2.startWindowThread()
-                cv2.imshow(f"Camera View for image type [{folder}]",gray)
-                gray = cv2.resize(gray, (self.width, self.height))
-                cv2.imwrite(folder+'/'+ str(self.label[i]) + str(count) + '.png', gray)
+                cv2.imshow(f"Camera View for image type [{folder}]", gray)
+                gray = cv2.resize(gray, (cls.width, cls.height))
+                cv2.imwrite(folder+'/'+ str(cls.label[i]) + str(count) + '.png', gray)
                 count=count+1
-                time.sleep(self.standby_time)
+                time.sleep(cls.standby_time)
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # set status
-        self._statusGray = 1
-        self._statusRGB = 0
+        cls._statusGray = 1
+        cls._statusRGB = 0
 
 
-    def rgb(self) -> None:
+    @classmethod
+    def rgb(cls) -> None:
         """
         Method for shooting images in RGB.
 
         Returns:
             None
         """
         print('\n')
         print('--- START TAKING PHOTOS ---')
-        camera = cv2.VideoCapture(self.index)
+        camera = cv2.VideoCapture(cls.index)
         # Index for files name 
         i = 0
-        for folder in self.label:
+        for folder in cls.label:
             count = 0
             print(f'Press [b] on the keyboard to start data collection of image type: [{folder}]')
             userinput = input()
             if userinput != 'b':
                 print("Wrong Input...press 'b'")
                 exit()
-            while count < self.num:
+            while count < cls.num:
                 status, frame = camera.read()
                 if not status:
                     print("frame doesn't been captured")
                     break
                 cv2.startWindowThread()
                 cv2.imshow(f"Camera View for image type [{folder}]", frame)
-                frame = cv2.resize(frame, (self.width, self.height))
-                cv2.imwrite(folder+'/'+ str(self.label[i]) + str(count) + '.png', frame)
+                frame = cv2.resize(frame, (cls.width, cls.height))
+                cv2.imwrite(folder+'/'+ str(cls.label[i]) + str(count) + '.png', frame)
                 count=count+1
-                time.sleep(self.standby_time)
+                time.sleep(cls.standby_time)
                 if cv2.waitKey(1) == ord('q'):
                     break
             i += 1
         camera.release()
         cv2.destroyAllWindows()
         cv2.waitKey(1)
         # Set status 
-        self._statusGray = 0
-        self._statusRGB = 1
-
+        cls._statusGray = 0
+        cls._statusRGB = 1
+    
 
-    def compress_train_test(self, perc: float = 0.1) -> None:
+    @classmethod
+    def compress_train_test(cls) -> None:
         """
         Saves the images shot in datasets divided by train and test like the mnist dataset.
     
-        Args:
-            perc (float): The percentage of images to assign to the test dataset.
-
         Raises:
             ValueError: If both rgb and gray functions have not been called before compressing a dataset.
             ValueError: If the percentage value for images in the test set is less than or equal to 0.
     
         Returns:
             None
         """
-        # percentage control 
-        if perc <= 0:
-            raise ValueError('(perc) Percentage value must be greater than 0...')
         # data control
-        if self._statusRGB == 0 and self._statusGray == 0:
+        if cls._statusRGB == 0 and cls._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
+        print('\n')
+        print('--- DATASET SETTING ---')
+        cls.perc = float(input('percentage of images in the test set (0,1): '))
+        if cls.perc <= 0:
+            raise ValueError('percentage value must be greater than 0...')
         # index for image type 
         i = 0
         # X
-        if self._statusGray == 1:
-            self._tensor['X'] = np.empty((0,self.height,self.width))
+        if cls._statusGray == 1:
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width))
         else:
-            self._tensor['X'] = np.empty((0,self.height,self.width,3))
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width,3))
         # y 
-        self._tensor['y'] = np.empty((0))
+        cls._tensor['y'] = np.empty((0))
         # (append) loop 
-        for lab in self.label:
+        for lab in cls.label:
             j = 0
-            if self._statusGray == 1:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if cls._statusGray == 1:
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width))
             else:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width, 3))
             # loop for convert image format  
             for file in os.listdir(lab):
-                if self._statusGray == 1:
+                if cls._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in _tensor class 
-                self._class_dict['t'+str(i)][j] = img
+                # save
+                cls._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors 
-            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
-            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
+            cls._tensor['X'] = np.append(cls._tensor['X'], cls._class_dict['t'+str(i)], axis = 0)
+            cls._tensor['y'] = np.append(cls._tensor['y'], np.repeat(i, cls.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self._tensor['X'] = self._tensor['X'].astype('uint8')
-        self._tensor['y'] = self._tensor['y'].astype('uint8')
-        self.X_train, self.X_test, self.y_train, self.y_test = train_test_split(self._tensor['X'], self._tensor['y'], test_size=perc, random_state=123)
-        np.savez('dataset.npz', X_train=self.X_train, X_test=self.X_test, y_train=self.y_train, y_test=self.y_test)
+        cls._tensor['X'] = cls._tensor['X'].astype('uint8')
+        cls._tensor['y'] = cls._tensor['y'].astype('uint8')
+        cls.X_train, cls.X_test, cls.y_train, cls.y_test = train_test_split(cls._tensor['X'], cls._tensor['y'], test_size=cls.perc, random_state=123)
+        np.savez('dataset.npz', X_train=cls.X_train, X_test=cls.X_test, y_train=cls.y_train, y_test=cls.y_test)
 
 
-    def compress_all(self) -> None:
+    @classmethod
+    def compress_all(cls) -> None:
         """
         Saves the images shot in a unique dataset.
     
         Raises:
             ValueError: If both rgb and gray functions have not been called before compressing a dataset.
         
         Returns:
             None
         """
         # data control
-        if self._statusRGB == 0 and self._statusGray == 0:
+        if cls._statusRGB == 0 and cls._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
         # index for image type 
         i = 0
         # X
-        if self._statusGray == 1:
-            self._tensor['X'] = np.empty((0,self.height,self.width))
+        if cls._statusGray == 1:
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width))
         else:
-            self._tensor['X'] = np.empty((0,self.height,self.width,3))
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width,3))
         # y 
-        self._tensor['y'] = np.empty((0))
+        cls._tensor['y'] = np.empty((0))
         # (append) loop 
-        for lab in self.label:
+        for lab in cls.label:
             j = 0
-            if self._statusGray == 1:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if cls._statusGray == 1:
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width))
             else:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self._statusGray == 1:
+                if cls._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in _tensor class 
-                self._class_dict['t'+str(i)][j] = img
+                # save 
+                cls._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors 
-            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
-            self._tensor['y'] = np.append(self._tensor['y'], np.repeat(i, self.num, axis = 0))
+            cls._tensor['X'] = np.append(cls._tensor['X'], cls._class_dict['t'+str(i)], axis = 0)
+            cls._tensor['y'] = np.append(cls._tensor['y'], np.repeat(i, cls.num, axis = 0))
             i += 1
         # create dataset (mnist style)
-        self._tensor['X'] = self._tensor['X'].astype('uint8')
-        self._tensor['y'] = self._tensor['y'].astype('uint8')
-        np.savez('datasetall.npz', x = self._tensor['X'], y = self._tensor['y'])
+        cls._tensor['X'] = cls._tensor['X'].astype('uint8')
+        cls._tensor['y'] = cls._tensor['y'].astype('uint8')
+        np.savez('datasetall.npz', x = cls._tensor['X'], y = cls._tensor['y'])
 
 
-    def just_compress(self, name: str = "dataset_raw") -> None:
+    @classmethod
+    def just_compress(cls) -> None:
         """
         Saves the images shot in a unique dataset without saving the y variable containing the type of the single image.
-
-        Args:
-            name (str): The name of the dataset (npz) to be saved.
     
         Raises:
             ValueError: If both rgb and gray functions have not been called before compressing a dataset.
         
         Returns:
             None
         """
         # data control
-        if self._statusRGB == 0 and self._statusGray == 0:
+        if cls._statusRGB == 0 and cls._statusGray == 0:
             raise ValueError('You have to call rgb or gray function before compress a dataset...')
+        # insert name for the compress file 
+        print('\n')
+        print('--- DATASET SETTING ---')
+        name = input('Select a name for the compressed file: ')
         # check the name for the dataset 
-        if len(str(name)) == 0:
-            raise ValueError("name: Insert a valide name for the compressed file...")
+        if len(name) == 0:
+            raise ValueError("Insert a valide name for the compress file...")
+        if name == "0":
+            pass
+        else:
+            cls.name = name 
         # index for image type 
         i = 0
         # X
-        if self._statusGray == 1:
-            self._tensor['X'] = np.empty((0,self.height,self.width))
+        if cls._statusGray == 1:
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width))
         else:
-            self._tensor['X'] = np.empty((0,self.height,self.width,3))
+            cls._tensor['X'] = np.empty((0,cls.height,cls.width,3))
         # (append) loop 
-        for lab in self.label:
+        for lab in cls.label:
             j = 0
-            if self._statusGray == 1:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width))
+            if cls._statusGray == 1:
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width))
             else:
-                self._class_dict['t'+str(i)] = np.empty((self.num, self.height, self.width, 3))
+                cls._class_dict['t'+str(i)] = np.empty((cls.num, cls.height, cls.width, 3))
             # loop for convert image format
             for file in os.listdir(lab):
-                if self._statusGray == 1:
+                if cls._statusGray == 1:
                     img = cv2.imread(lab + '/' + file, cv2.IMREAD_GRAYSCALE)
                 else:
                     img = cv2.imread(lab + '/' + file)
                     img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-                # save in _tensor class 
-                self._class_dict['t'+str(i)][j] = img
+                # save
+                cls._class_dict['t'+str(i)][j] = img
                 j += 1
             # unique final _tensors
-            self._tensor['X'] = np.append(self._tensor['X'], self._class_dict['t'+str(i)], axis = 0)
+            cls._tensor['X'] = np.append(cls._tensor['X'], cls._class_dict['t'+str(i)], axis = 0)
             i += 1
         # create dataset (mnist style)
-        self._tensor['X'] = self._tensor['X'].astype('uint8')
-        np.savez(f'{name}.npz', x = self._tensor['X'])
+        cls._tensor['X'] = cls._tensor['X'].astype('uint8')
+        np.savez(f'{cls.name}.npz', x = cls._tensor['X'])
 
 
-    def var_control(self) -> None:
+    @classmethod
+    def var_control(cls) -> None:
         """
-        Print the parameters specified in the init method about the dataset to create.
+        Print the parameters specified in the setup method about the dataset to create.
         """
         print('\n')
         print('--- PARAMETERS CONTROL ---')
-        print(f'Camera index: {self.index}')
-        print(f'Num. of images types: {self.img_types}')
-        print(f'Labels of images types: {self.label}')
-        print(f'Num. of images for type: {self.num}')
-        print(f'Single frame HEIGHT: {self.height}')
-        print(f'Single frame WIDTH: {self.width}')
-        print(f'Waiting time between frames: {self.standby_time}')
-        print(f'StatusGray: {self._statusGray}')
-        print(f'StatusRGB: {self._statusRGB}')
+        print(f'Camera index: {cls.index}')
+        print(f'Labels of images types: {cls.label}')
+        print(f'Num. of images for types: {cls.num}')
+        print(f'Single frame HEIGHT: {cls.height}')
+        print(f'Single frame WIDTH: {cls.width}')
+        print(f'Waiting time between frames: {cls.standby_time}')
+        print(f'Percentage of images in train dataset: {cls.perc}')
+        print(f'StatusGray: {cls._statusGray}')
+        print(f'StatusRGB: {cls._statusRGB}')
```

### Comparing `xeye-0.37/src/xeye/manual_dataset.py` & `xeye-0.38/src/xeye/manual_dataset.py`

 * *Files identical despite different names*

### Comparing `xeye-0.37/src/xeye.egg-info/PKG-INFO` & `xeye-0.38/src/xeye.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeye
-Version: 0.37
+Version: 0.38
 Summary: Create datasets for computer vision applications
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -76,15 +76,15 @@
 
 ```python
 data = xeye.Dataset()
 ```
 set the parameters related to the images with the **init** function
 
 ```python
-data.init()
+data.setup()
 
 ```
 the execution of this function causes the starting of the user interface in the **terminal** 
 
 
 ```console
 --- CAMERA SETTING ---
@@ -157,15 +157,15 @@
 * Train set:
   * **X_train**: matrices/tensors of every single image in the train dataset;
   * **y_train**: classes (ordinal values) are associated with every image in the train dataset.
 * Test set:
   * **X_test**: matrices/tensors of every single image in the test dataset;
   * **y_test**: classes (ordinal values) are associated with every image in the test dataset.
   
-(matrices for grayscale images: [Height$\times$Width$\times$1], tensors for RGB images:[Height$\times$Width$\times$3]).
+(matrices for grayscale images: [Height $\times$ Width $\times$ 1], tensors for RGB images:[Height $\times$ Width $\times$ 3]).
 
 An alternative approach is represented by the use of the function **compress_all**
 
 ```python
 data.compress_all()
 ```
```

