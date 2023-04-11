# Comparing `tmp/python_selenium_ctrl_package-0.0.90.tar.gz` & `tmp/python_selenium_ctrl_package-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_selenium_ctrl_package-0.0.90.tar", last modified: Thu Mar 30 09:49:39 2023, max compression
+gzip compressed data, was "python_selenium_ctrl_package-0.0.91.tar", last modified: Tue Apr 11 08:11:15 2023, max compression
```

## Comparing `python_selenium_ctrl_package-0.0.90.tar` & `python_selenium_ctrl_package-0.0.91.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.536554 python_selenium_ctrl_package-0.0.90/
--rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.90/LICENSE
--rw-rw-rw-   0        0        0     1177 2023-03-30 09:49:39.536554 python_selenium_ctrl_package-0.0.90/PKG-INFO
--rw-rw-rw-   0        0        0      683 2022-11-18 06:56:07.000000 python_selenium_ctrl_package-0.0.90/README.md
--rw-rw-rw-   0        0        0      947 2023-03-30 09:49:09.000000 python_selenium_ctrl_package-0.0.90/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 09:49:39.536554 python_selenium_ctrl_package-0.0.90/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.332647 python_selenium_ctrl_package-0.0.90/src/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.90/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.353738 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/
--rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.388601 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.393697 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/app/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/app/__init__.py
--rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/app/ports_conf.py
--rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/product_list.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.395697 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.404748 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/Website/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
--rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
--rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conf/rwd/__init__.py
--rw-rw-rw-   0        0        0    40500 2023-03-28 09:59:35.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conftest_base.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.416487 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.432499 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
--rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
--rw-rw-rw-   0        0        0     3327 2023-03-29 08:14:37.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
--rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
--rw-rw-rw-   0        0        0    16933 2022-11-21 09:45:38.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/driverfactory.py
--rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/main.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.460254 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/
--rw-rw-rw-   0        0        0    56689 2023-03-24 07:52:50.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/Base_Page.py
--rw-rw-rw-   0        0        0    25197 2023-03-21 17:06:12.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
--rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/__init__.py
--rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
--rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/zero_page.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.465795 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/remoteTest/
--rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/remoteTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.494430 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/__init__.py
--rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/email_conf.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.534547 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/
--rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
--rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
--rw-rw-rw-   0        0        0     8259 2023-03-28 09:48:42.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Wrapit.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/__init__.py
--rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
--rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
--rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/html_report_conf.py
--rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/remote_credentials.py
--rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/screenshot_conf.py
-drwxrwxrwx   0        0        0        0 2023-03-30 09:49:39.378303 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/
--rw-rw-rw-   0        0        0     1177 2023-03-30 09:49:39.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2378 2023-03-30 09:49:39.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 09:49:39.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      272 2023-03-30 09:49:39.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-03-30 09:49:39.000000 python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.144309 python_selenium_ctrl_package-0.0.91/
+-rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.91/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-04-11 08:11:15.143308 python_selenium_ctrl_package-0.0.91/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2022-11-18 06:56:07.000000 python_selenium_ctrl_package-0.0.91/README.md
+-rw-rw-rw-   0        0        0      942 2023-04-11 08:09:27.000000 python_selenium_ctrl_package-0.0.91/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 08:11:15.144309 python_selenium_ctrl_package-0.0.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.028230 python_selenium_ctrl_package-0.0.91/src/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.91/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.045231 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/
+-rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.069232 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.072232 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/app/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/app/__init__.py
+-rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/app/ports_conf.py
+-rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/product_list.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.073230 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.075230 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/Website/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
+-rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
+-rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conf/rwd/__init__.py
+-rw-rw-rw-   0        0        0    40500 2023-03-28 09:59:35.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conftest_base.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.078231 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.098230 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
+-rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
+-rw-rw-rw-   0        0        0     3327 2023-03-29 08:14:37.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
+-rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
+-rw-rw-rw-   0        0        0    16933 2022-11-21 09:45:38.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/driverfactory.py
+-rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.120309 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/
+-rw-rw-rw-   0        0        0    57649 2023-03-31 06:16:25.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/Base_Page.py
+-rw-rw-rw-   0        0        0    25197 2023-03-21 17:06:12.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/__init__.py
+-rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
+-rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/zero_page.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.123309 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/remoteTest/
+-rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/remoteTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.134308 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/email_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.141308 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/
+-rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
+-rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
+-rw-rw-rw-   0        0        0     8968 2023-04-11 08:09:09.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Wrapit.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/__init__.py
+-rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
+-rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
+-rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/html_report_conf.py
+-rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/remote_credentials.py
+-rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/screenshot_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:11:15.066232 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-04-11 08:11:14.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2378 2023-04-11 08:11:15.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:11:14.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      272 2023-04-11 08:11:14.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-11 08:11:14.000000 python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/top_level.txt
```

### Comparing `python_selenium_ctrl_package-0.0.90/LICENSE` & `python_selenium_ctrl_package-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/PKG-INFO` & `python_selenium_ctrl_package-0.0.91/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python_selenium_ctrl_package
-Version: 0.0.90
+Version: 0.0.91
 Summary: Base_page for selenium automation
