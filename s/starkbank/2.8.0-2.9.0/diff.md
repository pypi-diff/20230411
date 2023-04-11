# Comparing `tmp/starkbank-2.8.0.tar.gz` & `tmp/starkbank-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starkbank-2.8.0.tar", last modified: Tue Mar  9 14:48:48 2021, max compression
+gzip compressed data, was "dist/starkbank-2.9.0.tar", last modified: Mon Mar 22 17:49:41 2021, max compression
```

## Comparing `starkbank-2.8.0.tar` & `starkbank-2.9.0.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/
--rw-r--r--   0 caiodottori   (502) staff       (20)    49137 2021-03-09 14:48:48.000000 starkbank-2.8.0/PKG-INFO
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/webhook/
--rw-r--r--   0 caiodottori   (502) staff       (20)     4434 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/webhook/__webhook.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       56 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/webhook/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/brcodepreview/
--rw-r--r--   0 caiodottori   (502) staff       (20)       35 2020-11-16 20:03:30.000000 starkbank-2.8.0/starkbank/brcodepreview/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     2454 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/brcodepreview/__brcodepreview.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/transaction/
--rw-r--r--   0 caiodottori   (502) staff       (20)       52 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transaction/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     7288 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transaction/__transaction.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/deposit/
--rw-r--r--   0 caiodottori   (502) staff       (20)     6415 2021-02-04 17:54:28.000000 starkbank-2.8.0/starkbank/deposit/__deposit.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       85 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/deposit/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/deposit/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     4824 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/deposit/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/deposit/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      870 2021-03-09 14:36:51.000000 starkbank-2.8.0/starkbank/error.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boleto/
--rw-r--r--   0 caiodottori   (502) staff       (20)     9839 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boleto/__boleto.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      105 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boleto/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boleto/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     4785 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boleto/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boleto/log/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boletopayment/
--rw-r--r--   0 caiodottori   (502) staff       (20)      112 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletopayment/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boletopayment/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     5016 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletopayment/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletopayment/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     8055 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletopayment/__boletopayment.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      909 2020-06-03 21:10:23.000000 starkbank-2.8.0/starkbank/key.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/workspace/
--rw-r--r--   0 caiodottori   (502) staff       (20)       50 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/workspace/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     4887 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/workspace/__workspace.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/transfer/
--rw-r--r--   0 caiodottori   (502) staff       (20)      107 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transfer/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/transfer/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     4828 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transfer/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transfer/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)    10209 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/transfer/__transfer.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     1341 2021-03-09 14:39:07.000000 starkbank-2.8.0/starkbank/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/balance/
--rw-r--r--   0 caiodottori   (502) staff       (20)       27 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/balance/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     1628 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/balance/__balance.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/utils/
--rw-r--r--   0 caiodottori   (502) staff       (20)      166 2021-03-08 17:24:35.000000 starkbank-2.8.0/starkbank/utils/compatibility.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     2563 2021-01-12 16:22:24.000000 starkbank-2.8.0/starkbank/utils/checks.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     2979 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/utils/rest.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     2370 2021-03-08 21:00:12.000000 starkbank-2.8.0/starkbank/utils/request.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       12 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/utils/cache.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      319 2021-02-01 15:43:18.000000 starkbank-2.8.0/starkbank/utils/resource.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      183 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/utils/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      459 2021-03-08 17:24:35.000000 starkbank-2.8.0/starkbank/utils/url.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     1996 2020-11-16 20:03:30.000000 starkbank-2.8.0/starkbank/utils/api.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      340 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/utils/case.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      264 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/utils/enum.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      614 2021-02-01 15:43:18.000000 starkbank-2.8.0/starkbank/utils/subresource.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/user/
--rw-r--r--   0 caiodottori   (502) staff       (20)     2810 2021-02-01 15:43:18.000000 starkbank-2.8.0/starkbank/user/__organization.py
--rw-r--r--   0 caiodottori   (502) staff       (20)        0 2020-04-15 02:14:50.000000 starkbank-2.8.0/starkbank/user/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      463 2021-01-14 17:28:27.000000 starkbank-2.8.0/starkbank/user/__user.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     1924 2021-02-01 15:43:18.000000 starkbank-2.8.0/starkbank/user/__project.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/utilitypayment/
--rw-r--r--   0 caiodottori   (502) staff       (20)      113 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/utilitypayment/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/utilitypayment/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     5034 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/utilitypayment/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/utilitypayment/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     7920 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/utilitypayment/__utilitypayment.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/brcodepayment/
--rw-r--r--   0 caiodottori   (502) staff       (20)     8587 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/brcodepayment/__brcodepayment.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      112 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/brcodepayment/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/brcodepayment/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     5012 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/brcodepayment/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/brcodepayment/log/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boletoholmes/
--rw-r--r--   0 caiodottori   (502) staff       (20)       98 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletoholmes/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     5339 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletoholmes/__boletoholmes.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/boletoholmes/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     4859 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletoholmes/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/boletoholmes/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)      111 2021-03-08 21:00:12.000000 starkbank-2.8.0/starkbank/environment.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/dictkey/
--rw-r--r--   0 caiodottori   (502) staff       (20)     6467 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/dictkey/__dictkey.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       40 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/dictkey/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/event/
--rw-r--r--   0 caiodottori   (502) staff       (20)       61 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/event/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     9441 2021-03-08 17:24:35.000000 starkbank-2.8.0/starkbank/event/__event.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/paymentrequest/
--rw-r--r--   0 caiodottori   (502) staff       (20)     9658 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/paymentrequest/__paymentrequest.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       50 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/paymentrequest/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/invoice/
--rw-r--r--   0 caiodottori   (502) staff       (20)      154 2021-02-03 14:47:12.000000 starkbank-2.8.0/starkbank/invoice/__init__.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank/invoice/log/
--rw-r--r--   0 caiodottori   (502) staff       (20)     5399 2021-02-23 15:18:37.000000 starkbank-2.8.0/starkbank/invoice/log/__log.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       41 2021-02-23 15:18:37.000000 starkbank-2.8.0/starkbank/invoice/log/__init__.py
--rw-r--r--   0 caiodottori   (502) staff       (20)     1485 2021-02-01 15:43:18.000000 starkbank-2.8.0/starkbank/invoice/__payment.py
--rw-r--r--   0 caiodottori   (502) staff       (20)    12076 2021-03-08 17:33:17.000000 starkbank-2.8.0/starkbank/invoice/__invoice.py
-drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/
--rw-r--r--   0 caiodottori   (502) staff       (20)    49137 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (502) staff       (20)     2416 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (502) staff       (20)       40 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (502) staff       (20)       16 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/top_level.txt
--rw-r--r--   0 caiodottori   (502) staff       (20)        1 2021-03-09 14:48:48.000000 starkbank-2.8.0/starkbank.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (502) staff       (20)       49 2020-04-15 02:14:50.000000 starkbank-2.8.0/MANIFEST.in
--rw-r--r--   0 caiodottori   (502) staff       (20)    36356 2021-02-23 15:18:37.000000 starkbank-2.8.0/README.md
--rw-r--r--   0 caiodottori   (502) staff       (20)      838 2020-11-26 16:38:57.000000 starkbank-2.8.0/setup.py
--rw-r--r--   0 caiodottori   (502) staff       (20)       38 2021-03-09 14:48:48.000000 starkbank-2.8.0/setup.cfg
--rw-r--r--   0 caiodottori   (502) staff       (20)     1067 2020-04-15 02:14:50.000000 starkbank-2.8.0/LICENSE.txt
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/
+-rw-r--r--   0 caiodottori   (502) staff       (20)    49895 2021-03-22 17:49:41.000000 starkbank-2.9.0/PKG-INFO
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/webhook/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4434 2021-03-12 14:37:45.000000 starkbank-2.9.0/starkbank/webhook/__webhook.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       56 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/webhook/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/brcodepreview/
+-rw-r--r--   0 caiodottori   (502) staff       (20)       35 2020-11-16 20:03:30.000000 starkbank-2.9.0/starkbank/brcodepreview/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2454 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/brcodepreview/__brcodepreview.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/transaction/
+-rw-r--r--   0 caiodottori   (502) staff       (20)       52 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/transaction/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     7288 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/transaction/__transaction.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/deposit/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     6415 2021-02-04 17:54:28.000000 starkbank-2.9.0/starkbank/deposit/__deposit.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       85 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/deposit/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/deposit/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4824 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/deposit/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/deposit/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      870 2021-03-09 14:36:51.000000 starkbank-2.9.0/starkbank/error.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boleto/
+-rw-r--r--   0 caiodottori   (502) staff       (20)    10018 2021-03-22 16:56:31.000000 starkbank-2.9.0/starkbank/boleto/__boleto.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      105 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boleto/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boleto/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4785 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boleto/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boleto/log/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boletopayment/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      112 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletopayment/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boletopayment/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     5016 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletopayment/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletopayment/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     8055 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletopayment/__boletopayment.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      909 2020-06-03 21:10:23.000000 starkbank-2.9.0/starkbank/key.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/workspace/
+-rw-r--r--   0 caiodottori   (502) staff       (20)       50 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/workspace/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4887 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/workspace/__workspace.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/transfer/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      107 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/transfer/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/transfer/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4828 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/transfer/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/transfer/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)    10462 2021-03-22 16:57:48.000000 starkbank-2.9.0/starkbank/transfer/__transfer.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     1341 2021-03-22 16:59:12.000000 starkbank-2.9.0/starkbank/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/balance/
+-rw-r--r--   0 caiodottori   (502) staff       (20)       27 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/balance/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     1628 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/balance/__balance.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/utils/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      166 2021-03-08 17:24:35.000000 starkbank-2.9.0/starkbank/utils/compatibility.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2563 2021-01-12 16:22:24.000000 starkbank-2.9.0/starkbank/utils/checks.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     3357 2021-03-22 14:48:22.000000 starkbank-2.9.0/starkbank/utils/rest.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2370 2021-03-22 14:45:41.000000 starkbank-2.9.0/starkbank/utils/request.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       12 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/utils/cache.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      319 2021-02-01 15:43:18.000000 starkbank-2.9.0/starkbank/utils/resource.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      183 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/utils/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      459 2021-03-08 17:24:35.000000 starkbank-2.9.0/starkbank/utils/url.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2028 2021-03-22 14:48:22.000000 starkbank-2.9.0/starkbank/utils/api.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      340 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/utils/case.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      264 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/utils/enum.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      614 2021-02-01 15:43:18.000000 starkbank-2.9.0/starkbank/utils/subresource.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/user/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2810 2021-02-01 15:43:18.000000 starkbank-2.9.0/starkbank/user/__organization.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)        0 2020-04-15 02:14:50.000000 starkbank-2.9.0/starkbank/user/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      463 2021-01-14 17:28:27.000000 starkbank-2.9.0/starkbank/user/__user.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     1924 2021-02-01 15:43:18.000000 starkbank-2.9.0/starkbank/user/__project.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/utilitypayment/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      113 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/utilitypayment/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/utilitypayment/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     5034 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/utilitypayment/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/utilitypayment/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     7920 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/utilitypayment/__utilitypayment.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/brcodepayment/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     8587 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/brcodepayment/__brcodepayment.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      112 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/brcodepayment/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/brcodepayment/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     5012 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/brcodepayment/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/brcodepayment/log/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boletoholmes/
+-rw-r--r--   0 caiodottori   (502) staff       (20)       98 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletoholmes/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     5339 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletoholmes/__boletoholmes.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/boletoholmes/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4859 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletoholmes/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       36 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/boletoholmes/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)      111 2021-03-22 14:45:41.000000 starkbank-2.9.0/starkbank/environment.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/dictkey/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     6467 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/dictkey/__dictkey.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       40 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/dictkey/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/event/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      122 2021-03-22 14:48:22.000000 starkbank-2.9.0/starkbank/event/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     9441 2021-03-12 22:14:25.000000 starkbank-2.9.0/starkbank/event/__event.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/event/attempt/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     4965 2021-03-22 14:48:22.000000 starkbank-2.9.0/starkbank/event/attempt/__attempt.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       40 2021-03-22 14:48:22.000000 starkbank-2.9.0/starkbank/event/attempt/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/paymentrequest/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     9658 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/paymentrequest/__paymentrequest.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       50 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/paymentrequest/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/invoice/
+-rw-r--r--   0 caiodottori   (502) staff       (20)      154 2021-02-03 14:47:12.000000 starkbank-2.9.0/starkbank/invoice/__init__.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank/invoice/log/
+-rw-r--r--   0 caiodottori   (502) staff       (20)     5399 2021-02-23 15:18:37.000000 starkbank-2.9.0/starkbank/invoice/log/__log.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       41 2021-02-23 15:18:37.000000 starkbank-2.9.0/starkbank/invoice/log/__init__.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)     1485 2021-02-01 15:43:18.000000 starkbank-2.9.0/starkbank/invoice/__payment.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)    12076 2021-03-08 17:33:17.000000 starkbank-2.9.0/starkbank/invoice/__invoice.py
+drwxr-xr-x   0 caiodottori   (502) staff       (20)        0 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/
+-rw-r--r--   0 caiodottori   (502) staff       (20)    49895 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (502) staff       (20)     2489 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (502) staff       (20)       40 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (502) staff       (20)       16 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/top_level.txt
+-rw-r--r--   0 caiodottori   (502) staff       (20)        1 2021-03-22 17:49:41.000000 starkbank-2.9.0/starkbank.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (502) staff       (20)       49 2020-04-15 02:14:50.000000 starkbank-2.9.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (502) staff       (20)    36906 2021-03-22 14:48:22.000000 starkbank-2.9.0/README.md
+-rw-r--r--   0 caiodottori   (502) staff       (20)      838 2020-11-26 16:38:57.000000 starkbank-2.9.0/setup.py
+-rw-r--r--   0 caiodottori   (502) staff       (20)       38 2021-03-22 17:49:41.000000 starkbank-2.9.0/setup.cfg
+-rw-r--r--   0 caiodottori   (502) staff       (20)     1067 2020-04-15 02:14:50.000000 starkbank-2.9.0/LICENSE.txt
```

### Comparing `starkbank-2.8.0/PKG-INFO` & `starkbank-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkbank
-Version: 2.8.0
+Version: 2.9.0
 Summary: SDK to facilitate Python integrations with Stark Bank
 Home-page: https://github.com/starkbank/sdk-python
 Author: Stark Bank
 Author-email: developers@starkbank.com
 License: MIT License
 Description: # Stark Bank Python SDK
         
