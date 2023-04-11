# Comparing `tmp/scipion-installer-1.0.8.tar.gz` & `tmp/scipion-installer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scipion-installer-1.0.8.tar", last modified: Fri Sep 25 13:00:59 2020, max compression
+gzip compressed data, was "dist/scipion-installer-1.0.9.tar", last modified: Fri Sep 25 14:24:15 2020, max compression
```

## Comparing `scipion-installer-1.0.8.tar` & `scipion-installer-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 13:00:59.306854 scipion-installer-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (116)    35147 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5246 2020-09-25 13:00:59.306854 scipion-installer-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3489 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 13:00:59.306854 scipion-installer-1.0.8/scipion_installer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5246 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      434 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       68 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-09-25 13:00:59.000000 scipion-installer-1.0.8/scipion_installer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 13:00:59.306854 scipion-installer-1.0.8/scipioninstaller/
--rw-r--r--   0 runner    (1001) docker     (116)       55 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/scipioninstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       83 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/scipioninstaller/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11748 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/scipioninstaller/installer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1146 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/scipioninstaller/launchers.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-25 13:00:59.306854 scipion-installer-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2694 2020-09-25 13:00:53.000000 scipion-installer-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 14:24:15.954354 scipion-installer-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    35147 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5246 2020-09-25 14:24:15.954354 scipion-installer-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3489 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 14:24:15.954354 scipion-installer-1.0.9/scipion_installer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5246 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       68 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2020-09-25 14:24:15.000000 scipion-installer-1.0.9/scipion_installer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-09-25 14:24:15.954354 scipion-installer-1.0.9/scipioninstaller/
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/scipioninstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       83 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/scipioninstaller/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11737 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/scipioninstaller/installer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1146 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/scipioninstaller/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-09-25 14:24:15.954354 scipion-installer-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2694 2020-09-25 14:24:09.000000 scipion-installer-1.0.9/setup.py
```

### Comparing `scipion-installer-1.0.8/LICENSE` & `scipion-installer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-installer-1.0.8/PKG-INFO` & `scipion-installer-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-installer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Installs scipion 3 creating a virtual environment for it, for now only for developers.
 Home-page: https://github.com/scipion-em/scipion-installer
 Author: I2PC, Pablo Conesa, Yunior Fonseca
 Author-email: pconesa@cnb.csic.es, 
 License: UNKNOWN
 Description: =================
         Scipion installer
```

### Comparing `scipion-installer-1.0.8/README.rst` & `scipion-installer-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-installer-1.0.8/scipion_installer.egg-info/PKG-INFO` & `scipion-installer-1.0.9/scipion_installer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-installer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Installs scipion 3 creating a virtual environment for it, for now only for developers.
 Home-page: https://github.com/scipion-em/scipion-installer
 Author: I2PC, Pablo Conesa, Yunior Fonseca
 Author-email: pconesa@cnb.csic.es, 
 License: UNKNOWN
 Description: =================
         Scipion installer
```

### Comparing `scipion-installer-1.0.8/scipioninstaller/installer.py` & `scipion-installer-1.0.9/scipioninstaller/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,22 +123,22 @@
                           pipInstall=True, cloneFolder=''):
     
     # Choose url type: ssh or https
     cloneUrl= 'git@github.com:%s/%s.git' if not useHttps else 'https://github.com/%s/%s.git'
 
     # replace the repository name
     cloneUrl = cloneUrl % (organization, repoName)
-    
-    if not os.path.exists(os.path.join(scipionHome,
-                                       repoName if cloneFolder == '' else cloneFolder)):
+    folderName = repoName if cloneFolder == '' else cloneFolder
+
+    if not os.path.exists(os.path.join(scipionHome, folderName)):
         cmd = cmdfy("git clone --branch %s %s %s" % (branch, cloneUrl,
                                                      cloneFolder))
     else:
-        print("%s repository detected, it will be updated." % repoName)
-        cmd = cmdfy("cd %s" % repoName)
+        print("%s repository detected, it will be updated." % folderName)
+        cmd = cmdfy("cd %s" % folderName)
         cmd += cmdfy("git pull")
         cmd += cmdfy("cd ..")
 
     if pipInstall:
         cmd += cmdfy("pip install -e %s" % repoName)
 
     return cmd
```

### Comparing `scipion-installer-1.0.8/scipioninstaller/launchers.py` & `scipion-installer-1.0.9/scipioninstaller/launchers.py`

 * *Files identical despite different names*

### Comparing `scipion-installer-1.0.8/setup.py` & `scipion-installer-1.0.9/setup.py`

 * *Files identical despite different names*

