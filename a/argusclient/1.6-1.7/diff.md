# Comparing `tmp/argusclient-1.6.tar.gz` & `tmp/argusclient-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argusclient-1.6.tar", last modified: Mon Dec 20 18:33:06 2021, max compression
+gzip compressed data, was "argusclient-1.7.tar", last modified: Tue Apr 11 18:01:36 2023, max compression
```

## Comparing `argusclient-1.6.tar` & `argusclient-1.7.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 agosher    (503) staff       (20)        0 2021-12-20 18:33:06.349127 argusclient-1.6/
--rw-r--r--   0 agosher    (503) staff       (20)     1482 2021-12-07 18:47:29.000000 argusclient-1.6/LICENSE.txt
--rw-r--r--   0 agosher    (503) staff       (20)     7590 2021-12-20 18:33:06.348569 argusclient-1.6/PKG-INFO
--rw-r--r--   0 agosher    (503) staff       (20)     6993 2021-12-20 17:40:08.000000 argusclient-1.6/README.rst
-drwxr-xr-x   0 agosher    (503) staff       (20)        0 2021-12-20 18:33:06.343917 argusclient-1.6/argusclient/
--rw-r--r--   0 agosher    (503) staff       (20)      486 2021-12-07 18:47:29.000000 argusclient-1.6/argusclient/__init__.py
--rw-r--r--   0 agosher    (503) staff       (20)    48034 2021-12-07 18:47:29.000000 argusclient-1.6/argusclient/client.py
--rw-r--r--   0 agosher    (503) staff       (20)     4991 2021-12-07 18:47:29.000000 argusclient-1.6/argusclient/dashboardtags.py
--rw-r--r--   0 agosher    (503) staff       (20)    20262 2021-12-20 17:46:20.000000 argusclient-1.6/argusclient/model.py
-drwxr-xr-x   0 agosher    (503) staff       (20)        0 2021-12-20 18:33:06.346949 argusclient-1.6/argusclient.egg-info/
--rw-r--r--   0 agosher    (503) staff       (20)     7590 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/PKG-INFO
--rw-r--r--   0 agosher    (503) staff       (20)      420 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/SOURCES.txt
--rw-r--r--   0 agosher    (503) staff       (20)        1 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/dependency_links.txt
--rw-r--r--   0 agosher    (503) staff       (20)       37 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/entry_points.txt
--rw-r--r--   0 agosher    (503) staff       (20)       41 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/requires.txt
--rw-r--r--   0 agosher    (503) staff       (20)       24 2021-12-20 18:33:06.000000 argusclient-1.6/argusclient.egg-info/top_level.txt
--rw-r--r--   0 agosher    (503) staff       (20)        1 2021-12-07 18:52:07.000000 argusclient-1.6/argusclient.egg-info/zip-safe
-drwxr-xr-x   0 agosher    (503) staff       (20)        0 2021-12-20 18:33:06.347979 argusclient-1.6/monexclient/
--rw-r--r--   0 agosher    (503) staff       (20)        0 2021-12-07 18:47:29.000000 argusclient-1.6/monexclient/__init__.py
--rw-r--r--   0 agosher    (503) staff       (20)    10212 2021-12-07 18:47:29.000000 argusclient-1.6/monexclient/monexclient.py
--rw-r--r--   0 agosher    (503) staff       (20)       38 2021-12-20 18:33:06.349364 argusclient-1.6/setup.cfg
--rw-r--r--   0 agosher    (503) staff       (20)     1397 2021-12-20 17:48:06.000000 argusclient-1.6/setup.py
+drwxr-xr-x   0 agosher    (503) staff       (20)        0 2023-04-11 18:01:36.932404 argusclient-1.7/
+-rw-r--r--   0 agosher    (503) staff       (20)     1482 2022-08-05 00:16:55.000000 argusclient-1.7/LICENSE.txt
+-rw-r--r--   0 agosher    (503) staff       (20)     7570 2023-04-11 18:01:36.932072 argusclient-1.7/PKG-INFO
+-rw-r--r--   0 agosher    (503) staff       (20)     6993 2022-08-05 00:16:55.000000 argusclient-1.7/README.rst
+drwxr-xr-x   0 agosher    (503) staff       (20)        0 2023-04-11 18:01:36.926375 argusclient-1.7/argusclient/
+-rw-r--r--   0 agosher    (503) staff       (20)      486 2022-08-05 00:16:55.000000 argusclient-1.7/argusclient/__init__.py
+-rw-r--r--   0 agosher    (503) staff       (20)    48034 2022-08-05 00:16:55.000000 argusclient-1.7/argusclient/client.py
+-rw-r--r--   0 agosher    (503) staff       (20)     4991 2022-08-05 00:16:55.000000 argusclient-1.7/argusclient/dashboardtags.py
+-rw-r--r--   0 agosher    (503) staff       (20)    20390 2023-04-05 22:18:46.000000 argusclient-1.7/argusclient/model.py
+drwxr-xr-x   0 agosher    (503) staff       (20)        0 2023-04-11 18:01:36.930117 argusclient-1.7/argusclient.egg-info/
+-rw-r--r--   0 agosher    (503) staff       (20)     7570 2023-04-11 18:01:36.000000 argusclient-1.7/argusclient.egg-info/PKG-INFO
+-rw-r--r--   0 agosher    (503) staff       (20)      382 2023-04-11 18:01:36.000000 argusclient-1.7/argusclient.egg-info/SOURCES.txt
+-rw-r--r--   0 agosher    (503) staff       (20)        1 2023-04-11 18:01:36.000000 argusclient-1.7/argusclient.egg-info/dependency_links.txt
+-rw-r--r--   0 agosher    (503) staff       (20)       41 2023-04-11 18:01:36.000000 argusclient-1.7/argusclient.egg-info/requires.txt
+-rw-r--r--   0 agosher    (503) staff       (20)       24 2023-04-11 18:01:36.000000 argusclient-1.7/argusclient.egg-info/top_level.txt
+-rw-r--r--   0 agosher    (503) staff       (20)        1 2022-08-05 00:18:30.000000 argusclient-1.7/argusclient.egg-info/zip-safe
+drwxr-xr-x   0 agosher    (503) staff       (20)        0 2023-04-11 18:01:36.931445 argusclient-1.7/monexclient/
+-rw-r--r--   0 agosher    (503) staff       (20)        0 2022-08-05 00:16:55.000000 argusclient-1.7/monexclient/__init__.py
+-rw-r--r--   0 agosher    (503) staff       (20)    10212 2022-08-05 00:16:55.000000 argusclient-1.7/monexclient/monexclient.py
+-rw-r--r--   0 agosher    (503) staff       (20)       38 2023-04-11 18:01:36.932541 argusclient-1.7/setup.cfg
+-rw-r--r--   0 agosher    (503) staff       (20)     1397 2023-04-08 01:04:17.000000 argusclient-1.7/setup.py
```

### Comparing `argusclient-1.6/LICENSE.txt` & `argusclient-1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `argusclient-1.6/PKG-INFO` & `argusclient-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: argusclient
-Version: 1.6
+Version: 1.7
 Summary: Minimal client library for Argus webservice REST API
 Home-page: https://github.com/SalesforceEng/argusclient
 Author: Hari Krishna Dara
 Author-email: hdara@salesforce.com
 License: BSD-3-Clause
 Keywords: argus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -186,9 +185,7 @@
 ::
 
     logging.info("Creating new alert with alert name: %s", alert_name)
     alertobj = argus.alerts.add(Alert(alert_name, mquery, "* */1 * * *",
                                       trigger=Trigger("hdara.test.trigger", Trigger.GREATER_THAN, 100000, 600000),
                                       notification=Notification("hdara.test.notification", Notification.EMAIL, subscriptions=["hdara@salesforce.com"]),
                                       shared=True))
-
-
```

