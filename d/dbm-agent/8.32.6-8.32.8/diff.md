# Comparing `tmp/dbm-agent-8.32.6.tar.gz` & `tmp/dbm-agent-8.32.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.32.6.tar", last modified: Fri Apr  7 11:28:37 2023, max compression
+gzip compressed data, was "dbm-agent-8.32.8.tar", last modified: Tue Apr 11 08:47:11 2023, max compression
```

## Comparing `dbm-agent-8.32.6.tar` & `dbm-agent-8.32.8.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.474272 dbm-agent-8.32.6/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-07 11:28:37.474272 dbm-agent-8.32.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-04-07 08:20:26.000000 dbm-agent-8.32.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.453272 dbm-agent-8.32.6/bin/
--rw-r--r--   0 root         (0) root         (0)      860 2023-03-29 11:53:15.000000 dbm-agent-8.32.6/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.32.6/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      797 2023-03-29 12:36:40.000000 dbm-agent-8.32.6/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2388 2023-04-06 12:03:55.000000 dbm-agent-8.32.6/bin/dbma-cli-single-instance
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.453272 dbm-agent-8.32.6/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-07 11:28:37.000000 dbm-agent-8.32.6/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-07 11:28:37.000000 dbm-agent-8.32.6/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 11:28:37.000000 dbm-agent-8.32.6/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-07 11:28:37.000000 dbm-agent-8.32.6/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-07 11:28:37.000000 dbm-agent-8.32.6/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.454272 dbm-agent-8.32.6/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.32.6/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.456272 dbm-agent-8.32.6/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.32.6/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.32.6/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.456272 dbm-agent-8.32.6/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.32.6/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.460272 dbm-agent-8.32.6/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.32.6/dbma/components/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    20733 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15306 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-04-07 09:37:23.000000 dbm-agent-8.32.6/dbma/components/mysql/replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.461272 dbm-agent-8.32.6/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.32.6/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9574 2023-04-07 11:21:43.000000 dbm-agent-8.32.6/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-04-07 09:24:03.000000 dbm-agent-8.32.6/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.461272 dbm-agent-8.32.6/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.32.6/dbma/components/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.462272 dbm-agent-8.32.6/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.32.6/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.463272 dbm-agent-8.32.6/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.32.6/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-07 07:23:16.000000 dbm-agent-8.32.6/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.464272 dbm-agent-8.32.6/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.465272 dbm-agent-8.32.6/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.32.6/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.451272 dbm-agent-8.32.6/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.473272 dbm-agent-8.32.6/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.32.6/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 09:18:43.000000 dbm-agent-8.32.6/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17894 2023-03-29 03:33:50.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17894 2023-03-30 12:28:43.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.32.6/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 11:28:37.473272 dbm-agent-8.32.6/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.32.6/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-04-07 11:24:03.000000 dbm-agent-8.32.6/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 11:28:37.474272 dbm-agent-8.32.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-30 12:30:28.000000 dbm-agent-8.32.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-04-07 08:20:26.000000 dbm-agent-8.32.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.955536 dbm-agent-8.32.8/bin/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.32.8/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.32.8/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.32.8/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.32.8/bin/dbma-cli-single-instance
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.956536 dbm-agent-8.32.8/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-11 08:47:11.000000 dbm-agent-8.32.8/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.956536 dbm-agent-8.32.8/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.32.8/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.957536 dbm-agent-8.32.8/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.32.8/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.32.8/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.32.8/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.958536 dbm-agent-8.32.8/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.32.8/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.959536 dbm-agent-8.32.8/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.32.8/dbma/components/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.32.8/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    20949 2023-04-11 03:12:09.000000 dbm-agent-8.32.8/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15140 2023-04-11 07:41:26.000000 dbm-agent-8.32.8/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.32.8/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-04-11 08:19:15.000000 dbm-agent-8.32.8/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.960536 dbm-agent-8.32.8/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.32.8/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-04-11 07:58:31.000000 dbm-agent-8.32.8/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2023-04-11 08:12:23.000000 dbm-agent-8.32.8/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.960536 dbm-agent-8.32.8/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.32.8/dbma/components/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.961536 dbm-agent-8.32.8/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.32.8/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.962536 dbm-agent-8.32.8/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.32.8/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-07 07:23:16.000000 dbm-agent-8.32.8/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.963536 dbm-agent-8.32.8/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.965536 dbm-agent-8.32.8/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.32.8/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.954536 dbm-agent-8.32.8/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 09:18:43.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18705 2023-04-11 03:16:31.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18707 2023-04-11 03:16:16.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.32.8/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.32.8/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      346 2023-04-11 08:44:13.000000 dbm-agent-8.32.8/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 08:47:11.970536 dbm-agent-8.32.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-04-11 03:20:04.000000 dbm-agent-8.32.8/setup.py
```

### Comparing `dbm-agent-8.32.6/PKG-INFO` & `dbm-agent-8.32.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.32.6
+Version: 8.32.8
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.32.6/README.md` & `dbm-agent-8.32.8/README.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/bin/dbm-agent` & `dbm-agent-8.32.8/bin/dbm-agent`

 * *Files 22% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 
 import argparse
 from dbma.core.httpserver import start, stop
 from dbma.version import DBM_AGENT_VESION
 
 
 def parser_cmd_args():
-    parser = argparse.ArgumentParser(f'dbma-agent {DBM_AGENT_VESION}')
-    parser.add_argument('action', type=str, default='start', choices=(
-        'start', 'stop', 'version'), help='')
+    parser = argparse.ArgumentParser(f"dbma-agent {DBM_AGENT_VESION}")
+    parser.add_argument(
+        "action",
+        type=str,
+        default="start",
+        choices=("start", "stop", "version"),
+        help="",
+    )
     args = parser.parse_args()
     return args
 
 
 def main():
     args = parser_cmd_args()
-    if args.action == 'start':
+    if args.action == "start":
         start()
-    elif args.action == 'version':
-        print(f'dbma-agent {DBM_AGENT_VESION}')
-    elif args.action == 'stop':
+    elif args.action == "version":
+        print(f"dbma-agent {DBM_AGENT_VESION}")
+    elif args.action == "stop":
         stop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dbm-agent-8.32.6/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.32.8/dbm_agent.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.32.6
+Version: 8.32.8
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dbm-agent-8.32.6/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.32.8/dbm_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 dbma/components/mysql/__init__.py
 dbma/components/mysql/commons.py
 dbma/components/mysql/config.py
 dbma/components/mysql/exceptions.py
 dbma/components/mysql/install.py
 dbma/components/mysql/instance.py
 dbma/components/mysql/replica.py
+dbma/components/mysql/source.py
 dbma/components/mysql/views/__init__.py
 dbma/components/mysql/views/defaultsview.py
 dbma/components/mysql/views/handlers.py
 dbma/components/redis/__init__.py
 dbma/core/__init__.py
 dbma/core/configs.py
 dbma/core/exception.py
```

