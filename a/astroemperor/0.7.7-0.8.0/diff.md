# Comparing `tmp/astroemperor-0.7.7.tar.gz` & `tmp/astroemperor-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroemperor-0.7.7.tar", last modified: Wed Jan 18 04:27:28 2023, max compression
+gzip compressed data, was "astroemperor-0.8.0.tar", last modified: Tue Apr 11 17:20:58 2023, max compression
```

## Comparing `astroemperor-0.7.7.tar` & `astroemperor-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.835776 astroemperor-0.7.7/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1069 2022-03-30 16:38:19.000000 astroemperor-0.7.7/LICENSE
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      277 2023-01-17 19:51:16.000000 astroemperor-0.7.7/MANIFEST.in
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2457 2023-01-18 04:27:28.835776 astroemperor-0.7.7/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2081 2022-09-15 22:31:09.000000 astroemperor-0.7.7/README.md
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       85 2022-08-17 15:16:23.000000 astroemperor-0.7.7/pyproject.toml
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       38 2023-01-18 04:27:28.835776 astroemperor-0.7.7/setup.cfg
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1103 2023-01-18 04:17:35.000000 astroemperor-0.7.7/setup.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/astroemperor/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    58701 2023-01-18 03:58:36.000000 astroemperor-0.7.7/src/astroemperor/__init__.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    13847 2023-01-17 18:39:25.000000 astroemperor-0.7.7/src/astroemperor/block.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    20522 2023-01-17 19:07:03.000000 astroemperor-0.7.7/src/astroemperor/block_repo.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    29477 2023-01-17 19:56:29.000000 astroemperor-0.7.7/src/astroemperor/canvas.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     5918 2023-01-17 18:08:45.000000 astroemperor-0.7.7/src/astroemperor/model_repo.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/astroemperor/support/
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/astroemperor/support/PAE/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:23.000000 astroemperor-0.7.7/src/astroemperor/support/PAE/00.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      333 2022-12-29 16:47:23.000000 astroemperor-0.7.7/src/astroemperor/support/PAE/01.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      223 2022-12-29 16:47:27.000000 astroemperor-0.7.7/src/astroemperor/support/PAE/02.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      275 2022-12-29 16:47:30.000000 astroemperor-0.7.7/src/astroemperor/support/PAE/03.pae
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      152 2023-01-17 19:36:48.000000 astroemperor-0.7.7/src/astroemperor/support/__init__.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      765 2022-12-28 22:30:17.000000 astroemperor-0.7.7/src/astroemperor/support/endit.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1151 2023-01-02 18:48:43.000000 astroemperor-0.7.7/src/astroemperor/support/endit_dyn.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      120 2023-01-17 19:53:19.000000 astroemperor-0.7.7/src/astroemperor/support/init.scr
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      120 2023-01-17 19:52:38.000000 astroemperor-0.7.7/src/astroemperor/support/init_dyn.scr
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/astroemperor/support/likelihoods/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      173 2022-12-28 19:47:55.000000 astroemperor-0.7.7/src/astroemperor/support/likelihoods/00.like
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.835776 astroemperor-0.7.7/src/astroemperor/support/models/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      101 2023-01-05 19:26:19.000000 astroemperor-0.7.7/src/astroemperor/support/models/acc.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:16:53.000000 astroemperor-0.7.7/src/astroemperor/support/models/empty.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      166 2022-12-28 19:27:52.000000 astroemperor-0.7.7/src/astroemperor/support/models/ins00.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      736 2022-12-28 19:38:44.000000 astroemperor-0.7.7/src/astroemperor/support/models/ins01.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:16:39.000000 astroemperor-0.7.7/src/astroemperor/support/models/ins02.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      299 2022-12-28 03:15:07.000000 astroemperor-0.7.7/src/astroemperor/support/models/kep00.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      676 2022-12-29 20:00:49.000000 astroemperor-0.7.7/src/astroemperor/support/models/kep01.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      295 2022-12-28 19:20:49.000000 astroemperor-0.7.7/src/astroemperor/support/models/kep02.model
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      514 2022-12-28 19:21:54.000000 astroemperor-0.7.7/src/astroemperor/support/models/kep03.model
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.835776 astroemperor-0.7.7/src/astroemperor/support/pools/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       14 2022-12-28 20:00:54.000000 astroemperor-0.7.7/src/astroemperor/support/pools/00.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      131 2022-12-28 20:01:50.000000 astroemperor-0.7.7/src/astroemperor/support/pools/01.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       60 2022-12-28 20:01:44.000000 astroemperor-0.7.7/src/astroemperor/support/pools/02.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       74 2022-12-28 20:02:04.000000 astroemperor-0.7.7/src/astroemperor/support/pools/03.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       77 2022-12-28 20:02:17.000000 astroemperor-0.7.7/src/astroemperor/support/pools/04.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:32.000000 astroemperor-0.7.7/src/astroemperor/support/pools/05.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       64 2022-12-28 20:02:38.000000 astroemperor-0.7.7/src/astroemperor/support/pools/06.pool
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       63 2022-12-28 20:02:47.000000 astroemperor-0.7.7/src/astroemperor/support/pools/07.pool
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.835776 astroemperor-0.7.7/src/astroemperor/support/priors/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       44 2022-12-28 19:49:04.000000 astroemperor-0.7.7/src/astroemperor/support/priors/Fixed.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      193 2023-01-05 23:00:32.000000 astroemperor-0.7.7/src/astroemperor/support/priors/GaussianMixture.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      818 2022-12-29 14:42:23.000000 astroemperor-0.7.7/src/astroemperor/support/priors/Hill.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        0 2022-12-29 20:03:14.000000 astroemperor-0.7.7/src/astroemperor/support/priors/Jeffreys.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      205 2022-12-28 19:48:53.000000 astroemperor-0.7.7/src/astroemperor/support/priors/Normal.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      122 2022-12-28 19:48:39.000000 astroemperor-0.7.7/src/astroemperor/support/priors/Uniform.prior
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2940 2023-01-02 23:17:10.000000 astroemperor-0.7.7/src/astroemperor/unmodel_repo.py
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)    14072 2023-01-17 18:29:07.000000 astroemperor-0.7.7/src/astroemperor/utils.py
-drwxrwxr-x   0 reddtea   (1000) reddtea   (1000)        0 2023-01-18 04:27:28.831776 astroemperor-0.7.7/src/astroemperor.egg-info/
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     2457 2023-01-18 04:27:28.000000 astroemperor-0.7.7/src/astroemperor.egg-info/PKG-INFO
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)     1812 2023-01-18 04:27:28.000000 astroemperor-0.7.7/src/astroemperor.egg-info/SOURCES.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)        1 2023-01-18 04:27:28.000000 astroemperor-0.7.7/src/astroemperor.egg-info/dependency_links.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)      123 2023-01-18 04:27:28.000000 astroemperor-0.7.7/src/astroemperor.egg-info/requires.txt
--rw-rw-r--   0 reddtea   (1000) reddtea   (1000)       13 2023-01-18 04:27:28.000000 astroemperor-0.7.7/src/astroemperor.egg-info/top_level.txt
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.137462 astroemperor-0.8.0/
+-rw-r--r--   0 reddtea    (501) staff       (20)     1069 2022-03-30 16:38:19.000000 astroemperor-0.8.0/LICENSE
+-rw-r--r--   0 reddtea    (501) staff       (20)      277 2023-01-17 19:51:16.000000 astroemperor-0.8.0/MANIFEST.in
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:20:58.137182 astroemperor-0.8.0/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     2081 2022-09-15 22:31:09.000000 astroemperor-0.8.0/README.md
+-rw-r--r--   0 reddtea    (501) staff       (20)       85 2022-08-17 15:16:23.000000 astroemperor-0.8.0/pyproject.toml
+-rw-r--r--   0 reddtea    (501) staff       (20)       38 2023-04-11 17:20:58.137536 astroemperor-0.8.0/setup.cfg
+-rw-r--r--   0 reddtea    (501) staff       (20)     1103 2023-04-11 17:20:38.000000 astroemperor-0.8.0/setup.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.114130 astroemperor-0.8.0/src/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.121348 astroemperor-0.8.0/src/astroemperor/
+-rw-r--r--   0 reddtea    (501) staff       (20)    63076 2023-04-11 17:14:57.000000 astroemperor-0.8.0/src/astroemperor/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    13840 2023-04-11 17:12:19.000000 astroemperor-0.8.0/src/astroemperor/block.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    20632 2023-04-11 17:10:00.000000 astroemperor-0.8.0/src/astroemperor/block_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    29475 2023-04-11 17:08:29.000000 astroemperor-0.8.0/src/astroemperor/canvas.py
+-rw-r--r--   0 reddtea    (501) staff       (20)     5918 2023-04-11 17:08:32.000000 astroemperor-0.8.0/src/astroemperor/model_repo.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.125004 astroemperor-0.8.0/src/astroemperor/support/
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.127085 astroemperor-0.8.0/src/astroemperor/support/PAE/
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:23.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/00.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      333 2022-12-29 16:47:23.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/01.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      223 2022-12-29 16:47:27.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/02.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      275 2022-12-29 16:47:30.000000 astroemperor-0.8.0/src/astroemperor/support/PAE/03.pae
+-rw-r--r--   0 reddtea    (501) staff       (20)      152 2023-01-17 19:36:51.000000 astroemperor-0.8.0/src/astroemperor/support/__init__.py
+-rw-r--r--   0 reddtea    (501) staff       (20)      765 2022-12-28 22:30:54.000000 astroemperor-0.8.0/src/astroemperor/support/endit.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)     1151 2023-01-02 18:48:43.000000 astroemperor-0.8.0/src/astroemperor/support/endit_dyn.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      105 2022-12-29 16:50:21.000000 astroemperor-0.8.0/src/astroemperor/support/init.scr
+-rw-r--r--   0 reddtea    (501) staff       (20)      105 2022-12-29 16:50:21.000000 astroemperor-0.8.0/src/astroemperor/support/init_dyn.scr
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.127568 astroemperor-0.8.0/src/astroemperor/support/likelihoods/
+-rw-r--r--   0 reddtea    (501) staff       (20)      173 2022-12-28 20:41:05.000000 astroemperor-0.8.0/src/astroemperor/support/likelihoods/00.like
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.131250 astroemperor-0.8.0/src/astroemperor/support/models/
+-rw-r--r--   0 reddtea    (501) staff       (20)      101 2023-01-05 19:26:19.000000 astroemperor-0.8.0/src/astroemperor/support/models/acc.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:53.000000 astroemperor-0.8.0/src/astroemperor/support/models/empty.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      166 2022-12-28 19:27:52.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      736 2022-12-28 19:38:44.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 03:16:39.000000 astroemperor-0.8.0/src/astroemperor/support/models/ins02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      299 2022-12-28 19:17:04.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep00.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      676 2022-12-29 20:00:49.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep01.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      295 2022-12-28 19:20:51.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep02.model
+-rw-r--r--   0 reddtea    (501) staff       (20)      514 2022-12-28 19:21:54.000000 astroemperor-0.8.0/src/astroemperor/support/models/kep03.model
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.134736 astroemperor-0.8.0/src/astroemperor/support/pools/
+-rw-r--r--   0 reddtea    (501) staff       (20)       14 2022-12-28 20:00:54.000000 astroemperor-0.8.0/src/astroemperor/support/pools/00.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)      158 2023-01-20 19:38:29.000000 astroemperor-0.8.0/src/astroemperor/support/pools/01.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       60 2022-12-28 20:01:54.000000 astroemperor-0.8.0/src/astroemperor/support/pools/02.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       74 2022-12-28 20:02:04.000000 astroemperor-0.8.0/src/astroemperor/support/pools/03.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       77 2022-12-28 20:02:17.000000 astroemperor-0.8.0/src/astroemperor/support/pools/04.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:32.000000 astroemperor-0.8.0/src/astroemperor/support/pools/05.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       64 2022-12-28 20:02:38.000000 astroemperor-0.8.0/src/astroemperor/support/pools/06.pool
+-rw-r--r--   0 reddtea    (501) staff       (20)       63 2022-12-28 20:02:47.000000 astroemperor-0.8.0/src/astroemperor/support/pools/07.pool
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.136823 astroemperor-0.8.0/src/astroemperor/support/priors/
+-rw-r--r--   0 reddtea    (501) staff       (20)       44 2022-12-28 19:49:04.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Fixed.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      193 2023-01-05 23:00:32.000000 astroemperor-0.8.0/src/astroemperor/support/priors/GaussianMixture.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      818 2022-12-29 14:42:23.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Hill.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)        0 2022-12-29 20:03:14.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Jeffreys.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      205 2022-12-28 19:48:53.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Normal.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)      122 2022-12-28 19:48:39.000000 astroemperor-0.8.0/src/astroemperor/support/priors/Uniform.prior
+-rw-r--r--   0 reddtea    (501) staff       (20)     2940 2023-04-11 17:08:35.000000 astroemperor-0.8.0/src/astroemperor/unmodel_repo.py
+-rw-r--r--   0 reddtea    (501) staff       (20)    16306 2023-04-11 17:18:34.000000 astroemperor-0.8.0/src/astroemperor/utils.py
+drwxr-xr-x   0 reddtea    (501) staff       (20)        0 2023-04-11 17:20:58.122738 astroemperor-0.8.0/src/astroemperor.egg-info/
+-rw-r--r--   0 reddtea    (501) staff       (20)     2457 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/PKG-INFO
+-rw-r--r--   0 reddtea    (501) staff       (20)     1812 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/SOURCES.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)        1 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/dependency_links.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)      123 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/requires.txt
+-rw-r--r--   0 reddtea    (501) staff       (20)       13 2023-04-11 17:20:58.000000 astroemperor-0.8.0/src/astroemperor.egg-info/top_level.txt
```

### Comparing `astroemperor-0.7.7/LICENSE` & `astroemperor-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/PKG-INFO` & `astroemperor-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: astroemperor
-Version: 0.7.7
-Summary: PTMCMC sampler for exoplanet search
-Author: ReddTea
-Author-email: redd@tea.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Reddutils
 
 This is ReddTea's small package compiling useful self-made functions for an astrophysical context.
 
 # Overview
 Reddutils contains many functions and classes for personal use.
 Some of them may be of use for the community.
