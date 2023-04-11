# Comparing `tmp/square_artkov-0.2.tar.gz` & `tmp/square_artkov-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "square_artkov-0.2.tar", last modified: Sun Apr  9 14:33:43 2023, max compression
+gzip compressed data, was "square_artkov-0.3.tar", last modified: Tue Apr 11 18:39:28 2023, max compression
```

## Comparing `square_artkov-0.2.tar` & `square_artkov-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 artkov    (1000) artkov    (1000)        0 2023-04-09 14:33:43.754749 square_artkov-0.2/
--rw-rw-r--   0 artkov    (1000) artkov    (1000)      253 2023-04-09 14:33:43.754749 square_artkov-0.2/PKG-INFO
--rw-rw-r--   0 artkov    (1000) artkov    (1000)       38 2023-04-09 14:33:43.754749 square_artkov-0.2/setup.cfg
--rw-rw-r--   0 artkov    (1000) artkov    (1000)      270 2023-04-09 14:28:58.000000 square_artkov-0.2/setup.py
-drwxrwxr-x   0 artkov    (1000) artkov    (1000)        0 2023-04-09 14:33:43.754749 square_artkov-0.2/square_artkov.egg-info/
--rw-rw-r--   0 artkov    (1000) artkov    (1000)      253 2023-04-09 14:33:43.000000 square_artkov-0.2/square_artkov.egg-info/PKG-INFO
--rw-rw-r--   0 artkov    (1000) artkov    (1000)      156 2023-04-09 14:33:43.000000 square_artkov-0.2/square_artkov.egg-info/SOURCES.txt
--rw-rw-r--   0 artkov    (1000) artkov    (1000)        1 2023-04-09 14:33:43.000000 square_artkov-0.2/square_artkov.egg-info/dependency_links.txt
--rw-rw-r--   0 artkov    (1000) artkov    (1000)        1 2023-04-09 14:33:43.000000 square_artkov-0.2/square_artkov.egg-info/top_level.txt
+drwxrwxr-x   0 artkov    (1000) artkov    (1000)        0 2023-04-11 18:39:28.713693 square_artkov-0.3/
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)      156 2023-04-11 18:39:28.713693 square_artkov-0.3/PKG-INFO
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)       38 2023-04-11 18:39:28.713693 square_artkov-0.3/setup.cfg
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)      269 2023-04-11 18:39:25.000000 square_artkov-0.3/setup.py
+drwxrwxr-x   0 artkov    (1000) artkov    (1000)        0 2023-04-11 18:39:28.713693 square_artkov-0.3/square_artkov.egg-info/
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)      156 2023-04-11 18:39:28.000000 square_artkov-0.3/square_artkov.egg-info/PKG-INFO
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)      156 2023-04-11 18:39:28.000000 square_artkov-0.3/square_artkov.egg-info/SOURCES.txt
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)        1 2023-04-11 18:39:28.000000 square_artkov-0.3/square_artkov.egg-info/dependency_links.txt
+-rw-rw-r--   0 artkov    (1000) artkov    (1000)        1 2023-04-11 18:39:28.000000 square_artkov-0.3/square_artkov.egg-info/top_level.txt
```