### Comparing `dbm-agent-8.32.6/dbma/bil/daemon.py` & `dbm-agent-8.32.8/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/bil/fs.py` & `dbm-agent-8.32.8/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/bil/net.py` & `dbm-agent-8.32.8/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/bil/osuser.py` & `dbm-agent-8.32.8/dbma/bil/osuser.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/bil/sudos.py` & `dbm-agent-8.32.8/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/commons.py` & `dbm-agent-8.32.8/dbma/components/mysql/commons.py`

 * *Files 12% similar despite different names*

```diff
@@ -181,7 +181,28 @@
             mysql_lib_dir = pkg_to_basedir(pkg) / "lib/"
             f.write(str(mysql_lib_dir))
             f.write("\n")
 
     exe_shell_cmd("ldconfig")
 
     logging.info(messages.FUN_ENDS.format(fname()))
+
+
+def make_mysql_writable(port: int = 3306):
+    """把结点设置为可写
+    Parameters:
+    -----------
+    port: int
+        MySQL 端口号
+
+    Return
+    ------
+    None
+    """
+    logging.info(messages.FUN_STARTS.format(fname()))
+
+    with dbma_mysql_cnx(port) as cursor:
+        sql = "set @@global.read_only=OFF; set @@global.super_read_only=OFF;"
+        cursor.execute(sql)
+        logging.info("make mysql instance 127.0.0.1:{} writable .".format(port))
+        logging.info("sql = {}".format(cursor.statement))
+    logging.info(messages.FUN_ENDS.format(fname()))
```

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/config.py` & `dbm-agent-8.32.8/dbma/components/mysql/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,19 +156,24 @@
     enforce_gtid_consistency: str = "ON"
     gtid_executed_compression_period: int = 0
     # endregion gtids
 
     # region clone
     plugin_load_add: str = "mysql_clone.so"
     clone_autotune_concurrency: str = "ON"
