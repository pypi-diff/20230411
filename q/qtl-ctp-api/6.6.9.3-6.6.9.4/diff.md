# Comparing `tmp/qtl-ctp-api-6.6.9.3.tar.gz` & `tmp/qtl-ctp-api-6.6.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtl-ctp-api-6.6.9.3.tar", last modified: Fri Dec 16 04:31:48 2022, max compression
+gzip compressed data, was "qtl-ctp-api-6.6.9.4.tar", last modified: Tue Apr 11 07:20:29 2023, max compression
```

## Comparing `qtl-ctp-api-6.6.9.3.tar` & `qtl-ctp-api-6.6.9.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.627033 qtl-ctp-api-6.6.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.603032 qtl-ctp-api-6.6.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.607032 qtl-ctp-api-6.6.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-16 04:31:48.627033 qtl-ctp-api-6.6.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.603032 qtl-ctp-api-6.6.9.3/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.603032 qtl-ctp-api-6.6.9.3/libs/ctp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.607032 qtl-ctp-api-6.6.9.3/libs/ctp/include/
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcMdApi.h
--rw-r--r--   0 runner    (1001) docker     (123)    43382 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcTraderApi.h
--rw-r--r--   0 runner    (1001) docker     (123)   273909 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcUserApiDataType.h
--rw-r--r--   0 runner    (1001) docker     (123)   299614 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcUserApiStruct.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.615033 qtl-ctp-api-6.6.9.3/libs/ctp/lib/
--rw-r--r--   0 runner    (1001) docker     (123)  4818248 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/lib/libthostmduserapi_se.so
--rw-r--r--   0 runner    (1001) docker     (123)  5467003 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/libs/ctp/lib/libthosttraderapi_se.so
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.607032 qtl-ctp-api-6.6.9.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.619033 qtl-ctp-api-6.6.9.3/scripts/generator/
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.623033 qtl-ctp-api-6.6.9.3/scripts/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/bind_consts.cpp.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/bind_md_api.cpp.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/bind_td_api.cpp.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/md_api.cpp.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/md_api.h.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/td_api.cpp.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/scripts/generator/templates/td_api.h.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 04:31:48.627033 qtl-ctp-api-6.6.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.623033 qtl-ctp-api-6.6.9.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    66644 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_consts.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_consts.h
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_md_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_md_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_td_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/bind_td_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/dispatch_queue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/dispatch_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/md_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/md_api.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.623033 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.623033 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-16 04:31:48.000000 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2022-12-16 04:31:48.000000 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 04:31:48.000000 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-16 04:31:48.000000 qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    56797 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/td_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/td_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/src/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 04:31:48.627033 qtl-ctp-api-6.6.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/tests/test_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2022-12-16 04:31:35.000000 qtl-ctp-api-6.6.9.3/tests/test_td.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.896727 qtl-ctp-api-6.6.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.896727 qtl-ctp-api-6.6.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.896727 qtl-ctp-api-6.6.9.4/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.896727 qtl-ctp-api-6.6.9.4/libs/ctp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.900727 qtl-ctp-api-6.6.9.4/libs/ctp/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcMdApi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43382 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcTraderApi.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273909 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcUserApiDataType.h
+-rw-r--r--   0 runner    (1001) docker     (123)   299614 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcUserApiStruct.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.904727 qtl-ctp-api-6.6.9.4/libs/ctp/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)  4818248 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/lib/libthostmduserapi_se.so
+-rw-r--r--   0 runner    (1001) docker     (123)  5467003 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/libs/ctp/lib/libthosttraderapi_se.so
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.896727 qtl-ctp-api-6.6.9.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.908727 qtl-ctp-api-6.6.9.4/scripts/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.908727 qtl-ctp-api-6.6.9.4/scripts/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/bind_consts.cpp.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/bind_md_api.cpp.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/bind_td_api.cpp.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/md_api.cpp.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/md_api.h.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/td_api.cpp.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/scripts/generator/templates/td_api.h.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    66646 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_consts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_consts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_md_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_md_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_td_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/bind_td_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/dispatch_queue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/dispatch_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/md_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/md_api.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 07:20:29.000000 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 07:20:29.000000 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:20:29.000000 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-11 07:20:29.000000 qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/td_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/td_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/src/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:20:29.912727 qtl-ctp-api-6.6.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/tests/test_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-11 07:20:11.000000 qtl-ctp-api-6.6.9.4/tests/test_td.py
```

### Comparing `qtl-ctp-api-6.6.9.3/.github/workflows/publish-to-pypi.yml` & `qtl-ctp-api-6.6.9.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcMdApi.h` & `qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcMdApi.h`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcTraderApi.h` & `qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcTraderApi.h`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcUserApiDataType.h` & `qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcUserApiDataType.h`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/include/ThostFtdcUserApiStruct.h` & `qtl-ctp-api-6.6.9.4/libs/ctp/include/ThostFtdcUserApiStruct.h`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/lib/libthostmduserapi_se.so` & `qtl-ctp-api-6.6.9.4/libs/ctp/lib/libthostmduserapi_se.so`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/libs/ctp/lib/libthosttraderapi_se.so` & `qtl-ctp-api-6.6.9.4/libs/ctp/lib/libthosttraderapi_se.so`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/generate.py` & `qtl-ctp-api-6.6.9.4/scripts/generator/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,17 @@
         if type_ == 'int' and name == 'nTimeLapse':
             return 'time_lapse', 'int'
         if type_ == 'int' and name == 'nRequestID':
             return 'request_id', 'int'
         if type_ == 'bool' and name == 'bIsLast':
             return 'is_last', 'bool'
         if name == 'pRspInfo':
-            return 'error', 'const py::dict &'
+            return 'error', 'const nb::dict &'
         if type_.endswith(' *'):
-            return 'data', 'const py::dict &'
+            return 'data', 'const nb::dict &'
         return '', ''
 
     def parse_methods(self, cpp_header):
         on_methods = []
         req_methods = []
 
         for name, c in cpp_header.classes.items():
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/bind_md_api.cpp.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/bind_md_api.cpp.tpl`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "bind_md_api.h"
 
-void bind_md_api(py::module &m) {
-    py::class_<MdApi, PyMdApi> md_api(m, "MdApi", py::module_local());
+void bind_md_api(nb::module_ &m) {
+    nb::class_<MdApi, PyMdApi> md_api(m, "MdApi");
     md_api
-            .def(py::init<>())
+            .def(nb::init<>())
             .def("CreateApi", &MdApi::CreateApi)
             .def("Release", &MdApi::Release)
             .def("Init", &MdApi::Init)
             .def("Join", &MdApi::Join)
             .def_static("GetApiVersion", &MdApi::GetApiVersion)
             .def("GetTradingDay", &MdApi::GetTradingDay)
             .def("RegisterFront", &MdApi::RegisterFront)
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/bind_td_api.cpp.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/bind_td_api.cpp.tpl`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "bind_td_api.h"
 
