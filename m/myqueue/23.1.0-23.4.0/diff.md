# Comparing `tmp/myqueue-23.1.0.tar.gz` & `tmp/myqueue-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myqueue-23.1.0.tar", last modified: Tue Jan 10 11:07:36 2023, max compression
+gzip compressed data, was "myqueue-23.4.0.tar", last modified: Tue Apr 11 11:24:42 2023, max compression
```

## Comparing `myqueue-23.1.0.tar` & `myqueue-23.4.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-01-10 11:07:36.702991 myqueue-23.1.0/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2022-12-20 13:04:51.000000 myqueue-23.1.0/LICENSE
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       27 2022-12-20 13:04:51.000000 myqueue-23.1.0/MANIFEST.in
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4942 2023-01-10 11:07:36.702991 myqueue-23.1.0/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4128 2022-12-20 13:04:51.000000 myqueue-23.1.0/README.rst
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-01-10 11:07:36.698991 myqueue-23.1.0/myqueue/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      816 2023-01-10 11:03:53.000000 myqueue-23.1.0/myqueue/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/__main__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4428 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/caching.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    22924 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/cli.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7603 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/commands.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4535 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/complete.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6766 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/config.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4419 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/daemon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4148 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/email.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1281 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/errors.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1425 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/hold.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4191 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/info.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1856 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/kick.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2022-12-22 08:23:20.000000 myqueue-23.1.0/myqueue/migration.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1514 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/modify.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4118 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/pretty.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/py.typed
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13432 2023-01-10 10:49:51.000000 myqueue-23.1.0/myqueue/queue.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1089 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/remove.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8095 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/resources.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      976 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/resubmit.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-01-10 11:07:36.702991 myqueue-23.1.0/myqueue/schedulers/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      963 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8033 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/local.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4152 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/lsf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2975 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/pbs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1975 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/scheduler.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4417 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/slurm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3959 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/schedulers/test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2163 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/selection.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2940 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/states.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3922 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/submitting.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      756 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/syncronize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13876 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/task.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-01-10 11:07:36.702991 myqueue-23.1.0/myqueue/test/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      440 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1430 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/caching_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      285 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/command_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1253 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/complete_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      523 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/config_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1858 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/conftest.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      803 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/daemon_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      650 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/flow1.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      421 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/flow2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      787 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/hello.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2250 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/local_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      309 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/lock_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      215 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/mod.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2810 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/more_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5409 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/mq_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      740 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/name_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      953 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/notify_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      271 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/pp_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      305 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/queue_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/resources_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4215 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/rst_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2196 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/scheduler_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      459 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/sqlite_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/task_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      455 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/utils_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5070 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/test/workflow_test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9194 2023-01-10 10:44:29.000000 myqueue-23.1.0/myqueue/utils.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18585 2022-12-20 13:04:51.000000 myqueue-23.1.0/myqueue/workflow.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-01-10 11:07:36.698991 myqueue-23.1.0/myqueue.egg-info/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4942 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1630 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/SOURCES.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/dependency_links.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       41 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/entry_points.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       32 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/requires.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        8 2023-01-10 11:07:36.000000 myqueue-23.1.0/myqueue.egg-info/top_level.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2023-01-10 11:07:36.702991 myqueue-23.1.0/setup.cfg
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1318 2022-12-22 08:23:20.000000 myqueue-23.1.0/setup.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-04-11 11:24:42.338869 myqueue-23.4.0/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2022-12-20 13:04:51.000000 myqueue-23.4.0/LICENSE
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       27 2022-12-20 13:04:51.000000 myqueue-23.4.0/MANIFEST.in
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4942 2023-04-11 11:24:42.338869 myqueue-23.4.0/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4128 2022-12-20 13:04:51.000000 myqueue-23.4.0/README.rst
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-04-11 11:24:42.338869 myqueue-23.4.0/myqueue/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      816 2023-04-11 11:21:55.000000 myqueue-23.4.0/myqueue/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/__main__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4428 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/caching.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23070 2023-03-16 13:26:30.000000 myqueue-23.4.0/myqueue/cli.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7603 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/commands.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4473 2023-03-16 14:51:06.000000 myqueue-23.4.0/myqueue/complete.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6766 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/config.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4419 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/daemon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4148 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/email.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1281 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/errors.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1425 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/hold.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4191 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/info.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1856 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/kick.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2022-12-22 08:23:20.000000 myqueue-23.4.0/myqueue/migration.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1514 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/modify.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4118 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/pretty.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/py.typed
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13614 2023-04-11 11:24:07.000000 myqueue-23.4.0/myqueue/queue.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1089 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/remove.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8156 2023-03-16 13:26:30.000000 myqueue-23.4.0/myqueue/resources.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      976 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/resubmit.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-04-11 11:24:42.338869 myqueue-23.4.0/myqueue/schedulers/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      963 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8033 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/local.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4152 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/lsf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2975 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/pbs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1975 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/scheduler.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4417 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/slurm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3959 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/schedulers/test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2190 2023-01-31 14:03:45.000000 myqueue-23.4.0/myqueue/selection.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2940 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/states.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3922 2023-04-11 10:24:33.000000 myqueue-23.4.0/myqueue/submitting.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      756 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/syncronize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13876 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/task.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-04-11 11:24:42.338869 myqueue-23.4.0/myqueue/test/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      440 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1430 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/caching_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      285 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/command_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1358 2023-01-31 14:03:45.000000 myqueue-23.4.0/myqueue/test/complete_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      523 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/config_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1858 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/conftest.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      803 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/daemon_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      650 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/flow1.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      421 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/flow2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      787 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/hello.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2250 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/local_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      309 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/lock_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      215 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/mod.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2810 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/more_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5409 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/mq_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      740 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/name_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      953 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/notify_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      271 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/pp_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      305 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/queue_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/resources_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4215 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/rst_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2196 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/scheduler_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      459 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/sqlite_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/task_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      455 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/test/utils_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5606 2023-04-11 11:24:07.000000 myqueue-23.4.0/myqueue/test/workflow_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9194 2023-01-31 14:03:45.000000 myqueue-23.4.0/myqueue/utils.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18585 2022-12-20 13:04:51.000000 myqueue-23.4.0/myqueue/workflow.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-04-11 11:24:42.338869 myqueue-23.4.0/myqueue.egg-info/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4942 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1630 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       41 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/entry_points.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       32 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/requires.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        8 2023-04-11 11:24:42.000000 myqueue-23.4.0/myqueue.egg-info/top_level.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2023-04-11 11:24:42.338869 myqueue-23.4.0/setup.cfg
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1318 2022-12-22 08:23:20.000000 myqueue-23.4.0/setup.py
```

### Comparing `myqueue-23.1.0/LICENSE` & `myqueue-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/PKG-INFO` & `myqueue-23.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqueue
-Version: 23.1.0
+Version: 23.4.0
 Summary: Simple job queue
 Home-page: https://myqueue.readthedocs.io/
 Author: J. J. Mortensen
 Author-email: jjmo@dtu.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `myqueue-23.1.0/README.rst` & `myqueue-23.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/__init__.py` & `myqueue-23.4.0/myqueue/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from myqueue.task import Task
 
 
-__version__ = '23.1.0'
+__version__ = '23.4.0'
 
 
 def submit(*tasks: Task, verbosity: int = 1, dry_run: bool = False) -> None:
     """Submit tasks.
 
     Parameters
     ----------
```

