# Comparing `tmp/astroemperor-0.8.1.tar.gz` & `tmp/astroemperor-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroemperor-0.8.1.tar", last modified: Tue Apr 11 17:30:00 2023, max compression
+gzip compressed data, was "astroemperor-0.8.2.tar", last modified: Tue Apr 11 17:35:14 2023, max compression
```

## Comparing `astroemperor-0.8.1.tar` & `astroemperor-0.8.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.373513 astroemperor-0.8.1/
--rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.1/LICENSE
--rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.1/MANIFEST.in
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:30:00.373281 astroemperor-0.8.1/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.1/README.md
--rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.1/pyproject.toml
--rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:30:00.373587 astroemperor-0.8.1/setup.cfg
--rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:26:42.000000 astroemperor-0.8.1/setup.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.350186 astroemperor-0.8.1/src/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.357062 astroemperor-0.8.1/src/astroemperor/
--rw-r--r--   0 reddtea    (501) staff       (20)    63078 2023-04-11 17:25:52.000000 astroemperor-0.8.1/src/astroemperor/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)    13842 2023-04-11 17:25:49.000000 astroemperor-0.8.1/src/astroemperor/block.py
--rw-r--r--   0 reddtea    (501) staff       (20)    20634 2023-04-11 17:25:45.000000 astroemperor-0.8.1/src/astroemperor/block_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    29477 2023-04-11 17:25:55.000000 astroemperor-0.8.1/src/astroemperor/canvas.py
--rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.1/src/astroemperor/model_repo.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.360976 astroemperor-0.8.1/src/astroemperor/support/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.362872 astroemperor-0.8.1/src/astroemperor/support/PAE/
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/00.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/01.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/02.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/03.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.1/src/astroemperor/support/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.1/src/astroemperor/support/endit.scr
--rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.1/src/astroemperor/support/endit_dyn.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:10.000000 astroemperor-0.8.1/src/astroemperor/support/init.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:09.000000 astroemperor-0.8.1/src/astroemperor/support/init_dyn.scr
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.363304 astroemperor-0.8.1/src/astroemperor/support/likelihoods/
--rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.1/src/astroemperor/support/likelihoods/00.like
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.367165 astroemperor-0.8.1/src/astroemperor/support/models/
--rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.1/src/astroemperor/support/models/acc.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.1/src/astroemperor/support/models/empty.model
--rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep03.model
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.370825 astroemperor-0.8.1/src/astroemperor/support/pools/
--rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.1/src/astroemperor/support/pools/00.pool
--rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.1/src/astroemperor/support/pools/01.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.1/src/astroemperor/support/pools/02.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.1/src/astroemperor/support/pools/03.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.1/src/astroemperor/support/pools/04.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.1/src/astroemperor/support/pools/05.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.1/src/astroemperor/support/pools/06.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.1/src/astroemperor/support/pools/07.pool
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.372923 astroemperor-0.8.1/src/astroemperor/support/priors/
--rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Fixed.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.1/src/astroemperor/support/priors/GaussianMixture.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Hill.prior
--rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Jeffreys.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Normal.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Uniform.prior
--rw-r--r--   0 reddtea    (501) staff       (20)     2942 2023-04-11 17:25:59.000000 astroemperor-0.8.1/src/astroemperor/unmodel_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    16308 2023-04-11 17:26:03.000000 astroemperor-0.8.1/src/astroemperor/utils.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.358489 astroemperor-0.8.1/src/astroemperor.egg-info/
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/SOURCES.txt
--rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/dependency_links.txt
--rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/requires.txt
--rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/top_level.txt
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.053519 astroemperor-0.8.2/
+-rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.2/LICENSE
+-rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.2/MANIFEST.in
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:35:14.053288 astroemperor-0.8.2/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.2/README.md
+-rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.2/pyproject.toml
+-rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:35:14.053586 astroemperor-0.8.2/setup.cfg
+-rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:34:51.000000 astroemperor-0.8.2/setup.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.030222 astroemperor-0.8.2/src/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.036985 astroemperor-0.8.2/src/astroemperor/
+-rw-r--r--   0 reddtea    (501) staff       (20)    63078 2023-04-11 17:34:57.000000 astroemperor-0.8.2/src/astroemperor/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    13842 2023-04-11 17:25:49.000000 astroemperor-0.8.2/src/astroemperor/block.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    20634 2023-04-11 17:25:45.000000 astroemperor-0.8.2/src/astroemperor/block_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    29661 2023-04-11 17:34:26.000000 astroemperor-0.8.2/src/astroemperor/canvas.py
+-rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.2/src/astroemperor/model_repo.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.040741 astroemperor-0.8.2/src/astroemperor/support/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.042892 astroemperor-0.8.2/src/astroemperor/support/PAE/
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/00.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/01.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/02.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.2/src/astroemperor/support/PAE/03.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.2/src/astroemperor/support/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.2/src/astroemperor/support/endit.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.2/src/astroemperor/support/endit_dyn.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:10.000000 astroemperor-0.8.2/src/astroemperor/support/init.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:09.000000 astroemperor-0.8.2/src/astroemperor/support/init_dyn.scr
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.043366 astroemperor-0.8.2/src/astroemperor/support/likelihoods/
+-rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.2/src/astroemperor/support/likelihoods/00.like
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.047144 astroemperor-0.8.2/src/astroemperor/support/models/
+-rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.2/src/astroemperor/support/models/acc.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.2/src/astroemperor/support/models/empty.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.2/src/astroemperor/support/models/ins02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.2/src/astroemperor/support/models/kep03.model
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.050865 astroemperor-0.8.2/src/astroemperor/support/pools/
+-rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.2/src/astroemperor/support/pools/00.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.2/src/astroemperor/support/pools/01.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.2/src/astroemperor/support/pools/02.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.2/src/astroemperor/support/pools/03.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.2/src/astroemperor/support/pools/04.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.2/src/astroemperor/support/pools/05.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.2/src/astroemperor/support/pools/06.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.2/src/astroemperor/support/pools/07.pool
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.052950 astroemperor-0.8.2/src/astroemperor/support/priors/
+-rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Fixed.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.2/src/astroemperor/support/priors/GaussianMixture.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Hill.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Jeffreys.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Normal.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.2/src/astroemperor/support/priors/Uniform.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)     2942 2023-04-11 17:25:59.000000 astroemperor-0.8.2/src/astroemperor/unmodel_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    16308 2023-04-11 17:26:03.000000 astroemperor-0.8.2/src/astroemperor/utils.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:35:14.038373 astroemperor-0.8.2/src/astroemperor.egg-info/
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/SOURCES.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/dependency_links.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/requires.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:35:14.000000 astroemperor-0.8.2/src/astroemperor.egg-info/top_level.txt
```

### Comparing `astroemperor-0.8.1/LICENSE` & `astroemperor-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/PKG-INFO` & `astroemperor-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.1
+Version: 0.8.2
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.1/README.md` & `astroemperor-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/setup.py` & `astroemperor-0.8.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="astroemperor",
-    version="0.8.1",
+    version="0.8.2",
     author="ReddTea",
     author_email="redd@tea.com",
     description="PTMCMC sampler for exoplanet search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/pypa/sampleproject",
     classifiers=[
```

### Comparing `astroemperor-0.8.1/src/astroemperor/__init__.py` & `astroemperor-0.8.2/src/astroemperor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # version 0.8.1
 # date 11 apr 2023
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 __name__ = 'astroemperor'
 __all__ = ['support']
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.1/src/astroemperor/block.py` & `astroemperor-0.8.2/src/astroemperor/block.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/block_repo.py` & `astroemperor-0.8.2/src/astroemperor/block_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/canvas.py` & `astroemperor-0.8.2/src/astroemperor/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,30 +32,38 @@
 from .block import ReddModel
 from .utils import fold_dataframe, nullify_output, flatten, get_support
 
 
 rc = Palette()
 
 
-def plot_GM_Estimator(estimator, saveloc='', fmt='png', sig_factor=4, fill_cor=0, plot_name='', plot_title=None, plot_ylabel=None):
+def plot_GM_Estimator(estimator, options=None):
     # sourcery skip: use-fstring-for-formatting
+    if options is None:
+        options = {}
+    if True:
+        saveloc = options['saveloc']
+        saveplace = saveloc + '/plots/GMEstimates/'
 
-    cor = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
-    colors = np.array([cor,cor,cor,cor,cor]).flatten()
+        plot_fmt = options['format']  # 'png'
+        plot_nm = options['plot_name']  # ''
+        plot_title = options['plot_title']  # None
+        plot_ylabel = options['plot_ylabel'] # None
+        fill_cor = options['fill_cor']  # 0
+
+        sig_factor = options['sig_factor']
 
-    if plot_title is None:
-        plot_title = 'Optimal estimate with Gaussian Mixtures\n for '
+        if plot_title is None:
+            plot_title = 'Optimal estimate with Gaussian Mixtures\n for '
 
-    if plot_ylabel is None:
-        plot_ylabel = 'Probability Density'
-    ## COL
-    sig_factor = sig_factor
-    saveplace = saveloc + '/posteriors/GMEstimates/'
-    plot_fmt = fmt
-    plot_nm = plot_name
+        if plot_ylabel is None:
+            plot_ylabel = 'Probability Density'
+
+    cor = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
+    colors = np.array([cor,cor,cor,cor,cor]).flatten()
 
 
     n_components = estimator.n_components
 
     mu = estimator.mixture_mean
     var = estimator.mixture_variance
     sig = estimator.mixture_sigma
@@ -72,20 +80,20 @@
 
         yy.append(np.exp(estimator.score_samples(xx[i])))
 
         xx[i] = np.append(np.append(xx[i][0], xx[i]), xx[i][-1])
         yy[i] = np.append(np.append(0, yy[i]), 0)
         ax.fill(xx[i], yy[i], c=colors[fill_cor], alpha=1/sig_factor, zorder=2*(i+1)-1)
 
+        vlines_kwargs = {'lw':[1.5, 1.5], 'ls':['--']}
         ax.vlines([xx[i][0], xx[i][-1]], ymin=[min(yy[i]), min(yy[i])],
                                          ymax=[yy[i][1], yy[i][-2]],
                                          colors=[rc.fg, rc.fg],
-                                         lw=[1.5, 1.5],
-                                         ls=['--'],
-                                         zorder=2*(i+1))
+                                         zorder=2*(i+1),
+                                         **vlines_kwargs)
 
         xticks.extend((xx[i][0], xx[i][-1]))
     ax.vlines(mu, ymin=[min(yy[0])],
                   ymax=[np.exp(estimator.score_samples([[mu]]))],
                   colors=[rc.fg],
                   lw=[2],
                   ls=['-'],
@@ -121,16 +129,16 @@
     xticks = np.round(xticks, nround)
     yticks = np.round(np.linspace(0, max(yy[0]), 5), 2)
 
     ax.tick_params(axis='x', labelrotation=45)
     ax.set_xticks(xticks, minor=False)
     ax.set_yticks(yticks, minor=False)
     ax.legend(framealpha=0.)
-    ax.set_title(plot_title+'{}'.format(plot_nm))
-    ax.set_xlabel('{} [{}]'.format(plot_nm, estimator.unit))
+    ax.set_title(plot_title+'{}'.format(plot_nm[2:]))
+    ax.set_xlabel('{} {}'.format(plot_nm[2:], estimator.unit))
     ax.set_ylabel(plot_ylabel)
 
 
     pl.savefig(saveplace+'{}.{}'.format(plot_nm, plot_fmt),
                bbox_inches='tight')
 
     pl.close('all')
@@ -140,15 +148,15 @@
     if trace_modes is None:
         trace_modes = [0]
     # 0:trace, 1:norm_post, 2:dens_interv, 3:corner
     trace_mode_dic = {0:'Trace Plot',
                       1:'Normalised Posterior',
                       2:'Density Interval',
                       3:'Corner Plot'}
-    saveplace = saveloc + '/traces/'
+    saveplace = saveloc + '/plots/traces/'
 
     cor = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
     colors_ = np.array([cor,cor,cor,cor,cor]).flatten()
     vn = np.array(flatten(my_model.get_attr_param('name')))[my_model.C_]
     for trace_mode in trace_modes:
         try:
             if eng_name == 'reddemcee':
@@ -166,65 +174,62 @@
                                     figsize=(14, len(vn_b)*2.5),
                                     var_names=vn_b,
                                     circ_var_names=circ_var_names,
                                     plot_kwargs={'color':rc.fg},
                                     trace_kwargs={'color':rc.fg})
 
                         pl.subplots_adjust(hspace=0.60)