-void bind_td_api(py::module &m) {
-    py::class_<TdApi, PyTdApi> td_api(m, "TdApi", py::module_local());
+void bind_td_api(nb::module_ &m) {
+    nb::class_<TdApi, PyTdApi> td_api(m, "TdApi");
     td_api
-            .def(py::init<>())
+            .def(nb::init<>())
             .def("CreateApi", &TdApi::CreateApi)
             .def("Release", &TdApi::Release)
             .def("Init", &TdApi::Init)
             .def("Join", &TdApi::Join)
             .def_static("GetApiVersion", &TdApi::GetApiVersion)
             .def("GetTradingDay", &TdApi::GetTradingDay)
             .def("RegisterFront", &TdApi::RegisterFront)
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/md_api.cpp.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/md_api.cpp.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -76,24 +76,24 @@
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     {%- endif %}{% endfor %}
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         {%- for p in on_method['parameters'] %}{% if p['type'].endswith('*') and p['py_name'] == 'data' %}
-        py::dict py_data;
+        nb::dict py_data;
         if (has_data) {
             {%- for sp in structs[p['type'].strip(' *')] %}
             py_data["{{ sp['name'] }}"] = {% if sp['type']=='str' %}gbk_to_utf8({% elif sp['type']=='double' and ('Price' in sp['name'] or 'Delta' in sp['name']) %}adjust_number({% endif %}rsp_data.{{ sp['name'] }}{% if sp['type']=='str' or (sp['type']=='double' and ('Price' in sp['name'] or 'Delta' in sp['name'])) %}){% endif %};
             {%- endfor %}
         }
         {%- elif p['type'].endswith('*') and p['py_name'] == 'error' %}
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             {%- for sp in structs[p['type'].strip(' *')] %}
             py_error["{{ sp['name'] }}"] = {% if sp['type']=='str' %}gbk_to_utf8({% endif %}rsp_error.{{ sp['name'] }}{% if sp['type']=='str' %}){% endif %};
             {%- endfor %}
         }
         {%- endif %}{% endfor %}
         Py{{ on_method['name'] }}(
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/md_api.h.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/md_api.h.tpl`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #ifndef MD_API_H
 #define MD_API_H
 
 #include <iostream>
 #include <string>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
+#include <nanobind/nanobind.h>
+#include <nanobind/stl/vector.h>
+#include <nanobind/trampoline.h>
 
 #include "utils.h"
 #include "dispatch_queue.h"
 #include "ThostFtdcMdApi.h"
 
 
-namespace py = pybind11;
+namespace nb = nanobind;
 
 
 class MdApi : public CThostFtdcMdSpi {
 private:
     std::unique_ptr<DispatchQueue> queue_;
     CThostFtdcMdApi* api_;
 
@@ -51,28 +52,26 @@
     ) = 0;
 {%- endfor %}
 };
 
 
 class PyMdApi final : public MdApi {
 public:
-    using MdApi::MdApi;
+    NB_TRAMPOLINE(MdApi, {{md_on_methods|length}});
 {% for on_method in md_on_methods %}
     void Py{{ on_method['name'] }}(
         {%- for p in on_method['parameters'] -%}
         {{ p['py_type'] }}{% if not p['py_type'].endswith('&') %} {% endif %}{{ p['py_name'] }}{% if not loop.last %}, {% endif %}
         {%- endfor -%}
     ) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+        NB_OVERRIDE_PURE_NAME(
             "{{ on_method['name'] }}",
             Py{{ on_method['name'] }},
             {%- for p in on_method['parameters'] %}
             {{ p['py_name'] }}{% if not loop.last %},{% endif %}
             {%- endfor %}
-        )
+        );
     }
 {% endfor %}
 };
 
 #endif //MD_API_H
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/td_api.cpp.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/td_api.cpp.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -72,24 +72,24 @@
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     {%- endif %}{% endfor %}
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         {%- for p in on_method['parameters'] %}{% if p['type'].endswith('*') and p['py_name'] == 'data' %}
-        py::dict py_data;
+        nb::dict py_data;
         if (has_data) {
             {%- for sp in structs[p['type'].strip(' *')] %}
-            py_data["{{ sp['name'] }}"] = {% if sp['type'] == 'bytes' %}py::bytes({% elif sp['type']=='str' %}gbk_to_utf8({% elif sp['type']=='double' and ('MarginRatio' in sp['name']) %}adjust_number({% endif %}rsp_data.{{ sp['name'] }}{% if sp['type'] in ('str', 'bytes') or (sp['type']=='double' and ('MarginRatio' in sp['name'])) %}){% endif %};
+            py_data["{{ sp['name'] }}"] = {% if sp['type'] == 'bytes' %}nb::bytes({% elif sp['type']=='str' %}gbk_to_utf8({% elif sp['type']=='double' and ('MarginRatio' in sp['name']) %}adjust_number({% endif %}rsp_data.{{ sp['name'] }}{% if sp['type'] in ('str', 'bytes') or (sp['type']=='double' and ('MarginRatio' in sp['name'])) %}){% endif %};
             {%- endfor %}
         }
         {%- elif p['type'].endswith('*') and p['py_name'] == 'error' %}
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             {%- for sp in structs[p['type'].strip(' *')] %}
             py_error["{{ sp['name'] }}"] = {% if sp['type']=='str' %}gbk_to_utf8({% endif %}rsp_error.{{ sp['name'] }}{% if sp['type']=='str' %}){% endif %};
             {%- endfor %}
         }
         {%- endif %}{% endfor %}
         Py{{ on_method['name'] }}(
```

### Comparing `qtl-ctp-api-6.6.9.3/scripts/generator/templates/td_api.h.tpl` & `qtl-ctp-api-6.6.9.4/scripts/generator/templates/td_api.h.tpl`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #ifndef TD_API_H
 #define TD_API_H
 
 #include <iostream>
 #include <string>
-#include <pybind11/pybind11.h>
+#include <nanobind/nanobind.h>
+#include <nanobind/trampoline.h>
 
 #include "utils.h"
 #include "dispatch_queue.h"
 #include "ThostFtdcTraderApi.h"
 
 
-namespace py = pybind11;
+namespace nb = nanobind;
 
 
 class TdApi : public CThostFtdcTraderSpi {
 private:
     std::unique_ptr<DispatchQueue> queue_;
     CThostFtdcTraderApi* api_;
 
@@ -50,28 +51,26 @@
     ) = 0;
 {%- endfor %}
 };
 
 
 class PyTdApi final : public TdApi {
 public:
-    using TdApi::TdApi;
+    NB_TRAMPOLINE(TdApi, {{td_on_methods|length}});
 {% for on_method in td_on_methods %}
     void Py{{ on_method['name'] }}(
         {%- for p in on_method['parameters'] -%}
         {{ p['py_type'] }}{% if not p['py_type'].endswith('&') %} {% endif %}{{ p['py_name'] }}{% if not loop.last %}, {% endif %}
         {%- endfor -%}
     ) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            TdApi,
+        NB_OVERRIDE_PURE_NAME(
             "{{ on_method['name'] }}",
             Py{{ on_method['name'] }},
             {%- for p in on_method['parameters'] %}
             {{ p['py_name'] }}{% if not loop.last %},{% endif %}
             {%- endfor %}
-        )
+        );
     }
 {% endfor %}
 };
 
 #endif //TD_API_H
