# Comparing `tmp/simplerabbit-0.0.4.tar.gz` & `tmp/simplerabbit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.4.tar", last modified: Tue Apr 11 12:27:45 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.5.tar", last modified: Tue Apr 11 12:41:00 2023, max compression
```

## Comparing `simplerabbit-0.0.4.tar` & `simplerabbit-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.4/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:27:26.000000 simplerabbit-0.0.4/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/setup.cfg
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.313679 simplerabbit-0.0.4/src/
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.313679 simplerabbit-0.0.4/src/simplerabbit/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.4/src/simplerabbit/__init__.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3067 2023-04-11 12:11:18.000000 simplerabbit-0.0.4/src/simplerabbit/receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2768 2023-04-11 12:10:34.000000 simplerabbit-0.0.4/src/simplerabbit/sender.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/src/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-11 12:27:45.000000 simplerabbit-0.0.4/src/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:27:45.317679 simplerabbit-0.0.4/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:24:50.000000 simplerabbit-0.0.4/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.5/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-11 12:40:27.000000 simplerabbit-0.0.5/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/simplerabbit/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.5/src/simplerabbit/__init__.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     3067 2023-04-11 12:11:18.000000 simplerabbit-0.0.5/src/simplerabbit/receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2553 2023-04-11 12:40:10.000000 simplerabbit-0.0.5/src/simplerabbit/sender.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      283 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       13 2023-04-11 12:41:00.000000 simplerabbit-0.0.5/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-11 12:41:00.125262 simplerabbit-0.0.5/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.5/tests/test.py
```

### Comparing `simplerabbit-0.0.4/PKG-INFO` & `simplerabbit-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplerabbit-0.0.4/README.md` & `simplerabbit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.4/pyproject.toml` & `simplerabbit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.4/src/simplerabbit/receiver.py` & `simplerabbit-0.0.5/src/simplerabbit/receiver.py`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.4/src/simplerabbit/sender.py` & `simplerabbit-0.0.5/src/simplerabbit/sender.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,26 +48,22 @@
             properties = pika.BasicProperties(
                 correlation_id=str(msg_type),
                 headers=headers
             )
             self.lock.acquire()
             self.channel.basic_publish(exchange=exchange, routing_key=routing_key, body=message, properties=properties)
         except pika.exceptions.AMQPConnectionError as e:
-            MyLogger.info("Connection error:" + str(e))
             raise ConnectionError('Error sending message to ATOM')
 
         except pika.exceptions.AMQPChannelError as e:
-            MyLogger.info("Channel error:" + str(e))
             raise ConnectionError('Error sending message to ATOM')
         finally:
             self.lock.release()
 
     def close(self):
         self._stop_heartbeat_thread()
         if self.connection:
             self.connection.close()
-        MyLogger.info("RabbitSender connection closed.")
 
     def _stop_heartbeat_thread(self):
         self.is_heartbeat_running = False
         self.heartbeat_thread.join()
-        MyLogger.info('Hearbeat thread stopped')
```

### Comparing `simplerabbit-0.0.4/src/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.5/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

