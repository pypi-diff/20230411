# Comparing `tmp/Timecard-App-2.1.0.tar.gz` & `tmp/Timecard-App-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Timecard-App-2.1.0.tar", last modified: Fri Feb 25 02:05:29 2022, max compression
+gzip compressed data, was "Timecard-App-3.0.0.tar", last modified: Tue Apr 11 16:45:17 2023, max compression
```

## Comparing `Timecard-App-2.1.0.tar` & `Timecard-App-3.0.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.225847 Timecard-App-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/Timecard_App.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-25 02:05:29.000000 Timecard-App-2.1.0/src/Timecard_App.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/timecard/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/timecard/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4231 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/data/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/data/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8441 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/data/timelog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/timecard/interface/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/aboutview.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6104 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/appcontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)     8013 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/editview.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/focus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/logview.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/notes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/quitview.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/settingsview.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/systray.py
--rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/timecontrols.py
--rw-r--r--   0 runner    (1001) docker     (121)     6288 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/timedisplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/interface/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/timecard/logic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/logic/clock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 02:05:29.229847 Timecard-App-2.1.0/src/timecard/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     9552 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/resources/about.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9984 2022-02-25 02:05:17.000000 Timecard-App-2.1.0/src/timecard/resources/timecard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.385771 Timecard-App-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.385771 Timecard-App-3.0.0/src/Timecard_App.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 16:45:17.000000 Timecard-App-3.0.0/src/Timecard_App.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.385771 Timecard-App-3.0.0/src/timecard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.385771 Timecard-App-3.0.0/src/timecard/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/data/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/data/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/data/timelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/src/timecard/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/aboutview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/appcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/editview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/logview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/quitview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/settingsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/systray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/timecontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/timedisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/interface/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/src/timecard/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/logic/clock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:17.389771 Timecard-App-3.0.0/src/timecard/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/resources/about.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard/resources/timecard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 16:45:06.000000 Timecard-App-3.0.0/src/timecard-app.py
```

### Comparing `Timecard-App-2.1.0/LICENSE` & `Timecard-App-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Timecard-App-2.1.0/PKG-INFO` & `Timecard-App-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 Metadata-Version: 2.1
 Name: Timecard-App
-Version: 2.1.0
+Version: 3.0.0
 Summary: Track time beautifully.
-Home-page: https://github.com/codemouse92/timecard
-Author: Jason C. McDonald
-Author-email: codemouse92@outlook.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/codemouse92/timecard/issues
+Author-email: "Jason C. McDonald" <codemouse92@outlook.com>
+Maintainer-email: "Jason C. McDonald" <codemouse92@outlook.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2019, Jason C. McDonald
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://codemouse92.github.io/Timecard/
+Project-URL: Repository, https://github.com/codemouse92/timecard
+Project-URL: Issues, https://github.com/codemouse92/timecard/issues
 Project-URL: Funding, https://github.com/sponsors/CodeMouse92
-Project-URL: Source, https://github.com/codemouse92/timecard
-Keywords: time tracking office clock tool utility
-Platform: UNKNOWN
+Keywords: time,tracking,office,clock,tool,utility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Office/Business
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Python: <4,>=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Timecard
 
 **Track time beautifully.**
 
