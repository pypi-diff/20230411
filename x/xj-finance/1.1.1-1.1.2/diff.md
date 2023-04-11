# Comparing `tmp/xj_finance-1.1.1.tar.gz` & `tmp/xj_finance-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_finance-1.1.1.tar", last modified: Mon Apr 10 05:04:18 2023, max compression
+gzip compressed data, was "dist\xj_finance-1.1.2.tar", last modified: Tue Apr 11 05:21:17 2023, max compression
```

## Comparing `xj_finance-1.1.1.tar` & `xj_finance-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/
--rw-rw-rw-   0        0        0     1990 2023-04-10 05:04:18.000000 xj_finance-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-10 05:04:18.000000 xj_finance-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-04-10 02:12:25.000000 xj_finance-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/__init__.py
--rw-rw-rw-   0        0        0     3227 2023-03-07 08:56:37.000000 xj_finance-1.1.1/xj_finance/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/apis/__init__.py
--rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.1/xj_finance/apis/finance_apis.py
--rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.1/xj_finance/apis/finance_balance.py
--rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.1/xj_finance/apis/finance_contact_book.py
--rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.1/xj_finance/apis/finance_currency.py
--rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.1/xj_finance/apis/finance_export.py
--rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.1/xj_finance/apis/finance_pay_mode.py
--rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.1/xj_finance/apis/finance_sand_box.py
--rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.1/xj_finance/apis/finance_statistic.py
--rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.1/xj_finance/apis/finance_status_code.py
--rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.1/xj_finance/apis/finance_transact.py
--rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.1/xj_finance/apis/finance_transacts.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.1/xj_finance/apis/router.py
--rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.1/xj_finance/apps.py
--rw-rw-rw-   0        0        0     9325 2023-04-06 08:07:37.000000 xj_finance-1.1.1/xj_finance/models.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/services/__init__.py
--rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.1/xj_finance/services/finance_currency_service.py
--rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.1/xj_finance/services/finance_list_service.py
--rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.1/xj_finance/services/finance_pay_mode_service.py
--rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.1/xj_finance/services/finance_sand_box_service.py
--rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.1/xj_finance/services/finance_service v1.py
--rw-rw-rw-   0        0        0     9753 2023-04-07 08:55:14.000000 xj_finance-1.1.1/xj_finance/services/finance_service.py
--rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.1/xj_finance/services/finance_statistic_service.py
--rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.1/xj_finance/services/finance_status_code_service.py
--rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service v1.py
--rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service v2.py
--rw-rw-rw-   0        0        0    29283 2023-04-07 09:07:47.000000 xj_finance-1.1.1/xj_finance/services/finance_transact_service.py
--rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.1/xj_finance/services/finance_transacts_service v1.py
--rw-rw-rw-   0        0        0    16760 2023-04-07 08:48:42.000000 xj_finance-1.1.1/xj_finance/services/finance_transacts_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/tests.py
--rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.1/xj_finance/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.1/xj_finance/utils/custom_response.py
--rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.1/xj_finance/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.1/xj_finance/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.1/xj_finance/utils/j_dict.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.1/xj_finance/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.1/xj_finance/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.1/xj_finance/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.1/xj_finance/views.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2023-04-10 05:04:18.000000 xj_finance-1.1.1/xj_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-10 05:04:17.000000 xj_finance-1.1.1/xj_finance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 05:21:17.000000 xj_finance-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2022-08-16 02:23:15.000000 xj_finance-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 05:21:17.000000 xj_finance-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-04-11 05:18:34.000000 xj_finance-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-04-11 05:03:36.000000 xj_finance-1.1.2/xj_finance/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/apis/__init__.py
+-rw-rw-rw-   0        0        0     4422 2023-04-07 01:43:10.000000 xj_finance-1.1.2/xj_finance/apis/finance_apis.py
+-rw-rw-rw-   0        0        0     2233 2023-04-06 05:13:05.000000 xj_finance-1.1.2/xj_finance/apis/finance_balance.py
+-rw-rw-rw-   0        0        0     3084 2022-08-26 08:45:38.000000 xj_finance-1.1.2/xj_finance/apis/finance_contact_book.py
+-rw-rw-rw-   0        0        0     1012 2022-08-26 02:55:22.000000 xj_finance-1.1.2/xj_finance/apis/finance_currency.py
+-rw-rw-rw-   0        0        0     4772 2022-08-26 02:40:58.000000 xj_finance-1.1.2/xj_finance/apis/finance_export.py
+-rw-rw-rw-   0        0        0     1430 2023-01-04 01:15:24.000000 xj_finance-1.1.2/xj_finance/apis/finance_pay_mode.py
+-rw-rw-rw-   0        0        0     1006 2022-08-24 07:41:31.000000 xj_finance-1.1.2/xj_finance/apis/finance_sand_box.py
+-rw-rw-rw-   0        0        0     1549 2022-08-24 09:06:59.000000 xj_finance-1.1.2/xj_finance/apis/finance_statistic.py
+-rw-rw-rw-   0        0        0     1021 2023-01-18 07:58:44.000000 xj_finance-1.1.2/xj_finance/apis/finance_status_code.py
+-rw-rw-rw-   0        0        0     5419 2023-04-06 08:10:44.000000 xj_finance-1.1.2/xj_finance/apis/finance_transact.py
+-rw-rw-rw-   0        0        0     4661 2023-04-07 08:45:23.000000 xj_finance-1.1.2/xj_finance/apis/finance_transacts.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_finance-1.1.2/xj_finance/apis/router.py
+-rw-rw-rw-   0        0        0      208 2022-09-19 06:40:42.000000 xj_finance-1.1.2/xj_finance/apps.py
+-rw-rw-rw-   0        0        0     9246 2023-04-11 03:24:33.000000 xj_finance-1.1.2/xj_finance/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/xj_finance/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/services/__init__.py
+-rw-rw-rw-   0        0        0     1296 2022-08-24 02:05:06.000000 xj_finance-1.1.2/xj_finance/services/finance_currency_service.py
+-rw-rw-rw-   0        0        0      454 2022-08-23 09:51:33.000000 xj_finance-1.1.2/xj_finance/services/finance_list_service.py
+-rw-rw-rw-   0        0        0     1526 2023-01-04 01:25:29.000000 xj_finance-1.1.2/xj_finance/services/finance_pay_mode_service.py
+-rw-rw-rw-   0        0        0      982 2023-03-07 08:57:01.000000 xj_finance-1.1.2/xj_finance/services/finance_sand_box_service.py
+-rw-rw-rw-   0        0        0    15239 2023-04-01 16:10:40.000000 xj_finance-1.1.2/xj_finance/services/finance_service v1.py
+-rw-rw-rw-   0        0        0    10054 2023-04-11 02:20:14.000000 xj_finance-1.1.2/xj_finance/services/finance_service.py
+-rw-rw-rw-   0        0        0     4787 2022-08-24 09:08:36.000000 xj_finance-1.1.2/xj_finance/services/finance_statistic_service.py
+-rw-rw-rw-   0        0        0      934 2023-01-18 08:16:12.000000 xj_finance-1.1.2/xj_finance/services/finance_status_code_service.py
+-rw-rw-rw-   0        0        0    25531 2022-10-25 08:56:34.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service v1.py
+-rw-rw-rw-   0        0        0    37592 2023-03-30 05:27:34.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service v2.py
+-rw-rw-rw-   0        0        0    29283 2023-04-07 09:07:47.000000 xj_finance-1.1.2/xj_finance/services/finance_transact_service.py
+-rw-rw-rw-   0        0        0    31989 2023-03-30 07:10:48.000000 xj_finance-1.1.2/xj_finance/services/finance_transacts_service v1.py
+-rw-rw-rw-   0        0        0    17537 2023-04-11 02:56:58.000000 xj_finance-1.1.2/xj_finance/services/finance_transacts_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/tests.py
+-rw-rw-rw-   0        0        0     2509 2023-04-07 09:10:32.000000 xj_finance-1.1.2/xj_finance/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:17.000000 xj_finance-1.1.2/xj_finance/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_finance-1.1.2/xj_finance/utils/custom_response.py
+-rw-rw-rw-   0        0        0    10868 2023-03-01 02:16:37.000000 xj_finance-1.1.2/xj_finance/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_finance-1.1.2/xj_finance/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_finance-1.1.2/xj_finance/utils/j_dict.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_finance-1.1.2/xj_finance/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_finance-1.1.2/xj_finance/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_finance-1.1.2/xj_finance/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_finance-1.1.2/xj_finance/views.py
+drwxrwxrwx   0        0        0        0 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/
+-rw-rw-rw-   0        0        0     1990 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-11 05:21:16.000000 xj_finance-1.1.2/xj_finance.egg-info/top_level.txt
```

### Comparing `xj_finance-1.1.1/PKG-INFO` & `xj_finance-1.1.2/xj_finance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xj_finance
-Version: 1.1.1
+Name: xj-finance
+Version: 1.1.2
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.1/README.md` & `xj_finance-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/setup.py` & `xj_finance-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_finance',  # 模块名称
-    version='1.1.1',  # 模块版本
+    version='1.1.2',  # 模块版本
     description='资金模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='赵向明',  # 作者
     author_email='sieyoo@163.com',  # 作者邮箱
     maintainer=["莫小瑛", "高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_finance-1.1.1/xj_finance/admin.py` & `xj_finance-1.1.2/xj_finance/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,31 +32,29 @@
     fields = ('id', 'finance_status_code', 'finance_status_name', 'description',)
     list_display = ('id', 'finance_status_code', 'finance_status_name', 'description',)
     search_fields = ('id', 'finance_status_code', 'finance_status_name', 'description',)
     readonly_fields = ['id']
 
 
 class TransactAdmin(admin.ModelAdmin):
-    fields = ('id', 'account', 'their_account', 'transact_no', 'thread_id', 'enroll_id', 'transact_time', 'platform_id',
-              'order_no',
-              'opposite_account', 'summary', 'currency', 'income', 'outgo', 'balance', 'pay_mode', 'goods_info',
-              'pay_info', 'remark', 'images', 'sand_box', 'is_reverse', 'is_write_off', 'is_delete',
-              'sand_box_status_code', 'snapshot', 'finance_status_code')
-    list_display = (
-        'id', 'account', 'their_account', 'transact_no', 'thread_id', 'enroll_id', 'transact_time', 'platform_id',
-        'order_no',
-        'opposite_account', 'summary', 'currency', 'income', 'outgo', 'balance', 'pay_mode', 'goods_info',
-        'pay_info', 'remark', 'images', 'sand_box', 'is_reverse', 'is_write_off', 'is_delete', 'sand_box_status_code',
-        'finance_status_code')
+    fields = ('id', 'platform', 'thread', 'transact_no', 'enroll', 'enroll_record', 'order_no',
+              'account', 'their_account', 'transact_time', 'summary', 'currency', 'pay_mode', 'opposite_account',
+              'income',
+              'outgo',
+              'balance', 'goods_info', 'pay_info', 'remark', 'images', 'sand_box', 'finance_status_code',
+              'is_reverse', 'is_delete', 'is_write_off', 'sand_box_status_code', 'bookkeeping_type',)
+    list_display = ('id', 'platform_id', 'thread_id', 'transact_no', 'enroll_id', 'enroll_record_id', 'order_no',
+                    'account_id', 'their_account_id', 'transact_time', 'summary', 'currency_id', 'pay_mode_id', 'opposite_account',
+                    'income',
+                    'outgo',
+                    'balance', 'goods_info', 'pay_info', 'remark', 'images', 'sand_box_id', 'finance_status_code',
+                    'is_reverse', 'is_delete', 'is_write_off', 'sand_box_status_code', 'bookkeeping_type',)
     search_fields = (
         'id', 'account', 'their_account', 'transact_no', 'thread_id', 'enroll_id', 'transact_time', 'platform_id',
-        'order_no',
-        'opposite_account', 'summary', 'currency', 'income', 'outgo', 'balance', 'pay_mode', 'goods_info',
-        'pay_info', 'remark', 'images', 'sand_box', 'is_reverse', 'is_write_off', 'is_delete', 'sand_box_status_code',
-        'finance_status_code')
+        'order_no',)
     # list_filter = ['platform', 'currency', 'account', 'their_account', 'order_no']
     readonly_fields = ['id', 'transact_time']
     # def platform(self, obj):
     #     return obj.platform
 
     # 不起作用 https://docs.djangoproject.com/zh-hans/3.2/ref/contrib/admin/#django.contrib.admin.ModelAdmin.list_display
     # @admin.display(description='Name')
