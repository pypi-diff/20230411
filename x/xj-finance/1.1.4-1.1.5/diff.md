# Comparing `tmp/xj_finance-1.1.4.tar.gz` & `tmp/xj_finance-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_finance-1.1.4.tar", last modified: Tue Apr 11 06:59:34 2023, max compression
+gzip compressed data, was "dist\xj_finance-1.1.5.tar", last modified: Tue Apr 11 08:23:18 2023, max compression
```

## Comparing `xj_finance-1.1.4.tar` & `xj_finance-1.1.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/
--rw-rw-rw-   0        0        0     1990 2023-04-11 06:59:34.000000 xj_finance-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 06:59:34.000000 xj_finance-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-04-11 06:59:28.000000 xj_finance-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/__init__.py
--rw-rw-rw-   0        0        0     3115 2023-04-11 05:03:36.000000 xj_finance-1.1.4/xj_finance/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/apis/__init__.py
--rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.4/xj_finance/apis/finance_apis.py
--rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.4/xj_finance/apis/finance_balance.py
--rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.4/xj_finance/apis/finance_contact_book.py
--rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.4/xj_finance/apis/finance_currency.py
--rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.4/xj_finance/apis/finance_export.py
--rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.4/xj_finance/apis/finance_pay_mode.py
--rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.4/xj_finance/apis/finance_sand_box.py
--rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.4/xj_finance/apis/finance_statistic.py
--rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.4/xj_finance/apis/finance_status_code.py
--rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.4/xj_finance/apis/finance_transact.py
--rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.4/xj_finance/apis/finance_transacts.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.4/xj_finance/apis/router.py
--rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.4/xj_finance/apps.py
--rw-rw-rw-   0        0        0     9246 2023-04-11 03:24:33.000000 xj_finance-1.1.4/xj_finance/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/services/__init__.py
--rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.4/xj_finance/services/finance_currency_service.py
--rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.4/xj_finance/services/finance_list_service.py
--rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.4/xj_finance/services/finance_pay_mode_service.py
--rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.4/xj_finance/services/finance_sand_box_service.py
--rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.4/xj_finance/services/finance_service v1.py
--rw-rw-rw-   0        0        0    10054 2023-04-11 02:20:14.000000 xj_finance-1.1.4/xj_finance/services/finance_service.py
--rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.4/xj_finance/services/finance_statistic_service.py
--rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.4/xj_finance/services/finance_status_code_service.py
--rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.4/xj_finance/services/finance_transact_service v1.py
--rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.4/xj_finance/services/finance_transact_service v2.py
--rw-rw-rw-   0        0        0    29400 2023-04-11 06:58:55.000000 xj_finance-1.1.4/xj_finance/services/finance_transact_service.py
--rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.4/xj_finance/services/finance_transacts_service v1.py
--rw-rw-rw-   0        0        0    17590 2023-04-11 06:21:51.000000 xj_finance-1.1.4/xj_finance/services/finance_transacts_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/tests.py
--rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.4/xj_finance/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.4/xj_finance/utils/custom_response.py
--rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.4/xj_finance/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.4/xj_finance/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.4/xj_finance/utils/j_dict.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.4/xj_finance/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.4/xj_finance/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.4/xj_finance/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.4/xj_finance/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-11 06:59:34.000000 xj_finance-1.1.4/xj_finance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 08:23:18.000000 xj_finance-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:23:18.000000 xj_finance-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-04-11 08:22:53.000000 xj_finance-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-04-11 05:03:36.000000 xj_finance-1.1.5/xj_finance/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/apis/__init__.py
+-rw-rw-rw-   0        0        0     5602 2023-04-11 08:13:45.000000 xj_finance-1.1.5/xj_finance/apis/finance_apis.py
+-rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.5/xj_finance/apis/finance_balance.py
+-rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.5/xj_finance/apis/finance_contact_book.py
+-rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.5/xj_finance/apis/finance_currency.py
+-rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.5/xj_finance/apis/finance_export.py
+-rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.5/xj_finance/apis/finance_pay_mode.py
+-rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.5/xj_finance/apis/finance_sand_box.py
+-rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.5/xj_finance/apis/finance_statistic.py
+-rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.5/xj_finance/apis/finance_status_code.py
+-rw-rw-rw-   0        0        0     5422 2023-04-11 08:12:57.000000 xj_finance-1.1.5/xj_finance/apis/finance_transact.py
+-rw-rw-rw-   0        0        0     4665 2023-04-11 08:11:15.000000 xj_finance-1.1.5/xj_finance/apis/finance_transacts.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.5/xj_finance/apis/router.py
+-rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.5/xj_finance/apps.py
+-rw-rw-rw-   0        0        0     9246 2023-04-11 03:24:33.000000 xj_finance-1.1.5/xj_finance/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/services/__init__.py
+-rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.5/xj_finance/services/finance_currency_service.py
+-rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.5/xj_finance/services/finance_list_service.py
+-rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.5/xj_finance/services/finance_pay_mode_service.py
+-rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.5/xj_finance/services/finance_sand_box_service.py
+-rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.5/xj_finance/services/finance_service v1.py
+-rw-rw-rw-   0        0        0    10054 2023-04-11 02:20:14.000000 xj_finance-1.1.5/xj_finance/services/finance_service.py
+-rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.5/xj_finance/services/finance_statistic_service.py
+-rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.5/xj_finance/services/finance_status_code_service.py
+-rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.5/xj_finance/services/finance_transact_service v1.py
+-rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.5/xj_finance/services/finance_transact_service v2.py
+-rw-rw-rw-   0        0        0    29412 2023-04-11 08:20:29.000000 xj_finance-1.1.5/xj_finance/services/finance_transact_service.py
+-rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.5/xj_finance/services/finance_transacts_service v1.py
+-rw-rw-rw-   0        0        0    17590 2023-04-11 06:21:51.000000 xj_finance-1.1.5/xj_finance/services/finance_transacts_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/tests.py
+-rw-rw-rw-   0        0        0     2643 2023-04-11 08:15:33.000000 xj_finance-1.1.5/xj_finance/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.5/xj_finance/utils/custom_response.py
+-rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.5/xj_finance/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.5/xj_finance/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.5/xj_finance/utils/j_dict.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.5/xj_finance/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.5/xj_finance/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.5/xj_finance/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.5/xj_finance/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance.egg-info/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 08:23:18.000000 xj_finance-1.1.5/xj_finance.egg-info/top_level.txt
```

### Comparing `xj_finance-1.1.4/PKG-INFO` & `xj_finance-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_finance
-Version: 1.1.4
+Version: 1.1.5
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.4/README.md` & `xj_finance-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/setup.py` & `xj_finance-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_finance',  # 模块名称
-    version='1.1.4',  # 模块版本
+    version='1.1.5',  # 模块版本
     description='资金模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer=["莫小瑛", "高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_finance-1.1.4/xj_finance/admin.py` & `xj_finance-1.1.5/xj_finance/admin.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_balance.py` & `xj_finance-1.1.5/xj_finance/apis/finance_balance.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_contact_book.py` & `xj_finance-1.1.5/xj_finance/apis/finance_contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_currency.py` & `xj_finance-1.1.5/xj_finance/apis/finance_currency.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_export.py` & `xj_finance-1.1.5/xj_finance/apis/finance_export.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_pay_mode.py` & `xj_finance-1.1.5/xj_finance/apis/finance_pay_mode.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_sand_box.py` & `xj_finance-1.1.5/xj_finance/apis/finance_sand_box.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_statistic.py` & `xj_finance-1.1.5/xj_finance/apis/finance_statistic.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_status_code.py` & `xj_finance-1.1.5/xj_finance/apis/finance_status_code.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_transact.py` & `xj_finance-1.1.5/xj_finance/apis/finance_transact.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         token = self.request.META.get('HTTP_AUTHORIZATION', '')
         if not token:
             return util_response(err=4001, msg='缺少Token')
         data, err_txt = UserService.check_token(token)
         if not data:
             return util_response(err=4002, msg=err_txt)
         params = parse_data(request)
