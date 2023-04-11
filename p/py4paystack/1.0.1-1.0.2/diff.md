# Comparing `tmp/py4paystack-1.0.1.tar.gz` & `tmp/py4paystack-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4paystack-1.0.1.tar", last modified: Thu Mar 16 15:24:40 2023, max compression
+gzip compressed data, was "py4paystack-1.0.2.tar", last modified: Tue Apr 11 19:59:35 2023, max compression
```

## Comparing `py4paystack-1.0.1.tar` & `py4paystack-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.796779 py4paystack-1.0.1/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1072 2022-08-15 10:48:48.000000 py4paystack-1.0.1/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)    91824 2023-03-16 15:24:40.793445 py4paystack-1.0.1/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)    90015 2023-03-16 15:19:31.000000 py4paystack-1.0.1/README.md
--rw-r--r--   0 raphael   (1000) raphael   (1000)      663 2023-03-16 15:24:08.000000 py4paystack-1.0.1/pyproject.toml
--rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-03-16 15:24:40.796779 py4paystack-1.0.1/setup.cfg
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.773445 py4paystack-1.0.1/src/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.776778 py4paystack-1.0.1/src/py4paystack/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2601 2022-08-15 11:37:18.000000 py4paystack-1.0.1/src/py4paystack/paystack.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.790112 py4paystack-1.0.1/src/py4paystack/routes/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/routes/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1396 2023-03-16 13:40:27.000000 py4paystack-1.0.1/src/py4paystack/routes/apple_pay.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5516 2023-03-16 13:49:20.000000 py4paystack-1.0.1/src/py4paystack/routes/bulk_charges.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     9274 2023-03-16 13:51:16.000000 py4paystack-1.0.1/src/py4paystack/routes/charge.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      892 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/routes/control_panel.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7561 2023-03-16 14:06:02.000000 py4paystack-1.0.1/src/py4paystack/routes/customers.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     8338 2023-03-16 14:06:27.000000 py4paystack-1.0.1/src/py4paystack/routes/disputes.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    10607 2023-03-16 14:06:38.000000 py4paystack-1.0.1/src/py4paystack/routes/invoices.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/routes/miscellaneous.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5044 2023-03-16 14:07:00.000000 py4paystack-1.0.1/src/py4paystack/routes/payment_pages.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5767 2023-03-16 14:07:15.000000 py4paystack-1.0.1/src/py4paystack/routes/plans.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5289 2023-03-16 14:07:29.000000 py4paystack-1.0.1/src/py4paystack/routes/products.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-03-16 14:07:37.000000 py4paystack-1.0.1/src/py4paystack/routes/refund.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3380 2023-03-16 14:07:59.000000 py4paystack-1.0.1/src/py4paystack/routes/settlement.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7285 2023-03-16 14:08:09.000000 py4paystack-1.0.1/src/py4paystack/routes/subaccount.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     5004 2023-03-16 14:08:34.000000 py4paystack-1.0.1/src/py4paystack/routes/subscription.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)    19913 2023-03-16 14:08:56.000000 py4paystack-1.0.1/src/py4paystack/routes/transactions.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6434 2023-03-16 14:08:45.000000 py4paystack-1.0.1/src/py4paystack/routes/transactions_split.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7391 2023-03-16 14:09:07.000000 py4paystack-1.0.1/src/py4paystack/routes/transfer_recipient.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     6041 2023-03-16 14:09:20.000000 py4paystack-1.0.1/src/py4paystack/routes/transfers.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2848 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/routes/transfers_control.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3043 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/routes/verification.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7473 2023-03-16 14:09:30.000000 py4paystack-1.0.1/src/py4paystack/routes/virtual_accounts.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.793445 py4paystack-1.0.1/src/py4paystack/utilities/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/utilities/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1610 2023-03-16 14:59:50.000000 py4paystack-1.0.1/src/py4paystack/utilities/decorators.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      252 2022-08-15 10:48:48.000000 py4paystack-1.0.1/src/py4paystack/utilities/errors.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1568 2023-03-16 14:03:27.000000 py4paystack-1.0.1/src/py4paystack/utilities/request.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2011 2023-03-16 14:57:30.000000 py4paystack-1.0.1/src/py4paystack/utilities/settings.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4252 2023-03-16 14:10:10.000000 py4paystack-1.0.1/src/py4paystack/utilities/util.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-03-16 15:24:40.776778 py4paystack-1.0.1/src/py4paystack.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)    91824 2023-03-16 15:24:40.000000 py4paystack-1.0.1/src/py4paystack.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1340 2023-03-16 15:24:40.000000 py4paystack-1.0.1/src/py4paystack.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-03-16 15:24:40.000000 py4paystack-1.0.1/src/py4paystack.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-03-16 15:24:40.000000 py4paystack-1.0.1/src/py4paystack.egg-info/top_level.txt
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.077903 py4paystack-1.0.2/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1072 2022-08-15 10:48:48.000000 py4paystack-1.0.2/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      598 2023-04-11 19:59:35.077903 py4paystack-1.0.2/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    91188 2023-04-11 19:58:22.000000 py4paystack-1.0.2/README.md
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.061236 py4paystack-1.0.2/py4paystack/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2601 2022-08-15 11:37:18.000000 py4paystack-1.0.2/py4paystack/paystack.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.074569 py4paystack-1.0.2/py4paystack/routes/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1396 2023-03-16 13:40:27.000000 py4paystack-1.0.2/py4paystack/routes/apple_pay.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5516 2023-03-16 13:49:20.000000 py4paystack-1.0.2/py4paystack/routes/bulk_charges.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     9274 2023-03-16 13:51:16.000000 py4paystack-1.0.2/py4paystack/routes/charge.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      892 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/control_panel.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7561 2023-03-16 14:06:02.000000 py4paystack-1.0.2/py4paystack/routes/customer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     8338 2023-03-16 14:06:27.000000 py4paystack-1.0.2/py4paystack/routes/disputes.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    10607 2023-03-16 14:06:38.000000 py4paystack-1.0.2/py4paystack/routes/invoices.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-04-11 19:29:58.000000 py4paystack-1.0.2/py4paystack/routes/miscellaneous.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5044 2023-03-16 14:07:00.000000 py4paystack-1.0.2/py4paystack/routes/payment_pages.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5767 2023-03-16 14:07:15.000000 py4paystack-1.0.2/py4paystack/routes/plan.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5289 2023-03-16 14:07:29.000000 py4paystack-1.0.2/py4paystack/routes/product.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3532 2023-03-16 14:07:37.000000 py4paystack-1.0.2/py4paystack/routes/refund.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3379 2023-04-08 17:19:52.000000 py4paystack-1.0.2/py4paystack/routes/settlement.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7285 2023-03-16 14:08:09.000000 py4paystack-1.0.2/py4paystack/routes/subaccount.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     5004 2023-03-16 14:08:34.000000 py4paystack-1.0.2/py4paystack/routes/subscription.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    19913 2023-03-16 14:08:56.000000 py4paystack-1.0.2/py4paystack/routes/transaction.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6434 2023-03-16 14:08:45.000000 py4paystack-1.0.2/py4paystack/routes/transaction_split.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6041 2023-03-16 14:09:20.000000 py4paystack-1.0.2/py4paystack/routes/transfer.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2848 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/transfer_control.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7391 2023-03-16 14:09:07.000000 py4paystack-1.0.2/py4paystack/routes/transfer_recipient.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3043 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/routes/verification.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7473 2023-03-16 14:09:30.000000 py4paystack-1.0.2/py4paystack/routes/virtual_accounts.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.074569 py4paystack-1.0.2/py4paystack/utilities/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/utilities/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1610 2023-03-16 14:59:50.000000 py4paystack-1.0.2/py4paystack/utilities/decorators.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      252 2022-08-15 10:48:48.000000 py4paystack-1.0.2/py4paystack/utilities/errors.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1473 2023-04-11 19:43:22.000000 py4paystack-1.0.2/py4paystack/utilities/request.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2012 2023-04-10 10:29:15.000000 py4paystack-1.0.2/py4paystack/utilities/settings.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4252 2023-03-16 14:10:10.000000 py4paystack-1.0.2/py4paystack/utilities/util.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-11 19:59:35.061236 py4paystack-1.0.2/py4paystack.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      598 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1231 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       14 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-04-11 19:59:34.000000 py4paystack-1.0.2/py4paystack.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      103 2023-04-11 19:59:35.081236 py4paystack-1.0.2/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1289 2023-04-11 19:52:20.000000 py4paystack-1.0.2/setup.py
```

### Comparing `py4paystack-1.0.1/LICENSE` & `py4paystack-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/PKG-INFO` & `py4paystack-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,17 @@
-Metadata-Version: 2.1
-Name: py4paystack
-Version: 1.0.1
-Summary: A paystack API wrapper in python with type checking functionality
-Author-email: Raphael Ezeigwe <iraphael1308@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 Raphael Ezeigwe
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/devRaphael13/pypaystack
-Project-URL: Bug Tracker, https://github.com/devRaphael13/pypaystack/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Py4paystack
 
 A paystack API wrapper with type checking written in python
 
 ## Contents
 
 - [Installation](#installation)
 - [Type Checking](#type-checking)
 - [Requirements](#requirements)
+- [Changelog](#changelog)
 - [Accept payments](#accept-payments)
 - [Advanced Usage](#advanced-usage)
 - [API Routes](#routes)
 
 <br>
 <br>
 
@@ -62,26 +27,35 @@
 
 - python-dotenv
 
 <br>
 
 <br>
 
+## Changelog
+
+**V1.0.2**
+- Bug fixes
+
+<br>
+
+<br>
+
 ## Type Checking
 
 The Type checking funtion is on by default, turn of by setting `TYPE_CHECK` to `False` in your .env file.
 
 <br>
 
 ## Accept Payments
 
 To accept payments, you can import the Transaction class from the routes module if that'll be all you need, alternatively you can import the Paystack class like if you need more functionality.
 
 ```{python}
-from py4paystack.routes import Transaction # or from py4paystack import Paystack
+from py4paystack.routes.transactions import Transaction # or from py4paystack.paystack import Paystack
 
 trans = Transaction('ExampleSecretKey') # or
 trans = Paystack('ExampleSecretKey).transaction()
 
 res = trans.initialize('testemail@test.com', 120934)
 ```
 
@@ -125,28 +99,30 @@
 - [Plan](#plan)
 - [Product](#product)
 - [Refund](#refund)
 - [Settlements](#settlements)
 - [Subaccount](#subaccounts)
 - [Subscription](#subscription)
 - [Transaction Split](#transaction-split)
-- [Transactions](#transaction)
+- [Transaction](#transaction)
 - [Transfer Control](#transfer-control)
 - [Transfer Recipient](#transfer-recipient)
-- [Transfers](#transfer)
+- [Transfer](#transfer)
 - [Verification](#verification)
 
 <br>
 <br>
 <hr>
 <br>
 <br>
 
 ## **Paystack**
 
+    py4paystack.paystack.Paystack
+
 <br>
 
 `Paystack(secret_key: str)`
 
 General class that hold all the functionalities of the Paystack API (essentially a class to rule them all). Methods returns and instance of the class with the same name i.e `Paystack('Paystack secret_key').charge()` is equivalent to `Charge('Paystack secret_key')`, use the first approach if you are going to need multiple functionalities and don't want to import each class individually and the second when you just need one class or functionality e.g you just need the Transaction class.
 
 **Methods**
@@ -199,14 +175,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Apple Pay**
 
+    py4paystack.routes.apple_pay.ApplePay
+
 <br>
 
 `ApplePay(secret_key: str)`
 
 The Apple Pay API allows you register your application's top-level domain or subdomain
 
 <br>
@@ -254,14 +232,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Bulk Charges**
 
+    py4paystack.routes.bulk_charges.BulkCharges
+
 <br>
 
 `BulkCharges(secret_key: str)`
 
 The Bulk Charges API allows you create and manage multiple recurring payments from your customers
 
 <br>
@@ -375,14 +355,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Charge**
 
+    py4paystack.routes.charge.Charge
+
 <br>
 
 `Charge(secret_key: str)`
 
 The Charge API allows you to configure payment channel of your choice when initiating a payment.
 
 <br>
@@ -538,15 +520,15 @@
 <br>
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Control Panel**
-
+    py4paystack.routes.control_panel.ControlPanel
 <br>
 
 `ControlPanel(*args, **kwargs)`
 
 The Control Panel API allows you manage some settings on your integration
 <br>
 
@@ -577,15 +559,15 @@
 <br>
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Customer**
-
+    py4paystack.routes.customer.Customer
 <br>
 
 `Customer(secret_key: str)`
 
     The Customers class allows you create and manage customers on your integration.
 
 <br>
@@ -733,14 +715,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Disputes**
 
+    py4paystack.routes.disputes.Disputes
+
 <br>
 
 `Disputes(secret_key: str)`
 
 The Disputes API allows you manage transaction disputes on your integration
 
 <br>
@@ -909,14 +893,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Dedicated Virtual Accounts**
 
+    py4paystack.routes.virtual_accounts.DedicatedVirtualAccounts
+
 <br>
 
 `DedicatedVirtualAccounts(secret_key: str)`
 
 The Dedicated Virtual Account class enables Nigerian merchants to manage unique payment accounts of their customers.
 
 ### **Methods**:
@@ -1068,14 +1054,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Invoice**
 
+    py4paystack.routes.invoice.Invoice
+
 `Invoice(secret_key: str)`
 
 The Invoices API allows you issue out and manage payment requests
 
 ### **Methods**:
 
 - `archive(self, invoice: Union[int, str])`
@@ -1265,14 +1253,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Miscellaneous**
 
+    py4paystack.routes.miscellaneous.Miscellaneous
+
 <br>
 
 `Miscellaneous(secret_key: str)`
 
 The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs
 
 ### **Methods**:
@@ -1298,15 +1288,15 @@
 
         type (str, optional): Type of financial channel. For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels. Defaults to None.
 
         currency (str, optional): Any of NGN, USD, GHS or ZAR. Defaults to None.
 
   **Returns**:
 
-        JSON: Data fetched from API
+      JSON: Data fetched from API
 
 <br>
 
 - `list_providers(self, pay_with_bank_transfer: bool = None)`
 
   Get a list of all providers for Dedicated Virtual Account
 
@@ -1346,14 +1336,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Payment Pages**
 
+    py4paystack.routes.payment_pages.PaymentPages
+
 <br>
 
 `PaymentPages(secret_key: str)`
 
 The Payment Pages API provides a quick and secure way to collect payment for products.
 
 ### **Methods**:
@@ -1472,14 +1464,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Plan**
 
+    py4paystack.routes.plans.Plan
+
 <br>
 
 `Plan(secret_key: str)`
 
 The Plans API allows you create and manage installment payment options on your integration
 
 ### **Methods**:
@@ -1582,14 +1576,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Product**
 
+    py4paystack.routes.product.Product
+
 <br>
 
 `Product(secret_key: str)`
 
 The Products API allows you create and manage inventories on your integration
 
 ### **Methods**:
@@ -1682,14 +1678,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Refund**
 
+    py4paystack.routes.refund.Refund
+
 <br>
 
 `Refund(secret_key: str)`
 
 The Refunds API allows you create and manage transaction refunds
 
 ### **Methods**:
@@ -1758,14 +1756,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Settlements**
 
+    py4paystack.routes.settlement.Settlement
+
 <br>
 
 `Settlements(secret_key: str)`
 
 The Settlements API allows you gain insights into payouts made by Paystack to your bank account
 
 ### **Methods**:
@@ -1818,14 +1818,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **SubAccounts**
 
+    py4paystack.routes.subaccounts.SubAccounts
+
 <br>
 
 `SubAccounts(secret_key: str)`
 
 The Subaccounts API allows you create and manage subaccounts on your integration.
 Subaccounts can be used to split payment between two accounts (your main account and a sub account)
 
@@ -1939,14 +1941,16 @@
 
 ## **Subscription**
 
 <br>
 
 `Subscription(secret_key: str)`
 
+    py4paystack.routes.subscription.Subscription
+
 The Subscriptions API allows you create and manage recurring payment on your integration
 
 ### **Methods**:
 
 <br>
 
 - `create(self, email_or_customer_code: str, plan_code: str, authorization_code: str = None, start_date: Union[datetime.datetime, datetime.date, str] = None)`
@@ -2067,14 +2071,16 @@
 <br>
 <br>
 
 ## **Transaction Split**
 
 <br>
 
+    py4paystack.routes.transaction_split.TransactionSplit
+
 `TransactionSplit(secret_key: str)`
 
 Create, list, retrieve, update split transaction configuration with one or more SubAccounts (You should have subaccounts on your integration to use this)
 
 ### **Methods**:
 
 <br>
@@ -2201,14 +2207,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Transaction**
 
+    py4paystack.routes.transaction.Transaction
+
 <br>
 
 `Transaction(secret_key: str)`
 
 Accept payment from your customers.
 The Transactions API allows you create and manage payments on your integration
 
@@ -2476,14 +2484,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Transfer Recipient**
 
+    py4paystack.routes.transfer_recipient.TransferRecipient
+
 <br>
 
 `TransferRecipient(secret_key: str)`
 
 The Transfer Recipients API allows you create and manage beneficiaries that you send money to
 
 ### **Methods**:
@@ -2602,14 +2612,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Transfer Control**
 
+    py4paystack.routes.transfer_control.TransferControl
+
 <br>
 
 `TransferControl(secret_key: str)`
 
 The Transfers Control API allows you manage settings of your transfers
 
 ### **Methods**:
@@ -2693,14 +2705,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Transfer**
 
+    py4paystack.routes.transfer.Transfer
+
 <br>
 
 `Transfer(secret_key: str)`
 
 The Transfers API allows you automate sending money on your integration
 
 ### **Methods**:
@@ -2821,14 +2835,16 @@
 
 [Back to the top](#routes)
 <br>
 <br>
 
 ## **Verification**
 
+    py4paystack.routes.verification.Verification
+
 <br>
 
 `Verification(secret_key: str)`
 
 The Verification class allows you perform KYC ( Know Your Customer ) processes.
 This feature is only available to businesses in Nigeria.
```

### Comparing `py4paystack-1.0.1/src/py4paystack/paystack.py` & `py4paystack-1.0.2/py4paystack/paystack.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/apple_pay.py` & `py4paystack-1.0.2/py4paystack/routes/apple_pay.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/bulk_charges.py` & `py4paystack-1.0.2/py4paystack/routes/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/charge.py` & `py4paystack-1.0.2/py4paystack/routes/charge.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/control_panel.py` & `py4paystack-1.0.2/py4paystack/routes/control_panel.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/customers.py` & `py4paystack-1.0.2/py4paystack/routes/customer.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/disputes.py` & `py4paystack-1.0.2/py4paystack/routes/disputes.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/invoices.py` & `py4paystack-1.0.2/py4paystack/routes/invoices.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/miscellaneous.py` & `py4paystack-1.0.2/py4paystack/routes/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/payment_pages.py` & `py4paystack-1.0.2/py4paystack/routes/payment_pages.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/plans.py` & `py4paystack-1.0.2/py4paystack/routes/plan.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/products.py` & `py4paystack-1.0.2/py4paystack/routes/product.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/refund.py` & `py4paystack-1.0.2/py4paystack/routes/refund.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/settlement.py` & `py4paystack-1.0.2/py4paystack/routes/settlement.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Union
 from ..utilities import util, decorators, settings
 from ..utilities.request import Request
 
 
 @decorators.class_type_checker
-class Settlements(Request):
+class Settlement(Request):
 
     """
     The Settlements API allows you gain insights into payouts made by Paystack to your bank account
     """
 
     path = '/settlement'
```

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/subaccount.py` & `py4paystack-1.0.2/py4paystack/routes/subaccount.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/subscription.py` & `py4paystack-1.0.2/py4paystack/routes/subscription.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/transactions.py` & `py4paystack-1.0.2/py4paystack/routes/transaction.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/transactions_split.py` & `py4paystack-1.0.2/py4paystack/routes/transaction_split.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/transfer_recipient.py` & `py4paystack-1.0.2/py4paystack/routes/transfer_recipient.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/transfers.py` & `py4paystack-1.0.2/py4paystack/routes/transfer.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/transfers_control.py` & `py4paystack-1.0.2/py4paystack/routes/transfer_control.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/verification.py` & `py4paystack-1.0.2/py4paystack/routes/verification.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/routes/virtual_accounts.py` & `py4paystack-1.0.2/py4paystack/routes/virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/utilities/decorators.py` & `py4paystack-1.0.2/py4paystack/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack/utilities/request.py` & `py4paystack-1.0.2/py4paystack/utilities/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,16 @@
             'authorization': f'bearer {secret_key}',
             'Content-type': 'application/json',
         }
 
     @classmethod
     def request(cls, path: str, method: str, headers: dict = None, payload: dict = None):
         connection = http.client.HTTPSConnection('api.paystack.co')
-        if payload is not None:
-            connection.request(method, path, headers=headers, body=payload)
-        else:
-            connection.request(method, path, headers=headers)
-        return connection.getresponse().read().decode('utf-8')
+        connection.request(method, path, headers=headers, body=payload)
+        return json.loads(connection.getresponse().read().decode('utf-8'))
 
     def get(self, path: str):
         return self.request(path, 'GET', headers={'authorization': self.headers.pop('authorization')})
 
     def post(self, path: str, payload: Union[dict, Sequence, set] = None):
         if payload:
             return self.request(path, 'POST', headers=self.headers, payload=json.dumps(payload))
@@ -34,7 +31,8 @@
         return self.request(path, 'PUT', headers=self.headers, payload=json.dumps(payload))
 
     def delete(self, path: str, payload: dict = None):
         method = 'DELETE'
         if payload:
             return self.request(path, method, headers=self.headers, payload=payload)
         return self.request(path, method, headers={'authorization': self.headers.pop('authorization')})
+
```

### Comparing `py4paystack-1.0.1/src/py4paystack/utilities/settings.py` & `py4paystack-1.0.2/py4paystack/utilities/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from collections import namedtuple
 from dotenv import load_dotenv
 
+
 Code = namedtuple('Code', ['prefix', 'name'])
 SUBACCOUNT = Code('ACCT', 'subaccount')
 PLAN = Code('PLN', 'plan')
 SUBSCRIPTION = Code('SUB', 'subscription')
 AUTHORIZATION = Code('AUTH', 'authorization')
 SPLIT = Code('SPL', 'split')
 PRODUCT = Code('PROD', 'product')
```

### Comparing `py4paystack-1.0.1/src/py4paystack/utilities/util.py` & `py4paystack-1.0.2/py4paystack/utilities/util.py`

 * *Files identical despite different names*

### Comparing `py4paystack-1.0.1/src/py4paystack.egg-info/SOURCES.txt` & `py4paystack-1.0.2/py4paystack.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 LICENSE
 README.md
-pyproject.toml
-src/py4paystack/__init__.py
-src/py4paystack/paystack.py
-src/py4paystack.egg-info/PKG-INFO
-src/py4paystack.egg-info/SOURCES.txt
-src/py4paystack.egg-info/dependency_links.txt
-src/py4paystack.egg-info/top_level.txt
-src/py4paystack/routes/__init__.py
-src/py4paystack/routes/apple_pay.py
-src/py4paystack/routes/bulk_charges.py
-src/py4paystack/routes/charge.py
-src/py4paystack/routes/control_panel.py
-src/py4paystack/routes/customers.py
-src/py4paystack/routes/disputes.py
-src/py4paystack/routes/invoices.py
-src/py4paystack/routes/miscellaneous.py
-src/py4paystack/routes/payment_pages.py
-src/py4paystack/routes/plans.py
-src/py4paystack/routes/products.py
-src/py4paystack/routes/refund.py
-src/py4paystack/routes/settlement.py
-src/py4paystack/routes/subaccount.py
-src/py4paystack/routes/subscription.py
-src/py4paystack/routes/transactions.py
-src/py4paystack/routes/transactions_split.py
-src/py4paystack/routes/transfer_recipient.py
-src/py4paystack/routes/transfers.py
-src/py4paystack/routes/transfers_control.py
-src/py4paystack/routes/verification.py
-src/py4paystack/routes/virtual_accounts.py
-src/py4paystack/utilities/__init__.py
-src/py4paystack/utilities/decorators.py
-src/py4paystack/utilities/errors.py
-src/py4paystack/utilities/request.py
-src/py4paystack/utilities/settings.py
-src/py4paystack/utilities/util.py
+setup.cfg
+setup.py
+py4paystack/__init__.py
+py4paystack/paystack.py
+py4paystack.egg-info/PKG-INFO
+py4paystack.egg-info/SOURCES.txt
+py4paystack.egg-info/dependency_links.txt
+py4paystack.egg-info/requires.txt
+py4paystack.egg-info/top_level.txt
+py4paystack/routes/__init__.py
+py4paystack/routes/apple_pay.py
+py4paystack/routes/bulk_charges.py
+py4paystack/routes/charge.py
+py4paystack/routes/control_panel.py
+py4paystack/routes/customer.py
+py4paystack/routes/disputes.py
+py4paystack/routes/invoices.py
+py4paystack/routes/miscellaneous.py
+py4paystack/routes/payment_pages.py
+py4paystack/routes/plan.py
+py4paystack/routes/product.py
+py4paystack/routes/refund.py
+py4paystack/routes/settlement.py
+py4paystack/routes/subaccount.py
+py4paystack/routes/subscription.py
+py4paystack/routes/transaction.py
+py4paystack/routes/transaction_split.py
+py4paystack/routes/transfer.py
+py4paystack/routes/transfer_control.py
+py4paystack/routes/transfer_recipient.py
+py4paystack/routes/verification.py
+py4paystack/routes/virtual_accounts.py
+py4paystack/utilities/__init__.py
+py4paystack/utilities/decorators.py
+py4paystack/utilities/errors.py
+py4paystack/utilities/request.py
+py4paystack/utilities/settings.py
+py4paystack/utilities/util.py
```