```

### Comparing `astroemperor-0.7.7/README.md` & `astroemperor-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: astroemperor
+Version: 0.8.0
+Summary: PTMCMC sampler for exoplanet search
+Author: ReddTea
+Author-email: redd@tea.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Reddutils
 
 This is ReddTea's small package compiling useful self-made functions for an astrophysical context.
 
 # Overview
 Reddutils contains many functions and classes for personal use.
 Some of them may be of use for the community.
```

### Comparing `astroemperor-0.7.7/setup.py` & `astroemperor-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="astroemperor",
-    version="0.7.7",
+    version="0.8.0",
     author="ReddTea",
     author_email="redd@tea.com",
     description="PTMCMC sampler for exoplanet search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/pypa/sampleproject",
     classifiers=[
```

### Comparing `astroemperor-0.7.7/src/astroemperor/__init__.py` & `astroemperor-0.8.0/src/astroemperor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.7.1
-# date 17 jan 2023
+# version 0.8
+# date 11 apr 2023
 
-__version__ = '0.7.7'
+__version__ = '0.8.0'
 __name__ = 'astroemperor'
 __all__ = ['support']
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
@@ -16,18 +16,20 @@
 
 # sourcery skip: remove-redundant-if
 if True:
     import numpy as np
     import pandas as pd
     
     import os
+    import time
     import pickle
 
     import itertools
     import multiprocessing
+    from importlib import reload
 
     from tabulate import tabulate
     from termcolor import colored
     from tqdm import tqdm
 
 
     from .utils import *
@@ -42,16 +44,14 @@
         terminal_width = pd.get_option('display.width')
 
 stat_names_ = ['chi2', 'chi2_red', 'AIC', 'BIC',
                'DIC', 'HQIC', 'RMSE', 'post_max',
                'like_max', 'BayesFactor']
 
 
-
-
 class ModelSelectionObj:
     def __init__(self, crit):
         self._current_criteria = crit
         self._tolerance = 5
         self.compare_f = self.foobarmin
         self.dict = {'chi2':None, 'chi2_red':None, 'AIC':self.foobarmin, 'BIC':self.foobarmin,
                      'DIC':self.foobarmin, 'HQIC':self.foobarmin, 'RMSE':None, 'post_max':None,
@@ -118,15 +118,15 @@
 
         self.starmass = 1.
         Nonethings = ['starname', 'betas', 'saveplace']
         for c in Nonethings:
             setattr(self, c, None)
 
         switches = ['switch_first', 'switch_RV', 'switch_SA', 'switch_constrain',
-                    'switch_dynamics', 'dynamics_already_included']
+                    'switch_dynamics', 'dynamics_already_included', 'debug_mode']
         for switch in switches:
             setattr(self, switch, False)
 
         switches_T = ['switch_evidence', 'gaussian_mixtures_fit']
         for switch in switches_T:
             setattr(self, switch, True)
 
@@ -164,14 +164,15 @@
 
         # Writing stuff
         self.general_dependencies = []
         self.dynesty_config = {'dlogz_init':0.05,
                                 }
         self.reddemcee_config = {'burnin':'half',
                                 'thinby':1,
+                                'logger_level':'CRITICAL',
                                 }
 
         #self.ModelSelection = 'BIC'
         self.ModelSelection = ModelSelectionObj('BIC')
         self.evidence = 0, 0
 
 
@@ -183,32 +184,37 @@
         # plots
         self.instrument_names = None
 
 
         self.plot_gaussian_mixtures = {'plot':True,
                                         'sig_factor':4,
                                         'plot_title':None,
-                                        'plot_ylabel':None}
-        #self.plot_gaussian_mixtures = True
+                                        'plot_ylabel':None,
+                                        'saveloc':'',
+                                        'format':self.save_plots_fmt,
+                                        'fill_cor':0,
+                                        'plot_name':''}
+
         self.plot_keplerian_model = {'plot':True,
                                      'hist':True,
                                      'uncertain':True,
                                      'errors':False,
                                      'format':'png',
                                      'logger_level':'ERROR',
-                                     'gC':0}
+                                     'gC':0,
+                                     'saveloc':''}
 
         self.plot_trace = {'plot':True,
                            'modes':[0, 1, 2, 3],
                            'temp':0}
 
         self.parameter_histograms = False
         self.corner = (np.array(self.plot_trace['modes']) == 3).any()
 
