# Comparing `tmp/pylookout-0.2.4.tar.gz` & `tmp/pylookout-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookout-0.2.4.tar", last modified: Mon Apr  3 19:23:54 2023, max compression
+gzip compressed data, was "pylookout-0.2.5.tar", last modified: Tue Apr 11 19:28:57 2023, max compression
```

## Comparing `pylookout-0.2.4.tar` & `pylookout-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:23:54.408559 pylookout-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-03 19:23:45.000000 pylookout-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-03 19:23:54.408559 pylookout-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-03 19:23:45.000000 pylookout-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:23:54.408559 pylookout-0.2.4/pylookout/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-03 19:23:45.000000 pylookout-0.2.4/pylookout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-03 19:23:45.000000 pylookout-0.2.4/pylookout/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-03 19:23:45.000000 pylookout-0.2.4/pylookout/info_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-03 19:23:45.000000 pylookout-0.2.4/pylookout/lookout.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-03 19:23:45.000000 pylookout-0.2.4/pylookout/lookout_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 19:23:54.408559 pylookout-0.2.4/pylookout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 19:23:54.000000 pylookout-0.2.4/pylookout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-03 19:23:45.000000 pylookout-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-03 19:23:54.408559 pylookout-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 19:23:45.000000 pylookout-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 19:28:46.000000 pylookout-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 19:28:57.954370 pylookout-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 19:28:46.000000 pylookout-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/pylookout/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/info_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/lookout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/lookout_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 19:28:46.000000 pylookout-0.2.5/pylookout/notification_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:28:57.954370 pylookout-0.2.5/pylookout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 19:28:57.000000 pylookout-0.2.5/pylookout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-11 19:28:46.000000 pylookout-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 19:28:57.958370 pylookout-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:28:46.000000 pylookout-0.2.5/setup.py
```

### Comparing `pylookout-0.2.4/LICENSE` & `pylookout-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.4/PKG-INFO` & `pylookout-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookout
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple Linux system monitoring tool
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pylookout-0.2.4/README.md` & `pylookout-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.4/pylookout/info_collector.py` & `pylookout-0.2.5/pylookout/info_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     partitions: list = field(default_factory=list)
     disks_info: dict = field(default_factory=dict)
 
     # Login information
     logins: list = field(default_factory=list)
 
     def __post_init__(self, check_containers):
-        # do not calculate CPU usage if there is only one core
         self.cpu_detail = (
             {f"Core{i}": p for i, p in enumerate(cpu_percent(percpu=True))}
             if cpu_count() > 1
             else {"Core": 0}
         )
 
         self.ram_total = self._convert_bytes(ram().total)
@@ -107,14 +106,17 @@
                 os.popen(f"docker inspect {container}").read()
             )[0]
             container = self._inspect_container(inspect)
             containers_parsed[container["id"]] = container
         return containers_parsed
 
     def _get_logins(self):
+        """
+        Get information about current active logins.
+        """
         logins = []
         logins_bash = os.popen("who").read().split("\n")
         for login in logins_bash:
             who_info = login.split()
             if who_info:
                 logins.append(
                     {
```

### Comparing `pylookout-0.2.4/pylookout/lookout.py` & `pylookout-0.2.5/pylookout/lookout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import logging
 from pathlib import Path
-from os import getenv
 from time import sleep
-from urllib import request, parse
 from .info_collector import Collector
-
-from sendgrid import SendGridAPIClient
-from sendgrid.helpers.mail import Mail, Email, To, Content
+from .notification_methods import simple_push, sendgrid
 
 
 class PyLookout:
     def __init__(
         self,
         threshold=75,
         method="local",
@@ -59,71 +55,38 @@
         """
         if self.notification != []:
             title = self._format_message("starting")
             ending = self._format_message("finished")
             self.notification.insert(0, title)
             self.notification.append(ending)
 
-    def _simple_push(self):
-        """
-        Send notifications using Simplepush.
-        """
-        api_key = getenv("SIMPLEPUSH")
-        data = parse.urlencode(
-            {
-                "key": api_key,
-                "title": f"pyLookout on {self.info.hostname}\n",
-                "msg": "\n".join(self.notification),
-                "event": "event",
-            }
-        ).encode()
-        req = request.Request("https://api.simplepush.io/send", data=data)
-        request.urlopen(req)
-        self.logger.info("Notification sent successfully!")
-        self.logger.info("Notification message:")
-        self.logger.info(self.notification)
-
-    def _sendgrid(self):
-        """
-        Send notifications using SengGrid.
-        """
-        api_key = getenv("SENDGRID_API_KEY")
-        email_from = Email(getenv("SENDGRID_FROM"))
-        email_to = To(getenv("SENDGRID_TO"))
-
-        subject = f"pyLookout on {self.info.hostname}\n"
-        content = Content("text/plain", "\n".join(self.notification))
-        mail = Mail(email_from, email_to, subject, content)
-
-        response = SendGridAPIClient(api_key).client.mail.send.post(
-            request_body=mail.get()
-        )
-
-        if response.status_code == 202:
-            self.logger.info("Email sent succsessfully!")
-            self.logger.info("Emailed message:")
-            self.logger.info(self.notification)
-
     def _notify(self):
         """
         Send a notification.
         Available methods:
             * local (print to console)
             * simplepush
             * sendgrid
         """
         self._adjust_message()
         if self.method == "local":
-            print(self.info.logins)
-            for notification in self.notification:
-                self.logger.info(notification)
+            [self.logger.info(line) for line in self.notification]
+
         elif self.method == "simplepush":
-            self._simple_push()
+            simple_push(self.info.hostname, self.notification)
+            self.logger.info("Notification sent successfully!")
+            self.logger.info("Notification message:")
+            [self.logger.info(line) for line in self.notification]
+
         elif self.method == "sendgrid":
-            self._sendgrid()
+            status_code = sendgrid(self.info.hostname, self.notification)
+            if status_code == 202:
+                self.logger.info("Email sent succsessfully!")
+                self.logger.info("Emailed message:")
+                [self.logger.info(line) for line in self.notification]
 
     def _containers_status(self, containers):
         """
         Check all container statuses,
         send notifications if monitored container is down.
         """
         for container in containers.values():
```

### Comparing `pylookout-0.2.4/pylookout/lookout_cli.py` & `pylookout-0.2.5/pylookout/lookout_cli.py`

 * *Files identical despite different names*

### Comparing `pylookout-0.2.4/pylookout.egg-info/PKG-INFO` & `pylookout-0.2.5/pylookout.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookout
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple Linux system monitoring tool
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pylookout-0.2.4/setup.cfg` & `pylookout-0.2.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pylookout
-version = 0.2.4
+version = 0.2.5
 description = Simple Linux system monitoring tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