-                        savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], b.name_, fmt)
+                        savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {b.name_}.{fmt}'
                         pl.savefig(savefigname)
 
-                # distr
                 elif trace_mode == 1:
                     for b in my_model:
                         for p in b[b.C_]:
                             fig, ax = pl.subplots(1, 1)
                             fig.suptitle(p.name)
 
                             az.plot_dist(arviz_data.posterior[p.name].values,
                                         color=rc.fg,
                                         rug=True,
                                         #figsize=(8, 6),
                                         )
                             #pl.ylabel('Probability Density')
                             pl.xlabel('Value')
 
-                            savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], p.name, fmt)
+                            savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {p.name}.{fmt}'
                             pl.savefig(savefigname)
-                # density intervals
                 elif trace_mode == 2:
                     for b in my_model:
                         axes = az.plot_density(
                             [arviz_data],
                             var_names=np.array(b.get_attr('name'))[b.C_],
                             shade=0.2,
                             colors=colors_[b.bnumber_-1],
                             #hdi_markers='v'
                             )
 
                         fig = axes.flatten()[0].get_figure()
                         fig.suptitle("94% High Density Intervals")
 
-                        savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], b.name_, fmt)
+                        savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {b.name_}.{fmt}'
                         pl.savefig(savefigname)
