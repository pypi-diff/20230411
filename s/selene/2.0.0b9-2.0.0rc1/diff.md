# Comparing `tmp/selene-2.0.0b9.tar.gz` & `tmp/selene-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selene-2.0.0b9.tar", max compression
+gzip compressed data, was "selene-2.0.0rc1.tar", max compression
```

## Comparing `selene-2.0.0b9.tar` & `selene-2.0.0rc1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0     1077 2022-09-14 16:43:44.443996 selene-2.0.0b9/LICENSE
--rw-r--r--   0        0        0    12705 2022-09-14 16:43:44.443996 selene-2.0.0b9/README.md
--rw-r--r--   0        0        0     6860 2022-09-14 16:43:50.624171 selene-2.0.0b9/pyproject.toml
--rw-r--r--   0        0        0     5934 2022-09-14 16:43:50.672173 selene-2.0.0b9/selene/__init__.py
--rw-r--r--   0        0        0     1785 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/api/__init__.py
--rw-r--r--   0        0        0     1359 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/api/base/__init__.py
--rw-r--r--   0        0        0     1212 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/api/shared/__init__.py
--rw-r--r--   0        0        0        0 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/common/__init__.py
--rw-r--r--   0        0        0     2834 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/common/fp.py
--rw-r--r--   0        0        0     3022 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/common/helpers.py
--rw-r--r--   0        0        0     1464 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/common/none_object.py
--rw-r--r--   0        0        0     3497 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/common/predicate.py
--rw-r--r--   0        0        0     1116 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/__init__.py
--rw-r--r--   0        0        0     5556 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/command.py
--rw-r--r--   0        0        0     5583 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/condition.py
--rw-r--r--   0        0        0     1391 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/conditions.py
--rw-r--r--   0        0        0     8199 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/configuration.py
--rw-r--r--   0        0        0    42615 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/entity.py
--rw-r--r--   0        0        0     2397 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/exceptions.py
--rw-r--r--   0        0        0     1464 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/locator.py
--rw-r--r--   0        0        0    15853 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/match.py
--rw-r--r--   0        0        0     5170 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/query.py
--rw-r--r--   0        0        0     5501 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/core/wait.py
--rw-r--r--   0        0        0      107 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/__init__.py
--rw-r--r--   0        0        0     2310 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/_logging.py
--rw-r--r--   0        0        0     2867 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/by.py
--rw-r--r--   0        0        0        0 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/conditions/__init__.py
--rw-r--r--   0        0        0     1739 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/conditions/be.py
--rw-r--r--   0        0        0     5810 2022-09-14 16:43:44.447996 selene-2.0.0b9/selene/support/conditions/have.py
--rw-r--r--   0        0        0     8661 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/conditions/not_.py
--rw-r--r--   0        0        0     1823 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/jquery_style_selectors.py
--rw-r--r--   0        0        0     1321 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/shared/__init__.py
--rw-r--r--   0        0        0     8290 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/shared/browser.py
--rw-r--r--   0        0        0    21358 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/shared/config.py
--rw-r--r--   0        0        0     1447 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/shared/jquery_style.py
--rw-r--r--   0        0        0     2657 2022-09-14 16:43:44.451996 selene-2.0.0b9/selene/support/webdriver.py
--rw-r--r--   0        0        0    14295 1970-01-01 00:00:00.000000 selene-2.0.0b9/setup.py
--rw-r--r--   0        0        0    14150 1970-01-01 00:00:00.000000 selene-2.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0    16589 2023-04-10 12:28:03.426931 selene-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     7951 2023-04-10 11:04:48.138046 selene-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-04-01 13:26:39.498825 selene-2.0.0rc1/selene/__init__.py
+-rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc1/selene/_managed.py
+-rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc1/selene/api/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc1/selene/api/base/__init__.py
+-rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc1/selene/api/shared/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc1/selene/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc1/selene/common/data_structures/__init__.py
+-rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc1/selene/common/data_structures/persistent.py
+-rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc1/selene/common/fp.py
+-rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc1/selene/common/helpers.py
+-rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc1/selene/common/none_object.py
+-rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc1/selene/common/predicate.py
+-rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc1/selene/core/__init__.py
+-rw-r--r--   0        0        0     7107 2023-04-10 11:06:23.401462 selene-2.0.0rc1/selene/core/command.py
+-rw-r--r--   0        0        0     6608 2023-04-10 11:06:23.381272 selene-2.0.0rc1/selene/core/condition.py
+-rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc1/selene/core/conditions.py
+-rw-r--r--   0        0        0    50433 2023-04-11 00:26:18.593662 selene-2.0.0rc1/selene/core/configuration.py
+-rw-r--r--   0        0        0     9224 2023-04-11 01:37:57.353410 selene-2.0.0rc1/selene/core/configuration.pyi
+-rw-r--r--   0        0        0    44329 2023-04-11 01:51:05.070968 selene-2.0.0rc1/selene/core/entity.py
+-rw-r--r--   0        0        0    11983 2023-04-11 01:51:05.074766 selene-2.0.0rc1/selene/core/entity.pyi
+-rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc1/selene/core/exceptions.py
+-rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc1/selene/core/locator.py
+-rw-r--r--   0        0        0    17245 2023-04-10 11:06:23.584719 selene-2.0.0rc1/selene/core/match.py
+-rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc1/selene/core/query.py
+-rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc1/selene/core/wait.py
+-rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc1/selene/py.typed
+-rw-r--r--   0        0        0      107 2023-04-01 17:58:51.579568 selene-2.0.0rc1/selene/support/__init__.py
+-rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc1/selene/support/_logging.py
+-rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc1/selene/support/by.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc1/selene/support/conditions/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc1/selene/support/conditions/be.py
+-rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc1/selene/support/conditions/have.py
+-rw-r--r--   0        0        0     8989 2023-04-10 11:06:23.509416 selene-2.0.0rc1/selene/support/conditions/not_.py
+-rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc1/selene/support/shared/__init__.py
+-rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc1/selene/support/shared/browser.py
+-rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc1/selene/support/shared/config.py
+-rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc1/selene/support/shared/jquery_style.py
+-rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc1/selene/support/webdriver.py
+-rw-r--r--   0        0        0    18274 1970-01-01 00:00:00.000000 selene-2.0.0rc1/PKG-INFO
```

### Comparing `selene-2.0.0b9/LICENSE` & `selene-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/README.md` & `selene-2.0.0rc1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,433 +1,603 @@
+Metadata-Version: 2.1
+Name: selene
+Version: 2.0.0rc1
+Summary: User-oriented browser tests in Python (Selenide port)
+Home-page: https://yashaka.github.io/selene/
+License: MIT
+Keywords: testing,selenium,selenide,browser,pageobject,widget,wrapper
+Author: Iakiv Kramarenko
+Author-email: yashaka@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: future
+Requires-Dist: selenium (>=4.4.3)
+Requires-Dist: typing-extensions (==4.3.0)
+Requires-Dist: webdriver-manager (>=3.8.5)
+Project-URL: Changelog, https://github.com/yashaka/selene/releases
+Project-URL: Documentation, https://yashaka.github.io/selene/
+Project-URL: Repository, http://github.com/yashaka/selene/
+Description-Content-Type: text/markdown
+
+<!-- --8<-- [start:githubSection] -->
 # Selene - User-oriented Web UI browser tests in Python (Selenide port)
 