```

### Comparing `qtl-ctp-api-6.6.9.3/src/bind_consts.cpp` & `qtl-ctp-api-6.6.9.4/src/bind_consts.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // generated by script
 #include "bind_consts.h"
 
 
-void bind_consts(py::module &m) {
-    py::module consts = m.def_submodule("consts", "API Consts");
+void bind_consts(nb::module_ &m) {
+    nb::module_ consts = m.def_submodule("consts", "API Consts");
 
     consts.attr("THOST_TERT_RESTART") = 0;
     consts.attr("THOST_TERT_RESUME") = 1;
     consts.attr("THOST_TERT_QUICK") = 2;
     consts.attr("THOST_TERT_NONE") = 3;
     consts.attr("THOST_FTDC_EXP_Normal") = "0";
     consts.attr("THOST_FTDC_EXP_GenOrderByTrade") = "1";
```

### Comparing `qtl-ctp-api-6.6.9.3/src/bind_md_api.cpp` & `qtl-ctp-api-6.6.9.4/src/bind_md_api.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "bind_md_api.h"
 
-void bind_md_api(py::module &m) {
-    py::class_<MdApi, PyMdApi> md_api(m, "MdApi", py::module_local());
+void bind_md_api(nb::module_ &m) {
+    nb::class_<MdApi, PyMdApi> md_api(m, "MdApi");
     md_api
-            .def(py::init<>())
+            .def(nb::init<>())
             .def("CreateApi", &MdApi::CreateApi)
             .def("Release", &MdApi::Release)
             .def("Init", &MdApi::Init)
             .def("Join", &MdApi::Join)
             .def_static("GetApiVersion", &MdApi::GetApiVersion)
             .def("GetTradingDay", &MdApi::GetTradingDay)
             .def("RegisterFront", &MdApi::RegisterFront)
```

### Comparing `qtl-ctp-api-6.6.9.3/src/bind_td_api.cpp` & `qtl-ctp-api-6.6.9.4/src/bind_td_api.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "bind_td_api.h"
 
-void bind_td_api(py::module &m) {
-    py::class_<TdApi, PyTdApi> td_api(m, "TdApi", py::module_local());
+void bind_td_api(nb::module_ &m) {
+    nb::class_<TdApi, PyTdApi> td_api(m, "TdApi");
     td_api
-            .def(py::init<>())
+            .def(nb::init<>())
             .def("CreateApi", &TdApi::CreateApi)
             .def("Release", &TdApi::Release)
             .def("Init", &TdApi::Init)
             .def("Join", &TdApi::Join)
             .def_static("GetApiVersion", &TdApi::GetApiVersion)
             .def("GetTradingDay", &TdApi::GetTradingDay)
             .def("RegisterFront", &TdApi::RegisterFront)
```

### Comparing `qtl-ctp-api-6.6.9.3/src/dispatch_queue.cpp` & `qtl-ctp-api-6.6.9.4/src/dispatch_queue.cpp`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/src/dispatch_queue.h` & `qtl-ctp-api-6.6.9.4/src/dispatch_queue.h`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/src/md_api.cpp` & `qtl-ctp-api-6.6.9.4/src/md_api.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 int MdApi::UnSubscribeMarketData(const std::vector<std::string> &instrument_ids) {
     std::vector<char *> instrument_ids_{};
     for (const auto &i : instrument_ids) instrument_ids_.emplace_back(const_cast<char *>(i.c_str()));
     return api_->UnSubscribeMarketData(instrument_ids_.data(), instrument_ids_.size());
 }
 
-int MdApi::ReqUserLogin(const py::dict &data, int request_id) {
+int MdApi::ReqUserLogin(const nb::dict &data, int request_id) {
     CThostFtdcReqUserLoginField request{};
     set_str_field(request.TradingDay, data, "TradingDay", sizeof(request.TradingDay));
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     set_str_field(request.Password, data, "Password", sizeof(request.Password));
     set_str_field(request.UserProductInfo, data, "UserProductInfo", sizeof(request.UserProductInfo));
     set_str_field(request.InterfaceProductInfo, data, "InterfaceProductInfo", sizeof(request.InterfaceProductInfo));
@@ -59,38 +59,38 @@
     set_str_field(request.OneTimePassword, data, "OneTimePassword", sizeof(request.OneTimePassword));
     set_str_field(request.LoginRemark, data, "LoginRemark", sizeof(request.LoginRemark));
     set_int_field(request.ClientIPPort, data, "ClientIPPort");
     set_str_field(request.ClientIPAddress, data, "ClientIPAddress", sizeof(request.ClientIPAddress));
     return api_->ReqUserLogin(&request, request_id);
 }
 
-int MdApi::ReqUserLogout(const py::dict &data, int request_id) {
+int MdApi::ReqUserLogout(const nb::dict &data, int request_id) {
     CThostFtdcUserLogoutField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     return api_->ReqUserLogout(&request, request_id);
 }
 
 void MdApi::OnFrontConnected() {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnFrontConnected();
     });
 }
 
 void MdApi::OnFrontDisconnected(int reason) {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnFrontDisconnected(reason);
     });
 }
 
 void MdApi::OnHeartBeatWarning(int time_lapse) {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnHeartBeatWarning(time_lapse);
     });
 }
 
 void MdApi::OnRspUserLogin(CThostFtdcRspUserLoginField *data, CThostFtdcRspInfoField *error, int request_id, bool is_last) {
     CThostFtdcRspUserLoginField rsp_data{};
     bool has_data = false;
@@ -101,16 +101,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["TradingDay"] = gbk_to_utf8(rsp_data.TradingDay);
             py_data["LoginTime"] = gbk_to_utf8(rsp_data.LoginTime);
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["SystemName"] = gbk_to_utf8(rsp_data.SystemName);
             py_data["FrontID"] = rsp_data.FrontID;
@@ -120,15 +120,15 @@
             py_data["DCETime"] = gbk_to_utf8(rsp_data.DCETime);
             py_data["CZCETime"] = gbk_to_utf8(rsp_data.CZCETime);
             py_data["FFEXTime"] = gbk_to_utf8(rsp_data.FFEXTime);
             py_data["INETime"] = gbk_to_utf8(rsp_data.INETime);
             py_data["SysVersion"] = gbk_to_utf8(rsp_data.SysVersion);
             py_data["GFEXTime"] = gbk_to_utf8(rsp_data.GFEXTime);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspUserLogin(py_data, py_error, request_id, is_last);
     });
 }
