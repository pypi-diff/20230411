# Comparing `tmp/slack_exception_logger-0.2.tar.gz` & `tmp/slack_exception_logger-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slack_exception_logger-0.2.tar", last modified: Sun Jan 15 07:08:17 2023, max compression
+gzip compressed data, was "dist/slack_exception_logger-0.3.tar", last modified: Tue Apr 11 07:13:16 2023, max compression
```

## Comparing `slack_exception_logger-0.2.tar` & `slack_exception_logger-0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-01-15 07:08:17.518649 slack_exception_logger-0.2/
--rw-r--r--   0 dillibabukadati   (501) staff       (20)     1084 2023-01-15 06:18:14.000000 slack_exception_logger-0.2/LICENSE
--rw-r--r--   0 dillibabukadati   (501) staff       (20)     2472 2023-01-15 07:08:17.518103 slack_exception_logger-0.2/PKG-INFO
--rw-r--r--   0 dillibabukadati   (501) staff       (20)     1612 2023-01-15 06:58:39.000000 slack_exception_logger-0.2/README.md
--rw-r--r--   0 dillibabukadati   (501) staff       (20)       38 2023-01-15 07:08:17.519110 slack_exception_logger-0.2/setup.cfg
--rw-r--r--   0 dillibabukadati   (501) staff       (20)      774 2023-01-15 07:06:12.000000 slack_exception_logger-0.2/setup.py
-drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-01-15 07:08:17.513440 slack_exception_logger-0.2/slack_exception_logger/
--rw-r--r--   0 dillibabukadati   (501) staff       (20)       94 2023-01-15 06:09:45.000000 slack_exception_logger-0.2/slack_exception_logger/__init__.py
--rw-r--r--   0 dillibabukadati   (501) staff       (20)     1050 2023-01-15 06:18:47.000000 slack_exception_logger-0.2/slack_exception_logger/slack_exception_logger.py
-drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-01-15 07:08:17.517049 slack_exception_logger-0.2/slack_exception_logger.egg-info/
--rw-r--r--   0 dillibabukadati   (501) staff       (20)     2472 2023-01-15 07:08:17.000000 slack_exception_logger-0.2/slack_exception_logger.egg-info/PKG-INFO
--rw-r--r--   0 dillibabukadati   (501) staff       (20)      339 2023-01-15 07:08:17.000000 slack_exception_logger-0.2/slack_exception_logger.egg-info/SOURCES.txt
--rw-r--r--   0 dillibabukadati   (501) staff       (20)        1 2023-01-15 07:08:17.000000 slack_exception_logger-0.2/slack_exception_logger.egg-info/dependency_links.txt
--rw-r--r--   0 dillibabukadati   (501) staff       (20)        9 2023-01-15 07:08:17.000000 slack_exception_logger-0.2/slack_exception_logger.egg-info/requires.txt
--rw-r--r--   0 dillibabukadati   (501) staff       (20)       23 2023-01-15 07:08:17.000000 slack_exception_logger-0.2/slack_exception_logger.egg-info/top_level.txt
+drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-04-11 07:13:16.080392 slack_exception_logger-0.3/
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     1084 2023-01-15 06:18:14.000000 slack_exception_logger-0.3/LICENSE
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     3588 2023-04-11 07:13:16.080057 slack_exception_logger-0.3/PKG-INFO
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     3114 2023-04-11 06:56:37.000000 slack_exception_logger-0.3/README.md
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)       38 2023-04-11 07:13:16.080506 slack_exception_logger-0.3/setup.cfg
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)      774 2023-04-11 07:13:03.000000 slack_exception_logger-0.3/setup.py
+drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-04-11 07:13:16.075361 slack_exception_logger-0.3/slack_exception_logger/
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)       94 2023-01-15 06:09:45.000000 slack_exception_logger-0.3/slack_exception_logger/__init__.py
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     3060 2023-04-11 06:36:00.000000 slack_exception_logger-0.3/slack_exception_logger/slack_exception_logger.py
+drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-04-11 07:13:16.078517 slack_exception_logger-0.3/slack_exception_logger.egg-info/
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     3588 2023-04-11 07:13:15.000000 slack_exception_logger-0.3/slack_exception_logger.egg-info/PKG-INFO
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)      376 2023-04-11 07:13:15.000000 slack_exception_logger-0.3/slack_exception_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)        1 2023-04-11 07:13:15.000000 slack_exception_logger-0.3/slack_exception_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)        9 2023-04-11 07:13:15.000000 slack_exception_logger-0.3/slack_exception_logger.egg-info/requires.txt
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)       23 2023-04-11 07:13:15.000000 slack_exception_logger-0.3/slack_exception_logger.egg-info/top_level.txt
+drwxr-xr-x   0 dillibabukadati   (501) staff       (20)        0 2023-04-11 07:13:16.079037 slack_exception_logger-0.3/tests/
+-rw-r--r--   0 dillibabukadati   (501) staff       (20)     1968 2023-01-15 06:09:45.000000 slack_exception_logger-0.3/tests/test_slack_exception_logger.py
```

### Comparing `slack_exception_logger-0.2/LICENSE` & `slack_exception_logger-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_exception_logger-0.2/setup.py` & `slack_exception_logger-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='slack_exception_logger',
-    version='0.2',
+    version='0.3',
     author='Dilli Babu Kadati',
     author_email='dillibabukadati777@gmail.com',
     description='A Python library for logging exceptions to a Slack channel',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/dillibk777/slack_exception_logger',
     packages=find_packages(),
```