-        self.save_chains = [0]
+        self.save_chains = None #  [0]
         self.save_likelihoods = [0]
         self.save_posteriors = [0]
         self.logger('   ', center=True, save=False, c='green', attrs=['bold', 'reverse'])
         self.logger('~~ Simulation Successfully Initialized ~~', center=True, save=False, c='green', attrs=['bold', 'reverse'])
         self.logger('   ', center=True, save=False, c='green', attrs=['bold', 'reverse'])
 
 
@@ -232,19 +238,20 @@
 
         elif eng == 'pymc3':
             import pymc3 as pm
             self.engine__ = pm
         elif eng == 'reddemcee':
             import reddemcee
             self.engine__ = reddemcee
-            self.general_dependencies.append('reddemcee')
-            self.general_dependencies.append('emcee')
+            self.general_dependencies.extend(['reddemcee', 'emcee', 'logging'])
 
             self.reddemcee_config['burnin'] = 'half'
             self.reddemcee_config['thinby'] = 1
+            self.reddemcee_config['logger_level'] = 'CRITICAL'
+            
         else:
             raise Exception(self.logger('Failed to set engine properly. Try a string!', center=True, c='red'))
 
 
     def load_data(self, folder_name):
         self.starname = folder_name
         self.data_wrapper = DataWrapper(folder_name, read_loc=self.read_loc)
