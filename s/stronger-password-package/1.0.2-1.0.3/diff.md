# Comparing `tmp/stronger password package-1.0.2.tar.gz` & `tmp/stronger password package-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stronger password package-1.0.2.tar", last modified: Tue Apr 11 09:34:39 2023, max compression
+gzip compressed data, was "stronger password package-1.0.3.tar", last modified: Tue Apr 11 09:51:11 2023, max compression
```

## Comparing `stronger password package-1.0.2.tar` & `stronger password package-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:34:39.939191 stronger password package-1.0.2/
--rw-r--r--   0 benishtainberg   (501) staff       (20)     1076 2023-04-04 20:33:53.000000 stronger password package-1.0.2/LICENSE
--rw-r--r--   0 benishtainberg   (501) staff       (20)     2863 2023-04-11 09:34:39.939310 stronger password package-1.0.2/PKG-INFO
--rw-r--r--   0 benishtainberg   (501) staff       (20)     2330 2023-04-11 09:34:13.000000 stronger password package-1.0.2/README.md
--rw-r--r--   0 benishtainberg   (501) staff       (20)      128 2023-04-11 09:26:44.000000 stronger password package-1.0.2/pyproject.toml
--rw-r--r--   0 benishtainberg   (501) staff       (20)      657 2023-04-11 09:34:39.939705 stronger password package-1.0.2/setup.cfg
-drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:34:39.933798 stronger password package-1.0.2/src/
-drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:34:39.936234 stronger password package-1.0.2/src/stronger/
--rw-r--r--   0 benishtainberg   (501) staff       (20)        0 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/__init__.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      659 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/breached_password.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      470 2023-04-11 09:31:00.000000 stronger password package-1.0.2/src/stronger/multi_factor_authetication.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      732 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/password_generation.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      656 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/password_hash.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      553 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/strength_checker.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      917 2023-04-09 14:17:58.000000 stronger password package-1.0.2/src/stronger/suggest_improvements.py
-drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:34:39.937004 stronger password package-1.0.2/src/stronger_password_package.egg-info/
--rw-r--r--   0 benishtainberg   (501) staff       (20)     2863 2023-04-11 09:34:39.000000 stronger password package-1.0.2/src/stronger_password_package.egg-info/PKG-INFO
--rw-r--r--   0 benishtainberg   (501) staff       (20)      693 2023-04-11 09:34:39.000000 stronger password package-1.0.2/src/stronger_password_package.egg-info/SOURCES.txt
--rw-r--r--   0 benishtainberg   (501) staff       (20)        1 2023-04-11 09:34:39.000000 stronger password package-1.0.2/src/stronger_password_package.egg-info/dependency_links.txt
--rw-r--r--   0 benishtainberg   (501) staff       (20)        9 2023-04-11 09:34:39.000000 stronger password package-1.0.2/src/stronger_password_package.egg-info/top_level.txt
-drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:34:39.938928 stronger password package-1.0.2/tests/
--rw-r--r--   0 benishtainberg   (501) staff       (20)      235 2023-04-09 14:18:43.000000 stronger password package-1.0.2/tests/test_breached_password.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      297 2023-04-09 14:18:45.000000 stronger password package-1.0.2/tests/test_multi_factor_authetication.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      214 2023-04-09 14:18:47.000000 stronger password package-1.0.2/tests/test_password_generation.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      294 2023-04-09 14:18:47.000000 stronger password package-1.0.2/tests/test_password_hash.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      486 2023-04-09 14:18:47.000000 stronger password package-1.0.2/tests/test_strength_checker.py
--rw-r--r--   0 benishtainberg   (501) staff       (20)      625 2023-04-09 14:18:49.000000 stronger password package-1.0.2/tests/test_suggest_improvements.py
+drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:51:11.464292 stronger password package-1.0.3/
+-rw-r--r--   0 benishtainberg   (501) staff       (20)     1076 2023-04-04 20:33:53.000000 stronger password package-1.0.3/LICENSE
+-rw-r--r--   0 benishtainberg   (501) staff       (20)     2863 2023-04-11 09:51:11.464377 stronger password package-1.0.3/PKG-INFO
+-rw-r--r--   0 benishtainberg   (501) staff       (20)     2330 2023-04-11 09:34:13.000000 stronger password package-1.0.3/README.md
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      128 2023-04-11 09:26:44.000000 stronger password package-1.0.3/pyproject.toml
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      694 2023-04-11 09:51:11.464676 stronger password package-1.0.3/setup.cfg
+drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:51:11.459379 stronger password package-1.0.3/src/
+drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:51:11.461576 stronger password package-1.0.3/src/stronger/
+-rw-r--r--   0 benishtainberg   (501) staff       (20)        0 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/__init__.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      659 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/breached_password.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      470 2023-04-11 09:31:00.000000 stronger password package-1.0.3/src/stronger/multi_factor_authetication.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      732 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/password_generation.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      656 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/password_hash.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      553 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/strength_checker.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      917 2023-04-09 14:17:58.000000 stronger password package-1.0.3/src/stronger/suggest_improvements.py
+drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:51:11.462183 stronger password package-1.0.3/src/stronger_password_package.egg-info/
+-rw-r--r--   0 benishtainberg   (501) staff       (20)     2863 2023-04-11 09:51:11.000000 stronger password package-1.0.3/src/stronger_password_package.egg-info/PKG-INFO
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      745 2023-04-11 09:51:11.000000 stronger password package-1.0.3/src/stronger_password_package.egg-info/SOURCES.txt
+-rw-r--r--   0 benishtainberg   (501) staff       (20)        1 2023-04-11 09:51:11.000000 stronger password package-1.0.3/src/stronger_password_package.egg-info/dependency_links.txt
+-rw-r--r--   0 benishtainberg   (501) staff       (20)       15 2023-04-11 09:51:11.000000 stronger password package-1.0.3/src/stronger_password_package.egg-info/requires.txt
+-rw-r--r--   0 benishtainberg   (501) staff       (20)        9 2023-04-11 09:51:11.000000 stronger password package-1.0.3/src/stronger_password_package.egg-info/top_level.txt
+drwxr-xr-x   0 benishtainberg   (501) staff       (20)        0 2023-04-11 09:51:11.464063 stronger password package-1.0.3/tests/
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      235 2023-04-09 14:18:43.000000 stronger password package-1.0.3/tests/test_breached_password.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      297 2023-04-09 14:18:45.000000 stronger password package-1.0.3/tests/test_multi_factor_authetication.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      214 2023-04-09 14:18:47.000000 stronger password package-1.0.3/tests/test_password_generation.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      294 2023-04-09 14:18:47.000000 stronger password package-1.0.3/tests/test_password_hash.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      486 2023-04-09 14:18:47.000000 stronger password package-1.0.3/tests/test_strength_checker.py
+-rw-r--r--   0 benishtainberg   (501) staff       (20)      625 2023-04-09 14:18:49.000000 stronger password package-1.0.3/tests/test_suggest_improvements.py
```

### Comparing `stronger password package-1.0.2/LICENSE` & `stronger password package-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/PKG-INFO` & `stronger password package-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stronger password package
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for password security
 Home-page: https://github.com/Beny16112000/Stronger
 Author: Benjamin Shtainberg
 Author-email: benny132001@gmail.com
 Project-URL: Bug Tracker, https://github.com/Beny16112000/Stronger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stronger password package-1.0.2/README.md` & `stronger password package-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger/breached_password.py` & `stronger password package-1.0.3/src/stronger/breached_password.py`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger/password_generation.py` & `stronger password package-1.0.3/src/stronger/password_generation.py`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger/password_hash.py` & `stronger password package-1.0.3/src/stronger/password_hash.py`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger/strength_checker.py` & `stronger password package-1.0.3/src/stronger/strength_checker.py`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger/suggest_improvements.py` & `stronger password package-1.0.3/src/stronger/suggest_improvements.py`

 * *Files identical despite different names*

