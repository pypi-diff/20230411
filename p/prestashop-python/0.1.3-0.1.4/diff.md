# Comparing `tmp/prestashop_python-0.1.3.tar.gz` & `tmp/prestashop_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prestashop_python-0.1.3.tar", max compression
+gzip compressed data, was "prestashop_python-0.1.4.tar", max compression
```

## Comparing `prestashop_python-0.1.3.tar` & `prestashop_python-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-02-16 14:28:30.190420 prestashop_python-0.1.3/LICENSE
--rw-r--r--   0        0        0     1459 2023-03-28 15:08:42.545620 prestashop_python-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-02-16 14:28:30.190705 prestashop_python-0.1.3/prestashop/__init__.py
--rw-r--r--   0        0        0     5341 2023-02-21 14:35:48.447087 prestashop_python-0.1.3/prestashop/client.py
--rw-r--r--   0        0        0      190 2023-02-16 14:28:30.190996 prestashop_python-0.1.3/prestashop/exceptions.py
--rw-r--r--   0        0        0      402 2023-03-28 15:09:33.414911 prestashop_python-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 prestashop_python-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-16 14:28:30.190420 prestashop_python-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1555 2023-04-11 18:14:43.604264 prestashop_python-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-02-16 14:28:30.190705 prestashop_python-0.1.4/prestashop/__init__.py
+-rw-r--r--   0        0        0     4749 2023-04-11 18:14:43.604887 prestashop_python-0.1.4/prestashop/client.py
+-rw-r--r--   0        0        0      190 2023-02-16 14:28:30.190996 prestashop_python-0.1.4/prestashop/exceptions.py
+-rw-r--r--   0        0        0      402 2023-04-11 18:14:43.605395 prestashop_python-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 prestashop_python-0.1.4/PKG-INFO
```

### Comparing `prestashop_python-0.1.3/LICENSE` & `prestashop_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prestashop_python-0.1.3/README.md` & `prestashop_python-0.1.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-![](https://img.shields.io/badge/version-0.1.2-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)
+
 # prestashop-python
+![](https://img.shields.io/badge/version-0.1.4-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *prestashop-python* is an API wrapper for Prestashop, written in Python.
 ## Installing
 ```
 pip install prestashop-python
 ```
 ## Usage
 ```
 client = Client(webservice_key, domain)
 ```
 ### Check API features
 ```
 response = client.check_api_features()
 ```
-### List service (customers, orders, carts, countries, states and addresses)
+### List service (customers, orders, carts, countries, states...)
 ```
-response = client.list_customers(service, filter_field=None, filter_operator=None, filter_value=None, is_date_filter=False,
+response = client.list_service(service, filter_field=None, filter_operator=None, filter_value=None, is_date_filter=False,
                                  sort_field=None, sort_order="ASC", limit=100)
-# Service current options are: "customers", "orders", "carts", "countries", "states", "addresses"
+# Some service options are: "customers", "orders", "carts", "countries", "states", "addresses"
 # Filter operation options = "!" not equal, "" equal, ">" greater than,"<" less than
 # set is_date_filter to True if you are filtering a date field.
 ```
+For a full list of available services, check: https://devdocs.prestashop-project.org/8/webservice/resources/
 ### List inactive carts
 ```
 response = client.list_inactive_carts(inactive_before, inactive_from=None, sort_field=None, sort_order="ASC", limit=100)
 # Checks all carts without an order and inactive before parameter 'inactive_before'.  
 # If 'inactive_from' is added, it will check inactive carts between inactive_from and inactive_before time.  
 # inactive_before and inactive_from format must be: 2023-02-13 13:31:28 (string).  
 # Sort order only works if sort_field is added.
```

### Comparing `prestashop_python-0.1.3/prestashop/client.py` & `prestashop_python-0.1.4/prestashop/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,41 +25,30 @@
         filter_value=None,
         is_date_filter=False,
         sort_field=None,
         sort_order="ASC",
         limit=100,
     ):
         """
-        Service current options are: "customers", "orders", "carts", "addresses", "countries", "states" \n
         Filter operation options = "!" not equal, "" equal, ">" greater than,"<" less than.\n
         Set is_date_filter to True if you are filtering a date field.
         """
         params = {"limit": limit, "display": "full"}
         if is_date_filter:
             params.update({"date": "1"})
         if filter_field and filter_operator is not None and filter_value:
             filter_value = filter_value.replace(" ", "%20")
             params.update({f"filter[{filter_field}]": f"{filter_operator}[{filter_value}]"})
         if sort_field:
             sort = {"sort": f"[{sort_field}_{sort_order}]"}
             params.update(sort)
-        if service == "customers":
-            return self.get("customers/", params=params)
-        elif service == "orders":
-            return self.get("orders/", params=params)
-        elif service == "carts":
-            return self.get("carts/", params=params)
-        elif service == "addresses":
-            return self.get("addresses/", params=params)
-        elif service == "countries":
-            return self.get("countries/", params=params)
-        elif service == "states":
-            return self.get("states/", params=params)
-        else:
-            return f"No {service} service available for search"
+        try:
+            return self.get(f"{service}/", params=params)
+        except WrongFormatInputError as e:
+            return e
 
     def list_inactive_carts(self, inactive_before, inactive_from=None, sort_field=None, sort_order="ASC", limit=100):
         """ 
         Checks all carts without an order and inactive before parameter 'inactive_before'. \n
         If 'inactive_from' is added, it will check inactive carts between inactive_from and inactive_before time. \n
         inactive_before and inactive_from format must be: 2023-02-13 13:31:28 (string). \n
         Sort order only works if sort_field is added.
```

### Comparing `prestashop_python-0.1.3/PKG-INFO` & `prestashop_python-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prestashop-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: API wrapper for Prestashop written in Python
 License: MIT
 Author: Juan Carlos Rios
 Author-email: juankrios15@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,38 +12,40 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-![](https://img.shields.io/badge/version-0.1.2-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)
+
 # prestashop-python
+![](https://img.shields.io/badge/version-0.1.4-success) ![](https://img.shields.io/badge/Python-3.8%20|%203.9%20|%203.10%20|%203.11-4B8BBE?logo=python&logoColor=white)  
 
 *prestashop-python* is an API wrapper for Prestashop, written in Python.
 ## Installing
 ```
 pip install prestashop-python
 ```
 ## Usage
 ```
 client = Client(webservice_key, domain)
 ```
 ### Check API features
 ```
 response = client.check_api_features()
 ```
-### List service (customers, orders, carts, countries, states and addresses)
+### List service (customers, orders, carts, countries, states...)
 ```
-response = client.list_customers(service, filter_field=None, filter_operator=None, filter_value=None, is_date_filter=False,
+response = client.list_service(service, filter_field=None, filter_operator=None, filter_value=None, is_date_filter=False,
                                  sort_field=None, sort_order="ASC", limit=100)
-# Service current options are: "customers", "orders", "carts", "countries", "states", "addresses"
+# Some service options are: "customers", "orders", "carts", "countries", "states", "addresses"
 # Filter operation options = "!" not equal, "" equal, ">" greater than,"<" less than
 # set is_date_filter to True if you are filtering a date field.
 ```
+For a full list of available services, check: https://devdocs.prestashop-project.org/8/webservice/resources/
 ### List inactive carts
 ```
 response = client.list_inactive_carts(inactive_before, inactive_from=None, sort_field=None, sort_order="ASC", limit=100)
 # Checks all carts without an order and inactive before parameter 'inactive_before'.  
 # If 'inactive_from' is added, it will check inactive carts between inactive_from and inactive_before time.  
 # inactive_before and inactive_from format must be: 2023-02-13 13:31:28 (string).  
 # Sort order only works if sort_field is added.
```

