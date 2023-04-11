# Comparing `tmp/asimtote-0.16.3.tar.gz` & `tmp/asimtote-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimtote-0.16.3.tar", last modified: Wed Mar  8 18:03:45 2023, max compression
+gzip compressed data, was "asimtote-0.16.4.tar", last modified: Tue Apr 11 13:20:31 2023, max compression
```

## Comparing `asimtote-0.16.3.tar` & `asimtote-0.16.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.619607 asimtote-0.16.3/
--rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.3/.gitignore
--rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.3/LICENSE
--rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-02-18 00:53:45.000000 asimtote-0.16.3/Makefile
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-03-08 18:03:45.619485 asimtote-0.16.3/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-02-03 17:20:21.000000 asimtote-0.16.3/README.md
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.611074 asimtote-0.16.3/asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-03-08 17:51:55.000000 asimtote-0.16.3/asimtote/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-02-12 10:32:19.000000 asimtote-0.16.3/asimtote/__main__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-02-16 00:53:49.000000 asimtote-0.16.3/asimtote/config.py
--rw-r--r--   0 rcf34      (503) staff       (20)    70795 2023-03-07 16:56:28.000000 asimtote-0.16.3/asimtote/diff.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.612572 asimtote-0.16.3/asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-02-16 12:18:04.000000 asimtote-0.16.3/asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.614015 asimtote-0.16.3/asimtote/ios/commands/
--rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-02-03 17:20:21.000000 asimtote-0.16.3/asimtote/ios/commands/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    16197 2023-03-02 17:26:39.000000 asimtote-0.16.3/asimtote/ios/commands/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     5131 2023-02-12 10:32:19.000000 asimtote-0.16.3/asimtote/ios/commands/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     7274 2023-03-03 16:17:01.000000 asimtote-0.16.3/asimtote/ios/commands/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    25758 2023-03-08 09:52:31.000000 asimtote-0.16.3/asimtote/ios/commands/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-02-12 10:32:19.000000 asimtote-0.16.3/asimtote/ios/config.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.615407 asimtote-0.16.3/asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      741 2023-02-15 23:28:23.000000 asimtote-0.16.3/asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    27064 2023-03-07 17:56:33.000000 asimtote-0.16.3/asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2957 2023-02-03 17:20:21.000000 asimtote-0.16.3/asimtote/ios/converters/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     6888 2023-03-03 16:17:01.000000 asimtote-0.16.3/asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    20419 2023-03-08 17:32:05.000000 asimtote-0.16.3/asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     4466 2023-02-15 23:09:59.000000 asimtote-0.16.3/asimtote/ios/diff.py
--rw-r--r--   0 rcf34      (503) staff       (20)    21673 2023-02-16 12:18:04.000000 asimtote-0.16.3/asimtote/ios/utils.py
--rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-02-15 22:30:09.000000 asimtote-0.16.3/asimtote/misc.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.611794 asimtote-0.16.3/asimtote.egg-info/
--rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-03-08 18:03:45.000000 asimtote-0.16.3/asimtote.egg-info/PKG-INFO
--rw-r--r--   0 rcf34      (503) staff       (20)     1192 2023-03-08 18:03:45.000000 asimtote-0.16.3/asimtote.egg-info/SOURCES.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-03-08 18:03:45.000000 asimtote-0.16.3/asimtote.egg-info/dependency_links.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       23 2023-03-08 18:03:45.000000 asimtote-0.16.3/asimtote.egg-info/requires.txt
--rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-03-08 18:03:45.000000 asimtote-0.16.3/asimtote.egg-info/top_level.txt
--rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-03-08 18:03:45.619643 asimtote-0.16.3/setup.cfg
--rwxr-xr-x   0 rcf34      (503) staff       (20)      807 2023-02-03 17:20:21.000000 asimtote-0.16.3/setup.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.615725 asimtote-0.16.3/test_asimtote/
--rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-02-18 00:55:48.000000 asimtote-0.16.3/test_asimtote/__main__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.616110 asimtote-0.16.3/test_asimtote/ios/
--rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-02-18 00:55:48.000000 asimtote-0.16.3/test_asimtote/ios/__init__.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.617250 asimtote-0.16.3/test_asimtote/ios/config/
--rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-02-18 00:55:48.000000 asimtote-0.16.3/test_asimtote/ios/config/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-03-07 17:53:07.000000 asimtote-0.16.3/test_asimtote/ios/config/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    13995 2023-02-18 00:55:48.000000 asimtote-0.16.3/test_asimtote/ios/config/lists.py
--rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-03-03 16:17:01.000000 asimtote-0.16.3/test_asimtote/ios/config/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-03-08 09:52:31.000000 asimtote-0.16.3/test_asimtote/ios/config/router.py
-drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-03-08 18:03:45.618979 asimtote-0.16.3/test_asimtote/ios/converters/
--rw-r--r--   0 rcf34      (503) staff       (20)      281 2023-03-08 17:49:26.000000 asimtote-0.16.3/test_asimtote/ios/converters/__init__.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-03-08 00:35:35.000000 asimtote-0.16.3/test_asimtote/ios/converters/cvtunittest.py
--rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-03-07 17:53:07.000000 asimtote-0.16.3/test_asimtote/ios/converters/interface.py
--rw-r--r--   0 rcf34      (503) staff       (20)    24193 2023-03-03 16:17:01.000000 asimtote-0.16.3/test_asimtote/ios/converters/other.py
--rw-r--r--   0 rcf34      (503) staff       (20)    67751 2023-03-08 17:49:26.000000 asimtote-0.16.3/test_asimtote/ios/converters/router.py
--rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-02-18 00:55:48.000000 asimtote-0.16.3/test_asimtote/ios/utils.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.312187 asimtote-0.16.4/
+-rw-r--r--   0 rcf34      (503) staff       (20)     1334 2023-02-01 17:57:38.000000 asimtote-0.16.4/.gitignore
+-rw-r--r--   0 rcf34      (503) staff       (20)     1101 2023-02-01 17:57:38.000000 asimtote-0.16.4/LICENSE
+-rw-r--r--   0 rcf34      (503) staff       (20)      297 2023-04-11 11:31:06.000000 asimtote-0.16.4/Makefile
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-11 13:20:31.312038 asimtote-0.16.4/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     3016 2023-04-11 11:31:06.000000 asimtote-0.16.4/README.md
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.305708 asimtote-0.16.4/asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)       45 2023-04-11 11:43:19.000000 asimtote-0.16.4/asimtote/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13909 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/__main__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    16544 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/config.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    71507 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/diff.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.307058 asimtote-0.16.4/asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      188 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.308038 asimtote-0.16.4/asimtote/ios/commands/
+-rw-r--r--   0 rcf34      (503) staff       (20)      719 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/commands/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    18303 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/commands/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     5931 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/commands/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     8074 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/commands/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    26719 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/commands/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     6134 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/config.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.308851 asimtote-0.16.4/asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      741 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    30179 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     3433 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     7707 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    43929 2023-04-11 11:42:51.000000 asimtote-0.16.4/asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     4753 2023-04-11 11:42:51.000000 asimtote-0.16.4/asimtote/ios/diff.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    22009 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/ios/utils.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     1492 2023-04-11 11:31:06.000000 asimtote-0.16.4/asimtote/misc.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.306362 asimtote-0.16.4/asimtote.egg-info/
+-rw-r--r--   0 rcf34      (503) staff       (20)     3483 2023-04-11 13:20:31.000000 asimtote-0.16.4/asimtote.egg-info/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)     1230 2023-04-11 13:20:31.000000 asimtote-0.16.4/asimtote.egg-info/SOURCES.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-04-11 13:20:31.000000 asimtote-0.16.4/asimtote.egg-info/dependency_links.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       23 2023-04-11 13:20:31.000000 asimtote-0.16.4/asimtote.egg-info/requires.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        9 2023-04-11 13:20:31.000000 asimtote-0.16.4/asimtote.egg-info/top_level.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-04-11 13:20:31.312228 asimtote-0.16.4/setup.cfg
+-rwxr-xr-x   0 rcf34      (503) staff       (20)      807 2023-04-11 11:31:06.000000 asimtote-0.16.4/setup.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.309207 asimtote-0.16.4/test_asimtote/
+-rw-r--r--   0 rcf34      (503) staff       (20)      149 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/__main__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.309478 asimtote-0.16.4/test_asimtote/ios/
+-rw-r--r--   0 rcf34      (503) staff       (20)      143 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/__init__.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.310332 asimtote-0.16.4/test_asimtote/ios/config/
+-rw-r--r--   0 rcf34      (503) staff       (20)      328 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/config/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    34207 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/config/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    14804 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/config/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     9991 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/config/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    60416 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/config/router.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-04-11 13:20:31.311604 asimtote-0.16.4/test_asimtote/ios/converters/
+-rw-r--r--   0 rcf34      (503) staff       (20)      336 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/converters/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2646 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/converters/cvtunittest.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    95324 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/converters/interface.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    13090 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/converters/lists.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    24193 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/converters/other.py
+-rw-r--r--   0 rcf34      (503) staff       (20)   152946 2023-04-11 11:42:51.000000 asimtote-0.16.4/test_asimtote/ios/converters/router.py
+-rw-r--r--   0 rcf34      (503) staff       (20)     2220 2023-04-11 11:31:06.000000 asimtote-0.16.4/test_asimtote/ios/utils.py
```

### Comparing `asimtote-0.16.3/.gitignore` & `asimtote-0.16.4/.gitignore`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/LICENSE` & `asimtote-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/PKG-INFO` & `asimtote-0.16.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.3
+Version: 0.16.4
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.3/README.md` & `asimtote-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/__main__.py` & `asimtote-0.16.4/asimtote/__main__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/config.py` & `asimtote-0.16.4/asimtote/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/diff.py` & `asimtote-0.16.4/asimtote/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,22 +431,37 @@
         """Get the non-extended path for this converter (i.e. the
         'context' and 'cmd' paths joined, excluding the 'ext').
         """
 
         return self.context + self.cmd
 
 
-    def get_sorting_key(self):
+    def _get_full_sort_key(self):
+        """Get the full key used to order the converters within a block.
+
+        This consists of the context with the result of get_sort_key()
+        appended, and with all the None (wildcard) elements replaced
+        with the empty string.
+        """
+
+        key = self.context + self.get_sort_key()
+        return [ "" if i is None else i for i in key ]
+
+
+    def get_sort_key(self):
         """This method returns the key to be used for ordering the
-        converters.  By default, this returns the full path (which is
-        context + cmd + ext; see the constructor) but it can be modified
-        to adjust the order in which converters operate, within a block.
+        converters.  By default, this returns the command and extension
+        path (cmd + ext) but it can be modified to adjust the order in
+        which converters operate, within a block.
+
+        The _get_full_sort_key() method is used to retrieve the full
+        key that is used for sorting (which includes the context).
         """
 
-        return self._path_full
+        return self.cmd + self.ext
 
 
     def get_match_context(self, match):
         """Return the context portion of a particular match for this
         converter.
 
         This is used when a trigger is set, to extract the context of a
@@ -894,15 +909,15 @@
         but can be overridden, if required.
 
         This method is called by the constructor, after the converters
         have been added to ensure a consist order.
         """
 
         for block in self._cvts:
-            self._cvts[block].sort(key=lambda c: c.get_sorting_key())
+            self._cvts[block].sort(key=lambda c: c._get_full_sort_key())
 
 
     def _explain_comment(self, path):
         """This method returns a comment or other configuration item
         explaining the path supplied (which will typically be a match
         against a converter).  The path is supplied a list of levels and
         converted to a string using pathstr().
@@ -1379,18 +1394,45 @@
 
             for match in all_matches:
                 # handle REMOVE conversions, if matching
 
                 if match in remove_matches:
                     debug_msg = []
 
+
+                    # check if anything remains at this level or below
+                    # in the new configuration - if it does, we're doing
+                    # a partial removal
+
+                    remove_is_truncate = False
+
+                    try:
+                        # we don't want the result here, just to find
+                        # out if the path exists (if not, KeyError will
+                        # be raised)
+                        deepget(new_cfg, *match, default_error=True)
+
+                    except KeyError:
+                        # nothing remains so we're doing a full remove
+                        pass
+
+                    else:
+                        # something remains so this is partial
+                        if self._debug_convert >= DEBUG_CONVERT_STEPS:
+                            debug_msg.append(
+                                "-> subconfiguration not empty - truncate")
+                        remove_is_truncate = True
+
+
                     if self._debug_convert >= DEBUG_CONVERT_MATCH:
                         debug_msg.append(
-                            "=> remove match: "
-                                + pathstr(match, cvt.wildcard_indices))
+                            "=> "
+                            + ("truncate" if remove_is_truncate else "remove")
+                            + " match: "
+                            + pathstr(match, cvt.wildcard_indices))
 
 
                     # get elements in the path matching wildcards
 
                     args = cvt.get_wildcard_args(match)
 
 
@@ -1428,38 +1470,14 @@
                                 debug_msg,
                                 blank_if_single=
                                     self._debug_convert > DEBUG_CONVERT_MATCH)
 
                         continue
 
 
-                    # check if anything remains at this level or below
-                    # in the new configuration - if it does, we're doing
-                    # a partial removal
-
-                    remove_is_truncate = False
-
-                    try:
-                        # we don't want the result here, just to find
-                        # out if the path exists (if not, KeyError will
-                        # be raised)
-                        deepget(new_cfg, *match, default_error=True)
-
-                    except KeyError:
-                        # nothing remains so we're doing a full remove
-                        pass
-
-                    else:
-                        # something remains so this is partial
-                        if self._debug_convert >= DEBUG_CONVERT_STEPS:
-                            debug_msg.append(
-                                "-> subconfiguration not empty - truncate")
-                        remove_is_truncate = True
-
-
                     # get the old, remove and new parts of the
                     # configuration and remove difference dictionaries,
                     # for the path specified in the converter (ignoring
                     # the extension 'ext')
 
                     cvt_old = cvt.get_cfg(old_cfg, match)
                     cvt_rem = cvt.get_cfg(remove_cfg_full, match)
@@ -1593,18 +1611,36 @@
 
 
                 # handle UPDATE conversions, if matching
 
                 if match in update_matches:
                     debug_msg = []
 
+
+                    # check if there is anything for this level in the
+                    # old configuration - if not, we're actually adding
+                    # this, rather than updating it, so record that
+
+                    update_is_add = False
+
+                    try:
+                        deepget(old_cfg, *match, default_error=True)
+
+                    except KeyError:
+                        if self._debug_convert >= DEBUG_CONVERT_STEPS:
+                            debug_msg.append("-> no old configuration - add")
+                        update_is_add = True
+
+
                     if self._debug_convert >= DEBUG_CONVERT_MATCH:
                         debug_msg.append(
-                            "=> update match: "
-                                + pathstr(match, cvt.wildcard_indices))
+                            "=> "
+                            + ("add" if update_is_add else "update")
+                            + " match: "
+                            + pathstr(match, cvt.wildcard_indices))
 
 
                     # (same as in remove, above)
 
                     args = cvt.get_wildcard_args(match)
 
                     try:
@@ -1622,29 +1658,14 @@
                     if not filtered:
                         if self._debug_convert >= DEBUG_CONVERT_NODIFF:
                             debug_msg.append("-> filtered - skip")
                             self._print_debug(debug_msg)
                         continue
 
 
-                    # check if there is anything for this level in the
-                    # old configuration - if not, we're actually adding
-                    # this, rather than updating it, so record that
-
-                    update_is_add = False
-
-                    try:
-                        deepget(old_cfg, *match, default_error=True)
-
-                    except KeyError:
-                        if self._debug_convert >= DEBUG_CONVERT_STEPS:
-                            debug_msg.append("-> no old configuration - add")
-                        update_is_add = True
-
-
                     # get the old, update and new parts of the
                     # configuration difference dictionaries, for the
                     # path specified in the converter (ignoring the
                     # extension 'ext')
 
                     cvt_old = cvt.get_cfg(old_cfg, match)
                     cvt_upd = cvt.get_cfg(update_cfg, match)
```