+![Pre-release Version](https://img.shields.io/github/v/release/yashaka/selene?label=latest)
 [![tests](https://github.com/yashaka/selene/actions/workflows/tests.yml/badge.svg)](https://github.com/yashaka/selene/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/yashaka/selene/branch/master/graph/badge.svg)](https://codecov.io/gh/yashaka/selene)
 ![Free](https://img.shields.io/badge/free-open--source-green.svg)
-[![MIT License](http://img.shields.io/badge/license-MIT-green.svg)](https://github.com/yashaka/selene/blob/master/LICENSE)
-[![Project Template](http://img.shields.io/badge/project-template-9cf.svg)](https://github.com/yashaka/python-web-test)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Downloads](https://pepy.tech/badge/selene)](https://pepy.tech/project/selene)
+[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/yashaka/selene/blob/master/LICENSE)
 
-![GitHub stats in](https://raw.githubusercontent.com/yashaka/selene/traffic/traffic-selene/in_2021.svg)
-![GitHub views](https://raw.githubusercontent.com/yashaka/selene/traffic/traffic-selene/views.svg)
-![GitHub views per week](https://raw.githubusercontent.com/yashaka/selene/traffic/traffic-selene/views_per_week.svg)
-![GitHub clones](https://raw.githubusercontent.com/yashaka/selene/traffic/traffic-selene/clones.svg)
-![GitHub clones per week](https://raw.githubusercontent.com/yashaka/selene/traffic/traffic-selene/clones_per_week.svg)
+[![Downloads](https://pepy.tech/badge/selene)](https://pepy.tech/project/selene)
+[![Project Template](https://img.shields.io/badge/project-template-9cf.svg)](https://github.com/yashaka/python-web-test)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Join telegram chat https://t.me/selene_py](https://img.shields.io/badge/chat-telegram-blue)](https://t.me/selene_py)
 [![Присоединяйся к чату https://t.me/selene_py_ru](https://img.shields.io/badge/%D1%87%D0%B0%D1%82-telegram-red)](https://t.me/selene_py_ru)
 
-[![Sign up for a course http://autotest.how/selene](https://img.shields.io/badge/course-sign_up-blue)](http://autotest.how/selene)
-[![Запишись на курс http://autotest.how/selene-ru](https://img.shields.io/badge/%D0%BD%D0%B0%D0%B1%D0%BE%D1%80-%D0%BD%D0%B0%20%D0%BA%D1%83%D1%80%D1%81-red)](http://autotest.how/selene-ru)
-[![Учи Selene https://leanpub.com/selene-automation-ru](https://img.shields.io/badge/%D0%BA%D0%BD%D0%B8%D0%B3%D0%B0-leanpub-red)](https://leanpub.com/selene-automation-ru)
-[![Реєструйся на курс http://autotest.how/selene-uk](https://img.shields.io/badge/%D0%BD%D0%B0%D0%B1%D1%96%D1%80-%D0%BD%D0%B0_%D0%BA%D1%83%D1%80%D1%81-yellow)](http://autotest.how/selene-uk)
-
+[![Sign up for a course https://autotest.how/sdet-start](https://img.shields.io/badge/course-sign_up-blue)](https://autotest.how/sdet-start)
+[![Запишись на курс https://autotest.how/sdet-start-ru](https://img.shields.io/badge/%D0%BD%D0%B0%D0%B1%D0%BE%D1%80-%D0%BD%D0%B0%20%D0%BA%D1%83%D1%80%D1%81-red)](https://autotest.how/sdet-start-ru)
+[![Реєструйся на курс https://autotest.how/sdet-start-uk](https://img.shields.io/badge/%D0%BD%D0%B0%D0%B1%D1%96%D1%80-%D0%BD%D0%B0_%D0%BA%D1%83%D1%80%D1%81-yellow)](https://autotest.how/sdet-start-uk)
 
 Main features:
 
 - **User-oriented API for Selenium Webdriver** (code like speak common English)
 - **Ajax support** (Smart implicit waiting and retry mechanism)
 - **PageObjects support** (all elements are lazy-evaluated objects)
 - **Automatic driver management** (no need to install and setup driver for quick local execution)
 
+Selene was inspired by [Selenide][selenide] from Java world.
 
-Selene was inspired by [Selenide](http://selenide.org/) from Java world.
+Tests with Selene can be built either in a simple straightforward "selenide" style or with PageObjects composed from Widgets i.e. reusable element components.
 
-Tests with Selene can be built either in a simple straightforward "selenide' style or with PageObjects composed from Widgets i.e. reusable element components.
+- [Versions](#versions)
+    - [Migration Guide](#migration-guide)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+    - [Quick Start](#quick-start)
+    - [Core API](#core-api)
+    - [Automatic Driver and Browser Management](#automatic-driver-and-browser-management)
+    - [Advanced API](#advanced-api)
+- [Tutorials](#tutorials)
+- [Examples](#more-examples)
+- [Contribution](#contribution)
+- [Release Workflow](#release-workflow)
+- [Changelog](#changelog)
 
-## Table of content
+## Versions
 
-* [Versions](#versions)
-    * [Migration Guide](#migration-guide)
-* [Prerequisites](#prerequisites)
-* [Installation](#installation)
-* [Usage](#usage)
-    * [Quick Start](#quick-start)
-    * [Core API](#core-api)
-    * [Automatic Driver and Browser Management](#automatic-driver-and-browser-management)
-    * [Advanced API](#advanced-api)
-* [Tutorials](#tutorials)
-* [Examples](#more-examples)
-* [Contributing](#contributing)
-* [Release Process](#release-process)
-* [Changelog](#changelog)
+- Latest recommended version to use is [2.0.0b17+][latest-recommended-version]
+    - it's a completely new version of selene, with improved API and speed
+    - supports Python `3.7+`
+    - bundled with Selenium `4.1+`
+    - it's incompatible with [1.x][brunch-ver-1]
+    - current master branch is pointed to 2.x
+    - yet in alpha/beta stage, refining API, improving "migratability" and testing
+    - most active Selene users already upgraded to 2.0 alpha/beta 
+      and have been using it in production during last 2 years
+    - the only risk is API changes, 
+      some commands are in progress of deprecation and renaming
+- Latest version marked as stable is: [1.0.2][selene-stable]
+    - its sources and corresponding README version
+    can be found at [1.x][brunch-ver-1] branch.
+    - supports python `2.7, 3.5, 3.6, 3.7`
+
+THIS README DESCRIBES THE USAGE OF THE PRE-RELEASE version of Selene. For older docs look at [1.x][brunch-ver-1] branch.
 
-## Versions
-  
-* Latest recommended version to use is >= [2.0.0b6](https://pypi.org/project/selene/2.0.0b6/)
-  * it's a completely new version of selene, with improved API and speed
-  * supports 3.7 <= python <= 3.10,
-  * bundled with Selenium = 4.1
-  * it's incompatible with [1.x](https://github.com/yashaka/selene/tree/1.x)
-  * current master branch is pointed to 2.x
-  * yet in alpha/beta stage, refining API, improving "migratability", and testing
-  * it looks pretty stable, most users already upgraded to 2.0 alpha/beta
-
-* Latest version marked as stable is: [1.0.2](https://pypi.org/project/selene/1.0.2/)
-  * it is main version used by most selene users during last 2 years
-  * it was proven to be stable for production use
-  * its sources and corresponding README version can be found at [1.x](https://github.com/yashaka/selene/tree/1.x) branch.
-  * supports python 2.7, 3.5, 3.6, 3.7
-  
-THIS README DESCRIBES THE USAGE OF THE PRE-RELEASE version of Selene. For older docs look at [1.x](https://github.com/yashaka/selene/tree/1.x) branch.
-  
 ### Migration guide
 
-From 1.0.1 to 2.0.0aLATEST:
-* upgrade to python 3.7
-* update selene to 2.0.0aLATEST
-  * find&replace the `collection.first()` method from `.first()` to `.first`
-  * ensure all conditions like `text('foo')` are used via `be.*` or `have.*` syntax
-    * example:
-      * find&replace all
-        * `(text('foo'))` to `(have.text('foo'))`
-        * `(visible)` to `(be.visible)`
-      * smarter find&replace (with some manual refactoring)
-        * `.should(x, timeout=y)` to `.with_(timeout=y).should(x)`
-      * and add corresponding imports: `from selene import be, have`
-  * fix another broken imports if available
-  * run tests, read deprecation warnings, and refactor to new style recommended in warning messages
+From `1.0.2` to `2.0.0b<LATEST>`:
+
+- upgrade to Python 3.7+
+- update selene to `2.0.0b<LATEST>`
+    - find&replace the `collection.first()` method from `.first()` to `.first`
+    - ensure all conditions like `text('foo')` are used via `be.*` or `have.*` syntax
+        - example:
+            - find&replace all
+                - `(text('foo'))` to `(have.text('foo'))`
+                - `(visible)` to `(be.visible)`
+            - smarter find&replace (with some manual refactoring)
+                - `.should(x, timeout=y)` to `.with_(timeout=y).should(x)`
+                - `.should_not(be.*)` to `.should(be.not_.*)` or `.should(be.*.not_)`
+                - `.should_not(have.*)` to `.should(have.no.*)` or `.should(have.*.not_)`
+                - `.should_each(condition)` to `.should(condition.each)`
+            - and add corresponding imports:
+            `from selene import be, have`
+    - fix another broken imports if available
+    - run tests, read deprecation warnings, and refactor to new style recommended in warning messages
 
 ## Prerequisites
 
-[Python >= 3.7](https://www.python.org/downloads/release/python-370/)
+[Python 3.7+][python-37]
 
-Given [pyenv](https://github.com/pyenv/pyenv) installed, installing needed version of Python is pretty simple:
+Given [pyenv][pyenv] installed, installing needed version of Python is pretty simple:
 
-    $ pyenv install 3.7.3
-    $ pyenv global 3.7.3
-    $ python -V
-    Python 3.7.3
+```plain
+$ pyenv install 3.7.3
+$ pyenv global 3.7.3
+$ python -V
+Python 3.7.3
+```
 
 ## Installation
 
 ### via poetry + pyenv (recommended)
 
-GIVEN [poetry](https://poetry.eustace.io/) and [pyenv](https://github.com/pyenv/pyenv) installed ...
+GIVEN [poetry][poetry] and [pyenv][pyenv] installed ...
 
 AND
 
-    $ poetry new my-tests-with-selene
-    $ cd my-tests-with-selene
-    $ pyenv local 3.7.3
+```plain
+poetry new my-tests-with-selene
+cd my-tests-with-selene
+pyenv local 3.7.3
+```
 
 WHEN latest pre-release recommended version:
 
-    $ poetry add selene --allow-prereleases
+```plain
+poetry add selene --allow-prereleases
+```
 
 WHEN latest stable version:
 
-    $ poetry add selene
+```plain
+poetry add selene
+```
 
 THEN
 
-    $ poetry install
+```plain
+poetry install
+```
 
 ### via pip
 
 Latest recommended pre-release alpha version:
 
-    $ pip install selene --pre
+```plain
+pip install selene --pre
+```
 
 Latest stable version:
 
-    $ pip install selene
+```plain
+pip install selene
+```
 
 ### from sources
 
 GIVEN webdriver and webdriver_manager are already installed
 
 THEN
 
-    $ git clone https://github.com/yashaka/selene.git
-    $ python setup.py install
+```plain
+git clone https://github.com/yashaka/selene.git
+python setup.py install
+```
 
 or using pip:
 
-    $ pip install git+https://github.com/yashaka/selene.git
-    
+```plain
+pip install git+https://github.com/yashaka/selene.git
+```
 
 ## Usage
 
 ### Quick Start
 
 Simply...
 
 ```python
-from selene.support.shared import browser
-from selene import by, be, have
+from selene import browser, by, be, have
 
 browser.open('https://google.com/ncr')
 browser.element(by.name('q')).should(be.blank)\
     .type('selenium').press_enter()
-browser.all('.srg .g').should(have.size(10))\
+browser.all('#rso>div').should(have.size_greater_than(5))\
     .first.should(have.text('Selenium automates browsers'))
 ```
 
 OR with custom setup
 
 ```python
-from selene.support.shared import browser
-from selene import by, be, have
+from selene import browser, by, be, have
 
-browser.config.browser_name = 'firefox'
+browser.config.driver_name = 'firefox'
 browser.config.base_url = 'https://google.com'
 browser.config.timeout = 2
 # browser.config.* = ...
 
 browser.open('/ncr')
-browser.element(by.name('q')).should(be.blank)\
+browser.element(by.name('q')).should(be.blank) \
     .type('selenium').press_enter()
-browser.all('.srg .g').should(have.size(10))\
+browser.all('#rso>div').should(have.size_greater_than(5)) \
     .first.should(have.text('Selenium automates browsers'))
 ```
 
 OR more Selenide from java style:
 
 ```python
-from selene.support.shared import config, browser
-from selene import by, be, have
+from selene import browser, by, be, have
+from selene.support.shared import config
 from selene.support.shared.jquery_style import s, ss
 
 
 config.browser_name = 'firefox'
 config.base_url = 'https://google.com'
 config.timeout = 2
 # config.* = ...
 
 browser.open('/ncr')
-s(by.name('q')).should(be.blank)\
+s(by.name('q')).should(be.blank) \
     .type('selenium').press_enter()
-ss('.srg .g').should(have.size(10))\
+ss('#rso>div').should(have.size_greater_than(5)) \
     .first.should(have.text('Selenium automates browsers'))
 ```
 
 ### Core Api
 
-Given:
 
 ```python
+
+# Given:
 from selenium.webdriver import Chrome
-```
 
-AND chromedriver executable available in $PATH
+# AND chromedriver executable available in $PATH
 
-WHEN:
-```python
+# WHEN:
 from selene import Browser, Config
 
-browser = Browser(Config(
-    driver=Chrome(),
-    base_url='https://google.com',
-    timeout=2))
-```
-
-AND (uncomment if needed):
+browser = Browser(
+    Config(
+        driver=Chrome(),
+        base_url='https://google.com',
+        timeout=2,
+    )
+)
 
-```python
-# import atexit
-# atexit.register(browser.quit)
-```
-
-AND:
-
-```python
+# AND:
 browser.open('/ncr')
-```
-
-AND:
 
-```python
+# AND:
 # browser.element('//*[@name="q"]')).type('selenium').press_enter()
 # OR...
-
 # browser.element('[name=q]')).type('selenium').press_enter()
 # OR...
-
 from selene import by
-
 # browser.element(by.name('q')).type('selenium').press_enter()
 # OR...for total readability
-
-query = browser.element(by.name('q'))  # actual search doesn't start here, the element is "lazy"          
-     # here the actual webelement is found
+query = browser.element(by.name('q'))
+# actual search doesn't start on calling browser.element above, 
+# i.e. the element is "lazy"... or in other words it serves as locator         
+# Below, on calling actual first action, 
+#     ⬇ the actual webelement is located first time
 query.type('selenium').press_enter()       
-                      # and here it's located again, i.e. the element is "dynamic"
-```
+#                      ⬆
+#                  and here it's located again, i.e. the element is "dynamic"
 
-AND (in case we need to filter collection of items by some condition like visibility):
+# AND in case we need to filter collection of items 
+#     by some condition like visibility:
 
-```python
 from selene import be
+results = browser.all('#rso>div').by(be.visible)
 
-results = browser.all('.srg .g').filtered_by(be.visible)
-```
-
-THEN:
-
-```python
+# THEN we can assert some condition:
 from selene import have
-
-# results.should(have.size(10))
+# results.should(have.size_greater_than(5))
 # results.first.should(have.text('Selenium automates browsers'))
 # OR...
-
-results.should(have.size(10))\
+results.should(have.size_greater_than(5))\
     .first.should(have.text('Selenium automates browsers'))
-```
-
-FINALLY (if not registered "atexit" before):
 
-```python
+# FINALLY the browser can be quit:
 browser.quit()
+# but it's not mandatory, because by default Selenes kills all drivers on exit
+# that can be disabled by:
+browser.config.hold_driver_at_exit = True
 ```
 
 ### Automatic Driver and Browser Management
 
 Instead of:
 
 ```python
+from selenium.webdriver import Chrome
 from selene import Browser, Config
 
-browser = Browser(Config(
-    driver=Chrome(),
-    base_url='https://google.com',
-    timeout=2))
+browser = Browser(
+    Config(
+        driver=Chrome(),
+        base_url='https://google.com',
+        timeout=2
+    )
+)
+
+browser.open('/ncr')
 ```
-You can simply use the browser and config instance predefined for you in `selene.support.shared` module:
+
+You can simply use the browser instance predefined for you in `selene` module:
 
 ```python
-from selene.support.shared import browser, config
+from selene import browser
+
+browser.config.base_url = 'https://google.com'
+browser.config.timeout = 2
 
-# ... do the same with browser.*
+browser.open('/ncr')
 ```
+
 So you don't need to create you driver instance manually. It will be created for you automatically.
 
-Yet, if you need some special case, like working with remote driver, etc., you can still use shared browser object, while providing driver to it through:
+Yet, if you need some special case, like working with remote driver, etc., you can still use shared browser object with additional configuration:
+
+```python
+from selenium import webdriver
+from selene import browser
+
+options = webdriver.ChromeOptions()
+options.add_argument('--headless')
+options.add_argument('--no-sandbox')
+options.add_argument('--disable-gpu')
+options.add_argument('--disable-notifications')
+options.add_argument('--disable-extensions')
+options.add_argument('--disable-infobars')
+options.add_argument('--enable-automation')
+options.add_argument('--disable-dev-shm-usage')
+options.add_argument('--disable-setuid-sandbox')
+browser.config.driver_options = options
+browser.config.driver_remote_url = 'http://localhost:4444/wd/hub', 
+browser.config.base_url = 'https://google.com'
+browser.config.timeout = 2
+
+browser.open('/ncr')
+...
+```
+
+But if you like to create the driver on your own, you can do it too:
 
 ```python
-config.driver = my_remote_driver_instance
-# or
-browser.config.driver = my_remote_driver_instance
+from selenium import webdriver
+from selene import browser
+
+options = webdriver.ChromeOptions()
+options.add_argument('--headless')
+# ... other arguments
+browser.config.driver = webdriver.Remote(
+  'http://localhost:4444/wd/hub', 
+  options=options
+)
+# Once you start to build and set the driver on your own,
+# probably you are going to fully manage it life cycle,
+# thus, consider disabling the automatic driver reset on browser.open
+# if driver was crashed or quit:
+browser.config._reset_not_alive_driver_on_get_url = False
+# And consider disabling the automatic driver quit on exit:
+browser.config.hold_driver_at_exit = True
+# Other common options will still be useful:
+browser.config.base_url = 'https://google.com'
+browser.config.timeout = 2
+
+browser.open('/ncr')
+...
+
+# Finally, you can quit the driver manually:
+browser.quit()
 ```
 
 ### Advanced API
 
-Sometimes you might need some extra actions on elements, e.g. for workaround something through js:
+Sometimes you might need some extra things to reach your specific goals... Here go examples of Selene's `command`, `query`, custom conditions, `.matching(condition)` and `.wait_until(condition)`...
 
 ```python
+from selene import browser, have
+
+...
+
+###################################################
+# Maybe you need some advanced actions on elements,
+# e.g. for workaround something through js:
+
 from selene import command
 
 browser.element('#not-in-view').perform(command.js.scroll_into_view)
-```
 
-Probably you think that will need something like:
+...
+
+###################################################
+# Probably you think that will need something like:
 
-```python
 from selene import query
 
-product_text = browser.element('#to-assert-something-non-standard').get(query.text)
+...
+
+def my_int_from(text):
+    return int(text.split(' ')[0])
+
+product_text = browser.element('#price-label').get(query.text)
+# ... to assert something not standard:
 price = my_int_from(product_text)
 assert price > 100
-```
 
-But usually it's either better to implement your custom condition:
+# But such version is very unstable in dynamic web world...
+# Usually it's...
+# either better to implement your custom condition:
+
+from selene.core.condition import Condition
+from selene.core.conditions import ElementCondition
+from selene.core.entity import Element
+
+
+def have_in_text_the_int_number_more_than(number) -> Condition[Element]:
+    def fn(element: Element) -> None:
+        text = element.get(query.text)
+        parsed_number = my_int_from(text)
+        if not parsed_number > number:
+            raise AssertionError(
+                f'actual text was: {text}'
+                f'with parsed int number: {parsed_number}'
+            )
+    return ElementCondition(
+        f'has in text the int number more than: {number}', 
+        fn
+    )
+
+
+browser.element('#price-label').should(
+    have_in_text_the_int_number_more_than(100)
+)
+'''
+# You even can create your own project_package/selene_extensions/have.py
+# with the following content:
+
+from selene.support.conditioins.have import *
+
+def int_number_more_than(number) -> Condition[Element]:
+    def fn(element: Element) -> None:
+        text = element.get(query.text)
+        parsed_number = my_int_from(text)
+        if not parsed_number > number:
+            raise AssertionError(
+                f'actual text was: {text}'
+                f'with parsed int number: {parsed_number}'
+            )
+    return ElementCondition(
+        f'has in text the int number more than: {number}', 
+        fn
+    )
+    
+# And then in your test:
 
-```python
-browser.element('#to-assert-something-non-standard').should(have_in_text_the_int_number_more_than(100))
-```
+from project_package.selene_extensions import have
 
-Where the `have_in_text_the_int_number_more_than` is your defined custom condition. Such condition-based alternative will be less fragile, because python's assert does not have "implicit waiting", like selene's should ;)
+browser.element('#price-label').should(have.text('Price: ') \
+    .should(have.int_number_more_than(100))
 
+# i.e. using it same style as in selene,
+# with also access to all original selene conditions
+'''
 
-Furthermore, the good test is when you totally control your test data, and instead:
+# Such condition-based alternative to the original `assert price > 100` is less fragile,
+# because Python's `assert` does not have "implicit waiting",
+# while Selene's `should` command does have ;)
+
+# Furthermore, the good test is when you totally control your test data, 
+# and the code like below:
 
-```python
 product = browser.element('#to-remember-for-future')
 
 product_text_before = product.get(query.text)
 price_before = my_int_from(product_text_before)
 
-# ... do something
+... # some test steps
 
 product_text_after = product.get(query.text)
 price_after = my_int_from(product_text_after)
 
 assert price_after > price_before
-```
 
-Normally, better would be to refactor to something like:
+# – normally, should be refactored to something like:
 
-```python
 product = browser.element('#to-remember-for-future')
 
 product.should(have.text('100$'))
 
-# ... do something
+... # some test steps
 
 product.should(have.text('125$'))
-```
-You might think you need something like:
 
-```python
+
+###############################################
+# You might also think you need something like:
+
 from selene import query
 
 if browser.element('#i-might-say-yes-or-no').get(query.text) == 'yes':
-    # do something...
-```
+    ...  # do something...
 
-Or:
+# Or:
 
-```python
 from selene import query
 
 if browser.all('.option').get(query.size) >= 2:
-    # do something...
-```
+    ...  # do something...
 
-Maybe one day, you really find a use case:) But for above cases, probably easier would be:
+# – maybe, one day, you really find a use case:)
+
+# But for above cases, probably easier would be:
 
-```python
 if browser.element('#i-might-say-yes-or-no').wait_until(have.text('yes')):
-    # do something
+    ...  # do something
 
-# ...
+...
 
 if browser.all('.i-will-appear').wait_until(have.size_greater_than_or_equal(2)):
-    # do something
-```
+    ...  # do something
 
-Or, by using non-waiting versions, if "you are in a rush:)":
+# Or, by using non-waiting versions, if "you are in a rush:)":
 
-```python
 if browser.element('#i-might-say-yes-or-no').matching(have.text('yes')):
-    # do something
+    ...  # do something
 
-# ...
+...
 
 if browser.all('.i-will-appear').matching(have.size_greater_than_or_equal(2)):
-    # do something
+    ... # do something
 ```
 
-
 ## Tutorials
 
 TBD
 
-## More examples
+## More Examples
 
-* [Project template](https://github.com/yashaka/python-web-test)
+- [Project template][project-template]
 
 TBD
 
-## Contributing
+## Contribution
 
-[see CONTRIBUTING.md](https://github.com/yashaka/selene/blob/master/CONTRIBUTING.md)
+[see CONTRIBUTING.md][contribution]
 
-## Release Process
+## Release Workflow
 
-[see CONTRIBUTING.md#release-process](https://github.com/yashaka/selene/blob/master/CONTRIBUTING.md#release-process)
+[see Release workflow][release-workflow]
 
 ## Changelog
 
-[see CHANGELOG.md](https://github.com/yashaka/selene/blob/master/CHANGELOG.md)
+[see CHANGELOG.md][changelog]
+
+<!-- References -->
+[selenide]: http://selenide.org/
+[latest-recommended-version]: https://pypi.org/project/selene/2.0.0b17/
+[brunch-ver-1]: https://github.com/yashaka/selene/tree/1.x
+[selene-stable]: https://pypi.org/project/selene/1.0.2/
+[python-37]: https://www.python.org/downloads/release/python-370/
+[pyenv]: https://github.com/pyenv/pyenv
+[poetry]: https://python-poetry.org/
+[project-template]: https://github.com/yashaka/python-web-test
+<!-- --8<-- [end:githubSection] -->
+
+<!-- GitHub only references -->
+[contribution]: https://yashaka.github.io/selene/contribution/to-source-code-guide/
+[release-workflow]: https://yashaka.github.io/selene/contribution/release-workflow-guide/
+[changelog]: https://yashaka.github.io/selene/changelog/
+
```

### Comparing `selene-2.0.0b9/pyproject.toml` & `selene-2.0.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "selene"
-version = "2.0.0b9"
+version = "2.0.0rc1"
 description = "User-oriented browser tests in Python (Selenide port)"
 authors = ["Iakiv Kramarenko <yashaka@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
 	"testing",
 	"selenium",
 	"selenide",
 	"browser",
 	"pageobject",
 	"widget",
 	"wrapper"
 ]
-homepage = "http://github.com/yashaka/selene/"
+homepage = "https://yashaka.github.io/selene/"
+repository = "http://github.com/yashaka/selene/"
+documentation = "https://yashaka.github.io/selene/"
 classifiers = [
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Development Status :: 3 - Alpha",
 	"Natural Language :: English",
 	"Environment :: Web Environment",
 	"Intended Audience :: Developers",
@@ -33,37 +35,65 @@
 	{include = "selene"},
 	{include = "selene/api"},
 	{include = "selene/common"},
 	{include = "selene/core"},
 	{include = "selene/support"},
 	{include = "selene/support/shared"},
 	{include = "selene/support/conditions"},
+	{include = "selene/py.typed"}
 ]
 
+[tool.poetry.urls]
+Changelog = "https://github.com/yashaka/selene/releases"
+
 [tool.poetry.dependencies]
 python = "^3.7"
-selenium = "==4.2.0"
+selenium = ">=4.4.3"
 future = "*"
-webdriver-manager = "==3.7.0"
+webdriver-manager = ">=3.8.5"
 typing-extensions = "==4.3.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
+black = "^23.3.0"
 pycodestyle = "*"
 pylint = "^2.7.2"
 pytest = "*"
 pytest-cov = "*"
 codecov = "*"
+mypy = "*"
+pydantic = "^1.10.7"
+python-dotenv = "0.21.1"
+Appium-Python-Client = "^2.9.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.2"
+mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocs-redirects = "^1.2.0"
+mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.mypy]
+disable_error_code = 'annotation-unchecked'
+allow_redefinition = true  # TODO: how to properly make it work o_O ?
+color_output=1
+exclude = [
+    '^test_.+\.py$',
+	'^.+_test\.py$',
+]
+
+
 [tool.black]
-line-length = 79
+line-length = 88
 target-version = ['py37']
 skip-string-normalization = 1
 
 [tool.pylint]
 	[tool.pylint.master]
 	ignore=['CVS']
 	jobs=1
@@ -71,14 +101,28 @@
 	unsafe-load-any-extension=['no']
 	suggestion-mode=['yes']
 	fail-under=['10.0']
 
 	[tool.pylint.'MESSAGES CONTROL']
 	enable=['c-extension-no-member']
 	disable=['''no-else-return,
+		import-outside-toplevel,
+		too-many-locals,
+		too-many-lines,
+		invalid-name,
+		not-callable,
+		unused-argument,
+		protected-access,
+		pointless-string-statement,
+		too-few-public-methods,
+		too-many-public-methods,
+		redefined-outer-name,
+	    missing-class-docstring,
+	    missing-module-docstring,
+	    missing-function-docstring,
         no-else-raise,
         print-statement,
         parameter-unpacking,
         unpacking-in-except,
         old-raise-syntax,
         backtick,
         long-suffix,
@@ -170,15 +214,15 @@
 	logging-modules=['logging']
 
 	[tool.pylint.'SPELLING']
 	max-spelling-suggestions=4
 	spelling-store-unknown-words=['no']
 
 	[tool.pylint.'MISCELLANEOUS']
-	notes=['FIXME,XXX,TODO']
+	notes=['FIXME,XXX']
 
 	[tool.pylint.'TYPECHECK']
 	contextmanager-decorators=['contextlib.contextmanager']
 	ignore-mixin-members=['yes']
 	ignore-none=['yes']
 	ignore-on-opaque-inference=['yes']
 	ignored-classes=['optparse.Values,thread._local,_thread._local']
@@ -194,15 +238,15 @@
 	init-import=['no']
 	redefining-builtins-modules=['six.moves,past.builtins,future.builtins,builtins,io']
 
 	[tool.pylint.'FORMAT']
 	ignore-long-lines=['^\s*(# )?<?https?://\S+>?$']
 	indent-after-paren=4
 	indent-string='    '
-	max-line-length=79
+	max-line-length=88
 	max-module-lines=1000
 	single-line-class-stmt=['no']
 	single-line-if-stmt=['no']
 
 	[tool.pylint.'SIMILARITIES']
 	ignore-comments=['yes']
 	ignore-docstrings=['yes']
@@ -247,12 +291,12 @@
 	max-attributes=7
 	max-bool-expr=5
 	max-branches=12
 	max-locals=15
 	max-parents=7
 	max-public-methods=20
 	max-returns=6
-	max-statementts=50
+	max-statements=80
 	min-public-methods=2
 
 	[tool.pylint.'EXCEPTIONS']
-	overgeneral-exceptions=['BaseException,Exception']
+	overgeneral-exceptions=['BaseException,Exception']
```

### Comparing `selene-2.0.0b9/selene/__init__.py` & `selene-2.0.0rc1/selene/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,28 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from . import support
+
+from selene.core.configuration import (
+    Config as _CustomConfigForCustomBrowser,
+)
+
+Config = _CustomConfigForCustomBrowser
 
 from selene.core.entity import (
-    Browser as _custom_browser,
-    Config as _custom_config_for_custom_browser,
+    Browser as _CustomBrowser,
 )
 
-Config = _custom_config_for_custom_browser
-Browser = _custom_browser
+Browser = _CustomBrowser
+
 """
 Given::
 
     from selenium.webdriver import Chrome
 
 AND chromedriver executable available in $PATH
 
@@ -51,16 +57,19 @@
 
 AND::
 
     browser.open('/ncr')
 
 """
 
+from selene import _managed  # noqa
 
-from selene.support import by as _by_style_selectors
+browser = _managed.browser
+
+from selene.support import by as _by_style_selectors  # noqa
 
 by = _by_style_selectors
 """
 AND::
 
     # browser.element('//*[@name="q"]')).type('selenium').press_enter()
     # OR...
@@ -76,28 +85,26 @@
     query = browser.element(by.name('q'))  # actual search doesn't start here, the element is "lazy"
          # here the actual webelement is found
     query.type('selenium').press_enter()
                           # and here it's located again, i.e. the element is "dynamic"
 
 """
 
-
-from selene.support.conditions import be as _be_style_conditions
+from selene.support.conditions import be as _be_style_conditions  # noqa
 
 be = _be_style_conditions
 """
 AND (in case we need to filter collection of items by some condition like visibility)::
 
     from selene import be
 
     results = browser.all('.srg .g').filtered_by(be.visible)
 """
 
-
-from selene.support.conditions import have as _have_style_conditions
+from selene.support.conditions import have as _have_style_conditions  # noqa
 
 have = _have_style_conditions
 """
 THEN::
     from selene import have
 
     # results.should(have.size(10))
@@ -109,33 +116,33 @@
 
 FINALLY (if not registered "atexit" before)::
 
     browser.quit()
 """
 
 ####################
-# Advanced Helpers #  # todo: think on not adding them here...
+# Advanced Helpers #
 ####################
 
-from selene.core import command as _advanced_commands
+from selene.core import command as _advanced_commands  # noqa
 
 command = _advanced_commands
 """
 Sometimes you might need some extra actions on elements,
 e.g. for workaround something through js::
 
     from selene import command
 
     browser.element('#not-in-view').perform(command.js.scroll_into_view)
 """
 
-from selene.core import query as _advanced_queries
+from selene.core import query as _advanced_queries  # noqa
 
 query = _advanced_queries
-# its = _advanced_queries  # todo: do we really need it too? for better readability: .get(its.text)
+# its = _advanced_queries  # TODO: do we really need it too? for better readability: .get(its.text)
 """
 Probably you think that will need something like::
 
     from selene import query
 
     product_text = browser.element('#to-assert-something-non-standard').get(query.text)
     price = my_int_from(product_text)
@@ -214,10 +221,10 @@
         # do something
 
 """
 
 # """
 # Just types...
 # """
-# todo: add here some type imports like Element, Collection, etc.
+from selene.core.entity import Element, Collection  # noqa
 
-__version__ = '2.0.0b9'
+__version__ = '2.0.0rc1'
```

### Comparing `selene-2.0.0b9/selene/api/__init__.py` & `selene-2.0.0rc1/selene/api/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/selene/api/base/__init__.py` & `selene-2.0.0rc1/selene/api/base/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from selene.core.entity import Browser
 from selene.core.configuration import Config
 
 from selene.support import by
 
 from selene.support.conditions import be, have
 
-# todo: probably we don't need it... it's currently removed from distribution
+# TODO: probably we don't need it... it's currently removed from distribution
```

### Comparing `selene-2.0.0b9/selene/api/shared/__init__.py` & `selene-2.0.0rc1/selene/api/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/selene/common/fp.py` & `selene-2.0.0rc1/selene/common/fp.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import functools
-from typing import TypeVar, Callable, Optional
+from typing import TypeVar, Callable, Any, Tuple, Optional
 
+# T = TypeVar('T', bound=Callable[..., Any])
 T = TypeVar('T')
 '''
 A generic TypeVar to identify a Function Type, i.e. a function
 but to be imported and used as fp.T so you can guess from full name,
 that it is "function type", i.e. a function ;)
 '''
 F = TypeVar('F')
@@ -57,22 +58,45 @@
 '''
 
 
 def identity(it: T) -> T:
     return it
 
 
-def pipe(*functions):
+def pipe(*functions) -> Optional[Callable[[Any], Any]]:
     """
     pipes functions one by one in the provided order
     i.e. applies arg1, then arg2, then arg3, and so on
     if any arg is None, just skips it
     """
     return (
         functools.reduce(
             lambda f, g: lambda x: f(g(x)) if g else f(x),
             functions[::-1],
             lambda x: x,
         )
         if functions
         else None
     )
+
+
+def thread(arg, *functions):
+    return pipe(*functions)(arg)
+
+
+def do(function: Callable[[T], Any]) -> Callable[[T], T]:
+    def func(arg: T) -> T:
+        function(arg)
+        return arg
+
+    return func
+
+
+def write_silently(
+    file: str, string: str, encoding: str = 'utf-8'
+) -> Optional[Tuple[str, str]]:
+    try:
+        with open(file, 'w', encoding=encoding) as f:
+            f.write(string)
+            return file, string
+    except OSError:
+        return None
```

### Comparing `selene-2.0.0b9/selene/common/helpers.py` & `selene-2.0.0rc1/selene/common/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import warnings
-from typing import Union, Tuple, List, Type
+from typing import Union, Tuple, Iterable, Any
 
-from dataclasses import dataclass
 from selenium.webdriver.common.by import By
 
 
 def as_dict(o, skip_empty=True):
     return (
         {
             k: v
@@ -34,16 +32,16 @@
             if not (skip_empty and v is None) and not k.startswith('_')
         }
         if o
         else {}
     )
 
 
-def to_by(selector_or_by: Union[str, tuple]) -> Tuple[str, str]:
-    # todo: will it work `if isinstance(css_selector_or_by, Tuple[str, str]):` ?
+def to_by(selector_or_by: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
+    # TODO: will it work `if isinstance(css_selector_or_by, Tuple[str, str]):` ?
     if isinstance(selector_or_by, tuple):
         return selector_or_by
     if isinstance(selector_or_by, str):
         return (
             (By.XPATH, selector_or_by)
             if (
                 selector_or_by.startswith('/')
@@ -54,21 +52,25 @@
             else (By.CSS_SELECTOR, selector_or_by)
         )
     raise TypeError(
         'selector_or_by should be str with CSS selector or XPATH selector or Tuple[by:str, value:str]'
     )
 
 
-def flatten(list_of_lists: List[list]) -> list:
-    # todo: consider adding skip_none=False option
-    return [
-        item
-        for sublist in list_of_lists
-        for item in (sublist if isinstance(sublist, list) else [sublist])
-    ]
+def flatten(collection: Iterable[Union[Iterable[Any], Any]]) -> Iterable[Any]:
+    # TODO: consider adding skip_none=False option
+    return tuple(  # TODO: refactor to return tuple
+        item_or_inner
+        for item in collection
+        for item_or_inner in (
+            item
+            if (isinstance(item, Iterable) and not isinstance(item, str))
+            else [item]
+        )
+    )
 
 
 def dissoc(associated: dict, *keys: str) -> dict:
     return {k: v for k, v in associated.items() if k not in keys}
 
 
 def on_error_return_false(no_args_predicate):
```

### Comparing `selene-2.0.0b9/selene/common/none_object.py` & `selene-2.0.0rc1/selene/common/none_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,12 @@
 class _NoneObject:
     def __init__(self, description):
         # type: (str) -> None
         self.description = description
 
     def __getattr__(self, item):
         raise AttributeError(
-            "'NoneObject' for «'%s'» has no attribute '%s'"
-            % (self.description, item)
+            "'NoneObject' for «'%s'» has no attribute '%s'" % (self.description, item)
         )
 
     def __bool__(self):
         return False
```

### Comparing `selene-2.0.0b9/selene/common/predicate.py` & `selene-2.0.0rc1/selene/common/predicate.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,33 +70,31 @@
         except TypeError:
             return False
 
     return fn
 
 
 def includes_word_ignoring_case(expected):
-    return lambda actual: str(expected).lower() in re.split(
-        r'\s+', str(actual).lower()
-    )
+    return lambda actual: str(expected).lower() in re.split(r'\s+', str(actual).lower())
 
 
 def includes_word(expected, ignore_case=False):
     return (
         lambda actual: expected in re.split(r'\s+', actual)
         if not ignore_case
         else includes_ignoring_case(expected)
     )
 
 
-# will not work with empty seqs :( todo: fix
+# will not work with empty seqs :( TODO: fix
 # currently we use it only for non-empty seqs taking this into account
 seq_compare_by = (
     lambda f: lambda x=None, *xs: lambda y=None, *ys: True
     if x is None and y is None
-    else bool(f(x)(y)) and seq_compare_by(f)(*xs)(*ys)
+    else bool(f(x)(y)) and seq_compare_by(f)(*xs)(*ys)  # type: ignore
 )
 
 
 # def seq_compare_by_2(f):
 #     def fn(x, *xs):
 #         def fn(y, *ys):
 #             return True if x is None and y is None else \
```

### Comparing `selene-2.0.0b9/selene/core/__init__.py` & `selene-2.0.0rc1/selene/core/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/selene/core/condition.py` & `selene-2.0.0rc1/selene/core/condition.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,37 +19,43 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 import sys
-from typing import List, TypeVar, Generic
+import typing
+from typing import List, TypeVar, Generic, Iterable, Tuple, Optional
+
+from selene.core.exceptions import ConditionNotMatchedError
+from selene.core.wait import Predicate, Lambda
 
 if sys.version_info >= (3, 10):
     from collections.abc import Callable
 else:
     from typing import Callable
 
-from selene.core.exceptions import ConditionNotMatchedError
-from selene.core.wait import Predicate, Lambda
-
 
 E = TypeVar('E')
 R = TypeVar('R')
 
 
-class Condition(Generic[E], Callable[[E], None]):
+class Condition(Generic[E]):
+    """
+    Class for objects that are `Callable[[E], None]` like
+    and represent the "condition that can pass or fail".
+    """
+
     @classmethod
     def by_and(cls, *conditions):
-        def fn(entity):
+        def func(entity):
             for condition in conditions:
                 condition.call(entity)
 
-        return cls(' and '.join(map(str, conditions)), fn)
+        return cls(' and '.join(map(str, conditions)), func)
 
     @classmethod
     def by_or(cls, *conditions):
         def fn(entity):
             errors: List[Exception] = []
             for condition in conditions:
                 try:
@@ -58,45 +64,63 @@
                 except Exception as e:
                     errors.append(e)
             raise AssertionError('; '.join(map(str, errors)))
 
         return cls(' or '.join(map(str, conditions)), fn)
 
     @classmethod
+    def for_each(cls, condition) -> Condition[Iterable[E]]:
+        def fn(entity):
+            items_with_error: List[Tuple[str, str]] = []
+            index = None
+            for index, item in enumerate(entity):
+                try:
+                    condition.call(item)
+                except Exception as error:
+                    items_with_error.append((str(item), str(error)))
+            if items_with_error:
+                raise AssertionError(
+                    f'Not matched elements among all with indexes from 0 to {index}:\n'
+                    + '\n'.join(
+                        [f'{item}: {error}' for item, error in items_with_error]
+                    )
+                )
+
+        return typing.cast(Condition[Iterable[E]], cls(f' each {condition}', fn))
+
+    @classmethod
     def as_not(
-        cls, condition: Condition[E], description: str = None
+        cls, condition: Condition[E], description: Optional[str] = None
     ) -> Condition[E]:
-        # todo: how will it work composed conditions?
+        # TODO: how will it work composed conditions?
         condition_words = str(condition).split(' ')
         is_or_have = condition_words[0]
         name = ' '.join(condition_words[1:])
         no_or_not = 'not' if is_or_have == 'is' else 'no'
         new_description = description or f'{is_or_have} {no_or_not} ({name})'
 
         def fn(entity):
             try:
                 condition.call(entity)
             except Exception:
                 return
-            raise ConditionNotMatchedError()  # todo: try to handle printing actual values here too...
+            raise ConditionNotMatchedError()  # TODO: try to handle printing actual values here too...
 
         return cls(new_description, fn)
 
     # function throwIfNot<E>(predicate: (entity: E) => Promise<boolean>): Lambda<E, void> {
     #     return async (entity: E) => {
     #         if (!await predicate(entity)) {
     #             throw new ConditionNotMatchedError();
     #         }
     #     };
     # }
 
     @classmethod
-    def raise_if_not(
-        cls, description: str, predicate: Predicate[E]
-    ) -> Condition[E]:
+    def raise_if_not(cls, description: str, predicate: Predicate[E]) -> Condition[E]:
         def fn(entity: E) -> None:
             if not predicate(entity):
                 raise ConditionNotMatchedError()
 
         # TODO: consider the following style as one more option:
         #
         # @condition(description)  # or: @Condition.describe(description)
@@ -111,17 +135,15 @@
     @classmethod
     def raise_if_not_actual(
         cls, description: str, query: Lambda[E, R], predicate: Predicate[R]
     ) -> Condition[E]:
         def fn(entity: E) -> None:
             query_to_str = str(query)
             result = (
-                query.__name__
-                if query_to_str.startswith('<function')
-                else query_to_str
+                query.__name__ if query_to_str.startswith('<function') else query_to_str
             )
             actual = query(entity)
             if not predicate(actual):
                 raise AssertionError(f'actual {result}: {actual}')
 
         return cls(description, fn)
 
@@ -140,28 +162,32 @@
                 return True
             except Exception as e:
                 return False
 
         return fn
 
     @property
-    def not_(self) -> Condition[E]:  # todo: better name?
+    def not_(self) -> Condition[E]:  # TODO: better name?
         return self.__class__.as_not(self)
 
     def __call__(self, entity: E) -> None:
         return self._fn(entity)
 
     def __str__(self):
-        # todo: consider changing has to have on the fly for CollectionConditions
-        # todo: or changing in collection locator rendering `all` to `collection`
-        # todo: or changing in match.* names from collection_has_* to all_have_*
+        # TODO: consider changing has to have on the fly for CollectionConditions
+        # TODO: or changing in collection locator rendering `all` to `collection`
+        # TODO: or changing in match.* names from collection_has_* to all_have_*
         return self._description
 
     def and_(self, condition: Condition[E]) -> Condition[E]:
         return Condition.by_and(self, condition)
 
     def or_(self, condition: Condition[E]) -> Condition[E]:
         return Condition.by_or(self, condition)
 
+    @property
+    def each(self) -> Condition[Iterable[E]]:
+        return Condition.for_each(self)
+
 
-def not_(condition_to_be_inverted: Condition):  # todo: do we really need it?
+def not_(condition_to_be_inverted: Condition):  # TODO: do we really need it?
     return condition_to_be_inverted.not_
```

### Comparing `selene-2.0.0b9/selene/core/conditions.py` & `selene-2.0.0rc1/selene/core/conditions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/selene/core/entity.py` & `selene-2.0.0rc1/selene/core/entity.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,86 +15,96 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
 from __future__ import annotations
 
+import os
+import typing
 import warnings
 
 from abc import abstractmethod, ABC
-from typing import TypeVar, Union, List, Callable, Tuple
+from typing import TypeVar, Union, Callable, Tuple, Iterable, Optional
 
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.switch_to import SwitchTo
 from selenium.webdriver.remote.webelement import WebElement
 
 from selene.common.fp import pipe
+
 from selene.core.configuration import Config
 from selene.core.wait import Wait, Command, Query
 from selene.core.condition import Condition
 from selene.core.locator import Locator
 
 from selene.common.helpers import to_by, flatten, is_absolute_url
 from selene.core.exceptions import TimeoutException, _SeleneError
+from selene.support.webdriver import WebHelper
+
 
 E = TypeVar('E', bound='Assertable')
 R = TypeVar('R')
 
 
-class Assertable(ABC):
+class Assertable(ABC, typing.Generic[E]):
     @abstractmethod
     # TODO: shouldn't we type self too?
     #       see #generic-methods-and-generic-self
     #       at https://mypy.readthedocs.io/en/stable/generics.html
     # def should(self: E, condition: Condition[E]) -> E:
     def should(self, condition: Condition[E]) -> E:
         pass
 
 
-# todo: try as Matchable(ABC) and check if autocomplete will still work
-class Matchable(Assertable):
+# TODO: try as Matchable(ABC) and check if autocomplete will still work
+class Matchable(Assertable[E]):
     @abstractmethod
     def wait_until(self, condition: Condition[E]) -> bool:
         pass
 
     @abstractmethod
     def matching(self, condition: Condition[E]) -> bool:
         pass
 
 
+# class Configured(ABC, typing.Generic[E]):
 class Configured(ABC):
     @property
     @abstractmethod
     def config(self) -> Config:
         pass
 
+    # @abstractmethod
+    # def with_(self, config: Optional[Config] = None, **config_as_kwargs) -> E:
+    #     pass
 
-class WaitingEntity(Matchable, Configured):
+
+class WaitingEntity(Matchable[E], Configured):
     def __init__(self, config: Config):
         self._config = config
 
     @property
     def wait(self) -> Wait[E]:
-        return self.config.wait(self)
+        return self.config.wait(typing.cast(E, self))  # type: ignore
 
     def perform(self, command: Command[E]) -> E:
         """Useful to call external commands.
 
         Commands might be predefined in Selene:
             element.perform(command.js.scroll_into_view)
         or some custom defined by selene user:
             element.perform(my_action.triple_click)
 
-        You might think that it will be useful to use these methods also in Selene internally
+        You might think that it will be useful
+        to use these methods also in Selene internally
         in order to define built in commands e.g. in Element class, like:
 
             def click(self):
                 return self.perform(Command('click', lambda element: element().click()))
 
         instead of:
 
@@ -103,199 +113,239 @@
                 return self
 
         But so far, we use the latter version - though, less concise, but more explicit,
         making it more obvious that waiting is built in;)
 
         """
         self.wait.for_(command)
-        return self
+        return typing.cast(E, self)
 
-    # todo: what about `entity[query.something]` syntax over or in addition to `entity.get(query.something)` ?
+    # TODO: what about `entity[query.something]` syntax
+    #       over or in addition to `entity.get(query.something)` ?
     def get(self, query: Query[E, R]) -> R:
         return self.wait.for_(query)
 
     # --- Configured --- #
 
     @property
     def config(self) -> Config:
         return self._config
 
     # --- Assertable --- #
 
     def should(self, condition: Condition[E]) -> E:
         self.wait.for_(condition)
-        return self
+        return typing.cast(E, self)
 
     # --- Matchable --- #
 
     def wait_until(self, condition: Condition[E]) -> bool:
         return self.wait.until(condition)
 
     def matching(self, condition: Condition[E]) -> bool:
-        return condition.predicate(self)
+        return condition.predicate(typing.cast(E, self))
 
 
-class Element(WaitingEntity):
+class Element(WaitingEntity['Element']):
     @staticmethod
     def _log_webelement_outer_html_for(
         element: Element,
     ) -> Callable[[TimeoutException], Exception]:
         def log_webelement_outer_html(error: TimeoutException) -> Exception:
             from selene.core import query
             from selene.core.match import element_is_present
 
             cached = element.cached
 
             if cached.matching(element_is_present):
                 return TimeoutException(
-                    error.msg
-                    + f'\nActual webelement: {query.outer_html(element)}'
+                    f'{error.msg}\n'
+                    f'Actual webelement: {query.outer_html(element)}'  # type: ignore
                 )
             else:
                 return error
 
         return log_webelement_outer_html
 
-    # todo: should we move locator based init and with_ to Located base abstract class?
+    # TODO: should we move locator based init and with_ to Located base abstract class?
 
     def __init__(self, locator: Locator[WebElement], config: Config):
         self._locator = locator
         super().__init__(config)
 
     # --- Configured --- #
 
-    def with_(self, config: Config = None, **config_as_kwargs) -> Element:
+    def with_(self, config: Optional[Config] = None, **config_as_kwargs) -> Element:
         return Element(
-            self._locator, self.config.with_(config, **config_as_kwargs)
+            self._locator,
+            config if config else self.config.with_(**config_as_kwargs),
         )
 
     # --- Located --- #
 
     def __str__(self):
         return str(self._locator)
 
-    def __call__(self) -> WebElement:
+    def locate(self) -> WebElement:
         return self._locator()
 
+    @property
+    def __raw__(self):
+        return self.locate()
+
+    def __call__(self) -> WebElement:
+        return self.locate()
+
     # --- WaitingEntity --- #
 
     @property
-    def wait(self) -> Wait[E]:
-        # todo:  will not it break code like browser.with_(timeout=...)?
-        # todo: fix that will disable/break shared hooks (snapshots)
-        # return Wait(self,  # todo:  isn't it slower to create it each time from scratch? move to __init__?
+    def wait(self) -> Wait[Element]:
+        # TODO:  will not it break code like browser.with_(timeout=...)?
+        # TODO: fix that will disable/break shared hooks (snapshots)
+        # return Wait(self,  # TODO:  isn't it slower to create it each time from scratch? move to __init__?
         #             at_most=self.config.timeout,
         #             or_fail_with=pipe(
         #                 Element._log_webelement_outer_html_for(self),
         #                 self.config.hook_wait_failure))
         if self.config.log_outer_html_on_failure:
-            """
-            todo: remove this part completely from core.entity logic
-                  move it to support.shared.config
-            """
+            # TODO: remove this part completely from core.entity logic
+            #       move it to support.shared.config
             return super().wait.or_fail_with(
                 pipe(
                     Element._log_webelement_outer_html_for(self),
                     super().wait.hook_failure,
                 )
             )
         else:
             return super().wait
 
     @property
     def cached(self) -> Element:
-        # todo: do we need caching ? with lazy save of webelement to cache
+        # TODO: do we need caching ? with lazy save of webelement to cache
 
         cache = None
         error = None
         try:
             cache = self()
         except Exception as e:
             error = e
 
         def get_webelement():
             if cache:
                 return cache
             raise error
 
-        return Element(
-            Locator(f'{self}.cached', lambda: get_webelement()), self.config
-        )
+        return Element(Locator(f'{self}.cached', get_webelement), self.config)
 
     # --- Relative location --- #
 
-    def element(self, css_or_xpath_or_by: Union[str, tuple]) -> Element:
+    def element(self, css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Element:
         by = to_by(css_or_xpath_or_by)
 
         return Element(
             Locator(f'{self}.element({by})', lambda: self().find_element(*by)),
             self.config,
         )
 
-    def all(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
+    def all(self, css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Collection:
         by = to_by(css_or_xpath_or_by)
 
         return Collection(
             Locator(f'{self}.all({by})', lambda: self().find_elements(*by)),
             self.config,
         )
 
     # --- Commands --- #
 
-    def execute_script(self, script_on_self: str, *extra_args):
+    def execute_script(self, script_on_self: str, *arguments):
+        """
+        Executes JS script on self as webelement. Will not work for Mobile!
+
+        The script can use predefined parameters:
+        - ``element`` and ``self`` are aliases to this element handle, i.e. ``self.locate()`` or ``self()``.
+        - ``arguments`` are accessible from the script with same order and indexing as they are provided to the method
+
+        Examples::
+
+            browser.element('[id^=google_ads]').execute_script('element.remove()')
+            # OR
+            browser.element('[id^=google_ads]').execute_script('self.remove()')
+            '''
+            # are shortcuts to
+            browser.execute_script('arguments[0].remove()', browser.element('[id^=google_ads]')())
+            '''
+
+            browser.element('input').execute_script('element.value=arguments[0]', 'new value')
+            # OR
+            browser.element('input').execute_script('self.value=arguments[0]', 'new value')
+            '''
+            # are shortcuts to
+            browser.execute_script('arguments[0].value=arguments[1]', browser.element('input').locate(), 'new value')
+            '''
+        """
         driver: WebDriver = self.config.driver
         webelement = self()
-        # todo: should we wrap it in wait or not?
-        return driver.execute_script(script_on_self, webelement, *extra_args)
+        # TODO: should we wrap it in wait or not?
+        # TODO: should we add additional it and/or its aliases for element?
+        return driver.execute_script(
+            f'''
+                let element = arguments[0]
+                let self = arguments[0]
+                return (function(...args) {{
+                    {script_on_self}
+                }})(...arguments[1])
+            ''',
+            webelement,
+            arguments,
+        )
 
-    # todo: do we need this method?
+    # TODO: do we need this method?
     #       do we really need to wrap script into function(element,args) here?
     #       if yes... wouldn't it be better to use standard arguments name
     #       instead of args?
     #       for better integration with js support in jetbrains products?
     def _execute_script(
         self,
         script_on_self_element_and_args: str,
         *extra_args,
     ):
+        warnings.warn(
+            '._execute_script is now deprecated '
+            'in favor of .execute_script(script_on_self, *arguments) '
+            'that uses access to arguments (NOT args!) in the script',
+            DeprecationWarning,
+        )
         driver: WebDriver = self.config.driver
         webelement = self()
-        # todo: should we wrap it in wait or not?
+        # TODO: should we wrap it in wait or not?
         return driver.execute_script(
             f'''
                 return (function(element, args) {{
                     {script_on_self_element_and_args}
                 }})(arguments[0], arguments[1])
             ''',
             webelement,
             extra_args,
         )
 
-    # def __execute_script__(
-    #     self,
-    #     script_on_self_element_and_args: str,
-    #     *extra_args,
-    # ):
-    #     return self._execute_script(script_on_self_element_and_args, *extra_args)
-
     def set_value(self, value: Union[str, int]) -> Element:
-        # todo: should we move all commands like following or queries like in conditions - to separate py modules?
-        # todo: should we make them webelement based (Callable[[WebElement], None]) instead of element based?
+        # TODO: should we move all commands like following or queries like in conditions - to separate py modules?
+        # TODO: should we make them webelement based (Callable[[WebElement], None]) instead of element based?
         def fn(element: Element):
             webelement = (
                 element._actual_not_overlapped_webelement
                 if self.config.wait_for_no_overlap_found_by_js
                 else element()
             )
-            webelement.clear()  # todo: change to impl based not on clear, because clear generates post-events...
+            webelement.clear()  # TODO: change to impl based not on clear, because clear generates post-events...
             webelement.send_keys(str(value))
 
         from selene.core import command
 
-        # todo: should we log the webelement source in the command name below?
+        # TODO: should we log the webelement source in the command name below?
         #       i.e. change from:
         #
         #   else Command(f'set value: {value}', fn)
         #
         #       to more low level:
         #
         #   else (
@@ -307,31 +357,42 @@
         #
         self.wait.for_(
             command.js.set_value(value)
             if self.config.set_value_by_js
             else Command(f'set value: {value}', fn)
         )
 
-        # todo: consider returning self.cached, since after first successful call,
+        # TODO: consider returning self.cached, since after first successful call,
         #       all next ones should normally pass
         #       no waiting will be needed normally
         #       if yes - then we should pass fn commands to wait.for_ so the latter will return webelement to cache
         #       also it will make sense to make this behaviour configurable...
         return self
 
+    def set(self, value: Union[str, int]) -> Element:
+        """
+        Sounds similar to Element.set_value(self, value), but considered to be used in broader context.
+        For example, a use can say «Set gender radio to Male» but will hardly say «Set gender radio to value Male».
+        Now imagine, on your project you have custom html implementation of radio buttons,
+        and want to teach selene to set such radio-button controls
+        – you can do this via Element.set(self, value) method,
+        after monkey-patching it according to your behavior;)
+        """
+        return self.set_value(value)
+
     def _actual_visible_webelement_and_maybe_its_cover(
         self, center_x_offset=0, center_y_offset=0
     ) -> Tuple[WebElement, WebElement]:
-        # todo: will it be faster render outerHTML via lazy rendered SeleneError
+        # TODO: will it be faster render outerHTML via lazy rendered SeleneError
         #       instead of: throw `element ${element.outerHTML} is not visible`
         #       in below js
-        results = self._execute_script(
+        results = self.execute_script(
             '''
-                var centerXOffset = args[0];
-                var centerYOffset = args[1];
+                var centerXOffset = arguments[0];
+                var centerYOffset = arguments[1];
 
                 var isVisible = !!(
                     element.offsetWidth
                     || element.offsetHeight
                     || element.getClientRects().length
                 ) && window.getComputedStyle(element).visibility !== 'hidden'
 
@@ -399,14 +460,22 @@
             command.js.type(text)
             if self.config.type_by_js
             else Command(f'type: {text}', fn)
         )
 
         return self
 
+    def send_keys(self, *value) -> Element:
+        """
+        To be used for more low level operations like «uploading files», etc.
+        To simulate normal input of keys by user when typing – use Element.type(self, text).
+        """
+        self.wait.command('send keys', lambda element: element().send_keys(*value))
+        return self
+
     def press(self, *keys) -> Element:
         def fn(element: Element):
             webelement = (
                 element._actual_not_overlapped_webelement
                 if self.config.wait_for_no_overlap_found_by_js
                 else element()
             )
@@ -447,24 +516,27 @@
             )
             webelement.submit()
 
         self.wait.command('submit', fn)
 
         return self
 
-    # todo: add offset args with defaults, or add additional method, think on what is better
+    # TODO: add offset args with defaults, or add additional method, think on what is better
     def click(self) -> Element:
         """Just a normal click:)"""
 
+        def raw_click(element: Element):
+            element.locate().click()
+
         from selene.core import command
 
         self.wait.for_(
-            command.js.click
+            typing.cast(Command[Element], command.js.click)
             if self.config.click_by_js
-            else Command('click', lambda element: element().click())
+            else Command('click', raw_click)
         )
 
         return self
 
     def double_click(self) -> Element:
         actions: ActionChains = ActionChains(self.config.driver)
 
@@ -506,144 +578,111 @@
             )
             actions.move_to_element(webelement).perform()
 
         self.wait.command('hover', fn)
 
         return self
 
-    # todo: should we reflect queries as self methods? or not...
+    # TODO: should we reflect queries as self methods? or not...
     # pros: faster to query element attributes
     # cons: queries are not test oriented. test is steps + asserts
     #       so queries will be used only occasionally, then why to make a heap from Element?
     #       hence, occasionally it's enough to have them called as
     #           query.outer_html(element)  # non-waiting version
     #       or
     #           element.get(query.outer_html)  # waiting version
     # def outer_html(self) -> str:
     #     return self.wait.for_(query.outer_html)
 
-    # --- Assertable --- #
-
-    # we need this method here in order to make autocompletion work...
-    # unfortunately the "base class" version is not enough
-    def should(self, condition: Condition[Element]) -> Element:
-        super().should(condition)
-        return self
-
     # --- Deprecate or not? --- #
 
-    def s(self, css_or_xpath_or_by: Union[str, tuple]) -> Element:
+    def s(self, css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Element:
         # warnings.warn(
         #     "consider using more explicit `element` instead: browser.element('#foo').element('.bar')",
         #     SyntaxWarning)
         return self.element(css_or_xpath_or_by)
 
-    def ss(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
+    def ss(self, css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Collection:
         # warnings.warn(
         #     "consider using `all` instead: browser.element('#foo').all('.bar')",
         #     SyntaxWarning)
         return self.all(css_or_xpath_or_by)
 
-    def get_actual_webelement(self) -> WebElement:
-        warnings.warn(
-            "considering to be deprecated; use element as callable instead, like: browser.element('#foo')()",
-            PendingDeprecationWarning,
-        )
-        return self()
-
-    def set(self, value: Union[str, int]) -> Element:
-        warnings.warn(
-            "deprecated; use `set_value` method instead", DeprecationWarning
-        )
-        return self.set_value(value)
-
-    def send_keys(self, *value) -> Element:
-        # warnings.warn(
-        #     "send_keys is deprecated because the name is not user-oriented in context of web ui e2e tests; "
-        #     "use `type` for 'typing text', press(*key) or press_* for 'pressing keys' methods instead",
-        #     DeprecationWarning,
-        # )
-        # """
-        # was deprecated previously
-        # but deprecation was removed as an exception case
-        # because sometimes send_keys is used for low level stuff
-        # like sending values for files, etc...
-        # let's rethink this topic later...
-        # """
-        self.wait.command(
-            'send keys', lambda element: element().send_keys(*value)
-        )
-        return self
 
-
-class SeleneElement(Element):
-    warnings.warn(
-        'SeleneElement is deprecated, import Element class instead for  your needs'
-    )
-    pass
-
-
-class Collection(WaitingEntity):
-    def __init__(self, locator: Locator[List[WebElement]], config: Config):
+class Collection(WaitingEntity['Collection'], Iterable[Element]):
+    def __init__(self, locator: Locator[typing.Sequence[WebElement]], config: Config):
         self._locator = locator
         super().__init__(config)
 
-    def with_(self, config: Config = None, **config_as_kwargs) -> Collection:
+    def with_(self, config: Optional[Config] = None, **config_as_kwargs) -> Collection:
         return Collection(
-            self._locator, self.config.with_(config, **config_as_kwargs)
+            self._locator,
+            config if config else self.config.with_(**config_as_kwargs),
         )
 
     def __str__(self):
         return str(self._locator)
 
-    def __call__(self) -> List[WebElement]:
+    def locate(self) -> typing.Sequence[WebElement]:
         return self._locator()
 
     @property
+    def __raw__(self):
+        return self.locate()
+
+    def __call__(self) -> typing.Sequence[WebElement]:
+        return self.locate()
+
+    @property
     def cached(self) -> Collection:
         webelements = self()
-        return Collection(
-            Locator(f'{self}.cached', lambda: webelements), self.config
-        )
+        return Collection(Locator(f'{self}.cached', lambda: webelements), self.config)
 
     def __iter__(self):
         i = 0
         cached = self.cached
         while i < len(cached()):
             element = cached[i]
             yield element
             i += 1
 
     def __len__(self):
         from selene.core import query
 
         return self.get(query.size)
 
-    # todo: add config.index_collection_from_1, disabled by default
+    # TODO: add config.index_collection_from_1, disabled by default
     def element(self, index: int) -> Element:
         def find() -> WebElement:
-            webelements = self()
+            webelements = self.locate()
             length = len(webelements)
 
             if length <= index:
                 raise AssertionError(
                     f'Cannot get element with index {index} '
                     + f'from webelements collection with length {length}'
                 )
 
             return webelements[index]
 
         return Element(Locator(f'{self}[{index}]', find), self.config)
 
     @property
-    def first(self):
+    def first(self) -> Element:
         """
         A human-readable alias to .element(0) or [0]
         """
-        return self.element(0)
+        return typing.cast(Element, self[0])
+
+    @property
+    def second(self) -> Element:
+        """
+        A human-readable alias to .element(1) or [1]
+        """
+        return typing.cast(Element, self[1])
 
     @property
     def even(self):
         """
         A human-readable alias to [1::2], i.e. filtering collection to have only even elements
         """
         return self[1::2]
@@ -652,20 +691,23 @@
     def odd(self):
         """
         A human-readable alias to [::2], i.e. filtering collection to have only odd elements
         """
         return self[::2]
 
     def sliced(
-        self, start: int = None, stop: int = None, step: int = 1
+        self,
+        start: Optional[int] = None,
+        stop: Optional[int] = None,
+        step: int = 1,
     ) -> Collection:
-        def find() -> List[WebElement]:
+        def find() -> typing.Sequence[WebElement]:
             webelements = self()
 
-            # todo: assert length according to provided start, stop...
+            # TODO: assert length according to provided start, stop...
 
             return webelements[start:stop:step]
 
         return Collection(
             Locator(
                 f'{self}[{start or ""}'
                 f':{stop or ""}'
@@ -682,114 +724,132 @@
             return self.sliced(
                 index_or_slice.start, index_or_slice.stop, index_or_slice.step
             )
 
         return self.element(index_or_slice)
 
     def from_(self, start: int) -> Collection:
-        return self[start:]
+        return typing.cast(Collection, self[start:])
 
     def to(self, stop: int) -> Collection:
-        return self[:stop]
+        return typing.cast(Collection, self[:stop])
 
     def by(
-        self, condition: Union[Condition[Element], Callable[[E], None]]
+        self, condition: Union[Condition[Element], Callable[[Element], None]]
     ) -> Collection:
         condition = (
             condition
             if isinstance(condition, Condition)
             else Condition(str(condition), condition)
         )
 
         return Collection(
             Locator(
                 f'{self}.filtered_by({condition})',
                 lambda: [
-                    element()
-                    for element in self.cached
-                    if element.matching(condition)
+                    element() for element in self.cached if element.matching(condition)
                 ],
             ),
             self.config,
         )
 
     def filtered_by(
-        self, condition: Union[Condition[Element], Callable[[E], None]]
+        self, condition: Union[Condition[Element], Callable[[Element], None]]
     ) -> Collection:
+        warnings.warn(
+            'collection.filtered_by(condition) is deprecated in favor of collection.by(condition)',
+            DeprecationWarning,
+        )
         return self.by(condition)
 
-    def filtered_by_their(
+    def by_their(
         self,
-        selector_or_callable: Union[str, tuple, Callable[[Element], Element]],
+        selector: Union[str, Tuple[str, str], Callable[[Element], Element]],
         condition: Condition[Element],
     ) -> Collection:
         """
-        :param selector_or_callable:
-            - selector may be a str with css/xpath selector or tuple with by.* locator
-            - callable should be a function on element that returns element
-        :param condition: a condition to
-        :return: collection subset with inner/relative element matching condition
+        Returns elements from collection that have inner/relative element,
+        found by ``selector`` and matching ``condition``.
+
+        Is a shortcut for ``collection.by(lambda element: condition(element.element(selector))``.
+
+        Example (straightforward)
+        -------------------------
 
         GIVEN html elements somewhere in DOM::
             .result
                 .result-title
                 .result-url
                 .result-snippet
 
         THEN::
 
             browser.all('.result')\
-                .filtered_by_their('.result-title', have.text('Selene'))\
+                .by_their('.result-title', have.text('Selene'))\
                 .should(have.size(3))
 
-        ... is a shortcut for::
+        is similar to::
 
             browser.all('.result')\
-                .filtered_by_their(lambda it: have.text(text)(it.element('.result-title')))\
-                .should(have.size(3))
-
-        OR with PageObject:
-
-        THEN::
-
-            results.element_by_its(lambda it: Result(it).title, have.text(text))\
+                .by_their(lambda it: have.text(text)(it.element('.result-title')))\
                 .should(have.size(3))
 
-        Shortcut for::
+        Example (PageObject)
+        --------------------
 
-            results.element_by(lambda it: have.text(text)(Result(it).title))\
-                .should(have.size(3))
+        GIVEN html elements somewhere in DOM::
+            .result
+                .result-title
+                .result-url
+                .result-snippet
 
-        WHERE::
+        AND::
 
             results = browser.all('.result')
             class Result:
                 def __init__(self, element):
                     self.element = element
                     self.title = self.element.element('.result-title')
                     self.url = self.element.element('.result-url')
             # ...
+
+        THEN::
+
+            results.by_their(lambda it: Result(it).title, have.text(text))\
+                .should(have.size(3))
+
+        is similar to::
+
+            results.by_their(lambda it: have.text(text)(Result(it).title))\
+                .should(have.size(3))
         """
-        warnings.warn(
-            'filtered_by_their is experimental; might be renamed or removed in future',
-            FutureWarning,
-        )
 
-        def find_in(parent: Element):
-            if callable(selector_or_callable):
-                return selector_or_callable(parent)
+        def find_in(parent: Element) -> Element:
+            if callable(selector):
+                return selector(parent)
             else:
-                return parent.element(selector_or_callable)
+                return parent.element(selector)
 
-        return self.filtered_by(lambda it: condition(find_in(it)))
+        return self.by(lambda it: condition(find_in(it)))
 
     def element_by(
-        self, condition: Union[Condition[Element], Callable[[E], None]]
+        self, condition: Union[Condition[Element], Callable[[Element], None]]
     ) -> Element:
-        # todo: In the implementation below...
+        # TODO: a first_by(condition) alias would be shorter,
+        #  and more consistent with by(condition).first
+        #  but the phrase items.element_by(have.text('foo')) leads to a more
+        #  natural meaning that such element should be only one...
+        #  while items.first_by(have.text('foo')) gives a clue that
+        #  it's just one of many...
+        #  should we then make element_by fail
+        #  if the condition matches more than one element? (maybe we can control it via corresponding config option?)
+        #  yet we don't fail if browser.element(selector) or element.element(selector)
+        #  finds more than one element... o_O
+
+        # TODO: In the implementation below...
         #       We use condition in context of "matching", i.e. as a predicate...
         #       why then not accept Callable[[E], bool] also?
         #       (as you remember, Condition is Callable[[E], None] throwing Error)
         #       This will allow the following code be possible
         #           results.element_by(lambda it:
         #               Result(it).title.matching(have.text(text)))
         #       instead of:
@@ -818,344 +878,292 @@
                 if element.matching(condition):
                     return element()
 
             from selene.core import query
 
             if self.config.log_outer_html_on_failure:
                 """
-                todo: move it support.shared.config
+                TODO: move it support.shared.config
                 """
                 outer_htmls = [query.outer_html(element) for element in cached]
 
                 raise AssertionError(
                     f'\n\tCannot find element by condition «{condition}» '
                     f'\n\tAmong {self}'
                     f'\n\tActual webelements collection:'
                     f'\n\t{outer_htmls}'
-                )  # todo: isn't it better to print it all the time via hook, like for Element?
+                )  # TODO: isn't it better to print it all the time via hook, like for Element?
             else:
                 raise AssertionError(
                     f'\n\tCannot find element by condition «{condition}» '
                     f'\n\tAmong {self}'
                 )
 
-        return Element(
-            Locator(f'{self}.element_by({condition})', find), self.config
-        )
+        return Element(Locator(f'{self}.element_by({condition})', find), self.config)
 
     def element_by_its(
         self,
-        selector_or_callable: Union[str, tuple, Callable[[Element], Element]],
+        selector: Union[str, Tuple[str, str], Callable[[Element], Element]],
         condition: Condition[Element],
     ) -> Element:
         """
-        :param selector_or_callable:
-            - selector may be a str with css/xpath selector or tuple with by.* locator
-            - callable should be a function on element that returns element
-        :param condition: a condition to
-        :return: element from collection that has inner/relative element matching condition
+        Returns element from collection that has inner/relative element
+        found by ``selector`` and matching ``condition``.
+        Is a shortcut for ``collection.element_by(lambda its: condition(its.element(selector))``.
+
+        Example (straightforward)
+        -------------------------
 
         GIVEN html elements somewhere in DOM::
+
             .result
                 .result-title
                 .result-url
                 .result-snippet
 
         THEN::
 
             browser.all('.result')\
                 .element_by_its('.result-title', have.text(text))\
                 .element('.result-url').click()
 
         ... is a shortcut for::
 
             browser.all('.result')\
-                .element_by(lambda it: have.text(text)(it.element('.result-title')))\
+                .element_by(lambda its: have.text(text)(its.element('.result-title')))\
                 .element('.result-url').click()
 
-        OR with PageObject:
-
-        THEN::
-
-            Result(results.element_by_its(lambda it: Result(it).title, have.text(text)))\
-                .url.click()
+        Example (PageObject)
+        --------------------
 
-        Shortcut for::
+        GIVEN html elements somewhere in DOM::
 
-            Result(results.element_by(lambda it: have.text(text)(Result(it).title)))\
-                .url.click()
+            .result
+                .result-title
+                .result-url
+                .result-snippet
 
-        WHERE::
+        AND::
 
             results = browser.all('.result')
             class Result:
                 def __init__(self, element):
                     self.element = element
                     self.title = self.element.element('.result-title')
                     self.url = self.element.element('.result-url')
-            # ...
-        """
-        # todo: main questions to answer before removing warning:
-        #       - isn't it enough to allow Callable[[Element], bool] as condition?
-        #           browser.all('.result').element_by(
-        #               lambda it: it.element('.result-title').matching(have.text('browser tests in Python')))
-        #               .element('.result-url').click()
-        #       - how to improve error messages in case we pass lambda (not a fun with good name/str repr)?
-        #       - what about accepting collection condition? should we allow it?
-        warnings.warn(
-            'element_by_its is experimental; might be renamed or removed in future',
-            FutureWarning,
-        )
 
-        def find_in(parent: Element):
-            if callable(selector_or_callable):
-                return selector_or_callable(parent)
-            else:
-                return parent.element(selector_or_callable)
-
-        return self.element_by(lambda it: condition(find_in(it)))
+        THEN::
 
-    # todo: consider adding ss alias
-    def all(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
-        warnings.warn(
-            'might be renamed or deprecated in future; '
-            'all is actually a shortcut for collected(lambda element: element.all(selector)...'
-            'but we also have all_first and...'
-            'it is yet unclear what name would be best for all_first as addition to all... '
-            'all_first might confuse with all(...).first... I mean: '
-            'all_first(selector) is actually '
-            'collected(lambda e: e.element(selector)) '
-            'but it is not the same as '
-            'all(selector).first '
-            'that is collected(lambda e: e.all(selector)).first ... o_O ',
-            FutureWarning,
-        )
-        by = to_by(css_or_xpath_or_by)
+            Result(results.element_by_its(lambda it: Result(it).title, have.text(text)))\
+                .url.click()
 
-        # todo: consider implement it through calling self.collected
-        #       because actually the impl is self.collected(lambda element: element.all(selector))
+        is a shortcut for::
 
-        return Collection(
-            Locator(
-                f'{self}.all({by})',
-                lambda: flatten(
-                    [webelement.find_elements(*by) for webelement in self()]
-                ),
-            ),
-            self.config,
-        )
+            Result(results.element_by(lambda it: have.text(text)(Result(it).title)))\
+                .url.click()
+            # ...
+        """
 
-    # todo: consider adding s alias
-    def all_first(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
-        warnings.warn(
-            'might be renamed or deprecated in future; '
-            'it is yet unclear what name would be best... '
-            'all_first might confuse with all(...).first... I mean: '
-            'all_first(selector) is actually '
-            'collected(lambda e: e.element(selector)) '
-            'but it is not the same as '
-            'all(selector).first '
-            'that is collected(lambda e: e.all(selector)).first ... o_O ',
-            FutureWarning,
-        )
-        by = to_by(css_or_xpath_or_by)
+        # TODO: tune implementation to ensure error messages are ok
 
-        # todo: consider implement it through calling self.collected
-        #       because actually the impl is self.collected(lambda element: element.element(selector))
+        def find_in(parent: Element):
+            if callable(selector):
+                return selector(parent)
+            else:
+                return parent.element(selector)
 
-        return Collection(
-            Locator(
-                f'{self}.all_first({by})',
-                lambda: [
-                    webelement.find_element(*by) for webelement in self()
-                ],
-            ),
-            self.config,
-        )
+        return self.element_by(lambda it: condition(find_in(it)))
 
     def collected(
         self, finder: Callable[[Element], Union[Element, Collection]]
     ) -> Collection:
-        # todo: consider adding predefined queries to be able to write
+        # TODO: consider adding predefined queries to be able to write
         #         collected(query.element(selector))
         #       over
         #         collected(lambda element: element.element(selector))
         #       and
         #         collected(query.all(selector))
         #       over
         #         collected(lambda element: element.all(selector))
         #       consider also putting such element builders like to find.* module instead of query.* module
         #       because they are not supposed to be used in entity.get(*) context defined for other query.* fns
 
         return Collection(
             Locator(
                 f'{self}.collected({finder})',
-                # todo: consider skipping None while flattening
-                lambda: flatten(
-                    [finder(element)() for element in self.cached]
+                # TODO: consider skipping None while flattening
+                lambda: typing.cast(
+                    typing.Sequence[WebElement],
+                    flatten([finder(element)() for element in self.cached]),
                 ),
             ),
             self.config,
         )
 
-    # --- Assertable --- #
+    def all(self, selector: Union[str, Tuple[str, str]]) -> Collection:
+        """
+        Returns a collection of all elements found be selector inside each element of self
 
-    def should(
-        self,
-        condition: Union[Condition[Collection], Condition[Element]],
-    ) -> Collection:
-        if isinstance(condition, ElementCondition):
-            # todo: consider deprecating... makes everything too complicated...
-            for element in self:
-                element.should(condition)
-        else:
-            super().should(condition)
-        return self
+        An alias to ``collection.collected(lambda its: its.all(selector))``.
 
-    # --- Deprecated --- #
+        Example
+        -------
 
-    def get_actual_webelements(self) -> List[WebElement]:
-        warnings.warn(
-            "considering to be deprecated; use collection as callable instead, like: browser.all('.foo')()",
-            PendingDeprecationWarning,
-        )
-        return self()
+        Given html::
 
-    def caching(self) -> Collection:
-        warnings.warn(
-            "deprecated; use `cached` property instead: browser.all('#foo').cached",
-            DeprecationWarning,
-        )
-        return self.cached
+            <table>
+              <tr class="row">
+                <td class="cell">A1</td><td class="cell">A2</td>
+              </tr>
+              <tr class="row">
+                <td class="cell">B1</td><td class="cell">B2</td>
+              </tr>
+            </table>
 
-    def all_by(self, condition: Condition[Element]) -> Collection:
-        warnings.warn(
-            "deprecated; use `filtered_by` instead: browser.all('.foo').filtered_by(be.enabled)",
-            DeprecationWarning,
-        )
-        return self.filtered_by(condition)
+        Then::
 
-    def filter_by(self, condition: Condition[Element]) -> Collection:
-        warnings.warn(
-            "deprecated; use `filtered_by` instead: browser.all('.foo').filtered_by(be.enabled)",
-            DeprecationWarning,
-        )
-        return self.filtered_by(condition)
+            browser.all('.row').all('.cell')).should(have.texts('A1', 'A2', 'B1', 'B2'))
+        """
+        by = to_by(selector)
 
-    def find_by(self, condition: Condition[Element]) -> Element:
-        warnings.warn(
-            "deprecated; use `element_by` instead: browser.all('.foo').element_by(be.enabled)",
-            DeprecationWarning,
+        # TODO: consider implement it through calling self.collected
+        #       because actually the impl is self.collected(lambda element: element.all(selector))
+
+        return Collection(
+            Locator(
+                f'{self}.all({by})',
+                lambda: typing.cast(
+                    typing.Sequence[WebElement],
+                    flatten([webelement.find_elements(*by) for webelement in self()]),
+                ),
+            ),
+            self.config,
         )
-        return self.element_by(condition)
 
-    def size(self):
-        warnings.warn(
-            "deprecated; use `len` standard function instead: len(browser.all('.foo'))",
-            DeprecationWarning,
+    def all_first(self, selector: Union[str, Tuple[str, str]]) -> Collection:
+        """
+        Returns a collection of each first element found be selector inside each element of self
+
+        An alias to ``collection.collected(lambda its: its.element(selector))``.
+        Not same as ``collection.all(selector).first`` that is same as ``collection.first.element(selector)``
+
+        Example
+        -------
+
+        Given html::
+
+            <table>
+              <tr class="row">
+                <td class="cell">A1</td><td class="cell">A2</td>
+              </tr>
+              <tr class="row">
+                <td class="cell">B1</td><td class="cell">B2</td>
+              </tr>
+            </table>
+
+        Then::
+
+            browser.all('.row').all_first('.cell')).should(have.texts('A1', 'B1'))
+        """
+        by = to_by(selector)
+
+        # TODO: consider implement it through calling self.collected
+        #       because actually the impl is self.collected(lambda element: element.element(selector))
+
+        return Collection(
+            Locator(
+                f'{self}.all_first({by})',
+                lambda: [webelement.find_element(*by) for webelement in self()],
+            ),
+            self.config,
         )
-        return len(self)
 
-    def should_each(self, condition: ElementCondition) -> Collection:
-        # warnings.warn(
-        #     "deprecated; use `should` method instead: browser.all('.foo').should(have.css_class('bar'))",
-        #     DeprecationWarning,
-        # )
-        # """
-        # was deprecated
-        # but... probably making .should(condition) too smart was a bad idea...
-        # TODO: decide on the the .should_each fate...
-        # """
-        return self.should(condition)
-
-
-class SeleneCollection(Collection):
-    warnings.warn(
-        'SeleneCollection is deprecated, import Element class instead for  your needs'
-    )
-    pass
-
-
-class Browser(WaitingEntity):
-    def __init__(
-        self, config: Config
-    ):  # todo: what about adding **config_as_kwargs?
+
+class Browser(WaitingEntity['Browser']):
+    def __init__(self, config: Optional[Config] = None):
+        config = Config() if config is None else config
         super().__init__(config)
 
-    # todo: consider implement it as context manager too...
-    def with_(self, config: Config = None, **config_as_kwargs) -> Browser:
-        return Browser(self.config.with_(config, **config_as_kwargs))
+    def with_(self, config: Optional[Config] = None, **config_as_kwargs) -> Browser:
+        return (
+            Browser(config)
+            if config
+            else Browser(self.config.with_(**config_as_kwargs))
+        )
 
     def __str__(self):
         return 'browser'
 
-    # todo: consider making it callable ...
-
     @property
     def driver(self) -> WebDriver:
         return self.config.driver
 
+    # TODO: consider making it callable (self.__call__() to be shortcut to self.__raw__ ...)
+
+    @property
+    def __raw__(self):
+        return self.config.driver
+
     # @property
     # def actions(self) -> ActionChains:
     #     """
     #     It's kind of just a shortcut for pretty low level actions from selenium webdriver
     #     Yet unsure about this property here:)
     #     comparing to usual high level Selene API...
     #     Maybe later it would be better to make own Actions with selene-style retries, etc.
     #     """
     #     return ActionChains(self.config.driver)
 
     # --- Element builders --- #
 
-    def element(self, css_or_xpath_or_by: Union[str, tuple]) -> Element:
+    # TODO: consider None by default,
+    #       and *args, **kwargs to be able to pass custom things
+    #       to be processed by config.location_strategy
+    #       and by default process none as "element to skip all actions on it"
+    def element(
+        self, css_or_xpath_or_by: Union[str, Tuple[str, str], Locator]
+    ) -> Element:
+        if isinstance(css_or_xpath_or_by, Locator):
+            return Element(css_or_xpath_or_by, self.config)
+
         by = to_by(css_or_xpath_or_by)
 
         return Element(
-            Locator(
-                f'{self}.element({by})', lambda: self.driver.find_element(*by)
-            ),
+            Locator(f'{self}.element({by})', lambda: self.driver.find_element(*by)),
             self.config,
         )
 
-    def all(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
+    def all(
+        self, css_or_xpath_or_by: Union[str, Tuple[str, str], Locator]
+    ) -> Collection:
+        if isinstance(css_or_xpath_or_by, Locator):
+            return Collection(css_or_xpath_or_by, self.config)
+
         by = to_by(css_or_xpath_or_by)
 
         return Collection(
-            Locator(
-                f'{self}.all({by})', lambda: self.driver.find_elements(*by)
-            ),
+            Locator(f'{self}.all({by})', lambda: self.driver.find_elements(*by)),
             self.config,
         )
 
     # --- High Level Commands--- #
 
-    def open(self, relative_or_absolute_url: str) -> Browser:
-        width = self.config.window_width
-        height = self.config.window_height
-
-        if width and height:
-            self.driver.set_window_size(int(width), int(height))
-
-        is_absolute = is_absolute_url(relative_or_absolute_url)
-        base_url = self.config.base_url
-        url = (
-            relative_or_absolute_url
-            if is_absolute
-            else base_url + relative_or_absolute_url
-        )
+    def open(self, relative_or_absolute_url: Optional[str] = None) -> Browser:
+        # TODO: should we keep it less pretty but more KISS? like:
+        # self.config._driver_get_url_strategy(self.config)(relative_or_absolute_url)
+        self.config._executor.get_url(relative_or_absolute_url)
 
-        self.driver.get(url)
         return self
 
     def switch_to_next_tab(self) -> Browser:
         from selene.core import query
 
         self.driver.switch_to.window(query.next_tab(self))
 
-        # todo: should we user waiting version here (and in other similar cases)?
+        # TODO: should we use waiting version here (and in other similar cases)?
         # self.perform(Command(
         #     'open next tab',
         #     lambda browser: browser.driver.switch_to.window(query.next_tab(self))))
 
         return self
 
     def switch_to_previous_tab(self) -> Browser:
@@ -1171,94 +1179,123 @@
 
             self.driver.switch_to.window(query.tab(index)(self))
         else:
             self.driver.switch_to.window(index_or_name)
 
         return self
 
+    # TODO: consider deprecating
     @property
     def switch_to(self) -> SwitchTo:
         return self.driver.switch_to
 
-    # todo: should we add also a shortcut for self.driver.switch_to.alert ?
+    # TODO: should we add also a shortcut for self.driver.switch_to.alert ?
     #       if we don't need to switch_to.'back' after switch to alert - then for sure we should...
     #       question is - should we implement our own alert as waiting entity?
 
-    def close_current_tab(self) -> Browser:
-        self.driver.close()
-        return self
-
     def quit(self) -> None:
-        self.driver.quit()
-
-    def clear_local_storage(self) -> Browser:
-        self.driver.execute_script(
-            'window.localStorage.clear();'
-        )  # todo: should we catch and ignore errors?
-        return self
+        """
+        Quits the driver.
 
-    def clear_session_storage(self) -> Browser:
-        self.driver.execute_script('window.sessionStorage.clear();')
-        return self
+        If the driver was not even set, will build it just to quit it:D.
 
-    # --- Assertable --- #
+        Will fail if the driver was already quit or crashed.
+        """
+        self.driver.quit()
 
-    # we need this method here in order to make autocompletion work...
-    # unfortunately the "base class" version is not enough
-    def should(self, condition: BrowserCondition) -> Browser:
-        super().should(condition)
+    # TODO: consider deprecating, it does not close browser, it closes current tab/window
+    def close(self) -> Browser:
+        self.driver.close()
         return self
 
     # --- Deprecated --- #
 
-    def close(self) -> Browser:
+    # TODO: should we keep it?
+    def execute_script(self, script, *args):
         warnings.warn(
-            "deprecated; use a `close_current_tab` method instead",
+            'consider using browser.driver.execute_script '
+            'instead of browser.execute_script',
+            PendingDeprecationWarning,
+        )
+        return self.driver.execute_script(script, *args)
+
+    # TODO: should we move it to query.* and/or command.*?
+    #       like `browser.get(query.screenshot)` ?
+    #       like `browser.perform(command.save_screenshot)` ?
+    # TODO: deprecate file name, use path
+    #       because we can path folder path not file path and it will work
+    def save_screenshot(self, file: Optional[str] = None):
+        warnings.warn(
+            'browser.save_screenshot is deprecated, '
+            'use browser.get(query.screenshot_saved())',
             DeprecationWarning,
         )
 
-        return self.close_current_tab()
+        from selene.core import query  # type: ignore
+
+        return self.get(query.screenshot_saved())  # type: ignore
 
-    def s(self, css_or_xpath_or_by: Union[str, tuple]) -> Element:
+    @property
+    def last_screenshot(self) -> str:
         warnings.warn(
-            "deprecated; use an `element` method instead: "
-            "`browser.element('#foo')`",
+            'browser.last_screenshot is deprecated, '
+            'use browser.config.last_screenshot',
             DeprecationWarning,
         )
+        return self.config.last_screenshot  # type: ignore
 
-        return self.element(css_or_xpath_or_by)
+    # TODO: consider moving this to browser command.save_page_source(filename)
+    def save_page_source(self, file: Optional[str] = None) -> Optional[str]:
+        warnings.warn(
+            'browser.save_page_source is deprecated, '
+            'use browser.config.last_screenshot',
+            DeprecationWarning,
+        )
+
+        if file is None:
+            file = self.config._generate_filename(suffix='.html')  # type: ignore
 
-    def ss(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
+        saved_file = WebHelper(self.driver).save_page_source(file)
+
+        self.config.last_page_source = saved_file  # type: ignore
+
+        return saved_file
+
+    @property
+    def last_page_source(self) -> str:
         warnings.warn(
-            "deprecated; use an `all` method instead: "
-            "`browser.all('.foo')`",
+            'browser.last_page_source is deprecated, '
+            'use browser.config.last_page_source',
             DeprecationWarning,
         )
+        return self.config.last_page_source  # type: ignore
 
-        return self.all(css_or_xpath_or_by)
+    def close_current_tab(self) -> Browser:
+        warnings.warn(
+            'deprecated because the «tab» term is not relevant for mobile; '
+            'use a `browser.close()` or `browser.driver.close()` instead',
+            DeprecationWarning,
+        )
+        self.driver.close()
+        return self
 
-    def elements(self, css_or_xpath_or_by: Union[str, tuple]) -> Collection:
+    def clear_local_storage(self) -> Browser:
         warnings.warn(
-            "deprecated; use an `all` method instead: "
-            "`browser.all('.foo')`",
+            'deprecated because of js nature and not-relevance for mobile; '
+            'use `browser.perform(command.js.clear_local_storage)` instead',
             DeprecationWarning,
         )
+        from selene.core import command
 
-        return self.all(css_or_xpath_or_by)
+        self.perform(command.js.clear_local_storage)
+        return self
 
+    def clear_session_storage(self) -> Browser:
+        warnings.warn(
+            'deprecated because of js nature and not-relevance for mobile; '
+            'use `browser.perform(command.js.clear_session_storage)` instead',
+            DeprecationWarning,
+        )
+        from selene.core import command
 
-# TODO: probably this was needed for migration from 1.0 to 2.0...
-from selene.core.conditions import (
-    CollectionCondition,
-    ElementCondition,
-    BrowserCondition,
-)
-
-
-# --- Deprecated --- #  todo: remove in future versions
-
-
-class SeleneDriver(Browser):
-    warnings.warn(
-        'SeleneDriver is deprecated, import Browser class instead for  your needs'
-    )
-    pass
+        self.perform(command.js.clear_session_storage)
+        return self
```

### Comparing `selene-2.0.0b9/selene/core/exceptions.py` & `selene-2.0.0rc1/selene/core/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,31 +27,31 @@
         self.msg = msg
 
     def __str__(self):
         exception_msg = "Message: %s\n" % self.msg
         return exception_msg
 
 
-# todo: should we extend it from SeleneError and make lazy in same way?
+# TODO: should we extend it from SeleneError and make lazy in same way?
 class ConditionNotMatchedError(AssertionError):
     def __init__(self, message='condition not matched'):
         super().__init__(message)
 
 
-# todo: should we name it *Error or *Exception?
+# TODO: should we name it *Error or *Exception?
 #       (see
 #        https://www.python.org/dev/peps/pep-0008/#exception-names
 #        https://www.datacamp.com/community/tutorials/exception-handling-python
 #       )
 #       should we name it simply Error and allow to import as selene.Error ?
 #       should we name it SeleneError and still allow to import as selene.Error?
 class _SeleneError(AssertionError):
     def __init__(self, message: Union[str, Callable[[], str]]):
-        self._render_message: Callable[[], str] = (
-            (lambda: message) if isinstance(message, str) else message
+        self._render_message: Callable[[], str] = lambda: (
+            message() if callable(message) else message
         )
 
     @property
     def args(self):
         return (self._render_message(),)
 
     def __str__(self):
```

### Comparing `selene-2.0.0b9/selene/core/locator.py` & `selene-2.0.0rc1/selene/core/locator.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0b9/selene/core/match.py` & `selene-2.0.0rc1/selene/core/match.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,60 +16,54 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import warnings
-from typing import List, Any
+from typing import List, Any, Union, Iterable
 
-from selene.common import predicate
+from selene.common import predicate, helpers
 from selene.core import query
 from selene.core.condition import Condition
 from selene.core.conditions import (
     ElementCondition,
     CollectionCondition,
     BrowserCondition,
 )
 from selene.core.entity import Collection, Element, Browser
 
-# todo: consider moving to selene.match.element.is_visible, etc...
+# TODO: consider moving to selene.match.element.is_visible, etc...
 element_is_visible: Condition[Element] = ElementCondition.raise_if_not(
     'is visible', lambda element: element().is_displayed()
 )
 
 element_is_hidden: Condition[Element] = ElementCondition.as_not(
     element_is_visible, 'is hidden'
 )
 
 element_is_enabled: Condition[Element] = ElementCondition.raise_if_not(
     'is enabled', lambda element: element().is_enabled()
 )
 
-element_is_disabled: Condition[Element] = ElementCondition.as_not(
-    element_is_enabled
-)
+element_is_disabled: Condition[Element] = ElementCondition.as_not(element_is_enabled)
 
-element_is_clickable: Condition[Element] = element_is_visible.and_(
-    element_is_enabled
-)
+element_is_clickable: Condition[Element] = element_is_visible.and_(element_is_enabled)
 
 element_is_present: Condition[Element] = ElementCondition.raise_if_not(
     'is present in DOM', lambda element: element() is not None
 )
 
-element_is_absent: Condition[Element] = ElementCondition.as_not(
-    element_is_present
-)
+element_is_absent: Condition[Element] = ElementCondition.as_not(element_is_present)
 
+# TODO: how will it work for mobile?
 element_is_focused: Condition[Element] = ElementCondition.raise_if_not(
     'is focused',
-    # todo: change in the following line to element.execute_script or element.config.driver.execute_script
     lambda element: element()
-    == element._webdriver.execute_script('return document.activeElement'),
+    == element.config.driver.execute_script('return document.activeElement'),
 )
 
 
 def element_has_text(
     expected: str,
     describing_matched_to='has text',
     compared_by_predicate_to=predicate.includes,
@@ -82,15 +76,15 @@
 
 
 def element_has_exact_text(expected: str) -> Condition[Element]:
     return element_has_text(expected, 'has exact text', predicate.equals)
 
 
 def element_has_js_property(name: str):
-    # todo: should we keep simpler but less obvious name - *_has_property ?
+    # TODO: should we keep simpler but less obvious name - *_has_property ?
     def property_value(element: Element) -> str:
         return element().get_property(name)
 
     def property_values(collection: Collection) -> List[str]:
         return [element.get_property(name) for element in collection()]
 
     raw_property_condition = ElementCondition.raise_if_not_actual(
@@ -108,41 +102,43 @@
         def value_containing(self, expected: str) -> Condition[Element]:
             return ElementCondition.raise_if_not_actual(
                 f"has js property '{name}' with value containing '{expected}'",
                 property_value,
                 predicate.includes(expected),
             )
 
-        def values(self, *expected: str) -> Condition[Collection]:
+        def values(self, *expected: Union[str, Iterable[str]]) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has js property '{name}' with values '{expected}'",
+                f"has js property '{name}' with values '{expected_}'",
                 property_values,
-                predicate.equals_to_list(expected),
+                predicate.equals_to_list(expected_),
             )
 
-        def values_containing(self, *expected: str) -> Condition[Collection]:
+        def values_containing(
+            self, *expected: Union[str, Iterable[str]]
+        ) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has js property '{name}' with values containing '{expected}'",
+                f"has js property '{name}' with values containing '{expected_}'",
                 property_values,
-                predicate.equals_by_contains_to_list(expected),
+                predicate.equals_by_contains_to_list(expected_),
             )
 
-    return ConditionWithValues(
-        str(raw_property_condition), raw_property_condition.call
-    )
+    return ConditionWithValues(str(raw_property_condition), raw_property_condition.call)
 
 
 def element_has_css_property(name: str):
     def property_value(element: Element) -> str:
         return element().value_of_css_property(name)
 
     def property_values(collection: Collection) -> List[str]:
-        return [
-            element.value_of_css_property(name) for element in collection()
-        ]
+        return [element.value_of_css_property(name) for element in collection()]
 
     raw_property_condition = ElementCondition.raise_if_not_actual(
         'has css property ' + name, property_value, predicate.is_truthy
     )
 
     class ConditionWithValues(ElementCondition):
         def value(self, expected: str) -> Condition[Element]:
@@ -155,48 +151,51 @@
         def value_containing(self, expected: str) -> Condition[Element]:
             return ElementCondition.raise_if_not_actual(
                 f"has css property '{name}' with value containing '{expected}'",
                 property_value,
                 predicate.includes(expected),
             )
 
-        def values(self, *expected: str) -> Condition[Collection]:
+        def values(self, *expected: Union[str, Iterable[str]]) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has css property '{name}' with values '{expected}'",
+                f"has css property '{name}' with values '{expected_}'",
                 property_values,
-                predicate.equals_to_list(expected),
+                predicate.equals_to_list(expected_),
             )
 
-        def values_containing(self, *expected: str) -> Condition[Collection]:
+        def values_containing(
+            self, *expected: Union[str, Iterable[str]]
+        ) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has css property '{name}' with values containing '{expected}'",
+                f"has css property '{name}' with values containing '{expected_}'",
                 property_values,
-                predicate.equals_by_contains_to_list(expected),
+                predicate.equals_by_contains_to_list(expected_),
             )
 
-    return ConditionWithValues(
-        str(raw_property_condition), raw_property_condition.call
-    )
+    return ConditionWithValues(str(raw_property_condition), raw_property_condition.call)
 
 
 def element_has_attribute(name: str):
     def attribute_value(element: Element) -> str:
         return element().get_attribute(name)
 
     def attribute_values(collection: Collection) -> List[str]:
         return [element.get_attribute(name) for element in collection()]
 
     raw_attribute_condition = ElementCondition.raise_if_not_actual(
         'has attribute ' + name, attribute_value, predicate.is_truthy
     )
 
+    # TODO: is it OK to have some collection conditions inside a thing named element_has_attribute ? o_O
     class ConditionWithValues(ElementCondition):
-        def value(
-            self, expected: str, ignore_case=False
-        ) -> Condition[Element]:
+        def value(self, expected: str, ignore_case=False) -> Condition[Element]:
             if ignore_case:
                 warnings.warn(
                     'ignore_case syntax is experimental and might change in future',
                     FutureWarning,
                 )
             return ElementCondition.raise_if_not_actual(
                 f"has attribute '{name}' with value '{expected}'",
@@ -214,46 +213,62 @@
                 )
             return ElementCondition.raise_if_not_actual(
                 f"has attribute '{name}' with value containing '{expected}'",
                 attribute_value,
                 predicate.includes(expected, ignore_case),
             )
 
-        def values(self, *expected: str) -> Condition[Collection]:
+        def values(self, *expected: Union[str, Iterable[str]]) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has attribute '{name}' with values '{expected}'",
+                f"has attribute '{name}' with values '{expected_}'",
                 attribute_values,
-                predicate.equals_to_list(expected),
+                predicate.equals_to_list(expected_),
             )
 
-        def values_containing(self, *expected: str) -> Condition[Collection]:
+        def values_containing(
+            self, *expected: Union[str, Iterable[str]]
+        ) -> Condition[Collection]:
+            expected_ = helpers.flatten(expected)
+
             return CollectionCondition.raise_if_not_actual(
-                f"has attribute '{name}' with values containing '{expected}'",
+                f"has attribute '{name}' with values containing '{expected_}'",
                 attribute_values,
-                predicate.equals_by_contains_to_list(expected),
+                predicate.equals_by_contains_to_list(expected_),
             )
 
     return ConditionWithValues(
         str(raw_attribute_condition), raw_attribute_condition.call
     )
 
 
-element_is_selected: Condition[Element] = element_has_attribute(
-    'elementIsSelected'
-)
+element_is_selected: Condition[Element] = element_has_attribute('elementIsSelected')
 
 
 def element_has_value(expected: str) -> Condition[Element]:
     return element_has_attribute('value').value(expected)
 
 
 def element_has_value_containing(expected: str) -> Condition[Element]:
     return element_has_attribute('value').value_containing(expected)
 
 
+def collection_has_values(
+    *expected: Union[str, Iterable[str]]
+) -> Condition[Collection]:
+    return element_has_attribute('value').values(*expected)
+
+
+def collection_has_values_containing(
+    *expected: Union[str, Iterable[str]]
+) -> Condition[Collection]:
+    return element_has_attribute('value').values_containing(*expected)
+
+
 def element_has_css_class(expected: str) -> Condition[Element]:
     def class_attribute_value(element: Element) -> str:
         return element().get_attribute('class')
 
     return ElementCondition.raise_if_not_actual(
         f"has css class '{expected}'",
         class_attribute_value,
@@ -278,14 +293,17 @@
     )
 
 
 def element_has_tag_containing(expected: str) -> Condition[Element]:
     return element_has_tag(expected, 'has tag containing', predicate.includes)
 
 
+# TODO: should not we make empty to work on both elements and collections?
+#   to assert have.size(0) on collections
+#   to assert have.value('').and(have.exact_text('')) on element
 def _is_collection_empty(collection: Collection) -> bool:
     warnings.warn(
         'match.collection_is_empty or be.empty is deprecated; '
         'use more explicit and obvious have.size(0) instead',
         DeprecationWarning,
     )
     return len(collection()) == 0
@@ -324,62 +342,62 @@
         expected,
         'has size greater than or equal',
         predicate.is_greater_than_or_equal,
     )
 
 
 def collection_has_size_less_than(expected: int) -> Condition[Collection]:
-    return collection_has_size(
-        expected, 'has size less than', predicate.is_less_than
-    )
+    return collection_has_size(expected, 'has size less than', predicate.is_less_than)
 
 
 def collection_has_size_less_than_or_equal(
     expected: int,
 ) -> Condition[Collection]:
     return collection_has_size(
         expected,
         'has size less than or equal',
         predicate.is_less_than_or_equal,
     )
 
 
-# todo: make it configurable whether assert only visible texts or ot
-def collection_has_texts(*expected: str) -> Condition[Collection]:
+# TODO: make it configurable whether assert only visible texts or ot
+def collection_has_texts(*expected: Union[str, Iterable[str]]) -> Condition[Collection]:
+    expected_ = helpers.flatten(expected)
+
     def visible_texts(collection: Collection) -> List[str]:
         return [
-            webelement.text
-            for webelement in collection()
-            if webelement.is_displayed()
+            webelement.text for webelement in collection() if webelement.is_displayed()
         ]
 
     return CollectionCondition.raise_if_not_actual(
-        f'has texts {expected}',
+        f'has texts {expected_}',
         visible_texts,
-        predicate.equals_by_contains_to_list(expected),
+        predicate.equals_by_contains_to_list(expected_),
     )
 
 
-def collection_has_exact_texts(*expected: str) -> Condition[Collection]:
+def collection_has_exact_texts(
+    *expected: Union[str, Iterable[str]]
+) -> Condition[Collection]:
+    expected_ = helpers.flatten(expected)
+
     def visible_texts(collection: Collection) -> List[str]:
         return [
-            webelement.text
-            for webelement in collection()
-            if webelement.is_displayed()
+            webelement.text for webelement in collection() if webelement.is_displayed()
         ]
 
     return CollectionCondition.raise_if_not_actual(
-        f'has exact texts {expected}',
+        f'has exact texts {expected_}',
         visible_texts,
-        predicate.equals_to_list(expected),
+        predicate.equals_to_list(expected_),
     )
 
 
-# todo: consider refactoring the code like below by moving outside fns like url, title, etc...
-# todo: probably we will do that nevertheless when reusing "commands&queries" inside element class definitions
+# TODO: consider refactoring the code like below by moving outside fns like url, title, etc...
+# TODO: probably we will do that nevertheless when reusing "commands&queries" inside element class definitions
 def browser_has_url(
     expected: str,
     describing_matched_to='has url',
     compared_by_predicate_to=predicate.equals,
 ) -> Condition[Browser]:
     def url(browser: Browser) -> str:
         return browser.driver.current_url
@@ -407,17 +425,15 @@
         f"{describing_matched_to} '{expected}'",
         title,
         compared_by_predicate_to(expected),
     )
 
 
 def browser_has_title_containing(expected: str) -> Condition[Browser]:
-    return browser_has_title(
-        expected, 'has title containing', predicate.includes
-    )
+    return browser_has_title(expected, 'has title containing', predicate.includes)
 
 
 def browser_has_tabs_number(
     expected: int,
     describing_matched_to='has tabs number',
     compared_by_predicate_to=predicate.equals,
 ) -> Condition[Browser]:
@@ -459,15 +475,25 @@
     return browser_has_tabs_number(
         expected,
         'has tabs number less than or equal',
         predicate.is_less_than_or_equal,
     )
 
 
-def browser_has_js_returned(
+def browser_has_js_returned(expected: Any, script: str, *args) -> Condition[Browser]:
+    warnings.warn(
+        'deprecated because js does not work for mobile; '
+        'use have.script_returned(True, ...) instead',
+        DeprecationWarning,
+    )
+
+    return browser_has_script_returned(expected, script, *args)
+
+
+def browser_has_script_returned(
     expected: Any, script: str, *args
 ) -> Condition[Browser]:
     def script_result(browser: Browser):
         return browser.driver.execute_script(script, *args)
 
     return BrowserCondition.raise_if_not_actual(
         f'has the ```{script}``` script returned {expected}',
```

### Comparing `selene-2.0.0b9/selene/core/query.py` & `selene-2.0.0rc1/selene/core/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import typing
 from typing import List, Dict, Any, Union
 
+from selenium.webdriver.remote.webelement import WebElement
+
 from selene.core.entity import Browser, Element, Collection
 from selene.core.wait import Query
 
 
 def attribute(name: str) -> Query[Element, str]:
     def fn(element: Element) -> str:
         return element().get_attribute(name)
@@ -34,99 +37,104 @@
 
 inner_html = attribute('innerHTML')
 
 
 outer_html = attribute('outerHTML')
 
 
+text_content = attribute('textContent')
+"""
+full text of element without space normalization
+"""
+
+
 value = attribute('value')
 
-tag: Query[Element, str] = Query(
-    'tag name', lambda element: element().tag_name
-)
+tag: Query[Element, str] = Query('tag name', lambda element: element().tag_name)
 
 text: Query[Element, str] = Query('text', lambda element: element().text)
+"""
+normalized text of element
+"""
 
-# todo: do we need condition for the following?
+# TODO: do we need condition for the following?
 location_once_scrolled_into_view: Query[Element, Dict[str, int]] = Query(
     'location once scrolled into view',
     lambda element: element().location_once_scrolled_into_view,
 )
 
-# todo: what to do now with have.size* ? o_O
-size: Union[Query[Element, Dict[str, Any]], Query[Collection, int]] = Query(
+# TODO: what to do now with have.size* ? o_O
+size: Query[Union[Element, Collection, Browser], Union[dict, int]] = Query(
     'size',
-    lambda entity: entity().size
-    if isinstance(entity, Element)
-    else len(entity()),
+    lambda entity: (
+        entity().size
+        if isinstance(entity, Element)
+        else len(entity())
+        if isinstance(entity, Collection)
+        else typing.cast(Browser, entity).driver.get_window_size()
+    ),
 )
 
-# todo: do we need condition for the following?
+# TODO: do we need condition for the following?
 location: Query[Element, Dict[str, int]] = Query(
     'location', lambda element: element().location
 )
 
-# todo: do we need condition for the following?
-rect: Query[Element, Dict[str, Any]] = Query(
-    'rect', lambda element: element().rect
-)
+# TODO: do we need condition for the following?
+rect: Query[Element, Dict[str, Any]] = Query('rect', lambda element: element().rect)
 
 screenshot_as_base64: Query[Element, Any] = Query(
     'screenshot as base64', lambda element: element().screenshot_as_base64
 )
 
 screenshot_as_png: Query[Element, Any] = Query(
     'screenshot as png', lambda element: element().screenshot_as_png
 )
 
 
 def screenshot(filename: str) -> Query[Element, bool]:
-    def fn(element: Element) -> str:
+    def func(element: Element) -> bool:
         return element().screenshot(filename)
 
-    return Query(f'screenshot {filename}', fn)
+    return Query(f'screenshot {filename}', func)
 
 
 # not needed, because interfere with "parent element" meaning and usually can be workaround via element.config.driver
 # parent: Query[Element, Any] = \
 #     Query('parent', lambda element: element().parent)
-# todo: but should we add it with another name?
+# TODO: but should we add it with another name?
 
 
-internal_id: Query[Element, Any] = Query(
-    'internal id', lambda element: element().id
-)
+internal_id: Query[Element, Any] = Query('internal id', lambda element: element().id)
 
 
 def css_property(name: str) -> Query[Element, str]:
     def fn(element: Element) -> str:
         return element().value_of_css_property(name)
 
     return Query(f'css property {name}', fn)
 
 
-def js_property(name: str) -> Query[Element, str]:
-    def fn(element: Element) -> str:
+def js_property(
+    name: str,
+) -> Query[Element, Union[str, bool, WebElement, dict]]:
+    def func(element: Element) -> Union[str, bool, WebElement, dict]:
         return element().get_property(name)
 
-    return Query(f'js property {name}', fn)
+    return Query(f'js property {name}', func)
 
 
 # --- Collection queries --- #
 
 # --- Browser queries --- #
 
 
-url: Query[Browser, str] = Query(
-    'url', lambda browser: browser.driver.current_url
-)
+url: Query[Browser, str] = Query('url', lambda browser: browser.driver.current_url)
 
-title: Query[Browser, str] = Query(
-    'title', lambda browser: browser.driver.title
-)
+title: Query[Browser, str] = Query('title', lambda browser: browser.driver.title)
 
 tabs: Query[Browser, List[str]] = Query(
     'tabs', lambda browser: browser.driver.window_handles
 )
 
 tabs_number: Query[Browser, int] = Query(
     'tabs number', lambda browser: len(browser.driver.window_handles)
@@ -146,17 +154,15 @@
 )
 
 
 def __next_tab_fn(browser: Browser) -> str:
     tabs = browser.driver.window_handles
     current = browser.driver.current_window_handle
     current_index = tabs.index(current)
-    return (
-        tabs[0] if current_index >= len(tabs) - 1 else tabs[current_index + 1]
-    )
+    return tabs[0] if current_index >= len(tabs) - 1 else tabs[current_index + 1]
 
 
 next_tab: Query[Browser, str] = Query('next tab', __next_tab_fn)
 
 
 def __previous_tab_fn(browser: Browser) -> str:
     tabs = browser.driver.window_handles
@@ -167,7 +173,43 @@
 
 previous_tab: Query[Browser, str] = Query('previous tab', __previous_tab_fn)
 
 
 page_source: Query[Browser, str] = Query(
     'page source', lambda browser: browser.driver.page_source
 )
+
+
+# TODO: consider changing entity.get signature to accept query builders,
+#       not jus query objects
+def screenshot_saved(
+    path: typing.Optional[str] = None,
+) -> Query[Browser, typing.Optional[str]]:
+    query: Query[Browser, typing.Optional[str]] = Query(
+        'save and get screenshot',
+        lambda browser: browser.config._save_screenshot_strategy(browser.config, path),
+    )
+
+    if isinstance(path, Browser):
+        # somebody passed query as `.get(query.save_screenshot)`
+        # not as `.get(query.save_screenshot())`
+        browser = path
+        return query.__call__(browser)  # type: ignore
+
+    return query
+
+
+def page_source_saved(
+    path: typing.Optional[str] = None,
+) -> Query[Browser, typing.Optional[str]]:
+    query: Query[Browser, typing.Optional[str]] = Query(
+        'save and get page source',
+        lambda browser: browser.config._save_page_source_strategy(browser.config, path),
+    )
+
+    if isinstance(path, Browser):
+        # somebody passed query as `.get(query.save_screenshot)`
+        # not as `.get(query.page_source_saved())`
+        browser = path
+        return query.__call__(browser)  # type: ignore
+
+    return query
```

### Comparing `selene-2.0.0b9/selene/core/wait.py` & `selene-2.0.0rc1/selene/core/wait.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,54 +35,53 @@
 T = TypeVar('T')
 R = TypeVar('R')
 E = TypeVar('E')
 '''
 A generic TypeVar to identify an Entity Type, i.e. something to wait on
 '''
 
-# todo: not sure, if we need all these Lambda, Proc, Query, Command in python
-# todo: they was added just to quickly port selenidejs waiting mechanism
-# todo: let's consider removing them... or moving them e.g. to fp
+# TODO: not sure, if we need all these Lambda, Proc, Query, Command in python
+# TODO: they was added just to quickly port selenidejs waiting mechanism
+# TODO: let's consider removing them... or moving them e.g. to fp
 
 Lambda = Callable[[T], R]
 Proc = Callable[[T], None]
 Predicate = Callable[[T], bool]
 
 
 Fn = Callable[[T], R]
 
 
-# todo: consider moving outside of "wait" module... because there is no direct cohesion with it
-class Query(Generic[T, R]):
-    def __init__(self, description: str, fn: Callable[[T], R]):
+# TODO: consider moving outside of "wait" module... because there is no direct cohesion with it
+class Query(Generic[E, R]):
+    def __init__(self, description: str, fn: Callable[[E], R]):
         self._description = description
         self._fn = fn
 
-    def __call__(self, entity: T) -> R:
+    def __call__(self, entity: E) -> R:
         return self._fn(entity)
 
     def __str__(self):
         return self._description
 
 
-class Command(Query[T, None]):
+class Command(Generic[E], Query[E, None]):
     pass
 
 
-# todo: provide sexy fluent implementation via builder, i.e. Wait.the(element).atMost(3).orFailWith(hook)
+# TODO: provide sexy fluent implementation via builder, i.e. Wait.the(element).atMost(3).orFailWith(hook)
 class Wait(Generic[E]):
-
-    # todo: provide the smallest possible timeout default, something like 1ms
+    # TODO: provide the smallest possible timeout default, something like 1ms
     def __init__(
         self,
         entity: E,
-        at_most: int,
+        at_most: float,
         or_fail_with: Optional[Callable[[TimeoutException], Exception]] = None,
         _decorator: Callable[
-            [Wait[E]], Callable[[fp.T], fp.T]
+            [Wait[E]], Callable[[Callable[..., R]], Callable[..., R]]
         ] = lambda _: identity,
     ):
         self.entity = entity
         self._timeout = at_most
         self._hook_failure = or_fail_with or identity
         self._decorator = _decorator
 
@@ -91,71 +90,68 @@
         warnings.warn(
             'wait.entity will be removed in next version, '
             + 'please use wait.entity instead',
             DeprecationWarning,
         )
         return self.entity
 
-    def at_most(self, timeout: int) -> Wait[E]:
+    def at_most(self, timeout: float) -> Wait[E]:
         return Wait(self.entity, timeout, self._hook_failure)
 
     def or_fail_with(
         self, hook_failure: Optional[Callable[[TimeoutException], Exception]]
     ) -> Wait[E]:
-
         return Wait(self.entity, self._timeout, hook_failure)
 
     @property
     def hook_failure(
         self,
     ) -> Optional[Callable[[TimeoutException], Exception]]:
-        # todo: hook_failure or failure_hook?
+        # TODO: hook_failure or failure_hook?
         return self._hook_failure
 
-    # todo: consider renaming to `def to(...)`, though will sound awkward when wait.to(condition)
+    # TODO: consider renaming to `def to(...)`, though will sound awkward when wait.to(condition)
     def for_(self, fn: Callable[[E], R]) -> R:
-        @self._decorator(self)
-        def _(fn: Callable[[E], R]) -> R:
+        def logic(fn: Callable[[E], R]) -> R:
             finish_time = time.time() + self._timeout
 
             while True:
                 try:
                     return fn(self.entity)
                 except Exception as reason:
                     if time.time() > finish_time:
-
                         reason_message = str(reason)
 
                         reason_string = '{name}: {message}'.format(
                             name=reason.__class__.__name__,
                             message=reason_message,
                         )
-                        # todo: think on how can we improve logging failures in selene, e.g. reverse msg and stacktrace
+                        # TODO: think on how can we improve logging failures in selene, e.g. reverse msg and stacktrace
                         # stacktrace = getattr(reason, 'stacktrace', None)
                         timeout = self._timeout
                         entity = self.entity
 
                         failure = TimeoutException(
                             f'\n'
                             f'\nTimed out after {timeout}s, while waiting for:'
                             f'\n{entity}.{fn}'
                             f'\n'
                             f'\nReason: {reason_string}'
                         )
 
                         raise self._hook_failure(failure)
 
-        return _(fn)
+        return self._decorator(self)(logic)(fn)
 
     def until(self, fn: Callable[[E], R]) -> bool:
         try:
             self.for_(fn)
             return True
         except TimeoutException:
             return False
 
-    # todo: do we really need these aliases?
+    # TODO: do we really need these aliases?
     def command(self, description: str, fn: Callable[[E], None]) -> None:
         self.for_(Command(description, fn))
 
     def query(self, description: str, fn: Callable[[E], R]) -> R:
         return self.for_(Query(description, fn))
```

### Comparing `selene-2.0.0b9/selene/support/_logging.py` & `selene-2.0.0rc1/selene/support/_logging.py`

 * *Files 25% similar despite different names*

```diff
@@ -50,20 +50,49 @@
     :param context:
         Allure-like ContextManager factory
         (i.e. a type/class or function to return python context manager),
         that builds a context manager based on title string and params dict
     :param translations:
         Iterable of translations as (from, to) substitution pairs
         to apply to final title string to log
+
+    Examples:
+        Given added allure dependency to your project,
+        you can configure logging Selene commands to Allure report as simply as:
+
+        >>> from selene import browser, support
+        >>> import allure_commons
+        >>>
+        >>> browser.config._wait_decorator = support._logging.wait_with(
+        >>>     context=allure_commons._allure.StepContext
+        >>> )
+
+        You also can pass a list of translations to be applied to final message to log,
+        something like:
+
+        >>> from selene import browser, support
+        >>> import allure_commons
+        >>>
+        >>> browser.config._wait_decorator = support._logging.wait_with(
+        >>>   context=allure_commons._allure.StepContext,
+        >>>   translations=(
+        >>>         ('browser.element', '$'),
+        >>>         ('browser.all', '$$'),
+        >>>   )
+        >>> )
+
+        You can also implement your own version of StepContext – feel free to use
+        Alure's context manager as example.
+        Or check some examples in Selene's tests, like this one:
+        browser__config__wait_decorator_with_decorator_from_support_logging_test.py
     """
 
     def decorator_factory(wait):
         def decorator(for_):
             def decorated(fn):
-
                 title = f'{wait.entity}: {fn}'
 
                 def translate(initial: str, item: Tuple[str, str]):
                     old, new = item
                     return initial.replace(old, new)
 
                 translated_title = reduce(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `selene-2.0.0b9/selene/support/by.py` & `selene-2.0.0rc1/selene/support/by.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     return xpath(
         './/*[text()[contains(normalize-space(.), '
         + _escape_text_quotes_for_xpath(value)
         + ')]]'
     )
 
 
-# todo: deprecate be_* ? since they hide "xpath" logic, which may not be working in all cases
+# TODO: deprecate be_* ? since they hide "xpath" logic, which may not be working in all cases
 #       for example in case of mobile...
 #       maybe the only good thing to keep is by.text and by.partial_text
 
 
 def be_following_sibling(with_tag: str = '*'):
     warnings.warn(
         'deprecated; use xpath explicitly to not hide complexity in workaround',
```

### Comparing `selene-2.0.0b9/selene/support/conditions/be.py` & `selene-2.0.0rc1/selene/support/conditions/be.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 not_ = _not_
 
 visible = match.element_is_visible
 hidden = match.element_is_hidden
 selected = match.element_is_selected
 
 present = match.element_is_present
-in_dom = match.element_is_present  # todo: do we need both present and in_dom?
-existing = match.element_is_present  # todo: consider deprecating
+in_dom = match.element_is_present  # TODO: do we need both present and in_dom?
+existing = match.element_is_present  # TODO: consider deprecating
 
 absent = match.element_is_absent
 
 enabled = match.element_is_enabled
 disabled = match.element_is_disabled
 
 clickable = match.element_is_clickable
```

### Comparing `selene-2.0.0b9/selene/support/conditions/have.py` & `selene-2.0.0rc1/selene/support/conditions/have.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,75 +16,85 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import warnings
-from typing import Any
+from typing import Any, Union, Iterable, Optional
 
 from selene.core import match
 from selene.core.condition import Condition
 from selene.core.entity import Element, Collection, Browser
 from selene.support.conditions import not_ as _not_
 
 no = _not_
 
 
 def exact_text(value) -> Condition[Element]:
     return match.element_has_exact_text(value)
 
 
-# todo: consider accepting int
+# TODO: consider accepting int
 def text(partial_value) -> Condition[Element]:
     return match.element_has_text(partial_value)
 
 
-# todo: should we use here js.property style (and below for js.returned(...))
-def js_property(name: str, value: str = None):
+# TODO: should we use here js.property style (and below for js.returned(...))
+def js_property(name: str, value: Optional[str] = None):
     if value:
         warnings.warn(
             'passing second argument is deprecated; use have.js_property(foo).value(bar) instead',
             DeprecationWarning,
         )
         return match.element_has_js_property(name).value(value)
 
     return match.element_has_js_property(name)
 
 
-def css_property(name: str, value: str = None):
+def css_property(name: str, value: Optional[str] = None):
     if value:
         warnings.warn(
             'passing second argument is deprecated; use have.css_property(foo).value(bar) instead',
             DeprecationWarning,
         )
         return match.element_has_css_property(name).value(value)
 
     return match.element_has_css_property(name)
 
 
-def attribute(name: str, value: str = None):
+def attribute(name: str, value: Optional[str] = None):
     if value:
         warnings.warn(
             'passing second argument is deprecated; use have.attribute(foo).value(bar) instead',
             DeprecationWarning,
         )
         return match.element_has_attribute(name).value(value)
 
     return match.element_has_attribute(name)
 
 
 def value(text) -> Condition[Element]:
     return match.element_has_value(text)
 
 
+def values(*texts: Union[str, Iterable[str]]) -> Condition[Collection]:
+    return match.collection_has_values(*texts)
+
+
 def value_containing(partial_text) -> Condition[Element]:
     return match.element_has_value_containing(partial_text)
 
 
+def values_containing(
+    *partial_texts: Union[str, Iterable[str]]
+) -> Condition[Collection]:
+    return match.collection_has_values_containing(*partial_texts)
+
+
 def css_class(name) -> Condition[Element]:
     return match.element_has_css_class(name)
 
 
 def tag(name: str) -> Condition[Element]:
     return match.element_has_tag(name)
 
@@ -120,20 +130,20 @@
     return match.collection_has_size_greater_than_or_equal(number)
 
 
 def size_greater_than_or_equal(number: int) -> Condition[Collection]:
     return match.collection_has_size_greater_than_or_equal(number)
 
 
-# todo: consider accepting ints
-def texts(*partial_values: str) -> Condition[Collection]:
+# TODO: consider accepting ints
+def texts(*partial_values: Union[str, Iterable[str]]) -> Condition[Collection]:
     return match.collection_has_texts(*partial_values)
 
 
-def exact_texts(*values: str) -> Condition[Collection]:
+def exact_texts(*values: Union[str, Iterable[str]]) -> Condition[Collection]:
     return match.collection_has_exact_texts(*values)
 
 
 def url(exact_value: str) -> Condition[Browser]:
     return match.browser_has_url(exact_value)
 
 
@@ -167,15 +177,24 @@
 
 def tabs_number_greater_than_or_equal(value: int) -> Condition[Browser]:
     return match.browser_has_tabs_number_greater_than_or_equal(value)
 
 
 def js_returned_true(script_to_return_bool: str) -> Condition[Browser]:
     warnings.warn(
-        'might be deprecated; use have.js_returned(True, ...) instead',
-        PendingDeprecationWarning,
+        'deprecated; use have.script_returned(True, ...) instead',
+        DeprecationWarning,
     )
-    return match.browser_has_js_returned(True, script_to_return_bool)
+    return match.browser_has_script_returned(True, script_to_return_bool)
 
 
 def js_returned(expected: Any, script: str, *args) -> Condition[Browser]:
-    return match.browser_has_js_returned(expected, script, *args)
+    warnings.warn(
+        'deprecated because js does not work for mobile; '
+        'use have.script_returned(True, ...) instead',
+        DeprecationWarning,
+    )
+    return match.browser_has_script_returned(expected, script, *args)
+
+
+def script_returned(expected: Any, script: str, *args) -> Condition[Browser]:
+    return match.browser_has_script_returned(expected, script, *args)
```

### Comparing `selene-2.0.0b9/selene/support/conditions/not_.py` & `selene-2.0.0rc1/selene/support/conditions/not_.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from selene.core.entity import Element, Collection, Browser
 
 visible: Condition[Element] = _match.element_is_visible.not_
 hidden: Condition[Element] = _match.element_is_hidden.not_
 
 present: Condition[Element] = _match.element_is_present.not_
 in_dom: Condition[Element] = _match.element_is_present.not_
-# todo: do we need both present and in_dom?
-# todo: consider deprecating existing
+# TODO: do we need both present and in_dom?
+# TODO: consider deprecating existing
 existing: Condition[Element] = _match.element_is_present.not_
 
 absent: Condition[Element] = _match.element_is_absent.not_
 
 enabled: Condition[Element] = _match.element_is_enabled.not_
 disabled: Condition[Element] = _match.element_is_disabled.not_
 
@@ -48,36 +48,39 @@
 # --- have.* conditions --- #
 
 
 def exact_text(value) -> Condition[Element]:
     return _match.element_has_exact_text(value).not_
 
 
-# todo: consider accepting int
+# TODO: consider accepting int
 def text(partial_value) -> Condition[Element]:
     return _match.element_has_text(partial_value).not_
 
 
-def attribute(name: str, value: str = None):
-    if value:
+def attribute(name: str, *args, **kwargs):
+    if args or 'value' in kwargs:
         warnings.warn(
-            'passing second argument is deprecated; use have.attribute(foo).value(bar) instead',
+            'passing second argument is deprecated; '
+            'use have.attribute(foo).value(bar) instead',
             DeprecationWarning,
         )
-        return _match.element_has_attribute(name).value(value).not_
+        return (
+            _match.element_has_attribute(name)
+            .value(args[0] if args else kwargs['value'])
+            .not_
+        )
 
     original = _match.element_has_attribute(name)
     negated = original.not_
 
     def value(self, expected: str, ignore_case=False) -> Condition[Element]:
         return original.value(expected, ignore_case).not_
 
-    def value_containing(
-        self, expected: str, ignore_case=False
-    ) -> Condition[Element]:
+    def value_containing(self, expected: str, ignore_case=False) -> Condition[Element]:
         return original.value_containing(expected, ignore_case).not_
 
     def values(self, *expected: str) -> Condition[Collection]:
         return original.values(*expected).not_
 
     def values_containing(self, *expected: str) -> Condition[Collection]:
         return original.values_containing(*expected).not_
@@ -86,21 +89,26 @@
     negated.value_containing = value_containing
     negated.values = values
     negated.values_containing = values_containing
 
     return negated
 
 
-def js_property(name: str, value: str = None):
-    if value:
+def js_property(name: str, *args, **kwargs):
+    if args or 'value' in kwargs:
         warnings.warn(
-            'passing second argument is deprecated; use have.js_property(foo).value(bar) instead',
+            'passing second argument is deprecated; '
+            'use have.js_property(foo).value(bar) instead',
             DeprecationWarning,
         )
-        return _match.element_has_js_property(name).value(value).not_
+        return (
+            _match.element_has_js_property(name)
+            .value(args[0] if args else kwargs['value'])
+            .not_
+        )
 
     original = _match.element_has_js_property(name)
     negated = original.not_
 
     def value(self, expected: str) -> Condition[Element]:
         return original.value(expected).not_
 
@@ -117,21 +125,26 @@
     negated.value_containing = value_containing
     negated.values = values
     negated.values_containing = values_containing
 
     return negated
 
 
-def css_property(name: str, value: str = None):
-    if value:
+def css_property(name: str, *args, **kwargs):
+    if args or 'value' in kwargs:
         warnings.warn(
-            'passing second argument is deprecated; use have.css_property(foo).value(bar) instead',
+            'passing second argument is deprecated; '
+            'use have.css_property(foo).value(bar) instead',
             DeprecationWarning,
         )
-        return _match.element_has_css_property(name).value(value).not_
+        return (
+            _match.element_has_css_property(name)
+            .value(args[0] if args else kwargs['value'])
+            .not_
+        )
 
     original = _match.element_has_css_property(name)
     negated = original.not_
 
     def value(self, expected: str) -> Condition[Element]:
         return original.value(expected).not_
 
@@ -199,15 +212,15 @@
     return _match.collection_has_size_greater_than_or_equal(number).not_
 
 
 def size_greater_than_or_equal(number: int) -> Condition[Collection]:
     return _match.collection_has_size_greater_than_or_equal(number).not_
 
 
-# todo: consider accepting ints
+# TODO: consider accepting ints
 def texts(*partial_values: str) -> Condition[Collection]:
     return _match.collection_has_texts(*partial_values).not_
 
 
 def exact_texts(*values: str) -> Condition[Collection]:
     return _match.collection_has_exact_texts(*values).not_
```

### Comparing `selene-2.0.0b9/selene/support/jquery_style_selectors.py` & `selene-2.0.0rc1/selene/support/shared/jquery_style.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,30 +15,19 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import warnings
-from typing import Union
+from typing import Union, Tuple
 
 from selene.core.entity import Element, Collection
-from selene.support.shared import browser
+from selene import browser
 
 
-def s(css_or_xpath_or_by: Union[str, tuple]) -> Element:
-    warnings.warn(
-        'selene.support.jquery_style_selectors.s is deprecated; '
-        'use selene.support.shared.jquery_style.s instead',
-        DeprecationWarning,
-    )
+def s(css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Element:
     return browser.element(css_or_xpath_or_by)
 
 
-def ss(css_or_xpath_or_by: Union[str, tuple]) -> Collection:
-    warnings.warn(
-        'selene.support.jquery_style_selectors.ss is deprecated; '
-        'use selene.support.shared.jquery_style.ss instead',
-        DeprecationWarning,
-    )
+def ss(css_or_xpath_or_by: Union[str, Tuple[str, str]]) -> Collection:
     return browser.all(css_or_xpath_or_by)
```

### Comparing `selene-2.0.0b9/selene/support/shared/__init__.py` & `selene-2.0.0rc1/selene/support/shared/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,12 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
+from selene import _managed
 
-from selene.support.shared.browser import SharedBrowser
-from selene.support.shared.config import SharedConfig
 
-config = SharedConfig()
-
-browser = SharedBrowser(config)
+config = _managed.config
+browser = _managed.browser
```

### Comparing `selene-2.0.0b9/selene/support/shared/jquery_style.py` & `selene-2.0.0rc1/selene/support/shared/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-from typing import Union
+import warnings
 
-from selene.core.entity import Element, Collection
-from selene.support.shared import browser
+from selene.core.entity import Browser
 
 
-def s(css_or_xpath_or_by: Union[str, tuple]) -> Element:
-    return browser.element(css_or_xpath_or_by)
-
-
-def ss(css_or_xpath_or_by: Union[str, tuple]) -> Collection:
-    return browser.all(css_or_xpath_or_by)
+class SharedBrowser(Browser):
+    warnings.warn(
+        'SharedBrowser is deprecated, use Browser instead', DeprecationWarning
+    )
```

### Comparing `selene-2.0.0b9/selene/support/webdriver.py` & `selene-2.0.0rc1/selene/support/webdriver.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 from typing import Optional
 
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from selene.common.helpers import on_error_return_false
 
 
-class WebHelper:  # todo: should we make it private? like call it _Help (or think on better name)
+class WebHelper:
+    # TODO: should we make it private? like call it _Help (or think on better name)
     # what about this style for example: ExtendedWebdriver(driver).is_alive() ?
     # over: Help(driver).has_browser_still_alive() ?
 
-    def __init__(self, driver: Optional[WebDriver]):
+    def __init__(self, driver: WebDriver):
         self._driver = driver
 
+    # TODO: refactor to browser.get(query.is_alive)
+    #       or browser.get(query.is_driver_alive) ?
     def is_browser_still_alive(self):
         return on_error_return_false(lambda: self._driver.title is not None)
 
     def save_page_source(self, file: str) -> Optional[str]:
         if not file.lower().endswith('.html'):
             warnings.warn(
                 "name used for saved pagesource does not match file "
@@ -56,13 +59,13 @@
             del html
 
         return file
 
     def save_screenshot(self, file: str) -> Optional[str]:
         if not file.lower().endswith('.png'):
             warnings.warn(
-                "name used for saved pagesource does not match file "
+                "name used for saved screenshot does not match file "
                 "type. It should end with an `.png` extension",
                 UserWarning,
             )
 
         return file if self._driver.get_screenshot_as_file(file) else None
```

