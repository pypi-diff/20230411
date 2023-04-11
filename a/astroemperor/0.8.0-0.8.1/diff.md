# Comparing `tmp/astroemperor-0.8.0.tar.gz` & `tmp/astroemperor-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroemperor-0.8.0.tar", last modified: Tue Apr 11 17:20:58 2023, max compression
+gzip compressed data, was "astroemperor-0.8.1.tar", last modified: Tue Apr 11 17:30:00 2023, max compression
```

## Comparing `astroemperor-0.8.0.tar` & `astroemperor-0.8.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.137462 astroemperor-0.8.0/
--rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.0/LICENSE
--rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.0/MANIFEST.in
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:20:58.137182 astroemperor-0.8.0/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.0/README.md
--rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.0/pyproject.toml
--rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:20:58.137536 astroemperor-0.8.0/setup.cfg
--rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:20:38.000000 astroemperor-0.8.0/setup.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.114130 astroemperor-0.8.0/src/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.121348 astroemperor-0.8.0/src/astroemperor/
--rw-r--r--   0 reddtea    (501) staff       (20)    63076 2023-04-11 17:14:57.000000 astroemperor-0.8.0/src/astroemperor/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)    13840 2023-04-11 17:12:19.000000 astroemperor-0.8.0/src/astroemperor/block.py
--rw-r--r--   0 reddtea    (501) staff       (20)    20632 2023-04-11 17:10:00.000000 astroemperor-0.8.0/src/astroemperor/block_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    29475 2023-04-11 17:08:29.000000 astroemperor-0.8.0/src/astroemperor/canvas.py
--rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.0/src/astroemperor/model_repo.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.125004 astroemperor-0.8.0/src/astroemperor/support/
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.127085 astroemperor-0.8.0/src/astroemperor/support/PAE/
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/00.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/01.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/02.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/03.pae
--rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.0/src/astroemperor/support/__init__.py
--rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.0/src/astroemperor/support/endit.scr
--rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.0/src/astroemperor/support/endit_dyn.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      105 2022-12-29 16:50:21.000000 astroemperor-0.8.0/src/astroemperor/support/init.scr
--rw-r--r--   0 reddtea    (501) staff       (20)      105 2022-12-29 16:50:21.000000 astroemperor-0.8.0/src/astroemperor/support/init_dyn.scr
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.127568 astroemperor-0.8.0/src/astroemperor/support/likelihoods/
--rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.0/src/astroemperor/support/likelihoods/00.like
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.131250 astroemperor-0.8.0/src/astroemperor/support/models/
--rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.0/src/astroemperor/support/models/acc.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.0/src/astroemperor/support/models/empty.model
--rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep00.model
--rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep01.model
--rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep02.model
--rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep03.model
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.134736 astroemperor-0.8.0/src/astroemperor/support/pools/
--rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.0/src/astroemperor/support/pools/00.pool
--rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.0/src/astroemperor/support/pools/01.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.0/src/astroemperor/support/pools/02.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.0/src/astroemperor/support/pools/03.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.0/src/astroemperor/support/pools/04.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.0/src/astroemperor/support/pools/05.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.0/src/astroemperor/support/pools/06.pool
--rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.0/src/astroemperor/support/pools/07.pool
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.136823 astroemperor-0.8.0/src/astroemperor/support/priors/
--rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Fixed.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.0/src/astroemperor/support/priors/GaussianMixture.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Hill.prior
--rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Jeffreys.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Normal.prior
--rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Uniform.prior
--rw-r--r--   0 reddtea    (501) staff       (20)     2940 2023-04-11 17:08:35.000000 astroemperor-0.8.0/src/astroemperor/unmodel_repo.py
--rw-r--r--   0 reddtea    (501) staff       (20)    16306 2023-04-11 17:18:34.000000 astroemperor-0.8.0/src/astroemperor/utils.py
-drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.122738 astroemperor-0.8.0/src/astroemperor.egg-info/
--rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/PKG-INFO
--rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/SOURCES.txt
--rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/dependency_links.txt
--rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/requires.txt
--rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/top_level.txt
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.373513 astroemperor-0.8.1/
+-rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.1/LICENSE
+-rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.1/MANIFEST.in
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:30:00.373281 astroemperor-0.8.1/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.1/README.md
+-rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.1/pyproject.toml
+-rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:30:00.373587 astroemperor-0.8.1/setup.cfg
+-rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:26:42.000000 astroemperor-0.8.1/setup.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.350186 astroemperor-0.8.1/src/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.357062 astroemperor-0.8.1/src/astroemperor/
+-rw-r--r--   0 reddtea    (501) staff       (20)    63078 2023-04-11 17:25:52.000000 astroemperor-0.8.1/src/astroemperor/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    13842 2023-04-11 17:25:49.000000 astroemperor-0.8.1/src/astroemperor/block.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    20634 2023-04-11 17:25:45.000000 astroemperor-0.8.1/src/astroemperor/block_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    29477 2023-04-11 17:25:55.000000 astroemperor-0.8.1/src/astroemperor/canvas.py
+-rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.1/src/astroemperor/model_repo.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.360976 astroemperor-0.8.1/src/astroemperor/support/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.362872 astroemperor-0.8.1/src/astroemperor/support/PAE/
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/00.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/01.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/02.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.1/src/astroemperor/support/PAE/03.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.1/src/astroemperor/support/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.1/src/astroemperor/support/endit.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.1/src/astroemperor/support/endit_dyn.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:10.000000 astroemperor-0.8.1/src/astroemperor/support/init.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      118 2023-04-11 17:29:09.000000 astroemperor-0.8.1/src/astroemperor/support/init_dyn.scr
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.363304 astroemperor-0.8.1/src/astroemperor/support/likelihoods/
+-rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.1/src/astroemperor/support/likelihoods/00.like
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.367165 astroemperor-0.8.1/src/astroemperor/support/models/
+-rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.1/src/astroemperor/support/models/acc.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.1/src/astroemperor/support/models/empty.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.1/src/astroemperor/support/models/ins02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.1/src/astroemperor/support/models/kep03.model
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.370825 astroemperor-0.8.1/src/astroemperor/support/pools/
+-rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.1/src/astroemperor/support/pools/00.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.1/src/astroemperor/support/pools/01.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.1/src/astroemperor/support/pools/02.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.1/src/astroemperor/support/pools/03.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.1/src/astroemperor/support/pools/04.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.1/src/astroemperor/support/pools/05.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.1/src/astroemperor/support/pools/06.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.1/src/astroemperor/support/pools/07.pool
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.372923 astroemperor-0.8.1/src/astroemperor/support/priors/
+-rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Fixed.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.1/src/astroemperor/support/priors/GaussianMixture.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Hill.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Jeffreys.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Normal.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.1/src/astroemperor/support/priors/Uniform.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)     2942 2023-04-11 17:25:59.000000 astroemperor-0.8.1/src/astroemperor/unmodel_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    16308 2023-04-11 17:26:03.000000 astroemperor-0.8.1/src/astroemperor/utils.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:30:00.358489 astroemperor-0.8.1/src/astroemperor.egg-info/
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/SOURCES.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/dependency_links.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/requires.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:30:00.000000 astroemperor-0.8.1/src/astroemperor.egg-info/top_level.txt
```

### Comparing `astroemperor-0.8.0/LICENSE` & `astroemperor-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/PKG-INFO` & `astroemperor-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.0
+Version: 0.8.1
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.0/README.md` & `astroemperor-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/setup.py` & `astroemperor-0.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="astroemperor",
-    version="0.8.0",
+    version="0.8.1",
     author="ReddTea",
     author_email="redd@tea.com",
     description="PTMCMC sampler for exoplanet search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/pypa/sampleproject",
     classifiers=[
```

### Comparing `astroemperor-0.8.0/src/astroemperor/__init__.py` & `astroemperor-0.8.1/src/astroemperor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 __name__ = 'astroemperor'
 __all__ = ['support']
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.0/src/astroemperor/block.py` & `astroemperor-0.8.1/src/astroemperor/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.0/src/astroemperor/block_repo.py` & `astroemperor-0.8.1/src/astroemperor/block_repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.0/src/astroemperor/canvas.py` & `astroemperor-0.8.1/src/astroemperor/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # type: ignore
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 # sourcery skip
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
```

### Comparing `astroemperor-0.8.0/src/astroemperor/model_repo.py` & `astroemperor-0.8.1/src/astroemperor/model_repo.py`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/endit.scr` & `astroemperor-0.8.1/src/astroemperor/support/endit.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/endit_dyn.scr` & `astroemperor-0.8.1/src/astroemperor/support/endit_dyn.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/models/ins01.model` & `astroemperor-0.8.1/src/astroemperor/support/models/ins01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/models/kep01.model` & `astroemperor-0.8.1/src/astroemperor/support/models/kep01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/models/kep03.model` & `astroemperor-0.8.1/src/astroemperor/support/models/kep03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/support/priors/Hill.prior` & `astroemperor-0.8.1/src/astroemperor/support/priors/Hill.prior`

 * *Files identical despite different names*

### Comparing `astroemperor-0.8.0/src/astroemperor/unmodel_repo.py` & `astroemperor-0.8.1/src/astroemperor/unmodel_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.0/src/astroemperor/utils.py` & `astroemperor-0.8.1/src/astroemperor/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.8
+# version 0.8.1
 # date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.8.0/src/astroemperor.egg-info/PKG-INFO` & `astroemperor-0.8.1/src/astroemperor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.8.0
+Version: 0.8.1
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.8.0/src/astroemperor.egg-info/SOURCES.txt` & `astroemperor-0.8.1/src/astroemperor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