@@ -1403,15 +1403,15 @@
         
         events = starkbank.event.query(after="2020-03-20", is_delivered=False)
         
         for event in events:
             print(event)
         ```
         
-        ### Get webhook event
+        ### Get a webhook event
         
         You can get a specific webhook event by its id.
         
         ```python
         import starkbank
         
         event = starkbank.event.get("10827361982368179")
@@ -1441,14 +1441,40 @@
         import starkbank
         
         event = starkbank.event.update(id="129837198237192", is_delivered=True)
         
         print(event)
         ```
         
+        ### Query failed webhook event delivery attempts information
+        
+        You can also get information on failed webhook event delivery attempts.
+        
+        ```python
+        import starkbank
+        
+        attempts = starkbank.event.attempt.query(after="2020-03-20")
+        
+        for attempt in attempts:
+            print(attempt.code)
+            print(attempt.message)
+        ```
+        
+        ### Get a failed webhook event delivery attempt information
+        
+        To retrieve information on a single attempt, use the following function:
+        
+        ```python
+        import starkbank
+        
+        attempt = starkbank.event.attempt.get("1616161616161616")
+        
+        print(attempt)
+        ```
+        
         ### Get DICT key
         
         You can get the Pix key's parameters by its id.
         
         ```python
         import starkbank
