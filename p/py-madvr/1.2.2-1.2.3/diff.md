# Comparing `tmp/py_madvr-1.2.2.tar.gz` & `tmp/py_madvr-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.2.2.tar", last modified: Wed Mar 15 23:25:38 2023, max compression
+gzip compressed data, was "py_madvr-1.2.3.tar", last modified: Wed Mar 15 23:52:53 2023, max compression
```

## Comparing `py_madvr-1.2.2.tar` & `py_madvr-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:25:38.375641 py_madvr-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 23:25:28.000000 py_madvr-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:25:38.375641 py_madvr-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-15 23:25:28.000000 py_madvr-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:25:38.371641 py_madvr-1.2.2/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-15 23:25:28.000000 py_madvr-1.2.2/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-03-15 23:25:28.000000 py_madvr-1.2.2/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-15 23:25:28.000000 py_madvr-1.2.2/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-03-15 23:25:28.000000 py_madvr-1.2.2/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:25:38.375641 py_madvr-1.2.2/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:25:38.000000 py_madvr-1.2.2/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-15 23:25:38.000000 py_madvr-1.2.2/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:25:38.000000 py_madvr-1.2.2/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-15 23:25:38.000000 py_madvr-1.2.2/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 23:25:38.375641 py_madvr-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-15 23:25:28.000000 py_madvr-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:25:38.375641 py_madvr-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 23:25:28.000000 py_madvr-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-15 23:25:28.000000 py_madvr-1.2.2/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 23:52:43.000000 py_madvr-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:52:53.258067 py_madvr-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-15 23:52:43.000000 py_madvr-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-03-15 23:52:43.000000 py_madvr-1.2.3/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-15 23:52:53.000000 py_madvr-1.2.3/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 23:52:53.258067 py_madvr-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-15 23:52:43.000000 py_madvr-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:53.258067 py_madvr-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 23:52:43.000000 py_madvr-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-15 23:52:43.000000 py_madvr-1.2.3/tests/testMadVR.py
```

### Comparing `py_madvr-1.2.2/LICENSE` & `py_madvr-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.2/PKG-INFO` & `py_madvr-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.2/madvr/commands.py` & `py_madvr-1.2.3/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.2.2/madvr/madvr.py` & `py_madvr-1.2.3/madvr/madvr.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,39 +248,51 @@
 
             self.logger.debug("Handshakes complete")
 
             return
 
         raise HeartBeatError("Sending heartbeat fatal error")
 
-    def _construct_command(self, raw_command: str) -> tuple[bytes, bool, str]:
+    def _construct_command(self, raw_command: Union[str, list]) -> tuple[bytes, bool, str]:
         """
         Transform commands into their byte values from the string value
 
         Raises NotImplementedError
 
         Return:
             bytes: the value to send in bytes
             bool: if its informational
             str: the 'msg' field in the Enum used to filter notifications
         """
-        # split command into the base and the action like menu: left
         self.logger.debug("raw_command: %s", raw_command)
         skip_val = False
+        # HA seems to always send commands as a list even if you set them as a str
 
         # This lets you use single cmds or something with val like KEYPRESS
-        try:
-            # key_press, menu
-            command, raw_value = raw_command.split(",")
-            value = raw_value.strip()
-            self.logger.debug("using value %s", value)
-        # if valuerror it means theres just one command like PowerOff, so use that
-        except ValueError:
-            command = raw_command
-            skip_val = True
+        # If len is 1, then try to split, otherwise its just one word
+        if len(raw_command) == 1:
+            try:
+                # ['key_press, menu']
+                command, raw_value = raw_command[0].split(",")
+                # remove space
+                value = raw_value.strip()
+                self.logger.debug("using command %s and value %s", command, value)
+            # if valuerror it means theres just one command like PowerOff, so use that directly
+            except ValueError:
+                command = raw_command
+                skip_val = True
+        # if there are more than two values, this is incorrect, error
+        elif len(raw_command) > 2:
+            self.logger.error("More than two command values provided. Envy does not have more than 2 command values e.g KeyPress MENU")
+            raise NotImplementedError(f"Too many values provided {raw_command}")
+        else:
+            # else a command was provided as a proper list ['keypress', 'menu']
+            # raw command will be a list of 2
+            command, value = raw_command
+
 
         self.logger.debug("using command %s", command)
 
         # Check if command is implemented
         if not hasattr(Commands, command):
             raise NotImplementedError(f"Command not implemented: {command}")
 
@@ -323,15 +335,15 @@
                 self.logger.debug("OK found counter: %s", counter)
                 return True
 
             except (socket.timeout, socket.error):
                 self.logger.debug("Timeout reading ack with counter: %s", counter)
                 return False
 
-    def send_command(self, command: str) -> str:
+    def send_command(self, command: Union[str, list]) -> str:
         """
         send a given command same as the official madvr ones
 
         command: str - command to send like KeyPress, MENU
         Raises RetryExceededError
         """
```

### Comparing `py_madvr-1.2.2/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.2.3/py_madvr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.2.2/setup.py` & `py_madvr-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.2.2",
+    version="1.2.3",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.2.2/tests/testMadVR.py` & `py_madvr-1.2.3/tests/testMadVR.py`

 * *Files identical despite different names*

