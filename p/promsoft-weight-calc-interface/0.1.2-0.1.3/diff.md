# Comparing `tmp/promsoft_weight_calc_interface-0.1.2.tar.gz` & `tmp/promsoft_weight_calc_interface-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_weight_calc_interface-0.1.2.tar", max compression
+gzip compressed data, was "promsoft_weight_calc_interface-0.1.3.tar", max compression
```

## Comparing `promsoft_weight_calc_interface-0.1.2.tar` & `promsoft_weight_calc_interface-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      321 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.2/README.md
--rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.2/promsoft_weight_calc_interface/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.2/promsoft_weight_calc_interface/models.py
--rw-r--r--   0        0        0      521 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      477 2023-04-11 10:22:56.136598 promsoft_weight_calc_interface-0.1.3/README.md
+-rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/models.py
+-rw-r--r--   0        0        0      521 2023-04-11 10:22:56.136598 promsoft_weight_calc_interface-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.3/PKG-INFO
```

### Comparing `promsoft_weight_calc_interface-0.1.2/promsoft_weight_calc_interface/models.py` & `promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/models.py`

 * *Files identical despite different names*

### Comparing `promsoft_weight_calc_interface-0.1.2/pyproject.toml` & `promsoft_weight_calc_interface-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promsoft_weight_calc_interface"
-version = "0.1.2"
+version = "0.1.3"
 description = "Интерфейс для сервиса weight_calc."
 authors = ["Alena Chegodaikina <alena@promsoft.ru>"]
 readme = "README.md"
 packages = [{include = "promsoft_weight_calc_interface"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