@@ -143,21 +143,21 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspUserLogout(py_data, py_error, request_id, is_last);
     });
 }
@@ -166,16 +166,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_error;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspError(py_error, request_id, is_last);
     });
 }
@@ -190,20 +190,20 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspSubMarketData(py_data, py_error, request_id, is_last);
     });
 }
@@ -218,20 +218,20 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspUnSubMarketData(py_data, py_error, request_id, is_last);
     });
 }
@@ -240,16 +240,16 @@
     CThostFtdcDepthMarketDataField rsp_data{};
     bool has_data = false;
     if (data) {
         rsp_data = *data;
         has_data = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["TradingDay"] = gbk_to_utf8(rsp_data.TradingDay);
             py_data["ExchangeID"] = gbk_to_utf8(rsp_data.ExchangeID);
             py_data["LastPrice"] = adjust_number(rsp_data.LastPrice);
             py_data["PreSettlementPrice"] = adjust_number(rsp_data.PreSettlementPrice);
             py_data["PreClosePrice"] = adjust_number(rsp_data.PreClosePrice);
             py_data["PreOpenInterest"] = rsp_data.PreOpenInterest;
```

### Comparing `qtl-ctp-api-6.6.9.3/src/md_api.h` & `qtl-ctp-api-6.6.9.4/src/md_api.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #ifndef MD_API_H
 #define MD_API_H
 
 #include <iostream>
 #include <string>
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
+#include <nanobind/nanobind.h>
+#include <nanobind/stl/vector.h>
+#include <nanobind/trampoline.h>
 
 #include "utils.h"
 #include "dispatch_queue.h"
 #include "ThostFtdcMdApi.h"
 
 
-namespace py = pybind11;
+namespace nb = nanobind;
 
 
 class MdApi : public CThostFtdcMdSpi {
 private:
     std::unique_ptr<DispatchQueue> queue_;
     CThostFtdcMdApi* api_;
 
@@ -26,142 +27,124 @@
     int Join();
     static std::string GetApiVersion();
     std::string GetTradingDay();
     void RegisterFront(const std::string &front_address);
     int SubscribeMarketData(const std::vector<std::string> &instrument_ids);
     int UnSubscribeMarketData(const std::vector<std::string> &instrument_ids);
 
-    int ReqUserLogin(const py::dict &data, int request_id);
-    int ReqUserLogout(const py::dict &data, int request_id);
+    int ReqUserLogin(const nb::dict &data, int request_id);
+    int ReqUserLogout(const nb::dict &data, int request_id);
 
     void OnFrontConnected() override;
     void OnFrontDisconnected(int nReason) override;
     void OnHeartBeatWarning(int nTimeLapse) override;
     void OnRspUserLogin(CThostFtdcRspUserLoginField *pRspUserLogin, CThostFtdcRspInfoField *pRspInfo, int nRequestID, bool bIsLast) override;
     void OnRspUserLogout(CThostFtdcUserLogoutField *pUserLogout, CThostFtdcRspInfoField *pRspInfo, int nRequestID, bool bIsLast) override;
     void OnRspError(CThostFtdcRspInfoField *pRspInfo, int nRequestID, bool bIsLast) override;
     void OnRspSubMarketData(CThostFtdcSpecificInstrumentField *pSpecificInstrument, CThostFtdcRspInfoField *pRspInfo, int nRequestID, bool bIsLast) override;
     void OnRspUnSubMarketData(CThostFtdcSpecificInstrumentField *pSpecificInstrument, CThostFtdcRspInfoField *pRspInfo, int nRequestID, bool bIsLast) override;
     void OnRtnDepthMarketData(CThostFtdcDepthMarketDataField *pDepthMarketData) override;
 
     virtual void PyOnFrontConnected() = 0;
     virtual void PyOnFrontDisconnected(int reason) = 0;
     virtual void PyOnHeartBeatWarning(int time_lapse) = 0;
-    virtual void PyOnRspUserLogin(const py::dict &data, const py::dict &error, int request_id, bool is_last) = 0;
-    virtual void PyOnRspUserLogout(const py::dict &data, const py::dict &error, int request_id, bool is_last) = 0;
-    virtual void PyOnRspError(const py::dict &error, int request_id, bool is_last) = 0;
-    virtual void PyOnRspSubMarketData(const py::dict &data, const py::dict &error, int request_id, bool is_last) = 0;
-    virtual void PyOnRspUnSubMarketData(const py::dict &data, const py::dict &error, int request_id, bool is_last) = 0;
-    virtual void PyOnRtnDepthMarketData(const py::dict &data) = 0;
+    virtual void PyOnRspUserLogin(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) = 0;
+    virtual void PyOnRspUserLogout(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) = 0;
+    virtual void PyOnRspError(const nb::dict &error, int request_id, bool is_last) = 0;
+    virtual void PyOnRspSubMarketData(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) = 0;
+    virtual void PyOnRspUnSubMarketData(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) = 0;
+    virtual void PyOnRtnDepthMarketData(const nb::dict &data) = 0;
 };
 
 
 class PyMdApi final : public MdApi {
 public:
-    using MdApi::MdApi;
+    NB_TRAMPOLINE(MdApi, 9);
 
     void PyOnFrontConnected() override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+        NB_OVERRIDE_PURE_NAME(
             "OnFrontConnected",
             PyOnFrontConnected,
-        )
+        );
     }
 
     void PyOnFrontDisconnected(int reason) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+        NB_OVERRIDE_PURE_NAME(
             "OnFrontDisconnected",
             PyOnFrontDisconnected,
             reason
-        )
+        );
     }
 
     void PyOnHeartBeatWarning(int time_lapse) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+        NB_OVERRIDE_PURE_NAME(
             "OnHeartBeatWarning",
             PyOnHeartBeatWarning,
             time_lapse
-        )
+        );
     }
 
-    void PyOnRspUserLogin(const py::dict &data, const py::dict &error, int request_id, bool is_last) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRspUserLogin(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRspUserLogin",
             PyOnRspUserLogin,
             data,
             error,
             request_id,
             is_last
-        )
+        );
     }
 
-    void PyOnRspUserLogout(const py::dict &data, const py::dict &error, int request_id, bool is_last) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRspUserLogout(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRspUserLogout",
             PyOnRspUserLogout,
             data,
             error,
             request_id,
             is_last
-        )
+        );
     }
 
