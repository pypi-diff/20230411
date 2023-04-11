# Comparing `tmp/SimpleEngine-0.2.tar.gz` & `tmp/SimpleEngine-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleEngine-0.2.tar", last modified: Mon Apr 10 22:57:16 2023, max compression
+gzip compressed data, was "SimpleEngine-0.3.tar", last modified: Tue Apr 11 00:52:10 2023, max compression
```

## Comparing `SimpleEngine-0.2.tar` & `SimpleEngine-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.302839 SimpleEngine-0.2/
--rw-rw-rw-   0        0        0      235 2023-04-10 22:46:36.000000 SimpleEngine-0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      875 2023-04-10 22:57:16.301842 SimpleEngine-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-04-10 22:53:34.000000 SimpleEngine-0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.290872 SimpleEngine-0.2/SimpleEngine/
--rw-rw-rw-   0        0        0     4107 2023-04-10 22:41:36.000000 SimpleEngine-0.2/SimpleEngine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.300844 SimpleEngine-0.2/SimpleEngine.egg-info/
--rw-rw-rw-   0        0        0      875 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:57:16.302839 SimpleEngine-0.2/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-04-10 22:56:58.000000 SimpleEngine-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.617382 SimpleEngine-0.3/
+-rw-rw-rw-   0        0        0      330 2023-04-11 00:51:46.000000 SimpleEngine-0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      972 2023-04-11 00:52:10.616385 SimpleEngine-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-04-11 00:46:00.000000 SimpleEngine-0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.605414 SimpleEngine-0.3/SimpleEngine/
+-rw-rw-rw-   0        0        0     4249 2023-04-11 00:40:43.000000 SimpleEngine-0.3/SimpleEngine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:52:10.615387 SimpleEngine-0.3/SimpleEngine.egg-info/
+-rw-rw-rw-   0        0        0      972 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 00:52:10.000000 SimpleEngine-0.3/SimpleEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 00:52:10.617382 SimpleEngine-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-04-11 00:51:09.000000 SimpleEngine-0.3/setup.py
```

### Comparing `SimpleEngine-0.2/LICENCE.txt` & `SimpleEngine-0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `SimpleEngine-0.2/PKG-INFO` & `SimpleEngine-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.2
+Version: 0.3
 Summary: A simple game engine
 Home-page: 
 Author: Gust Schadron
 Author-email: gustscd@gmail.com
 License: MIT
 Keywords: game
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
 
+
 Change Log
 ==========
 
 0.1 (10/4/2023)
 ----------------
 - First release
 ----------------
 0.2 (11/4/2023)
 ----------------
 - added move() function to objects
 - added collisionCheck() function
 - added GetKeysPressed() function
+----------------
+0.3 (11/4/2023)
+----------------
+- added drawHitbox() function to objects
 License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.2/SimpleEngine/__init__.py` & `SimpleEngine-0.3/SimpleEngine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     def move(self, x, y):
         self.x += x
         self.y += y
     
     def draw(self, clr=WHITE):
         self.hitbox = pygame.Rect(self.x-(self.width/2), self.y-(self.height/2), self.width, self.height)
         pygame.draw.rect(self.screen, clr, self.hitbox)
+    
+    def drawHitbox(self):
         pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Circle():
     def __init__(self, x, y, radius, screen):
         self.x = x
         self.y = y
         self.radius = radius
@@ -57,14 +59,17 @@
     def move(self, x, y):
         self.x += x
         self.y += y
     
     def draw(self, clr=WHITE):
         self.hitbox = pygame.Rect(self.x-self.radius, self.y-self.radius, self.radius*2, self.radius*2)
         pygame.draw.circle(self.screen, clr, (self.x, self.y), self.radius)
+        
+    
+    def drawHitbox(self):
         pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Triangle():
     def __init__(self, x, y, width, height, screen):
         self.width = width
         self.height = height
         self.screen = screen
@@ -85,14 +90,16 @@
         self.x3 += x+(self.width/2)
         self.y3 += y+(self.height/2)
 
 
     def draw(self, clr=WHITE):
         self.hitbox = pygame.Rect(self.x1-(self.width/2), self.y1, self.width, self.height)
         pygame.draw.polygon( self.screen, clr, ((self.x1, self.y1), (self.x2, self.y2), (self.x3, self.y3)) )
+    
+    def drawHitbox(self):
         pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Sprite(pygame.sprite.Sprite):
     def __init__(self, x, y, screen,image):
         super().__init__()
         self.x = x
         self.y = y
@@ -104,14 +111,16 @@
     def move(self, x, y):
         self.x += x
         self.y += y
 
     def draw(self):
         self.hitbox = pygame.Rect(self.x-(Image.open(self.img).width/2), self.y-(Image.open(self.img).height/2), Image.open(self.img).width, Image.open(self.img).height)
         self.screen.blit(self.image, (self.x-(Image.open(self.img).width/2), self.y-(Image.open(self.img).height/2)))
+    
+    def drawHitbox(self):
         pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 def createWindow(width, height, name):
     screen = pygame.display.set_mode((width, height))
     pygame.display.set_caption(name)
     return screen
```

### Comparing `SimpleEngine-0.2/SimpleEngine.egg-info/PKG-INFO` & `SimpleEngine-0.3/SimpleEngine.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.2
+Version: 0.3
 Summary: A simple game engine
 Home-page: 
 Author: Gust Schadron
 Author-email: gustscd@gmail.com
 License: MIT
 Keywords: game
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
 
+
 Change Log
 ==========
 
 0.1 (10/4/2023)
 ----------------
 - First release
 ----------------
 0.2 (11/4/2023)
 ----------------
 - added move() function to objects
 - added collisionCheck() function
 - added GetKeysPressed() function
+----------------
+0.3 (11/4/2023)
+----------------
+- added drawHitbox() function to objects
 License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.2/setup.py` & `SimpleEngine-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SimpleEngine',
-  version='0.2',
+  version='0.3',
   description='A simple game engine',
   long_description_content_type=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Gust Schadron',
   author_email='gustscd@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='game', 
   packages=find_packages(),
-  install_requires=['pygame', 'pillow'] 
+  install_requires=['pygame', 'pillow']
 )
```