### Comparing `asimtote-0.16.3/asimtote/ios/commands/__init__.py` & `asimtote-0.16.4/asimtote/ios/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/ios/commands/interface.py` & `asimtote-0.16.4/asimtote/ios/commands/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# adimtote.ios.commands.interface
+# asimtote.ios.commands.interface
 #
 # Copyright (C) Robert Franklin <rcf34@cam.ac.uk>
 
 
 
 # --- imports ---
 
@@ -92,15 +92,19 @@
 class Cmd_Int_IPAccGrp(CmdContext_Int):
     match = r"ip access-group (?P<acl_name>\S+) (?P<dir_>in|out)"
 
     def parse(self, cfg, acl_name, dir_):
         cfg.setdefault("ip-access-group", {})[dir_] = acl_name
 
 
+
+# =============================================================================
 # ip address ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPAddr(CmdContext_Int):
     match = r"ip address (?P<addr>\S+ \S+)"
 
     def parse(self, cfg, addr):
         # TODO: should parse to fields and canonicalise address
@@ -112,15 +116,19 @@
 
     def parse(self, cfg, addr):
         # secondary address - record it in a set
         # TODO: should parse to fields and canonicalise address
         cfg.setdefault("ip-address-secondary", set()).add(addr)
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPFlowMon(CmdContext_Int):
     match = r"ip flow monitor (?P<flowmon>\S+) (?P<dir_>input|output)"
 
     def parse(self, cfg, flowmon, dir_):
         deepsetdefault(cfg, "ip-flow-monitor")[dir_] = flowmon
