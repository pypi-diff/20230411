# Comparing `tmp/pytest-embedded-qemu-1.2.4.tar.gz` & `tmp/pytest-embedded-qemu-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-qemu-1.2.4.tar", last modified: Fri Mar 10 07:12:30 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-qemu-1.2.5.tar", last modified: Tue Apr 11 05:40:52 2023, max compression
```

## Comparing `pytest-embedded-qemu-1.2.4.tar` & `pytest-embedded-qemu-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/qemu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 07:12:30.000000 pytest-embedded-qemu-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-10 07:12:19.000000 pytest-embedded-qemu-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/qemu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/setup.py
```

### Comparing `pytest-embedded-qemu-1.2.4/PKG-INFO` & `pytest-embedded-qemu-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-qemu
```

### Comparing `pytest-embedded-qemu-1.2.4/README.md` & `pytest-embedded-qemu-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/app.py` & `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.2.4/pytest_embedded_qemu/qemu.py` & `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/qemu.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.2.4/pytest_embedded_qemu.egg-info/PKG-INFO` & `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-qemu
```

### Comparing `pytest-embedded-qemu-1.2.4/setup.py` & `pytest-embedded-qemu-1.2.5/setup.py`

 * *Files identical despite different names*