-                # corner plot
                 elif trace_mode == 3:
                     ax = az.plot_pair(arviz_data,
                             kind=["scatter", "kde"],
                             marginals=True,
                             marginal_kwargs={'color':rc.fg},
                             point_estimate="median",
                             scatter_kwargs={'color':rc.fg},
                             point_estimate_kwargs={'color':'red'},
                             point_estimate_marker_kwargs={'color':'red',
                                                         's':200,
                                                         'alpha':0.75},
                             )
 
-                    savefigname = saveplace+'{}.{}'.format(trace_mode_dic[trace_mode], fmt)
+                    savefigname = saveplace + f'{trace_mode_dic[trace_mode]}.{fmt}'
                     pl.savefig(savefigname)
 
             elif eng_name == 'dynesty':
                 from dynesty import plotting as dyplot
                 res2 = sampler
 
                 if trace_mode == 0:
@@ -232,31 +237,29 @@
                     for b in my_model:
                         vnb = np.array(b.get_attr('name'))[b.C_]
                         fig, axes = dyplot.traceplot(res2,
                                                     post_color=rc.fg,
                                                     trace_color=rc.fg,
                                                     labels=vnb,
                                                     dims=b.slice_true)
-                        savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], b.name_, fmt)
+                        savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {b.name_}.{fmt}'
                         pl.savefig(savefigname)