```

### Comparing `starkbank-2.8.0/starkbank/webhook/__webhook.py` & `starkbank-2.9.0/starkbank/webhook/__webhook.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/brcodepreview/__brcodepreview.py` & `starkbank-2.9.0/starkbank/brcodepreview/__brcodepreview.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/transaction/__transaction.py` & `starkbank-2.9.0/starkbank/transaction/__transaction.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/deposit/__deposit.py` & `starkbank-2.9.0/starkbank/deposit/__deposit.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/deposit/log/__log.py` & `starkbank-2.9.0/starkbank/deposit/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/error.py` & `starkbank-2.9.0/starkbank/error.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/boleto/__boleto.py` & `starkbank-2.9.0/starkbank/boleto/__boleto.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,23 @@
     - receiver_tax_id [string]: receiver (Sacador Avalista) tax ID (CPF or CNPJ) with or without formatting. ex: "01234567890" or "20.018.183/0001-80"
     ## Attributes (return-only):
     - id [string, default None]: unique id returned when Boleto is created. ex: "5656565656565656"
     - fee [integer, default None]: fee charged when Boleto is paid. ex: 200 (= R$ 2.00)
     - line [string, default None]: generated Boleto line for payment. ex: "34191.09008 63571.277308 71444.640008 5 81960000000062"
     - bar_code [string, default None]: generated Boleto bar-code for payment. ex: "34195819600000000621090063571277307144464000"
     - status [string, default None]: current Boleto status. ex: "registered" or "paid"