### Comparing `argusclient-1.6/README.rst` & `argusclient-1.7/README.rst`

 * *Files identical despite different names*

### Comparing `argusclient-1.6/argusclient/client.py` & `argusclient-1.7/argusclient/client.py`

 * *Files identical despite different names*

### Comparing `argusclient-1.6/argusclient/dashboardtags.py` & `argusclient-1.7/argusclient/dashboardtags.py`

 * *Files identical despite different names*

### Comparing `argusclient-1.6/argusclient/model.py` & `argusclient-1.7/argusclient/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,15 +437,15 @@
 
     **Required parameters to the constructor:**
 
     :param name: The name of the notification
     :type name: str
     :param notifierName: The name of the notifier implementation. Must be one of :attr:`EMAIL`, :attr:`AUDIT`,
             :attr:`GOC`, :attr:`GUS`, :attr:`CALLBACK`, :attr:`PAGER_DUTY`, :attr:`REFOCUS_BOOLEAN`,
-            :attr:`REFOCUS_VALUE`, :attr:`SLACK`, :attr:`ALERT_ROUTER`, :attr:`CUSTOM_SLACK`
+            :attr:`REFOCUS_VALUE`, :attr:`SLACK`, :attr:`ALERT_ROUTER`, :attr:`CUSTOM_SLACK`, :attr:`SQS_SUBSTRATE`
     :type notifierName or notifier: str
 
     **Optional parameters to the constructor:**
 
     :param subscriptions: The subscriptions for the notifier implementation, such as email ids in case of :attr:`EMAIL`.
     :type subscriptions: list of str
     :param cooldownPeriod: The cooldown period
