# Comparing `tmp/SimpleEngine-0.1.tar.gz` & `tmp/SimpleEngine-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleEngine-0.1.tar", last modified: Mon Apr 10 17:35:22 2023, max compression
+gzip compressed data, was "SimpleEngine-0.2.tar", last modified: Mon Apr 10 22:57:16 2023, max compression
```

## Comparing `SimpleEngine-0.1.tar` & `SimpleEngine-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:35:22.806955 SimpleEngine-0.1/
--rw-rw-rw-   0        0        0       76 2023-04-10 17:26:26.000000 SimpleEngine-0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      692 2023-04-10 17:35:22.806955 SimpleEngine-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-04-10 17:30:17.000000 SimpleEngine-0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 17:35:22.790998 SimpleEngine-0.1/SimpleEngine/
--rw-rw-rw-   0        0        0     2335 2023-04-10 17:21:55.000000 SimpleEngine-0.1/SimpleEngine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:35:22.805957 SimpleEngine-0.1/SimpleEngine.egg-info/
--rw-rw-rw-   0        0        0      692 2023-04-10 17:35:22.000000 SimpleEngine-0.1/SimpleEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-04-10 17:35:22.000000 SimpleEngine-0.1/SimpleEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:35:22.000000 SimpleEngine-0.1/SimpleEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 17:35:22.000000 SimpleEngine-0.1/SimpleEngine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 17:35:22.000000 SimpleEngine-0.1/SimpleEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 17:35:22.807953 SimpleEngine-0.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-10 17:31:13.000000 SimpleEngine-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.302839 SimpleEngine-0.2/
+-rw-rw-rw-   0        0        0      235 2023-04-10 22:46:36.000000 SimpleEngine-0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-04-10 17:28:33.000000 SimpleEngine-0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 17:28:35.000000 SimpleEngine-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      875 2023-04-10 22:57:16.301842 SimpleEngine-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-04-10 22:53:34.000000 SimpleEngine-0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.290872 SimpleEngine-0.2/SimpleEngine/
+-rw-rw-rw-   0        0        0     4107 2023-04-10 22:41:36.000000 SimpleEngine-0.2/SimpleEngine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:57:16.300844 SimpleEngine-0.2/SimpleEngine.egg-info/
+-rw-rw-rw-   0        0        0      875 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-10 22:57:16.000000 SimpleEngine-0.2/SimpleEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 22:57:16.302839 SimpleEngine-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      710 2023-04-10 22:56:58.000000 SimpleEngine-0.2/setup.py
```

### Comparing `SimpleEngine-0.1/LICENCE.txt` & `SimpleEngine-0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `SimpleEngine-0.1/PKG-INFO` & `SimpleEngine-0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.1
+Version: 0.2
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
-License-File: LICENCE.txt
-
-SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
+Description-Content-Type: SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
 
 Change Log
 ==========
 
 0.1 (10/4/2023)
 ----------------
 - First release
+----------------
+0.2 (11/4/2023)
+----------------
+- added move() function to objects
+- added collisionCheck() function
+- added GetKeysPressed() function
+License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.1/SimpleEngine/__init__.py` & `SimpleEngine-0.2/SimpleEngine/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,128 @@
 import pygame
+from PIL import Image
 
 WHITE = (255, 255, 255)
 BLACK = (0,0,0)
 RED = (255,0,0)
 GREEN = (0,255,0)
 BLUE = (0,0,255)
 YELLOW = (255,255,0)
 CYAN = (0,255,255)
 MAGENTA = (255,0,255)
 GRAY = (128,128,128)
 
+keyPressed = ""
 
 def StartGame(update, start):
     start()
     setFPS()
     running = True
     while running:
-        update()
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
+        keyPressed = pygame.key.get_pressed()
+        update()
     
 def setFPS(fps=30):
     clock = pygame.time.Clock()
     clock.tick(fps)
     
-    
-
 class Rect():
     def __init__(self, x, y, width, height, screen):
         self.x = x
         self.y = y
         self.width = width
         self.height = height
         self.screen = screen
+        self.hitbox = pygame.Rect(self.x-(self.width/2), self.y-(self.height/2), self.width, self.height)
     
-    def draw(self, x, y, clr=WHITE):
-        rect = pygame.Rect(self.x, self.y, self.width, self.height)
-        pygame.draw.rect(self.screen, clr, rect)
+    def move(self, x, y):
+        self.x += x
+        self.y += y
+    
+    def draw(self, clr=WHITE):
+        self.hitbox = pygame.Rect(self.x-(self.width/2), self.y-(self.height/2), self.width, self.height)
+        pygame.draw.rect(self.screen, clr, self.hitbox)
+        pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Circle():
     def __init__(self, x, y, radius, screen):
         self.x = x
         self.y = y
         self.radius = radius
         self.screen = screen
+        self.hitbox = pygame.Rect(self.x-self.radius, self.y-self.radius, self.radius*2, self.radius*2)
     
-    def draw(self, x, y, clr=WHITE):
+    def move(self, x, y):
+        self.x += x
+        self.y += y
+    
+    def draw(self, clr=WHITE):
+        self.hitbox = pygame.Rect(self.x-self.radius, self.y-self.radius, self.radius*2, self.radius*2)
         pygame.draw.circle(self.screen, clr, (self.x, self.y), self.radius)
+        pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Triangle():
     def __init__(self, x, y, width, height, screen):
         self.width = width
         self.height = height
         self.screen = screen
-        self.updatePosition(x, y)
-    
-    def updatePosition(self, x, y):
-        self.x1 = x
-        self.y1 = y-(self.height/2)
-        self.x2 = x-(self.width/2)
-        self.y2 = y+(self.height/2)
-        self.x3 = x+(self.width/2)
-        self.y3 = y+(self.height/2)
+        self.hitbox = pygame.Rect(self.x1, self.y1, self.width, self.height)
+        self.x1 = 0
+        self.x2 = 0
+        self.y1 = 0
+        self.y2 = 0
+        self.x3 = 0
+        self.y3 = 0
+        self.move(x, y)
+    
+    def move(self, x, y):
+        self.x1 += x
+        self.y1 += y-(self.height/2)
+        self.x2 += x-(self.width/2)
+        self.y2 += y+(self.height/2)
+        self.x3 += x+(self.width/2)
+        self.y3 += y+(self.height/2)
+
 
-    def draw(self, x, y, clr=WHITE):
-        self.updatePosition(x, y)
+    def draw(self, clr=WHITE):
+        self.hitbox = pygame.Rect(self.x1-(self.width/2), self.y1, self.width, self.height)
         pygame.draw.polygon( self.screen, clr, ((self.x1, self.y1), (self.x2, self.y2), (self.x3, self.y3)) )
+        pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 class Sprite(pygame.sprite.Sprite):
     def __init__(self, x, y, screen,image):
         super().__init__()
         self.x = x
         self.y = y
+        self.img = image
         self.image = pygame.image.load(image)
+        self.hitbox = pygame.Rect(self.x-(Image.open(self.img).width/2), self.y-(Image.open(self.img).height/2), Image.open(self.img).width, Image.open(self.img).height)
         self.screen = screen
-    
+
+    def move(self, x, y):
+        self.x += x
+        self.y += y
+
     def draw(self):
-        self.screen.blit(self.image, (self.x, self.y))
+        self.hitbox = pygame.Rect(self.x-(Image.open(self.img).width/2), self.y-(Image.open(self.img).height/2), Image.open(self.img).width, Image.open(self.img).height)
+        self.screen.blit(self.image, (self.x-(Image.open(self.img).width/2), self.y-(Image.open(self.img).height/2)))
+        pygame.draw.rect(self.screen, GREEN, self.hitbox,  2)
 
 def createWindow(width, height, name):
     screen = pygame.display.set_mode((width, height))
     pygame.display.set_caption(name)
     return screen
 
 def fillScreen(screen, color):
     screen.fill(color)
+
+def updateScreen():
+    pygame.display.update()
+
+def collisionCheck(rect1, rect2):
+    return pygame.Rect.colliderect(rect1, rect2)
+
+def GetKeysPressed():
+    return pygame.key.get_pressed()
```

### Comparing `SimpleEngine-0.1/SimpleEngine.egg-info/PKG-INFO` & `SimpleEngine-0.2/SimpleEngine.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: SimpleEngine
-Version: 0.1
+Version: 0.2
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
-License-File: LICENCE.txt
-
-SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
+Description-Content-Type: SimpleEngine is a simple game engine build on pygame, it can be used to create a window, draw simple shapes and draw sprites
 
 Change Log
 ==========
 
 0.1 (10/4/2023)
 ----------------
 - First release
+----------------
+0.2 (11/4/2023)
+----------------
+- added move() function to objects
+- added collisionCheck() function
+- added GetKeysPressed() function
+License-File: LICENCE.txt
```

### Comparing `SimpleEngine-0.1/setup.py` & `SimpleEngine-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='SimpleEngine',
-  version='0.1',
+  version='0.2',
   description='A simple game engine',
-  long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  long_description_content_type=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Gust Schadron',
   author_email='gustscd@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='game', 
   packages=find_packages(),
-  install_requires=['pygame'] 
+  install_requires=['pygame', 'pillow'] 
 )
```