-    clone_buffer_size: int = 4194304
-    clone_block_ddl: str = "ON"
+    clone_buffer_size: str = "16M"
+    clone_block_ddl: str = "OFF"
+    clone_delay_after_data_drop: int = 300
     clone_ddl_timeout: int = 300
-    clone_enable_compression: str = "OFF"
+    clone_donor_timeout_after_network_failure: int = 5
+    clone_enable_compression: str = "ON"
     clone_max_concurrency: int = 16
+    clone_max_data_bandwidth: int = 0
+    clone_max_network_bandwidth: int = 0
+    clone_valid_donor_list: str = "NULL"
     # endregion clone
 
     # region replication
     rpl_semi_sync_master_enabled: str = "ON"
     rpl_semi_sync_slave_enabled: str = "ON"
     rpl_semi_sync_master_timeout: int = 1000
     rpl_semi_sync_master_wait_point: str = "AFTER_SYNC"
```

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/install.py` & `dbm-agent-8.32.8/dbma/components/mysql/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,18 +413,15 @@
         f.write("dbm-agent")
 
     # 解压完成
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def create_mysql_config_file(
-    port: int = 3306,
-    basedir: Path = None,
-    innodb_buffer_pool_size: str = "128M",
-    read_only=True,
+    port: int = 3306, basedir: Path = None, innodb_buffer_pool_size: str = "128M"
 ):
     """创建 MySQL 配置文件
 
     Parameter:
     ----------
     port: int
         MySQL 端口号、默认值 3306
@@ -446,18 +443,14 @@
         )
     )
 
     config = MySQLConfig(
         basedir=str(basedir), port=port, innodb_buffer_pool_size=innodb_buffer_pool_size
     )
 
-    if read_only == False:
-        config.read_only = "OFF"
-        config.super_read_only = "OFF"
-
     config.calcu_second_attrs()
     config.generate_cnf_config_file()
     config.generate_init_cnf_config_file()
     config.generate_systemd_cnf_config()
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
@@ -490,18 +483,15 @@
     # 执行 init 操作
     exe_shell_cmd(init_cmd)
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def install_mysql(
-    port: int = 3306,
-    pkg: Path = None,
-    innodb_buffer_pool_size: str = "128M",
-    read_only=True,
+    port: int = 3306, pkg: Path = None, innodb_buffer_pool_size: str = "128M"
 ):
     """安装 MySQL 实例
 
     Parameter:
     ----------
     port: int
         MySQL 端口号
@@ -542,20 +532,18 @@
 
     # 第二步 解压安装包
     decompression_pkg(pkg)
 
     # 第三步 计算 basedir
     basedir = pkg_to_basedir(pkg)
 
+    # TODO 清理掉 read_only 参数
     # 第四步 创建配置文件
     create_mysql_config_file(
-        port=port,
-        basedir=basedir,
-        innodb_buffer_pool_size=innodb_buffer_pool_size,
-        read_only=read_only,
+        port=port, basedir=basedir, innodb_buffer_pool_size=innodb_buffer_pool_size
     )
 
     # 第五步 复制 init 文件
     create_init_sql_file(version)
 
     # 第五步 初始化 mysql 实例
     init_mysql(port=port, basedir=basedir)
```

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/instance.py` & `dbm-agent-8.32.8/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/replica.py` & `dbm-agent-8.32.8/dbma/components/mysql/replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     with dbma_mysql_cnx(port) as cursor:
         cursor.execute(stmt)
         logging.info(stmt)
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
-def install_replica(
+def install_mysql_replica(
     port: int = 3306,
     pkg: Path = None,
     innodb_buffer_pool_size: str = "128M",
     source_ip: str = None,
     source_port: int = None,
 ):
     """安装 MySQL Replica 结点
@@ -153,18 +153,18 @@
         Source 实例的端口
     """
     logging.info(messages.FUN_STARTS.format(fname()))
 
     version = get_mysql_version(pkg.name)
 
     # 第一步安装 MySQL Replica 结点
-    install_mysql(port, pkg, innodb_buffer_pool_size, read_only=True)
+    install_mysql(port, pkg, innodb_buffer_pool_size)
 
     # MySQL 安装之后要 sleep 一下，希望这个时候 MySQL 的监听已经完成
-    seconds = 5
+    seconds = 11
     time.sleep(seconds)
 
     # 第二步执行 change-master-to
     change_replica_to(port, version, source_ip=source_ip, source_port=source_port)
 
     # 第三步执行 start-replica
     start_replica(port, version, source_ip=source_ip, source_port=source_port)
```

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.32.8/dbma/components/mysql/views/defaultsview.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from aiohttp import web
 from pathlib import Path
 from dbma.bil.sudos import sudo
 from dbma.core.router import routes
 from dbma.core.configs import dbm_agent_config
 from dbma.core.threads.backends import threads
 from dbma.core.views.response import ResponseEntity
+from dbma.components.mysql.install import uninstall_mysql
 from dbma.components.mysql.instance import is_instance_exists
-from dbma.components.mysql.install import install_mysql, uninstall_mysql
-from dbma.components.mysql.views.handlers import install_mysql_task_handler
+from dbma.components.mysql.views.handlers import install_mysql_source_task_handler
 from dbma.components.mysql.views.handlers import install_mysql_replica_task_handler
 
 
 @routes.view("/apis/mysqls/defaults")
 class MySQLDefaultsView(web.View):
     """
     MySQL 的全局默认配置
@@ -75,109 +75,112 @@
         # 检查 pkg-name
         if "pkg-name" not in data:
             response.message = "pkg-name not in post dict"
             logging.warn(response.message)
             return web.json_response(response.to_dict(), status=500)
         pkg_name = data["pkg-name"]
         pkg = Path("/usr/local/dbm-agent/pkgs/") / pkg_name
-        
-        # 检查 source ? 
+
+        # 检查 source ?
         if "source" not in data:
             source = None
         else:
-            source = data['source']
+            source = data["source"]
             # 检查格式是否有问题
             p = re.compile("\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3}:\d{1,4}")
             if not p.match(source):
                 response.message = "source arg format error"
                 return web.json_response(response.to_dict(), status=500)
             source_ip, source_port = source.split(":")
-        
-        # 检查 role 
+
+        # 检查 role
         if "role" not in data:
             response.message = "instance 'role' arg missage, you can choise one of ['master', 'slave', 'source', 'replica']"
             return web.json_response(response.to_dict(), status=500)
         else:
-            role = data['role']
+            role = data["role"]
 
         # 检查 task-id ? 参数
         if "task-id" not in data:
             task_id = None
         else:
             task_id = data["task-id"]
-            
+
         # 检查各个参数之间的逻辑关系
-        if role in ('slave', 'replica'):
+        if role in ("slave", "replica"):
             # 在 role 是备机的情况下要求指定 source 参数
             if source is None:
-                response.message = "args role = '{}', you must give 'source' arg ".format(role)
-                return web.json_response(response.to_dict(), status=500)     
+                response.message = (
+                    "args role = '{}', you must give 'source' arg ".format(role)
+                )
+                return web.json_response(response.to_dict(), status=500)
 
         # endregion args-check
 
         # 打印一下接收到的参数
         logging.info(
             "port = '{}', ibps = '{}', pkg-name = '{}', pkg = '{}', source = '{}', role = '{}' task-id = {} .".format(
                 port, ibps, pkg_name, pkg, source, role, task_id
             )
         )
-        
+
         # 根据 task_id 是不是 None 来决定接口是同步执行还是异步执行
         if task_id is not None:
             # 进入异步处理逻辑
-            #---------------
-            if role in ('master', 'source'):
+            # ---------------
+            if role in ("master", "source"):
                 # 进入安装单机/主库的处理逻辑
                 threads.submit(
-                    install_mysql_task_handler,
+                    install_mysql_source_task_handler,
                     port=port,
                     ibps=ibps,
                     pkg=pkg,
-                    task_id=task_id
+                    task_id=task_id,
                 )
-                response.message = "submit install mysql 'master|source' task to backends threads."
-            elif role in ('slave', 'replica'):
+                response.message = (
+                    "submit install mysql 'master|source' task to backends threads."
+                )
+            elif role in ("slave", "replica"):
                 # 进入备机的处理逻辑
                 threads.submit(
                     install_mysql_replica_task_handler,
                     port=port,
                     ibps=ibps,
                     pkg=pkg,
                     source_ip=source_ip,
                     source_port=source_port,
-                    task_id=task_id
+                    task_id=task_id,
+                )
+                response.message = (
+                    "submit install mysql 'slave|replica' task to backends threads."
                 )
-                response.message = "submit install mysql 'slave|replica' task to backends threads."
-                
+
             return web.json_response(response.to_dict(), status=200)
         else:
             # 进入同步处理逻辑
             # -------------
-            if role in ('master', 'source'):
+            if role in ("master", "source"):
                 # 进入安装单机/主库的处理逻辑
-                install_mysql_task_handler(
-                    port=port,
-                    ibps=ibps,
-                    pkg=pkg,
-                    task_id=task_id)
+                install_mysql_source_task_handler(
+                    port=port, ibps=ibps, pkg=pkg, task_id=task_id
+                )
                 response.message = "install mysql 'master|source' complete ."
-            elif role in ('slave', 'replica'):
+            elif role in ("slave", "replica"):
                 # 进入备机的处理逻辑
                 install_mysql_replica_task_handler(
                     port=port,
                     ibps=ibps,
                     pkg=pkg,
                     source_ip=source_ip,
                     source_port=source_port,
-                    task_id=task_id
+                    task_id=task_id,
                 )
                 response.message = "install mysql 'slave|replica' complete ."
-            
-            return web.json_response(response.to_dict(), status=200)
 
+            return web.json_response(response.to_dict(), status=200)
 
 
 @routes.view("/apis/mysqls/uninstall")
 class MySQLUninstallView(web.View):
     """MySQL 卸载逻辑
 
     1. 检查 port 参数有没有传递
```

### Comparing `dbm-agent-8.32.6/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.32.8/dbma/components/mysql/views/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 """dbm-agent 收到操作请求(task)之后，如果请求中没有带 task_id ，说明要求同步执行；如果有带 task_id 那么我们要把 task 放到后台线程中执行。
 
 """
 
 import logging
 from pathlib import Path
 from dbma.bil.sudos import sudo
-from dbma.components.mysql.install import install_mysql
-from dbma.components.mysql.replica import install_replica
+from dbma.components.mysql.source import install_mysql_source
+from dbma.components.mysql.replica import install_mysql_replica
 
 
 def update_task_state_callback(
     task_id: int = None, state: str = None, message: str = None
 ):
     """调用 dbm-center 的接口更新回调任务的状态"""
     logging.info("starts update task state callback .")
     # TODO 调用更新接口ends
     logging.info("task_id = {}".format(task_id))
     logging.info("ends update task state callback .")
 
 
-def install_mysql_task_handler(
+def install_mysql_source_task_handler(
     port: int = 3306, ibps: str = "128M", pkg: Path = None, task_id: int = None
 ):
     """让安装 MySQL 的逻辑放后台执行
 
     Parameters:
     -----------
 
@@ -42,15 +42,15 @@
     -------
     None
     """
     logging.info("starts install mysql 'master|source' task handler .")
     try:
         # 提升后台线程的权限到 root
         with sudo("install mysql task handler"):
-            install_mysql(port=port, innodb_buffer_pool_size=ibps, pkg=pkg)
+            install_mysql_source(port=port, innodb_buffer_pool_size=ibps, pkg=pkg)
         logging.info("install mysql complete")
 
         # 是否更新任务信息到 dbm-center
         if not task_id is None:
             logging.warn(
                 "install mysql task handler's callback function is None, skip callback"
             )
@@ -59,15 +59,20 @@
 
     except Exception as err:
         logging.error("install mysql task handler got error ")
     logging.info("ends install mysql task handler .")
 
 
 def install_mysql_replica_task_handler(
-    port: int = 3306, ibps: str = "128M", pkg: Path = None, source_ip: str = None, source_port: str = None, task_id: int = None
+    port: int = 3306,
+    ibps: str = "128M",
+    pkg: Path = None,
+    source_ip: str = None,
+    source_port: str = None,
+    task_id: int = None,
 ):
     """让安装 MySQL 备机的逻辑放后台执行
 
     Parameters:
     -----------
 
     port: int
@@ -84,22 +89,29 @@
     None
     """
     logging.info("starts install mysql 'slave|replica' task handler .")
     try:
         # 提升后台线程的权限到 root
         with sudo("install mysql task handler"):
             # install_mysql(port=port, innodb_buffer_pool_size=ibps, pkg=pkg)
-            install_replica(port=port, pkg=pkg, innodb_buffer_pool_size=ibps,
-                            source_ip=source_ip, source_port=source_port)
+            install_mysql_replica(
+                port=port,
+                pkg=pkg,
+                innodb_buffer_pool_size=ibps,
+                source_ip=source_ip,
+                source_port=source_port,
+            )
         logging.info("install mysql 'slave|replica' complete")
 
         # 是否更新任务信息到 dbm-center
         if not task_id is None:
             logging.warn(
                 "install mysql 'slave|replica' task handler's callback function is None, skip callback"
             )
         else:
-            update_task_state_callback(task_id, 200, "install mysql 'slave|replica' complete")
+            update_task_state_callback(
+                task_id, 200, "install mysql 'slave|replica' complete"
+            )
 
     except Exception as err:
         logging.error("install mysql 'slave|replica' task handler got error ")
     logging.info("ends install mysql 'slave|replica' task handler .")
```

### Comparing `dbm-agent-8.32.6/dbma/core/agent/init.py` & `dbm-agent-8.32.8/dbma/core/agent/init.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/core/configs.py` & `dbm-agent-8.32.8/dbma/core/configs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/core/httpserver.py` & `dbm-agent-8.32.8/dbma/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/core/messages.py` & `dbm-agent-8.32.8/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/core/threads/backends.py` & `dbm-agent-8.32.8/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.32.8/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.32.8/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/init-8.0.x.sql` & `dbm-agent-8.32.8/dbma/static/cnfs/init-8.0.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -126,14 +126,25 @@
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
 
 #### for clone 
 plugin-load-add                          = mysql_clone.so
 clone                                    = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
 
 
 #### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
```

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -124,16 +124,27 @@
 gtid_mode                                = {{gtid_mode}}
 binlog_gtid_simple_recovery              = {{binlog_gtid_simple_recovery}}
 enforce_gtid_consistency                 = {{enforce_gtid_consistency}}
 gtid_executed_compression_period         = {{gtid_executed_compression_period}}
 
 
 #### for clone 
-plugin-load-add                          = mysql_clone.so
-clone                                    = FORCE_PLUS_PERMANENT
+plugin-load-add                           = mysql_clone.so
+clone                                     = FORCE_PLUS_PERMANENT
+clone_autotune_concurrency                = {{ clone_autotune_concurrency}}
+clone_buffer_size                         = {{ clone_buffer_size}}
+clone_block_ddl                           = {{ clone_block_ddl}}
+clone_delay_after_data_drop               = {{ clone_delay_after_data_drop}}
+clone_ddl_timeout                         = {{ clone_ddl_timeout}}
+clone_donor_timeout_after_network_failure = {{ clone_donor_timeout_after_network_failure}}
+clone_enable_compression                  = {{ clone_enable_compression}}
+clone_max_concurrency                     = {{ clone_max_concurrency}}
+clone_max_data_bandwidth                  = {{ clone_max_data_bandwidth}}
+clone_max_network_bandwidth               = {{ clone_max_network_bandwidth}}
+clone_valid_donor_list                    = {{ clone_valid_donor_list}}
 
 
 #### for engines 
 default_storage_engine                   = {{default_storage_engine}}
 default_tmp_storage_engine               = {{default_tmp_storage_engine}}
 internal_tmp_mem_storage_engine          = {{internal_tmp_mem_storage_engine}}
```

### Comparing `dbm-agent-8.32.6/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.32.8/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.32.6/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.32.8/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