@@ -154,15 +162,19 @@
 class Cmd_Int_IPMcastBdry(CmdContext_Int):
     match = r"ip multicast boundary (?P<acl>\S+)"
 
     def parse(self, cfg, acl):
         cfg["ip-multicast-boundary"] = acl
 
 
+
+# =============================================================================
 # ip ospf ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPOSPFArea(CmdContext_Int):
     match = r"ip ospf (?P<proc>\d+) area (?P<area>[.0-9]+)"
 
     def parse(self, cfg, proc, area):
         a = deepsetdefault(cfg, "ip-ospf", "area")
@@ -211,15 +223,19 @@
     match = (r"ip ospf network (?P<net>broadcast|non-broadcast|"
              r"point-to-multipoint|point-to-point)")
 
     def parse(self, cfg, net):
         cfg.setdefault("ip-ospf", {})["network"] = net
 
 
+
+# =============================================================================
 # ip pim ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPPIMMode(CmdContext_Int):
     match = r"ip pim ((?P<mode>sparse|dense|sparse-dense)-mode)"
 
     def parse(self, cfg, mode):
         cfg.setdefault("ip-pim", {})["mode"] = mode
@@ -228,15 +244,19 @@
 class Cmd_Int_IPPIMBSRBdr(CmdContext_Int):
     match = r"ip pim bsr-border"
 
     def parse(self, cfg):
         cfg.setdefault("ip-pim", {})["bsr-border"] = True
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPPolicyRtMap(CmdContext_Int):
     match = r"ip policy route-map (?P<rtmap>\S+)"
 
     def parse(self, cfg, rtmap):
         cfg["ip-policy-route-map"] = rtmap