-Author-email: "SimonPoon (simon_poon)" <simon.poon@qhms.com>
+Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python_selenium_ctrl_package-0.0.90/README.md` & `python_selenium_ctrl_package-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/pyproject.toml` & `python_selenium_ctrl_package-0.0.91/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_selenium_ctrl_package"
-version = "0.0.90"
+version = "0.0.91"
 authors = [
-  { name="SimonPoon (simon_poon)", email="simon.poon@qhms.com" },
+  { name="QHMS(App team)", email="qhmsqaexpert@gmail.com" },
 ]
 description = "Base_page for selenium automation"
 keywords = ['python', 'automation', 'appium', 'selenium', 'pytest', 'automation framework']
 dependencies = ['requests', 'reportportal-client', 'pytest', 'selenium', 'python_dotenv', 'Appium_Python_Client', 'pytest-xdist', 'pytest-html', 'pytest-rerunfailures', 'pytest_reportportal', 'pillow', 'tesults', 'loguru', 'imageio', 'questionary', 'clear-screen', 'prompt-toolkit', 'openpyxl', 'pytest-bdd', 'pandas', 'webdriver-manager', 'PyHamcrest']
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/conftest_base.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/conftest_base.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/drivers/driverfactory.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/drivers/driverfactory.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/main.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/main.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/Base_Page.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/Base_Page.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from ..utils import remote_credentials
 from ..conf.rwd.Website import base_url_conf
 from ..utils import screenshot_conf
 from ..utils.general import Gif_Maker
 from datetime import datetime
 from ..utils.general.Wrapit import Wrapit
 from hamcrest import assert_that, equal_to, none, not_none, contains_string
-
 from pytest_html import extras
 
 
 class Borg:
     # The borg design pattern is to share state
     # Src: http://code.activestate.com/recipes/66531/
     __shared_state = {}
@@ -269,15 +268,15 @@
             test_file = test_file.split(os.sep)[-1]
             testname = test_file.split('.py')[0]
             self.set_calling_module(testname)
 
         return self.calling_module
 
     def set_directory_structure(self):
-        "Setup the required directory structure if it is not already present"
+        "Set up the required directory structure if it is not already present"
         try:
             self.screenshots_parent_dir = os.path.abspath(
                 os.path.join(os.curdir, 'screenshots', self.product))  # Real screencap folder dir
             if not os.path.exists(self.screenshots_parent_dir):
                 os.makedirs(self.screenshots_parent_dir)
             self.logs_parent_dir = os.path.abspath(os.path.join(os.curdir, 'log',
                                                                 self.product))  # Real log file dir base on Base_Logging.py constructor
@@ -547,34 +546,35 @@
     def get_element_attribute_value(self, element, attribute_name):
         "Return the elements attribute value if present"
         attribute_value = None
         # Original code, can't get the attribute value I want
         # if (hasattr(element, attribute_name)):
         #     attribute_value = element.get_attribute(attribute_name)
         attribute_value = element.get_attribute(attribute_name)
-
         return attribute_value
 
     def check_alert(self):
         result_flag = False
         try:
-            self.driver.switch_to.alert
+            alert = self.driver.switch_to.alert
             result_flag = True
         except:
             pass
         return result_flag
 
     def switch_and_close_alert(self):
         try:
             alert = self.driver.switch_to.alert
             msg = alert.text
             alert.accept()
             self.write('Close Alert box with message: ' + msg)
+            return True
         except:
             self.write('Switch and close alert box error')
+            return False
 
     def highlight_element(self, element, wait_seconds=0):
         "Highlights a Selenium webdriver element"
         original_style = self.get_element_attribute_value(element, 'style')
         self.apply_style_to_element(element, "border: 4px solid #F6F7AD;")
         self.wait(wait_seconds)
         self.apply_style_to_element(element, original_style)
@@ -602,15 +602,14 @@
                 self.highlight_element(dom_element)
         except Exception as e:
             if verbose_flag is True:
                 self.write(str(e), 'debug')
                 self.write("Check your locator-'%s,%s' in the conf/locators.conf file" % (locator[0], locator[1]))
             self.exceptions.append(
                 "Check your locator-'%s,%s' in the conf/locators.conf file" % (locator[0], locator[1]))
-
         return dom_element
 
     def get_dropdown_element(self, locator, verbose_flag=True):
         "Return the DOM element of the path or 'None' if the element is not found "
         dom_element = None
         try:
             locator = self.split_locator(locator)
@@ -631,28 +630,28 @@
         result = ()
         try:
             result = tuple(locator.split(',', 1))
         except Exception as e:
             self.write(str(e), 'debug')
             self.write("Error while parsing locator")
             self.exceptions.append(
-                "Unable to split the locator-'%s' in the conf/locators.conf file" % (locator[0], locator[1]))
+                "Unable to split the locator-'%s,%s' in the conf/locators.conf file" % (locator[0], locator[1]))
 
         return result
 
     def get_elements(self, locator, msg_flag=True):
         "Return a list of DOM elements that match the locator"
         dom_elements = []
         try:
             locator = self.split_locator(locator)
             dom_elements = self.driver.find_elements(*locator)
             if self.highlight_flag is True:
                 self.highlight_elements(dom_elements)
         except Exception as e:
-            if msg_flag == True:
+            if msg_flag:
                 self.write(str(e), 'debug')
                 self.write("Check your locator-'%s,%s' in the conf/locators.conf file" % (locator[0], locator[1]))
             self.exceptions.append(
                 "Unable to locate the dom_element with the xpath -'%s,%s' in the conf/locators.conf file" % (
                     locator[0], locator[1]))
 
         return dom_elements
@@ -661,38 +660,36 @@
         "Return a list of DOM elements that with provided tag"
         dom_elements = []
         try:
             dom_elements = self.driver.find_elements_by_tag_name(tag)
             if self.highlight_flag is True:
                 self.highlight_elements(dom_elements)
         except Exception as e:
-            if msg_flag == True:
+            if msg_flag:
                 self.write(str(e), 'debug')
                 self.write("Check your tag -'%s' " % tag)
             self.exceptions.append(
                 "Unable to locate the dom_elements with tag %s" % (
                     tag))
-
         return dom_elements
 
     def get_elements_under_element_by_tag(self, element, tag, msg_flag=True):
         "Provide an element, return a list of DOM elements that with provided tag under that element"
         dom_elements = []
         try:
             dom_elements = element.find_elements_by_tag_name(tag)
             if self.highlight_flag is True:
                 self.highlight_elements(dom_elements)
         except Exception as e:
-            if msg_flag == True:
+            if msg_flag:
                 self.write(str(e), 'debug')
                 self.write("Check your tag -'%s' " % tag)
             self.exceptions.append(
                 "Unable to locate the dom_elements under element %s with tag %s" % (
                     element, tag))
-
         return dom_elements
 
     def click_element(self, locator, wait_time=1):
         "Click the button supplied"
         result_flag = False
         try:
             link = self.get_element(locator)
