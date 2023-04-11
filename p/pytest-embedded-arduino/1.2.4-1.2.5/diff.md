# Comparing `tmp/pytest-embedded-arduino-1.2.4.tar.gz` & `tmp/pytest-embedded-arduino-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-arduino-1.2.4.tar", last modified: Fri Mar 10 07:12:30 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-arduino-1.2.5.tar", last modified: Tue Apr 11 05:40:52 2023, max compression
```

## Comparing `pytest-embedded-arduino-1.2.4.tar` & `pytest-embedded-arduino-1.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-10 07:12:19.000000 pytest-embedded-arduino-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-10 07:12:19.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-10 07:12:19.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-10 07:12:19.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 07:12:30.000000 pytest-embedded-arduino-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-10 07:12:19.000000 pytest-embedded-arduino-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-11 05:40:39.000000 pytest-embedded-arduino-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 05:40:39.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-11 05:40:39.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-11 05:40:39.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:52.000000 pytest-embedded-arduino-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-11 05:40:39.000000 pytest-embedded-arduino-1.2.5/setup.py
```

### Comparing `pytest-embedded-arduino-1.2.4/PKG-INFO` & `pytest-embedded-arduino-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for Arduino projects
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Abdelatif Guettouche
 Author-email: abdelatif.guettouche@espressif.com
 License: MIT
 Description: ### pytest-embedded-arduino
```

### Comparing `pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/app.py` & `pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-arduino-1.2.4/pytest_embedded_arduino/serial.py` & `pytest-embedded-arduino-1.2.5/pytest_embedded_arduino/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,9 @@
             self.stub.change_baud(self.esptool_baud)
             esptool.detect_flash_size(self.stub, flash_args)
             esptool.write_flash(self.stub, flash_args)
             self.stub.change_baud(self.baud)
         except Exception:
             raise
         finally:
-            for (_, f) in flash_files:
+            for _, f in flash_files:
                 f.close()
```

### Comparing `pytest-embedded-arduino-1.2.4/pytest_embedded_arduino.egg-info/PKG-INFO` & `pytest-embedded-arduino-1.2.5/pytest_embedded_arduino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.2.4
+Version: 1.2.5
 Summary: pytest embedded plugin for Arduino projects
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Abdelatif Guettouche
 Author-email: abdelatif.guettouche@espressif.com
 License: MIT
 Description: ### pytest-embedded-arduino
```

### Comparing `pytest-embedded-arduino-1.2.4/setup.py` & `pytest-embedded-arduino-1.2.5/setup.py`

 * *Files identical despite different names*

