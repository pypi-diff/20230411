# Comparing `tmp/py4paystack-1.0.2.tar.gz` & `tmp/py4paystack-1.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4paystack-1.0.2.tar", last modified: Tue Apr 11 19:59:35 2023, max compression
+gzip compressed data, was "py4paystack-1.0.2.post1.tar", last modified: Tue Apr 11 20:25:11 2023, max compression
```

## Comparing `py4paystack-1.0.2.tar` & `py4paystack-1.0.2.post1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.077903 py4paystack-1.0.2/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1072 2022-08-15 10:48:48.000000 py4paystack-1.0.2/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)      598 2023-04-11 19:59:35.077903 py4paystack-1.0.2/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)    91188 2023-04-11 19:58:22.000000 py4paystack-1.0.2/README.md
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.061236 py4paystack-1.0.2/py4paystack/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2601 2022-08-15 11:37:18.000000 py4paystack-1.0.2/py4paystack/paystack.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.074569 py4paystack-1.0.2/py4paystack/routes/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1396 2023-03-16 13:40:27.000000 py4paystack-1.0.2/py4paystack/routes/apple_pay.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5516 2023-03-16 13:49:20.000000 py4paystack-1.0.2/py4paystack/routes/bulk_charges.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     9274 2023-03-16 13:51:16.000000 py4paystack-1.0.2/py4paystack/routes/charge.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      892 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/control_panel.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7561 2023-03-16 14:06:02.000000 py4paystack-1.0.2/py4paystack/routes/customer.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8338 2023-03-16 14:06:27.000000 py4paystack-1.0.2/py4paystack/routes/disputes.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10607 2023-03-16 14:06:38.000000 py4paystack-1.0.2/py4paystack/routes/invoices.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-04-11 19:29:58.000000 py4paystack-1.0.2/py4paystack/routes/miscellaneous.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5044 2023-03-16 14:07:00.000000 py4paystack-1.0.2/py4paystack/routes/payment_pages.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5767 2023-03-16 14:07:15.000000 py4paystack-1.0.2/py4paystack/routes/plan.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5289 2023-03-16 14:07:29.000000 py4paystack-1.0.2/py4paystack/routes/product.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-03-16 14:07:37.000000 py4paystack-1.0.2/py4paystack/routes/refund.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3379 2023-04-08 17:19:52.000000 py4paystack-1.0.2/py4paystack/routes/settlement.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7285 2023-03-16 14:08:09.000000 py4paystack-1.0.2/py4paystack/routes/subaccount.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5004 2023-03-16 14:08:34.000000 py4paystack-1.0.2/py4paystack/routes/subscription.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    19913 2023-03-16 14:08:56.000000 py4paystack-1.0.2/py4paystack/routes/transaction.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6434 2023-03-16 14:08:45.000000 py4paystack-1.0.2/py4paystack/routes/transaction_split.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6041 2023-03-16 14:09:20.000000 py4paystack-1.0.2/py4paystack/routes/transfer.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2848 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/transfer_control.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7391 2023-03-16 14:09:07.000000 py4paystack-1.0.2/py4paystack/routes/transfer_recipient.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3043 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/verification.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7473 2023-03-16 14:09:30.000000 py4paystack-1.0.2/py4paystack/routes/virtual_accounts.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.074569 py4paystack-1.0.2/py4paystack/utilities/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/utilities/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1610 2023-03-16 14:59:50.000000 py4paystack-1.0.2/py4paystack/utilities/decorators.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      252 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/utilities/errors.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1473 2023-04-11 19:43:22.000000 py4paystack-1.0.2/py4paystack/utilities/request.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2012 2023-04-10 10:29:15.000000 py4paystack-1.0.2/py4paystack/utilities/settings.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4252 2023-03-16 14:10:10.000000 py4paystack-1.0.2/py4paystack/utilities/util.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.061236 py4paystack-1.0.2/py4paystack.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      598 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1231 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       14 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      103 2023-04-11 19:59:35.081236 py4paystack-1.0.2/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1289 2023-04-11 19:52:20.000000 py4paystack-1.0.2/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 20:25:11.627802 py4paystack-1.0.2.post1/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1072 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    91793 2023-04-11 20:25:11.627802 py4paystack-1.0.2.post1/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    91188 2023-04-11 19:58:22.000000 py4paystack-1.0.2.post1/README.md
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 20:25:11.611135 py4paystack-1.0.2.post1/py4paystack/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2601 2022-08-15 11:37:18.000000 py4paystack-1.0.2.post1/py4paystack/paystack.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 20:25:11.624468 py4paystack-1.0.2.post1/py4paystack/routes/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/routes/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1396 2023-03-16 13:40:27.000000 py4paystack-1.0.2.post1/py4paystack/routes/apple_pay.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5516 2023-03-16 13:49:20.000000 py4paystack-1.0.2.post1/py4paystack/routes/bulk_charges.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     9274 2023-03-16 13:51:16.000000 py4paystack-1.0.2.post1/py4paystack/routes/charge.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      892 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/routes/control_panel.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7561 2023-03-16 14:06:02.000000 py4paystack-1.0.2.post1/py4paystack/routes/customer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8338 2023-03-16 14:06:27.000000 py4paystack-1.0.2.post1/py4paystack/routes/disputes.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    10607 2023-03-16 14:06:38.000000 py4paystack-1.0.2.post1/py4paystack/routes/invoices.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-04-11 19:29:58.000000 py4paystack-1.0.2.post1/py4paystack/routes/miscellaneous.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5044 2023-03-16 14:07:00.000000 py4paystack-1.0.2.post1/py4paystack/routes/payment_pages.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5767 2023-03-16 14:07:15.000000 py4paystack-1.0.2.post1/py4paystack/routes/plan.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5289 2023-03-16 14:07:29.000000 py4paystack-1.0.2.post1/py4paystack/routes/product.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-03-16 14:07:37.000000 py4paystack-1.0.2.post1/py4paystack/routes/refund.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3379 2023-04-08 17:19:52.000000 py4paystack-1.0.2.post1/py4paystack/routes/settlement.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7285 2023-03-16 14:08:09.000000 py4paystack-1.0.2.post1/py4paystack/routes/subaccount.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5004 2023-03-16 14:08:34.000000 py4paystack-1.0.2.post1/py4paystack/routes/subscription.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    19913 2023-03-16 14:08:56.000000 py4paystack-1.0.2.post1/py4paystack/routes/transaction.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6434 2023-03-16 14:08:45.000000 py4paystack-1.0.2.post1/py4paystack/routes/transaction_split.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6041 2023-03-16 14:09:20.000000 py4paystack-1.0.2.post1/py4paystack/routes/transfer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2848 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/routes/transfer_control.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7391 2023-03-16 14:09:07.000000 py4paystack-1.0.2.post1/py4paystack/routes/transfer_recipient.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3043 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/routes/verification.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7473 2023-03-16 14:09:30.000000 py4paystack-1.0.2.post1/py4paystack/routes/virtual_accounts.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 20:25:11.627802 py4paystack-1.0.2.post1/py4paystack/utilities/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/utilities/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1610 2023-03-16 14:59:50.000000 py4paystack-1.0.2.post1/py4paystack/utilities/decorators.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      252 2022-08-15 10:48:48.000000 py4paystack-1.0.2.post1/py4paystack/utilities/errors.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1473 2023-04-11 19:43:22.000000 py4paystack-1.0.2.post1/py4paystack/utilities/request.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2012 2023-04-10 10:29:15.000000 py4paystack-1.0.2.post1/py4paystack/utilities/settings.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4252 2023-03-16 14:10:10.000000 py4paystack-1.0.2.post1/py4paystack/utilities/util.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 20:25:11.614468 py4paystack-1.0.2.post1/py4paystack.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    91793 2023-04-11 20:25:11.000000 py4paystack-1.0.2.post1/py4paystack.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1221 2023-04-11 20:25:11.000000 py4paystack-1.0.2.post1/py4paystack.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-11 20:25:11.000000 py4paystack-1.0.2.post1/py4paystack.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       14 2023-04-11 20:25:11.000000 py4paystack-1.0.2.post1/py4paystack.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-04-11 20:25:11.000000 py4paystack-1.0.2.post1/py4paystack.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-04-11 20:25:11.627802 py4paystack-1.0.2.post1/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1636 2023-04-11 20:24:56.000000 py4paystack-1.0.2.post1/setup.py
```

### Comparing `py4paystack-1.0.2/LICENSE` & `py4paystack-1.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/README.md` & `py4paystack-1.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/paystack.py` & `py4paystack-1.0.2.post1/py4paystack/paystack.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/apple_pay.py` & `py4paystack-1.0.2.post1/py4paystack/routes/apple_pay.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/bulk_charges.py` & `py4paystack-1.0.2.post1/py4paystack/routes/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/charge.py` & `py4paystack-1.0.2.post1/py4paystack/routes/charge.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/control_panel.py` & `py4paystack-1.0.2.post1/py4paystack/routes/control_panel.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/customer.py` & `py4paystack-1.0.2.post1/py4paystack/routes/customer.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/disputes.py` & `py4paystack-1.0.2.post1/py4paystack/routes/disputes.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/invoices.py` & `py4paystack-1.0.2.post1/py4paystack/routes/invoices.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/miscellaneous.py` & `py4paystack-1.0.2.post1/py4paystack/routes/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/payment_pages.py` & `py4paystack-1.0.2.post1/py4paystack/routes/payment_pages.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/plan.py` & `py4paystack-1.0.2.post1/py4paystack/routes/plan.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/product.py` & `py4paystack-1.0.2.post1/py4paystack/routes/product.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/refund.py` & `py4paystack-1.0.2.post1/py4paystack/routes/refund.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/settlement.py` & `py4paystack-1.0.2.post1/py4paystack/routes/settlement.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/subaccount.py` & `py4paystack-1.0.2.post1/py4paystack/routes/subaccount.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/subscription.py` & `py4paystack-1.0.2.post1/py4paystack/routes/subscription.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/transaction.py` & `py4paystack-1.0.2.post1/py4paystack/routes/transaction.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/transaction_split.py` & `py4paystack-1.0.2.post1/py4paystack/routes/transaction_split.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/transfer.py` & `py4paystack-1.0.2.post1/py4paystack/routes/transfer.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/transfer_control.py` & `py4paystack-1.0.2.post1/py4paystack/routes/transfer_control.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/transfer_recipient.py` & `py4paystack-1.0.2.post1/py4paystack/routes/transfer_recipient.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/verification.py` & `py4paystack-1.0.2.post1/py4paystack/routes/verification.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/routes/virtual_accounts.py` & `py4paystack-1.0.2.post1/py4paystack/routes/virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/utilities/decorators.py` & `py4paystack-1.0.2.post1/py4paystack/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/utilities/request.py` & `py4paystack-1.0.2.post1/py4paystack/utilities/request.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/utilities/settings.py` & `py4paystack-1.0.2.post1/py4paystack/utilities/settings.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack/utilities/util.py` & `py4paystack-1.0.2.post1/py4paystack/utilities/util.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.2/py4paystack.egg-info/SOURCES.txt` & `py4paystack-1.0.2.post1/py4paystack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 py4paystack/__init__.py
 py4paystack/paystack.py
 py4paystack.egg-info/PKG-INFO
 py4paystack.egg-info/SOURCES.txt
 py4paystack.egg-info/dependency_links.txt
 py4paystack.egg-info/requires.txt
```

### Comparing `py4paystack-1.0.2/setup.py` & `py4paystack-1.0.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 from setuptools import setup, find_packages
+import os
+
+# Optional project description in README.md:
+
+current_directory = os.path.dirname(os.path.abspath(__file__))
+
+try:
+
+    with open(os.path.join(current_directory, 'README.md'), encoding='utf-8') as f:
+
+        long_description = f.read()
+        
+except Exception:
+
+    long_description = ''
 
 
 setup(
 
     # Project name:
 
     name='py4paystack',
 
     # Packages to include in the distribution:
 
     packages=find_packages(),
 
     # Project version number:
 
-    version='1.0.2',
+    version='1.0.2post1',
 
     # List a license for the project, eg. MIT License
 
     license='MIT License',
 
     # Short description of your library:
 
     description='A paystack API wrapper in python with optional type checking functionality',
 
     # Long description of your library:
 
+    long_description=long_description,
+
     long_description_content_type='text/markdown',
 
     # Your name:
 
     author='Raphael Ezeigwe',
 
     # Your email address:
```

