# Comparing `tmp/xj_finance-1.1.2.tar.gz` & `tmp/xj_finance-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_finance-1.1.2.tar", last modified: Tue Apr 11 05:21:17 2023, max compression
+gzip compressed data, was "dist\xj_finance-1.1.3.tar", last modified: Tue Apr 11 06:35:49 2023, max compression
```

## Comparing `xj_finance-1.1.2.tar` & `xj_finance-1.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/
--rw-rw-rw-   0        0        0     1990 2023-04-11 05:21:17.000000 xj_finance-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 05:21:17.000000 xj_finance-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-04-11 05:18:34.000000 xj_finance-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/__init__.py
--rw-rw-rw-   0        0        0     3115 2023-04-11 05:03:36.000000 xj_finance-1.1.2/xj_finance/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/apis/__init__.py
--rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.2/xj_finance/apis/finance_apis.py
--rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.2/xj_finance/apis/finance_balance.py
--rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.2/xj_finance/apis/finance_contact_book.py
--rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.2/xj_finance/apis/finance_currency.py
--rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.2/xj_finance/apis/finance_export.py
--rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.2/xj_finance/apis/finance_pay_mode.py
--rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.2/xj_finance/apis/finance_sand_box.py
--rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.2/xj_finance/apis/finance_statistic.py
--rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.2/xj_finance/apis/finance_status_code.py
--rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.2/xj_finance/apis/finance_transact.py
--rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.2/xj_finance/apis/finance_transacts.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.2/xj_finance/apis/router.py
--rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.2/xj_finance/apps.py
--rw-rw-rw-   0        0        0     9246 2023-04-11 03:24:33.000000 xj_finance-1.1.2/xj_finance/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/xj_finance/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/services/__init__.py
--rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.2/xj_finance/services/finance_currency_service.py
--rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.2/xj_finance/services/finance_list_service.py
--rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.2/xj_finance/services/finance_pay_mode_service.py
--rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.2/xj_finance/services/finance_sand_box_service.py
--rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.2/xj_finance/services/finance_service v1.py
--rw-rw-rw-   0        0        0    10054 2023-04-11 02:20:14.000000 xj_finance-1.1.2/xj_finance/services/finance_service.py
--rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.2/xj_finance/services/finance_statistic_service.py
--rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.2/xj_finance/services/finance_status_code_service.py
--rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service v1.py
--rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service v2.py
--rw-rw-rw-   0        0        0    29283 2023-04-07 09:07:47.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service.py
--rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.2/xj_finance/services/finance_transacts_service v1.py
--rw-rw-rw-   0        0        0    17537 2023-04-11 02:56:58.000000 xj_finance-1.1.2/xj_finance/services/finance_transacts_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/tests.py
--rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.2/xj_finance/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/xj_finance/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.2/xj_finance/utils/custom_response.py
--rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.2/xj_finance/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.2/xj_finance/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.2/xj_finance/utils/j_dict.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.2/xj_finance/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.2/xj_finance/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.2/xj_finance/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 06:35:49.000000 xj_finance-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 06:35:49.000000 xj_finance-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-04-11 06:35:46.000000 xj_finance-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-04-11 05:03:36.000000 xj_finance-1.1.3/xj_finance/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/apis/__init__.py
+-rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.3/xj_finance/apis/finance_apis.py
+-rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.3/xj_finance/apis/finance_balance.py
+-rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.3/xj_finance/apis/finance_contact_book.py
+-rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.3/xj_finance/apis/finance_currency.py
+-rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.3/xj_finance/apis/finance_export.py
+-rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.3/xj_finance/apis/finance_pay_mode.py
+-rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.3/xj_finance/apis/finance_sand_box.py
+-rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.3/xj_finance/apis/finance_statistic.py
+-rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.3/xj_finance/apis/finance_status_code.py
+-rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.3/xj_finance/apis/finance_transact.py
+-rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.3/xj_finance/apis/finance_transacts.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.3/xj_finance/apis/router.py
+-rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.3/xj_finance/apps.py
+-rw-rw-rw-   0        0        0     9246 2023-04-11 03:24:33.000000 xj_finance-1.1.3/xj_finance/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/services/__init__.py
+-rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.3/xj_finance/services/finance_currency_service.py
+-rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.3/xj_finance/services/finance_list_service.py
+-rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.3/xj_finance/services/finance_pay_mode_service.py
+-rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.3/xj_finance/services/finance_sand_box_service.py
+-rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.3/xj_finance/services/finance_service v1.py
+-rw-rw-rw-   0        0        0    10054 2023-04-11 02:20:14.000000 xj_finance-1.1.3/xj_finance/services/finance_service.py
+-rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.3/xj_finance/services/finance_statistic_service.py
+-rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.3/xj_finance/services/finance_status_code_service.py
+-rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.3/xj_finance/services/finance_transact_service v1.py
+-rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.3/xj_finance/services/finance_transact_service v2.py
+-rw-rw-rw-   0        0        0    29459 2023-04-11 06:35:00.000000 xj_finance-1.1.3/xj_finance/services/finance_transact_service.py
+-rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.3/xj_finance/services/finance_transacts_service v1.py
+-rw-rw-rw-   0        0        0    17590 2023-04-11 06:21:51.000000 xj_finance-1.1.3/xj_finance/services/finance_transacts_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/tests.py
+-rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.3/xj_finance/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.3/xj_finance/utils/custom_response.py
+-rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.3/xj_finance/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.3/xj_finance/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.3/xj_finance/utils/j_dict.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.3/xj_finance/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.3/xj_finance/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.3/xj_finance/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.3/xj_finance/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance.egg-info/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 06:35:49.000000 xj_finance-1.1.3/xj_finance.egg-info/top_level.txt
```

### Comparing `xj_finance-1.1.2/PKG-INFO` & `xj_finance-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_finance
-Version: 1.1.2
+Version: 1.1.3
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.2/README.md` & `xj_finance-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/setup.py` & `xj_finance-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_finance',  # 模块名称
-    version='1.1.2',  # 模块版本
+    version='1.1.3',  # 模块版本
     description='资金模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer=["莫小瑛", "高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_finance-1.1.2/xj_finance/admin.py` & `xj_finance-1.1.3/xj_finance/admin.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_apis.py` & `xj_finance-1.1.3/xj_finance/apis/finance_apis.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_balance.py` & `xj_finance-1.1.3/xj_finance/apis/finance_balance.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_contact_book.py` & `xj_finance-1.1.3/xj_finance/apis/finance_contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_currency.py` & `xj_finance-1.1.3/xj_finance/apis/finance_currency.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_export.py` & `xj_finance-1.1.3/xj_finance/apis/finance_export.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_pay_mode.py` & `xj_finance-1.1.3/xj_finance/apis/finance_pay_mode.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_sand_box.py` & `xj_finance-1.1.3/xj_finance/apis/finance_sand_box.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_statistic.py` & `xj_finance-1.1.3/xj_finance/apis/finance_statistic.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_status_code.py` & `xj_finance-1.1.3/xj_finance/apis/finance_status_code.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_transact.py` & `xj_finance-1.1.3/xj_finance/apis/finance_transact.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/finance_transacts.py` & `xj_finance-1.1.3/xj_finance/apis/finance_transacts.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/middleware.py` & `xj_finance-1.1.3/xj_finance/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/apis/router.py` & `xj_finance-1.1.3/xj_finance/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/models.py` & `xj_finance-1.1.3/xj_finance/models.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_currency_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_currency_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_pay_mode_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_pay_mode_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_sand_box_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_sand_box_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_service v1.py` & `xj_finance-1.1.3/xj_finance/services/finance_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_statistic_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_statistic_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_status_code_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_status_code_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_transact_service v1.py` & `xj_finance-1.1.3/xj_finance/services/finance_transact_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_transact_service v2.py` & `xj_finance-1.1.3/xj_finance/services/finance_transact_service v2.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_transact_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_transact_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,28 +85,28 @@
         now_time = timezone.now().astimezone(tz=tz).strftime("%Y-%m-%d %H:%M:%S")
         now = datetime.strptime(now_time, '%Y-%m-%d %H:%M:%S')
         return now
 
     @staticmethod
     def keep_two_decimal_places(str_num):
         result_num = format(float(str_num), ",")