### Comparing `myqueue-23.1.0/myqueue/caching.py` & `myqueue-23.4.0/myqueue/caching.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/cli.py` & `myqueue-23.4.0/myqueue/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 import argparse
 import os
 import sys
 import textwrap
 from pathlib import Path
 from time import time
+from typing import Any
 
 
 class MQError(Exception):
     """For nice (expected) CLI errors."""
 
 
 def error(*args: str) -> None:
@@ -168,15 +169,15 @@
         p = subparsers.add_parser(cmd,
                                   description=description,
                                   help=help,
                                   formatter_class=Formatter,
                                   aliases=[alias for alias in aliases
                                            if aliases[alias] == cmd])
 
-        def a(*args, **kwargs):  # type: ignore
+        def a(*args: str, **kwargs: Any) -> None:
             """Wrapper for Parser.add_argument().
 
             Hack to fix argparse's handling of options.  See
             fix_option_order() function below."""
 
             x = p.add_argument(*args, **kwargs)
             if x is None:
@@ -243,15 +244,17 @@
               '"h" for hours and "d" for days. '
               '"16:1:30m": 16 cores, 1 process, half an hour. '
               '"1:xeon40:5m":  1 core on "xeon40" for 5 minutes.')
             a('-w', '--workflow', action='store_true',
               help='Write <task-name>.state file when task has finished.')
             a('-X', '--extra-scheduler-args', action='append', default=[],
               help='Extra arguments for scheudler.  Example: '
-              '-X "--gres=gpu:4".  Can be used multiple times.')
+              '-X bla-bla.  For arguments that start with a dash, '
+              'leave out the space: -X--gres=gpu:4 or -X=--gres=gpu:4. '
+              'Can be used multiple times.')
 
         if cmd == 'modify':
             a('-E', '--email', default='u', metavar='STATES',
               help='Send email when state changes to one of the specified '
               'states (one or more of the letters: rdFCTMA).')
             a('-N', '--new-state', default='u',
               help='New state (one of the letters: qhrdFCTM).')
