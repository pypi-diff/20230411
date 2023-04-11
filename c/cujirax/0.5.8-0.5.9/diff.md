# Comparing `tmp/cujirax-0.5.8.tar.gz` & `tmp/cujirax-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.5.8.tar", last modified: Thu Mar 30 15:44:01 2023, max compression
+gzip compressed data, was "cujirax-0.5.9.tar", last modified: Fri Mar 31 00:59:20 2023, max compression
```

## Comparing `cujirax-0.5.8.tar` & `cujirax-0.5.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.5.8/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.5.8/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.5.8/README.md
--rw-r--r--   0        0        0     9355 2023-03-30 15:43:52.378712 cujirax-0.5.8/cujirax/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.5.8/cujirax/cucumber.py
--rw-r--r--   0        0        0     3618 2023-03-30 09:13:16.351957 cujirax-0.5.8/cujirax/jira.py
--rw-r--r--   0        0        0     1840 2023-03-28 16:21:23.991726 cujirax-0.5.8/cujirax/xray/__init__.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.5.8/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.5.8/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.5.9/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.5.9/README.md
+-rw-r--r--   0        0        0     9417 2023-03-31 00:59:00.087141 cujirax-0.5.9/cujirax/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.5.9/cujirax/cucumber.py
+-rw-r--r--   0        0        0     3618 2023-03-30 09:13:16.351957 cujirax-0.5.9/cujirax/jira.py
+-rw-r--r--   0        0        0     1840 2023-03-28 16:21:23.991726 cujirax-0.5.9/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.5.9/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.5.9/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.5.9/PKG-INFO
```

### Comparing `cujirax-0.5.8/.gitignore` & `cujirax-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/LICENSE` & `cujirax-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/README.md` & `cujirax-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/cujirax/__init__.py` & `cujirax-0.5.9/cujirax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
@@ -179,17 +179,17 @@
                     raise ValueError("More than 1 test key detected: ", tests, test_name)
             logger.info("search test case: " + test_name)
             logger.info(tests)
             found.append(el) if j.get_tests(test_name) else not_found.append(el)
         
         # check duplicate for new test
         if not ignore_duplicate:
-            duplicates = [item for item, count in Counter(not_found).items() if count > 1]
+            new_testnames = [cls.scenarioid_to_tescasename(el.id, el.keyword) for el in not_found]
+            duplicates = [item for item, count in Counter(new_testnames).items() if count > 1]
             if duplicates:
-                logger.error(duplicates)
                 raise ValueError("More than 1 same test detected: ", duplicates)
 
         return found, not_found
     
     @classmethod
     def _new_testcase(
         cls,
```

### Comparing `cujirax-0.5.8/cujirax/cucumber.py` & `cujirax-0.5.9/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/cujirax/jira.py` & `cujirax-0.5.9/cujirax/jira.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/cujirax/xray/__init__.py` & `cujirax-0.5.9/cujirax/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/cujirax/xray/import_results.py` & `cujirax-0.5.9/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/cujirax/xray/import_tests.py` & `cujirax-0.5.9/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.8/PKG-INFO` & `cujirax-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.5.8
+Version: 0.5.9
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