### Comparing `stronger password package-1.0.2/src/stronger_password_package.egg-info/PKG-INFO` & `stronger password package-1.0.3/src/stronger_password_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stronger-password-package
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for password security
 Home-page: https://github.com/Beny16112000/Stronger
 Author: Benjamin Shtainberg
 Author-email: benny132001@gmail.com
 Project-URL: Bug Tracker, https://github.com/Beny16112000/Stronger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stronger password package-1.0.2/src/stronger_password_package.egg-info/SOURCES.txt` & `stronger password package-1.0.3/src/stronger_password_package.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/stronger/password_generation.py
 src/stronger/password_hash.py
 src/stronger/strength_checker.py
 src/stronger/suggest_improvements.py
 src/stronger_password_package.egg-info/PKG-INFO
 src/stronger_password_package.egg-info/SOURCES.txt
 src/stronger_password_package.egg-info/dependency_links.txt
+src/stronger_password_package.egg-info/requires.txt
 src/stronger_password_package.egg-info/top_level.txt
 tests/test_breached_password.py
 tests/test_multi_factor_authetication.py
 tests/test_password_generation.py
 tests/test_password_hash.py
 tests/test_strength_checker.py
 tests/test_suggest_improvements.py
```

### Comparing `stronger password package-1.0.2/tests/test_suggest_improvements.py` & `stronger password package-1.0.3/tests/test_suggest_improvements.py`

 * *Files identical despite different names*