-    void PyOnRspError(const py::dict &error, int request_id, bool is_last) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRspError(const nb::dict &error, int request_id, bool is_last) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRspError",
             PyOnRspError,
             error,
             request_id,
             is_last
-        )
+        );
     }
 
-    void PyOnRspSubMarketData(const py::dict &data, const py::dict &error, int request_id, bool is_last) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRspSubMarketData(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRspSubMarketData",
             PyOnRspSubMarketData,
             data,
             error,
             request_id,
             is_last
-        )
+        );
     }
 
-    void PyOnRspUnSubMarketData(const py::dict &data, const py::dict &error, int request_id, bool is_last) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRspUnSubMarketData(const nb::dict &data, const nb::dict &error, int request_id, bool is_last) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRspUnSubMarketData",
             PyOnRspUnSubMarketData,
             data,
             error,
             request_id,
             is_last
-        )
+        );
     }
 
-    void PyOnRtnDepthMarketData(const py::dict &data) override {
-        PYBIND11_OVERLOAD_PURE_NAME(
-            void,
-            MdApi,
+    void PyOnRtnDepthMarketData(const nb::dict &data) override {
+        NB_OVERRIDE_PURE_NAME(
             "OnRtnDepthMarketData",
             PyOnRtnDepthMarketData,
             data
-        )
+        );
     }
 
 };
 
 #endif //MD_API_H
```

### Comparing `qtl-ctp-api-6.6.9.3/src/qtl_ctp_api.egg-info/SOURCES.txt` & `qtl-ctp-api-6.6.9.4/src/qtl_ctp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/src/td_api.cpp` & `qtl-ctp-api-6.6.9.4/src/td_api.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,25 @@
     api_->SubscribePrivateTopic((THOST_TE_RESUME_TYPE)resume_type);
 }
 
 void TdApi::SubscribePublicTopic(int resume_type) {
     api_->SubscribePublicTopic((THOST_TE_RESUME_TYPE)resume_type);
 }
 