+    - transaction_ids [list of strings]: ledger transaction ids linked to this boleto. ex: ["19827356981273"]
     - created [datetime.datetime, default None]: creation datetime for the Boleto. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - our_number [string, default None]: Reference number registered at the settlement bank. ex:"10131474"
     """
 
     def __init__(self, amount, name, tax_id, street_line_1, street_line_2, district, city, state_code, zip_code,
                  due=None, fine=None, interest=None, overdue_limit=None, tags=None, descriptions=None, discounts=None,
                  receiver_name=None, receiver_tax_id=None, id=None, fee=None, line=None, bar_code=None, status=None,
-                 created=None, our_number=None):
+                 transaction_ids=None, created=None, our_number=None):
         Resource.__init__(self, id=id)
 
         self.amount = amount
         self.fee = fee
         self.name = name
         self.tax_id = tax_id
         self.street_line_1 = street_line_1
@@ -62,14 +63,15 @@
         self.overdue_limit = overdue_limit
         self.tags = tags
         self.descriptions = descriptions
         self.discounts = discounts
         self.line = line
         self.bar_code = bar_code
         self.status = status
+        self.transaction_ids = transaction_ids
         self.created = check_datetime(created)
         self.our_number = our_number
 
 
 _resource = {"class": Boleto, "name": "Boleto"}
```

### Comparing `starkbank-2.8.0/starkbank/boleto/log/__log.py` & `starkbank-2.9.0/starkbank/boleto/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/boletopayment/log/__log.py` & `starkbank-2.9.0/starkbank/boletopayment/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/boletopayment/__boletopayment.py` & `starkbank-2.9.0/starkbank/boletopayment/__boletopayment.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/key.py` & `starkbank-2.9.0/starkbank/key.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/workspace/__workspace.py` & `starkbank-2.9.0/starkbank/workspace/__workspace.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/transfer/log/__log.py` & `starkbank-2.9.0/starkbank/transfer/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/transfer/__transfer.py` & `starkbank-2.9.0/starkbank/transfer/__transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,40 @@
     - bank_code [string]: code of the receiver bank institution in Brazil. If an ISPB (8 digits) is informed, a PIX transfer will be created, else a TED will be issued. ex: "20018183" or "341"
     - branch_code [string]: receiver bank account branch. Use '-' in case there is a verifier digit. ex: "1357-9"
     - account_number [string]: receiver bank account number. Use '-' before the verifier digit. ex: "876543-2"
     ## Parameters (optional):
     - account_type [string, default "checking"]: Receiver bank account type. This parameter only has effect on Pix Transfers. ex: "checking", "savings" or "salary"
     - external_id [string, default None]: url safe string that must be unique among all your transfers. Duplicated external_ids will cause failures. By default, this parameter will block any transfer that repeats amount and receiver information on the same date. ex: "my-internal-id-123456"
     - scheduled [datetime.date, datetime.datetime or string, default now]: date or datetime when the transfer will be processed. May be pushed to next business day if necessary. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
+    - description [string, default None]: optional description to override default description to be shown in the bank statement. ex: "Payment for service #1234"
     - tags [list of strings]: list of strings for reference when searching for transfers. ex: ["employees", "monthly"]
     ## Attributes (return-only):
     - id [string, default None]: unique id returned when the transfer is created. ex: "5656565656565656"
     - fee [integer, default None]: fee charged when transfer is created. ex: 200 (= R$ 2.00)
     - status [string, default None]: current transfer status. ex: "success" or "failed"
     - transaction_ids [list of strings, default None]: ledger transaction ids linked to this transfer (if there are two, second is the chargeback). ex: ["19827356981273"]
     - created [datetime.datetime, default None]: creation datetime for the transfer. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     - updated [datetime.datetime, default None]: latest update datetime for the transfer. ex: datetime.datetime(2020, 3, 10, 10, 30, 0, 0)
     """
 
