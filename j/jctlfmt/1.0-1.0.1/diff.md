# Comparing `tmp/jctlfmt-1.0.tar.gz` & `tmp/jctlfmt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jctlfmt-1.0.tar", last modified: Sat Jan 21 23:59:37 2023, max compression
+gzip compressed data, was "jctlfmt-1.0.1.tar", last modified: Tue Apr 11 21:31:10 2023, max compression
```

## Comparing `jctlfmt-1.0.tar` & `jctlfmt-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 23:59:37.884012 jctlfmt-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-21 23:59:21.000000 jctlfmt-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-21 23:59:37.884012 jctlfmt-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-21 23:59:21.000000 jctlfmt-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 23:59:37.884012 jctlfmt-1.0/jctlfmt/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-01-21 23:59:21.000000 jctlfmt-1.0/jctlfmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-21 23:59:37.884012 jctlfmt-1.0/jctlfmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-21 23:59:37.000000 jctlfmt-1.0/jctlfmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-21 23:59:37.000000 jctlfmt-1.0/jctlfmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-21 23:59:37.000000 jctlfmt-1.0/jctlfmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-21 23:59:37.000000 jctlfmt-1.0/jctlfmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-21 23:59:37.888012 jctlfmt-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-21 23:59:21.000000 jctlfmt-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/jctlfmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/jctlfmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/jctlfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 21:31:10.000000 jctlfmt-1.0.1/jctlfmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-11 21:31:10.219041 jctlfmt-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 21:30:53.000000 jctlfmt-1.0.1/setup.py
```

### Comparing `jctlfmt-1.0/LICENSE` & `jctlfmt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jctlfmt-1.0/PKG-INFO` & `jctlfmt-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jctlfmt
-Version: 1.0
+Version: 1.0.1
 Summary: Python Journalctl parsing and formatting library
 Home-page: https://github.com/dmotte/jctlfmt
 Author: dmotte
 License: MIT
 Keywords: fmt journal parsing log text formatting systemd format logs msg message journald messages filtering journalctl systemd-journald jctl
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
```

### Comparing `jctlfmt-1.0/README.md` & `jctlfmt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jctlfmt-1.0/jctlfmt/__init__.py` & `jctlfmt-1.0.1/jctlfmt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,44 +40,42 @@
 
         self.hostname: str = raw['_HOSTNAME']
         'Name of the host that generated the journal message'
 
         self.unit: str = raw.get('_SYSTEMD_UNIT', '')
         'Systemd unit name'
 
-        self.ident: str = raw['SYSLOG_IDENTIFIER']
+        self.ident: str = raw.get('SYSLOG_IDENTIFIER', '')
         'Syslog identifier'
 
         self.pid: str = raw.get('_PID', '')
         'Process ID'
 
         self.prio = int(raw.get('PRIORITY', -1))
         'Priority of the message (as int)'
 
         self.msg: str = raw['MESSAGE']
         'Message text'
 
     @property
     def str_ui(self):
         '''
-        Returns `(unit) ident` or just `ident` if unit is empty
+        Returns `(unit) ident` omitting the empty parts
         '''
         if self.unit == '':
             return self.ident
+        elif self.ident == '':
+            return f'({self.unit})'
         else:
             return f'({self.unit}) {self.ident}'
 
     @property
     def str_uip(self):
         '''
-        Returns:
-        - `(unit) ident[pid]` or
-        - `(unit) ident` if pid is empty, or
-        - `ident[pid]` if unit is empty, or
-        - `ident` if unit and pid are both empty
+        Returns `(unit) ident[pid]` omitting the empty parts
         '''
         if self.pid == '':
             return self.str_ui
         else:
             return f'{self.str_ui}[{self.pid}]'
 
     @property
```

### Comparing `jctlfmt-1.0/jctlfmt.egg-info/PKG-INFO` & `jctlfmt-1.0.1/jctlfmt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jctlfmt
-Version: 1.0
+Version: 1.0.1
 Summary: Python Journalctl parsing and formatting library
 Home-page: https://github.com/dmotte/jctlfmt
 Author: dmotte
 License: MIT
 Keywords: fmt journal parsing log text formatting systemd format logs msg message journald messages filtering journalctl systemd-journald jctl
 Classifier: Intended Audience :: System Administrators
 Classifier: Environment :: Console
```

### Comparing `jctlfmt-1.0/setup.cfg` & `jctlfmt-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Natural Language :: English
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Topic :: Utilities
-version = 1.0
+version = 1.0.1
 
 [options]
 install_requires = 
 python_requires = >=3.9.1
 packages = jctlfmt
 
 [egg_info]
```

