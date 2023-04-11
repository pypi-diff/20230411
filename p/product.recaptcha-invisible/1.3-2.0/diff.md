# Comparing `tmp/product.recaptcha_invisible-1.3.tar.gz` & `tmp/product.recaptcha_invisible-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/product.recaptcha_invisible-1.3.tar", last modified: Tue Mar 21 07:44:42 2023, max compression
+gzip compressed data, was "product.recaptcha_invisible-2.0.tar", last modified: Tue Apr 11 12:07:28 2023, max compression
```

## Comparing `product.recaptcha_invisible-1.3.tar` & `product.recaptcha_invisible-2.0.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/
--rwxr-xr-x   0 root         (0) plone_group  (1000)      561 2023-03-21 07:43:33.000000 product.recaptcha_invisible-1.3/CHANGES.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)       62 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/CONTRIBUTORS.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)      586 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/DEVELOP.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)      667 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/LICENSE.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)       64 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) plone_group  (1000)     3315 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/PKG-INFO
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1022 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/README.rst
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/docs/
--rwxr-xr-x   0 root         (0) plone_group  (1000)     7933 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/docs/conf.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      104 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/docs/index.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)      321 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/setup.cfg
--rwxr-xr-x   0 root         (0) plone_group  (1000)     2301 2023-03-21 07:42:18.000000 product.recaptcha_invisible-1.3/setup.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/
--rwxr-xr-x   0 root         (0) plone_group  (1000)       80 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/__init__.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/
--rwxr-xr-x   0 root         (0) plone_group  (1000)      122 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/__init__.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/__init__.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      969 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/configure.zcml
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/overrides/
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/overrides/.gitkeep
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/static/
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/static/.gitkeep
--rwxr-xr-x   0 root         (0) plone_group  (1000)     3019 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/verify.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1285 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/configure.zcml
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1139 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/controlpanel.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      554 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/controlpanel.zcml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      614 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/field.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      715 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/field.zcml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      526 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/interfaces.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/
--rwxr-xr-x   0 root         (0) plone_group  (1000)      611 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/README.rst
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/__init__.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/ca/
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1778 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.po
--rwxr-xr-x   0 root         (0) plone_group  (1000)       99 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/compile.sh
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/en/
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1747 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.po
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/es/
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1788 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.po
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/manual.pot
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1386 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/product.recaptcha_invisible.pot
--rwxr-xr-x   0 root         (0) plone_group  (1000)      559 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/update.sh
--rwxr-xr-x   0 root         (0) plone_group  (1000)      260 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/permissions.zcml
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/
--rwxr-xr-x   0 root         (0) plone_group  (1000)      206 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/browserlayer.xml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      609 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/controlpanel.xml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      120 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/metadata.xml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      176 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/registry.xml
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/uninstall/
--rwxr-xr-x   0 root         (0) plone_group  (1000)      137 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/uninstall/browserlayer.xml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      628 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/setuphandlers.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1694 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/testing.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/
--rwxr-xr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/__init__.py
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/robot/
--rwxr-xr-x   0 root         (0) plone_group  (1000)     2039 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/robot/test_example.robot
--rwxr-xr-x   0 root         (0) plone_group  (1000)      922 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/test_robot.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)     2582 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/test_setup.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      782 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/validator.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1064 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget.py
--rwxr-xr-x   0 root         (0) plone_group  (1000)      627 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget.zcml
--rwxr-xr-x   0 root         (0) plone_group  (1000)      187 2023-03-21 07:32:14.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget_display.pt
--rwxr-xr-x   0 root         (0) plone_group  (1000)     1516 2023-03-21 07:41:02.000000 product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget_input.pt
-drwxr-sr-x   0 root         (0) plone_group  (1000)        0 2023-03-21 07:44:42.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/
--rw-r--r--   0 root         (0) plone_group  (1000)     3315 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) plone_group  (1000)     2683 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) plone_group  (1000)        1 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) plone_group  (1000)      152 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) plone_group  (1000)        8 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) plone_group  (1000)        1 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) plone_group  (1000)      173 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/requires.txt
--rw-r--r--   0 root         (0) plone_group  (1000)        8 2023-03-21 07:44:41.000000 product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.878365 product.recaptcha_invisible-2.0/
+-rwxrwxrwx   0 root         (0) root         (0)      654 2023-04-11 12:04:08.000000 product.recaptcha_invisible-2.0/CHANGES.rst
+-rwxrwxrwx   0 root         (0) root         (0)       62 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/CONTRIBUTORS.rst
+-rwxrwxrwx   0 root         (0) root         (0)      586 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/DEVELOP.rst
+-rwxrwxrwx   0 root         (0) root         (0)    18092 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/LICENSE.GPL
+-rwxrwxrwx   0 root         (0) root         (0)      667 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/LICENSE.rst
+-rwxrwxrwx   0 root         (0) root         (0)       64 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-11 12:07:28.878365 product.recaptcha_invisible-2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1022 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.869365 product.recaptcha_invisible-2.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     7933 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/docs/conf.py
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/docs/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)      321 2023-04-11 12:07:28.878365 product.recaptcha_invisible-2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2253 2023-04-11 12:06:21.000000 product.recaptcha_invisible-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.864365 product.recaptcha_invisible-2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.870365 product.recaptcha_invisible-2.0/src/product/
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.873365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/
+-rwxrwxrwx   0 root         (0) root         (0)      122 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.873365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      969 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/configure.zcml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.874365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/overrides/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/overrides/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.874365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/static/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/static/.gitkeep
+-rwxrwxrwx   0 root         (0) root         (0)     3019 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/verify.py
+-rwxrwxrwx   0 root         (0) root         (0)     1285 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/configure.zcml
+-rwxrwxrwx   0 root         (0) root         (0)     1139 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/controlpanel.py
+-rwxrwxrwx   0 root         (0) root         (0)      554 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/controlpanel.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/field.py
+-rwxrwxrwx   0 root         (0) root         (0)      715 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/field.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      526 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.875365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/
+-rwxrwxrwx   0 root         (0) root         (0)      611 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.865365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.876365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-11 12:04:04.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.mo
+-rwxrwxrwx   0 root         (0) root         (0)     1778 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.po
+-rwxrwxrwx   0 root         (0) root         (0)       99 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/compile.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.866365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.876365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-04-11 12:04:04.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.mo
+-rwxrwxrwx   0 root         (0) root         (0)     1747 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.867365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.876365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-04-11 12:04:04.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.mo
+-rwxrwxrwx   0 root         (0) root         (0)     1788 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.po
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/manual.pot
+-rwxrwxrwx   0 root         (0) root         (0)     1386 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/product.recaptcha_invisible.pot
+-rwxrwxrwx   0 root         (0) root         (0)      559 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/update.sh
+-rwxrwxrwx   0 root         (0) root         (0)      260 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/permissions.zcml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.867365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.877365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/
+-rwxrwxrwx   0 root         (0) root         (0)      206 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/browserlayer.xml
+-rwxrwxrwx   0 root         (0) root         (0)      609 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/controlpanel.xml
+-rwxrwxrwx   0 root         (0) root         (0)      120 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/metadata.xml
+-rwxrwxrwx   0 root         (0) root         (0)      176 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/registry.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.877365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/uninstall/
+-rwxrwxrwx   0 root         (0) root         (0)      137 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/uninstall/browserlayer.xml
+-rwxrwxrwx   0 root         (0) root         (0)      628 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/setuphandlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1694 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.877365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.878365 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/robot/
+-rwxrwxrwx   0 root         (0) root         (0)     2039 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/robot/test_example.robot
+-rwxrwxrwx   0 root         (0) root         (0)      922 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/test_robot.py
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/test_setup.py
+-rwxrwxrwx   0 root         (0) root         (0)      782 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/validator.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget.py
+-rwxrwxrwx   0 root         (0) root         (0)      655 2023-04-11 12:05:10.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      187 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget_display.pt
+-rwxrwxrwx   0 root         (0) root         (0)     1516 2023-04-11 12:00:08.000000 product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget_input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:07:28.871365 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:01:54.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      173 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 12:07:28.000000 product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `product.recaptcha_invisible-1.3/CHANGES.rst` & `product.recaptcha_invisible-2.0/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.0 (11/04/2023)
+------------------
+
+- Update widget to Boostrap 5 and Plone 6 [csanahuja]
+
+
 1.3 (21/03/2023)
 ------------------
 
 Fixes:
 
 - Fix widget for easyform when more than one button with submit-widget class exists
   [csanahuja]
```