-int TdApi::ReqAuthenticate(const py::dict &data, int request_id) {
+int TdApi::ReqAuthenticate(const nb::dict &data, int request_id) {
     CThostFtdcReqAuthenticateField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     set_str_field(request.UserProductInfo, data, "UserProductInfo", sizeof(request.UserProductInfo));
     set_str_field(request.AuthCode, data, "AuthCode", sizeof(request.AuthCode));
     set_str_field(request.AppID, data, "AppID", sizeof(request.AppID));
     return api_->ReqAuthenticate(&request, request_id);
 }
 
-int TdApi::ReqUserLogin(const py::dict &data, int request_id) {
+int TdApi::ReqUserLogin(const nb::dict &data, int request_id) {
     CThostFtdcReqUserLoginField request{};
     set_str_field(request.TradingDay, data, "TradingDay", sizeof(request.TradingDay));
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     set_str_field(request.Password, data, "Password", sizeof(request.Password));
     set_str_field(request.UserProductInfo, data, "UserProductInfo", sizeof(request.UserProductInfo));
     set_str_field(request.InterfaceProductInfo, data, "InterfaceProductInfo", sizeof(request.InterfaceProductInfo));
@@ -65,31 +65,31 @@
     set_str_field(request.OneTimePassword, data, "OneTimePassword", sizeof(request.OneTimePassword));
     set_str_field(request.LoginRemark, data, "LoginRemark", sizeof(request.LoginRemark));
     set_int_field(request.ClientIPPort, data, "ClientIPPort");
     set_str_field(request.ClientIPAddress, data, "ClientIPAddress", sizeof(request.ClientIPAddress));
     return api_->ReqUserLogin(&request, request_id);
 }
 
-int TdApi::ReqUserLogout(const py::dict &data, int request_id) {
+int TdApi::ReqUserLogout(const nb::dict &data, int request_id) {
     CThostFtdcUserLogoutField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     return api_->ReqUserLogout(&request, request_id);
 }
 
-int TdApi::ReqUserPasswordUpdate(const py::dict &data, int request_id) {
+int TdApi::ReqUserPasswordUpdate(const nb::dict &data, int request_id) {
     CThostFtdcUserPasswordUpdateField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     set_str_field(request.OldPassword, data, "OldPassword", sizeof(request.OldPassword));
     set_str_field(request.NewPassword, data, "NewPassword", sizeof(request.NewPassword));
     return api_->ReqUserPasswordUpdate(&request, request_id);
 }
 
-int TdApi::ReqOrderInsert(const py::dict &data, int request_id) {
+int TdApi::ReqOrderInsert(const nb::dict &data, int request_id) {
     CThostFtdcInputOrderField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.OrderRef, data, "OrderRef", sizeof(request.OrderRef));
     set_str_field(request.UserID, data, "UserID", sizeof(request.UserID));
     set_char_field(request.OrderPriceType, data, "OrderPriceType");
     set_char_field(request.Direction, data, "Direction");
@@ -116,15 +116,15 @@
     set_str_field(request.ClientID, data, "ClientID", sizeof(request.ClientID));
     set_str_field(request.MacAddress, data, "MacAddress", sizeof(request.MacAddress));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     set_str_field(request.IPAddress, data, "IPAddress", sizeof(request.IPAddress));
     return api_->ReqOrderInsert(&request, request_id);
 }
 
-int TdApi::ReqOrderAction(const py::dict &data, int request_id) {
+int TdApi::ReqOrderAction(const nb::dict &data, int request_id) {
     CThostFtdcInputOrderActionField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_int_field(request.OrderActionRef, data, "OrderActionRef");
     set_str_field(request.OrderRef, data, "OrderRef", sizeof(request.OrderRef));
     set_int_field(request.RequestID, data, "RequestID");
     set_int_field(request.FrontID, data, "FrontID");
@@ -138,108 +138,108 @@
     set_str_field(request.InvestUnitID, data, "InvestUnitID", sizeof(request.InvestUnitID));
     set_str_field(request.MacAddress, data, "MacAddress", sizeof(request.MacAddress));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     set_str_field(request.IPAddress, data, "IPAddress", sizeof(request.IPAddress));
     return api_->ReqOrderAction(&request, request_id);
 }
 
-int TdApi::ReqSettlementInfoConfirm(const py::dict &data, int request_id) {
+int TdApi::ReqSettlementInfoConfirm(const nb::dict &data, int request_id) {
     CThostFtdcSettlementInfoConfirmField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.ConfirmDate, data, "ConfirmDate", sizeof(request.ConfirmDate));
     set_str_field(request.ConfirmTime, data, "ConfirmTime", sizeof(request.ConfirmTime));
     set_int_field(request.SettlementID, data, "SettlementID");
     set_str_field(request.AccountID, data, "AccountID", sizeof(request.AccountID));
     set_str_field(request.CurrencyID, data, "CurrencyID", sizeof(request.CurrencyID));
     return api_->ReqSettlementInfoConfirm(&request, request_id);
 }
 
-int TdApi::ReqQryOrder(const py::dict &data, int request_id) {
+int TdApi::ReqQryOrder(const nb::dict &data, int request_id) {
     CThostFtdcQryOrderField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.ExchangeID, data, "ExchangeID", sizeof(request.ExchangeID));
     set_str_field(request.OrderSysID, data, "OrderSysID", sizeof(request.OrderSysID));
     set_str_field(request.InsertTimeStart, data, "InsertTimeStart", sizeof(request.InsertTimeStart));
     set_str_field(request.InsertTimeEnd, data, "InsertTimeEnd", sizeof(request.InsertTimeEnd));
     set_str_field(request.InvestUnitID, data, "InvestUnitID", sizeof(request.InvestUnitID));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     return api_->ReqQryOrder(&request, request_id);
 }
 
-int TdApi::ReqQryTrade(const py::dict &data, int request_id) {
+int TdApi::ReqQryTrade(const nb::dict &data, int request_id) {
     CThostFtdcQryTradeField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.ExchangeID, data, "ExchangeID", sizeof(request.ExchangeID));
     set_str_field(request.TradeID, data, "TradeID", sizeof(request.TradeID));
     set_str_field(request.TradeTimeStart, data, "TradeTimeStart", sizeof(request.TradeTimeStart));
     set_str_field(request.TradeTimeEnd, data, "TradeTimeEnd", sizeof(request.TradeTimeEnd));
     set_str_field(request.InvestUnitID, data, "InvestUnitID", sizeof(request.InvestUnitID));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     return api_->ReqQryTrade(&request, request_id);
 }
 
-int TdApi::ReqQryInvestorPosition(const py::dict &data, int request_id) {
+int TdApi::ReqQryInvestorPosition(const nb::dict &data, int request_id) {
     CThostFtdcQryInvestorPositionField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.ExchangeID, data, "ExchangeID", sizeof(request.ExchangeID));
     set_str_field(request.InvestUnitID, data, "InvestUnitID", sizeof(request.InvestUnitID));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     return api_->ReqQryInvestorPosition(&request, request_id);
 }
 
-int TdApi::ReqQryTradingAccount(const py::dict &data, int request_id) {
+int TdApi::ReqQryTradingAccount(const nb::dict &data, int request_id) {
     CThostFtdcQryTradingAccountField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.CurrencyID, data, "CurrencyID", sizeof(request.CurrencyID));
     set_char_field(request.BizType, data, "BizType");
     set_str_field(request.AccountID, data, "AccountID", sizeof(request.AccountID));
     return api_->ReqQryTradingAccount(&request, request_id);
 }
 
-int TdApi::ReqQryInstrument(const py::dict &data, int request_id) {
+int TdApi::ReqQryInstrument(const nb::dict &data, int request_id) {
     CThostFtdcQryInstrumentField request{};
     set_str_field(request.ExchangeID, data, "ExchangeID", sizeof(request.ExchangeID));
     set_str_field(request.InstrumentID, data, "InstrumentID", sizeof(request.InstrumentID));
     set_str_field(request.ExchangeInstID, data, "ExchangeInstID", sizeof(request.ExchangeInstID));
     set_str_field(request.ProductID, data, "ProductID", sizeof(request.ProductID));
     return api_->ReqQryInstrument(&request, request_id);
 }
 
-int TdApi::ReqQrySettlementInfo(const py::dict &data, int request_id) {
+int TdApi::ReqQrySettlementInfo(const nb::dict &data, int request_id) {
     CThostFtdcQrySettlementInfoField request{};
     set_str_field(request.BrokerID, data, "BrokerID", sizeof(request.BrokerID));
     set_str_field(request.InvestorID, data, "InvestorID", sizeof(request.InvestorID));
     set_str_field(request.TradingDay, data, "TradingDay", sizeof(request.TradingDay));
     set_str_field(request.AccountID, data, "AccountID", sizeof(request.AccountID));
     set_str_field(request.CurrencyID, data, "CurrencyID", sizeof(request.CurrencyID));
     return api_->ReqQrySettlementInfo(&request, request_id);
 }
 
 void TdApi::OnFrontConnected() {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnFrontConnected();
     });
 }
 
 void TdApi::OnFrontDisconnected(int reason) {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnFrontDisconnected(reason);
     });
 }
 
 void TdApi::OnHeartBeatWarning(int time_lapse) {
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
+        nb::gil_scoped_acquire acquire;
         PyOnHeartBeatWarning(time_lapse);
     });
 }
 
 void TdApi::OnRspAuthenticate(CThostFtdcRspAuthenticateField *data, CThostFtdcRspInfoField *error, int request_id, bool is_last) {
     CThostFtdcRspAuthenticateField rsp_data{};
     bool has_data = false;
@@ -250,24 +250,24 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["UserProductInfo"] = gbk_to_utf8(rsp_data.UserProductInfo);
             py_data["AppID"] = gbk_to_utf8(rsp_data.AppID);
             py_data["AppType"] = rsp_data.AppType;
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspAuthenticate(py_data, py_error, request_id, is_last);
     });
 }
@@ -282,16 +282,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["TradingDay"] = gbk_to_utf8(rsp_data.TradingDay);
             py_data["LoginTime"] = gbk_to_utf8(rsp_data.LoginTime);
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["SystemName"] = gbk_to_utf8(rsp_data.SystemName);
             py_data["FrontID"] = rsp_data.FrontID;
@@ -301,15 +301,15 @@
             py_data["DCETime"] = gbk_to_utf8(rsp_data.DCETime);
             py_data["CZCETime"] = gbk_to_utf8(rsp_data.CZCETime);
             py_data["FFEXTime"] = gbk_to_utf8(rsp_data.FFEXTime);
             py_data["INETime"] = gbk_to_utf8(rsp_data.INETime);
             py_data["SysVersion"] = gbk_to_utf8(rsp_data.SysVersion);
             py_data["GFEXTime"] = gbk_to_utf8(rsp_data.GFEXTime);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspUserLogin(py_data, py_error, request_id, is_last);
     });
 }
@@ -324,21 +324,21 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspUserLogout(py_data, py_error, request_id, is_last);
     });
 }
@@ -353,16 +353,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["OrderPriceType"] = rsp_data.OrderPriceType;
             py_data["Direction"] = rsp_data.Direction;
@@ -387,15 +387,15 @@
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["CurrencyID"] = gbk_to_utf8(rsp_data.CurrencyID);
             py_data["ClientID"] = gbk_to_utf8(rsp_data.ClientID);
             py_data["MacAddress"] = gbk_to_utf8(rsp_data.MacAddress);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["IPAddress"] = gbk_to_utf8(rsp_data.IPAddress);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspOrderInsert(py_data, py_error, request_id, is_last);
     });
 }