-                # Normalised Posterior
-                elif trace_mode == 1:   
+                elif trace_mode == 1:
                     arviz_data = az.from_emcee(sampler=sampler,
                                                 var_names=vn)
 
                     for b in my_model:
                         for p in b[b.C_]:
                             fig, ax = pl.subplots(1, 1)
                             fig.suptitle(p.name)
 
                             az.plot_dist(arviz_data.posterior[p.name].values)
 
-                            savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], p.name, fmt)
+                            savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {p.name}.{fmt}'
                             pl.savefig(savefigname)
-                # density intervals
                 elif trace_mode == 2:
                     arviz_data = az.from_emcee(sampler=sampler,
                                                 var_names=vn)
 
                     for b in my_model:
                         axes = az.plot_density(
                             [arviz_data],
@@ -264,60 +267,63 @@
                             shade=0.2,
                             #hdi_markers='v'
                             )
 
                         fig = axes.flatten()[0].get_figure()
                         fig.suptitle("94% High Density Intervals")
 
-                        savefigname = saveplace+'{} {}.{}'.format(trace_mode_dic[trace_mode], b.name_, fmt)
+                        savefigname = saveplace + f'{trace_mode_dic[trace_mode]} {b.name_}.{fmt}'
                         pl.savefig(savefigname)