-    def __init__(self, amount, name, tax_id, bank_code, branch_code, account_number, account_type=None, external_id=None, scheduled=None, transaction_ids=None, fee=None, tags=None, status=None, id=None, created=None, updated=None):
+    def __init__(self, amount, name, tax_id, bank_code, branch_code, account_number, account_type=None,
+                 external_id=None, scheduled=None, description=None, transaction_ids=None, fee=None, tags=None,
+                 status=None, id=None, created=None, updated=None):
         Resource.__init__(self, id=id)
 
         self.tax_id = tax_id
         self.amount = amount
         self.name = name
         self.bank_code = bank_code
         self.branch_code = branch_code
         self.account_number = account_number
         self.account_type = account_type
         self.external_id = external_id
         self.scheduled = check_datetime_or_date(scheduled)
+        self.description = description
         self.tags = tags
         self.fee = fee
         self.status = status
         self.created = check_datetime(created)
         self.updated = check_datetime(updated)
         self.transaction_ids = transaction_ids
```

### Comparing `starkbank-2.8.0/starkbank/__init__.py` & `starkbank-2.9.0/starkbank/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = "2.8.0"
+version = "2.9.0"
 
 user = None
 language = "en-US"
 timeout = 15
 
 from .user.__organization import Organization
 from .user.__project import Project
