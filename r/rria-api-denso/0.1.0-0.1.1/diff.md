# Comparing `tmp/rria_api_denso-0.1.0.tar.gz` & `tmp/rria_api_denso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rria_api_denso-0.1.0.tar", max compression
+gzip compressed data, was "rria_api_denso-0.1.1.tar", max compression
```

## Comparing `rria_api_denso-0.1.0.tar` & `rria_api_denso-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      429 2023-04-11 13:34:27.746727 rria_api_denso-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      734 2023-04-11 13:18:18.010294 rria_api_denso-0.1.0/README.md
--rw-r--r--   0        0        0       29 2023-04-10 18:27:25.603229 rria_api_denso-0.1.0/rria_api_denso/__init__.py
--rw-r--r--   0        0        0     2137 2023-04-11 14:08:29.694958 rria_api_denso-0.1.0/rria_api_denso/action_denso.py
--rw-r--r--   0        0        0     2499 2023-04-11 13:45:57.095581 rria_api_denso-0.1.0/rria_api_denso/connect_denso.py
--rw-r--r--   0        0        0     9023 2023-04-11 13:40:39.705864 rria_api_denso-0.1.0/rria_api_denso/robot_object.py
--rw-r--r--   0        0        0       36 2023-04-10 18:48:49.767729 rria_api_denso-0.1.0/rria_api_denso/utils/__init__.py
--rw-r--r--   0        0        0    29774 2023-04-11 13:37:53.672705 rria_api_denso-0.1.0/rria_api_denso/utils/bcapclient.py
--rw-r--r--   0        0        0     2753 2023-04-10 18:48:49.781127 rria_api_denso-0.1.0/rria_api_denso/utils/orinexception.py
--rw-r--r--   0        0        0     2255 2023-04-10 18:48:49.788166 rria_api_denso-0.1.0/rria_api_denso/utils/variant.py
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 rria_api_denso-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-04-11 15:02:42.161206 rria_api_denso-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      759 2023-04-11 15:02:42.164207 rria_api_denso-0.1.1/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 18:27:25.603229 rria_api_denso-0.1.1/rria_api_denso/__init__.py
+-rw-r--r--   0        0        0     2137 2023-04-11 14:08:29.694958 rria_api_denso-0.1.1/rria_api_denso/action_denso.py
+-rw-r--r--   0        0        0     2499 2023-04-11 13:45:57.095581 rria_api_denso-0.1.1/rria_api_denso/connect_denso.py
+-rw-r--r--   0        0        0     9023 2023-04-11 13:40:39.705864 rria_api_denso-0.1.1/rria_api_denso/robot_object.py
+-rw-r--r--   0        0        0       36 2023-04-10 18:48:49.767729 rria_api_denso-0.1.1/rria_api_denso/utils/__init__.py
+-rw-r--r--   0        0        0    29774 2023-04-11 13:37:53.672705 rria_api_denso-0.1.1/rria_api_denso/utils/bcapclient.py
+-rw-r--r--   0        0        0     2753 2023-04-10 18:48:49.781127 rria_api_denso-0.1.1/rria_api_denso/utils/orinexception.py
+-rw-r--r--   0        0        0     2255 2023-04-10 18:48:49.788166 rria_api_denso-0.1.1/rria_api_denso/utils/variant.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 rria_api_denso-0.1.1/PKG-INFO
```

### Comparing `rria_api_denso-0.1.0/README.md` & `rria_api_denso-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,11 @@
 
 denso_robot.motor_on()
 
 denso_robot.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 
 denso_robot.move_to_home()
 
+denso_robot.motor_off()
+
 denso_robot.safe_disconnect()
 ```
```

### Comparing `rria_api_denso-0.1.0/rria_api_denso/action_denso.py` & `rria_api_denso-0.1.1/rria_api_denso/action_denso.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/rria_api_denso/connect_denso.py` & `rria_api_denso-0.1.1/rria_api_denso/connect_denso.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/rria_api_denso/robot_object.py` & `rria_api_denso-0.1.1/rria_api_denso/robot_object.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/rria_api_denso/utils/bcapclient.py` & `rria_api_denso-0.1.1/rria_api_denso/utils/bcapclient.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/rria_api_denso/utils/orinexception.py` & `rria_api_denso-0.1.1/rria_api_denso/utils/orinexception.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/rria_api_denso/utils/variant.py` & `rria_api_denso-0.1.1/rria_api_denso/utils/variant.py`

 * *Files identical despite different names*

### Comparing `rria_api_denso-0.1.0/PKG-INFO` & `rria_api_denso-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rria-api-denso
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Felipe Augusto
 Author-email: 97059009+felipeadsm@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pywin32 (>=306,<307)
@@ -39,9 +39,11 @@
 
 denso_robot.motor_on()
 
 denso_robot.move_joints(30.0, 30.0, 30.0, 30.0, 30.0, 30.0)
 
 denso_robot.move_to_home()
 
+denso_robot.motor_off()
+
 denso_robot.safe_disconnect()
 ```
```