-                # corner plot
                 elif trace_mode == 3:
                     arviz_data = az.from_emcee(sampler=sampler,
                                                 var_names=vn)
 
                     ax = az.plot_pair(arviz_data,
                             kind=["scatter", "kde"],
                             marginals=True,
                             marginal_kwargs={'color':rc.fg},
                             point_estimate="median",
                             scatter_kwargs={'color':rc.fg},
                             point_estimate_kwargs={'color':'red'},
                             point_estimate_marker_kwargs={'color':'red',
                                                         's':90},
                             )
-                    savefigname = saveplace+'{}.{}'.format(trace_mode_dic[trace_mode], fmt)
+                    savefigname = saveplace + f'{trace_mode_dic[trace_mode]}.{fmt}'
                     pl.savefig(savefigname)
 
             else:
-                print('Method is not yet implemented for {}'.format(eng_name))
+                print(f'Method is not yet implemented for {eng_name}')
                 return None
 
             pl.close('all')
         except:
             print(f'Trace plot for {trace_mode_dic[trace_mode]} failed!')
 
 
-def plot_KeplerianModel(my_data, my_model, res, saveloc='', options=None):
+def plot_KeplerianModel(my_data, my_model, res, options=None):
     if options is None:
         options = {}
     if True:
-        saveplace = saveloc + '/models/'
-        unsaveplace = saveloc + '/models/uncertainpy/'
+        saveloc = options['saveloc']
+        saveplace = saveloc + '/plots/models/'
+        unsaveplace = saveloc + '/plots/models/uncertainpy/'
 
         plot_fmt = options['format']
         switch_histogram = options['hist']
         switch_uncertain = options['uncertain']
         switch_errors = options['errors']
         logger_level = options['logger_level']
         gC = options['gC']
 
-
+        axhline_kwargs = {'color':'gray', 'linewidth':2}
+        errorbar_kwargs = {'marker':'o', 'ls':''}
+       
         posterior_method = 'GM'
-        c = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
+        #c = ['C0', 'C1', 'C2', 'C4', 'C5', 'C6', 'C7', 'C8', 'C9']
+        c = ['C0', 'C1', 'C2', 'C4', 'C6', 'C7', 'C8', 'C9']
         colors = np.array([c,c,c,c,c]).flatten()
 
         temp_file_names = []
         temp_mod_names = []
         temp_dat_names = []
 
         if switch_uncertain:
@@ -328,18 +334,18 @@
                 logging.getLogger("numpoly").setLevel(logger_level)
 
 
     def create_mod(data_arg, blocks_arg, tail_x, mod_number=0):
         x = ReddModel(data_arg, blocks_arg)
         x.A_ = []
 
-        temp_script = 'temp_mod_0{}.py'.format(mod_number)
+        temp_script = f'temp_mod_0{mod_number}.py'
         temp_file_names.append(temp_script)
-        temp_mod_names.append('{}/temp/temp_model_{}{}.py'.format(saveloc, x.model_script_no, tail_x))
-        temp_dat_names.append('{}/temp/temp_data{}.csv'.format(saveloc, tail_x))
+        temp_mod_names.append(f'{saveloc}/temp/temp_model_{x.model_script_no}{tail_x}.py')
+        temp_dat_names.append(f'{saveloc}/temp/temp_data{tail_x}.csv')
 
         with open(temp_script, 'w') as f:
             f.write(open(get_support('init.scr')).read())
             # DEPENDENCIES
             f.write('''
 import kepler
 ''')
@@ -411,58 +417,57 @@
                 axrh = fig.add_subplot(gs[2, 3], sharey=axr)
 
             else:
                 ax = fig.add_subplot(gs[:2, :])
                 axr = fig.add_subplot(gs[2, :], sharex=ax)
 
             pl.subplots_adjust(hspace=0)