```

### Comparing `starkbank-2.8.0/starkbank/balance/__balance.py` & `starkbank-2.9.0/starkbank/balance/__balance.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/utils/checks.py` & `starkbank-2.9.0/starkbank/utils/checks.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/utils/rest.py` & `starkbank-2.9.0/starkbank/utils/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
 def get_sub_resource(resource, id, sub_resource, user=None, **kwargs):
     path = "{endpoint}/{id}/{sub_resource}".format(endpoint=endpoint(resource), id=id, sub_resource=endpoint(sub_resource))
     entity = fetch(method=get, path=path, query=kwargs, user=user).json()[last_name(sub_resource)]
     return from_api_json(sub_resource, entity)
 
 
+def get_sub_resources(resource, id, sub_resource, user=None, **kwargs):
+    path = "{endpoint}/{id}/{sub_resource}".format(endpoint=endpoint(resource), id=id, sub_resource=endpoint(sub_resource))
+    entities = fetch(method=get, path=path, query=kwargs, user=user).json()[last_name_plural(sub_resource)]
+    return [from_api_json(sub_resource, entity) for entity in entities]
+
+
 def post_multi(resource, entities, user=None):
     json = fetch(method=post, path=endpoint(resource), user=user, payload={
         last_name_plural(resource): [api_json(entity) for entity in entities]
     }).json()
     entities = json[last_name_plural(resource)]
     return [from_api_json(resource, entity) for entity in entities]
```

### Comparing `starkbank-2.8.0/starkbank/utils/request.py` & `starkbank-2.9.0/starkbank/utils/request.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/utils/api.py` & `starkbank-2.9.0/starkbank/utils/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     for param in params - set(snakes):
         snakes[param] = None
 
     return resource["class"](**snakes)
 
 
 def endpoint(resource):
-    return camel_to_kebab(resource["name"]).replace("-log", "/log")
+    return camel_to_kebab(resource["name"]).replace("-log", "/log").replace("-attempt", "/attempt")
 
 
 def last_name(resource):
     return camel_to_kebab(resource["name"]).split("-")[-1]
 
 
 def last_name_plural(resource):
```

### Comparing `starkbank-2.8.0/starkbank/utils/subresource.py` & `starkbank-2.9.0/starkbank/utils/subresource.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/user/__organization.py` & `starkbank-2.9.0/starkbank/user/__organization.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/user/__project.py` & `starkbank-2.9.0/starkbank/user/__project.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/utilitypayment/log/__log.py` & `starkbank-2.9.0/starkbank/utilitypayment/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/utilitypayment/__utilitypayment.py` & `starkbank-2.9.0/starkbank/utilitypayment/__utilitypayment.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/brcodepayment/__brcodepayment.py` & `starkbank-2.9.0/starkbank/brcodepayment/__brcodepayment.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/brcodepayment/log/__log.py` & `starkbank-2.9.0/starkbank/brcodepayment/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/boletoholmes/__boletoholmes.py` & `starkbank-2.9.0/starkbank/boletoholmes/__boletoholmes.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/boletoholmes/log/__log.py` & `starkbank-2.9.0/starkbank/boletoholmes/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/dictkey/__dictkey.py` & `starkbank-2.9.0/starkbank/dictkey/__dictkey.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/event/__event.py` & `starkbank-2.9.0/starkbank/event/__event.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/paymentrequest/__paymentrequest.py` & `starkbank-2.9.0/starkbank/paymentrequest/__paymentrequest.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/invoice/log/__log.py` & `starkbank-2.9.0/starkbank/invoice/log/__log.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/invoice/__payment.py` & `starkbank-2.9.0/starkbank/invoice/__payment.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank/invoice/__invoice.py` & `starkbank-2.9.0/starkbank/invoice/__invoice.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/starkbank.egg-info/PKG-INFO` & `starkbank-2.9.0/starkbank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starkbank
-Version: 2.8.0
+Version: 2.9.0
 Summary: SDK to facilitate Python integrations with Stark Bank
 Home-page: https://github.com/starkbank/sdk-python
 Author: Stark Bank
 Author-email: developers@starkbank.com
 License: MIT License
 Description: # Stark Bank Python SDK
         