@@ -111,9 +142,7 @@
 
 Bug reports and pull requests are welcome via
 [GitHub](https://github.com/codemouse92/timecard)!
 
 ## License
 
 Timecard 2 is licensed under the BSD-3-Clause license (see `LICENSE`).
-
-
```

### Comparing `Timecard-App-2.1.0/README.md` & `Timecard-App-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Timecard-App-2.1.0/src/Timecard_App.egg-info/PKG-INFO` & `Timecard-App-3.0.0/src/Timecard_App.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 Metadata-Version: 2.1
 Name: Timecard-App
-Version: 2.1.0
+Version: 3.0.0
 Summary: Track time beautifully.
-Home-page: https://github.com/codemouse92/timecard
-Author: Jason C. McDonald
-Author-email: codemouse92@outlook.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/codemouse92/timecard/issues
+Author-email: "Jason C. McDonald" <codemouse92@outlook.com>
+Maintainer-email: "Jason C. McDonald" <codemouse92@outlook.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2019, Jason C. McDonald
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://codemouse92.github.io/Timecard/
+Project-URL: Repository, https://github.com/codemouse92/timecard
+Project-URL: Issues, https://github.com/codemouse92/timecard/issues
 Project-URL: Funding, https://github.com/sponsors/CodeMouse92
-Project-URL: Source, https://github.com/codemouse92/timecard
-Keywords: time tracking office clock tool utility
-Platform: UNKNOWN
+Keywords: time,tracking,office,clock,tool,utility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Office/Business
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Python: <4,>=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Timecard
 
 **Track time beautifully.**
 
@@ -111,9 +142,7 @@
 
 Bug reports and pull requests are welcome via
 [GitHub](https://github.com/codemouse92/timecard)!
 
 ## License
 
 Timecard 2 is licensed under the BSD-3-Clause license (see `LICENSE`).
-
-
```

### Comparing `Timecard-App-2.1.0/src/Timecard_App.egg-info/SOURCES.txt` & `Timecard-App-3.0.0/src/Timecard_App.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+src/timecard-app.py
 src/Timecard_App.egg-info/PKG-INFO
 src/Timecard_App.egg-info/SOURCES.txt
 src/Timecard_App.egg-info/dependency_links.txt
 src/Timecard_App.egg-info/entry_points.txt
 src/Timecard_App.egg-info/requires.txt
 src/Timecard_App.egg-info/top_level.txt
 src/timecard/__init__.py
@@ -29,9 +30,10 @@
 src/timecard/interface/settingsview.py
 src/timecard/interface/systray.py
 src/timecard/interface/timecontrols.py
 src/timecard/interface/timedisplay.py
 src/timecard/interface/workspace.py
 src/timecard/logic/__init__.py
 src/timecard/logic/clock.py
+src/timecard/resources/__init__.py
 src/timecard/resources/about.txt
 src/timecard/resources/timecard.svg
```

### Comparing `Timecard-App-2.1.0/src/timecard/data/backup.py` & `Timecard-App-3.0.0/src/timecard/data/backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,57 @@
 
 Stores the current state of the program in a temporary file, in case of
 crash or accidental quit.
 """
 
 import logging
 from datetime import datetime
-from time import time, sleep
-from appdirs import user_cache_dir
 from pathlib import Path
+from time import sleep, time
+
+from appdirs import user_cache_dir
 
-from timecard.interface.timedisplay import TimeDisplay
 from timecard.interface.notes import Notes
 from timecard.interface.timecontrols import TimeControls
+from timecard.interface.timedisplay import TimeDisplay
 
 
 class Backup:
-
     _active = False
     # use the system epoch as a unique instance identifier
-    _backup_dir = Path(user_cache_dir('timecard'))
+    _backup_dir = Path(user_cache_dir("timecard"))
     _instance_id = str(int(time()))
-    _storage = _backup_dir / f'{_instance_id}.backup'
-    _staging = _backup_dir / f'{_instance_id}.backup~'
-    _query = _backup_dir / f'{_instance_id}.query'
+    _storage = _backup_dir / f"{_instance_id}.backup"
+    _staging = _backup_dir / f"{_instance_id}.backup~"
+    _query = _backup_dir / f"{_instance_id}.query"
 
     @classmethod
     def check_for_recall(cls):
         """Check if there is a backup that needs to be grabbed.
         If there are multiple backups, grab one (doesn't matter which)."""
         try:
-            for backup in cls._backup_dir.glob('*.backup'):
+            for backup in cls._backup_dir.glob("*.backup"):
                 # Check for signs of life
-                query = cls._backup_dir / f'{backup.stem}.query'
+                query = cls._backup_dir / f"{backup.stem}.query"
                 # Create a query file to see if this instance ID is alive.
                 query.touch(exist_ok=True)
                 # Wait a literal second to let any other instances "respond"
                 sleep(1)
                 # If the other instance was alive, it would delete the query...
                 if not query.exists():
                     # In that case, this one is occupied. Next!
                     continue
 
-                with backup.open('r') as file:
+                with backup.open("r") as file:
                     recovered = [s.strip() for s in file.readlines()]
 
                     # Attempt to restore the recovered data.
-                    timestamp = datetime(*(int(v) for v in recovered[0].split(':')))
+                    timestamp = datetime(
+                        *(int(v) for v in recovered[0].split(":"))
+                    )
                     duration = int(recovered[1])
                     TimeDisplay.restore_from_backup(timestamp, duration)
                     notes = recovered[2]
                     Notes.restore_from_backup(notes)
 
                     # Allow the user to either reset or save.
                     TimeControls._set_mode_save()
@@ -77,19 +79,19 @@
     def remember(cls, hours, minutes, seconds):
         # Don't store when clock resets, only if minutes or hours has a value
         if hours or minutes:
             # Grab data in advance
             data = [
                 TimeDisplay.get_timestamp_string() + "\n",
                 TimeDisplay.get_time_ms_string() + "\n",
-                Notes.get_text() + "\n"
+                Notes.get_text() + "\n",
             ]
 
             # Write data to staging file
-            with cls._staging.open('w') as file:
+            with cls._staging.open("w") as file:
                 file.writelines(data)
             cls._staging.replace(cls._storage)  # Move into place
 
     @classmethod
     def forget(cls):
         """Clear backups for instance."""
         cls._storage.unlink(missing_ok=True)
```

### Comparing `Timecard-App-2.1.0/src/timecard/data/settings.py` & `Timecard-App-3.0.0/src/timecard/data/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,40 +4,45 @@
 Manages access, storage, and file read/write for application settings.
 """
 
 import functools
 import logging
 import os
 from pathlib import Path
+
 from appdirs import user_config_dir, user_data_dir
 
 
 def settings_getter(func):
     """Ensure settings are loaded appropriately."""
+
     @functools.wraps(func)
     def wrapper(*args, **vargs):
         Settings.load()
         return func(*args, **vargs)
+
     return wrapper
 
 
 def settings_setter(func):
     """Ensure settings are loaded from and saved to file appropriately."""
+
     @functools.wraps(func)
     def wrapper(*args, **vargs):
         Settings.load()
         r = func(*args, **vargs)
         Settings.save()
         return r
+
     return wrapper
 
 
 class Settings:
     _settings = None
-    _settings_path = Path(user_config_dir('timecard'), "settings.conf")
+    _settings_path = Path(user_config_dir("timecard"), "settings.conf")
     # Other places to read the settings from (will not save to)
     _settings_path_alts = (Path(Path.home(), ".timecardrc"),)
     # Whether we loaded from an alt location
     _from_alt = False
 
     @classmethod
     def load(cls, force=False):
@@ -70,182 +75,184 @@
         """Load the settings from file.
         You probably shouldn't use this directly; use Settings.load() instead.
         """
         cls._settings = dict()
 
         logging.debug(f"Loading settings from {str(settings_path)}")
 
-        with settings_path.open('r', encoding='utf-8') as file:
+        with settings_path.open("r", encoding="utf-8") as file:
             for lineno, line in enumerate(file, start=1):
                 try:
-                    if line[0] == '#':
+                    if line[0] == "#":
                         # Line is a comment, ignore.
                         continue
                     # Split line around the = operator
-                    k, v = (s.strip() for s in line.split(sep='=', maxsplit=2))
+                    k, v = (s.strip() for s in line.split(sep="=", maxsplit=2))
                 except ValueError:
-                    logging.warning(f"Invalid entry in {settings_path}:{lineno}\n"
-                                    f"  {line}")
+                    logging.warning(
+                        f"Invalid entry in {settings_path}:{lineno}\n"
+                        f"  {line}"
+                    )
                 else:
                     cls._settings[k] = v
 
     @classmethod
     def load_from_default(cls):
         """Load the settings from default.
         You probably shouldn't use this directly; use Settings.load() instead.
         """
         cls._settings = dict()
 
-        cls._settings['datefmt'] = cls.get_datefmt()
-        cls._settings['decdur'] = str(cls.get_decdur())
-        cls._settings['logdir'] = cls.get_logdir_str()
-        cls._settings['logname'] = cls.get_logname()
-        cls._settings['persist'] = str(cls.get_persist())
+        cls._settings["datefmt"] = cls.get_datefmt()
+        cls._settings["decdur"] = str(cls.get_decdur())
+        cls._settings["logdir"] = cls.get_logdir_str()
+        cls._settings["logname"] = cls.get_logname()
+        cls._settings["persist"] = str(cls.get_persist())
 
     @classmethod
     def save(cls):
         """Save the log to file."""
         cls._settings_path.parent.mkdir(parents=True, exist_ok=True)
-        with cls._settings_path.open('w', encoding='utf-8') as file:
+        with cls._settings_path.open("w", encoding="utf-8") as file:
             for key, value in cls._settings.items():
                 file.write(f"{key}={value}\n")
         # Clean up alternatives
         if cls._from_alt:
             cls.cleanup_alts()
 
     @classmethod
     def cleanup_alts(cls):
         """Rewrite alternative files to discourage their continued use."""
         message = [
             "# Your settings have automatically been migrated!\n",
-            f"# See {cls._settings_path}\n"
+            f"# See {cls._settings_path}\n",
         ]
         for settings_path in cls._settings_path_alts:
             if not settings_path.exists():
                 continue
-            with settings_path.open('r') as file:
+            with settings_path.open("r") as file:
                 original = file.readlines()
 
             # If file was already processed by this instance...
             if original[:2] == message:
                 continue
             # If file was previously processed, strip prior comments...
             elif original[:1] == message[:1]:
                 original = original[2:]
 
             # Prepend processing comments
-            with settings_path.open('w', encoding='utf-8') as file:
+            with settings_path.open("w", encoding="utf-8") as file:
                 file.writelines(message)
                 file.writelines(original)
 
     @classmethod
     @settings_getter
     def get_logdir_str(cls):
         """Get the log directory path as a string."""
         try:
-            logdir = cls._settings['logdir']
+            logdir = cls._settings["logdir"]
             return os.path.normpath(logdir)
         except KeyError:
-            return str(Path(user_data_dir('timecard')))
+            return str(Path(user_data_dir("timecard")))
 
     @classmethod
     @settings_getter
     def get_logdir(cls):
         """Get the log directory path."""
         logdir = cls.get_logdir_str()
         return Path(*(logdir.split(os.pathsep)))
 
     @classmethod
     @settings_setter
     def set_logdir(cls, logdir):
         """Set the log path."""
-        cls._settings['logdir'] = logdir
+        cls._settings["logdir"] = logdir
 
     @classmethod
     @settings_getter
     def get_logname(cls):
         """Get the log filename."""
         try:
-            return cls._settings['logname']
+            return cls._settings["logname"]
         except KeyError:
             return "time.log"
 
     @classmethod
     @settings_setter
     def set_logname(cls, logname):
         """Set the log path."""
-        cls._settings['logname'] = logname
+        cls._settings["logname"] = logname
 
     @classmethod
     @settings_getter
     def get_logpath(cls):
         """Get the full log path."""
         return cls.get_logdir().joinpath(cls.get_logname())
 
     @classmethod
     @settings_getter
     def get_persist(cls):
         """Returns whether closing the window should hide it or quit."""
         try:
-            return cls._settings['persist'] != 'False'
+            return cls._settings["persist"] != "False"
         except KeyError:
             return True
 
     @classmethod
     @settings_setter
     def set_persist(cls, persist):
         """Sets persistence."""
-        cls._settings['persist'] = str(persist)
+        cls._settings["persist"] = str(persist)
 
     @classmethod
     @settings_getter
     def get_datefmt(cls):
         """Returns timestamp format (should be in 1989 C standard)."""
         try:
-            return cls._settings['datefmt']
+            return cls._settings["datefmt"]
         except KeyError:
             return "%Y-%m-%d %H:%M:%S"
 
     @classmethod
     @settings_setter
     def set_datefmt(cls, datefmt):
-        cls._settings['datefmt'] = datefmt
+        cls._settings["datefmt"] = datefmt
 
     @classmethod
     @settings_getter
     def get_decdur(cls):
         """Returns whether duration should be displayed as decimal
         or HH:MM;SS.
         """
         try:
-            return cls._settings['decdur'] != 'False'
+            return cls._settings["decdur"] != "False"
         except KeyError:
             return False
 
     @classmethod
     @settings_setter
     def set_decdur(cls, decdur):
         """Sets whether duration should be displayed as decimal."""
-        cls._settings['decdur'] = str(decdur)
+        cls._settings["decdur"] = str(decdur)
 
     @classmethod
     @settings_getter
     def get_focus(cls):
         """Returns focus reminder interval and randomization."""
         try:
             return (
-                int(cls._settings['focus']),
-                (cls._settings['focus_randomize'] != 'False')
+                int(cls._settings["focus"]),
+                (cls._settings["focus_randomize"] != "False"),
             )
         except KeyError:
             # Use default
             return (0, False)
         except ValueError:
             # The integer couldn't be read, but the boolean is good.
-            return (0, (cls._settings['focus_randomize'] != 'False'))
+            return (0, (cls._settings["focus_randomize"] != "False"))
 
     @classmethod
     @settings_setter
     def set_focus(cls, interval, randomize):
         """Sets focus reminder settings."""
-        cls._settings['focus'] = str(interval)
-        cls._settings['focus_randomize'] = str(randomize)
+        cls._settings["focus"] = str(interval)
+        cls._settings["focus_randomize"] = str(randomize)
```

### Comparing `Timecard-App-2.1.0/src/timecard/data/timelog.py` & `Timecard-App-3.0.0/src/timecard/data/timelog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 """Time Log [Timecard]
 Author(s): Jason C. McDonald
 
 Manages access, storage, and file read/write for the time log.
 Also contains the class representing a single time log entry.
 """
 
-from datetime import datetime
 import functools
 import logging
 import os
+from datetime import datetime
 
 from timecard.data.settings import Settings
 
 
 def timelog_getter(func):
     """Ensure settings are loaded appropriately."""
+
     @functools.wraps(func)
     def wrapper(*args, **vargs):
         # Ensure log is loaded from file
         TimeLog.load()
         return func(*args, **vargs)
+
     return wrapper
 
 
 def timelog_setter(func):
     """Ensure settings are loaded from and saved to file appropriately."""
+
     @functools.wraps(func)
     def wrapper(*args, **vargs):
         # Ensure log is loaded from file
         TimeLog.load()
         r = func(*args, **vargs)
         # Immediately write the log to file
         TimeLog.save()
         return r
+
     return wrapper
 
 
 class LogEntry:
-
     def __init__(self, timestamp=None, duration=(0, 0, 0), notes=""):
         self.timestamp = timestamp
         self.duration = duration
         self.notes = notes
 
     @staticmethod
     def normalize_timestamp(timestamp):
         """Normalizes the timestamp, throwing away milliseconds and
         timezone data.
 
         timestamp -- the timestamp to normalize
 
         Returns the normalized timestamp.
         """
-        return datetime(timestamp.year,
-                        timestamp.month,
-                        timestamp.day,
-                        timestamp.hour,
-                        timestamp.minute,
-                        timestamp.second
-                        )
+        return datetime(
+            timestamp.year,
+            timestamp.month,
+            timestamp.day,
+            timestamp.hour,
+            timestamp.minute,
+            timestamp.second,
+        )
 
     def set_timestamp(self, timestamp):
         """Normalize and set the timestamp."""
         self.timestamp = LogEntry.normalize_timestamp(timestamp)
 
     def set_timestamp_from_string(self, timestamp_str):
         """Set the timestamp from dash-delimited string."""
         try:
-            ts = [int(n) for n in timestamp_str.split('-')]
+            ts = [int(n) for n in timestamp_str.split("-")]
             self.timestamp = datetime(*ts)
         except (TypeError, ValueError):
             return False
         return True
 
     def set_duration(self, hours, minutes, seconds):
         """Set duration from tuple.
@@ -81,57 +85,62 @@
         seconds -- the number of seconds
         """
         self.duration = (hours, minutes, seconds)
 
     def set_duration_from_string(self, duration_str):
         """Set duration from colon-delimited string."""
         try:
-            duration = [int(n) for n in duration_str.split(':')]
+            duration = [int(n) for n in duration_str.split(":")]
             self.set_duration(*duration)
         except (TypeError, ValueError):
             return False
         return True
 
     def timestamp_as_string(self):
         """Retrieve timestamp as dash-delimited string."""
-        return (f"{self.timestamp.year}-{self.timestamp.month}-"
-                f"{self.timestamp.day}-{self.timestamp.hour}-"
-                f"{self.timestamp.minute}-{self.timestamp.second}")
+        return (
+            f"{self.timestamp.year}-{self.timestamp.month}-"
+            f"{self.timestamp.day}-{self.timestamp.hour}-"
+            f"{self.timestamp.minute}-{self.timestamp.second}"
+        )
 
     def timestamp_as_format(self, format):
         """Retrieve timestamp according to given format string."""
         return self.timestamp.strftime(format)
 
     def duration_as_string(self, as_decimal=False):
         """Retrieve duration in format HH:MM:SS"""
         if as_decimal:
             decdur = self.duration[0] + (self.duration[1] / 60)
             return f"{decdur:.2f}"
         else:
-            return (f"{self.duration[0]:02}:"
-                    f"{self.duration[1]:02}:"
-                    f"{self.duration[2]:02}")
+            return (
+                f"{self.duration[0]:02}:"
+                f"{self.duration[1]:02}:"
+                f"{self.duration[2]:02}"
+            )
 
     def set_notes(self, notes):
         """Retrive note string."""
         self.notes = notes
 
 
 class TimeLog:
     _log = None
 
     @staticmethod
     def increment_timestamp(timestamp):
-        return datetime(timestamp.year,
-                        timestamp.month,
-                        timestamp.day,
-                        timestamp.hour,
-                        timestamp.minute,
-                        timestamp.second + 1
-                        )
+        return datetime(
+            timestamp.year,
+            timestamp.month,
+            timestamp.day,
+            timestamp.hour,
+            timestamp.minute,
+            timestamp.second + 1,
+        )
 
     @classmethod
     def load(cls, force=False):
         """Load the time log from file."""
 
         # If we've already loaded, don't reload unless forced to.
         if not force and cls._log is not None:
@@ -142,25 +151,26 @@
 
         logging.debug(f"Loading time log from {path}")
 
         # Initialize an empty log.
         cls._log = dict()
         # Attempt to open and parse the file.
         try:
-            with path.open('r', encoding='utf-8') as file:
+            with path.open("r", encoding="utf-8") as file:
                 # Process each line in the log file
                 for lineno, line in enumerate(file, start=1):
                     # Each entry consists of three fields, separated by pipes
-                    entry_raw = line.strip().split('|', 3)
+                    entry_raw = line.strip().split("|", 3)
 
                     # If we don't get three fields,
                     # log a warning and skip the entry.
                     if len(entry_raw) != 3:
-                        logging.warning(f"Invalid entry in {path}:{lineno}\n"
-                                        f"  {line}")
+                        logging.warning(
+                            f"Invalid entry in {path}:{lineno}\n" f"  {line}"
+                        )
                         continue
 
                     # Create a log entry from the data line.
                     entry = LogEntry()
                     entry.set_timestamp_from_string(entry_raw[0])
                     entry.set_duration_from_string(entry_raw[1])
                     entry.set_notes(entry_raw[2])
@@ -181,19 +191,23 @@
         # Create the save directory if necessary
         if not logdir.exists():
             os.makedirs(logdir)
 
         # Retrieve the full save path from settings
         logpath = Settings.get_logpath()
         # Write the log out to the file.
-        with logpath.open('w', encoding='utf-8') as file:
+        with logpath.open("w", encoding="utf-8") as file:
             for entry in cls._log.values():
-                file.write((f"{entry.timestamp_as_string()}|"
-                            f"{entry.duration_as_string()}|"
-                            f"{entry.notes}\n"))
+                file.write(
+                    (
+                        f"{entry.timestamp_as_string()}|"
+                        f"{entry.duration_as_string()}|"
+                        f"{entry.notes}\n"
+                    )
+                )
 
     @classmethod
     @timelog_getter
     def retrieve_log(cls):
         """Returns the log as a list, loading it from file if necessary."""
         return [entry for entry in cls._log.values()]
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/aboutview.py` & `Timecard-App-3.0.0/src/timecard/interface/aboutview.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 """About View [Timecard]
 Author(s): Jason C. McDonald
 
 Displays "about" data for Timecard.
 """
 
-import os
+from importlib import resources
 from pathlib import Path
-from pkg_resources import resource_filename
 
-from PySide2.QtCore import Qt
-from PySide2.QtWidgets import QWidget, QVBoxLayout, QTextEdit
+from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QTextEdit, QVBoxLayout, QWidget
 
 
 class AboutView:
     widget = QWidget()
     layout = QVBoxLayout()
     lbl_info = QTextEdit()
 
     @classmethod
     def build(cls):
         """Build the interface."""
         cls.lbl_info = QTextEdit()
 
-        about_path = resource_filename(
-            'timecard',
-            os.path.join('resources', 'about.txt')
+        about_file = Path(
+            resources.files("timecard.resources").joinpath("about.txt")
         )
-        about_file = Path(about_path)
         try:
-            with about_file.open('r', encoding='utf-8') as file:
+            with about_file.open("r", encoding="utf-8") as file:
                 cls.lbl_info.setPlainText(file.read())
         except FileNotFoundError:
-            cls.lbl_info.setPlainText("TIMECARD\n"
-                                      "Created by Jason C. McDonald\n\n"
-                                      "ERROR: `resources/about.txt` missing")
+            cls.lbl_info.setPlainText(
+                "TIMECARD\n"
+                "Created by Jason C. McDonald\n\n"
+                "ERROR: `resources/about.txt` missing"
+            )
         cls.lbl_info.setWhatsThis("Credits and license for Timecard.")
         cls.lbl_info.setReadOnly(True)
         cls.lbl_info.setAlignment(Qt.AlignCenter)
 
         cls.widget.setLayout(cls.layout)
         cls.layout.addWidget(cls.lbl_info)
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/app.py` & `Timecard-App-3.0.0/src/timecard/interface/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Author(s): Jason C. McDonald
 
 The main application classes. Most of the interface modules rely on this,
 so it should not rely on any other module in the interface subpackage.
 """
 
 import logging
-import os
-from pkg_resources import resource_filename
+from importlib import resources
 
-from PySide2.QtWidgets import QApplication, QVBoxLayout, QWidget
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import QApplication, QVBoxLayout, QWidget
 
 from timecard.data.settings import Settings
 
+VERSION = "3.0.0"
 
 class MainWindow(QWidget):
     def closeEvent(self, event):
         """Hide the window on close."""
         if Settings.get_persist():
             App.hide_window()
             event.ignore()
@@ -26,17 +26,16 @@
 
 
 class App:
     app = QApplication()
     window = MainWindow()
     layout = QVBoxLayout()
 
-    icon_path = resource_filename(
-        'timecard',
-        os.path.join('resources', 'timecard.svg')
+    icon_path = str(
+        resources.files("timecard.resources").joinpath("timecard.svg")
     )
     icon = QIcon(icon_path)
 
     hide_callback = []
 
     @classmethod
     def run(cls):
@@ -49,16 +48,16 @@
         return cls.app.exec_()
 
     @classmethod
     def build(cls):
         """Construct the application."""
         logging.debug("Building application.")
         cls.app.setApplicationName("Timecard")
-        cls.app.setApplicationVersion('2.1.0')
-        cls.app.setDesktopFileName('com.codemouse92.timecard')
+        cls.app.setApplicationVersion(VERSION)
+        cls.app.setDesktopFileName("com.codemouse92.timecard")
         cls.app.setWindowIcon(cls.icon)
 
         logging.debug("Building main window.")
         cls.window.resize(500, 400)
         cls.window.setLayout(cls.layout)
 
     @classmethod
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/appcontrols.py` & `Timecard-App-3.0.0/src/timecard/interface/appcontrols.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """App Controls [Timecard]
 Author(s): Jason C. McDonald
 
 Allows switching between major application views.
 """
 
-from PySide2.QtWidgets import QPushButton, QHBoxLayout, QWidget
-from PySide2.QtWidgets import QWhatsThis
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import QHBoxLayout, QPushButton, QWhatsThis, QWidget
 
-from timecard.interface.workspace import Workspace
 from timecard.interface.quitview import QuitView
+from timecard.interface.workspace import Workspace
 
 
 class AppControls:
     widget = QWidget()
     layout = QHBoxLayout()
     btn_settings = QPushButton()
     btn_about = QPushButton()
@@ -62,105 +61,105 @@
 
     @classmethod
     def _set_mode_default(cls):
         """Set buttons to those for Log (default) mode."""
         cls._disconnect_buttons()
 
         cls.btn_settings.setText("Settings")
-        cls.btn_settings.setIcon(QIcon.fromTheme('preferences-system'))
+        cls.btn_settings.setIcon(QIcon.fromTheme("preferences-system"))
         cls.btn_settings.setWhatsThis("View and edit settings.")
         cls.btn_settings.clicked.connect(cls.settings)
 
         cls.btn_about.setText("About")
-        cls.btn_about.setIcon(QIcon.fromTheme('help-about'))
+        cls.btn_about.setIcon(QIcon.fromTheme("help-about"))
         cls.btn_about.setWhatsThis("View Timecard credits and license.")
         cls.btn_about.clicked.connect(cls.about)
 
         cls.btn_help.setText("Help")
-        cls.btn_help.setIcon(QIcon.fromTheme('help-contents'))
+        cls.btn_help.setIcon(QIcon.fromTheme("help-contents"))
         cls.btn_help.setWhatsThis("Display help for a clicked item.")
         cls.btn_help.clicked.connect(cls.help)
 
         cls.btn_quit.setText("Quit")
-        cls.btn_quit.setIcon(QIcon.fromTheme('application-exit'))
+        cls.btn_quit.setIcon(QIcon.fromTheme("application-exit"))
         cls.btn_quit.setWhatsThis("Quit Timecard.")
         cls.btn_quit.clicked.connect(cls.quit)
 
     @classmethod
     def _set_mode_settings(cls):
         """Set buttons to those for Settings mode."""
         cls._disconnect_buttons()
 
         cls.btn_settings.setText("Log")
-        cls.btn_settings.setIcon(QIcon.fromTheme('go-home'))
+        cls.btn_settings.setIcon(QIcon.fromTheme("go-home"))
         cls.btn_settings.setWhatsThis("Return to time log.")
         cls.btn_settings.clicked.connect(cls.default)
 
         cls.btn_about.setText("About")
-        cls.btn_about.setIcon(QIcon.fromTheme('help-about'))
+        cls.btn_about.setIcon(QIcon.fromTheme("help-about"))
         cls.btn_about.setWhatsThis("View Timecard credits and license.")
         cls.btn_about.clicked.connect(cls.about)
 
         cls.btn_help.setText("Help")
-        cls.btn_help.setIcon(QIcon.fromTheme('help-contents'))
+        cls.btn_help.setIcon(QIcon.fromTheme("help-contents"))
         cls.btn_help.setWhatsThis("Display help for a clicked item.")
         cls.btn_help.clicked.connect(cls.help)
 
         cls.btn_quit.setText("Quit")
-        cls.btn_quit.setIcon(QIcon.fromTheme('application-exit'))
+        cls.btn_quit.setIcon(QIcon.fromTheme("application-exit"))
         cls.btn_quit.setWhatsThis("Quit Timecard.")
         cls.btn_quit.clicked.connect(cls.quit)
 
     @classmethod
     def _set_mode_about(cls):
         """Set buttons to those for About mode."""
         cls._disconnect_buttons()
 
         cls.btn_settings.setText("Settings")
-        cls.btn_settings.setIcon(QIcon.fromTheme('preferences-system'))
+        cls.btn_settings.setIcon(QIcon.fromTheme("preferences-system"))
         cls.btn_settings.setWhatsThis("View and edit settings.")
         cls.btn_settings.clicked.connect(cls.settings)
 
         cls.btn_about.setText("Log")
-        cls.btn_about.setIcon(QIcon.fromTheme('go-home'))
+        cls.btn_about.setIcon(QIcon.fromTheme("go-home"))
         cls.btn_about.setWhatsThis("Return to time log.")
         cls.btn_about.clicked.connect(cls.default)
 
         cls.btn_help.setText("Help")
-        cls.btn_help.setIcon(QIcon.fromTheme('help-contents'))
+        cls.btn_help.setIcon(QIcon.fromTheme("help-contents"))
         cls.btn_help.setWhatsThis("Display help for a clicked item.")
         cls.btn_help.clicked.connect(cls.help)
 
         cls.btn_quit.setText("Quit")
-        cls.btn_quit.setIcon(QIcon.fromTheme('application-exit'))
+        cls.btn_quit.setIcon(QIcon.fromTheme("application-exit"))
         cls.btn_quit.setWhatsThis("Quit Timecard.")
         cls.btn_quit.clicked.connect(cls.quit)
 
     @classmethod
     def _set_mode_quit(cls):
         """Set buttons to those for Quit Prompt mode."""
         cls._disconnect_buttons()
 
         cls.btn_settings.setText("Settings")
-        cls.btn_settings.setIcon(QIcon.fromTheme('preferences-system'))
+        cls.btn_settings.setIcon(QIcon.fromTheme("preferences-system"))
         cls.btn_settings.setWhatsThis("View and edit settings.")
         cls.btn_settings.clicked.connect(cls.settings)
 
         cls.btn_about.setText("About")
-        cls.btn_about.setIcon(QIcon.fromTheme('help-about'))
+        cls.btn_about.setIcon(QIcon.fromTheme("help-about"))
         cls.btn_about.setWhatsThis("View Timecard credits and license.")
         cls.btn_about.clicked.connect(cls.about)
 
         cls.btn_help.setText("Help")
-        cls.btn_help.setIcon(QIcon.fromTheme('help-contents'))
+        cls.btn_help.setIcon(QIcon.fromTheme("help-contents"))
         cls.btn_help.setWhatsThis("Display help for a clicked item.")
         cls.btn_help.clicked.connect(cls.help)
 
         cls.btn_quit.setText("Log")
-        cls.btn_quit.setIcon(QIcon.fromTheme('go-home'))
+        cls.btn_quit.setIcon(QIcon.fromTheme("go-home"))
         cls.btn_quit.setWhatsThis("Return to time log.")
         cls.btn_quit.clicked.connect(cls.default)
 
     @classmethod
     def default(cls):
         cls._set_mode_default()
         Workspace.set_mode_timelog()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/editview.py` & `Timecard-App-3.0.0/src/timecard/interface/editview.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,27 @@
 Author(s): Jason C. McDonald
 
 Allows editing a single time log entry.
 """
 
 from datetime import datetime
 
-from PySide2.QtWidgets import QWidget, QGridLayout, QHBoxLayout, QVBoxLayout
-from PySide2.QtWidgets import QPushButton
-from PySide2.QtWidgets import QLabel, QLineEdit, QDateTimeEdit, QSpinBox
-from PySide2.QtGui import QIcon
-from PySide2.QtCore import QDateTime, QDate, QTime
+from PySide6.QtCore import QDate, QDateTime, QTime
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import (
+    QDateTimeEdit,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
+    QSpinBox,
+    QVBoxLayout,
+    QWidget,
+)
 
 from timecard.data.timelog import TimeLog
 
 
 class EditView:
     widget = QWidget()
     layout = QVBoxLayout()
@@ -40,17 +48,17 @@
     spn_sec = QSpinBox()
     spn_sec.setMaximum(61)
     spn_sec.setMinimum(-1)  # this will get changed to 0 as needed in normalize
 
     lbl_activity = QLabel("Activity")
     txt_activity = QLineEdit()
 
-    btn_done = QPushButton(QIcon.fromTheme('cancel'), "Done")
-    btn_revert = QPushButton(QIcon.fromTheme('edit-undo'), "Revert")
-    btn_save = QPushButton(QIcon.fromTheme('document-save'), "Save")
+    btn_done = QPushButton(QIcon.fromTheme("cancel"), "Done")
+    btn_revert = QPushButton(QIcon.fromTheme("edit-undo"), "Revert")
+    btn_save = QPushButton(QIcon.fromTheme("document-save"), "Save")
 
     index = None
     entry = None
 
     done_callback = []
 
     @classmethod
@@ -164,15 +172,14 @@
         cls.spn_sec.setMinimum(-1 if (min or hour) else 0)
 
         # Reconnect the signals
         cls.spn_hour.valueChanged.connect(cls.edited)
         cls.spn_min.valueChanged.connect(cls.edited)
         cls.spn_sec.valueChanged.connect(cls.edited)
 
-
     @classmethod
     def edited(cls):
         # Normalize times
         cls.normalize()
         # Change interface to allow saving or reverting.
         cls.btn_done.setEnabled(False)
         cls.btn_revert.setEnabled(True)
@@ -186,45 +193,45 @@
 
     @classmethod
     def refresh(cls):
         if cls.entry is None:
             return
         timestamp = cls.entry.timestamp
         datetime = QDateTime()
-        datetime.setDate(QDate(timestamp.year,
-                               timestamp.month,
-                               timestamp.day))
-        datetime.setTime(QTime(timestamp.hour,
-                               timestamp.minute,
-                               timestamp.second))
+        datetime.setDate(QDate(timestamp.year, timestamp.month, timestamp.day))
+        datetime.setTime(
+            QTime(timestamp.hour, timestamp.minute, timestamp.second)
+        )
         cls.cal_timestamp.setDateTime(datetime)
 
         hours, minutes, seconds = cls.entry.duration
         cls.spn_hour.setValue(hours)
         cls.spn_min.setValue(minutes)
         cls.spn_sec.setValue(seconds)
 
         cls.txt_activity.setText(cls.entry.notes)
 
         cls.not_edited()
 
     @classmethod
     def save(cls):
         TimeLog.remove_from_log(cls.entry.timestamp)
-        timestamp = datetime(cls.cal_timestamp.date().year(),
-                             cls.cal_timestamp.date().month(),
-                             cls.cal_timestamp.date().day(),
-                             cls.cal_timestamp.time().hour(),
-                             cls.cal_timestamp.time().minute(),
-                             cls.cal_timestamp.time().second()
-                             )
-        new_timestamp = TimeLog.add_to_log(timestamp,
-                                           cls.spn_hour.value(),
-                                           cls.spn_min.value(),
-                                           cls.spn_sec.value(),
-                                           cls.txt_activity.text()
-                                           )
+        timestamp = datetime(
+            cls.cal_timestamp.date().year(),
+            cls.cal_timestamp.date().month(),
+            cls.cal_timestamp.date().day(),
+            cls.cal_timestamp.time().hour(),
+            cls.cal_timestamp.time().minute(),
+            cls.cal_timestamp.time().second(),
+        )
+        new_timestamp = TimeLog.add_to_log(
+            timestamp,
+            cls.spn_hour.value(),
+            cls.spn_min.value(),
+            cls.spn_sec.value(),
+            cls.txt_activity.text(),
+        )
         cls.not_edited()
 
         cls.entry = TimeLog.retrieve_from_log(new_timestamp)
         # Display the revised data.
         cls.refresh()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/focus.py` & `Timecard-App-3.0.0/src/timecard/interface/focus.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 Display popup notifications to check if the user is focusing.
 """
 
 import random
 import string
 
 from timecard.data.settings import Settings
+from timecard.interface.notes import Notes
 from timecard.interface.systray import SysTray
 from timecard.interface.timedisplay import TimeDisplay
-from timecard.interface.notes import Notes
 
 
 class Focus:
-
     prompt_with_note = [
         string.Template("Are you still focusing on $task?"),
         string.Template("Are you focused on $task?"),
         string.Template("You are tracking time on $task."),
         string.Template("Is $task still your focus?"),
-        string.Template("Hey there! How is $task going?")
+        string.Template("Hey there! How is $task going?"),
     ]
 
     prompt_no_note = [
         "Are you still focusing?",
         "How's your focus right now?",
         "You are still tracking time.",
-        "Hi there! Still focusing okay?"
+        "Hi there! Still focusing okay?",
     ]
 
     interval = 0
     randomize = False
     last_at = 0
     next_at = 0
 
@@ -73,15 +72,17 @@
     def notify(cls, hours, minutes, seconds):
         """Display notification."""
         if not cls.check():
             return
         cls.last_at = TimeDisplay.get_time_min()
         activity = Notes.get_text()
         if activity:
-            message = random.choice(cls.prompt_with_note).substitute(task=activity)
+            message = random.choice(cls.prompt_with_note).substitute(
+                task=activity
+            )
         else:
             message = random.choice(cls.prompt_no_note)
 
         # Show the notification
         SysTray.popup(message)
         # Determine when next notification should appear
         cls.calculate_next()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/interface.py` & `Timecard-App-3.0.0/src/timecard/interface/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Interface [Timecard]
 Author(s): Jason C. McDonald
 
 Top-level functions for the interface sub-package. These are the functions
 initially called to build and run the interface.
 """
 
-from timecard.interface.app import App
+from timecard.interface.app import App  # isort: skip <- this must come first!
+from timecard.data.backup import Backup
 from timecard.interface.appcontrols import AppControls
 from timecard.interface.focus import Focus
 from timecard.interface.notes import Notes
+from timecard.interface.systray import SysTray
 from timecard.interface.timecontrols import TimeControls
 from timecard.interface.timedisplay import TimeDisplay
-from timecard.interface.systray import SysTray
 from timecard.interface.workspace import Workspace
-
-from timecard.data.backup import Backup
-
 from timecard.logic.clock import Clock
 
 
 def build():
     """Construct the interface."""
     # Build the actual interface.
     App.build()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/logview.py` & `Timecard-App-3.0.0/src/timecard/interface/logview.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Log View [Timecard]
 Author(s): Jason C. McDonald
 
 Displays the current log entries and allows deleting or triggering edits
 on them.
 """
 
-from PySide2.QtWidgets import QWidget, QTreeWidget, QGridLayout, QPushButton
-from PySide2.QtWidgets import QTreeWidgetItem
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import (
+    QGridLayout,
+    QPushButton,
+    QTreeWidget,
+    QTreeWidgetItem,
+    QWidget,
+)
 
-from timecard.data.timelog import TimeLog
 from timecard.data.settings import Settings
+from timecard.data.timelog import TimeLog
 
 # Datestamp | Duration | Description
 
 
 class LogViewEntry(QTreeWidgetItem):
-
     def __init__(self, entry, *args, **kwargs):
         self.entry = entry
         super().__init__(*args, **kwargs)
 
         self.setText(0, self.entry.timestamp_as_format(Settings.get_datefmt()))
         self.setText(1, self.entry.duration_as_string(Settings.get_decdur()))
         self.setText(2, self.entry.notes)
@@ -42,17 +46,15 @@
 
     edit_callback = []
 
     @classmethod
     def build(cls):
         """Build the interface"""
         cls.tree_log.setWhatsThis("The time log.")
-        cls.tree_log.setHeaderLabels(
-            ["Date", "Duration", "Activity"]
-        )
+        cls.tree_log.setHeaderLabels(["Date", "Duration", "Activity"])
         cls.tree_log.setSortingEnabled(True)
         cls.layout.addWidget(cls.tree_log, 0, 0, 3, 3)
         cls.refresh()
 
         cls.layout.addWidget(cls.btn_delete, 3, 1, 1, 1)
         cls.layout.addWidget(cls.btn_edit, 3, 2, 1, 1)
         cls.unselected()
@@ -92,34 +94,34 @@
             pass
 
     @classmethod
     def _set_mode_default(cls):
         cls._disconnect_buttons()
 
         cls.btn_delete.setText("Delete")
-        cls.btn_delete.setIcon(QIcon.fromTheme('edit-delete'))
+        cls.btn_delete.setIcon(QIcon.fromTheme("edit-delete"))
         cls.btn_delete.setWhatsThis("Delete the selected log entry.")
         cls.btn_delete.clicked.connect(cls.prompt_delete)
 
         cls.btn_edit.setText("Edit")
-        cls.btn_edit.setIcon(QIcon.fromTheme('document-properties'))
+        cls.btn_edit.setIcon(QIcon.fromTheme("document-properties"))
         cls.btn_edit.setWhatsThis("Edit the selected log entry.")
         cls.btn_edit.clicked.connect(cls.edit)
 
     @classmethod
     def _set_mode_prompt_delete(cls):
         cls._disconnect_buttons()
 
         cls.btn_delete.setText("Confirm Delete")
-        cls.btn_delete.setIcon(QIcon.fromTheme('edit-delete'))
+        cls.btn_delete.setIcon(QIcon.fromTheme("edit-delete"))
         cls.btn_delete.setWhatsThis("Delete the selected log entry.")
         cls.btn_delete.clicked.connect(cls.delete)
 
         cls.btn_edit.setText("Keep")
-        cls.btn_edit.setIcon(QIcon.fromTheme('edit-undo'))
+        cls.btn_edit.setIcon(QIcon.fromTheme("edit-undo"))
         cls.btn_edit.setWhatsThis("Keep the selected log entry.")
         cls.btn_edit.clicked.connect(cls.cancel)
 
     @classmethod
     def _selected_entry(cls):
         item = cls.tree_log.selectedItems()[0]
         return item.get_timestamp()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/notes.py` & `Timecard-App-3.0.0/src/timecard/interface/notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Notes [Timecard]
 Author(s): Jason C. McDonald
 
 The box for entering session activity notes.
 """
 
-from PySide2.QtWidgets import QLineEdit
+from PySide6.QtWidgets import QLineEdit
 
 
 class Notes:
     txt_notes = QLineEdit()
 
     @classmethod
     def build(cls):
         """Build the notes interface."""
         cls.txt_notes.setPlaceholderText("What are you doing?")
-        cls.txt_notes.setWhatsThis("A description for your current activity. "
-                                   "This will be saved with the log entry.")
+        cls.txt_notes.setWhatsThis(
+            "A description for your current activity. "
+            "This will be saved with the log entry."
+        )
         return cls.txt_notes
 
     @classmethod
     def restore_from_backup(cls, notes):
         """Sets value from backup."""
         cls.txt_notes.setText(notes)
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/quitview.py` & `Timecard-App-3.0.0/src/timecard/interface/quitview.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Quit View [Timecard]
 Author(s): Jason C. McDonald
 
 Prompts the user whether they want to quit or not.
 """
 
-from PySide2.QtCore import Qt
-from PySide2.QtWidgets import QWidget, QGridLayout, QLabel, QPushButton
-from PySide2.QtGui import QIcon
+from PySide6.QtCore import Qt
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import QGridLayout, QLabel, QPushButton, QWidget
 
 from timecard.interface.app import App
 
 
 class QuitView:
     widget = QWidget()
     layout = QGridLayout()
@@ -22,24 +22,25 @@
     @classmethod
     def build(cls):
         """Build the interface."""
         cls.layout.addWidget(cls.lbl_prompt, 0, 0, 1, 2)
         cls.layout.addWidget(cls.btn_no, 1, 0)
         cls.layout.addWidget(cls.btn_yes, 1, 1)
 
-        cls.lbl_prompt.setText("Are you SURE you want to quit?\n"
-                               "Any unsaved time will be lost.")
+        cls.lbl_prompt.setText(
+            "Are you SURE you want to quit?\n" "Any unsaved time will be lost."
+        )
         cls.lbl_prompt.setAlignment(Qt.AlignCenter)
 
-        cls.btn_no.setIcon(QIcon.fromTheme('go-previous'))
+        cls.btn_no.setIcon(QIcon.fromTheme("go-previous"))
         cls.btn_no.setText("Keep Going")
         cls.btn_no.setWhatsThis("Return to time log view.")
         cls.btn_no.clicked.connect(cls.no)
 
-        cls.btn_yes.setIcon(QIcon.fromTheme('application-exit'))
+        cls.btn_yes.setIcon(QIcon.fromTheme("application-exit"))
         cls.btn_yes.setText("Quit")
         cls.btn_yes.setWhatsThis("Quit Timecard.")
         cls.btn_yes.clicked.connect(cls.yes)
 
         cls.widget.setLayout(cls.layout)
         return cls.widget
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/settingsview.py` & `Timecard-App-3.0.0/src/timecard/interface/settingsview.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,29 @@
 Author(s): Jason C. McDonald
 
 Allows viewing and editing application settings.
 """
 
 from datetime import datetime
 
-from PySide2.QtWidgets import QWidget, QGridLayout, QHBoxLayout, QVBoxLayout
-from PySide2.QtWidgets import QLabel, QCheckBox, QLineEdit, QPushButton, QSpinBox
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import (
+    QCheckBox,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
+    QSpinBox,
+    QVBoxLayout,
+    QWidget,
+)
 
-from timecard.data.timelog import TimeLog
 from timecard.data.settings import Settings
+from timecard.data.timelog import TimeLog
 from timecard.interface.focus import Focus
 
 
 class SettingsView:
     widget = QWidget()
     layout = QVBoxLayout()
     grid_widget = QWidget()
@@ -33,62 +42,75 @@
     txt_logname = QLineEdit()
     chk_persist = QCheckBox("Keep in Notification Area")
     lbl_datefmt = QLabel("Timestamp Format")
     txt_datefmt = QLineEdit()
     lbl_datefmt_test = QLabel()
     chk_decdur = QCheckBox("Show Duration as Decimal")
 
-    btn_revert = QPushButton(QIcon.fromTheme('edit-undo'), "Revert")
-    btn_save = QPushButton(QIcon.fromTheme('document-save'), "Save")
+    btn_revert = QPushButton(QIcon.fromTheme("edit-undo"), "Revert")
+    btn_save = QPushButton(QIcon.fromTheme("document-save"), "Save")
 
     reload_log = False
     reload_focus = False
 
     @classmethod
     def build(cls):
         """Build the interface."""
-        cls.lbl_focus.setWhatsThis("Periodic popup notifications to ensure you're focused.")
-        cls.spn_focus.setWhatsThis("How many minutes between focus reminders (0 to disable).")
+        cls.lbl_focus.setWhatsThis(
+            "Periodic popup notifications to ensure you're focused."
+        )
+        cls.spn_focus.setWhatsThis(
+            "How many minutes between focus reminders (0 to disable)."
+        )
         cls.spn_focus.setSuffix(" min")
         cls.spn_focus.setRange(0, 60)
         cls.spn_focus.setSingleStep(5)
         cls.spn_focus.valueChanged.connect(cls.edited)
         cls.spn_focus.valueChanged.connect(cls.focus_edited)
-        cls.chk_focus_random.setWhatsThis("Randomize reminders within 20% of selected time.")
+        cls.chk_focus_random.setWhatsThis(
+            "Randomize reminders within 20% of selected time."
+        )
         cls.chk_focus_random.stateChanged.connect(cls.edited)
         cls.chk_focus_random.stateChanged.connect(cls.focus_edited)
 
         cls.txt_logdir.textEdited.connect(cls.edited)
         cls.txt_logdir.textEdited.connect(cls.logpath_edited)
         cls.lbl_logdir.setWhatsThis("The directory where the logs are saved.")
         cls.txt_logdir.setWhatsThis("The directory where the logs are saved.")
         cls.txt_logname.textEdited.connect(cls.edited)
         cls.txt_logname.textEdited.connect(cls.logpath_edited)
         cls.lbl_logname.setWhatsThis("The filename for the log.")
         cls.txt_logname.setWhatsThis("The filename for the log.")
 
         cls.chk_persist.stateChanged.connect(cls.edited)
-        cls.chk_persist.setWhatsThis("When window is closed, keep application "
-                                     "running in notification area. WARNING: "
-                                     "If unchecked, closing the window will "
-                                     "immediately quit, discarding any "
-                                     "unsaved time.")
+        cls.chk_persist.setWhatsThis(
+            "When window is closed, keep application "
+            "running in notification area. WARNING: "
+            "If unchecked, closing the window will "
+            "immediately quit, discarding any "
+            "unsaved time."
+        )
 
         cls.txt_datefmt.textEdited.connect(cls.edited)
         cls.txt_datefmt.textEdited.connect(cls.datefmt_edited)
-        cls.lbl_datefmt.setWhatsThis("The format for the timestamp. "
-                                     "Uses 1989 C standard.")
-        cls.txt_datefmt.setWhatsThis("The format for the timestamp. "
-                                     "Uses 1989 C standard.")
-        cls.lbl_datefmt_test.setWhatsThis("Preview of the timestamp format. "
-                                          "Displays: 02 Jan 1998 14:30:25")
+        cls.lbl_datefmt.setWhatsThis(
+            "The format for the timestamp. " "Uses 1989 C standard."
+        )
+        cls.txt_datefmt.setWhatsThis(
+            "The format for the timestamp. " "Uses 1989 C standard."
+        )
+        cls.lbl_datefmt_test.setWhatsThis(
+            "Preview of the timestamp format. " "Displays: 02 Jan 1998 14:30:25"
+        )
 
         cls.chk_decdur.stateChanged.connect(cls.edited)
-        cls.chk_decdur.setWhatsThis("Display duration in log as decimal "
-                                    "instead of HH:MM:SS. (Ignores seconds.)")
+        cls.chk_decdur.setWhatsThis(
+            "Display duration in log as decimal "
+            "instead of HH:MM:SS. (Ignores seconds.)"
+        )
 
         cls.grid_layout.addWidget(cls.lbl_focus, 0, 0)
         cls.grid_layout.addWidget(cls.spn_focus, 0, 1)
 
         cls.grid_layout.addWidget(cls.chk_focus_random, 1, 1)
 
         cls.grid_layout.addWidget(cls.lbl_logdir, 2, 0)
@@ -171,15 +193,17 @@
         # Update interface controls.
         cls.datefmt_edited()
         cls.not_edited()
 
     @classmethod
     def save(cls):
         """Save the new settings."""
-        Settings.set_focus(cls.spn_focus.value(), cls.chk_focus_random.isChecked())
+        Settings.set_focus(
+            cls.spn_focus.value(), cls.chk_focus_random.isChecked()
+        )
         Settings.set_logdir(cls.txt_logdir.text())
         Settings.set_logname(cls.txt_logname.text())
         Settings.set_persist(cls.chk_persist.isChecked())
         Settings.set_datefmt(cls.txt_datefmt.text())
         Settings.set_decdur(cls.chk_decdur.isChecked())
         cls.not_edited()
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/systray.py` & `Timecard-App-3.0.0/src/timecard/interface/systray.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """System Tray [Timecard]
 Author(s): Jason C. McDonald
 
 The application system tray and its menu.
 """
 
-from PySide2.QtWidgets import QMenu, QSystemTrayIcon
-from PySide2.QtWidgets import QAction  # will import from QtGui in PySide6
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QAction, QIcon
+from PySide6.QtWidgets import QMenu, QSystemTrayIcon
 
 from timecard.interface.app import App
 from timecard.interface.timecontrols import TimeControls
 from timecard.interface.timedisplay import TimeDisplay
 
 
 class SysTray:
@@ -34,37 +33,37 @@
         cls.menu.addAction(cls.act_status)
 
         cls.menu.addAction(cls.act_time)
         cls.set_mode_stopped()
 
         cls.menu.addSeparator()
 
-        cls.act_toggle.setIcon(QIcon.fromTheme('view-restore'))
+        cls.act_toggle.setIcon(QIcon.fromTheme("view-restore"))
         cls.act_toggle.setText("Show/Hide Window")
         cls.act_toggle.triggered.connect(cls.toggle_window)
         cls.menu.addAction(cls.act_toggle)
 
         cls.menu.addSeparator()
 
-        cls.act_quit.setIcon(QIcon.fromTheme('application-exit'))
+        cls.act_quit.setIcon(QIcon.fromTheme("application-exit"))
         cls.act_quit.setText("Quit Timecard")
         cls.act_quit.triggered.connect(cls.quit_app)
         cls.menu.addAction(cls.act_quit)
 
         cls.systray.setContextMenu(cls.menu)
         cls.systray.show()
 
         TimeDisplay.connect(on_tick=cls.update_time)
         TimeControls.connect(
             on_start=cls.set_mode_running,
             on_resume=cls.set_mode_running,
             on_pause=cls.set_mode_paused,
             on_stop=cls.set_mode_save,
             on_save=cls.set_mode_stopped,
-            on_reset=cls.set_mode_stopped
+            on_reset=cls.set_mode_stopped,
         )
         App.connect(on_hide=cls.popup)
 
         return cls.systray
 
     @classmethod
     def popup(cls, message, callback=None):
@@ -84,33 +83,33 @@
 
     @classmethod
     def set_mode_stopped(cls):
         cls._disconnect_actions()
         cls.act_quit.setEnabled(True)
         cls.act_time.setEnabled(True)
         cls.act_time.setText("Start")
-        cls.act_time.setIcon(QIcon.fromTheme('media-playback-start'))
+        cls.act_time.setIcon(QIcon.fromTheme("media-playback-start"))
         cls.act_time.triggered.connect(TimeControls.start)
 
     @classmethod
     def set_mode_running(cls):
         cls._disconnect_actions()
         cls.act_quit.setEnabled(False)
         cls.act_time.setEnabled(True)
         cls.act_time.setText("Pause")
-        cls.act_time.setIcon(QIcon.fromTheme('media-playback-pause'))
+        cls.act_time.setIcon(QIcon.fromTheme("media-playback-pause"))
         cls.act_time.triggered.connect(TimeControls.pause)
 
     @classmethod
     def set_mode_paused(cls):
         cls._disconnect_actions()
         cls.act_quit.setEnabled(False)
         cls.act_time.setEnabled(True)
         cls.act_time.setText("Resume")
-        cls.act_time.setIcon(QIcon.fromTheme('media-playback-start'))
+        cls.act_time.setIcon(QIcon.fromTheme("media-playback-start"))
         cls.act_time.triggered.connect(TimeControls.resume)
 
     @classmethod
     def set_mode_save(cls):
         cls._disconnect_actions()
         cls.act_quit.setEnabled(False)
         cls.act_time.setEnabled(False)
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/timecontrols.py` & `Timecard-App-3.0.0/src/timecard/interface/timecontrols.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Time Controls [Timecard]
 Author(s): Jason C. McDonald
 
 Controls the timer and saves the time entries to the log.
 """
 
-from PySide2.QtWidgets import QPushButton, QHBoxLayout, QWidget
-from PySide2.QtGui import QIcon
+from PySide6.QtGui import QIcon
+from PySide6.QtWidgets import QHBoxLayout, QPushButton, QWidget
 
-from timecard.interface.notes import Notes
-from timecard.interface.timedisplay import TimeDisplay
 from timecard.data.timelog import TimeLog
 from timecard.interface.logview import LogView
+from timecard.interface.notes import Notes
+from timecard.interface.timedisplay import TimeDisplay
 
 
 class TimeControls:
     widget = QWidget()
     layout = QHBoxLayout()
     btn_startpause = QPushButton()
     btn_stopsave = QPushButton()
@@ -34,16 +34,23 @@
         cls.layout.addWidget(cls.btn_stopsave)
 
         cls._set_mode_stopped()
 
         return cls.widget
 
     @classmethod
-    def connect(cls, on_start=None, on_resume=None, on_pause=None,
-                on_stop=None, on_save=None, on_reset=None):
+    def connect(
+        cls,
+        on_start=None,
+        on_resume=None,
+        on_pause=None,
+        on_stop=None,
+        on_save=None,
+        on_reset=None,
+    ):
         """Connect callbacks to the time control events.
         Any callbacks not specified will not be overridden.
         (See disconnect() for removing callbacks.)
 
         Keyword arguments:
         on_start -- called when a new timer is started
         on_resume -- called when a timer is un-paused
@@ -67,16 +74,23 @@
         if on_save and on_save not in cls.save_callback:
             cls.save_callback.append(on_save)
 
         if on_reset and on_reset not in cls.reset_callback:
             cls.reset_callback.append(on_reset)
 
     @classmethod
-    def disconnect(cls, on_start=None, on_resume=None, on_pause=None,
-                   on_stop=None, on_save=None, on_reset=None):
+    def disconnect(
+        cls,
+        on_start=None,
+        on_resume=None,
+        on_pause=None,
+        on_stop=None,
+        on_save=None,
+        on_reset=None,
+    ):
         """Disconnect functions from the time control events.
         Pass the function to remove from the callback.
 
         Keyword arguments:
         on_start -- called when a new timer is started
         on_resume -- called when a timer is un-paused
         on_pause -- called when a timer is paused or tentatively-stopped
@@ -131,15 +145,15 @@
 
     @classmethod
     def _set_mode_stopped(cls):
         """Set buttons to stopped-clock state."""
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Start")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('media-playback-start'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("media-playback-start"))
         cls.btn_startpause.setWhatsThis("Start a new timer.")
         cls.btn_startpause.clicked.connect(cls.start)
 
         cls.btn_stopsave.setIcon(QIcon.fromTheme(None))
         cls.btn_stopsave.setText("Stopped")
         cls.btn_stopsave.setWhatsThis("Timer is already stopped.")
         cls.btn_stopsave.setEnabled(False)
@@ -147,92 +161,95 @@
     @classmethod
     def _set_mode_save(cls):
         """Set buttons to save-or-reset state."""
 
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Reset")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('edit-undo'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("edit-undo"))
         cls.btn_startpause.setWhatsThis("Discard time and reset timer.")
         cls.btn_startpause.clicked.connect(cls.prompt_reset)
 
-        cls.btn_stopsave.setIcon(QIcon.fromTheme('document-save'))
+        cls.btn_stopsave.setIcon(QIcon.fromTheme("document-save"))
         cls.btn_stopsave.setWhatsThis("Save time and notes to log.")
         cls.btn_stopsave.setText("Save")
         cls.btn_stopsave.setEnabled(True)
         cls.btn_stopsave.clicked.connect(cls.save)
 
     @classmethod
     def _set_mode_prompt_reset(cls):
         """Set buttons to reset-prompt state."""
 
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Confirm Reset")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('edit-undo'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("edit-undo"))
         cls.btn_startpause.setWhatsThis("Discard time and reset timer.")
         cls.btn_startpause.clicked.connect(cls.reset)
 
-        cls.btn_stopsave.setIcon(QIcon.fromTheme('document-save'))
+        cls.btn_stopsave.setIcon(QIcon.fromTheme("document-save"))
         cls.btn_stopsave.setWhatsThis("Save time and notes to log.")
         cls.btn_stopsave.setText("Save")
         cls.btn_stopsave.setEnabled(True)
         cls.btn_stopsave.clicked.connect(cls.save)
 
     @classmethod
     def _set_mode_prompt_stop(cls):
         """Set buttons to stopped-clock state."""
 
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Resume")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('media-playback-start'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("media-playback-start"))
         cls.btn_startpause.setWhatsThis("Resume timer from current time.")
         cls.btn_startpause.clicked.connect(cls.resume)
 
         cls.btn_stopsave.setText("Confirm Stop")
-        cls.btn_stopsave.setIcon(QIcon.fromTheme('media-playback-stop'))
-        cls.btn_stopsave.setWhatsThis("Stop timer. Timer must be stopped "
-                                      "before you can save.")
+        cls.btn_stopsave.setIcon(QIcon.fromTheme("media-playback-stop"))
+        cls.btn_stopsave.setWhatsThis(
+            "Stop timer. Timer must be stopped " "before you can save."
+        )
         cls.btn_stopsave.clicked.connect(cls.stop)
         cls.btn_stopsave.setEnabled(True)
 
     @classmethod
     def _set_mode_running(cls):
         """Set buttons to running-clock state."""
 
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Pause")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('media-playback-pause'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("media-playback-pause"))
         cls.btn_startpause.setWhatsThis("Pause timer.")
         cls.btn_startpause.clicked.connect(cls.pause)
 
         cls.btn_stopsave.setText("Stop")
-        cls.btn_stopsave.setIcon(QIcon.fromTheme('media-playback-stop'))
-        cls.btn_stopsave.setWhatsThis("Stop timer. Timer must be stopped "
-                                      "before you can save.")
+        cls.btn_stopsave.setIcon(QIcon.fromTheme("media-playback-stop"))
+        cls.btn_stopsave.setWhatsThis(
+            "Stop timer. Timer must be stopped " "before you can save."
+        )
         cls.btn_stopsave.clicked.connect(cls.prompt_stop)
         cls.btn_stopsave.setEnabled(True)
 
     @classmethod
     def _set_mode_paused(cls):
         """Set buttons to paused-time state."""
 
         cls._disconnect_buttons()
 
         cls.btn_startpause.setText("Resume")
-        cls.btn_startpause.setIcon(QIcon.fromTheme('media-playback-start'))
+        cls.btn_startpause.setIcon(QIcon.fromTheme("media-playback-start"))
         cls.btn_startpause.setWhatsThis("Resume timer from current time.")
         cls.btn_startpause.clicked.connect(cls.resume)
         cls.btn_stopsave.setText("Stop")
 
-        cls.btn_stopsave.setIcon(QIcon.fromTheme('media-playback-stop'))
-        cls.btn_stopsave.setWhatsThis("Stop timer. Timer must be stopped "
-                                      "before you can save.")
+        cls.btn_stopsave.setIcon(QIcon.fromTheme("media-playback-stop"))
+        cls.btn_stopsave.setWhatsThis(
+            "Stop timer. Timer must be stopped " "before you can save."
+        )
         cls.btn_stopsave.clicked.connect(cls.prompt_stop)
         cls.btn_stopsave.setEnabled(True)
 
     @classmethod
     def start(cls):
         """Start a new timer."""
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/timedisplay.py` & `Timecard-App-3.0.0/src/timecard/interface/timedisplay.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 Displays and stores the current timer duration, including its start timestamp
 and state.
 """
 
 from datetime import datetime
 
-from PySide2.QtCore import QDateTime, QDate, QTime, QElapsedTimer
-from PySide2.QtWidgets import QLCDNumber
+from PySide6.QtCore import QDate, QDateTime, QElapsedTimer, QTime
+from PySide6.QtWidgets import QLCDNumber
 
 from timecard.logic.clock import Clock
 
 
 class TimeDisplay:
-
     lcd = QLCDNumber(8)
     time = None
     timestamp = None
     # Stored time in ms from prior pause(s)
     freeze = 0
     paused = False
 
@@ -27,16 +26,17 @@
     callback_tick = []
     callback_minute = []
     callback_stop = []
 
     @classmethod
     def build(cls):
         """Build the time display GUI."""
-        cls.lcd.setWhatsThis("The time elapsed on the current timer. "
-                             "(Hours:Minutes:Seconds)")
+        cls.lcd.setWhatsThis(
+            "The time elapsed on the current timer. " "(Hours:Minutes:Seconds)"
+        )
         cls.show_default()
         cls.lcd.setMinimumSize(0, 100)
         return cls.lcd
 
     @classmethod
     def restore_from_backup(cls, timestamp: datetime, elapsed):
         """Restore the timer state from backup."""
@@ -45,15 +45,15 @@
             return
 
         # If loading from backup, indicate that fact so we don't clobber timestamp.
         cls.from_backup = True
         # Restore the timestamp.
         cls.timestamp = QDateTime(
             QDate(timestamp.year, timestamp.month, timestamp.day),
-            QTime(timestamp.hour, timestamp.minute, timestamp.second)
+            QTime(timestamp.hour, timestamp.minute, timestamp.second),
         )
         # Restore the duration
         cls.freeze = elapsed
         # Force the user to either save or reset. Resuming makes no sense.
         cls.paused = False
         # Show the time.
         cls.show_time(*cls.get_time())
@@ -119,16 +119,15 @@
 
         Clock.disconnect(on_tick=cls.update_time)
 
         cls.paused = True
 
     @classmethod
     def reset_time(cls, erase=False):
-        """Prepare timer for reset, optionally erasing the last session's time.
-        """
+        """Prepare timer for reset, optionally erasing the last session's time."""
         cls.time = None
         if erase:
             cls.freeze = 0
         for callback in cls.callback_stop:
             callback(erase)
 
     @classmethod
@@ -141,15 +140,15 @@
     @classmethod
     def get_time_ms_string(cls):
         return str(cls.get_time_ms())
 
     @classmethod
     def get_time_min(cls):
         """Returns the current elapsed time in truncated minutes."""
-        return (cls.get_time_ms() // 1000 // 60)
+        return cls.get_time_ms() // 1000 // 60
 
     @classmethod
     def get_time(cls):
         """Returns the current elapsed time as a tuple
         (hours, minutes, seconds)
         """
 
@@ -163,33 +162,35 @@
         minutes -= hours * 60
 
         return (hours, minutes, seconds)
 
     @classmethod
     def get_timestamp(cls):
         """Returns the timestamp of the last timer as a datetime object."""
-        timestamp = datetime(cls.timestamp.date().year(),
-                             cls.timestamp.date().month(),
-                             cls.timestamp.date().day(),
-                             cls.timestamp.time().hour(),
-                             cls.timestamp.time().minute(),
-                             cls.timestamp.time().second()
-                             )
+        timestamp = datetime(
+            cls.timestamp.date().year(),
+            cls.timestamp.date().month(),
+            cls.timestamp.date().day(),
+            cls.timestamp.time().hour(),
+            cls.timestamp.time().minute(),
+            cls.timestamp.time().second(),
+        )
         return timestamp
 
     @classmethod
     def get_timestamp_string(cls):
         """Returns the timestamp as a storable string."""
-        return (f"{cls.timestamp.date().year()}:"
-                f"{cls.timestamp.date().month()}:"
-                f"{cls.timestamp.date().day()}:"
-                f"{cls.timestamp.time().hour()}:"
-                f"{cls.timestamp.time().minute()}:"
-                f"{cls.timestamp.time().second()}"
-                )
+        return (
+            f"{cls.timestamp.date().year()}:"
+            f"{cls.timestamp.date().month()}:"
+            f"{cls.timestamp.date().day()}:"
+            f"{cls.timestamp.time().hour()}:"
+            f"{cls.timestamp.time().minute()}:"
+            f"{cls.timestamp.time().second()}"
+        )
 
     @classmethod
     def connect(cls, on_tick=None, on_minute=None, on_stop=None):
         """Subscribe to timer events.
 
         on_tick= fires every second. Callback must accept (hours, minutes, seconds)
         on_minute= fires every minute. Callback must accept (hours, minutes, seconds)
```

### Comparing `Timecard-App-2.1.0/src/timecard/interface/workspace.py` & `Timecard-App-3.0.0/src/timecard/interface/workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Workspace [Timecard]
 Author(s): Jason C. McDonald
 
 Switches between Views in the application.
 """
 
-from PySide2.QtWidgets import QWidget, QStackedLayout
+from PySide6.QtWidgets import QStackedLayout, QWidget
 
 from timecard.interface.aboutview import AboutView
 from timecard.interface.editview import EditView
 from timecard.interface.logview import LogView
-from timecard.interface.settingsview import SettingsView
 from timecard.interface.quitview import QuitView
+from timecard.interface.settingsview import SettingsView
 
 
 class Workspace:
-
     widget = QWidget()
     layout = QStackedLayout()
     previous = None
 
     @classmethod
     def build(cls):
         cls.widget.setLayout(cls.layout)
```

### Comparing `Timecard-App-2.1.0/src/timecard/logic/clock.py` & `Timecard-App-3.0.0/src/timecard/logic/clock.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Clock [Timecard]
 Author(s): Jason C. McDonald
 
 The core clock/timer functionality, to which pretty much everything else connects.
 """
 
-from PySide2.QtCore import QTimer
+from PySide6.QtCore import QTimer
 
 
 class Clock:
-
     clock = None
     callback_tick = []
 
     @classmethod
     def start(cls):
         """Start the clock."""
         cls.clock = QTimer()
```

### Comparing `Timecard-App-2.1.0/src/timecard/resources/about.txt` & `Timecard-App-3.0.0/src/timecard/resources/about.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-TIMECARD 2.1.0
+TIMECARD v3.0.0
 
 Created by Jason C. McDonald
 (CodeMouse92)
 
 ============================
 
 TIMECARD LICENSE
@@ -18,15 +18,15 @@
 
 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ============================
 
-PYSIDE2 LICENSE
+PYSIDE6 LICENSE
 GNU LESSER GENERAL PUBLIC LICENSE
 
 The Qt Toolkit is Copyright (C) 2016 The Qt Company Ltd.
 Contact: http://www.qt.io/licensing/
 
 You may use, distribute and copy the Qt Toolkit under the terms of GNU Lesser General Public License version 3, which is displayed below. This license makes reference to the version 3 of the GNU General Public License, which you can find in the LICENSE.GPLv3 file.
```

### Comparing `Timecard-App-2.1.0/src/timecard/resources/timecard.svg` & `Timecard-App-3.0.0/src/timecard/resources/timecard.svg`

 * *Files identical despite different names*

