# Comparing `tmp/CircleBlock-1.0.7.tar.gz` & `tmp/circleblock-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.7.tar", last modified: Sun Apr  9 17:09:26 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.8.tar", last modified: Mon Apr 10 04:38:04 2023, max compression
```

## Comparing `CircleBlock-1.0.7.tar` & `circleblock-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.560352 CircleBlock-1.0.7/
--rw-r--r--   0 phil       (501) staff       (20)      411 2023-04-09 17:08:56.000000 CircleBlock-1.0.7/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.559402 CircleBlock-1.0.7/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       57 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       12 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.7/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 17:08:22.000000 CircleBlock-1.0.7/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 17:09:26.560139 CircleBlock-1.0.7/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.7/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.559945 CircleBlock-1.0.7/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 17:05:19.000000 CircleBlock-1.0.7/circleblock/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4729 2023-04-09 16:45:25.000000 CircleBlock-1.0.7/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3120 2023-04-09 17:08:08.000000 CircleBlock-1.0.7/circleblock/circleblock_cli.py
--rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.7/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 17:09:26.560398 CircleBlock-1.0.7/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1033 2023-04-09 17:08:51.000000 CircleBlock-1.0.7/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-10 04:38:04.350747 CircleBlock-1.0.8/
+-rw-r--r--   0 phil       (501) staff       (20)      465 2023-04-09 23:43:17.000000 CircleBlock-1.0.8/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-10 04:38:04.350084 CircleBlock-1.0.8/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      352 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       26 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       12 2023-04-10 04:38:04.000000 CircleBlock-1.0.8/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 23:37:41.000000 CircleBlock-1.0.8/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      179 2023-04-10 01:25:56.000000 CircleBlock-1.0.8/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-10 04:38:04.350613 CircleBlock-1.0.8/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2730 2023-04-10 00:37:06.000000 CircleBlock-1.0.8/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-10 04:38:04.350437 CircleBlock-1.0.8/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-10 04:24:40.000000 CircleBlock-1.0.8/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4729 2023-04-09 23:37:41.000000 CircleBlock-1.0.8/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)      956 2023-04-10 00:30:14.000000 CircleBlock-1.0.8/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)     3254 2023-04-10 04:17:15.000000 CircleBlock-1.0.8/circleblock_cli.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-10 04:38:04.350798 CircleBlock-1.0.8/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1061 2023-04-10 04:01:17.000000 CircleBlock-1.0.8/setup.py
```

### Comparing `CircleBlock-1.0.7/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.8/CircleBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.7/LICENSE` & `CircleBlock-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.7/PKG-INFO` & `CircleBlock-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.7/README.md` & `CircleBlock-1.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 <div style="display: flex; justify-content: center;">
   <img src="images/logo.png" alt="CircleBlock Logo">
 
 </div>
 <div style="display: flex; justify-content: center;">
     <h1>CircleBlock</h1>
+
 </div>
 
 CircleBlock is a class that monitors the file system in the project root directory. This class detects changes in the file system and automatically updates the exportable functions of each module in each package's `__init__.py` file.
 
-[한국어로 읽기](./README.ko.md)
+[![English](https://img.shields.io/badge/language-English-orange.svg)](README.md) [![Korean](https://img.shields.io/badge/language-Korean-blue.svg)](README.ko.md)
 
 ## Features
 
 1. Start/stop file system monitoring
 2. Get a list of exportable functions within a module
 3. Initialize and update all `__init__.py` files in a directory
 
 ## Installation
 
 To install CircleBlock, use the following command:
 
 ```
-pip install circleblock
+pipenv install circleblock
 ```
 
 ## Usage (CLI)
 
 ### Start monitoring
 
 To start monitoring the file system, use the following command:
```

### Comparing `CircleBlock-1.0.7/circleblock/changer.py` & `CircleBlock-1.0.8/circleblock/changer.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.7/circleblock/watcher.py` & `CircleBlock-1.0.8/circleblock/watcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 class FileWatcher:
     def __init__(self, project_root: str, changer=None):
         self.project_root = project_root
         self.changer = changer
         self.observer = Observer()
 
-    def start_watching(self):
+    def start(self):
         """
         변경 사항을 감시하기 위해 루트 디렉토리를 감시하고 circleblock_cli.py 파일을 생성/업데이트합니다.
         """
         typer.echo(f'변경 사항 감시 시작...')
         typer.echo(f'프로젝트 루트: {self.project_root}')
 
         self.observer.schedule(self.changer, self.project_root, recursive=True)
         self.observer.start()
-        signal.signal(signal.SIGINT, lambda *args, **kwargs: self.stop_watching())
+        signal.signal(signal.SIGINT, lambda *args, **kwargs: self.stop())
         signal.pause()
 
-    def stop_watching(self):
+    def stop(self):
         """
         변경 사항을 감지하는 루트 디렉토리의 감시를 중지합니다.
         """
         self.observer.stop()
         self.observer.join()
```

### Comparing `CircleBlock-1.0.7/setup.py` & `CircleBlock-1.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.7',
+    version='1.0.8',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
         'typer',
-        'daemonize'
+        'daemonocle'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
@@ -24,11 +24,13 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=circleblock.circleblock_cli:app'
+            'ccbk=circleblock_cli:cli'
         ]
     }
 )
+# pipenv install -e .
+# pipenv run ccbk
```

