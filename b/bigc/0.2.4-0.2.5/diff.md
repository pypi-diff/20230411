# Comparing `tmp/bigc-0.2.4.tar.gz` & `tmp/bigc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigc-0.2.4.tar", max compression
+gzip compressed data, was "bigc-0.2.5.tar", max compression
```

## Comparing `bigc-0.2.4.tar` & `bigc-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-02-24 20:48:30.355472 bigc-0.2.4/LICENSE.txt
--rw-r--r--   0        0        0     1596 2023-02-24 20:48:30.355472 bigc-0.2.4/README.md
--rw-r--r--   0        0        0       32 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/__init__.py
--rw-r--r--   0        0        0     1069 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/api.py
--rw-r--r--   0        0        0     6458 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/api_client.py
--rw-r--r--   0        0        0       49 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/data/__init__.py
--rw-r--r--   0        0        0      482 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/data/order_status.py
--rw-r--r--   0        0        0     1639 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/exceptions.py
--rw-r--r--   0        0        0      431 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/__init__.py
--rw-r--r--   0        0        0     1741 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/carts.py
--rw-r--r--   0        0        0     1180 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/categories.py
--rw-r--r--   0        0        0     4116 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/checkouts.py
--rw-r--r--   0        0        0     1178 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/customer_groups.py
--rw-r--r--   0        0        0     2922 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/customers.py
--rw-r--r--   0        0        0     3575 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/orders.py
--rw-r--r--   0        0        0     1414 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/product_variants.py
--rw-r--r--   0        0        0     2682 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/products.py
--rw-r--r--   0        0        0     1205 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/resources/webhooks.py
--rw-r--r--   0        0        0      557 2023-02-24 20:48:30.355472 bigc-0.2.4/bigc/utils.py
--rw-r--r--   0        0        0      770 2023-02-24 20:48:30.355472 bigc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 bigc-0.2.4/setup.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-11 19:29:46.699022 bigc-0.2.5/LICENSE.txt
+-rw-r--r--   0        0        0     1596 2023-04-11 19:29:46.699022 bigc-0.2.5/README.md
+-rw-r--r--   0        0        0       32 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/__init__.py
+-rw-r--r--   0        0        0     1069 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/api.py
+-rw-r--r--   0        0        0     6458 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/api_client.py
+-rw-r--r--   0        0        0       49 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/data/__init__.py
+-rw-r--r--   0        0        0      482 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/data/order_status.py
+-rw-r--r--   0        0        0     1639 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/exceptions.py
+-rw-r--r--   0        0        0      431 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/__init__.py
+-rw-r--r--   0        0        0     1741 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/carts.py
+-rw-r--r--   0        0        0     1180 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/categories.py
+-rw-r--r--   0        0        0     4116 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/checkouts.py
+-rw-r--r--   0        0        0     1178 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/customer_groups.py
+-rw-r--r--   0        0        0     2922 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/customers.py
+-rw-r--r--   0        0        0     3832 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/orders.py
+-rw-r--r--   0        0        0     1414 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/product_variants.py
+-rw-r--r--   0        0        0     2682 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/products.py
+-rw-r--r--   0        0        0     1205 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/resources/webhooks.py
+-rw-r--r--   0        0        0      557 2023-04-11 19:29:46.699022 bigc-0.2.5/bigc/utils.py
+-rw-r--r--   0        0        0      770 2023-04-11 19:29:46.699022 bigc-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 bigc-0.2.5/PKG-INFO
```

### Comparing `bigc-0.2.4/LICENSE.txt` & `bigc-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/README.md` & `bigc-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/api.py` & `bigc-0.2.5/bigc/api.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/api_client.py` & `bigc-0.2.5/bigc/api_client.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/exceptions.py` & `bigc-0.2.5/bigc/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/carts.py` & `bigc-0.2.5/bigc/resources/carts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/categories.py` & `bigc-0.2.5/bigc/resources/categories.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/checkouts.py` & `bigc-0.2.5/bigc/resources/checkouts.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/customer_groups.py` & `bigc-0.2.5/bigc/resources/customer_groups.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/customers.py` & `bigc-0.2.5/bigc/resources/customers.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/orders.py` & `bigc-0.2.5/bigc/resources/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,18 @@
         """Return an iterator for all order shipping addresses in an order"""
         return self._api.v2.get_many(f'/orders/{order_id}/shipping_addresses')
 
     def get_shipping_address(self, order_id: int, address_id: int) -> dict:
         """Get a specific shipping address in an order by ID"""
         return self._api.v2.get(f'/orders/{order_id}/shipping_addresses/{address_id}')
 
+    def update_shipping_address(self, order_id: int, address_id: int, **kwargs) -> dict:
+        """Update a specific shipping address in an order by ID"""
+        return self._api.v2.put(f'/orders/{order_id}/shipping_addresses/{address_id}', json=kwargs)
+
     def all_shipments(self, order_id: int) -> Iterator[dict]:
         """Returns all shipments for a specified order"""
 
         return self._api.v2.get_many(f'/orders/{order_id}/shipments')
 
     def create_shipment(self, order_id: int, *, order_address_id: int, items: list[dict], **kwargs) -> dict:
         """Creates an order shipment for the specified order"""