@@ -410,16 +410,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderActionRef"] = rsp_data.OrderActionRef;
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["RequestID"] = rsp_data.RequestID;
             py_data["FrontID"] = rsp_data.FrontID;
@@ -431,15 +431,15 @@
             py_data["VolumeChange"] = rsp_data.VolumeChange;
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["InvestUnitID"] = gbk_to_utf8(rsp_data.InvestUnitID);
             py_data["MacAddress"] = gbk_to_utf8(rsp_data.MacAddress);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["IPAddress"] = gbk_to_utf8(rsp_data.IPAddress);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspOrderAction(py_data, py_error, request_id, is_last);
     });
 }
@@ -454,26 +454,26 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["ConfirmDate"] = gbk_to_utf8(rsp_data.ConfirmDate);
             py_data["ConfirmTime"] = gbk_to_utf8(rsp_data.ConfirmTime);
             py_data["SettlementID"] = rsp_data.SettlementID;
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["CurrencyID"] = gbk_to_utf8(rsp_data.CurrencyID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspSettlementInfoConfirm(py_data, py_error, request_id, is_last);
     });
 }
@@ -488,16 +488,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["OrderPriceType"] = rsp_data.OrderPriceType;
             py_data["Direction"] = rsp_data.Direction;
@@ -555,15 +555,15 @@
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["CurrencyID"] = gbk_to_utf8(rsp_data.CurrencyID);
             py_data["MacAddress"] = gbk_to_utf8(rsp_data.MacAddress);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["ExchangeInstID"] = gbk_to_utf8(rsp_data.ExchangeInstID);
             py_data["IPAddress"] = gbk_to_utf8(rsp_data.IPAddress);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQryOrder(py_data, py_error, request_id, is_last);
     });
 }
@@ -578,16 +578,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["ExchangeID"] = gbk_to_utf8(rsp_data.ExchangeID);
             py_data["TradeID"] = gbk_to_utf8(rsp_data.TradeID);
@@ -613,15 +613,15 @@
             py_data["SettlementID"] = rsp_data.SettlementID;
             py_data["BrokerOrderSeq"] = rsp_data.BrokerOrderSeq;
             py_data["TradeSource"] = rsp_data.TradeSource;
             py_data["InvestUnitID"] = gbk_to_utf8(rsp_data.InvestUnitID);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["ExchangeInstID"] = gbk_to_utf8(rsp_data.ExchangeInstID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQryTrade(py_data, py_error, request_id, is_last);
     });
 }
@@ -636,16 +636,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["PosiDirection"] = rsp_data.PosiDirection;
             py_data["HedgeFlag"] = rsp_data.HedgeFlag;
             py_data["PositionDate"] = rsp_data.PositionDate;
             py_data["YdPosition"] = rsp_data.YdPosition;
@@ -689,15 +689,15 @@
             py_data["YdStrikeFrozen"] = rsp_data.YdStrikeFrozen;
             py_data["InvestUnitID"] = gbk_to_utf8(rsp_data.InvestUnitID);
             py_data["PositionCostOffset"] = rsp_data.PositionCostOffset;
             py_data["TasPosition"] = rsp_data.TasPosition;
             py_data["TasPositionCost"] = rsp_data.TasPositionCost;
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQryInvestorPosition(py_data, py_error, request_id, is_last);
     });
 }
@@ -712,16 +712,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["PreMortgage"] = rsp_data.PreMortgage;
             py_data["PreCredit"] = rsp_data.PreCredit;
             py_data["PreDeposit"] = rsp_data.PreDeposit;
             py_data["PreBalance"] = rsp_data.PreBalance;
@@ -765,15 +765,15 @@
             py_data["SpecProductCloseProfit"] = rsp_data.SpecProductCloseProfit;
             py_data["SpecProductPositionProfitByAlg"] = rsp_data.SpecProductPositionProfitByAlg;
             py_data["SpecProductExchangeMargin"] = rsp_data.SpecProductExchangeMargin;
             py_data["BizType"] = rsp_data.BizType;
             py_data["FrozenSwap"] = rsp_data.FrozenSwap;
             py_data["RemainSwap"] = rsp_data.RemainSwap;
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQryTradingAccount(py_data, py_error, request_id, is_last);
     });
 }
@@ -788,16 +788,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["ExchangeID"] = gbk_to_utf8(rsp_data.ExchangeID);
             py_data["InstrumentName"] = gbk_to_utf8(rsp_data.InstrumentName);
             py_data["ProductClass"] = rsp_data.ProductClass;
             py_data["DeliveryYear"] = rsp_data.DeliveryYear;
             py_data["DeliveryMonth"] = rsp_data.DeliveryMonth;
             py_data["MaxMarketOrderVolume"] = rsp_data.MaxMarketOrderVolume;
@@ -823,15 +823,15 @@
             py_data["UnderlyingMultiple"] = rsp_data.UnderlyingMultiple;
             py_data["CombinationType"] = rsp_data.CombinationType;
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["ExchangeInstID"] = gbk_to_utf8(rsp_data.ExchangeInstID);
             py_data["ProductID"] = gbk_to_utf8(rsp_data.ProductID);
             py_data["UnderlyingInstrID"] = gbk_to_utf8(rsp_data.UnderlyingInstrID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQryInstrument(py_data, py_error, request_id, is_last);
     });
 }
@@ -846,27 +846,27 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["TradingDay"] = gbk_to_utf8(rsp_data.TradingDay);
             py_data["SettlementID"] = rsp_data.SettlementID;
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["SequenceNo"] = rsp_data.SequenceNo;
-            py_data["Content"] = py::bytes(rsp_data.Content);
+            py_data["Content"] = nb::bytes(rsp_data.Content);
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["CurrencyID"] = gbk_to_utf8(rsp_data.CurrencyID);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspQrySettlementInfo(py_data, py_error, request_id, is_last);
     });
 }
@@ -875,16 +875,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_error;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnRspError(py_error, request_id, is_last);
     });
 }
@@ -893,16 +893,16 @@
     CThostFtdcOrderField rsp_data{};
     bool has_data = false;
     if (data) {
         rsp_data = *data;
         has_data = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["OrderPriceType"] = rsp_data.OrderPriceType;
             py_data["Direction"] = rsp_data.Direction;
@@ -972,16 +972,16 @@
     CThostFtdcTradeField rsp_data{};
     bool has_data = false;
     if (data) {
         rsp_data = *data;
         has_data = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["ExchangeID"] = gbk_to_utf8(rsp_data.ExchangeID);
             py_data["TradeID"] = gbk_to_utf8(rsp_data.TradeID);
@@ -1025,16 +1025,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["UserID"] = gbk_to_utf8(rsp_data.UserID);
             py_data["OrderPriceType"] = rsp_data.OrderPriceType;
             py_data["Direction"] = rsp_data.Direction;
@@ -1059,15 +1059,15 @@
             py_data["AccountID"] = gbk_to_utf8(rsp_data.AccountID);
             py_data["CurrencyID"] = gbk_to_utf8(rsp_data.CurrencyID);
             py_data["ClientID"] = gbk_to_utf8(rsp_data.ClientID);
             py_data["MacAddress"] = gbk_to_utf8(rsp_data.MacAddress);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["IPAddress"] = gbk_to_utf8(rsp_data.IPAddress);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnErrRtnOrderInsert(py_data, py_error);
     });
 }