```

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_apis.py` & `xj_finance-1.1.2/xj_finance/apis/finance_apis.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_balance.py` & `xj_finance-1.1.2/xj_finance/apis/finance_balance.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_contact_book.py` & `xj_finance-1.1.2/xj_finance/apis/finance_contact_book.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_currency.py` & `xj_finance-1.1.2/xj_finance/apis/finance_currency.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_export.py` & `xj_finance-1.1.2/xj_finance/apis/finance_export.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_pay_mode.py` & `xj_finance-1.1.2/xj_finance/apis/finance_pay_mode.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_sand_box.py` & `xj_finance-1.1.2/xj_finance/apis/finance_sand_box.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_statistic.py` & `xj_finance-1.1.2/xj_finance/apis/finance_statistic.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_status_code.py` & `xj_finance-1.1.2/xj_finance/apis/finance_status_code.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_transact.py` & `xj_finance-1.1.2/xj_finance/apis/finance_transact.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/finance_transacts.py` & `xj_finance-1.1.2/xj_finance/apis/finance_transacts.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/middleware.py` & `xj_finance-1.1.2/xj_finance/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/apis/router.py` & `xj_finance-1.1.2/xj_finance/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/models.py` & `xj_finance-1.1.2/xj_finance/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
                                  on_delete=models.DO_NOTHING, unique=False, blank=True, null=True, db_index=True,
                                  db_constraint=False, )
     finance_status_code = models.CharField(verbose_name='资金状态码', default='', max_length=32, blank=True, null=True)
     is_reverse = models.BooleanField(verbose_name='是否红冲', blank=True, null=True)
     is_delete = models.BooleanField(verbose_name='是否删除', blank=True, null=True)
     is_write_off = models.BooleanField(verbose_name='是否核销', max_length=255, blank=True, null=True)
     sand_box_status_code = models.CharField(verbose_name='沙盒状态码', max_length=32, blank=True, null=True)
-    snapshot = models.JSONField(verbose_name='快照', blank=True, null=True)
     bookkeeping_type = models.CharField(verbose_name='记账类型', blank=True, null=True, max_length=1000)
 
     class Meta:
         db_table = 'finance_transact'
         verbose_name_plural = "1. 财务 - 交易明细"
 
     def to_dict(self):
```

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_currency_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_currency_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_pay_mode_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_pay_mode_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_sand_box_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_sand_box_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_service v1.py` & `xj_finance-1.1.2/xj_finance/services/finance_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
 import time
 import os
 import datetime
 
 from django.db.models import Q
 from django.db.models import F
 from django.forms import model_to_dict