```

### Comparing `myqueue-23.1.0/myqueue/commands.py` & `myqueue-23.4.0/myqueue/commands.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/complete.py` & `myqueue-23.4.0/myqueue/complete.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
     complete -o default -C "python3 -m myqueue.complete" mq
 
 """
 
 from __future__ import annotations
 import os
 import sys
-from typing import Any, Iterable, Mapping
+from typing import Iterable, Mapping, TYPE_CHECKING
+if TYPE_CHECKING:
+    from myqueue.task import Task
 
 
-def read() -> dict[str, Any]:
+def read() -> list[Task]:
     """Read queue as a dict."""
     from pathlib import Path
-    import json
-    from myqueue.config import find_home_folder
-    home = find_home_folder(Path('.').resolve())
-    path = home / '.myqueue/queue.json'
-    try:
-        dct: dict[str, Any] = json.loads(path.read_text())
-        return dct
-    except Exception:
-        return {}
+    from myqueue.config import Configuration
+    from myqueue.queue import Queue
+    from myqueue.selection import Selection
+
+    config = Configuration.read()
+    with Queue(config, need_lock=False) as queue:
+        return queue.select(Selection(folders=[Path('.').resolve()]))
 
 
 # Beginning of computer generated data:
 commands = {
     'completion':
         ['-v', '--verbose', '-q', '--quiet', '-T', '--traceback'],
     'config':
@@ -100,24 +100,21 @@
             return opts
         return list(commands) + list(aliases) + opts
 
     if word[:1] == '-':
         return commands[command]
 
     if previous in ['-n', '--name']:
-        dct = read()
-        words = set()
-        for task in dct['tasks']:
-            cmd = task['cmd']
-            words.add((cmd['cmd'] + '+' + '_'.join(cmd['args'])).rstrip('+'))
+        tasks = read()
+        words = [task.cmd.name for task in tasks]
         return words
 
     if previous in ['-i', '--id']:
-        dct = read()
-        return {str(task['id']) for task in dct['tasks']}
+        tasks = read()
+        return {str(task.id) for task in tasks}
 
     if command == 'help':
         return [cmd for cmd in (list(commands) + list(aliases))
                 if cmd != 'help']
 
     if command == 'daemon':
         return ['start', 'stop', 'status']
```

### Comparing `myqueue-23.1.0/myqueue/config.py` & `myqueue-23.4.0/myqueue/config.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/daemon.py` & `myqueue-23.4.0/myqueue/daemon.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/email.py` & `myqueue-23.4.0/myqueue/email.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/errors.py` & `myqueue-23.4.0/myqueue/errors.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/hold.py` & `myqueue-23.4.0/myqueue/hold.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/info.py` & `myqueue-23.4.0/myqueue/info.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/kick.py` & `myqueue-23.4.0/myqueue/kick.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/migration.py` & `myqueue-23.4.0/myqueue/migration.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/modify.py` & `myqueue-23.4.0/myqueue/modify.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/pretty.py` & `myqueue-23.4.0/myqueue/pretty.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/queue.py` & `myqueue-23.4.0/myqueue/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from __future__ import annotations
 
 import sqlite3
 import sys
 import time
 from pathlib import Path
 from types import TracebackType
-from typing import Iterator, Iterable, Sequence
-from typing_extensions import LiteralString
+from typing import Iterable, Iterator, Sequence
 
 from myqueue.config import Configuration
+from myqueue.migration import migrate
 from myqueue.schedulers import Scheduler, get_scheduler
+from myqueue.selection import Selection
 from myqueue.states import State
 from myqueue.task import Task, create_task
-from myqueue.utils import Lock, cached_property, normalize_folder
-from myqueue.selection import Selection
-from myqueue.migration import migrate
+from myqueue.utils import Lock, cached_property, normalize_folder, plural
+from typing_extensions import LiteralString
 
 VERSION = 11
 
 INIT = """\
 CREATE TABLE tasks (
     id INTEGER PRIMARY KEY,
     folder TEXT,
@@ -331,14 +331,15 @@
 
     name_to_id_and_state: dict[str, tuple[int, str]] = {}
 
     if done is not None:
         for task in done:
             name_to_id_and_state[str(task.dname.relative_to(root))] = (0, 'd')
 
+    skipped = 0
     for task in tasks:
         task.dtasks = []
         deps = []
         for dname in task.deps:
             name = str(dname.relative_to(root))
             dtask = name_to_task.get(name)
             if dtask is None:
@@ -356,25 +357,31 @@
                 if state in 'qhr':
                     dtask = create_task('dummy')
                     dtask.id = id
                     dtask.state = State(state)
                 elif state == 'd':
                     continue
                 else:
-                    raise DependencyError(f'Bad state ({state}): {name}')
+                    task.state = State.CANCELED
+                    skipped += 1
+                    continue
 
             task.dtasks.append(dtask)
             deps.append(dname)
         task.deps = deps
 
+    if skipped:
+        print(f'Skipping {plural(skipped, "task")} '
+              'because of dependency in bad state')
+
 
 def dump_db(path: Path) -> None:
     """Pretty-print content of sqlite3 db file."""
-    from rich.table import Table
     from rich.console import Console
+    from rich.table import Table
     prnt = Console().print
     db = sqlite3.connect(path)
     table = Table(title=str(path))
     columns = [line.strip().split()[0]
                for line in INIT.split(';', maxsplit=1)[0].splitlines()[1:]]
     for name in columns:
         table.add_column(name)
```

### Comparing `myqueue-23.1.0/myqueue/remove.py` & `myqueue-23.4.0/myqueue/remove.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/resources.py` & `myqueue-23.4.0/myqueue/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,19 @@
         if self.weight == -1.0:
             self.weight = weight
 
     @staticmethod
     def from_string(s: str) -> Resources:
         """Create Resource object from string.
 
-        >>> Resources.from_string('16:1:xeon8:2h')
+        >>> r = Resources.from_string('16:1:xeon8:2h')
+        >>> r
         Resources(cores=16, processes=1, tmax=7200, nodename='xeon8')
+        >>> print(r)
+        16:1:xeon8:2h
         >>> Resources.from_string('16:1m')
         Resources(cores=16, tmax=60)
         >>> r = Resources.from_string('16:1m:25')
         >>> r
         Resources(cores=16, tmax=60, weight=25.0)
         >>> print(r)
         16:1m:25
@@ -140,18 +143,18 @@
                     '"cores", "nodename", "processes", "tmax" or "weight". '
                     f'See {url}/documentation.html#resources')
 
         return Resources(cores, nodename, processes, T(tmax or '10m'), weight)
 
     def __str__(self) -> str:
         s = str(self.cores)
-        if self.nodename:
-            s += ':' + self.nodename
         if self.processes != self.cores:
             s += ':' + str(self.processes)
+        if self.nodename:
+            s += ':' + self.nodename
         s += ':' + seconds_to_short_time_string(self.tmax)
         if self.weight > 0.0:
             s += f':{int(self.weight)}'
         return s
 
     def __repr__(self) -> str:
         args = ', '.join(f'{key}={value!r}'
```

### Comparing `myqueue-23.1.0/myqueue/resubmit.py` & `myqueue-23.4.0/myqueue/resubmit.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/__init__.py` & `myqueue-23.4.0/myqueue/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/local.py` & `myqueue-23.4.0/myqueue/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/lsf.py` & `myqueue-23.4.0/myqueue/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/pbs.py` & `myqueue-23.4.0/myqueue/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/scheduler.py` & `myqueue-23.4.0/myqueue/schedulers/scheduler.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/slurm.py` & `myqueue-23.4.0/myqueue/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/schedulers/test.py` & `myqueue-23.4.0/myqueue/schedulers/test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/selection.py` & `myqueue-23.4.0/myqueue/selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Selection:
     """Object used for selecting tasks."""
 
     def __init__(self,
                  ids: set[int] | None = None,
                  name: str | None = None,
-                 states: set[State] = set(),
+                 states: set[State] = None,
                  folders: list[Path] = [],
                  recursive: bool = True,
                  error: str | None = None):
         """Selection.
 
         Selection is based on:
 
@@ -42,15 +42,15 @@
     def sql_where_statement(self, root: Path) -> tuple[str, list]:
         if self.ids is not None:
             q = ', '.join('?' * len(self.ids))
             return (f'id IN ({q})', list(self.ids))
 
         parts = []
         args = []
-        if len(self.states) < 8:
+        if self.states is not None and len(self.states) < 8:
             q = ', '.join('?' * len(self.states))
             parts.append(f'state IN ({q})')
             args += [state.value for state in self.states]
 
         if self.folders:
             part = []
             for folder in self.folders:
```

### Comparing `myqueue-23.1.0/myqueue/states.py` & `myqueue-23.4.0/myqueue/states.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/submitting.py` & `myqueue-23.4.0/myqueue/submitting.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/syncronize.py` & `myqueue-23.4.0/myqueue/syncronize.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/task.py` & `myqueue-23.4.0/myqueue/task.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/caching_test.py` & `myqueue-23.4.0/myqueue/test/caching_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/complete_test.py` & `myqueue-23.4.0/myqueue/test/complete_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-import json
 import os
 
 from myqueue.complete import complete, main
+from myqueue.queue import Queue
+from myqueue.task import create_task
 
 
 def test_ls():
     words = complete('-', 'ls', 'mq ls -', 7)
     assert '--not-recursive' in words
 
 
@@ -43,13 +44,16 @@
     assert words == []
 
 
 def test_read(tmp_path):
     os.chdir(tmp_path)
     mq = tmp_path / '.myqueue'
     mq.mkdir()
-    dct = {'tasks': [{'cmd': {'cmd': 'abc123', 'args': []}, 'id': 117}]}
-    (mq / 'queue.json').write_text(json.dumps(dct))
+    (mq / 'config.py').write_text('config = {"scheduler": "local"}\n')
+    task = create_task('abc123')
+    task.id = 117
+    with Queue() as queue:
+        queue.add(task)
     words = complete('', '-n', 'mq ls -n ', 9)
-    assert words == {'abc123'}
+    assert words == ['abc123']
     words = complete('', '-i', 'mq ls -i ', 9)
     assert words == {'117'}
```

### Comparing `myqueue-23.1.0/myqueue/test/config_test.py` & `myqueue-23.4.0/myqueue/test/config_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/conftest.py` & `myqueue-23.4.0/myqueue/test/conftest.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/daemon_test.py` & `myqueue-23.4.0/myqueue/test/daemon_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/flow1.py` & `myqueue-23.4.0/myqueue/test/flow1.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/hello.py` & `myqueue-23.4.0/myqueue/test/hello.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/local_test.py` & `myqueue-23.4.0/myqueue/test/local_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/more_test.py` & `myqueue-23.4.0/myqueue/test/more_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/mq_test.py` & `myqueue-23.4.0/myqueue/test/mq_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/name_test.py` & `myqueue-23.4.0/myqueue/test/name_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/notify_test.py` & `myqueue-23.4.0/myqueue/test/notify_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/rst_test.py` & `myqueue-23.4.0/myqueue/test/rst_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/scheduler_test.py` & `myqueue-23.4.0/myqueue/test/scheduler_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/task_test.py` & `myqueue-23.4.0/myqueue/test/task_test.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/test/workflow_test.py` & `myqueue-23.4.0/myqueue/test/workflow_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -117,14 +117,34 @@
     mq('workflow wf.py . --force --dry-run')
     assert mq.wait() == 'FC'
 
     mq('workflow wf.py . --force')
     assert mq.wait() == 'Fdd'
 
 
+wf_block = """
+from myqueue.task import task
+def create_tasks():
+    t1 = task('shell:sleep+a')
+    t2 = task('shell:echo+hello', deps=[t1], name='hello')
+    t3 = task('shell:echo+bye')
+    return [t1, t2, t3]
+"""
+
+
+def test_workflow_with_failed_job_blocking(mq):
+    """Failefd dependency (t1) for t2 should not block t3."""
+    Path('wf.py').write_text(wf_block)
+    mq('workflow wf.py . -t hello')  # submit t1 and t2
+    assert mq.wait() == 'FC'
+    mq('rm -sC . --force')
+    mq('workflow wf.py .')
+    assert mq.wait() == 'Fd'
+
+
 wf2 = """
 from myqueue.task import task
 def create_tasks(name, n):
     assert name == 'hello'
     assert n == 5
     return [task('shell:echo+hi', name=f'x{i}', weight=1) for i in range(4)]
 """
```

### Comparing `myqueue-23.1.0/myqueue/utils.py` & `myqueue-23.4.0/myqueue/utils.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue/workflow.py` & `myqueue-23.4.0/myqueue/workflow.py`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/myqueue.egg-info/PKG-INFO` & `myqueue-23.4.0/myqueue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqueue
-Version: 23.1.0
+Version: 23.4.0
 Summary: Simple job queue
 Home-page: https://myqueue.readthedocs.io/
 Author: J. J. Mortensen
 Author-email: jjmo@dtu.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `myqueue-23.1.0/myqueue.egg-info/SOURCES.txt` & `myqueue-23.4.0/myqueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myqueue-23.1.0/setup.py` & `myqueue-23.4.0/setup.py`

 * *Files identical despite different names*