@@ -329,22 +336,27 @@
         #if self.model.update_additional_priors():
         #    self.update_additional_priors_block()
         self.model.refresh__()
 
 
     def run(self, setup, progress=True):
         ### assert errors!
-        ##
+        if self.debug_mode:
+            #self.set_marker('begin run')
+            print(f'run  : begin | {time.time()-self.debug_timer}')
+
         if self.constrain_method == 'GM':
             if not self.gaussian_mixtures_fit:
                 msg = 'Invalid constrain_method = GM with .gaussian_mixtures_fit = False'
                 raise SyntaxError(msg)
 
         self.apply_conditions()
         self.saveplace = ensure_dir(self.starname, loc=self.save_loc)
+        self.plot_keplerian_model['saveloc'] = self.saveplace
+        self.plot_gaussian_mixtures['saveloc'] = self.saveplace
         #self.temp_script = self.saveplace+'/temp/temp_script.py'
         self.temp_script = 'temp_script.py'
 
         if not self.switch_first:
             self.logger('\n')
             self.logger('~~ Setup Info ~~', center=True, c='blue', attrs=['reverse'])
             self.logger('\nCurrent Engine is  '+colored(self.engine__.__name__+' '+self.engine__.__version__, attrs=['bold']), c='blue')
@@ -433,37 +445,41 @@
 
             self.logger('\n')
             for b in self:
                 self.logger('Math for {}:\n'.format(b.name_), c='yellow')
                 self.logger('{}'.format(b.math_display_), center=True, c='yellow')
 
             self.logger('\n')
-
-
+        if self.debug_mode:
+            print(f'run  : init sampler | {time.time()-self.debug_timer}')
         if self.engine__.__name__ == 'reddemcee':
             from emcee.backends import HDFBackend
             ntemps, nwalkers, nsteps = setup
-
-            self.write_model()
-
-            os.system('ipython {}'.format(self.temp_script))
-
+            if self.debug_mode:
+                print(f'run  : Write_script() | {time.time()-self.debug_timer}')
+            self.write_script()
+
+            if self.debug_mode:
+                #self.set_marker('begin run_script.py')
+                print(f'run  : os <run temp_script.py> | {time.time()-self.debug_timer}')
+            os.system(f'ipython {self.temp_script}')
             self.sampler = self.engine__.PTSampler(nwalkers, self.model.ndim__,
-                                         self.model.evaluate_loglikelihood,
-                                         self.model.evaluate_logprior,
+                                         self.temp_like_func,
+                                         self.temp_prior_func,
                                          logl_args=[], logl_kwargs={},
                                          logp_args=[], logp_kwargs={},
                                          ntemps=ntemps, pool=None)
 
             #self.sampler = [None for _ in range(ntemps)]
             with open('sampler_pickle.pkl', 'rb') as sampler_metadata:
                 self.sampler_metadata_dict = pickle.load(sampler_metadata)
-
+            os.system(f'mv sampler_pickle.pkl {self.saveplace}/restore/sampler_pickle.pkl')
+            
             for t in range(ntemps):
-                loc_t = '{}emperor_backend_{}.h5'.format(self.saveplace+'/temp/', t)
+                loc_t = '{}emperor_backend_{}.h5'.format(self.saveplace+'/restore/backends/', t)
                 self.sampler[t] = HDFBackend(loc_t)
 
         if self.engine__.__name__ == 'dynesty':
             # TRANSFORM TO PTFORMARGS
             # This is missing additional_parameters ! !
 
             self.ptformargs0 = []
@@ -485,30 +501,35 @@
                         self.ptformargs0.append(p.ptformargs)
 
 
             if self.engine__args == 'dynamic':
                 # SET SETUP
                 nlive0, nlive_batch0 = setup
                 # SET SAMPLER
-                self.write_model()
+                self.write_script()
 
                 # RUN SAMPLER
                 os.system('ipython {}'.format(self.temp_script))
 
                 with open('sampler_pickle.pkl', 'rb') as sampler_metadata:
                     self.sampler_metadata_dict = pickle.load(sampler_metadata)
-                pass
+                os.system(f'mv sampler_pickle.pkl {self.saveplace}/restore/sampler_pickle.pkl')
             else:
                 # SET SETUP
                 # SET SAMPLER
                 # RUN SAMPLER
                 pass
 
-
+        
     def run_auto(self, setup, k_start=0, k_end=10, parameterisation=1, moav=0, accel=0, progress=True):
+        if self.debug_mode:
+            #self.set_marker('begin autorun')
+            self.debug_timer = time.time()
+            print(f'run_auto : INIT run_auto | {time.time()-self.debug_timer}')
+
         self.auto_setup = setup
         if self.engine__.__name__ in ['emcee', 'dynesty', 'pymc3', 'reddemcee']:
 
             if self.switch_RV and not self.switch_SA:
                 self.add_instrumental_blocks(moav=moav)
             if accel:
                 self.add_acceleration_block(accel=accel)
@@ -569,18 +590,31 @@
                                         self.add_condition([p.name, 'prior', 'Normal'])
                                         self.add_condition([p.name, 'prargs', prarg0])
 
                                     elif p.GM_parameter.n_components > 1:
                                         self.add_condition([p.name, 'prior', 'GaussianMixture'])
                                         self.add_condition([p.name, 'prargs', [self.model.C_[count]]])
                                     count += 1
+
+                if True:
+                    run_metadata = {}
+
+                    # to restore, we need
+                    # my_data
+                    # model? .evaluate_model?!?!?!
+                    # ymod, ferr2, residuals
+
+                    with open(f'{self.saveplace}/restore/run_pickle.pkl','wb') as md_save:
+                        pickle.dump(run_metadata, md_save)
+
+
                 # if not continue, model selec
                 if self.ModelSelection.compare(self.BIC, oldBIC):
-                    oldbic_display = np.round(oldBIC, 3)
-                    newbic_display = np.round(self.BIC, 3)
+                    #oldbic_display = np.round(oldBIC, 3)
+                    #newbic_display = np.round(self.BIC, 3)
                     self.logger('\nBIC condition met!!', c='blue', attrs=['bold'])
                     self.logger('present BIC < past BIC - 5', c='blue')
                     self.logger(self.ModelSelection.msg, c='blue')
                 else:
                     self.logger('\nBIC condition not met', c='blue')
                     self.logger('present BIC < past BIC - 5', c='blue')
                     self.logger(self.ModelSelection.msg, c='blue')
