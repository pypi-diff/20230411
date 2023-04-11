# Comparing `tmp/mollie-api-python-3.1.1.tar.gz` & `tmp/mollie-api-python-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mollie-api-python-3.1.1.tar", last modified: Tue Feb 28 13:58:33 2023, max compression
+gzip compressed data, was "mollie-api-python-3.2.0.tar", last modified: Tue Apr 11 07:15:20 2023, max compression
```

## Comparing `mollie-api-python-3.1.1.tar` & `mollie-api-python-3.2.0.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.759712 mollie-api-python-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-02-28 13:58:33.759712 mollie-api-python-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.751712 mollie-api-python-3.1.1/mollie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.751712 mollie-api-python-3.1.1/mollie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.755712 mollie-api-python-3.1.1/mollie/api/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/chargeback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/issuer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/order_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/shipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/objects/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.759712 mollie-api-python-3.1.1/mollie/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/chargebacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/mandates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/order_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/payment_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/settlements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/shipments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/mollie/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 13:58:33.759712 mollie-api-python-3.1.1/mollie_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-02-28 13:58:33.000000 mollie-api-python-3.1.1/mollie_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-28 13:58:33.000000 mollie-api-python-3.1.1/mollie_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 13:58:33.000000 mollie-api-python-3.1.1/mollie_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-28 13:58:33.000000 mollie-api-python-3.1.1/mollie_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-28 13:58:33.000000 mollie-api-python-3.1.1/mollie_api_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 13:58:33.759712 mollie-api-python-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-02-28 13:58:21.000000 mollie-api-python-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.305022 mollie-api-python-3.2.0/mollie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.305022 mollie-api-python-3.2.0/mollie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.309022 mollie-api-python-3.2.0/mollie/api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/chargeback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/issuer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/order_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/objects/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/mollie/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/chargebacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/mandates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/payment_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/settlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/mollie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/mollie_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 07:15:20.000000 mollie-api-python-3.2.0/mollie_api_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:15:20.317022 mollie-api-python-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-11 07:14:56.000000 mollie-api-python-3.2.0/setup.py
```

### Comparing `mollie-api-python-3.1.1/LICENSE.txt` & `mollie-api-python-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/PKG-INFO` & `mollie-api-python-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.1.1
+Version: 3.2.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
```

### Comparing `mollie-api-python-3.1.1/README.md` & `mollie-api-python-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/client.py` & `mollie-api-python-3.2.0/mollie/api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import requests
 from requests_oauthlib import OAuth2Session
 from urllib3.util import Retry
 
 from .error import RequestError, RequestSetupError
 from .resources import (
+    Balances,
     Chargebacks,
     Clients,
     Customers,
     Invoices,
     Methods,
     Onboarding,
     Orders,
@@ -101,14 +102,15 @@
         self.orders = Orders(self)
         self.organizations = Organizations(self)
         self.invoices = Invoices(self)
         self.permissions = Permissions(self)
         self.onboarding = Onboarding(self)
         self.settlements = Settlements(self)
         self.subscriptions = Subscriptions(self)
+        self.balances = Balances(self)
 
         # compose base user agent string
         self.user_agent_components = OrderedDict()
         self.set_user_agent_component("Mollie", self.CLIENT_VERSION)
         self.set_user_agent_component("Python", platform.python_version())
         self.set_user_agent_component(
             "OpenSSL", ssl.OPENSSL_VERSION.split(" ")[1], sanitize=False
@@ -186,80 +188,100 @@
 
     def _perform_http_call_apikey(
         self,
         http_method: str,
         path: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        idempotency_key: str = "",
     ) -> requests.Response:
         if not self.api_key:
             raise RequestSetupError("You have not set an API key. Please use set_api_key() to set the API key.")
 
         if not hasattr(self, "_client"):
             self._client = requests.Session()
             self._client.verify = True
             self._setup_retry()
 
         url, payload, params = self._format_request_data(path, data, params)
         try:
+
+            headers = {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.api_key}",
+                "Content-Type": "application/json",
+                "User-Agent": self.user_agent,
+                "X-Mollie-Client-Info": self.UNAME,
+            }
+
+            if idempotency_key:
+                headers.update({"Idempotency-Key": idempotency_key})
+
             response = self._client.request(
                 method=http_method,
                 url=url,
-                headers={
-                    "Accept": "application/json",
-                    "Authorization": f"Bearer {self.api_key}",
-                    "Content-Type": "application/json",
-                    "User-Agent": self.user_agent,
-                    "X-Mollie-Client-Info": self.UNAME,
-                },
+                headers=headers,
                 params=params,
                 data=payload,
                 timeout=self.timeout,
             )
         except requests.exceptions.RequestException as err:
             raise RequestError(f"Unable to communicate with Mollie: {err}")
+
         return response
 
     def _perform_http_call_oauth(
         self,
         http_method: str,
         path: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        idempotency_key: str = "",
     ) -> requests.Response:
         url, payload, params = self._format_request_data(path, data, params)
         try:
+
+            headers = {
+                "Accept": "application/json",
+                "Content-Type": "application/json",
+                "User-Agent": self.user_agent,
+                "X-Mollie-Client-Info": self.UNAME,
+            }
+
+            if idempotency_key:
+                headers.update({"Idempotency-Key": idempotency_key})
+
             response = self._oauth_client.request(
                 method=http_method,
                 url=url,
-                headers={
-                    "Accept": "application/json",
-                    "Content-Type": "application/json",
-                    "User-Agent": self.user_agent,
-                    "X-Mollie-Client-Info": self.UNAME,
-                },
+                headers=headers,
                 params=params,
                 data=payload,
                 timeout=self.timeout,
             )
         except requests.exceptions.RequestException as err:
             raise RequestError(f"Unable to communicate with Mollie: {err}")
         return response
 
     def perform_http_call(
         self,
         http_method: str,
         path: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        idempotency_key: str = "",
     ) -> requests.Response:
         if hasattr(self, "_oauth_client"):
-            return self._perform_http_call_oauth(http_method, path, data=data, params=params)
+            return self._perform_http_call_oauth(
+                http_method, path, data=data, params=params, idempotency_key=idempotency_key
+            )
         else:
-            return self._perform_http_call_apikey(http_method, path, data=data, params=params)
+            return self._perform_http_call_apikey(
+                http_method, path, data=data, params=params, idempotency_key=idempotency_key
+            )
 
     def setup_oauth(
         self,
         client_id: str,
         client_secret: str,
         redirect_uri: str,
         scope: List[str],
```

### Comparing `mollie-api-python-3.1.1/mollie/api/error.py` & `mollie-api-python-3.2.0/mollie/api/error.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,63 +19,92 @@
 class IdentifierError(RequestSetupError):
     """Errors related to invalid resource identifiers that will be requested from the API."""
 
     pass
 
 
 class ResponseHandlingError(Error):
-    """Errors related to handling the response from the API."""
+    """Errors related to handling the response from the API.
 
-    pass
+    When receiving an error while performing a POST, PATCH or DELETE action,
+    an idempotency_key is available that can be used for replicating the request.
+    """
+
+    idempotency_key = ""
+
+    def __init__(self, message, idempotency_key=""):
+        super().__init__(message)
+        self.idempotency_key = idempotency_key
 
 
 class ResponseError(Error):
-    """Errors reported by the API."""
+    """Errors reported by the API.
+
+    When receiving an error while performing a POST, PATCH or DELETE action,
+    an idempotency_key is available that can be used for replicating the request.
+    """
 
     status = None
     field = None
+    idempotency_key = ""
 
-    def __init__(self, resp=None):
+    def __init__(self, resp=None, idempotency_key=""):
         message = resp["detail"]
         super().__init__(message)
         self.status = resp["status"]
         if "field" in resp:
             self.field = resp["field"]
 
+        self.idempotency_key = idempotency_key
+
     @staticmethod
-    def factory(resp):
+    def factory(resp, idempotency_key=""):
         """Return a ResponseError subclass based on the API payload.
 
         All errors are documented: https://docs.mollie.com/guides/handling-errors#all-possible-status-codes
         More exceptions should be added here when appropriate, and when useful examples of API errors are available.
         """
         status = resp["status"]
-        if status == 401:
-            return UnauthorizedError(resp)
+        if status == 400:
+            return BadRequestError(resp, idempotency_key=idempotency_key)
+        elif status == 401:
+            return UnauthorizedError(resp, idempotency_key=idempotency_key)
         elif status == 404:
-            return NotFoundError(resp)
+            return NotFoundError(resp, idempotency_key=idempotency_key)
+        elif status == 409:
+            return ConflictError(resp, idempotency_key=idempotency_key)
         elif status == 422:
-            return UnprocessableEntityError(resp)
+            return UnprocessableEntityError(resp, idempotency_key=idempotency_key)
         else:
             # generic fallback
-            return ResponseError(resp)
+            return ResponseError(resp, idempotency_key=idempotency_key)
 
 
 class UnauthorizedError(ResponseError):
     """Your request wasn't executed due to failed authentication. Check your API key."""
 
     pass
 
 
 class NotFoundError(ResponseError):
     """The object referenced by your API request does not exist."""
 
     pass
 
 
+class BadRequestError(ResponseError):
+
+    pass
+
+
+class ConflictError(ResponseError):
+
+    pass
+
+
 class UnprocessableEntityError(ResponseError):
     """We could not process your request due to another reason than the ones listed above.
 
     The response usually contains a field property to indicate which field is causing the issue.
     """
 
     pass
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/base.py` & `mollie-api-python-3.2.0/mollie/api/objects/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/capture.py` & `mollie-api-python-3.2.0/mollie/api/objects/capture.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/chargeback.py` & `mollie-api-python-3.2.0/mollie/api/objects/chargeback.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/client.py` & `mollie-api-python-3.2.0/mollie/api/objects/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/customer.py` & `mollie-api-python-3.2.0/mollie/api/objects/customer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/invoice.py` & `mollie-api-python-3.2.0/mollie/api/objects/invoice.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/issuer.py` & `mollie-api-python-3.2.0/mollie/api/objects/issuer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/list.py` & `mollie-api-python-3.2.0/mollie/api/objects/list.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/mandate.py` & `mollie-api-python-3.2.0/mollie/api/objects/mandate.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/method.py` & `mollie-api-python-3.2.0/mollie/api/objects/method.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/onboarding.py` & `mollie-api-python-3.2.0/mollie/api/objects/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/order.py` & `mollie-api-python-3.2.0/mollie/api/objects/order.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,33 +128,33 @@
     @property
     def checkout_url(self):
         return self._get_link("checkout")
 
     # additional methods
 
     def is_created(self):
-        return self._get_property("status") == self.STATUS_CREATED
+        return self.status == self.STATUS_CREATED
 
     def is_paid(self):
-        return self._get_property("status") == self.STATUS_PAID
+        return self.status == self.STATUS_PAID
 
     def is_authorized(self):
-        return self._get_property("status") == self.STATUS_AUTHORIZED
+        return self.status == self.STATUS_AUTHORIZED
 
     def is_canceled(self):
-        return self._get_property("status") == self.STATUS_CANCELED
+        return self.status == self.STATUS_CANCELED
 
     def is_shipping(self):
-        return self._get_property("status") == self.STATUS_SHIPPING
+        return self.status == self.STATUS_SHIPPING
 
     def is_completed(self):
-        return self._get_property("status") == self.STATUS_COMPLETED
+        return self.status == self.STATUS_COMPLETED
 
     def is_expired(self):
-        return self._get_property("status") == self.STATUS_EXPIRED
+        return self.status == self.STATUS_EXPIRED
 
     def has_refunds(self):
         return self.amount_refunded is not None
 
     @property
     def refunds(self):
         from ..resources import OrderRefunds
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/order_line.py` & `mollie-api-python-3.2.0/mollie/api/objects/order_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,23 +126,23 @@
     @property
     def metadata(self):
         return self._get_property("metadata")
 
     # additional methods
 
     def is_created(self):
-        return self._get_property("status") == self.STATUS_CREATED
+        return self.status == self.STATUS_CREATED
 
     def is_authorized(self):
-        return self._get_property("status") == self.STATUS_AUTHORIZED
+        return self.status == self.STATUS_AUTHORIZED
 
     def is_paid(self):
-        return self._get_property("status") == self.STATUS_PAID
+        return self.status == self.STATUS_PAID
 
     def is_shipping(self):
-        return self._get_property("status") == self.STATUS_SHIPPING
+        return self.status == self.STATUS_SHIPPING
 
     def is_canceled(self):
-        return self._get_property("status") == self.STATUS_CANCELED
+        return self.status == self.STATUS_CANCELED
 
     def is_completed(self):
-        return self._get_property("status") == self.STATUS_COMPLETED
+        return self.status == self.STATUS_COMPLETED
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/organization.py` & `mollie-api-python-3.2.0/mollie/api/objects/organization.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/payment.py` & `mollie-api-python-3.2.0/mollie/api/objects/payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,14 +159,18 @@
     def routing(self):
         return self._get_property("routing")
 
     @property
     def subscription_id(self):
         return self._get_property("subscriptionId")
 
+    @property
+    def cancel_url(self):
+        return self._get_property("cancelUrl")
+
     # documented _links
 
     @property
     def checkout_url(self):
         return self._get_link("checkout")
 
     @property
@@ -194,18 +198,14 @@
     @property
     def captures(self):
         """Return the captures related to this payment"""
         from ..resources import PaymentCaptures
 
         return PaymentCaptures(self.client, self)
 
-    @property
-    def cancel_url(self):
-        return self._get_property("cancelUrl")
-
     def get_settlement(self):
         """Return the settlement for this payment."""
         if self.settlement_id:
             return self.client.settlements.get(self.settlement_id)
 
     def get_mandate(self):
         """Return the mandate for this payment."""
@@ -236,47 +236,50 @@
         url = self._get_link("order")
         if url:
             return self.client.orders.from_url(url)
 
     # additional methods
 
     def is_open(self):
-        return self._get_property("status") == self.STATUS_OPEN
+        return self.status == self.STATUS_OPEN
 
     def is_pending(self):
-        return self._get_property("status") == self.STATUS_PENDING
+        return self.status == self.STATUS_PENDING
 
     def is_canceled(self):
-        return self._get_property("status") == self.STATUS_CANCELED
+        return self.status == self.STATUS_CANCELED
 
     def is_expired(self):
-        return self._get_property("status") == self.STATUS_EXPIRED
+        return self.status == self.STATUS_EXPIRED
 
     def is_failed(self):
-        return self._get_property("status") == self.STATUS_FAILED
+        return self.status == self.STATUS_FAILED
 
     def is_authorized(self):
-        return self._get_property("status") == self.STATUS_AUTHORIZED
+        return self.status == self.STATUS_AUTHORIZED
 
     def is_paid(self):
-        return self._get_property("paidAt") is not None
+        return self.paid_at is not None
 
     def has_refunds(self):
         return self._get_link("refunds") is not None
 
     def has_chargebacks(self):
         return self._get_link("chargebacks") is not None
 
     def has_captures(self):
         return self._get_link("captures") is not None
 
+    def has_settlement(self):
+        return self.settlement_id is not None
+
     def has_split_payments(self):
-        return self._get_property("routing") is not None
+        return self.routing is not None
 
     def can_be_refunded(self):
-        return self._get_property("amountRemaining") is not None
+        return self.amount_remaining is not None
 
     def has_sequence_type_first(self):
-        return self._get_property("sequenceType") == self.SEQUENCETYPE_FIRST
+        return self.sequence_type == self.SEQUENCETYPE_FIRST
 
     def has_sequence_type_recurring(self):
-        return self._get_property("sequenceType") == self.SEQUENCETYPE_RECURRING
+        return self.sequence_type == self.SEQUENCETYPE_RECURRING
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/payment_link.py` & `mollie-api-python-3.2.0/mollie/api/objects/payment_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     @property
     def payment_link(self):
         return self._get_link("paymentLink")
 
     # additional methods
 
     def is_paid(self):
-        return self._get_property("paidAt") is not None
+        return self.paid_at is not None
 
     def has_expiration_date(self):
-        return self._get_property("expiresAt") is not None
+        return self.expires_at is not None
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/permission.py` & `mollie-api-python-3.2.0/mollie/api/objects/permission.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/profile.py` & `mollie-api-python-3.2.0/mollie/api/objects/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,14 @@
     @property
     def checkout_preview_url(self):
         return self._get_link("checkoutPreviewUrl")
 
     # additional methods
 
     def is_unverified(self):
-        return self._get_property("status") == self.STATUS_UNVERIFIED
+        return self.status == self.STATUS_UNVERIFIED
 
     def is_verified(self):
-        return self._get_property("status") == self.STATUS_VERIFIED
+        return self.status == self.STATUS_VERIFIED
 
     def is_blocked(self):
-        return self._get_property("status") == self.STATUS_BLOCKED
+        return self.status == self.STATUS_BLOCKED
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/refund.py` & `mollie-api-python-3.2.0/mollie/api/objects/refund.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/settlement.py` & `mollie-api-python-3.2.0/mollie/api/objects/settlement.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,24 +52,24 @@
             APIDeprecationWarning,
         )
         return self._get_property("invoiceId")
 
     # Additional methods
 
     def is_open(self):
-        return self._get_property("status") == self.STATUS_OPEN
+        return self.status == self.STATUS_OPEN
 
     def is_pending(self):
-        return self._get_property("status") == self.STATUS_PENDING
+        return self.status == self.STATUS_PENDING
 
     def is_canceled(self):
-        return self._get_property("status") == self.STATUS_PAIDOUT
+        return self.status == self.STATUS_PAIDOUT
 
     def is_failed(self):
-        return self._get_property("status") == self.STATUS_FAILED
+        return self.status == self.STATUS_FAILED
 
     @property
     def payments(self):
         """Return the payments related to this settlement."""
         from ..resources import SettlementPayments
 
         return SettlementPayments(self.client, self)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/shipment.py` & `mollie-api-python-3.2.0/mollie/api/objects/shipment.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/objects/subscription.py` & `mollie-api-python-3.2.0/mollie/api/objects/subscription.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/__init__.py` & `mollie-api-python-3.2.0/mollie/api/resources/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .balances import *  # noqa: F401, F403
 from .captures import *  # noqa: F401, F403
 from .chargebacks import *  # noqa: F401, F403
 from .clients import *  # noqa: F401, F403
 from .customers import *  # noqa: F401, F403
 from .invoices import *  # noqa: F401, F403
 from .mandates import *  # noqa: F401, F403
 from .methods import *  # noqa: F401, F403
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/captures.py` & `mollie-api-python-3.2.0/mollie/api/resources/captures.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/chargebacks.py` & `mollie-api-python-3.2.0/mollie/api/resources/chargebacks.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/clients.py` & `mollie-api-python-3.2.0/mollie/api/resources/clients.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/customers.py` & `mollie-api-python-3.2.0/mollie/api/resources/customers.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     def get_resource_object(self, result: dict) -> Customer:
         return Customer(result, self.client)
 
     def get(self, resource_id: str, **params: Any) -> Customer:
         self.validate_resource_id(resource_id, "customer ID")
         return super().get(resource_id, **params)
 
-    def update(self, resource_id: str, data: Optional[Dict[str, Any]] = None, **params: Any) -> Customer:
+    def update(
+        self, resource_id: str, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any
+    ) -> Customer:
         self.validate_resource_id(resource_id, "customer ID")
-        return super().update(resource_id, data, **params)
+        return super().update(resource_id, data, idempotency_key, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         self.validate_resource_id(resource_id, "customer ID")
-        return super().delete(resource_id, **params)
+        return super().delete(resource_id, idempotency_key, **params)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/invoices.py` & `mollie-api-python-3.2.0/mollie/api/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/mandates.py` & `mollie-api-python-3.2.0/mollie/api/resources/mandates.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,10 +30,10 @@
     def get_resource_object(self, result: dict) -> Mandate:
         return Mandate(result, self.client)
 
     def get(self, resource_id: str, **params: Any) -> Mandate:
         self.validate_resource_id(resource_id, "mandate ID")
         return super().get(resource_id, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         self.validate_resource_id(resource_id, "mandate ID")
-        return super().delete(resource_id, **params)
+        return super().delete(resource_id, idempotency_key, **params)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/methods.py` & `mollie-api-python-3.2.0/mollie/api/resources/methods.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/onboarding.py` & `mollie-api-python-3.2.0/mollie/api/resources/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/order_lines.py` & `mollie-api-python-3.2.0/mollie/api/resources/order_lines.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/orders.py` & `mollie-api-python-3.2.0/mollie/api/resources/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,23 @@
     def get_resource_object(self, result: dict) -> Order:
         return Order(result, self.client)
 
     def get(self, resource_id: str, **params: Any) -> Order:
         self.validate_resource_id(resource_id, "order ID")
         return super().get(resource_id, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         """Cancel order and return the order object.
 
         Deleting an order causes the order status to change to canceled.
         The updated order object is returned.
         """
         self.validate_resource_id(resource_id, "order ID")
         result = super().delete(resource_id, **params)
         return self.get_resource_object(result)
 
-    def update(self, resource_id: str, data: Optional[Dict[str, Any]] = None, **params: Any) -> Order:
+    def update(
+        self, resource_id: str, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any
+    ) -> Order:
         """Update an order, and return the updated order."""
         self.validate_resource_id(resource_id, "order ID")
-        return super().update(resource_id, data, **params)
+        return super().update(resource_id, data, idempotency_key, **params)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/organizations.py` & `mollie-api-python-3.2.0/mollie/api/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/payment_links.py` & `mollie-api-python-3.2.0/mollie/api/resources/payment_links.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/payments.py` & `mollie-api-python-3.2.0/mollie/api/resources/payments.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,29 @@
 ):
     """Resource handler for the `/payments` endpoint."""
 
     def get(self, resource_id: str, **params: Any) -> Payment:
         self.validate_resource_id(resource_id, "payment ID")
         return super().get(resource_id, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         """Cancel payment and return the payment object.
 
         Deleting a payment causes the payment status to change to canceled.
         The updated payment object is returned.
         """
         self.validate_resource_id(resource_id, "payment ID")
-        result = super().delete(resource_id, **params)
+        result = super().delete(resource_id, idempotency_key, **params)
         return self.get_resource_object(result)
 
-    def update(self, resource_id: str, data: Optional[Dict[str, Any]] = None, **params: Any) -> Payment:
+    def update(
+        self, resource_id: str, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any
+    ) -> Payment:
         self.validate_resource_id(resource_id, "payment ID")
-        return super().update(resource_id, data, **params)
+        return super().update(resource_id, data, idempotency_key, **params)
 
 
 class OrderPayments(PaymentsBase, ResourceCreateMixin):
     """Resource handler for the `/orders/:order_id:/payments` endpoint."""
 
     _order: Order
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/permissions.py` & `mollie-api-python-3.2.0/mollie/api/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/refunds.py` & `mollie-api-python-3.2.0/mollie/api/resources/refunds.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,36 +45,36 @@
     def get_resource_path(self) -> str:
         return f"payments/{self._payment.id}/refunds"
 
     def get(self, resource_id: str, **params: Any) -> Refund:
         self.validate_resource_id(resource_id, "Refund ID")
         return super().get(resource_id, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         self.validate_resource_id(resource_id, "Refund ID")
-        return super().delete(resource_id, **params)
+        return super().delete(resource_id, idempotency_key, **params)
 
 
 class OrderRefunds(RefundsBase, ResourceCreateMixin, ResourceListMixin):
     """Resource handler for the `/orders/:order_id:/refunds` endpoint."""
 
     _order: Order
 
     def __init__(self, client: "Client", order: Order) -> None:
         super().__init__(client)
         self._order = order
 
     def get_resource_path(self) -> str:
         return f"orders/{self._order.id}/refunds"
 
-    def create(self, data: Optional[Dict[str, Any]] = None, **params: Any) -> Refund:
+    def create(self, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any) -> Refund:
         """Create a refund for the order. When no data arg is given, a refund for all order lines is assumed."""
         if not data:
             data = {"lines": []}
-        return super().create(data, **params)
+        return super().create(data, idempotency_key, **params)
 
 
 class SettlementRefunds(RefundsBase, ResourceListMixin):
     """ResourceHandler for the `/settlements/:settlement_id:/refunds` endpoint."""
 
     _settlement: "Settlement"
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/settlements.py` & `mollie-api-python-3.2.0/mollie/api/resources/settlements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from typing import Any, Pattern
 
-from ..error import IdentifierError
 from ..objects.settlement import Settlement
 from .base import ResourceGetMixin, ResourceListMixin
 
 
 class Settlements(ResourceGetMixin, ResourceListMixin):
     """Resource handler for the `/settlements` endpoint."""
 
@@ -40,15 +39,12 @@
         if resource_id in ["next", "open"]:
             return
 
         elif cls.BANK_REFERENCE_REGEX.match(str(resource_id)):
             return
 
         else:
-            try:
-                super().validate_resource_id(resource_id)
-            except IdentifierError:
-                raise IdentifierError(exc_message)
+            super().validate_resource_id(resource_id, message=exc_message)
 
     def get(self, resource_id: str, **params: Any) -> Settlement:
         self.validate_resource_id(resource_id)
         return super().get(resource_id, **params)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/shipments.py` & `mollie-api-python-3.2.0/mollie/api/resources/shipments.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 
     def get_resource_object(self, result: dict) -> Shipment:
         return Shipment(result, self.client)
 
     def get_resource_path(self) -> str:
         return f"orders/{self._order.id}/shipments"
 
-    def create(self, data: Optional[Dict[str, Any]] = None, **params: Any) -> Shipment:
+    def create(self, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any) -> Shipment:
         """Create a shipment for an order.
 
         If the data parameter is omitted, a shipment for all order lines is assumed.
         """
         if data is None:
             data = {"lines": []}
-        return super().create(data, **params)
+        return super().create(data, idempotency_key, **params)
 
     def get(self, resource_id: str, **params: Any) -> Shipment:
         self.validate_resource_id(resource_id, "shipment ID")
         return super().get(resource_id, **params)
 
-    def update(self, resource_id: str, data: Optional[Dict[str, Any]] = None, **params: Any) -> Shipment:
+    def update(
+        self, resource_id: str, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any
+    ) -> Shipment:
         self.validate_resource_id(resource_id, "shipment ID")
-        return super().update(resource_id, data, **params)
+        return super().update(resource_id, data, idempotency_key, **params)
```

### Comparing `mollie-api-python-3.1.1/mollie/api/resources/subscriptions.py` & `mollie-api-python-3.2.0/mollie/api/resources/subscriptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,15 +52,17 @@
     def get_resource_path(self) -> str:
         return f"customers/{self._customer.id}/subscriptions"
 
     def get(self, resource_id: str, **params: Any) -> Subscription:
         self.validate_resource_id(resource_id, "subscription ID")
         return super().get(resource_id, **params)
 
-    def update(self, resource_id: str, data: Optional[Dict[str, Any]] = None, **params: Any) -> Subscription:
+    def update(
+        self, resource_id: str, data: Optional[Dict[str, Any]] = None, idempotency_key: str = "", **params: Any
+    ) -> Subscription:
         self.validate_resource_id(resource_id, "subscription ID")
-        return super().update(resource_id, data, **params)
+        return super().update(resource_id, data, idempotency_key, **params)
 
-    def delete(self, resource_id: str, **params: Any) -> dict:
+    def delete(self, resource_id: str, idempotency_key: str = "", **params: Any) -> dict:
         self.validate_resource_id(resource_id, "subscription ID")
-        resp = super().delete(resource_id, **params)
+        resp = super().delete(resource_id, idempotency_key, **params)
         return self.get_resource_object(resp)
```

### Comparing `mollie-api-python-3.1.1/mollie_api_python.egg-info/PKG-INFO` & `mollie-api-python-3.2.0/mollie_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.1.1
+Version: 3.2.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
```

### Comparing `mollie-api-python-3.1.1/mollie_api_python.egg-info/SOURCES.txt` & `mollie-api-python-3.2.0/mollie_api_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 mollie/__init__.py
 mollie/py.typed
 mollie/api/__init__.py
 mollie/api/client.py
 mollie/api/error.py
 mollie/api/version.py
 mollie/api/objects/__init__.py
+mollie/api/objects/balance.py
+mollie/api/objects/balance_report.py
+mollie/api/objects/balance_transaction.py
 mollie/api/objects/base.py
 mollie/api/objects/capture.py
 mollie/api/objects/chargeback.py
 mollie/api/objects/client.py
 mollie/api/objects/customer.py
 mollie/api/objects/invoice.py
 mollie/api/objects/issuer.py
@@ -29,14 +32,15 @@
 mollie/api/objects/permission.py
 mollie/api/objects/profile.py
 mollie/api/objects/refund.py
 mollie/api/objects/settlement.py
 mollie/api/objects/shipment.py
 mollie/api/objects/subscription.py
 mollie/api/resources/__init__.py
+mollie/api/resources/balances.py
 mollie/api/resources/base.py
 mollie/api/resources/captures.py
 mollie/api/resources/chargebacks.py
 mollie/api/resources/clients.py
 mollie/api/resources/customers.py
 mollie/api/resources/invoices.py
 mollie/api/resources/mandates.py
```

### Comparing `mollie-api-python-3.1.1/setup.py` & `mollie-api-python-3.2.0/setup.py`

 * *Files identical despite different names*