@@ -1082,16 +1082,16 @@
     CThostFtdcRspInfoField rsp_error{};
     bool has_error = false;
     if (error) {
         rsp_error = *error;
         has_error = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["BrokerID"] = gbk_to_utf8(rsp_data.BrokerID);
             py_data["InvestorID"] = gbk_to_utf8(rsp_data.InvestorID);
             py_data["OrderActionRef"] = rsp_data.OrderActionRef;
             py_data["OrderRef"] = gbk_to_utf8(rsp_data.OrderRef);
             py_data["RequestID"] = rsp_data.RequestID;
             py_data["FrontID"] = rsp_data.FrontID;
@@ -1115,15 +1115,15 @@
             py_data["StatusMsg"] = gbk_to_utf8(rsp_data.StatusMsg);
             py_data["BranchID"] = gbk_to_utf8(rsp_data.BranchID);
             py_data["InvestUnitID"] = gbk_to_utf8(rsp_data.InvestUnitID);
             py_data["MacAddress"] = gbk_to_utf8(rsp_data.MacAddress);
             py_data["InstrumentID"] = gbk_to_utf8(rsp_data.InstrumentID);
             py_data["IPAddress"] = gbk_to_utf8(rsp_data.IPAddress);
         }
-        py::dict py_error;
+        nb::dict py_error;
         if (has_error) {
             py_error["ErrorID"] = rsp_error.ErrorID;
             py_error["ErrorMsg"] = gbk_to_utf8(rsp_error.ErrorMsg);
         }
         PyOnErrRtnOrderAction(py_data, py_error);
     });
 }
@@ -1132,16 +1132,16 @@
     CThostFtdcInstrumentStatusField rsp_data{};
     bool has_data = false;
     if (data) {
         rsp_data = *data;
         has_data = true;
     }
     queue_->dispatch([=]() {
-        py::gil_scoped_acquire acquire;
-        py::dict py_data;
+        nb::gil_scoped_acquire acquire;
+        nb::dict py_data;
         if (has_data) {
             py_data["ExchangeID"] = gbk_to_utf8(rsp_data.ExchangeID);
             py_data["SettlementGroupID"] = gbk_to_utf8(rsp_data.SettlementGroupID);
             py_data["InstrumentStatus"] = rsp_data.InstrumentStatus;
             py_data["TradingSegmentSN"] = rsp_data.TradingSegmentSN;
             py_data["EnterTime"] = gbk_to_utf8(rsp_data.EnterTime);
             py_data["EnterReason"] = rsp_data.EnterReason;
```

### Comparing `qtl-ctp-api-6.6.9.3/src/utils.h` & `qtl-ctp-api-6.6.9.4/src/utils.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #ifndef UTILS_H
 #define UTILS_H
 
 #include <string>
 #include <codecvt>
 #include <locale>
 #include <limits>
-#include <pybind11/pybind11.h>
+#include <vector>
+#include <nanobind/nanobind.h>
+#include <nanobind/stl/string.h>
 
 
-namespace py = pybind11;
+namespace nb = nanobind;
 
 
 inline std::string gbk_to_utf8(const std::string& gbk) {
     static const std::locale loc("zh_CN.GBK");
 
     std::vector<wchar_t> wstr(gbk.size());
     wchar_t* wstr_end = nullptr;
@@ -33,32 +35,41 @@
 template <class NumberType>
 inline NumberType adjust_number(NumberType number) {
     NumberType ret = number;
     if (number >= std::numeric_limits<NumberType>::max() - NumberType(1e-6)) ret = NumberType(0);
     return ret;
 }
 
-inline void set_str_field(char *field, const py::dict &input, const char *field_name, size_t size) {
-    if (input.contains(field_name)) {
-        strncpy(field, input[field_name].cast<std::string>().c_str(), size);
+inline bool contains(const nb::dict &d, const std::string &k) {
+    for (auto i: d) {
+        if (nb::cast<std::string>(i.first) == k) {
+            return true;
+        }
     }
+    return false;
 }
 
-inline void set_char_field(char &field, const py::dict &input, const char *field_name) {
-    if (input.contains(field_name)) {
-        field = input[field_name].cast<char>();
+inline void set_str_field(char *field, const nb::dict &input, const char *field_name, size_t size) {
+    if (contains(input, field_name)) {
+        strncpy(field, nb::cast<std::string>(input[field_name]).c_str(), size);
     }
 }
 
-inline void set_int_field(int &field, const py::dict &input, const char *field_name) {
-    if (input.contains(field_name)) {
-        field = input[field_name].cast<int>();
+inline void set_char_field(char &field, const nb::dict &input, const char *field_name) {
+    if (contains(input, field_name)) {
+        field = nb::cast<int>(input[field_name]);  // todo
     }
 }
 
-inline void set_double_field(double &field, const py::dict &input, const char *field_name) {
-    if (input.contains(field_name)) {
-        field = input[field_name].cast<double>();
+inline void set_int_field(int &field, const nb::dict &input, const char *field_name) {
+    if (contains(input, field_name)) {
+        field = nb::cast<int>(input[field_name]);
+    }
+}
+
+inline void set_double_field(double &field, const nb::dict &input, const char *field_name) {
+    if (contains(input, field_name)) {
+        field = nb::cast<double>(input[field_name]);
     }
 }
 
 #endif //UTILS_H
```

### Comparing `qtl-ctp-api-6.6.9.3/tests/test_md.py` & `qtl-ctp-api-6.6.9.4/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `qtl-ctp-api-6.6.9.3/tests/test_td.py` & `qtl-ctp-api-6.6.9.4/tests/test_td.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,16 @@
 
 def test():
     print('test TdApi...')
     print(f'version: {TdApi.GetApiVersion()}')
     settings = {
         'address': 'tcp://180.168.146.187:10201',
         'broker_id': '9999',
-        'user_id': '',
-        'password': '',
+        'user_id': '113635',
+        'password': 'da20200925',
         'flow_path': 'flow',
         'app_id': 'simnow_client_test',
         'auth_code': '0000000000000000',
     }
 
     td_api = PyTdApi(settings)
     td_api.connect()
```