+
         if len(result_num.split(".")[-1]) < 2:
             result_num = result_num + "0"
         return result_num
 
     # 资金检查
     @staticmethod
     def balance_check(account_id, platform, currency, amount, account_wechat_appid=None):
         # 根据账户id查询
         if account_id:
             account, account_err = DetailInfoService.get_detail(account_id)
         # 根据平台用户查询
         elif account_wechat_appid:
             account, account_err = UserSsoServeService.user_sso_serve(account_wechat_appid)
-
         if account_err:
             return None, '用户不存在'
         balance = FinanceService.check_balance(account_id=account['user_id'], platform=platform,
                                                currency=currency,
                                                sand_box=None)
         if float(balance['balance']) < float(amount):
             return None, "余额不足,当前余额：【 " + str(
@@ -197,15 +197,14 @@
 
         if goods_info:
             user_finance_data['goods_info'] = goods_info
             platform_finance_data['goods_info'] = goods_info
         if sand_box_status_code:
             user_finance_data['sand_box_status_code'] = str(upper(sand_box_status_code))
             platform_finance_data['sand_box_status_code'] = str(upper(sand_box_status_code))
-
         if images:
             user_finance_data['images'] = images
             platform_finance_data['images'] = images
         # 充值行为 TOP_UP （线上支付 生成真实记录）| OFFLINE（线下支付 生成沙盒记录 审核成功后核销沙盒 生成真实记录）
         if finance_type == "TOP_UP" or finance_type == "OFFLINE":
             try:
                 user_finance_data['bookkeeping_type'] = "TOP_UP"  # 充值行为
@@ -292,26 +291,28 @@
 
             user_finance_data['sand_box'] = sand_box_cash_withdrawal  # 提现
             user_finance_data['amount'] = -abs(float(amount))
             user_finance_data['order_no'] = FinanceService.make_unicode()
             user_finance_data['transact_no'] = FinanceService.make_unicode(str(user_finance_data['account_id']))
             user_finance_data['bookkeeping_type'] = "WITHDRAW"  # 提现行为
             user_finance_data['sand_box_status_code'] = "WITHDRAWING"  # 沙盒状态码 WITHDRAWING 提现中
+            user_finance_data['finance_status_name'] = "已评价"  # 资金状态码
             user_finance_data['summary'] = "【" + user_set['full_name'] + "】" + " 提现 " + str(amount) + " 元"
             user_add_data, user_err_txt = FinanceTransactService.add(user_finance_data)
             if user_err_txt:
                 return None, user_err_txt
             platform_finance_data['sand_box'] = sand_box_cash_withdrawal  # 提现
             platform_finance_data['amount'] = -abs(float(amount))
             platform_finance_data['order_no'] = FinanceService.make_unicode()
             platform_finance_data['transact_no'] = FinanceService.make_unicode(
                 str(platform_finance_data['account_wechat_appid']))
             platform_finance_data['bookkeeping_type'] = "WITHDRAW"  # 提现行为
             platform_finance_data['change'] = False  # 是否变动
             platform_finance_data['sand_box_status_code'] = "WITHDRAWING"  # 沙盒状态码 WITHDRAWING 提现中
+            platform_finance_data['finance_status_name'] = "已评价"  # 资金状态码
             platform_finance_data['summary'] = "【" + user_set['full_name'] + "】" + " 提现 " + str(amount) + " 元"
             platform_add_data, err_txt = FinanceTransactService.add(platform_finance_data)
 
             if err_txt:
                 return None, err_txt
             return user_finance_data['order_no'], None
         else:
```

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_transacts_service v1.py` & `xj_finance-1.1.3/xj_finance/services/finance_transacts_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/services/finance_transacts_service.py` & `xj_finance-1.1.3/xj_finance/services/finance_transacts_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,33 +111,34 @@
         outgo = transacts.aggregate(outgo=Sum("outgo"))
         #
         current_page_set = transacts[page * size: page * size + size] if page >= 0 and size > 0 else transacts
         res_list = []
 
         for i, it in enumerate(current_page_set):
             it['order'] = page * size + i + 1
-            it['income'] = FinanceTransactService.keep_two_decimal_places(it['income'])
-            it['outgo'] = FinanceTransactService.keep_two_decimal_places(it['outgo'])
             it['balance'] = FinanceTransactService.keep_two_decimal_places(it['balance'])
-            it['amount'] = it['income'] if float(it['income']) > 0 else FinanceTransactService.keep_two_decimal_places(
+            it['amount'] = FinanceTransactService.keep_two_decimal_places(it['income']) if it[
+                                                                                               'income'] > 0 else FinanceTransactService.keep_two_decimal_places(
                 -abs(float(it['outgo'])))
+            it['income'] = FinanceTransactService.keep_two_decimal_places(it['income'])
+            it['outgo'] = FinanceTransactService.keep_two_decimal_places(it['outgo'])
             res_list.append(it)
         data = res_list
         thread_id_list = [item.get("thread_id", None) for item in res_list]
         thread_list, err = ThreadListService.search(thread_id_list)
         if thread_list:
             data = JoinList(res_list, thread_list, "thread_id", "id").join()
 
-        income = income.get("income", 0.0)
-        outgo = outgo.get("outgo", 0.0)
+        income = income.get("income", "0.0")
+        outgo = outgo.get("outgo", "0.00")
         statistics = {
             "income": FinanceTransactService.keep_two_decimal_places(
-                income) if FinanceTransactService.keep_two_decimal_places(income) else 0.0,
+                income) if income else "0.00",
             "outgo": FinanceTransactService.keep_two_decimal_places(
-                outgo) if FinanceTransactService.keep_two_decimal_places(outgo) else 0.0,
+                outgo) if outgo else "0.00",
         }
         return {'size': int(size), 'page': int(page + 1), 'total': total, 'list': data, "statistics": statistics}, None
 
     @staticmethod
     def detail(pk=None, order_no=None, transact_no=None, field_list=None):
         """
         查询订单-单笔订单
```

### Comparing `xj_finance-1.1.2/xj_finance/urls.py` & `xj_finance-1.1.3/xj_finance/urls.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/custom_response.py` & `xj_finance-1.1.3/xj_finance/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/custom_tool.py` & `xj_finance-1.1.3/xj_finance/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/j_config.py` & `xj_finance-1.1.3/xj_finance/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/jt.py` & `xj_finance-1.1.3/xj_finance/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/model_handle.py` & `xj_finance-1.1.3/xj_finance/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/utils/user_wrapper.py` & `xj_finance-1.1.3/xj_finance/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance/views.py` & `xj_finance-1.1.3/xj_finance/views.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.2/xj_finance.egg-info/PKG-INFO` & `xj_finance-1.1.3/xj_finance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-finance
-Version: 1.1.2
+Version: 1.1.3
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.2/xj_finance.egg-info/SOURCES.txt` & `xj_finance-1.1.3/xj_finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