@@ -701,52 +698,68 @@
                 result_flag = True
                 self.wait(wait_time)
         except Exception as e:
             self.write(str(e), 'debug')
             self.write('Exception when clicking link with path: %s' % locator)
             self.exceptions.append(
                 "Error when clicking the dom_element with path,'%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def click_dom_element(self, dom_element, wait_time=1):
-        "Click the button supplied, the dom_element should be get by get_elements"
+        "Click the button supplied, the dom_element should be got by get_elements"
         result_flag = False
         try:
             link = dom_element
             if link is not None:
                 link.click()
                 result_flag = True
                 self.wait(wait_time)
         except Exception as e:
             self.write(str(e), 'debug')
             self.write('Exception when clicking link with path: %s' % dom_element)
             self.exceptions.append(
                 "Error when clicking the dom_element with path,'%s' in the conf/locators.conf file" % dom_element)
-
         return result_flag
 
     def double_click_element(self, locator, wait_time=1):
-        "Double click the element"
+        "Double-click the element"
         # Note: perform() of ActionChains does not return a bool
         # So we have no way of returning a bool when hover is called
-        element = self.get_element(locator)
-        action_obj = ActionChains(self.driver)
-        action_obj.double_click(element)
-        action_obj.perform()
-        self.wait(wait_time)
+        result_flag = False
+        try:
+            element = self.get_element(locator)
+            action_obj = ActionChains(self.driver)
+            action_obj.double_click(element)
+            action_obj.perform()
+            self.wait(wait_time)
+            result_flag = True
+        except Exception as e:
+            self.write(str(e), 'debug')
+            self.write('Exception when clicking link with path: %s' % locator)
+            self.exceptions.append(
+                "Error when double clicking the element with path,'%s' in the conf/locators.conf file" % locator)
+        return result_flag
 
     def double_click_dom_element(self, element, wait_time=1):
-        "Double click the element"
+        "Double-click the element"
         # Note: perform() of ActionChains does not return a bool
         # So we have no way of returning a bool when hover is called
-        action_obj = ActionChains(self.driver)
-        action_obj.double_click(element)
-        action_obj.perform()
-        self.wait(wait_time)
+        result_flag = False
+        try:
+            action_obj = ActionChains(self.driver)
+            action_obj.double_click(element)
+            action_obj.perform()
+            self.wait(wait_time)
+            result_flag = True
+        except Exception as e:
+            self.write(str(e), 'debug')
+            self.write('Exception when clicking link with path: %s' % element)
+            self.exceptions.append(
+                "Error when double clicking the dom_element with path,'%s' in the conf/locators.conf file" % element)
+        return result_flag
 
     def set_text(self, locator, value, clear_flag=True):
         "Set the value of the text field"
         text_field = None
         try:
             text_field = self.get_element(locator)
             if text_field is not None and clear_flag is True:
@@ -764,15 +777,14 @@
             try:
                 text_field.send_keys(value)
                 result_flag = True
             except Exception as e:
                 self.write('Could not write to text field: %s' % locator, 'debug')
                 self.write(str(e), 'debug')
                 self.exceptions.append("Could not write to text field- '%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def set_dom_text(self, dom_element, value, clear_flag=True):
         "Set the value of the text field"
         text_field = dom_element
         if text_field is not None and clear_flag is True:
             try:
@@ -811,73 +823,68 @@
         try:
             text = dom_element.text
         except Exception as e:
             self.write(e)
             self.exceptions.append(
                 # "Error when getting text from the DOM dom_element-'%s' in the conf/locators.conf file" % locator)
                 "Error when getting text from the DOM dom_element-'%s' in the conf/locators.conf file" % dom_element)
-
         return text
 
     def select_checkbox(self, locator):
         "Select a checkbox if not already selected"
         result_flag = False
         try:
             checkbox = self.get_element(locator)
             if checkbox.is_selected() is False:
                 result_flag = self.toggle_checkbox(locator)
             else:
                 result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when selecting checkbox-'%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def select_dom_checkbox(self, element):
         "Select a checkbox if not already selected"
         result_flag = False
         try:
             if element.is_selected() is False:
                 result_flag = self.toggle_dom_checkbox(element)
             else:
                 result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when selecting checkbox-'%s' by dom element" % element)
-
         return result_flag
 
     def deselect_checkbox(self, locator):
         "Deselect a checkbox if it is not already deselected"
         result_flag = False
         try:
             checkbox = self.get_element(locator)
             if checkbox.is_selected() is True:
                 result_flag = self.toggle_checkbox(locator)
             else:
                 result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when deselecting checkbox-'%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def deselect_dom_checkbox(self, element):
         "Deselect a checkbox if not already selected"
         result_flag = False
         try:
             if element.is_selected() is True:
                 result_flag = self.toggle_dom_checkbox(element)
             else:
                 result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when deselecting checkbox-'%s' by dom element" % element)
-
         return result_flag
 
     unselect_checkbox = deselect_checkbox  # alias the method
     unselect_dom_checkbox = deselect_dom_checkbox  # alias the method
 
     def toggle_checkbox(self, locator):
         "Toggle a checkbox"
@@ -930,15 +937,14 @@
                 if option.text == option_text:
                     option.click()
                     result_flag = True
                     break
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when selecting option from the drop-down '%s' " % locator)
-
         return result_flag
 
     def select_dropdown_option_by_textContent(self, locator, option_text):
         "Selects the option in the drop-down by text"
         result_flag = False
         try:
             dropdown = self.get_element(locator)
@@ -948,15 +954,14 @@
                 if option.text == option_text:
                     option.click()
                     result_flag = True
                     break
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when selecting option from the drop-down '%s' " % locator)
-
         return result_flag
 
     def select_dropdown_option_by_value(self, locator, value):
         "Selects the option in the drop-down by value"
         result_flag = False
         try:
             dropdown = self.get_element(locator)
@@ -964,102 +969,94 @@
                 if self.get_element_attribute_value(option, 'value') == value:
                     option.click()
                     result_flag = True
                     break
         except Exception as e:
             self.write(e)
             self.exceptions.append("Error when selecting option from the drop-down '%s' " % locator)
-
         return result_flag
 
     def select_dropdownelement_option_by_text(self, element, option_text):
         """element should be a Selenium Select object"""
         result_flag = True
         try:
             element.select_by_visible_text(option_text)
         except Exception as e:
             result_flag = False
             self.write(e)
             self.exceptions.append("Unable to find %s in dom dropdown %s by visible text" % (option_text, element))
-
         return result_flag
 
     def elementIsDisplayed(self, element):
         """element should be a Selenium Select object"""
         result_flag = True
         try:
             element.is_displayed()
         except Exception as e:
             result_flag = False
             self.write(e)
             self.exceptions.append("Element is not displayed" % (element))
-
         return result_flag
 
     def select_dropdownelement_option_by_value(self, element, option_value):
         """element should be a Selenium Select object"""
         result_flag = True
         try:
             element.select_by_value(option_value)
         except Exception as e:
             result_flag = False
             self.write(e)
             self.exceptions.append("Unable to find %s in dom dropdown %s by value" % (option_value, element))
-
         return result_flag
 
     def check_element_present(self, locator):
         "This method checks if the web element is present in page or not and returns True or False accordingly"
         result_flag = False
         if self.get_element(locator, verbose_flag=False) is not None:
             result_flag = True
-
         return result_flag
 
     def check_element_displayed(self, locator):
         "This method checks if the web dom_element is present in page or not and returns True or False accordingly"
         result_flag = False
         try:
             if self.get_element(locator) is not None:
                 element = self.get_element(locator, verbose_flag=False)
                 if element.is_displayed() is True:
                     result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append(
                 "Web element not present in the page, please check the locator is correct -'%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def check_element_enabled(self, locator):
         "This method checks if the web dom_element is enabled in page or not and returns True or False accordingly"
         result_flag = False
         try:
             if self.get_element(locator) is not None:
                 element = self.get_element(locator, verbose_flag=False)
                 if element.is_enabled() is True:
                     result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append(
                 "Web element not present in the page, please check the locator is correct -'%s' in the conf/locators.conf file" % locator)
-
         return result_flag
 
     def check_dom_enabled(self, element):
         "This method checks if the web dom_element is enabled in page or not and returns True or False accordingly"
         result_flag = False
         try:
             if element.is_enabled() is True:
                 result_flag = True
         except Exception as e:
             self.write(e)
             self.exceptions.append(
                 "Web element not present in the page, please check the element is correct %s" % element)
-
         return result_flag
 
     def hit_enter(self, locator, wait_time=0.5):
         "Hit enter"
         try:
             element = self.get_element(locator)
             element.send_keys(Keys.ENTER)
@@ -1071,51 +1068,55 @@
 
     def hit_down(self, locator, wait_time=0.5):
         "Hit enter"
         try:
             element = self.get_element(locator)
             element.send_keys(Keys.ARROW_DOWN)
             self.wait(wait_time)
+            return True
         except Exception as e:
             self.write(str(e), 'debug')
             self.exceptions.append("An exception occurred when hitting enter")
-            return None
+            return False
 
     def scroll_down(self, locator, wait_time=0.5):
         "Scroll down"
         try:
             element = self.get_element(locator)
             element.send_keys(Keys.PAGE_DOWN)
             self.wait(wait_time)
+            return True
         except Exception as e:
             self.write(str(e), 'debug')
-            self.exceptions.append("An exception occured when scrolling down")
-            return None
+            self.exceptions.append("An exception occurred when scrolling down")
+            return False
 
     def scroll_up(self, locator, wait_time=0.5):
         "Scroll down"
         try:
             element = self.get_element(locator)
             element.send_keys(Keys.PAGE_UP)
             self.wait(wait_time)
+            return True
         except Exception as e:
             self.write(str(e), 'debug')
-            self.exceptions.append("An exception occured when scrolling up")
-            return None
+            self.exceptions.append("An exception occurred when scrolling up")
+            return False
 
     def key_press_END(self, locator, wait_time=0.5):
         "Scroll down"
         try:
             element = self.get_element(locator)
             element.send_keys(Keys.END)
             self.wait(wait_time)
+            return True
         except Exception as e:
             self.write(str(e), 'debug')
-            self.exceptions.append("An exception occured when scrolling down")
-            return None
+            self.exceptions.append("An exception occurred when scrolling down")
+            return False
 
     def hover(self, locator, wait_seconds=0.5):
         "Hover over the element"
         # Note: perform() of ActionChains does not return a bool
         # So we have no way of returning a bool when hover is called
         element = self.get_element(locator)
         action_obj = ActionChains(self.driver)
@@ -1185,22 +1186,22 @@
         # self.gif_file_name = Gif_Maker.make_gif(self.screenshot_dir, name=self.calling_module)
         #
         # return self.gif_file_name
         if self.screenshot != 'off':
             self.gif_file_name = Gif_Maker.make_gif(self.screenshot_dir, name=self.calling_module)
             return self.gif_file_name
 
-    def wait(self, wait_seconds=5, locator=None):
+    def wait(self, wait_seconds=5.0, locator=None):
         "Performs wait for time provided"
         if locator is not None:
             self.smart_wait(locator, wait_seconds=wait_seconds)
         else:
             time.sleep(wait_seconds)
 
-    def smart_wait(self, locator, wait_seconds=5, verbose_flag=True):
+    def smart_wait(self, locator, wait_seconds=5.0, verbose_flag=True):
         "Performs an explicit wait for a particular dom_element. Return True if wait success"
         result_flag = False
         try:
             path = self.split_locator(locator)
             WebDriverWait(self.driver, wait_seconds).until(EC.presence_of_element_located(path))
             result_flag = True
         except Exception:
@@ -1266,15 +1267,15 @@
             if flag is True:
                 self.write(positive, level='info')
                 self.mini_check_pass_counter += 1
             else:
                 self.write(negative, level='error')
 
     def execute_javascript(self, js_script, *args):
-        "Execute javascipt"
+        "Execute javascript"
         try:
             self.driver.execute_script(js_script)
             result_flag = True
         except Exception as e:
             result_flag = False
 
         return result_flag
@@ -1285,15 +1286,15 @@
         try:
             result = self.driver.execute_script("return " + js_script)
         except Exception as e:
             raise ("Error when execute javascript: %s" % js_script)
         return result
 
     def write_test_summary(self):
-        "Print out a useful, human readable summary"
+        "Print out a useful, human-readable summary"
         self.write(
             '\n\n************************\n--------RESULT--------\nTotal number of checks=%d' % self.result_counter)
         self.write(
             'Total number of checks passed=%d\n----------------------\n************************\n\n' % self.pass_counter)
         self.write('Total number of mini-checks=%d' % self.mini_check_counter)
         self.write('Total number of mini-checks passed=%d' % self.mini_check_pass_counter)
         failure_message_list = self.get_failure_message_list()
@@ -1317,20 +1318,20 @@
 
     def start(self):
         "Overwrite this method in your Page module if you want to visit a specific URL"
         pass
 
     @Wrapit._screenshot
     def take_screenshot(self):
-        """Use this function to take screenshot, the screen shot will take only when screenshot option = all"""
+        """Use this function to take screenshot, the screenshot will take only when screenshot option = all"""
         return True
 
     @Wrapit._screenshot
     def take_force_screenshot(self):
-        """Use this function to take screenshot, the screen shot will take even use screenshot option = failonly"""
+        """Use this function to take screenshot, the screenshot will take even use screenshot option = failonly"""
         return False
 
     @Wrapit._check_browser_console_log
     def get_console_log(self):
         """After run this function, Base_page.current_console_log_errors should store the console log"""
         pass
 
@@ -1342,11 +1343,11 @@
 
     def scroll_by_amount(self, locator, delta_x: int, delta_y: int):
         try:
             element = self.get_element(locator)
             element.scroll_by_amount(delta_x, delta_y)
         except Exception as e:
             self.write(str(e), 'debug')
-            self.exceptions.append("An exception occured when scroll by amount")
+            self.exceptions.append("An exception occurred when scroll by amount")
             return None
 
     # _get_locator = staticmethod(_get_locator) "COMMENT BECAUSE _get_locator commented"
```

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/email_conf.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/email_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Base_Logging.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Base_Logging.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/Wrapit.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/Wrapit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Class to hold miscellaneous but useful decorators for our framework
 """
-
+import os
 from inspect import getfullargspec
 import traceback
-
 import pytest_html
 
 
 class Wrapit():
     "Wrapit class to hold decorator functions"
 
     def _exceptionHandler(f):
@@ -39,46 +38,49 @@
             # args[0].screenshot_counter += 1
             # args[0].save_screenshot(screenshot_name)
             #
             # return result
 
             # Run function with _screenshot decorator, get the return result (Expect boolean)
             result = func(*args, **kwargs)
+
             # If return True, only take screenshot if option -screenshot all
             # If return False, take screenshot for both -screenshot all/failonly
             # If not return boolean, skip screenshot
-            if args[0].screenshot == 'all':
-                screenshot_name = '%003d' % args[0].screenshot_counter + '_' + func.__name__
-                args[0].screenshot_counter += 1
-                args[0].save_screenshot(screenshot_name)
-            elif args[0].screenshot == 'failonly' and result is False:
-                screenshot_name = '%003d' % args[0].screenshot_counter + '_' + func.__name__
-                args[0].screenshot_counter += 1
-                args[0].save_screenshot(screenshot_name)
+            if not args[0].check_alert():              # Skip screenshot when there is an alert, otherwise will throw UnexpectedAlertPresentException
+                if args[0].screenshot == 'all':
+                    screenshot_name = '%003d' % args[0].screenshot_counter + '_' + func.__name__
+                    args[0].screenshot_counter += 1
+                    args[0].save_screenshot(screenshot_name)
+                elif args[0].screenshot == 'failonly' and result is False:
+                    screenshot_name = '%003d' % args[0].screenshot_counter + '_' + func.__name__
+                    args[0].screenshot_counter += 1
+                    args[0].save_screenshot(screenshot_name)
             return result
 
         return wrapper
 
     def _logging_decorator(func):
 
         def wrapper(test_obj, product, cases, extra, testID, *args, **kwargs):
             try:
                 result = func(test_obj, product, cases, extra, testID, *args, **kwargs)
                 test_obj.gif_file_name = test_obj.write_test_summary()
             except Exception as e:
                 print("Exception when trying to run test: %s" % __file__)
                 print("Python says:%s" % str(e))
                 test_obj.write(traceback.format_exc())
-                if test_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
-                    screenshot_name = '%003d' % test_obj.screenshot_counter + '_' + func.__name__
-                    test_obj.screenshot_counter += 1
-                    test_obj.save_screenshot(screenshot_name)
+                if not test_obj.check_alert():              # Skip screenshot when there is an alert, otherwise will throw UnexpectedAlertPresentException
+                    if test_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
+                        screenshot_name = '%003d' % test_obj.screenshot_counter + '_' + func.__name__
+                        test_obj.screenshot_counter += 1
+                        test_obj.save_screenshot(screenshot_name)
 
                 # Detail print in last line
-                with open(test_obj.logs_parent_dir + "\\" + test_obj.log_name, "a") as logfile:
+                with open(os.path.join(test_obj.logs_parent_dir, test_obj.log_name), "a") as logfile:
                     traceback.print_exc(file=logfile)
                 globals()['gif_file'] = test_obj.write_test_summary()
                 raise
             return result
 
         return wrapper
 
@@ -88,21 +90,22 @@
             try:
                 result = func(test_obj, product, poc_cases, extra, testID, *args, **kwargs)
                 test_obj.gif_file_name = test_obj.write_test_summary()
             except Exception as e:
                 print("Exception when trying to run test: %s" % __file__)
                 print("Python says:%s" % str(e))
                 test_obj.write(traceback.format_exc())
-                if test_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
-                    screenshot_name = '%003d' % test_obj.screenshot_counter + '_' + func.__name__
-                    test_obj.screenshot_counter += 1
-                    test_obj.save_screenshot(screenshot_name)
+                if not test_obj.check_alert():  # Skip screenshot when there is an alert, otherwise will throw UnexpectedAlertPresentException
+                    if test_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
+                        screenshot_name = '%003d' % test_obj.screenshot_counter + '_' + func.__name__
+                        test_obj.screenshot_counter += 1
+                        test_obj.save_screenshot(screenshot_name)
 
                 # Detail print in last line
-                with open(test_obj.logs_parent_dir + "\\" + test_obj.log_name, "a") as logfile:
+                with open(os.path.join(test_obj.logs_parent_dir, test_obj.log_name), "a") as logfile:
                     traceback.print_exc(file=logfile)
                 globals()['gif_file'] = test_obj.write_test_summary()
                 raise
             return result
 
         return wrapper
 
@@ -112,21 +115,22 @@
             try:
                 result = func(test_mobile_obj, product, cases, extra, testID, *args, **kwargs)
                 test_mobile_obj.gif_file_name = test_mobile_obj.write_test_summary()
             except Exception as e:
                 print("Exception when trying to run test: %s" % __file__)
                 print("Python says:%s" % str(e))
                 test_mobile_obj.write(traceback.format_exc())
-                if test_mobile_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
-                    screenshot_name = '%003d' % test_mobile_obj.screenshot_counter + '_' + func.__name__
-                    test_mobile_obj.screenshot_counter += 1
-                    test_mobile_obj.save_screenshot(screenshot_name)
+                if not test_mobile_obj.check_alert():  # Skip screenshot when there is an alert, otherwise will throw UnexpectedAlertPresentException
+                    if test_mobile_obj.screenshot != 'off':        # Add for handling fail screenshot *Break case (Take screenshot for non off case)
+                        screenshot_name = '%003d' % test_mobile_obj.screenshot_counter + '_' + func.__name__
+                        test_mobile_obj.screenshot_counter += 1
+                        test_mobile_obj.save_screenshot(screenshot_name)
 
                 # Detail print in last line
-                with open(test_mobile_obj.logs_parent_dir + "\\" + test_mobile_obj.log_name, "a") as logfile:
+                with open(os.path.join(test_mobile_obj.logs_parent_dir, test_mobile_obj.log_name), "a") as logfile:
                     traceback.print_exc(file=logfile)
                 globals()['gif_file'] = test_mobile_obj.write_test_summary()
                 raise
             return result
 
         return wrapper
```

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/PKG-INFO` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-selenium-ctrl-package
-Version: 0.0.90
+Version: 0.0.91
 Summary: Base_page for selenium automation
-Author-email: "SimonPoon (simon_poon)" <simon.poon@qhms.com>
+Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python_selenium_ctrl_package-0.0.90/src/python_selenium_ctrl_package.egg-info/SOURCES.txt` & `python_selenium_ctrl_package-0.0.91/src/python_selenium_ctrl_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