-
-            ax.axhline(0, color='gray', linewidth=2)
-            axr.axhline(0, color='gray', linewidth=2)
+            ax.axhline(0, **axhline_kwargs)
+            axr.axhline(0, **axhline_kwargs)
 
             pl.subplots_adjust(wspace=0.15)
 
         # First we plot the data
         if True:
             for b_ins in NDB_A:
                 if b_ins.type_ == 'Instrumental':
                     mask = D['Flag'] == b_ins.number_
                     if switch_errors:
                         ax.errorbar(D[mask]['BJD'], D[mask]['RV'], D[mask]['eRV'],
-                                c=colors[b_ins.number_-1], marker='o', label=b_ins.instrument_label,
-                                ls='')
+                                c=colors[b_ins.number_-1], label=b_ins.instrument_label,
+                                **errorbar_kwargs)
 
                         axr.errorbar(D[mask]['BJD'], D[mask]['residuals'], D[mask]['eRV'],
-                                c=colors[b_ins.number_-1], marker='o',
-                                ls='')
+                                c=colors[b_ins.number_-1],
+                                **errorbar_kwargs)
                     else:
                         ax.plot(D[mask]['BJD'], D[mask]['RV'],
                                 colors[b_ins.number_-1]+'o', label=b_ins.instrument_label)
 
                         axr.plot(D[mask]['BJD'], D[mask]['residuals'], colors[b_ins.number_-1]+'o')
         # We set unmodels for uncertainties
         if True:
             for b in DB_A:
                 if b.parameterisation == 0:
-                    kepmod = Keplerian_Model
+                    #kepmod = Keplerian_Model
                     unkepmod = unKeplerian_Model
                     un_model_name = "unKeplerian_Model"
                     chaos_names = ['Period', 'Amplitude', 'Phase', 'Eccentricity', 'Longitude_Periastron']
                 if b.parameterisation == 1:
-                    kepmod = Keplerian_Model_1
+                    #kepmod = Keplerian_Model_1
                     unkepmod = unKeplerian_Model_1
                     un_model_name = "unKeplerian_Model_1"
                     chaos_names = ['lPeriod', 'Amp_sin', 'Amp_cos', 'Ecc_sin', 'Ecc_cos']
                 if b.parameterisation == 2:
-                    kepmod = Keplerian_Model_2
+                    #kepmod = Keplerian_Model_2
                     unkepmod = unKeplerian_Model_2
                     un_model_name = "unKeplerian_Model_2"
                     chaos_names = ['Period', 'Amplitude', 'Time_Periastron', 'Eccentricity', 'Longitude_Periastron']
                 if b.parameterisation == 3:
-                    kepmod = Keplerian_Model_3
+                    #kepmod = Keplerian_Model_3
                     unkepmod = unKeplerian_Model_3
                     un_model_name = "unKeplerian_Model_3"
                     chaos_names = ['Period', 'Amplitude', 'Time_Periastron', 'Ecc_sin', 'Ecc_cos']
 
         # Now we plot our line
         DB_AC = deepcopy(DB_A)
 
@@ -503,19 +508,19 @@
 
             axrh.set_xlabel('Counts')
         # Ticks and labels
         if True:
             ax.tick_params(axis="x", labelbottom=False)
 
             ax.set_title('Keplerian Model')
-            ax.set_ylabel(r'RVs $\frac{m}{s}$')
+            ax.set_ylabel(r'RVs ($\frac{m}{s}$)')
             ax.legend(fontsize=10)#, framealpha=0)
 
             axr.set_xlabel('BJD (days)')
-            axr.set_ylabel(r'Residuals $\frac{m}{s}$')
+            axr.set_ylabel(r'Residuals ($\frac{m}{s}$)')
 
             pl.savefig(saveplace+'{}.{}'.format('keplerian_model', plot_fmt),
                        bbox_inches='tight')
 
             # here we plot the phasefolded versions
 
         # we also need a grid for the residuals