```

### Comparing `bigc-0.2.4/bigc/resources/product_variants.py` & `bigc-0.2.5/bigc/resources/product_variants.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/products.py` & `bigc-0.2.5/bigc/resources/products.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/resources/webhooks.py` & `bigc-0.2.5/bigc/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/bigc/utils.py` & `bigc-0.2.5/bigc/utils.py`

 * *Files identical despite different names*

### Comparing `bigc-0.2.4/pyproject.toml` & `bigc-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigc"
-version = "0.2.4"
+version = "0.2.5"
 description = "Unofficial client for the BigCommerce API"
 license = "MIT"
 authors = ["Ryan Thomson <ryan@medshift.com>", "Dillon Hartley <dillon@medshift.com>", "Adam Walsh <adam@medshift.com>"]
 readme = "README.md"
 homepage = "https://github.com/MedShift/bigc"
 repository = "https://github.com/MedShift/bigc.git"
 keywords = ["bigcommerce", "api", "client"]
```

### Comparing `bigc-0.2.4/setup.py` & `bigc-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bigc
+Version: 0.2.5
+Summary: Unofficial client for the BigCommerce API
+Home-page: https://github.com/MedShift/bigc
+License: MIT
+Keywords: bigcommerce,api,client
+Author: Ryan Thomson
+Author-email: ryan@medshift.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.27,<3.0)
+Project-URL: Repository, https://github.com/MedShift/bigc.git
+Description-Content-Type: text/markdown
 
-packages = \
-['bigc', 'bigc.data', 'bigc.resources']
+# bigc
 
-package_data = \
-{'': ['*']}
+An unofficial Python client for the BigCommerce API.
 
-install_requires = \
-['requests>=2.27,<3.0']
-
-setup_kwargs = {
-    'name': 'bigc',
-    'version': '0.2.4',
-    'description': 'Unofficial client for the BigCommerce API',
-    'long_description': "# bigc\n\nAn unofficial Python client for the BigCommerce API.\n\n_This project is currently in an alpha state._\n\n## Installation\n\n```shell\npip install bigc \n```\n\n## Usage\n\nTo authenticate, you'll need the BigCommerce store's hash and an access token.\n\n```python\nfrom bigc import BigCommerceAPI\n\n\nstore_hash = '000000000'\naccess_token = '0000000000000000000000000000000'\nbigcommerce = BigCommerceAPI(store_hash, access_token)\n\norder: dict = bigcommerce.orders.get(101)\norders: list[dict] = list(bigcommerce.orders.all(customer_id=1))\n```\n\nThe following resources are currently supported:\n\n- `carts`\n- `categories`\n- `checkouts`\n- `customer_groups`\n- `customers`\n- `orders`\n- `products`\n- `product_variants`\n- `webhooks`\n\n### Direct API Access\n\nFor resources or parameters that aren't officially supported yet, bigc also includes a flexible API client that can be used to make direct requests to the BigCommerce API.\n\n```python\nbigcommerce = BigCommerceAPI(store_hash, access_token)\n\nproduct = bigcommerce.api.v3.get('/products/77', params={'include': 'videos'})\norder_messages = bigcommerce.api.v2.get_many('/orders/101/messages')\n```\n\n### Utilities\n\nSome extra utility functions that don't interact with the BigCommerce API are available in `bigc.utils`.\n\n- `bigc.utils.parse_rfc2822_date`: Convert an [RFC-2822 date] (used by some BigCommerce APIs) to a `datetime`\n\n[RFC-2822 date]: https://www.rfc-editor.org/rfc/rfc2822#section-3.3\n\n### Constants\n\nFor convenience, some constants are made available in `bigc.data`.\n\n- `bigc.data.BigCommerceOrderStatus`: An `Enum` of order statuses and their IDs\n",
-    'author': 'Ryan Thomson',
-    'author_email': 'ryan@medshift.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/MedShift/bigc',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+_This project is currently in an alpha state._
 
+## Installation
+
+```shell
+pip install bigc 
+```
+
+## Usage
+
+To authenticate, you'll need the BigCommerce store's hash and an access token.
+
+```python
+from bigc import BigCommerceAPI
+
+
+store_hash = '000000000'
+access_token = '0000000000000000000000000000000'
+bigcommerce = BigCommerceAPI(store_hash, access_token)
+
+order: dict = bigcommerce.orders.get(101)
+orders: list[dict] = list(bigcommerce.orders.all(customer_id=1))
+```
+
+The following resources are currently supported:
+
+- `carts`
+- `categories`
+- `checkouts`
+- `customer_groups`
+- `customers`
+- `orders`
+- `products`
+- `product_variants`
+- `webhooks`
+
+### Direct API Access
+
+For resources or parameters that aren't officially supported yet, bigc also includes a flexible API client that can be used to make direct requests to the BigCommerce API.
+
+```python
+bigcommerce = BigCommerceAPI(store_hash, access_token)
+
+product = bigcommerce.api.v3.get('/products/77', params={'include': 'videos'})
+order_messages = bigcommerce.api.v2.get_many('/orders/101/messages')
+```
+
+### Utilities
+
+Some extra utility functions that don't interact with the BigCommerce API are available in `bigc.utils`.
+
+- `bigc.utils.parse_rfc2822_date`: Convert an [RFC-2822 date] (used by some BigCommerce APIs) to a `datetime`
+
+[RFC-2822 date]: https://www.rfc-editor.org/rfc/rfc2822#section-3.3
+
+### Constants
+
+For convenience, some constants are made available in `bigc.data`.
+
+- `bigc.data.BigCommerceOrderStatus`: An `Enum` of order statuses and their IDs
 
-setup(**setup_kwargs)
```