@@ -1403,15 +1403,15 @@
         
         events = starkbank.event.query(after="2020-03-20", is_delivered=False)
         
         for event in events:
             print(event)
         ```
         
-        ### Get webhook event
+        ### Get a webhook event
         
         You can get a specific webhook event by its id.
         
         ```python
         import starkbank
         
         event = starkbank.event.get("10827361982368179")
@@ -1441,14 +1441,40 @@
         import starkbank
         
         event = starkbank.event.update(id="129837198237192", is_delivered=True)
         
         print(event)
         ```
         
+        ### Query failed webhook event delivery attempts information
+        
+        You can also get information on failed webhook event delivery attempts.
+        
+        ```python
+        import starkbank
+        
+        attempts = starkbank.event.attempt.query(after="2020-03-20")
+        
+        for attempt in attempts:
+            print(attempt.code)
+            print(attempt.message)
+        ```
+        
+        ### Get a failed webhook event delivery attempt information
+        
+        To retrieve information on a single attempt, use the following function:
+        
+        ```python
+        import starkbank
+        
+        attempt = starkbank.event.attempt.get("1616161616161616")
+        
+        print(attempt)
+        ```
+        
         ### Get DICT key
         
         You can get the Pix key's parameters by its id.
         
         ```python
         import starkbank
```

### Comparing `starkbank-2.8.0/starkbank.egg-info/SOURCES.txt` & `starkbank-2.9.0/starkbank.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 starkbank/deposit/__init__.py
 starkbank/deposit/log/__init__.py
 starkbank/deposit/log/__log.py
 starkbank/dictkey/__dictkey.py
 starkbank/dictkey/__init__.py
 starkbank/event/__event.py
 starkbank/event/__init__.py
+starkbank/event/attempt/__attempt.py
+starkbank/event/attempt/__init__.py
 starkbank/invoice/__init__.py
 starkbank/invoice/__invoice.py
 starkbank/invoice/__payment.py
 starkbank/invoice/log/__init__.py
 starkbank/invoice/log/__log.py
 starkbank/paymentrequest/__init__.py
 starkbank/paymentrequest/__paymentrequest.py
```

### Comparing `starkbank-2.8.0/README.md` & `starkbank-2.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1395,15 +1395,15 @@
 
 events = starkbank.event.query(after="2020-03-20", is_delivered=False)
 
 for event in events:
     print(event)
 ```
 
-### Get webhook event
+### Get a webhook event
 
 You can get a specific webhook event by its id.
 
 ```python
 import starkbank
 
 event = starkbank.event.get("10827361982368179")
@@ -1433,14 +1433,40 @@
 import starkbank
 
 event = starkbank.event.update(id="129837198237192", is_delivered=True)
 
 print(event)
 ```
 
+### Query failed webhook event delivery attempts information
+
+You can also get information on failed webhook event delivery attempts.
+
+```python
+import starkbank
+
+attempts = starkbank.event.attempt.query(after="2020-03-20")
+
+for attempt in attempts:
+    print(attempt.code)
+    print(attempt.message)
+```
+
+### Get a failed webhook event delivery attempt information
+
+To retrieve information on a single attempt, use the following function:
+
+```python
+import starkbank
+
+attempt = starkbank.event.attempt.get("1616161616161616")
+
+print(attempt)
+```
+
 ### Get DICT key
 
 You can get the Pix key's parameters by its id.
 
 ```python
 import starkbank
```

### Comparing `starkbank-2.8.0/setup.py` & `starkbank-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `starkbank-2.8.0/LICENSE.txt` & `starkbank-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

