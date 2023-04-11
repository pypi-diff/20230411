# Comparing `tmp/promsoft_cdek_interface-0.1.1.tar.gz` & `tmp/promsoft_cdek_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_cdek_interface-0.1.1.tar", max compression
+gzip compressed data, was "promsoft_cdek_interface-0.1.2.tar", max compression
```

## Comparing `promsoft_cdek_interface-0.1.1.tar` & `promsoft_cdek_interface-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      313 2023-04-11 04:48:24.411279 promsoft_cdek_interface-0.1.1/README.md
--rw-r--r--   0        0        0      363 2023-04-11 04:48:24.411279 promsoft_cdek_interface-0.1.1/promsoft_cdek_interface/__init__.py
--rw-r--r--   0        0        0    20161 2023-04-11 04:48:24.411279 promsoft_cdek_interface-0.1.1/promsoft_cdek_interface/models.py
--rw-r--r--   0        0        0      473 2023-04-11 04:48:24.415279 promsoft_cdek_interface-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 promsoft_cdek_interface-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      313 2023-04-11 04:47:49.587553 promsoft_cdek_interface-0.1.2/README.md
+-rw-r--r--   0        0        0      363 2023-04-11 04:47:49.587553 promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/__init__.py
+-rw-r--r--   0        0        0    20275 2023-04-11 05:08:21.468321 promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/models.py
+-rw-r--r--   0        0        0      473 2023-04-11 05:08:21.468321 promsoft_cdek_interface-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 promsoft_cdek_interface-0.1.2/PKG-INFO
```

### Comparing `promsoft_cdek_interface-0.1.1/promsoft_cdek_interface/models.py` & `promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 
     passport_series: str | None = Field(
         None, max_length=255, description="Серия паспорта"
     )
     passport_number: str | None = Field(
         None, max_length=255, description="Номер паспорта"
     )
+    passport_type: str | None = Field(
+        None, max_length=255, description="Тип паспорта"
+    )
+
     passport_date_of_issue: Optional[datetime.date] = None  # Дата выдачи паспорта
     passport_organization: str | None = Field(
         None, max_length=255, description="Орган выдачи паспорта"
     )
     passport_date_of_birth: Optional[datetime.date] = None  # Дата рождения
 
     # Требования по паспортным данным удовлетворены (актуально для международных заказов):
```

### Comparing `promsoft_cdek_interface-0.1.1/PKG-INFO` & `promsoft_cdek_interface-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promsoft-cdek-interface
-Version: 0.1.1
+Version: 0.1.2
 Summary: An interface for CDEK HTTP API
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

