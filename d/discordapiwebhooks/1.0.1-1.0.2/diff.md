# Comparing `tmp/discordapiwebhooks-1.0.1.tar.gz` & `tmp/discordapiwebhooks-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordapiwebhooks-1.0.1.tar", last modified: Mon Apr 10 13:25:17 2023, max compression
+gzip compressed data, was "discordapiwebhooks-1.0.2.tar", last modified: Tue Apr 11 06:27:37 2023, max compression
```

## Comparing `discordapiwebhooks-1.0.1.tar` & `discordapiwebhooks-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.354673 discordapiwebhooks-1.0.1/
--rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-10 13:25:17.346673 discordapiwebhooks-1.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 discordapiwebhooks-1.0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.286672 discordapiwebhooks-1.0.1/discordapiwebhooks/
--rw-rw----   0 root         (0) everybody  (9997)     2498 2023-04-10 13:17:43.000000 discordapiwebhooks-1.0.1/discordapiwebhooks/discordapiwebhooks.py
--rw-rw----   0 root         (0) everybody  (9997)     1693 2023-04-10 12:10:56.000000 discordapiwebhooks-1.0.1/discordapiwebhooks/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-10 13:25:17.342672 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      255 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       19 2023-04-10 13:25:17.000000 discordapiwebhooks-1.0.1/discordapiwebhooks.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-10 13:25:17.354673 discordapiwebhooks-1.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      368 2023-04-10 13:22:19.000000 discordapiwebhooks-1.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 06:27:37.734197 discordapiwebhooks-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-11 06:27:37.726197 discordapiwebhooks-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 discordapiwebhooks-1.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 06:27:37.674197 discordapiwebhooks-1.0.2/discordapiwebhooks/
+-rw-rw----   0 root         (0) everybody  (9997)     2498 2023-04-10 13:17:43.000000 discordapiwebhooks-1.0.2/discordapiwebhooks/discordapiwebhooks.py
+-rw-rw----   0 root         (0) everybody  (9997)     1693 2023-04-10 12:10:56.000000 discordapiwebhooks-1.0.2/discordapiwebhooks/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-11 06:27:37.718197 discordapiwebhooks-1.0.2/discordapiwebhooks.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      344 2023-04-11 06:27:37.000000 discordapiwebhooks-1.0.2/discordapiwebhooks.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      255 2023-04-11 06:27:37.000000 discordapiwebhooks-1.0.2/discordapiwebhooks.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-11 06:27:37.000000 discordapiwebhooks-1.0.2/discordapiwebhooks.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       19 2023-04-11 06:27:37.000000 discordapiwebhooks-1.0.2/discordapiwebhooks.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-11 06:27:37.734197 discordapiwebhooks-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      368 2023-04-11 06:26:35.000000 discordapiwebhooks-1.0.2/setup.py
```

### Comparing `discordapiwebhooks-1.0.1/README.md` & `discordapiwebhooks-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discordapiwebhooks-1.0.1/discordapiwebhooks/discordapiwebhooks.py` & `discordapiwebhooks-1.0.2/discordapiwebhooks/discordapiwebhooks.py`

 * *Files identical despite different names*

### Comparing `discordapiwebhooks-1.0.1/discordapiwebhooks/setup.py` & `discordapiwebhooks-1.0.2/discordapiwebhooks/setup.py`

 * *Files identical despite different names*