@@ -714,44 +748,51 @@
             self.fit_max = raw_chain[0][best_loc]
             self.fit_mean = raw_chain[0][best_loc]
             self.fit_median = raw_chain[0][best_loc]
 
             print('\n\n------------ Dynesty Summary -----------\n\n')
             print(str(results.summary()))
 
-
         chains = raw_chain
         posts = raw_posts
         likes = raw_likes
 
-
         ###########################################
         ###########################################
         # GET STATS
         if True:
             if self.switch_RV:
-                ymod, err2 = self.model.evaluate_model(self.ajuste)
+                ymod, err2 = self.temp_model_func(self.ajuste)
+                ymod, err2 = ymod.values, err2.values
+
                 ferr2 = err2 + self.my_data['eRV'].values ** 2
                 residuals = self.my_data['RV'].values - ymod
 
                 ndim = self.model.ndim__
                 ndat = self.model.ndata
 
+                np.savetxt(f'{self.saveplace}/restore/residuals.dat', np.array([self.my_data['BJD'].values,
+                                                      residuals,
+                                                      self.my_data['eRV'].values,
+                                                      self.my_data['Flag'].values,
+                                                      ]))
+
                 rss = np.sum(residuals**2)
 
                 self.dof = ndat - ndim
                 self.chi2 = rss / self.dof
                 self.chi2_red = np.sum(residuals**2 / ferr2) / self.dof
                 self.RMSE = np.sqrt(np.sum(residuals ** 2) / len(residuals))
 
                 self.AIC = 2 * ndim - 2 * self.like_max
                 self.BIC = np.log(ndat) * ndim - 2 * self.like_max
 
                 tm = np.mean(raw_chain[0], axis=0)
-                self.DIC = -2 * self.model.evaluate_loglikelihood(tm) + np.var(-2 * likes[0])
+
+                self.DIC = -2 * self.temp_like_func(tm) + np.var(-2 * likes[0])
 
                 self.post_true = self.post_max - self.evidence[0]
                 self.BayesFactor = self.like_max - self.evidence[0]
 
                 self.HQIC = 2 * ndim * np.log(np.log(ndat)) - 2 * self.like_max
 
         ## SET P.VALUES P.SIGMA
@@ -1078,44 +1119,37 @@
         # PLOT GM PER PARAMETER
         if self.gaussian_mixtures_fit:
             if self.plot_gaussian_mixtures['plot']:
                 self.logger('Plotting Gaussian Mixtures', center=True, c='green')
                 pbar_tot = self.model.ndim__
                 pbar = tqdm(total=pbar_tot)
                 for b in self:
+                    self.plot_gaussian_mixtures['fill_cor'] = b.bnumber_-1
                     for p in b[b.C_]:
+                        self.plot_gaussian_mixtures['plot_name'] = f'{b.bnumber_} {p.GM_parameter.name}'
+
                         plot_GM_Estimator(p.GM_parameter,
-                                        saveloc=self.saveplace,
-                                        fmt=self.save_plots_fmt,
-                                        sig_factor=self.plot_gaussian_mixtures['sig_factor'],
-                                        fill_cor=b.bnumber_-1,
-                                        plot_name='{} '.format(b.bnumber_) + p.GM_parameter.name,
-                                        plot_title=self.plot_gaussian_mixtures['plot_title'],
-                                        plot_ylabel=self.plot_gaussian_mixtures['plot_ylabel'])
+                                          options=self.plot_gaussian_mixtures)
+
                         pbar.update(1)
                     for p in b.additional_parameters:
                         if p.has_posterior:
+                            self.plot_gaussian_mixtures['plot_name'] = f'{b.bnumber_} {p.GM_parameter.name}'
                             plot_GM_Estimator(p.GM_parameter,
-                                            saveloc=self.saveplace,
-                                            fmt=self.save_plots_fmt,
-                                            sig_factor=self.plot_gaussian_mixtures['sig_factor'],
-                                            fill_cor=b.bnumber_-1,
-                                            plot_name='{} '.format(b.bnumber_) + p.GM_parameter.name,
-                                            plot_title=self.plot_gaussian_mixtures['plot_title'],
-                                            plot_ylabel=self.plot_gaussian_mixtures['plot_ylabel'])
+                                            options=self.plot_gaussian_mixtures)
                 pbar.close()
 
         # PLOT Keplerian Model and uncertainties
         if self.kplanets__ > 0:
             if self.plot_keplerian_model['plot']:
                 res_max = flatten(self.get_attr_param('value_max'))
                 self.logger('Plotting Keplerian Models', center=True, c='green')
                 if True:
                     plot_KeplerianModel(self.my_data, self.model,
-                                        res_max, saveloc=self.saveplace,
+                                        res_max,
                                         options = self.plot_keplerian_model)
                 else:
                     print('Model plot failed miserably :(\n')
 
         # PLOT stuff with arviz, including corner!!
 
         if self.plot_trace['plot']:
@@ -1126,14 +1160,17 @@
                                 self.model, saveloc=self.saveplace,
                                 trace_modes=self.plot_trace['modes'], fmt='png')
 
         # SAVE LOG
         if self.save_log:
             self.logger.saveto(self.saveplace)
 
+        # CLEAN A BIT
+        os.system(f'mv {self.temp_script} {self.saveplace}/temp/{self.temp_script}')
+
 
     def get_attr_param(self, call, flat=False, asarray=False):
         ret = [b.get_attr(call) for b in self]
         if flat:
             ret = flatten(ret)
         if asarray:
             ret = np.array(ret)
@@ -1149,32 +1186,32 @@
         return ret
 
 
     def save_chain(self, chains):
         temps = self.save_chains
         if self.engine__.__name__ == 'reddemcee':
             for temp in temps:
-                np.savez_compressed(f'{self.saveplace}/chains/chain_{str(temp)}', chains[temp])
+                np.savez_compressed(f'{self.saveplace}/samples/chains/chain_{str(temp)}', chains[temp])
 
 
     def save_posterior(self, posts):
         temps = self.save_posteriors
         if self.engine__.__name__ == 'reddemcee':
             for temp in temps:
                 np.savez_compressed(
-                    f'{self.saveplace}/posteriors/posterior_{str(temp)}',
+                    f'{self.saveplace}/samples/posteriors/posterior_{str(temp)}',
                     posts[temp],
                 )
 
 
     def save_loglikelihood(self, likes):
         temps = self.save_likelihoods
         if self.engine__.__name__ == 'reddemcee':
             for temp in temps:
-                np.savez_compressed(self.saveplace + '/likelihoods/likelihood_'+str(temp), likes[temp])
+                np.savez_compressed(self.saveplace + '/samples/likelihoods/likelihood_'+str(temp), likes[temp])
 
 
     def apply_conditions(self):
         applied = []
         for b in self:
             for p in b:
                 for c in self.conds:
@@ -1200,54 +1237,73 @@
             self.conds.remove(ap)
 
 
     def add_condition(self, cond):
         self.conds.append(cond)
 
 
-    def write_model(self):
-
+    def write_script(self):
+        if self.debug_mode:
+            print(f'write_script() : INIT | {time.time()-self.debug_timer}')
         self.dir_work = os.path.dirname(os.path.realpath(__file__))
         self.dir_save = self.saveplace
 
         self.script_pool_opt = get_support(f'pools/0{self.multiprocess_method}.pool')
 
         if self.engine__.__name__ == 'reddemcee':
-
-
             ntemps, nwalkers, nsteps = self.auto_setup
             #self.my_data.to_csv('{}/temp/temp_data.csv'.format(self.saveplace))
+            if self.debug_mode:
+                print(f'write_script() : open(temp_script.py, w) | {time.time()-self.debug_timer}')
+            
             with open(self.temp_script, 'w') as f:
                 f.write(open(get_support('init.scr')).read())
-
+                if self.debug_mode:
+                    #marker = self.set_marker('begin writing script', ret=self.debug_mode)                
+                    f.write(f'''
+print('temp_script.py   : INIT | {time.time()-self.debug_timer}')
+''')
                 # DEPENDENCIES
                 for d in self.general_dependencies:
-                    f.write('''
-import {}
-'''.format(d))
-
+                    f.write(f'''
+import {d}
+''')
+                # MODEL DEPENDENCIES
                 f.write('''
 import kepler
 ''')
-                # CONSTANTS
                 f.write('''
+logging.getLogger('emcee').setLevel('{}')
+'''.format(self.reddemcee_config['logger_level']))
+                # CONSTANTS
+                f.write(f'''
 nan = np.nan
-A_ = {}
-mod_fixed_ = {}
+A_ = {self.model.A_}
+mod_fixed_ = {self.model.mod_fixed}
 gaussian_mixture_objects = dict()
 
-'''.format(self.model.A_, self.model.mod_fixed))
+''')
 
                 # MODEL
                 f.write(open(self.model.write_model_(loc=self.saveplace)).read())
+                if self.debug_mode:
+                    #marker = self.set_marker('end writing model', ret=self.debug_mode)
+                    f.write(f'''
+print('temp_script.py   : model.write_model_() | {time.time()-self.debug_timer}')
+''')
 
                 # LIKELIHOOD
                 f.write(open(get_support('likelihoods/00.like')).read())
 
                 # PRIOR
+                if self.debug_mode:
+                    #marker = self.set_marker('begin writing prior', ret=self.debug_mode)
+                    f.write(f'''
+print('temp_script.py   : prior_script.read() | {time.time()-self.debug_timer}')
+''')
                 for prior_script in os.listdir(get_support('priors')):
                     f.write(open(get_support(f'priors/{prior_script}')).read())
                     f.write('''
 ''')
                 count = 0
                 for b in self:
                     for p in b[b.C_]:
@@ -1344,14 +1400,16 @@
 
     return lp
 
 
 ''')
 
                 # MULTIPROCESSING
+                if self.debug_mode:
+                    print(f'write_script() : import multiprocessing pool | {time.time()-self.debug_timer}')
                 f.write(open(self.script_pool_opt).read())
 
                 # SETUP CONSTS
                 f.write('''
 
 ntemps, nwalkers, nsteps = {0}, {1}, {2}
 setup = ntemps, nwalkers, nsteps
@@ -1367,16 +1425,22 @@
     backends[t].reset(nwalkers, ndim)
 
 sampler = reddemcee.PTSampler(nwalkers, ndim,
                              my_likelihood,
                              my_prior,
                              ntemps=ntemps, pool=mypool,
                              backend=backends)
-'''.format(self.saveplace+'/temp/'))
+'''.format(self.saveplace+'/restore/backends/'))
 
+                pos0_bool = 'False'
+                if self.debug_mode:
+                    pos0_bool = 'True'
+                    f.write(f'''
+print('temp_script.py   : set_init()  pos0 | {time.time()-self.debug_timer}')
+''')
                 # POS 0
                 f.write('''
 def set_init():
     pos = np.zeros((ntemps, nwalkers, ndim))
 
     for t in range(ntemps):
         j = 0
@@ -1394,46 +1458,60 @@
         dist = np.sort(np.random.uniform(0, 1, nwalkers))
         pos[t][:, j] = r * (2 * dist - 1) + m
         np.random.shuffle(pos[t, :, j])
         j += 1
 
 '''.format(p.limits[1], p.limits[0], r))
 
-
                 f.write('''
     return list(pos)
 
 
 ''')
 
                 f.write('''
 def test_init(max_repeats={0}):
     p0 = set_init()
 
     is_bad_position = True
     repeat_number = 0
 
-    while is_bad_position and repeat_number < max_repeats:
+    while is_bad_position and (repeat_number < max_repeats):
         is_bad_position = False
         for t in range(ntemps):
             for n in range(nwalkers):
                 position_evaluated = p0[t][n]
                 if my_prior(position_evaluated) == -np.inf:
                     is_bad_position = True
                     p0[t][n] = set_init()[t][n]
         repeat_number += 1
+        if {1}:
+            print('test_init ', repeat_number)
+
+    if is_bad_position:
+        print('COULDNT FIND VALID INITIAL POSITION')
     return p0
 
-'''.format(100))
-            # RUN
+'''.format(100, pos0_bool))
+
+                if self.debug_mode:
+                    f.write(f'''
+print('temp_script.py   : test_init()  pos0 | {time.time()-self.debug_timer}')
+''')
                 f.write('''
 
 p1 = test_init()
 
 ''')
+
+                # RUN
+                if self.debug_mode:
+                    f.write(f'''
+print('temp_script.py   : run __main__ | {time.time()-self.debug_timer}')
+''')
                 f.write(open(get_support('endit.scr')).read())
 
         if self.engine__.__name__ == 'dynesty':
             if self.engine__args == 'dynamic':
                 nlive, nlive_batch = self.auto_setup
                 with open(self.temp_script, 'w') as f:
                     f.write(open(get_support('init.scr')).read())
