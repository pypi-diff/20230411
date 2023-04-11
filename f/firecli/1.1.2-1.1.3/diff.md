# Comparing `tmp/firecli-1.1.2.tar.gz` & `tmp/firecli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecli-1.1.2.tar", last modified: Tue Apr 11 19:08:51 2023, max compression
+gzip compressed data, was "firecli-1.1.3.tar", last modified: Tue Apr 11 19:12:22 2023, max compression
```

## Comparing `firecli-1.1.2.tar` & `firecli-1.1.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.588545 firecli-1.1.2/
--rw-rw-r--   0 okaiser    (502) staff       (20)     1023 2023-03-22 14:08:15.000000 firecli-1.1.2/LICENSE.md
--rw-r--r--   0 okaiser    (502) staff       (20)     2372 2023-04-11 19:08:51.588624 firecli-1.1.2/PKG-INFO
--rw-rw-r--   0 okaiser    (502) staff       (20)     1730 2023-02-16 13:11:19.000000 firecli-1.1.2/README.md
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.564283 firecli-1.1.2/etc/
--rw-rw-r--   0 okaiser    (502) staff       (20)      865 2021-10-27 13:51:43.000000 firecli-1.1.2/etc/firecli-complete.sh
--rw-rw-r--   0 okaiser    (502) staff       (20)     2335 2023-03-19 17:05:37.000000 firecli-1.1.2/etc/firecli.yml
--rw-rw-r--   0 okaiser    (502) staff       (20)      851 2021-10-27 13:51:43.000000 firecli-1.1.2/etc/logging.yml
--rw-rw-r--   0 okaiser    (502) staff       (20)     1873 2023-03-12 12:51:26.000000 firecli-1.1.2/etc/overrides.yml
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.565798 firecli-1.1.2/firecli/
--rw-rw-r--   0 okaiser    (502) staff       (20)     3927 2023-03-12 12:42:36.000000 firecli-1.1.2/firecli/__init__.py
--rwxrwxr-x   0 okaiser    (502) staff       (20)      308 2023-03-12 12:43:03.000000 firecli-1.1.2/firecli/__main__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.568299 firecli-1.1.2/firecli/api/
--rw-rw-r--   0 okaiser    (502) staff       (20)    36074 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.569373 firecli-1.1.2/firecli/api/afa/
--rw-rw-r--   0 okaiser    (502) staff       (20)     6978 2023-02-16 13:13:28.000000 firecli-1.1.2/firecli/api/afa/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.569887 firecli-1.1.2/firecli/api/cache/
--rw-rw-r--   0 okaiser    (502) staff       (20)     4654 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/cache/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.570319 firecli-1.1.2/firecli/api/cfg/
--rw-rw-r--   0 okaiser    (502) staff       (20)    15992 2023-03-21 12:18:46.000000 firecli-1.1.2/firecli/api/cfg/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.571521 firecli-1.1.2/firecli/api/click/
--rw-rw-r--   0 okaiser    (502) staff       (20)     3452 2023-03-19 17:17:28.000000 firecli-1.1.2/firecli/api/click/__init__.py
--rw-rw-r--   0 okaiser    (502) staff       (20)     3255 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/click/callback.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.571937 firecli-1.1.2/firecli/api/compliance/
--rw-rw-r--   0 okaiser    (502) staff       (20)     4663 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/compliance/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.572363 firecli-1.1.2/firecli/api/helper/
--rw-rw-r--   0 okaiser    (502) staff       (20)     4221 2023-03-22 13:50:11.000000 firecli-1.1.2/firecli/api/helper/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.572897 firecli-1.1.2/firecli/api/report/
--rw-rw-r--   0 okaiser    (502) staff       (20)     9349 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/report/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.573278 firecli-1.1.2/firecli/api/state/
--rw-rw-r--   0 okaiser    (502) staff       (20)      264 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/api/state/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.574126 firecli-1.1.2/firecli/cli/
--rw-rw-r--   0 okaiser    (502) staff       (20)     6451 2023-03-19 17:17:53.000000 firecli-1.1.2/firecli/cli/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.574525 firecli-1.1.2/firecli/cli/accesspolicy/
--rw-rw-r--   0 okaiser    (502) staff       (20)     5092 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/accesspolicy/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.574913 firecli-1.1.2/firecli/cli/accesspolicy/filepolicy/
--rw-rw-r--   0 okaiser    (502) staff       (20)     1738 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/accesspolicy/filepolicy/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.575284 firecli-1.1.2/firecli/cli/cache/
--rw-rw-r--   0 okaiser    (502) staff       (20)      836 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/cache/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.575663 firecli-1.1.2/firecli/cli/compliance/
--rw-rw-r--   0 okaiser    (502) staff       (20)     2836 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/compliance/__init__.py
--rw-rw-r--   0 okaiser    (502) staff       (20)     1364 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/helper.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.576060 firecli-1.1.2/firecli/cli/log/
--rw-rw-r--   0 okaiser    (502) staff       (20)     3543 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/log/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.576436 firecli-1.1.2/firecli/cli/object/
--rw-rw-r--   0 okaiser    (502) staff       (20)     1009 2023-03-12 10:34:30.000000 firecli-1.1.2/firecli/cli/object/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.576947 firecli-1.1.2/firecli/cli/object/dnsservergroup/
--rw-rw-r--   0 okaiser    (502) staff       (20)      434 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/dnsservergroup/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.577325 firecli-1.1.2/firecli/cli/object/dnsservergroup/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     8630 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/dnsservergroup/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.577804 firecli-1.1.2/firecli/cli/object/host/
--rw-rw-r--   0 okaiser    (502) staff       (20)      384 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/host/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.578181 firecli-1.1.2/firecli/cli/object/host/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     7594 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/host/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.578578 firecli-1.1.2/firecli/cli/object/ipv4addresspool/
--rw-r--r--   0 okaiser    (502) staff       (20)      439 2023-03-12 10:34:16.000000 firecli-1.1.2/firecli/cli/object/ipv4addresspool/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.579068 firecli-1.1.2/firecli/cli/object/ipv4addresspool/override/
--rw-r--r--   0 okaiser    (502) staff       (20)     9041 2023-03-21 13:07:57.000000 firecli-1.1.2/firecli/cli/object/ipv4addresspool/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.579568 firecli-1.1.2/firecli/cli/object/network/
--rw-rw-r--   0 okaiser    (502) staff       (20)      314 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/network/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.579947 firecli-1.1.2/firecli/cli/object/network/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     7730 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/network/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.580337 firecli-1.1.2/firecli/cli/object/networkgroup/
--rw-rw-r--   0 okaiser    (502) staff       (20)      424 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/networkgroup/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.580827 firecli-1.1.2/firecli/cli/object/networkgroup/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     8538 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/networkgroup/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.581328 firecli-1.1.2/firecli/cli/object/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     6158 2023-03-19 16:00:05.000000 firecli-1.1.2/firecli/cli/object/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.581803 firecli-1.1.2/firecli/cli/object/range/
--rw-rw-r--   0 okaiser    (502) staff       (20)      413 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/range/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.582187 firecli-1.1.2/firecli/cli/object/range/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     7681 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/range/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.582553 firecli-1.1.2/firecli/cli/object/timezone/
--rw-rw-r--   0 okaiser    (502) staff       (20)      404 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/timezone/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.582925 firecli-1.1.2/firecli/cli/object/timezone/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     7840 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/timezone/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.583305 firecli-1.1.2/firecli/cli/object/url/
--rw-rw-r--   0 okaiser    (502) staff       (20)      379 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/url/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.583660 firecli-1.1.2/firecli/cli/object/url/override/
--rw-rw-r--   0 okaiser    (502) staff       (20)     7422 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/object/url/override/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.584040 firecli-1.1.2/firecli/cli/report/
--rw-rw-r--   0 okaiser    (502) staff       (20)    15198 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/report/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.584405 firecli-1.1.2/firecli/cli/s2svpn/
--rw-rw-r--   0 okaiser    (502) staff       (20)      391 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/s2svpn/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.584774 firecli-1.1.2/firecli/cli/s2svpn/point2point/
--rw-rw-r--   0 okaiser    (502) staff       (20)     6333 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/s2svpn/point2point/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.585167 firecli-1.1.2/firecli/cli/sync/
--rw-rw-r--   0 okaiser    (502) staff       (20)     1687 2021-10-27 13:51:43.000000 firecli-1.1.2/firecli/cli/sync/__init__.py
--rw-rw-r--   0 okaiser    (502) staff       (20)       22 2023-03-21 13:15:34.000000 firecli-1.1.2/firecli/version.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.567947 firecli-1.1.2/firecli.egg-info/
--rw-r--r--   0 okaiser    (502) staff       (20)     2372 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/PKG-INFO
--rw-r--r--   0 okaiser    (502) staff       (20)     2013 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/SOURCES.txt
--rw-r--r--   0 okaiser    (502) staff       (20)        1 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/dependency_links.txt
--rw-r--r--   0 okaiser    (502) staff       (20)       45 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/entry_points.txt
--rw-r--r--   0 okaiser    (502) staff       (20)      174 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/requires.txt
--rw-r--r--   0 okaiser    (502) staff       (20)       13 2023-04-11 19:08:51.000000 firecli-1.1.2/firecli.egg-info/top_level.txt
--rw-rw-r--   0 okaiser    (502) staff       (20)      208 2021-10-27 13:51:43.000000 firecli-1.1.2/pyproject.toml
--rw-rw-r--   0 okaiser    (502) staff       (20)       63 2023-04-11 19:08:51.588940 firecli-1.1.2/setup.cfg
--rwxrwxr-x   0 okaiser    (502) staff       (20)     1554 2023-04-11 19:08:44.000000 firecli-1.1.2/setup.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.585828 firecli-1.1.2/test/
--rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.2/test/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.586195 firecli-1.1.2/test/api/
--rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.2/test/api/__init__.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.586826 firecli-1.1.2/test/api/cfg/
--rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.2/test/api/cfg/__init__.py
--rw-rw-r--   0 okaiser    (502) staff       (20)      751 2021-10-27 13:51:43.000000 firecli-1.1.2/test/api/cfg/test_cfg.py
-drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:08:51.588251 firecli-1.1.2/test/cli/
--rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.2/test/cli/__init__.py
--rw-rw-r--   0 okaiser    (502) staff       (20)      606 2021-10-27 13:51:43.000000 firecli-1.1.2/test/cli/test_cli.py
--rw-rw-r--   0 okaiser    (502) staff       (20)      401 2021-10-27 13:51:43.000000 firecli-1.1.2/test/cli/test_log.py
--rw-rw-r--   0 okaiser    (502) staff       (20)     1273 2021-10-27 13:51:43.000000 firecli-1.1.2/test/cli/test_report.py
--rw-rw-r--   0 okaiser    (502) staff       (20)      112 2021-10-27 13:51:43.000000 firecli-1.1.2/test/conftest.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.675725 firecli-1.1.3/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1023 2023-03-22 14:08:15.000000 firecli-1.1.3/LICENSE.md
+-rw-r--r--   0 okaiser    (502) staff       (20)     2372 2023-04-11 19:12:22.675815 firecli-1.1.3/PKG-INFO
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1730 2023-02-16 13:11:19.000000 firecli-1.1.3/README.md
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.649057 firecli-1.1.3/etc/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      865 2021-10-27 13:51:43.000000 firecli-1.1.3/etc/firecli-complete.sh
+-rw-rw-r--   0 okaiser    (502) staff       (20)     2335 2023-03-19 17:05:37.000000 firecli-1.1.3/etc/firecli.yml
+-rw-rw-r--   0 okaiser    (502) staff       (20)      851 2021-10-27 13:51:43.000000 firecli-1.1.3/etc/logging.yml
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1873 2023-03-12 12:51:26.000000 firecli-1.1.3/etc/overrides.yml
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.650626 firecli-1.1.3/firecli/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     3927 2023-03-12 12:42:36.000000 firecli-1.1.3/firecli/__init__.py
+-rwxrwxr-x   0 okaiser    (502) staff       (20)      308 2023-03-12 12:43:03.000000 firecli-1.1.3/firecli/__main__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.653271 firecli-1.1.3/firecli/api/
+-rw-rw-r--   0 okaiser    (502) staff       (20)    36074 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.654101 firecli-1.1.3/firecli/api/afa/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     6978 2023-02-16 13:13:28.000000 firecli-1.1.3/firecli/api/afa/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.654650 firecli-1.1.3/firecli/api/cache/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     4654 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/cache/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.655099 firecli-1.1.3/firecli/api/cfg/
+-rw-rw-r--   0 okaiser    (502) staff       (20)    15992 2023-03-21 12:18:46.000000 firecli-1.1.3/firecli/api/cfg/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.656196 firecli-1.1.3/firecli/api/click/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     3452 2023-03-19 17:17:28.000000 firecli-1.1.3/firecli/api/click/__init__.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)     3255 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/click/callback.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.656623 firecli-1.1.3/firecli/api/compliance/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     4663 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/compliance/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.657005 firecli-1.1.3/firecli/api/helper/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     4221 2023-03-22 13:50:11.000000 firecli-1.1.3/firecli/api/helper/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.657496 firecli-1.1.3/firecli/api/report/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     9349 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/report/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.657878 firecli-1.1.3/firecli/api/state/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      264 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/api/state/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.658872 firecli-1.1.3/firecli/cli/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     6451 2023-03-19 17:17:53.000000 firecli-1.1.3/firecli/cli/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.659268 firecli-1.1.3/firecli/cli/accesspolicy/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     5092 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/accesspolicy/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.659697 firecli-1.1.3/firecli/cli/accesspolicy/filepolicy/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1738 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/accesspolicy/filepolicy/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.660229 firecli-1.1.3/firecli/cli/cache/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      836 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/cache/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.660616 firecli-1.1.3/firecli/cli/compliance/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     2836 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/compliance/__init__.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1364 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/helper.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.660990 firecli-1.1.3/firecli/cli/log/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     3543 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/log/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.661367 firecli-1.1.3/firecli/cli/object/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1009 2023-03-12 10:34:30.000000 firecli-1.1.3/firecli/cli/object/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.661878 firecli-1.1.3/firecli/cli/object/dnsservergroup/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      434 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/dnsservergroup/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.662314 firecli-1.1.3/firecli/cli/object/dnsservergroup/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     8630 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/dnsservergroup/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.662822 firecli-1.1.3/firecli/cli/object/host/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      384 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/host/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.663200 firecli-1.1.3/firecli/cli/object/host/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     7594 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/host/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.663601 firecli-1.1.3/firecli/cli/object/ipv4addresspool/
+-rw-r--r--   0 okaiser    (502) staff       (20)      439 2023-03-12 10:34:16.000000 firecli-1.1.3/firecli/cli/object/ipv4addresspool/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.664129 firecli-1.1.3/firecli/cli/object/ipv4addresspool/override/
+-rw-r--r--   0 okaiser    (502) staff       (20)     9041 2023-03-21 13:07:57.000000 firecli-1.1.3/firecli/cli/object/ipv4addresspool/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.664677 firecli-1.1.3/firecli/cli/object/network/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      314 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/network/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.665078 firecli-1.1.3/firecli/cli/object/network/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     7730 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/network/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.665473 firecli-1.1.3/firecli/cli/object/networkgroup/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      424 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/networkgroup/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.665987 firecli-1.1.3/firecli/cli/object/networkgroup/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     8538 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/networkgroup/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.666561 firecli-1.1.3/firecli/cli/object/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     6158 2023-03-19 16:00:05.000000 firecli-1.1.3/firecli/cli/object/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.667090 firecli-1.1.3/firecli/cli/object/range/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      413 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/range/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.667515 firecli-1.1.3/firecli/cli/object/range/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     7681 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/range/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.667971 firecli-1.1.3/firecli/cli/object/timezone/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      404 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/timezone/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.668448 firecli-1.1.3/firecli/cli/object/timezone/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     7840 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/timezone/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.668876 firecli-1.1.3/firecli/cli/object/url/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      379 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/url/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.669391 firecli-1.1.3/firecli/cli/object/url/override/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     7422 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/object/url/override/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.669831 firecli-1.1.3/firecli/cli/report/
+-rw-rw-r--   0 okaiser    (502) staff       (20)    15198 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/report/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.670234 firecli-1.1.3/firecli/cli/s2svpn/
+-rw-rw-r--   0 okaiser    (502) staff       (20)      391 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/s2svpn/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.670617 firecli-1.1.3/firecli/cli/s2svpn/point2point/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     6333 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/s2svpn/point2point/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.671061 firecli-1.1.3/firecli/cli/sync/
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1687 2021-10-27 13:51:43.000000 firecli-1.1.3/firecli/cli/sync/__init__.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)       22 2023-04-11 19:12:14.000000 firecli-1.1.3/firecli/version.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.652907 firecli-1.1.3/firecli.egg-info/
+-rw-r--r--   0 okaiser    (502) staff       (20)     2372 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/PKG-INFO
+-rw-r--r--   0 okaiser    (502) staff       (20)     2013 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/SOURCES.txt
+-rw-r--r--   0 okaiser    (502) staff       (20)        1 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/dependency_links.txt
+-rw-r--r--   0 okaiser    (502) staff       (20)       45 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/entry_points.txt
+-rw-r--r--   0 okaiser    (502) staff       (20)      174 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/requires.txt
+-rw-r--r--   0 okaiser    (502) staff       (20)       13 2023-04-11 19:12:22.000000 firecli-1.1.3/firecli.egg-info/top_level.txt
+-rw-rw-r--   0 okaiser    (502) staff       (20)      208 2021-10-27 13:51:43.000000 firecli-1.1.3/pyproject.toml
+-rw-rw-r--   0 okaiser    (502) staff       (20)       63 2023-04-11 19:12:22.676149 firecli-1.1.3/setup.cfg
+-rwxrwxr-x   0 okaiser    (502) staff       (20)     1554 2023-04-11 19:11:04.000000 firecli-1.1.3/setup.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.671796 firecli-1.1.3/test/
+-rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.3/test/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.672408 firecli-1.1.3/test/api/
+-rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.3/test/api/__init__.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.673376 firecli-1.1.3/test/api/cfg/
+-rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.3/test/api/cfg/__init__.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)      751 2021-10-27 13:51:43.000000 firecli-1.1.3/test/api/cfg/test_cfg.py
+drwxr-xr-x   0 okaiser    (502) staff       (20)        0 2023-04-11 19:12:22.675261 firecli-1.1.3/test/cli/
+-rw-rw-r--   0 okaiser    (502) staff       (20)        0 2021-10-27 13:51:43.000000 firecli-1.1.3/test/cli/__init__.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)      606 2021-10-27 13:51:43.000000 firecli-1.1.3/test/cli/test_cli.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)      401 2021-10-27 13:51:43.000000 firecli-1.1.3/test/cli/test_log.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)     1273 2021-10-27 13:51:43.000000 firecli-1.1.3/test/cli/test_report.py
+-rw-rw-r--   0 okaiser    (502) staff       (20)      112 2021-10-27 13:51:43.000000 firecli-1.1.3/test/conftest.py
```

### Comparing `firecli-1.1.2/LICENSE.md` & `firecli-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/PKG-INFO` & `firecli-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firecli
-Version: 1.1.2
+Version: 1.1.3
 Summary: FireCLI is a command line interface to Firepower Management Center
 Home-page: https://git.ong.at/cisco/firecli.git
 Author: Oliver Kaiser
 Author-email: oliver.kaiser@outlook.com
 Keywords: cisco firepower fmc ftd fpr api rest python api cli
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `firecli-1.1.2/README.md` & `firecli-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/etc/firecli-complete.sh` & `firecli-1.1.3/etc/firecli-complete.sh`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/etc/firecli.yml` & `firecli-1.1.3/etc/firecli.yml`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/etc/logging.yml` & `firecli-1.1.3/etc/logging.yml`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/etc/overrides.yml` & `firecli-1.1.3/etc/overrides.yml`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/__init__.py` & `firecli-1.1.3/firecli/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/__init__.py` & `firecli-1.1.3/firecli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/afa/__init__.py` & `firecli-1.1.3/firecli/api/afa/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/cache/__init__.py` & `firecli-1.1.3/firecli/api/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/cfg/__init__.py` & `firecli-1.1.3/firecli/api/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/click/__init__.py` & `firecli-1.1.3/firecli/api/click/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/click/callback.py` & `firecli-1.1.3/firecli/api/click/callback.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/compliance/__init__.py` & `firecli-1.1.3/firecli/api/compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/helper/__init__.py` & `firecli-1.1.3/firecli/api/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/api/report/__init__.py` & `firecli-1.1.3/firecli/api/report/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/__init__.py` & `firecli-1.1.3/firecli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/accesspolicy/__init__.py` & `firecli-1.1.3/firecli/cli/accesspolicy/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/accesspolicy/filepolicy/__init__.py` & `firecli-1.1.3/firecli/cli/accesspolicy/filepolicy/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/cache/__init__.py` & `firecli-1.1.3/firecli/cli/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/compliance/__init__.py` & `firecli-1.1.3/firecli/cli/compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/helper.py` & `firecli-1.1.3/firecli/cli/helper.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/log/__init__.py` & `firecli-1.1.3/firecli/cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/__init__.py` & `firecli-1.1.3/firecli/cli/object/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/dnsservergroup/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/dnsservergroup/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/host/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/host/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/ipv4addresspool/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/ipv4addresspool/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/network/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/network/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/networkgroup/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/networkgroup/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/range/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/range/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/timezone/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/timezone/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/object/url/override/__init__.py` & `firecli-1.1.3/firecli/cli/object/url/override/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/report/__init__.py` & `firecli-1.1.3/firecli/cli/report/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/s2svpn/point2point/__init__.py` & `firecli-1.1.3/firecli/cli/s2svpn/point2point/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli/cli/sync/__init__.py` & `firecli-1.1.3/firecli/cli/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/firecli.egg-info/PKG-INFO` & `firecli-1.1.3/firecli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firecli
-Version: 1.1.2
+Version: 1.1.3
 Summary: FireCLI is a command line interface to Firepower Management Center
 Home-page: https://git.ong.at/cisco/firecli.git
 Author: Oliver Kaiser
 Author-email: oliver.kaiser@outlook.com
 Keywords: cisco firepower fmc ftd fpr api rest python api cli
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `firecli-1.1.2/firecli.egg-info/SOURCES.txt` & `firecli-1.1.3/firecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/setup.py` & `firecli-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     description='FireCLI is a command line interface to Firepower Management Center',
     keywords='cisco firepower fmc ftd fpr api rest python api cli',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://git.ong.at/cisco/firecli.git',
     packages=setuptools.find_packages(),
     install_requires=[
-        'click>=7.1.2',
+        'click<=8.0.4',
         'fireREST>=1.0.9',
         'jsonschema>=3.2.0',
         'netaddr>=0.8.0',
         'openpyxl>=3.0.3',
         'PyYAML>=5.3.1',
         'python-benedict>=0.18.1',
         'python-json-logger>=2.0.1',
```

### Comparing `firecli-1.1.2/test/api/cfg/test_cfg.py` & `firecli-1.1.3/test/api/cfg/test_cfg.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/test/cli/test_cli.py` & `firecli-1.1.3/test/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `firecli-1.1.2/test/cli/test_report.py` & `firecli-1.1.3/test/cli/test_report.py`

 * *Files identical despite different names*

