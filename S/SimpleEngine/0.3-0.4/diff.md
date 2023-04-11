# Comparing `tmp/SimpleEngine-0.3.tar.gz` & `tmp/SimpleEngine-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleEngine-0.3.tar", last modified: Tue Apr 11 00:52:10 2023, max compression
+gzip compressed data, was "SimpleEngine-0.4.tar", last modified: Tue Apr 11 14:53:37 2023, max compression
```

## Comparing `SimpleEngine-0.3.tar` & `SimpleEngine-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.617382 SimpleEngine-0.3/
--rw-rw-rw-   0        0        0      330 2023-04-11 00:51:46.000000 SimpleEngine-0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      972 2023-04-11 00:52:10.616385 SimpleEngine-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-04-11 00:46:00.000000 SimpleEngine-0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.605414 SimpleEngine-0.3/SimpleEngine/
--rw-rw-rw-   0        0        0     4249 2023-04-11 00:40:43.000000 SimpleEngine-0.3/SimpleEngine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.615387 SimpleEngine-0.3/SimpleEngine.egg-info/
--rw-rw-rw-   0        0        0      972 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 00:52:10.617382 SimpleEngine-0.3/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-04-11 00:51:09.000000 SimpleEngine-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:37.329341 SimpleEngine-0.4/
+-rw-rw-rw-   0        0        0      398 2023-04-11 14:53:24.000000 SimpleEngine-0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1040 2023-04-11 14:53:37.328344 SimpleEngine-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-04-11 00:46:00.000000 SimpleEngine-0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:37.319368 SimpleEngine-0.4/SimpleEngine/
+-rw-rw-rw-   0        0        0     4904 2023-04-11 14:51:51.000000 SimpleEngine-0.4/SimpleEngine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 14:53:37.327347 SimpleEngine-0.4/SimpleEngine.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-04-11 14:53:37.000000 SimpleEngine-0.4/SimpleEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 14:53:37.000000 SimpleEngine-0.4/SimpleEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 14:53:37.000000 SimpleEngine-0.4/SimpleEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 14:53:37.000000 SimpleEngine-0.4/SimpleEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 14:53:37.000000 SimpleEngine-0.4/SimpleEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 14:53:37.329341 SimpleEngine-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-04-11 14:53:30.000000 SimpleEngine-0.4/setup.py
```

### Comparing `SimpleEngine-0.3/LICENCE.txt` & `SimpleEngine-0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `SimpleEngine-0.3/PKG-INFO` & `SimpleEngine-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.3
+Version: 0.4
 Summary: A simple game engine
 Home-page: 
 Author: Gust Schadron
 Author-email: gustscd@gmail.com
 License: MIT
 Keywords: game
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,8 +27,12 @@
 - added move() function to objects
 - added collisionCheck() function
 - added GetKeysPressed() function
 ----------------
 0.3 (11/4/2023)
 ----------------
 - added drawHitbox() function to objects
+----------------
+0.4 (11/4/2023)
+----------------
+- added text 
 License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.3/SimpleEngine/__init__.py` & `SimpleEngine-0.4/SimpleEngine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,8 +130,29 @@
 def updateScreen():
     pygame.display.update()
 
 def collisionCheck(rect1, rect2):
     return pygame.Rect.colliderect(rect1, rect2)
 
 def GetKeysPressed():
-    return pygame.key.get_pressed()
+    return pygame.key.get_pressed()
+
+def text(text, x, y, font, size,color=WHITE):
+    font = pygame.font.Font(font, size)
+    img = font.render(text, True, color)
+
+class Text():
+    def __init__(self, x, y, text,size, font, color, screen):
+        self.size = size
+        self.font = font
+        self.x = x
+        self.y = y
+        self.color = color
+        self.hitbox
+        self.screen = screen
+    
+    def draw(self):
+        font = pygame.font.Font(self.font, self.size)
+        text = font.render(self.text, True, self.color)
+        self.hitbox = text.get_rect()
+        self.hitbox.center = (self.x, self.y)
+        self.screen.blit(text, self.hitbox)
```

### Comparing `SimpleEngine-0.3/SimpleEngine.egg-info/PKG-INFO` & `SimpleEngine-0.4/SimpleEngine.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.3
+Version: 0.4
 Summary: A simple game engine
 Home-page: 
 Author: Gust Schadron
 Author-email: gustscd@gmail.com
 License: MIT
 Keywords: game
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,8 +27,12 @@
 - added move() function to objects
 - added collisionCheck() function
 - added GetKeysPressed() function
 ----------------
 0.3 (11/4/2023)
 ----------------
 - added drawHitbox() function to objects
+----------------
+0.4 (11/4/2023)
+----------------
+- added text 
 License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.3/setup.py` & `SimpleEngine-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SimpleEngine',
-  version='0.3',
+  version='0.4',
   description='A simple game engine',
   long_description_content_type=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Gust Schadron',
   author_email='gustscd@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