@@ -468,18 +468,19 @@
     CALLBACK = "com.salesforce.dva.argus.service.alert.notifier.CallbackNotifier"
     PAGER_DUTY = "com.salesforce.dva.argus.service.alert.notifier.PagerDutyNotifier"
     REFOCUS_BOOLEAN = "com.salesforce.dva.argus.service.alert.notifier.RefocusBooleanNotifier"
     REFOCUS_VALUE = "com.salesforce.dva.argus.service.alert.notifier.RefocusValueNotifier"
     SLACK = "com.salesforce.dva.argus.service.alert.notifier.SlackNotifier"
     ALERT_ROUTER = "com.salesforce.dva.argus.service.alert.notifier.AlertRouterNotifier"
     CUSTOM_SLACK = "com.salesforce.dva.argus.service.alert.notifier.CustomSlackNotifier"
+    SQS_SUBSTRATE = "com.salesforce.dva.argus.service.alert.notifier.SQSSubtrateNotifier"
 
     #: Set of all valid notifier implementation names.
     VALID_NOTIFIERS = frozenset((EMAIL, AUDIT, GOC, GUS, CALLBACK, PAGER_DUTY,
-                                 REFOCUS_BOOLEAN, REFOCUS_VALUE, SLACK, ALERT_ROUTER, CUSTOM_SLACK))
+                                 REFOCUS_BOOLEAN, REFOCUS_VALUE, SLACK, ALERT_ROUTER, CUSTOM_SLACK, SQS_SUBSTRATE))
 
     def __init__(self, name, notifierName=None, metricsToAnnotate=None, **kwargs):
         notifierName = notifierName or kwargs.get('notifier')
         assert notifierName in Notification.VALID_NOTIFIERS, "notifierName is not valid: %s" % notifierName
         super(Notification, self).__init__(name=name, notifierName=notifierName,
                                            metricsToAnnotate=metricsToAnnotate or [],
                                            **kwargs)
```

### Comparing `argusclient-1.6/argusclient.egg-info/PKG-INFO` & `argusclient-1.7/argusclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: argusclient
-Version: 1.6
+Version: 1.7
 Summary: Minimal client library for Argus webservice REST API
 Home-page: https://github.com/SalesforceEng/argusclient
 Author: Hari Krishna Dara
 Author-email: hdara@salesforce.com
 License: BSD-3-Clause
 Keywords: argus
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -186,9 +185,7 @@
 ::
 
     logging.info("Creating new alert with alert name: %s", alert_name)
     alertobj = argus.alerts.add(Alert(alert_name, mquery, "* */1 * * *",
                                       trigger=Trigger("hdara.test.trigger", Trigger.GREATER_THAN, 100000, 600000),
                                       notification=Notification("hdara.test.notification", Notification.EMAIL, subscriptions=["hdara@salesforce.com"]),
                                       shared=True))
-
-
```

### Comparing `argusclient-1.6/monexclient/monexclient.py` & `argusclient-1.7/monexclient/monexclient.py`

 * *Files identical despite different names*

### Comparing `argusclient-1.6/setup.py` & `argusclient-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All rights reserved.
 # Licensed under the BSD 3-Clause license. 
 # For full license text, see LICENSE.txt file in the repo root  or https://opensource.org/licenses/BSD-3-Clause
 #
 
 from setuptools import setup, find_packages
 
-version = '1.6'
+version = '1.7'
 
 with open("README.rst", 'r') as fin:
     README = fin.read()
 
 
 setup(name='argusclient',
       version=version,
```