@@ -1494,14 +1572,42 @@
                     nested_dict = self.dynesty_config
                     nested_args = ''
                     for key in [*nested_dict]:
                         nested_args += f'{key} = {nested_dict[key]}, '
 
                     f.write(open(get_support('endit_dyn.scr')).read().format(pool_bool, self.cores__, nested_args))
 
+        # load just the model into emperor
+        if self.debug_mode:
+            print('write_script() : imports & reloads | {time.time()-self.debug_timer}')
+
+        try:
+            temp_script = reload(temp_script)    
+        except:
+            import temp_script
+        
+        self.temp_model_func = temp_script.my_model
+        self.temp_like_func = temp_script.my_likelihood
+        self.temp_prior_func = temp_script.my_prior
+
+        if self.debug_mode:
+            print('write_script() : END | {time.time()-self.debug_timer}')
+
+
+    def set_marker(self, marker: str, ret: bool=False):
+        if self.debug_mode:
+            marker = f'%% {marker}'
+            print(marker)
+        if ret:
+            return marker
+        return ''
+
+
+    def load_run(self):
+        
         pass
 
 
     def __getitem__(self, n):
         return self.blocks__[n]
 
 
@@ -1509,13 +1615,8 @@
         #return self.model
         return str([self.blocks__[i].name_ for i in range(len(self.blocks__))])
 
 
     def __len__(self):
         return np.sum([len(b) for b in self])
 
-
-
-
-
-
 #
```

### Comparing `astroemperor-0.7.7/src/astroemperor/block.py` & `astroemperor-0.8.0/src/astroemperor/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-
-# version 0.3
-# date 14 nov 2022
+# version 0.8
+# date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
+
 import numpy as np
 from .utils import flatten, cps, GM_Estimator, get_support
 
 class Parameter(object):
     def __init__(self, attributes_dict: dict):
         '''
         value, prior, limits, type, name, prargs, ptformargs,
@@ -463,14 +463,8 @@
     def GaussianMixture(x, limits, args):
         #  = my_bgm.bgm_estimator[0]
         if limits[0] <= x <= limits[1]:
             return 0
         else:
             return -np.inf
 
-
-
-
-
-
-
-#
+#
```

### Comparing `astroemperor-0.7.7/src/astroemperor/block_repo.py` & `astroemperor-0.8.0/src/astroemperor/block_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.3
-# date 14 nov 2022
+# version 0.8
+# date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -361,37 +361,39 @@
 
             '''
             b.add_additional_priors([['Eccentricity', norm, ecc_limits, ecc_prargs],
                                    ['Longitude', uni, [0, 2*np.pi], []],
                                    ])
             '''
         if d['starmass']:
-            _extracted_from_SmartLimits_122(b, uni)
-        if not d['dynamics_already_included'] and d['kplan'] > 1:
-            d0 = {'name': 'Hill',
-                  'display_name': 'Dynamical Criteria',
-                  'prior': 'Hill',
-                  'limits':[None, None],
-                  'prargs':[d['kplan'], d['starmass']],
-                  'has_prior':True,
-                  'has_posterior':False,
-                  'unit':None,
-                  'fixed':None,
-                  }
-            d['dynamics_already_included'] = True
-            b.add_additional_parameters(d0)
+            sma_minmass_add_additional(b, uni)
+        
+            if d['dynamics']:
+                if not d['dynamics_already_included'] and d['kplan'] > 1:
+                    d0 = {'name': 'Hill',
+                        'display_name': 'Dynamical Criteria',
+                        'prior': 'Hill',
+                        'limits':[None, None],
+                        'prargs':[d['kplan'], d['starmass']],
+                        'has_prior':True,
+                        'has_posterior':False,
+                        'unit':None,
+                        'fixed':None,
+                        }
+                    d['dynamics_already_included'] = True
+                    b.add_additional_parameters(d0)
         '''
             if d['dynamics']:
                 if d['kplan'] > 1 and b.number_ == d['kplan']:
                     prarg = [d['kplan'], d['starmass']]
                     b.add_additional_priors([['Hill', 'Hill', [None, None], prarg]])
                     b.dynamics_bool = True
                 else:
                     b.dynamics_bool = False
-            '''
+        '''
 
     elif b.type_ == 'Instrumental':
         jit_limits, jit_prargs = args
 
         mask = my_data['Flag']==b.number_
         jit_limiter = my_data[mask]['RV'].abs().max()
 
@@ -459,15 +461,15 @@
 
     b.set_attr('limits', lims, silent=True)
     b.set_attr('prior', priors, silent=True)
     b.set_attr('prargs', prargs, silent=True)
 
 
 # TODO Rename this here and in `SmartLimits`
-def _extracted_from_SmartLimits_122(b, uni):
+def sma_minmass_add_additional(b, uni):
     pnames = ['Semi-Major Axis', 'Minimum Mass']
     pdisplay_names = [f'{x} {b.number_}' for x in pnames]
     ppriors = [uni, uni]
     plims = [[1e-5, 1000], [1e-5, 1000]]
     pprargs = [[], []]
     phas_prior = [False, False]
     phas_posterior = [True, True]
@@ -521,8 +523,8 @@
 # ~𝓤()
 # ~𝓝()
 # ~𝓖()
 # ~ 𝓙()
 
 # ✅ ✔ ✓
 # ◯
-# ❎ ❌ ✘ ✗ ☒
+# ❎ ❌ ✘ ✗ ☒
```

### Comparing `astroemperor-0.7.7/src/astroemperor/canvas.py` & `astroemperor-0.8.0/src/astroemperor/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # type: ignore
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.3.0
-# date 29 nov 2022
+# version 0.8
+# date 11 apr 2023
 # sourcery skip
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
```

### Comparing `astroemperor-0.7.7/src/astroemperor/model_repo.py` & `astroemperor-0.8.0/src/astroemperor/model_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.3
-# date 14 nov 2022
+# version 0.8
+# date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
```

### Comparing `astroemperor-0.7.7/src/astroemperor/support/endit.scr` & `astroemperor-0.8.0/src/astroemperor/support/endit.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/support/endit_dyn.scr` & `astroemperor-0.8.0/src/astroemperor/support/endit_dyn.scr`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/support/models/ins01.model` & `astroemperor-0.8.0/src/astroemperor/support/models/ins01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/support/models/kep01.model` & `astroemperor-0.8.0/src/astroemperor/support/models/kep01.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/support/models/kep03.model` & `astroemperor-0.8.0/src/astroemperor/support/models/kep03.model`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/support/priors/Hill.prior` & `astroemperor-0.8.0/src/astroemperor/support/priors/Hill.prior`

 * *Files identical despite different names*

### Comparing `astroemperor-0.7.7/src/astroemperor/unmodel_repo.py` & `astroemperor-0.8.0/src/astroemperor/unmodel_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.3
-# date 14 nov 2022
+# version 0.8
+# date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
```

### Comparing `astroemperor-0.7.7/src/astroemperor/utils.py` & `astroemperor-0.8.0/src/astroemperor/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/ /^\s*class/
+# @auto-fold regex /^\s*if/ /^\s*else/ /^\s*def/
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# version 0.3
-# date 14 nov 2022
+# version 0.8
+# date 11 apr 2023
 
 # my coding convention
 # **EVAL : evaluate the performance of this method
 # **RED  : redo this
 # **DEB  : debugging needed in this part
 # **DEL  : DELETE AT SOME POINT
 # **FIN  : Finish this
