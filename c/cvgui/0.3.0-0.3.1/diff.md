# Comparing `tmp/cvgui-0.3.0.tar.gz` & `tmp/cvgui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvgui-0.3.0.tar", last modified: Fri Apr  7 16:51:00 2023, max compression
+gzip compressed data, was "cvgui-0.3.1.tar", last modified: Tue Apr 11 19:00:47 2023, max compression
```

## Comparing `cvgui-0.3.0.tar` & `cvgui-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.734373 cvgui-0.3.0/
--rw-rw-rw-   0        0        0     1094 2023-03-28 14:37:35.000000 cvgui-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      386 2023-04-07 16:51:00.734373 cvgui-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2897 2023-04-07 16:50:32.000000 cvgui-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.678373 cvgui-0.3.0/cvgui/
--rw-rw-rw-   0        0        0      376 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.705374 cvgui-0.3.0/cvgui/activity/
--rw-rw-rw-   0        0        0      494 2023-03-28 14:37:35.000000 cvgui-0.3.0/cvgui/activity/__init__.py
--rw-rw-rw-   0        0        0     6826 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/activity/activity.py
--rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/activity/scene.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.706376 cvgui-0.3.0/cvgui/core/
--rw-rw-rw-   0        0        0      889 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.710372 cvgui-0.3.0/cvgui/core/displaying/
--rw-rw-rw-   0        0        0      356 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/__init__.py
--rw-rw-rw-   0        0        0     7695 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/components.py
--rw-rw-rw-   0        0        0     2857 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/displaying/service.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.713372 cvgui-0.3.0/cvgui/core/logging/
--rw-rw-rw-   0        0        0      252 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/logging/__init__.py
--rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/logging/service.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.715372 cvgui-0.3.0/cvgui/core/receiving/
--rw-rw-rw-   0        0        0      370 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/receiving/__init__.py
--rw-rw-rw-   0        0        0     3508 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/core/receiving/service.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.716376 cvgui-0.3.0/cvgui/inputs/
--rw-rw-rw-   0        0        0      148 2023-03-28 14:37:35.000000 cvgui-0.3.0/cvgui/inputs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.719375 cvgui-0.3.0/cvgui/inputs/computer_vision/
--rw-rw-rw-   0        0        0      400 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/__init__.py
--rw-rw-rw-   0        0        0     3557 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.721373 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/
--rw-rw-rw-   0        0        0      103 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/__init__.py
--rw-rw-rw-   0        0        0     3422 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/blazepose.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.724373 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/
--rw-rw-rw-   0        0        0       78 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/__init__.py
--rw-rw-rw-   0        0        0     1495 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/webcam.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.725374 cvgui-0.3.0/cvgui/outputs/
--rw-rw-rw-   0        0        0      133 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.728374 cvgui-0.3.0/cvgui/outputs/loggers/
--rw-rw-rw-   0        0        0      178 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/loggers/__init__.py
--rw-rw-rw-   0        0        0     3809 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/outputs/loggers/csv_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.729373 cvgui-0.3.0/cvgui/user_interface/
--rw-rw-rw-   0        0        0      190 2023-04-07 15:07:31.000000 cvgui-0.3.0/cvgui/user_interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.732373 cvgui-0.3.0/cvgui/user_interface/pygame_ui/
--rw-rw-rw-   0        0        0      150 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/user_interface/pygame_ui/__init__.py
--rw-rw-rw-   0        0        0     8951 2023-04-07 16:50:32.000000 cvgui-0.3.0/cvgui/user_interface/pygame_ui/pygame.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:51:00.701375 cvgui-0.3.0/cvgui.egg-info/
--rw-rw-rw-   0        0        0      386 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1064 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-07 16:51:00.000000 cvgui-0.3.0/cvgui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-07 16:51:00.735375 cvgui-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-07 16:50:32.000000 cvgui-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.233363 cvgui-0.3.1/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 14:37:35.000000 cvgui-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      386 2023-04-11 19:00:47.233363 cvgui-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-04-07 16:50:32.000000 cvgui-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.184364 cvgui-0.3.1/cvgui/
+-rw-rw-rw-   0        0        0      376 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.207364 cvgui-0.3.1/cvgui/activity/
+-rw-rw-rw-   0        0        0      494 2023-03-28 14:37:35.000000 cvgui-0.3.1/cvgui/activity/__init__.py
+-rw-rw-rw-   0        0        0     6826 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/activity/activity.py
+-rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/activity/scene.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.208363 cvgui-0.3.1/cvgui/core/
+-rw-rw-rw-   0        0        0      889 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.211362 cvgui-0.3.1/cvgui/core/displaying/
+-rw-rw-rw-   0        0        0      356 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/displaying/__init__.py
+-rw-rw-rw-   0        0        0     7695 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/displaying/components.py
+-rw-rw-rw-   0        0        0     2857 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/displaying/service.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.213362 cvgui-0.3.1/cvgui/core/logging/
+-rw-rw-rw-   0        0        0      252 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/logging/__init__.py
+-rw-rw-rw-   0        0        0      831 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/logging/service.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.216362 cvgui-0.3.1/cvgui/core/receiving/
+-rw-rw-rw-   0        0        0      370 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/receiving/__init__.py
+-rw-rw-rw-   0        0        0     3508 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/core/receiving/service.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.217364 cvgui-0.3.1/cvgui/inputs/
+-rw-rw-rw-   0        0        0      148 2023-03-28 14:37:35.000000 cvgui-0.3.1/cvgui/inputs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.219361 cvgui-0.3.1/cvgui/inputs/computer_vision/
+-rw-rw-rw-   0        0        0      400 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/__init__.py
+-rw-rw-rw-   0        0        0     3557 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.222362 cvgui-0.3.1/cvgui/inputs/computer_vision/cv_model/
+-rw-rw-rw-   0        0        0      103 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/cv_model/__init__.py
+-rw-rw-rw-   0        0        0     3422 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/cv_model/blazepose.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.224362 cvgui-0.3.1/cvgui/inputs/computer_vision/frame_input/
+-rw-rw-rw-   0        0        0       78 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/frame_input/__init__.py
+-rw-rw-rw-   0        0        0     1510 2023-04-11 19:00:38.000000 cvgui-0.3.1/cvgui/inputs/computer_vision/frame_input/webcam.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.225365 cvgui-0.3.1/cvgui/outputs/
+-rw-rw-rw-   0        0        0      133 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/outputs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.228364 cvgui-0.3.1/cvgui/outputs/loggers/
+-rw-rw-rw-   0        0        0      178 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/outputs/loggers/__init__.py
+-rw-rw-rw-   0        0        0     3809 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/outputs/loggers/csv_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.229364 cvgui-0.3.1/cvgui/user_interface/
+-rw-rw-rw-   0        0        0      190 2023-04-07 15:07:31.000000 cvgui-0.3.1/cvgui/user_interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.231363 cvgui-0.3.1/cvgui/user_interface/pygame_ui/
+-rw-rw-rw-   0        0        0      150 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/user_interface/pygame_ui/__init__.py
+-rw-rw-rw-   0        0        0     8951 2023-04-07 16:50:32.000000 cvgui-0.3.1/cvgui/user_interface/pygame_ui/pygame.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:00:47.203362 cvgui-0.3.1/cvgui.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-04-11 19:00:46.000000 cvgui-0.3.1/cvgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2023-04-11 19:00:46.000000 cvgui-0.3.1/cvgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:00:46.000000 cvgui-0.3.1/cvgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-11 19:00:46.000000 cvgui-0.3.1/cvgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 19:00:46.000000 cvgui-0.3.1/cvgui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-11 19:00:47.235363 cvgui-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-11 19:00:38.000000 cvgui-0.3.1/setup.py
```

### Comparing `cvgui-0.3.0/LICENSE.txt` & `cvgui-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/README.md` & `cvgui-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/activity/activity.py` & `cvgui-0.3.1/cvgui/activity/activity.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/activity/scene.py` & `cvgui-0.3.1/cvgui/activity/scene.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/core/__init__.py` & `cvgui-0.3.1/cvgui/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/core/displaying/components.py` & `cvgui-0.3.1/cvgui/core/displaying/components.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/core/displaying/service.py` & `cvgui-0.3.1/cvgui/core/displaying/service.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/core/logging/service.py` & `cvgui-0.3.1/cvgui/core/logging/service.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/core/receiving/service.py` & `cvgui-0.3.1/cvgui/core/receiving/service.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/inputs/computer_vision/computer_vision.py` & `cvgui-0.3.1/cvgui/inputs/computer_vision/computer_vision.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/inputs/computer_vision/cv_model/blazepose.py` & `cvgui-0.3.1/cvgui/inputs/computer_vision/cv_model/blazepose.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/inputs/computer_vision/frame_input/webcam.py` & `cvgui-0.3.1/cvgui/inputs/computer_vision/frame_input/webcam.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def _configure(self) -> None:
         """
         Create and configures the capture object.
 
         This cannot be done in the init function because of how \
         Windows handles multiprocessing.
         """