### Comparing `product.recaptcha_invisible-1.3/DEVELOP.rst` & `product.recaptcha_invisible-2.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/LICENSE.rst` & `product.recaptcha_invisible-2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/README.rst` & `product.recaptcha_invisible-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/docs/conf.py` & `product.recaptcha_invisible-2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/setup.py` & `product.recaptcha_invisible-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='product.recaptcha_invisible',
-    version='1.3',
+    version='2.0',
     description="Recaptcha Invisible suport for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone',
     author='csanahuja',
     author_email='csanahuja10@gmail.com',
     url='https://gitlab.com/csanahuja/product.recaptcha_invisible',
@@ -39,15 +38,15 @@
     },
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['product'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
         'z3c.jbot',
         'plone.api>=1.8.4',
         'plone.restapi',
         'plone.app.dexterity',
```

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/configure.zcml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/browser/verify.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/browser/verify.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/configure.zcml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/configure.zcml`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/controlpanel.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/controlpanel.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/controlpanel.zcml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/controlpanel.zcml`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/field.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/field.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/field.zcml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/field.zcml`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/interfaces.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/interfaces.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/README.rst` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/README.rst`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.po` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.po`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.po` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.po`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.po` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.po`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/product.recaptcha_invisible.pot` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/product.recaptcha_invisible.pot`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/locales/update.sh` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/locales/update.sh`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/profiles/default/controlpanel.xml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/setuphandlers.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/testing.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/testing.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/robot/test_example.robot` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/test_robot.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/tests/test_setup.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/validator.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/validator.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget.py` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget.py`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget.zcml` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,20 @@
     xmlns="http://namespaces.zope.org/zope"
     xmlns:z3c="http://namespaces.zope.org/z3c">
 
     <adapter factory=".widget.ReCaptchaInvisibleFieldWidget" />
 
     <z3c:widgetTemplate
         template="widget_display.pt"
-        layer="z3c.form.interfaces.IFormLayer"
+        layer="plone.app.z3cform.interfaces.IPloneFormLayer"
         mode="display"
         widget="product.recaptcha_invisible.interfaces.IRecaptchaInvisibleWidget"
         />
 
     <z3c:widgetTemplate
         template="widget_input.pt"
-        layer="z3c.form.interfaces.IFormLayer"
+        layer="plone.app.z3cform.interfaces.IPloneFormLayer"
         mode="input"
         widget="product.recaptcha_invisible.interfaces.IRecaptchaInvisibleWidget"
         />
 
 </configure>
```

### Comparing `product.recaptcha_invisible-1.3/src/product/recaptcha_invisible/widget_input.pt` & `product.recaptcha_invisible-2.0/src/product/recaptcha_invisible/widget_input.pt`

 * *Files identical despite different names*

### Comparing `product.recaptcha_invisible-1.3/src/product.recaptcha_invisible.egg-info/SOURCES.txt` & `product.recaptcha_invisible-2.0/src/product.recaptcha_invisible.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
@@ -39,16 +40,19 @@
 src/product/recaptcha_invisible/browser/static/.gitkeep
 src/product/recaptcha_invisible/locales/README.rst
 src/product/recaptcha_invisible/locales/__init__.py
 src/product/recaptcha_invisible/locales/compile.sh
 src/product/recaptcha_invisible/locales/manual.pot
 src/product/recaptcha_invisible/locales/product.recaptcha_invisible.pot
 src/product/recaptcha_invisible/locales/update.sh
+src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.mo
 src/product/recaptcha_invisible/locales/ca/LC_MESSAGES/product.recaptcha_invisible.po
+src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.mo
 src/product/recaptcha_invisible/locales/en/LC_MESSAGES/product.recaptcha_invisible.po
+src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.mo
 src/product/recaptcha_invisible/locales/es/LC_MESSAGES/product.recaptcha_invisible.po
 src/product/recaptcha_invisible/profiles/default/browserlayer.xml
 src/product/recaptcha_invisible/profiles/default/controlpanel.xml
 src/product/recaptcha_invisible/profiles/default/metadata.xml
 src/product/recaptcha_invisible/profiles/default/registry.xml
 src/product/recaptcha_invisible/profiles/uninstall/browserlayer.xml
 src/product/recaptcha_invisible/tests/__init__.py
```