@@ -577,18 +582,20 @@
             ## plot data per instrument
             for b_ins in NDB_A:
                 if b_ins.type_ == 'Instrumental':
                     mask = D_PF['Flag']==b_ins.number_
                     
                     if switch_errors:
                         ax.errorbar(D_PF[mask]['BJD'], D_PF[mask]['RV_D'], yerr=D_PF[mask]['eRV'],
-                                    c=colors[b_ins.number_-1], marker='o', ls='', label=b_ins.instrument_label)
+                                    c=colors[b_ins.number_-1], label=b_ins.instrument_label,
+                                    **errorbar_kwargs)
 
                         axr.errorbar(D_PF[mask]['BJD'], D_PF[mask]['residuals'], yerr=D_PF[mask]['eRV'],
-                                c=colors[b_ins.number_-1], marker='o', ls='')
+                                c=colors[b_ins.number_-1],
+                                **errorbar_kwargs)
                     else:
                         ax.plot(D_PF[mask]['BJD'], D_PF[mask]['RV_D'],
                                 colors[b_ins.number_-1]+'o', label=b_ins.instrument_label)
 
                         axr.plot(D_PF[mask]['BJD'], D_PF[mask]['residuals'],
                                 colors[b_ins.number_-1]+'o')
 
@@ -679,15 +686,15 @@
                         axs.set_title('First-order Sobol indices')
                         axs.set_xlabel('BJD (days)')
                         axs.set_ylabel('First-order Sobol indices')
                         axs.legend(parameters.get_from_uncertain(),
                                             loc='upper right',
                                             framealpha=0.5)
 
-                        figs.savefig(saveplace+'sobol_{}.{}'.format(b.name_+name_tail, plot_fmt),
+                        figs.savefig(saveplace+f'sobol_{b.name_+name_tail}.{plot_fmt}',
                                    bbox_inches='tight')
                         pl.close(figs)
                 # Plot Histogram Model
                 if switch_histogram:
                     nbins = 5
                     while nbins < len(D_PF):
                         counts, bins = np.histogram(D_PF['RV_D'], bins=nbins)
@@ -720,31 +727,31 @@
                         axrh.tick_params(axis="y", labelleft=False)
 
                     ax.set_title('Keplerian Model')
                     ax.set_ylabel(r'RVs $\frac{m}{s}$')
                     ax.legend(fontsize=10)#, framealpha=0)
 
                     axr.set_xlabel('BJD (days)')
-                    axr.set_ylabel(r'Residuals $\frac{m}{s}$')
+                    axr.set_ylabel(r'Residuals ($\frac{m}{s}$)')
 
 
 
-            pl.savefig(saveplace+'{}.{}'.format(b.name_+name_tail, plot_fmt),
+            pl.savefig(saveplace+f'{b.name_+name_tail}.{plot_fmt}',
                        bbox_inches='tight')
 
             nb_ += 1
 
             pbar.update(1)
 
 
             # print('MARKER 5')
             if nb_ == len(DB_A):
                 pbar.close()
 
-    temp_file_folder = saveloc+'/models/temp/'
+    temp_file_folder = saveloc+'/temp/models/'
 
 
     with nullify_output():
         for file in list(set(temp_file_names)):
             try:
                 os.system('mv {0} {1}{0}'.format(file, temp_file_folder))
             except Warning:
```

### Comparing `astroemperor-0.8.1/src/astroemperor/model_repo.py` & `astroemperor-0.8.2/src/astroemperor/model_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/endit.scr` & `astroemperor-0.8.2/src/astroemperor/support/endit.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/endit_dyn.scr` & `astroemperor-0.8.2/src/astroemperor/support/endit_dyn.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/models/ins01.model` & `astroemperor-0.8.2/src/astroemperor/support/models/ins01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/models/kep01.model` & `astroemperor-0.8.2/src/astroemperor/support/models/kep01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/models/kep03.model` & `astroemperor-0.8.2/src/astroemperor/support/models/kep03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/support/priors/Hill.prior` & `astroemperor-0.8.2/src/astroemperor/support/priors/Hill.prior`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/unmodel_repo.py` & `astroemperor-0.8.2/src/astroemperor/unmodel_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor/utils.py` & `astroemperor-0.8.2/src/astroemperor/utils.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.1/src/astroemperor.egg-info/PKG-INFO` & `astroemperor-0.8.2/src/astroemperor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.1
+Version: 0.8.2
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.1/src/astroemperor.egg-info/SOURCES.txt` & `astroemperor-0.8.2/src/astroemperor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