-        self.cap = cv2.VideoCapture(self.device_num)
+        self.cap = cv2.VideoCapture(self.device_num, cv2.CAP_DSHOW)
         self.cap.set(cv2.CAP_PROP_FPS, self.fps)
         self.cap.set(cv2.CAP_PROP_FOURCC,
                      cv2.VideoWriter_fourcc("M", "J", "P", "G"))
 
     def get_frame(self) -> np.ndarray:
         """Get a frame from the webcam."""
         if self.cap is None:
```

### Comparing `cvgui-0.3.0/cvgui/outputs/loggers/csv_logger.py` & `cvgui-0.3.1/cvgui/outputs/loggers/csv_logger.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui/user_interface/pygame_ui/pygame.py` & `cvgui-0.3.1/cvgui/user_interface/pygame_ui/pygame.py`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/cvgui.egg-info/SOURCES.txt` & `cvgui-0.3.1/cvgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvgui-0.3.0/setup.py` & `cvgui-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 NAME = "cvgui"
 DESCRIPTION = "A library for creating body-interactive guis using computer vision."
 URL = "https://github.com/mitchellss/cvgui"
 EMAIL = "stephen.mitchell2299@gmail.com"
 AUTHOR = "Stephen Mitchell"
 REQUIRES_PYTHON = ">=3.9"
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 REQUIRED = [
     "mediapipe>=0.8.7.2",
     "numpy>=1.21.2",
     "opencv_python>=4.3.0.38",
     "typing_extensions>=4.3.0",
     "pygame>=2.0.0"
```