+
 from xj_user.services.user_platform_service import UserPlatformService
 from ..models import *
 from ..models import StatusCode
 
 from decimal import Decimal
 from ..utils.custom_tool import format_params_handle
 
@@ -83,15 +85,18 @@
         if sand_box is None:
             transact_set_new = transact_set_new.filter(Q(sand_box__sand_box_name__isnull=True))
         else:
             transact_set_new = transact_set_new.filter(Q(sand_box__sand_box_name=sand_box))
         transact_set_new = transact_set_new.order_by('-transact_time').first()
         if transact_set_new:
             transact_set_new = model_to_dict(transact_set_new)
-            return {"balance": transact_set_new['balance']}
+            if not sys.modules.get("xj_finance.service.finance_transact_service.FinanceTransactService"):
+                from xj_finance.services.finance_transact_service import FinanceTransactService
+                balance = FinanceTransactService.keep_two_decimal_places(transact_set_new['balance'])
+            return {"balance": balance}
 
         return {"balance": 0}
 
         # return True
 
     # 生成交易号：2位数（当前年份后2位数字）+8位数（当前时间戳去头2位）+6位数（用户名 经过hash crc16生成的 4位十六进制 转成5位数 然后头为补0）
     @staticmethod
```

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_statistic_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_statistic_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_status_code_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_status_code_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_transact_service v1.py` & `xj_finance-1.1.2/xj_finance/services/finance_transact_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_transact_service v2.py` & `xj_finance-1.1.2/xj_finance/services/finance_transact_service v2.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_transact_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_transact_service.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_transacts_service v1.py` & `xj_finance-1.1.2/xj_finance/services/finance_transacts_service v1.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/services/finance_transacts_service.py` & `xj_finance-1.1.2/xj_finance/services/finance_transacts_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,33 +100,44 @@
         # ========== 四、相关前置业务逻辑处理 ==========
 
         # ========== 五、翻页 ==========
 
         page = int(params['page']) - 1 if 'page' in params else 0
         size = int(params['size']) if 'size' in params else 10
         #
+        if not sys.modules.get("xj_finance.service.finance_transact_service.FinanceTransactService"):
+            from xj_finance.services.finance_transact_service import FinanceTransactService
         total = transacts.count()
         income = transacts.aggregate(income=Sum("income"))
         outgo = transacts.aggregate(outgo=Sum("outgo"))
         #
         current_page_set = transacts[page * size: page * size + size] if page >= 0 and size > 0 else transacts
         res_list = []
+
         for i, it in enumerate(current_page_set):
             it['order'] = page * size + i + 1
-            it['amount'] = it['income'] if it['income'] > 0 else -abs(float(it['outgo']))
+            it['income'] = FinanceTransactService.keep_two_decimal_places(it['income'])
+            it['outgo'] = FinanceTransactService.keep_two_decimal_places(it['outgo'])
+            it['balance'] = FinanceTransactService.keep_two_decimal_places(it['balance'])
+            it['amount'] = it['income'] if float(it['income']) > 0 else FinanceTransactService.keep_two_decimal_places(
+                -abs(float(it['outgo'])))
             res_list.append(it)
         data = res_list
         thread_id_list = [item.get("thread_id", None) for item in res_list]
         thread_list, err = ThreadListService.search(thread_id_list)
         if thread_list:
             data = JoinList(res_list, thread_list, "thread_id", "id").join()
 
+        income = income.get("income", 0.0)
+        outgo = outgo.get("outgo", 0.0)
         statistics = {
-            "income": income.get("income", 0.0) if income.get("income", 0.0) else 0.0,
-            "outgo": outgo.get("outgo", 0.0) if outgo.get("outgo", 0.0) else 0.0,
+            "income": FinanceTransactService.keep_two_decimal_places(
+                income) if FinanceTransactService.keep_two_decimal_places(income) else 0.0,
+            "outgo": FinanceTransactService.keep_two_decimal_places(
+                outgo) if FinanceTransactService.keep_two_decimal_places(outgo) else 0.0,
         }
         return {'size': int(size), 'page': int(page + 1), 'total': total, 'list': data, "statistics": statistics}, None
 
     @staticmethod
     def detail(pk=None, order_no=None, transact_no=None, field_list=None):
         """
         查询订单-单笔订单
```

### Comparing `xj_finance-1.1.1/xj_finance/urls.py` & `xj_finance-1.1.2/xj_finance/urls.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/custom_response.py` & `xj_finance-1.1.2/xj_finance/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/custom_tool.py` & `xj_finance-1.1.2/xj_finance/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/j_config.py` & `xj_finance-1.1.2/xj_finance/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/jt.py` & `xj_finance-1.1.2/xj_finance/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/model_handle.py` & `xj_finance-1.1.2/xj_finance/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/utils/user_wrapper.py` & `xj_finance-1.1.2/xj_finance/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance/views.py` & `xj_finance-1.1.2/xj_finance/views.py`

 * *Files identical despite different names*

### Comparing `xj_finance-1.1.1/xj_finance.egg-info/PKG-INFO` & `xj_finance-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xj-finance
-Version: 1.1.1
+Name: xj_finance
+Version: 1.1.2
 Summary: 资金模块
 Home-page: UNKNOWN
 Author: 赵向明
 Author-email: sieyoo@163.com
 Maintainer: ['莫小瑛', '高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
```

### Comparing `xj_finance-1.1.1/xj_finance.egg-info/SOURCES.txt` & `xj_finance-1.1.2/xj_finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