@@ -253,15 +273,19 @@
     match = r"ip verify unicast (?P<opt>.+)"
 
     def parse(self, cfg, opt):
         # TODO: should parse to fields
         cfg["ip-verify-unicast"] = opt
 
 
+
+# =============================================================================
 # ipv6 ...
+# =============================================================================
+
 
 
 class Cmd_Int_IPv6Addr(CmdContext_Int):
     match = r"ipv6 address (?P<addr>\S+)"
 
     def parse(self, cfg, addr):
         # IPv6 addresses involve letters so we lower case for
@@ -363,15 +387,19 @@
     match = r"ipv6 verify unicast (?P<opt>.+)"
 
     def parse(self, cfg, opt):
         # TODO: should parse to fields
         cfg["ipv6-verify-unicast"] = opt
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_MPLSIP(CmdContext_Int):
     match = r"mpls ip"
 
     def parse(self, cfg):
         cfg["mpls-ip"] = True
@@ -380,15 +408,19 @@
 class Cmd_Int_MTU(CmdContext_Int):
     match = r"mtu (?P<size>\d+)"
 
     def parse(self, cfg, size):
         cfg["mtu"] = int(size)
 
 
+
+# =============================================================================
 # ospfv3 ...
+# =============================================================================
+
 
 
 class Cmd_Int_OSPFv3Area(CmdContext_Int):
     match = r"ospfv3 (?P<proc>\d+) (?P<proto>ipv[46]) area (?P<area>[.0-9]+)"
 
     def parse(self, cfg, proc, proto, area):
         a = deepsetdefault(cfg, "ospfv3", "area", proto)
@@ -421,15 +453,19 @@
     match = (r"ospfv3 network (?P<net>broadcast|non-broadcast|"
              r"point-to-multipoint|point-to-point)")
 
     def parse(self, cfg, net):
         cfg.setdefault("ospfv3", {})["network"] = net
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_ServPol(CmdContext_Int):
     match = (r"service-policy( type (?P<type_>\S+))? (?P<dir_>input|output)"
              r" (?P<policy>\S+)")
 
     def parse(self, cfg, type_, dir_, policy):
@@ -439,15 +475,19 @@
 class Cmd_Int_Shutdown(CmdContext_Int):
     match = r"(?P<no>no )?shutdown"
 
     def parse(self, cfg, no):
         cfg["shutdown"] = not no
 
 
+
+# =============================================================================
 # standby ...