@@ -23,14 +23,81 @@
 
 _ROOT = os.path.dirname(__file__)
 
 def get_support(path):
     return os.path.join(_ROOT, 'support', path)
 
 
+from functools import singledispatch
+import shutil
+
+class nuker(object):
+    def __init__(self, loc=''):
+        self._loc = loc
+        self._target_folder = ''
+        self._dr = ''
+        self.IamSure = False
+        self._nuclear = False
+
+    @property
+    def dr(self):
+        return self._dr
+
+    @dr.setter
+    def dr(self, val):
+        self._dr = val
+
+    @property
+    def loc(self):
+        return self._loc
+    
+    @loc.setter
+    def loc(self, val: str):
+        self._loc = val
+
+    
+    def aim(self, target):
+        if type(target) == str:
+            self._target_folder = target
+            self._dr = f'{self._loc}datalogs/{self._target_folder}/'
+            self._target_list = os.listdir(self._dr)
+
+        if type(target) == tuple:
+            holder = []
+            tmin, tmax = target[0], target[1] + 1
+            for i in range(tmin, tmax):
+                run_name = f'run_{i}'
+                if run_name in self._target_list:
+                    holder.append(run_name)
+            self._target_list = holder
+
+        if type(target) == bool and target:
+            self._dr = f'{self._loc}datalogs/'
+            self._nuclear = True
+            self._target_list = os.listdir(self._dr)
+
+        for x in self._target_list:
+            if x[0] == '.':
+                self._target_list.remove(x)
+                
+
+    def nuke(self):
+        if not self.IamSure:
+            print('You are about to delete the following directories:\n')
+            for tg in self._target_list:
+                print(f'    - {self._dr}{tg}\n')
+            print('if you are really sure, set nuker.IamSure = True')
+        else:
+            if type(self._target_list) == str:
+                shutil.rmtree(self._dr)
+            if type(self._target_list) == list:
+                for tg in self._target_list:
+                    shutil.rmtree(f'{self._dr}{tg}')
+
+
 def fold(x, y, yerr=None, per=None):
     if per is None:
         per = 2. * np.pi
     x_f = x % per
     order = np.argsort(x_f)
     if yerr is None:
         return x_f[order], y[order]
@@ -195,24 +262,31 @@
 def ensure_dir(name, loc=''):
     dr = f'{loc}datalogs/{name}/run_1'
     while os.path.exists(dr):
         aux = int(dr.split('_')[-1]) + 1
         dr = dr.split('_')[0] + '_' + str(aux)
 
     os.makedirs(dr)
-    os.makedirs(f'{dr}/histograms')
-    os.makedirs(f'{dr}/posteriors')
-    os.makedirs(f'{dr}/posteriors/GMEstimates')
-    os.makedirs(f'{dr}/likelihoods')
-    os.makedirs(f'{dr}/chains')
-    os.makedirs(f'{dr}/traces')
-    os.makedirs(f'{dr}/models')
-    os.makedirs(f'{dr}/models/uncertainpy')
-    os.makedirs(f'{dr}/models/temp')
+    os.makedirs(f'{dr}/plots')
+    os.makedirs(f'{dr}/plots/histograms')
+    os.makedirs(f'{dr}/plots/GMEstimates')
+    os.makedirs(f'{dr}/plots/traces')
+    os.makedirs(f'{dr}/plots/models')
+    os.makedirs(f'{dr}/plots/models/uncertainpy')
+
+    os.makedirs(f'{dr}/samples')
+    os.makedirs(f'{dr}/samples/posteriors')
+    os.makedirs(f'{dr}/samples/likelihoods')
+    os.makedirs(f'{dr}/samples/chains')
+
     os.makedirs(f'{dr}/temp')
+    os.makedirs(f'{dr}/temp/models')
+
+    os.makedirs(f'{dr}/restore')
+    os.makedirs(f'{dr}/restore/backends')
 
     return dr
 
 
 def set_pos0(setup, model_obj):
     ntemps, nwalkers, nsteps = setup
     ndim = model_obj.ndim__
@@ -299,29 +373,34 @@
 class reddlog(object):
     def __init__(self):
         self.log = ''
         try:
             self.terminal_width = os.get_terminal_size().columns
         except:
             self.terminal_width = pd.get_option('display.width')
+        self.baddies_list = ["\x1b[", '0m', '1m', '4m', '7m', '31m', '32m']
 
     def saveto(self, location):
         np.savetxt(f'{location}/log.dat', np.array([self.log]), fmt='%100s')
 
     def help(self):
         print('Colors: grey, red, green, yellow, blue, magenta, cyan, white')
         print('On_Colors: on_<color>')
         print('Attrs: bold, dark, underline, blink, reverse, concealed')
 
 
     def __call__(self, msg, center=False, save=True, c=None, oc=None, attrs=None):
         if attrs is None:
             attrs = []
         if save:
-            self.log += msg
+            msg0 = msg
+            for b in self.baddies_list:
+                msg0 = msg0.replace(b, '')
+
+            self.log += msg0
         if center:
             msg = msg.center(self.terminal_width)
         if c:
             msg = colored(msg, c, oc, attrs)
         print(msg)
 
 '''
@@ -495,10 +574,8 @@
         self.fargs = fargs
         self.fkwargs = fkwargs
 
     def __call__(self, x):
         return self.func(x, *self.fargs, **self.fkwargs)
 
 
-
-
-#
+#
```

### Comparing `astroemperor-0.7.7/src/astroemperor.egg-info/PKG-INFO` & `astroemperor-0.8.0/src/astroemperor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroemperor
-Version: 0.7.7
+Version: 0.8.0
 Summary: PTMCMC sampler for exoplanet search
 Author: ReddTea
 Author-email: redd@tea.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `astroemperor-0.7.7/src/astroemperor.egg-info/SOURCES.txt` & `astroemperor-0.8.0/src/astroemperor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