-        if not params.get("account_id",None):
+        if not params.get("account_id", None):
             params['account_id'] = data['user_id']
         if not params:
             return util_response(err=6046, msg='至少需要一个请求参数')
         data, err_txt = FinanceTransactService.post(params)
         if err_txt is None:
             return util_response(data=data)
         return util_response(err=47767, msg=err_txt)
@@ -124,8 +124,8 @@
     @request_params_wrapper
     def balance_validation(self, *args, user_info=None, request_params=None, **kwargs):
         if request_params is None:
             request_params = {}
         data, err_txt = FinanceService.balance_validation(request_params)
         if err_txt is None:
             return util_response(data=data)
-        return util_response(err=47767, msg=err_txt)
+        return util_response(err=47767, msg=err_txt)
```

### Comparing `xj_finance-1.1.4/xj_finance/apis/finance_transacts.py` & `xj_finance-1.1.5/xj_finance/apis/finance_transacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,7 +120,9 @@
     # 应收应付生成
     def create_or_write_off(self):
         params = parse_data(self)
         data, err = FinanceTransactsService.finance_create_or_write_off(params)
         if err is None:
             return util_response(data=data)
         return util_response(err=47767, msg=err)
+
+
```

### Comparing `xj_finance-1.1.4/xj_finance/apis/middleware.py` & `xj_finance-1.1.5/xj_finance/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/apis/router.py` & `xj_finance-1.1.5/xj_finance/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/models.py` & `xj_finance-1.1.5/xj_finance/models.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_currency_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_currency_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_pay_mode_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_pay_mode_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_sand_box_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_sand_box_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_service v1.py` & `xj_finance-1.1.5/xj_finance/services/finance_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_statistic_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_statistic_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_status_code_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_status_code_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_transact_service v1.py` & `xj_finance-1.1.5/xj_finance/services/finance_transact_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_transact_service v2.py` & `xj_finance-1.1.5/xj_finance/services/finance_transact_service v2.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_transact_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_transact_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
         if enroll_id:
             item['enroll_id'] = enroll_id
         # 信息id
         if thread_id:
             item['thread_id'] = thread_id
         # 沙盒状态码
         if sand_box_status_code:
-            item['sand_box_status_code'] = sand_box_status_code
+            item['sand_box_status_code'] = str(upper(sand_box_status_code))
 
         # 判断资金状态码是否存在，并根据支付方式判断是否要从内部余额中扣款
         if finance_status_name:
             status_set = StatusCode.objects.filter(finance_status_name=finance_status_name).first()
             if not status_set:
                 return None, '资金状态码不存在'
             item['finance_status_code'] = status_set.finance_status_code
```

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_transacts_service v1.py` & `xj_finance-1.1.5/xj_finance/services/finance_transacts_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/services/finance_transacts_service.py` & `xj_finance-1.1.5/xj_finance/services/finance_transacts_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/urls.py` & `xj_finance-1.1.5/xj_finance/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     re_path(r'^currency/?$', FinanceCurrency.as_view(), ),
     re_path(r'^sand_box/?$', FinanceSandBox.as_view(), ),
     re_path(r'^contact_book/?$', UserContactBook.as_view(), ),
     re_path(r'^statistic/?$', FinanceStatistic.as_view(), ),
 
     re_path(r'^transacts/?$', FinanceApi.list, ),  # 财务交易列表
     re_path(r'^transact/?$', FinanceApi.detail, ),  # 财务交详细
+    re_path(r'^add/?$', FinanceApi.add, ),  # 财务交易添加
+    re_path(r'^edit/?$', FinanceApi.edit, ),  # 财务交易修改
     re_path(r'^balance/?$', FinanceApi.balance, ),  # 获取余额
     re_path(r'^cash_withdrawal/?$', FinanceApi.cash_withdrawal, ),  # 财务提现
     re_path(r'^large_transfer/?$', FinanceApi.large_transfer, ),  # 大额转账
     re_path(r'^examine_approve/?$', FinanceApi.examine_approve, ),  # 财务审批
 
     re_path(r'^write_off/?$', FinanceTransacts.large_transfer, ),
     re_path(r'^large_amount_audit/?$', FinanceTransacts.large_amount_audit, ),
```

### Comparing `xj_finance-1.1.4/xj_finance/utils/custom_response.py` & `xj_finance-1.1.5/xj_finance/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/utils/custom_tool.py` & `xj_finance-1.1.5/xj_finance/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/utils/j_config.py` & `xj_finance-1.1.5/xj_finance/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/utils/jt.py` & `xj_finance-1.1.5/xj_finance/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/utils/model_handle.py` & `xj_finance-1.1.5/xj_finance/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/utils/user_wrapper.py` & `xj_finance-1.1.5/xj_finance/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance/views.py` & `xj_finance-1.1.5/xj_finance/views.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.4/xj_finance.egg-info/PKG-INFO` & `xj_finance-1.1.5/xj_finance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-finance
-Version: 1.1.4
+Version: 1.1.5
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.4/xj_finance.egg-info/SOURCES.txt` & `xj_finance-1.1.5/xj_finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