+# =============================================================================
+
 
 
 class Cmd_Int_StandbyIP(CmdContext_Int):
     match = r"standby (?P<grp>\d+) ip (?P<addr>\S+)"
 
     def parse(self, cfg, grp, addr):
         deepsetdefault(
@@ -508,26 +548,34 @@
 class Cmd_Int_StandbyVer(CmdContext_Int):
     match = r"standby version (?P<ver>[12])"
 
     def parse(self, cfg, ver):
         deepsetdefault(cfg, "standby")["version"] = int(ver)
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_StormCtrl(CmdContext_Int):
     match = (r"storm-control (?P<traffic>unicast|multicast|broadcast)"
              r" level (?P<level>[0-9.]+)")
 
     def parse(self, cfg, traffic, level):
         deepsetdefault(cfg, "storm-control")[traffic] = float(level)
 
 
+
+# =============================================================================
 # switchport ...
+# =============================================================================
+
 
 
 class Cmd_Int_SwPort(CmdContext_Int):
     match = r"(?P<no>no )?switchport"
 
     def parse(self, cfg, no):
         cfg["switchport"] = not no
@@ -573,15 +621,19 @@
             cfg.setdefault("switchport-trunk-allow", set()).update(
                 expand_set(vlans))
 
         else:
             cfg["switchport-trunk-allow"] = expand_set(vlans)
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cmd_Int_PcMinLinks(CmdContext_Int):
     match = r"port-channel min-links (?P<links>\d+)"
 
     def parse(self, cfg, links):
         cfg["port-channel-min-links"] = int(links)
```

### Comparing `asimtote-0.16.3/asimtote/ios/commands/lists.py` & `asimtote-0.16.4/asimtote/ios/commands/lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 
 # --- configuration command classes ---
 
 
 
+# =============================================================================
 # ip access-list standard ...
+# =============================================================================
 
 
 
 class Cmd_ACLStdRule(IndentedContextualCommand):
     match = r"access-list (?P<num>\d{1,2}|1[3-9]\d{2}) (?P<rule>.+)"
 
     def parse(self, cfg, num, rule):
@@ -55,15 +57,17 @@
         # store the rule at the specified sequence number, or 10 greater
         # than the maximum existing rule number, or 10 if the list is
         # empty
         cfg[int(seq) if seq else ((max(cfg) + 10) if cfg else 10)] = rule
 
 
 
+# =============================================================================
 # ip access-list extended ...
+# =============================================================================
 
 
 
 class Cmd_ACLExtRule(IndentedContextualCommand):
     match = r"access-list (?P<num>1\d{2}|2[0-6]\d{2}) (?P<rule>(permit|deny) .+)"
 
     def parse(self, cfg, num, rule):
@@ -88,15 +92,17 @@
             return
 
         cfg[int(seq) if seq else ((max(cfg) + 10) if cfg else 10)] = (
             ip_acl_ext_rule_canonicalize(rule))
 
 
 
+# =============================================================================
 # ipv6 access-list ...
+# =============================================================================
 
 
 
 class Cmd_IPv6ACL(IndentedContextualCommand):
     match = r"ipv6 access-list (?P<name>.+)"
     enter_context = "ipv6-acl"
 
@@ -113,15 +119,17 @@
         # with the same sequence number as an existing rule will replace
         # it, rather than produce an error
         cfg[int(seq) if seq else ((max(cfg) + 10) if cfg else 10)] = (
             ipv6_acl_rule_canonicalize(rule))
 
 
 
+# =============================================================================
 # ip as-path access-list ...
+# =============================================================================
 
 
 
 class Cmd_IPASPathACL(IndentedContextualCommand):
     match = (r"ip as-path access-list (?P<num>\d+) (?P<action>permit|deny)"
              r" (?P<re>\S+)")
 
@@ -129,15 +137,17 @@
         # an AS path access-list is just a sequence of tuples giving the
         # action and the regexp
         l = deepsetdefault(cfg, "ip-as-path-access-list", int(num), last=[])
         l.append( (action, re) )
 
 
 
+# =============================================================================
 # ip[v6] prefix-list ...
+# =============================================================================
 
 
 
 class Cmd_IPPfxList(IndentedContextualCommand):
     match = (r"ip prefix-list (?P<list_>\S+)( seq (?P<seq>\d+))? "
              r"(?P<rule>(permit|deny) .+)")
```

### Comparing `asimtote-0.16.3/asimtote/ios/commands/other.py` & `asimtote-0.16.4/asimtote/ios/commands/other.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 
 
 # --- configuration command classes ---
 
 
 
+# =============================================================================
 # system
+# =============================================================================
 
 
 
 class Cmd_Comment(IndentedContextualCommand):
     # we don't really need to match comments as they do nothing but it
     # avoids chugging through the entire list of commands and doing
     # nothing
@@ -35,15 +37,17 @@
     match = r"hostname (?P<hostname>\S+)"
 
     def parse(self, cfg, hostname):
         cfg["hostname"] = hostname
 
 
 
+# =============================================================================
 # [no] spanning-tree ...
+# =============================================================================
 
 
 
 class Cmd_NoSTP(IndentedContextualCommand):
     match = r"no spanning-tree vlan (?P<tags>[-0-9,]+)"
 
     def parse(self, cfg, tags):
@@ -57,15 +61,17 @@
     def parse(self, cfg, tags, pri):
         cfg_stp_pri = cfg.setdefault("spanning-tree-vlan-priority", {})
         for tag in expand_set(tags):
             cfg_stp_pri[int(tag)] = int(pri)
 
 
 
+# =============================================================================
 # track ...
+# =============================================================================
 
 
 
 class Cmd_TrackModify(IndentedContextualCommand):
     match = r"track (?P<obj>\d+)"
     enter_context = "track"
 
@@ -178,15 +184,17 @@
     match = r"object (?P<obj>.+)"
 
     def parse(self, cfg, obj):
         deepsetdefault(cfg, "object", last=set()).add(int(obj))
 
 
 
+# =============================================================================
 # vlan ...
+# =============================================================================
 
 
 
 class Cmd_VLAN(IndentedContextualCommand):
     match = r"vlan (?P<tag>\d+)"
     enter_context = "vlan"
 
@@ -210,15 +218,17 @@
     match = r"name (?P<name>.+)"
 
     def parse(self, cfg, name):
         cfg["name"] = name.strip()
 
 
 
+# =============================================================================
 # vrf ...
+# =============================================================================
 
 
 
 class Cmd_VRF(IndentedContextualCommand):
     match = r"vrf definition (?P<name>\S+)"
     enter_context = "vrf"
```

### Comparing `asimtote-0.16.3/asimtote/ios/commands/router.py` & `asimtote-0.16.4/asimtote/ios/commands/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 
 
 
 # --- configuration command classes ---
 
 
 
+# =============================================================================
 # ip[v6] route ...
+# =============================================================================
 
 
 
 class Cmd_IPRoute(IndentedContextualCommand):
     match = (r"ip route( vrf (?P<vrf>\S+))? (?P<base>\S+) (?P<netmask>\S+)"
              r"( (?P<int_name>[-A-Za-z]+[0-9/.]+))?( (?P<router>[0-9.]+))?"
              r"( (?P<metric1>\d+))?( tag (?P<tag>\d+))?( (?P<metric2>\d+))?")
@@ -98,15 +100,17 @@
         if tag:
             r["tag"] = int(tag)
 
         deepsetdefault(cfg, "ipv6-route", vrf, net)[id] = r
 
 
 
+# =============================================================================
 # route-map ...
+# =============================================================================
 
 
 
 class Cmd_RtMap(IndentedContextualCommand):
     match = (r"route-map (?P<rtmap>\S+)( (?P<action>permit|deny))?"
              r"( (?P<seq>\d+))?")
     enter_context = "route-map"
@@ -258,15 +262,17 @@
     def parse(self, cfg, vrf):
         # the global routing table is indicated by an empty string VRF
         # setting
         deepsetdefault(cfg, "set", "vrf", last=vrf or "")
 
 
 
+# =============================================================================
 # router bgp ...
+# =============================================================================
 
 
 
 class Cmd_RtrBGP(IndentedContextualCommand):
     # ASNs can be in 'n' as well as 'n.n' format so we can't just use an
     # integer
     match = r"router bgp (?P<asn>\d+(\.\d+)?)"
@@ -353,15 +359,19 @@
 
     def parse(self, cfg, nbr, int_name):
         deepsetdefault(
             cfg["neighbor"][neighbor_canonicalize(nbr)])["update-source"] = (
                 int_name)
 
 
+
+# =============================================================================
 # router bgp ... address-family ... [vrf ...]
+# =============================================================================
+
 
 
 class Cmd_RtrBGP_AF(CmdContext_RtrBGP):
     # this regexp will match 'vpnv[46] vrf ...' which is illegal, but we're
     # not trying to validate commands
     match = (r"address-family (?P<af>ipv[46]( (?P<cast>unicast|multicast))?|"
              r"vpnv4|vpnv6)( vrf (?P<vrf>\S+))?")
@@ -417,15 +427,14 @@
             a["all"] = True
         if best_n:
             a["best"] = int(best_n)
         if grp_best:
             a["group-best"] = True
 
 
-
 class Cmd_RtrBGP_AF_NbrAlwAS(CmdContext_RtrBGP_AF):
     match = r"neighbor (?P<nbr>\S+) allowas-in( (?P<max>\d+))?"
 
     def parse(self, cfg, nbr, max):
         # we can't just use None for an empty 'allowas-in' maximum as
         # this cannot be changed to, as a different type
         n = deepsetdefault(cfg, "neighbor", neighbor_canonicalize(nbr))
@@ -602,15 +611,17 @@
         if rtmap:
             r["route-map"] = rtmap
         if met:
             r["metric"] = int(met)
 
 
 
+# =============================================================================
 # router ospf ...
+# =============================================================================
 
 
 
 # this function is used for both ospf and ospfv3 so is shared
 
 def _ospf_passive_interface(cfg, int_name, passive):
     """This function maintains a "passive-interface" dictionary under
@@ -712,15 +723,17 @@
     match = r"(?P<no>no )?passive-interface (?P<int_name>\S+)"
 
     def parse(self, cfg, no, int_name):
         _ospf_passive_interface(cfg, int_name, not no)
 
 
 
+# =============================================================================
 # router ospfv3 ...
+# =============================================================================
 
 
 
 class Cmd_RtrOSPFv3(IndentedContextualCommand):
     match = r"router ospfv3 (?P<proc>\d+)"
     enter_context = "router-ospfv3"
```

### Comparing `asimtote-0.16.3/asimtote/ios/config.py` & `asimtote-0.16.4/asimtote/ios/config.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/ios/converters/__init__.py` & `asimtote-0.16.4/asimtote/ios/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote/ios/converters/interface.py` & `asimtote-0.16.4/asimtote/ios/converters/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,28 +45,42 @@
 class DiffConvert_Int(DiffConvert):
     context = Cvt_Int.cmd
 
     def enter(self, int_name):
         return ["interface " + int_name]
 
 
+
+# =============================================================================
+# shutdown
+# =============================================================================
+
+
+
 # we put the 'interface / shutdown' at the start to shut it down before
 # we do any [re]configuration
 
 class Cvt_Int_Shutdown(DiffConvert_Int):
     cmd = "shutdown",
     block = "int-shutdown"
 
     def update(self, old, upd, new, int_name):
         # we only 'shutdown' if we are disabling the port ('no shutdown'
         # happens at the end of interface configuration)
         if new:
             return self.enter(int_name) + [" shutdown"]
 
 
+
+# =============================================================================
+# ...
+# =============================================================================
+
+
+
 # converter to detect a VRF change and fire a trigger to make changes
 # required before it is actually changed
 
 class Cvt_VRFTrgr_VRFFwd(DiffConvert_Int):
     cmd = "vrf-forwarding",
     block = "int-vrf-trigger"
     trigger_blocks = { "int-vrf-pre" }
@@ -151,15 +165,19 @@
     def remove(self, old, int_name, dir_):
         return self.enter(int_name) + [" no ip access-group " + dir_]
 
     def update(self, old, upd, new, int_name, dir_):
         return self.enter(int_name) + [" ip access-group %s %s" % (new, dir_)]
 
 
+
+# =============================================================================
 # ip address ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPAddr(DiffConvert_Int):
     cmd = "ip-address",
     block = "int-vrf-post"
 
     def remove(self, old, int_name):
@@ -176,15 +194,19 @@
     def remove(self, old, int_name, addr):
         return self.enter(int_name) + [" no ip address %s secondary" % addr]
 
     def update(self, old, upd, new, int_name, addr):
         return self.enter(int_name) + [" ip address %s secondary" % addr]
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPFlowMon(DiffConvert_Int):
     cmd = "ip-flow-monitor", None
 
     def remove(self, old, int_name, dir_):
         return self.enter(int_name) + [
@@ -197,16 +219,21 @@
         if old:
             l += [" no ip flow monitor %s %s" % (old, dir_)]
 
         l += [" ip flow monitor %s %s" % (new, dir_)]
         return l
 
 
+
+# =============================================================================
 # ip helper-address ...
-#
+# =============================================================================
+
+
+
 # This command is odd in that changing VRF causes it to be modified but
 # not removed (as configuration items mentioning IP addresses are).  For
 # example, if the interface is not in a VRF but is being moved into one,
 # the VRF change will cause it to change to 'ip helper-address global
 # ADDR'; removing it from a VRF change it to 'ip helper-address vrf
 # VRF-NAME ADDR'.
 #
@@ -253,15 +280,19 @@
 
     # removing helper addresses is done before the VRF changes
 
     def update(self, old, upd, new, int_name, helper):
         return self.enter(int_name) + [" " + self._cmd(new)]
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPIGMPVer(DiffConvert_Int):
     cmd = "ip-igmp-version",
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip igmp version"]
@@ -276,15 +307,19 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip multicast boundary"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ip multicast boundary " + new]
 
 
-# ip-ospf ...
+
+# =============================================================================
+# ip ospf ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPOSPFArea(DiffConvert_Int):
     cmd = "ip-ospf", "area"
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [
@@ -353,15 +388,19 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip ospf network"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ip ospf network " + new]
 
 
-# ip-pim ...
+
+# =============================================================================
+# ip pim ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPPIMMode(DiffConvert_Int):
     cmd = "ip-pim", "mode"
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip pim %s-mode" % old]
@@ -377,15 +416,19 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip pim bsr-border"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ip pim bsr-border"]
 
 
+
+# =============================================================================
 # ip (other) ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPPolicyRtMap(DiffConvert_Int):
     cmd = "ip-policy-route-map",
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip policy route-map"]
@@ -414,15 +457,19 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ip verify unicast"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ip verify unicast " + new]
 
 
+
+# =============================================================================
 # ipv6 ...
+# =============================================================================
+
 
 
 class Cvt_Int_IPv6Addr(DiffConvert_Int):
     cmd = "ipv6-address", None
     block = "int-vrf-post"
 
     def remove(self, old, int_name, addr):
@@ -498,28 +545,36 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ipv6 verify unicast"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ipv6 verify unicast " + new]
 
 
+
+# =============================================================================
 # mpls ...
+# =============================================================================
+
 
 
 class Cvt_Int_MPLSIP(DiffConvert_Int):
     cmd = "mpls-ip",
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no mpls ip"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" mpls ip"]
 
 
+
+# =============================================================================
 # mtu ...
+# =============================================================================
+
 
 
 class Cvt_Int_MTU(DiffConvert_Int):
     cmd = tuple()
     ext = "mtu",
 
     def remove(self, old, int_name):
@@ -534,15 +589,19 @@
         # TODO: handle what happens if interface converting to channel-group
         if new and "channel-group" in new:
             return None
 
         return self.enter(int_name) + [" mtu " + str(self.get_ext(new))]
 
 
+
+# =============================================================================
 # ospfv3 ...
+# =============================================================================
+
 
 
 class Cvt_Int_OSPFv3Area(DiffConvert_Int):
     cmd = "ospfv3", "area", None
 
     def remove(self, old, int_name, proto):
         return self.enter(int_name) + [
@@ -591,15 +650,19 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no ospfv3 network"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" ospfv3 network " + new]
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cvt_Int_ServPol(DiffConvert_Int):
     cmd = "service-policy", None, None
 
     def _cmd(self, type_, dir_, name):
         return ("service-policy"
@@ -618,15 +681,19 @@
             l.append(" no " + self._cmd(type_, dir_, old))
 
         l.append(" " + self._cmd(type_, dir_, new))
 
         return l
 
 
+
+# =============================================================================
 # standby ...
+# =============================================================================
+
 
 
 class Cvt_Int_NoStandbyIPSec(DiffConvert_Int):
     cmd = "standby", "group", None, "ip-secondary", None
     block = "int-vrf-pre"
 
     def remove(self, old, int_name, grp, addr):
@@ -733,29 +800,37 @@
         # only set this here if we're switching to version < 2 (so we
         # need to do it after removing all the high-numbered groups)
         if new >= 2:
             return
         return self.enter(int_name) + [" standby version " + str(new)]
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cvt_Int_StormCtrl(DiffConvert_Int):
     cmd = "storm-control", None
 
     def remove(self, old, int_name, traffic):
         return self.enter(int_name) + [" no storm-control %s level" % traffic]
 
     def update(self, old, upd, new, int_name, traffic):
         return self.enter(int_name) + [
                    " storm-control %s level %.2f" % (traffic, new)]
 
 
+
+# =============================================================================
 # switchport ...
+# =============================================================================
+
 
 
 class Cvt_Int_SwPort(DiffConvert_Int):
     cmd = "switchport",
 
     def remove(self, old, int_name):
         # if the 'switchport' option is not present, that doesn't mean
@@ -859,15 +934,19 @@
 
         for tag in sorted(self.get_ext(upd)):
             l.append(" switchport trunk allowed vlan add " + str(tag))
 
         return l
 
 
+
+# =============================================================================
 # ...
+# =============================================================================
+
 
 
 class Cvt_Int_PcMinLinks(DiffConvert_Int):
     cmd = "port-channel-min-links",
 
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no port-channel min-links"]
@@ -882,14 +961,21 @@
     def remove(self, old, int_name):
         return self.enter(int_name) + [" no xconnect"]
 
     def update(self, old, upd, new, int_name):
         return self.enter(int_name) + [" xconnect " + new]
 
 
+
+# =============================================================================
+# no shutdown
+# =============================================================================
+
+
+
 # we put the 'interface / no shutdown' at the end to only enable the
 # interface once it's been correctly [re]configured
 
 class Cvt_Int_NoShutdown(DiffConvert_Int):
     cmd = "shutdown",
     block = "int-noshutdown"
```

### Comparing `asimtote-0.16.3/asimtote/ios/converters/lists.py` & `asimtote-0.16.4/asimtote/ios/converters/lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 
 
 # --- converter classes ---
 
 
 
-# IP[V6] ACCESS-LIST ...
+# =============================================================================
+# ip[v6] access-list ...
+# =============================================================================
 
 
 
 class Cvt_IPACL_Std(DiffConvert):
     cmd = "ip-access-list-standard", None
 
     def remove(self, old, acl_name):
@@ -48,15 +50,15 @@
         if old:
             r.append("no ip access-list extended " + acl_name)
         r.append("ip access-list extended " + acl_name)
         r.extend(explain_diffs(old, new, indent=" "))
         return r
 
 
-class Cvt_IPv6ACL_Ext(DiffConvert):
+class Cvt_IPv6ACL(DiffConvert):
     cmd = "ipv6-access-list", None
 
     def remove(self, old, acl_name):
         return "no ipv6 access-list " + acl_name
 
     def update(self, old, upd, new, acl_name):
         r = []
@@ -64,15 +66,17 @@
             r.append("no ipv6 access-list " + acl_name)
         r.append("ipv6 access-list " + acl_name)
         r.extend(explain_diffs(old, new, indent=" "))
         return r
 
 
 
-# IP AS-PATH ACCESS-LIST ...
+# =============================================================================
+# ip as-path access-list ...
+# =============================================================================
 
 
 
 class Cvt_IPASPathACL(DiffConvert):
     cmd = "ip-as-path-access-list", None
 
     def to_str(self, rule):
@@ -88,15 +92,17 @@
             r += ["no ip as-path access-list " + str(num)]
         r += explain_diffs(old, new, prefix="ip as-path access-list %d " % num,
                            to_str_func=self.to_str)
         return r
 
 
 
-# IP[V6] PREFIX-LIST ...
+# =============================================================================
+# ip[v6] prefix-list ...
+# =============================================================================
 
 
 
 class Cvt_IPPfxList(DiffConvert):
     cmd = "ip-prefix-list", None
 
     def remove(self, old, pfx_name):
```

### Comparing `asimtote-0.16.3/asimtote/ios/converters/other.py` & `asimtote-0.16.4/asimtote/ios/converters/other.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# asimtote.ios.converters.all
+# asimtote.ios.converters.other
 #
 # Copyright (C) Robert Franklin <rcf34@cam.ac.uk>
 
 
 
 # --- imports ---
 
@@ -12,30 +12,34 @@
 
 
 
 # --- converter classes ---
 
 
 
-# SYSTEM
+# =============================================================================
+# hostname ...
+# =============================================================================
 
 
 
 class Cvt_Hostname(DiffConvert):
     cmd = "hostname",
 
     def remove(self, old):
         return "no hostname"
 
     def update(self, old, upd, new):
         return "hostname " + new
 
 
 
-# [NO] SPANNING-TREE ...
+# =============================================================================
+# [no] spanning-tree ...
+# =============================================================================
 
 
 
 class Cvt_NoSTP(DiffConvert):
     cmd = "no-spanning-tree-vlan", None
 
     def remove(self, old, tag):
@@ -54,15 +58,17 @@
         return "no spanning-tree vlan %d priority" % tag
 
     def update(self, old, upd, new, tag):
         return "spanning-tree vlan %d priority %d" % (tag, new)
 
 
 
-# TRACK ...
+# =============================================================================
+# track ...
+# =============================================================================
 
 
 
 # the track command is odd in that it doesn't allow the type of tracking
 # object to be changed (e.g. from an interface to a route) and must be
 # destroyed and created anew
 #
@@ -185,15 +191,17 @@
         return self.enter(obj) + [" no object " + str(sub_obj)]
 
     def update(self, old, upd, new, obj, sub_obj):
         return self.enter(obj) + [" object " + str(sub_obj)]
 
 
 
-# VLAN ...
+# =============================================================================
+# vlan ...
+# =============================================================================
 
 
 
 class Cvt_VLAN(DiffConvert):
     cmd = "vlan", None
 
     def remove(self, old, tag):
@@ -211,15 +219,17 @@
         return "vlan " + str(tag), " no name"
 
     def update(self, old, upd, new, tag):
         return "vlan " + str(tag), " name " + new
 
 
 
-# VRF ...
+# =============================================================================
+# vrf definition ...
+# =============================================================================
 
 
 
 class Cvt_VRF(DiffConvert):
     cmd = "vrf", None
 
     def remove(self, old, name):
```

### Comparing `asimtote-0.16.3/asimtote/ios/diff.py` & `asimtote-0.16.4/asimtote/ios/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,20 @@
             # tracking objects are deleted in the 'None' block,
             # including if they are changing type; the new object is
             # then created, then the sub-configuration (which may need
             # to be triggered after a type change, to be reapplied)
             "track-create",
             "track-sub",
 
+            # if changing a BGP neighbor peer-group, we need to delete
+            # the neighbor first and recreate it, which means we need
+            # to re apply the 'activate' with a trigger, so have to have
+            # a separate block for that
+            "bgp-nbr-activate",
+
             # if we're enabling interfaces, we do that after we've done
             # all the other configuration on them
             "int-noshutdown",
         ]
 
 
     def _add_converters(self):
```

### Comparing `asimtote-0.16.3/asimtote/ios/utils.py` & `asimtote-0.16.4/asimtote/ios/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,20 @@
     interact around.  Presumably this is done to optimise processing.
 
     The solution adopted here is to build the ACLs up in blocks.  Each
     block is a set of rules where the address portions don't overlap;
     these are built, sorting each block into address order, before
     adding the sorted rules in the block into the resulting list.
 
+    Note that this can result in 'permit' and 'deny' entries swapping
+    order, as long as the addresses don't overlap.  For example, 'permit
+    host 20.0.0.1', 'deny host 10.0.0.1' would be reversed into 'deny
+    host 10.0.0.1', 'permit host 20.0.0.1' as the rules are organised
+    into addresses order ('10.0.0.1' < '20.0.0.1').
+
     The result is lists which are not necessarily in the same order as
     they were constructed, nor how IOS stores them, but two lists should
     at least be in the same order so they can be directly compared.
 
     This function is applied to each list, after the configuration is
     read, and the returned list used to replace the order in which the
     rules were read.
```

### Comparing `asimtote-0.16.3/asimtote/misc.py` & `asimtote-0.16.4/asimtote/misc.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/asimtote.egg-info/PKG-INFO` & `asimtote-0.16.4/asimtote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimtote
-Version: 0.16.3
+Version: 0.16.4
 Summary: Compare network device configuration files using contextual structures
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/asimtote
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimtote-0.16.3/asimtote.egg-info/SOURCES.txt` & `asimtote-0.16.4/asimtote.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 test_asimtote/ios/config/interface.py
 test_asimtote/ios/config/lists.py
 test_asimtote/ios/config/other.py
 test_asimtote/ios/config/router.py
 test_asimtote/ios/converters/__init__.py
 test_asimtote/ios/converters/cvtunittest.py
 test_asimtote/ios/converters/interface.py
+test_asimtote/ios/converters/lists.py
 test_asimtote/ios/converters/other.py
 test_asimtote/ios/converters/router.py
```

### Comparing `asimtote-0.16.3/setup.py` & `asimtote-0.16.4/setup.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/config/interface.py` & `asimtote-0.16.4/test_asimtote/ios/config/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/config/lists.py` & `asimtote-0.16.4/test_asimtote/ios/config/lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
                     ("deny", "_20$")
                 ]
             }
         })
 
 
     # -------------------------------------------------------------------------
-    # ip[v6] prefix-list ...
+    # ip prefix-list ...
     # -------------------------------------------------------------------------
 
 
     def test_IPPfxList_simple(self):
         self.cfg.parse_str("""
 ip prefix-list TestPfxList permit 10.0.0.0/8
 """)
@@ -428,14 +428,28 @@
                 "TestPfxList": [
                     "permit 10.0.0.0/8 le 24"
                 ]
             }
         })
 
 
+    def test_IPPfxList_all(self):
+        self.cfg.parse_str("""
+ip prefix-list TestPfxList permit 0.0.0.0/0 le 32
+""")
+
+        self.assertEqual(self.cfg, {
+            "ip-prefix-list": {
+                "TestPfxList": [
+                    "permit 0.0.0.0/0 le 32"
+                ]
+            }
+        })
+
+
     def test_IPPfxList_list(self):
         self.cfg.parse_str("""
 ip prefix-list TestPfxList permit 10.0.0.0/8
 ip prefix-list TestPfxList deny 20.0.0.0/16
 """)
 
         self.assertEqual(self.cfg, {
@@ -464,14 +478,19 @@
                     "deny 30.0.0.0/8",
                     "permit 40.0.0.0/8"
                 ]
             }
         })
 
 
+    # -------------------------------------------------------------------------
+    # ipv6 prefix-list ...
+    # -------------------------------------------------------------------------
+
+
     def test_IPv6PfxList_simple(self):
         self.cfg.parse_str("""
 ipv6 prefix-list TestPfxList permit 10::/48
 """)
 
         self.assertEqual(self.cfg, {
             "ipv6-prefix-list": {
@@ -492,14 +511,28 @@
                 "TestPfxList": [
                     "permit 10::/48 le 64"
                 ]
             }
         })
 
 
+    def test_IPv6PfxList_all(self):
+        self.cfg.parse_str("""
+ipv6 prefix-list TestPfxList permit ::/0 le 128
+""")
+
+        self.assertEqual(self.cfg, {
+            "ipv6-prefix-list": {
+                "TestPfxList": [
+                    "permit ::/0 le 128"
+                ]
+            }
+        })
+
+
     def test_IPv6PfxList_list(self):
         self.cfg.parse_str("""
 ipv6 prefix-list TestPfxList permit 10::/48
 ipv6 prefix-list TestPfxList permit 20::/48
 """)
 
         self.assertEqual(self.cfg, {
```

### Comparing `asimtote-0.16.3/test_asimtote/ios/config/other.py` & `asimtote-0.16.4/test_asimtote/ios/config/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/config/router.py` & `asimtote-0.16.4/test_asimtote/ios/config/router.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/converters/cvtunittest.py` & `asimtote-0.16.4/test_asimtote/ios/converters/cvtunittest.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/converters/interface.py` & `asimtote-0.16.4/test_asimtote/ios/converters/interface.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/converters/other.py` & `asimtote-0.16.4/test_asimtote/ios/converters/other.py`

 * *Files identical despite different names*

### Comparing `asimtote-0.16.3/test_asimtote/ios/utils.py` & `asimtote-0.16.4/test_asimtote/ios/utils.py`

 * *Files identical despite different names*

