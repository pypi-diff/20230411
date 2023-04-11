# Comparing `tmp/qasync-0.9.4.tar.gz` & `tmp/qasync-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qasync-0.9.4.tar", last modified: Wed Feb 26 20:12:41 2020, max compression
+gzip compressed data, was "dist\qasync-0.9.5.tar", last modified: Mon Oct 26 18:27:23 2020, max compression
```

## Comparing `qasync-0.9.4.tar` & `qasync-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-02-26 20:12:41.561463 qasync-0.9.4/
--rw-rw-rw-   0        0        0     1413 2019-11-24 18:03:55.000000 qasync-0.9.4/LICENSE
--rw-rw-rw-   0        0        0       28 2019-11-02 18:03:36.000000 qasync-0.9.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2195 2020-02-26 20:12:41.560463 qasync-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0      928 2020-02-25 08:45:19.000000 qasync-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2020-02-26 20:12:41.549452 qasync-0.9.4/qasync/
--rw-rw-rw-   0        0        0    22578 2020-02-26 20:11:48.000000 qasync-0.9.4/qasync/__init__.py
--rw-rw-rw-   0        0        0      622 2019-11-24 18:03:55.000000 qasync-0.9.4/qasync/_common.py
--rw-rw-rw-   0        0        0     7127 2019-11-24 18:03:55.000000 qasync-0.9.4/qasync/_unix.py
--rw-rw-rw-   0        0        0     6148 2019-11-24 18:26:30.000000 qasync-0.9.4/qasync/_windows.py
-drwxrwxrwx   0        0        0        0 2020-02-26 20:12:41.559462 qasync-0.9.4/qasync.egg-info/
--rw-rw-rw-   0        0        0     2195 2020-02-26 20:12:41.000000 qasync-0.9.4/qasync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2020-02-26 20:12:41.000000 qasync-0.9.4/qasync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-02-26 20:12:41.000000 qasync-0.9.4/qasync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-02-26 20:12:41.000000 qasync-0.9.4/qasync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-02-26 20:12:41.561463 qasync-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1680 2020-02-26 19:45:02.000000 qasync-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2020-10-26 18:27:23.202653 qasync-0.9.5/
+-rw-rw-rw-   0        0        0     1413 2020-02-29 09:51:18.000000 qasync-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0       28 2019-11-02 18:03:36.000000 qasync-0.9.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2623 2020-10-26 18:27:23.201651 qasync-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2020-04-25 19:06:37.000000 qasync-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2020-10-26 18:27:23.196646 qasync-0.9.5/qasync/
+-rw-rw-rw-   0        0        0    22613 2020-10-26 18:26:21.000000 qasync-0.9.5/qasync/__init__.py
+-rw-rw-rw-   0        0        0      622 2020-02-29 09:51:18.000000 qasync-0.9.5/qasync/_common.py
+-rw-rw-rw-   0        0        0     7148 2020-10-26 17:52:45.000000 qasync-0.9.5/qasync/_unix.py
+-rw-rw-rw-   0        0        0     6148 2020-02-29 09:51:18.000000 qasync-0.9.5/qasync/_windows.py
+drwxrwxrwx   0        0        0        0 2020-10-26 18:27:23.199649 qasync-0.9.5/qasync.egg-info/
+-rw-rw-rw-   0        0        0     2623 2020-10-26 18:27:23.000000 qasync-0.9.5/qasync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2020-10-26 18:27:23.000000 qasync-0.9.5/qasync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-10-26 18:27:23.000000 qasync-0.9.5/qasync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2020-10-26 18:27:23.000000 qasync-0.9.5/qasync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-10-26 18:27:23.202653 qasync-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1680 2020-10-26 18:25:45.000000 qasync-0.9.5/setup.py
```

### Comparing `qasync-0.9.4/LICENSE` & `qasync-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qasync-0.9.4/PKG-INFO` & `qasync-0.9.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: qasync
-Version: 0.9.4
+Version: 0.9.5
 Summary: Implementation of the PEP 3156 Event-Loop with Qt.
 Home-page: https://github.com/CabbageDevelopment/qasync
 Author: Sam McCormack, Gerard Marull-Paretas, Mark Harviston, Arve Knudsen
 Author-email: contact@cabbagedevelopment.com, gerard@teslabs.com, mark.harviston@gmail.com, arve.knudsen@gmail.com
 License: BSD
 Description: # qasync
         
         ![Maintenance](https://img.shields.io/maintenance/yes/2020)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qasync)
         ![PyPI - License](https://img.shields.io/pypi/l/qasync)
         ![PyPI](https://img.shields.io/pypi/v/qasync)
         
         ## Introduction
         
-        `qasync` allows you to use coroutines in PyQt/PySide applications by providing an implementation of the `PEP 3156` event-loop. 
+        `qasync` allows coroutines to be used in PyQt/PySide applications by providing an implementation of the `PEP 3156` event-loop. 
         
         `qasync` is a fork of [asyncqt](https://github.com/gmarull/asyncqt), which is a fork of [quamash](https://github.com/harvimt/quamash). May it live longer than its predecessors. 
         
+        #### The future of `qasync`
+        
+        `qasync` was created because `asyncqt` and `quamash` were no longer maintained. However, as of 28th February 2020, `asyncqt` appears to be active once more. 
+        
+        **`qasync` will continue to be maintained, and will still be accepting pull requests.** Improvements to `asyncqt` will be pulled downstream, and improvements to `qasync` will be sent upstream.
+        
         ## Requirements
         
-        `qasync` requires Python 3.6 or greater, and PyQt5 or PySide2.
+        `qasync` requires Python >= 3.6, and PyQt5 or PySide2.
         
         ## Installation
         
         To install `qasync`, use `pip`:
         
         ```
         pip install qasync
```

### Comparing `qasync-0.9.4/qasync/__init__.py` & `qasync-0.9.5/qasync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 BSD License
 """
 
 __author__ = ('Sam McCormack',
               'Gerard Marull-Paretas <gerard@teslabs.com>, '
               'Mark Harviston <mark.harviston@gmail.com>, '
               'Arve Knudsen <arve.knudsen@gmail.com>')
-__version__ = '0.9.4'
+__version__ = '0.9.5'
 __url__ = 'https://github.com/CabbageDevelopment/qasync'
 __license__ = 'BSD'
 __all__ = ['QEventLoop', 'QThreadExecutor', 'asyncSlot', 'asyncClose']
 
 import asyncio
 import functools
 import importlib
@@ -390,21 +390,21 @@
         try:
             existing = self._read_notifiers[fd]
         except KeyError:
             pass
         else:
             # this is necessary to avoid race condition-like issues
             existing.setEnabled(False)
-            existing.activated.disconnect()
+            existing.activated['int'].disconnect()
             # will get overwritten by the assignment below anyways
 
         notifier = QtCore.QSocketNotifier(fd, QtCore.QSocketNotifier.Read)
         notifier.setEnabled(True)
         self._logger.debug('Adding reader callback for file descriptor {}'.format(fd))
-        notifier.activated.connect(
+        notifier.activated['int'].connect(
             lambda: self.__on_notifier_ready(
                 self._read_notifiers, notifier, fd, callback, args)  # noqa: C812
         )
         self._read_notifiers[fd] = notifier
 
     def remove_reader(self, fd):
         """Remove reader callback."""
@@ -426,21 +426,21 @@
         try:
             existing = self._write_notifiers[fd]
         except KeyError:
             pass
         else:
             # this is necessary to avoid race condition-like issues
             existing.setEnabled(False)
-            existing.activated.disconnect()
+            existing.activated['int'].disconnect()
             # will get overwritten by the assignment below anyways
 
         notifier = QtCore.QSocketNotifier(fd, QtCore.QSocketNotifier.Write)
         notifier.setEnabled(True)
         self._logger.debug('Adding writer callback for file descriptor {}'.format(fd))
-        notifier.activated.connect(
+        notifier.activated['int'].connect(
             lambda: self.__on_notifier_ready(
                 self._write_notifiers, notifier, fd, callback, args)  # noqa: C812
         )
         self._write_notifiers[fd] = notifier
 
     def remove_writer(self, fd):
         """Remove writer callback."""
@@ -466,15 +466,15 @@
             callback(*args)
         finally:
             # The notifier might have been overriden by the
             # callback. We must not re-enable it in that case.
             if notifiers.get(fd, None) is notifier:
                 notifier.setEnabled(True)
             else:
-                notifier.activated.disconnect()
+                notifier.activated['int'].disconnect()
 
     def __on_notifier_ready(self, notifiers, notifier, fd, callback, args):
         if fd not in notifiers:
             self._logger.warning(
                 'Socket notifier for fd {} is ready, even though it should be disabled, not calling {} and disabling'
                     .format(fd, callback),
             )
```

### Comparing `qasync-0.9.4/qasync/_common.py` & `qasync-0.9.5/qasync/_common.py`

 * *Files identical despite different names*

### Comparing `qasync-0.9.4/qasync/_unix.py` & `qasync-0.9.5/qasync/_unix.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,19 +106,19 @@
         if key.fd in self._fd_to_key:
             raise KeyError("{!r} (FD {}) is already registered".format(fileobj, key.fd))
 
         self._fd_to_key[key.fd] = key
 
         if events & EVENT_READ:
             notifier = QtCore.QSocketNotifier(key.fd, QtCore.QSocketNotifier.Read)
-            notifier.activated.connect(self.__on_read_activated)
+            notifier.activated['int'].connect(self.__on_read_activated)
             self.__read_notifiers[key.fd] = notifier
         if events & EVENT_WRITE:
             notifier = QtCore.QSocketNotifier(key.fd, QtCore.QSocketNotifier.Write)
-            notifier.activated.connect(self.__on_write_activated)
+            notifier.activated['int'].connect(self.__on_write_activated)
             self.__write_notifiers[key.fd] = notifier
 
         return key
 
     def __on_read_activated(self, fd):
         self._logger.debug('File {} ready to read'.format(fd))
         key = self._key_from_fd(fd)
@@ -134,15 +134,15 @@
     def unregister(self, fileobj):
         def drop_notifier(notifiers):
             try:
                 notifier = notifiers.pop(key.fd)
             except KeyError:
                 pass
             else:
-                notifier.activated.disconnect()
+                notifier.activated['int'].disconnect()
 
         try:
             key = self._fd_to_key.pop(self._fileobj_lookup(fileobj))
         except KeyError:
             raise KeyError("{!r} is not registered".format(fileobj)) from None
 
         drop_notifier(self.__read_notifiers)
```

### Comparing `qasync-0.9.4/qasync/_windows.py` & `qasync-0.9.5/qasync/_windows.py`

 * *Files identical despite different names*

### Comparing `qasync-0.9.4/qasync.egg-info/PKG-INFO` & `qasync-0.9.5/qasync.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: qasync
-Version: 0.9.4
+Version: 0.9.5
 Summary: Implementation of the PEP 3156 Event-Loop with Qt.
 Home-page: https://github.com/CabbageDevelopment/qasync
 Author: Sam McCormack, Gerard Marull-Paretas, Mark Harviston, Arve Knudsen
 Author-email: contact@cabbagedevelopment.com, gerard@teslabs.com, mark.harviston@gmail.com, arve.knudsen@gmail.com
 License: BSD
 Description: # qasync
         
         ![Maintenance](https://img.shields.io/maintenance/yes/2020)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qasync)
         ![PyPI - License](https://img.shields.io/pypi/l/qasync)
         ![PyPI](https://img.shields.io/pypi/v/qasync)
         
         ## Introduction
         
-        `qasync` allows you to use coroutines in PyQt/PySide applications by providing an implementation of the `PEP 3156` event-loop. 
+        `qasync` allows coroutines to be used in PyQt/PySide applications by providing an implementation of the `PEP 3156` event-loop. 
         
         `qasync` is a fork of [asyncqt](https://github.com/gmarull/asyncqt), which is a fork of [quamash](https://github.com/harvimt/quamash). May it live longer than its predecessors. 
         
+        #### The future of `qasync`
+        
+        `qasync` was created because `asyncqt` and `quamash` were no longer maintained. However, as of 28th February 2020, `asyncqt` appears to be active once more. 
+        
+        **`qasync` will continue to be maintained, and will still be accepting pull requests.** Improvements to `asyncqt` will be pulled downstream, and improvements to `qasync` will be sent upstream.
+        
         ## Requirements
         
-        `qasync` requires Python 3.6 or greater, and PyQt5 or PySide2.
+        `qasync` requires Python >= 3.6, and PyQt5 or PySide2.
         
         ## Installation
         
         To install `qasync`, use `pip`:
         
         ```
         pip install qasync
```

### Comparing `qasync-0.9.4/setup.py` & `qasync-0.9.5/setup.py`

 * *Files identical despite different names*

