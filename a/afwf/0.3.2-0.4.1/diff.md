# Comparing `tmp/afwf-0.3.2.tar.gz` & `tmp/afwf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afwf-0.3.2.tar", last modified: Sat Apr  8 05:19:20 2023, max compression
+gzip compressed data, was "afwf-0.4.1.tar", last modified: Tue Apr 11 02:23:53 2023, max compression
```

## Comparing `afwf-0.3.2.tar` & `afwf-0.4.1.tar`

### file list

```diff
@@ -1,118 +1,146 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.456626 afwf-0.3.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-04-08 04:39:55.000000 afwf-0.3.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-04-08 04:39:55.000000 afwf-0.3.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-04-08 04:39:55.000000 afwf-0.3.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5404 2023-04-08 05:19:20.456424 afwf-0.3.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4220 2023-04-08 05:14:38.000000 afwf-0.3.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.441029 afwf-0.3.2/afwf/
--rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.443410 afwf-0.3.2/afwf/__pycache__/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1037 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      220 2023-04-08 05:19:19.000000 afwf-0.3.2/afwf/__pycache__/_version.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     2015 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/enumeration.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     3966 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     2762 2023-04-08 05:19:19.000000 afwf-0.3.2/afwf/__pycache__/icon.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)    10567 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/item.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/path.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1736 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/query.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1888 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/script_filter.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     1809 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/script_filter_object.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)     4871 2023-04-08 04:41:08.000000 afwf-0.3.2/afwf/__pycache__/workflow.cpython-38.pyc
--rw-r--r--   0 sanhehu    (501) staff       (20)      818 2023-04-08 05:17:16.000000 afwf-0.3.2/afwf/_icon.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-04-08 05:14:50.000000 afwf-0.3.2/afwf/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.443530 afwf-0.3.2/afwf/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1284 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/enumeration.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.443924 afwf-0.3.2/afwf/example_wf/
--rw-r--r--   0 sanhehu    (501) staff       (20)      132 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/example_wf/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/example_wf/cache.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.444214 afwf-0.3.2/afwf/example_wf/handlers/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/example_wf/handlers/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2148 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/example_wf/handlers/python_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3496 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/handler.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3297 2023-04-08 05:17:18.000000 afwf-0.3.2/afwf/icon.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.454301 afwf-0.3.2/afwf/icons/
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/android-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      648 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/archive-folder-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-04-08 09:08:18.000000 afwf-0.3.2/afwf/icons/bash-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      401 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/bookmark-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      525 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/box-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      570 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/calendar-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1702 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/chat-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      342 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/check-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      422 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/close-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1127 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/code-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-04-08 04:55:02.000000 afwf-0.3.2/afwf/icons/console-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1886 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/debug-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      306 2023-04-08 04:55:03.000000 afwf-0.3.2/afwf/icons/desktop-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      860 2023-04-08 09:08:18.000000 afwf-0.3.2/afwf/icons/dictionary-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      464 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/download-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      901 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/error-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1390 2023-04-08 04:48:18.000000 afwf-0.3.2/afwf/icons/explosion-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-04-08 04:55:00.000000 afwf-0.3.2/afwf/icons/file-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1174 2023-04-08 04:46:09.000000 afwf-0.3.2/afwf/icons/fire-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1217 2023-04-08 04:55:03.000000 afwf-0.3.2/afwf/icons/flask-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-04-08 04:55:00.000000 afwf-0.3.2/afwf/icons/folder-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1370 2023-04-08 04:44:43.000000 afwf-0.3.2/afwf/icons/gear-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-04-08 09:08:18.000000 afwf-0.3.2/afwf/icons/git-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     2305 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/groupchat-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1025 2023-04-08 09:08:18.000000 afwf-0.3.2/afwf/icons/id-card-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1584 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/idea-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-04-08 04:43:07.000000 afwf-0.3.2/afwf/icons/info-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     2388 2023-04-08 04:55:01.000000 afwf-0.3.2/afwf/icons/internet-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      581 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/iphone-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      578 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/landline-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-04-08 04:55:02.000000 afwf-0.3.2/afwf/icons/laptop-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      684 2023-04-08 04:54:57.000000 afwf-0.3.2/afwf/icons/mail-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1244 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/meeting-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      476 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/message-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      794 2023-04-08 04:54:59.000000 afwf-0.3.2/afwf/icons/microsoft-excel-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      718 2023-04-08 04:54:58.000000 afwf-0.3.2/afwf/icons/microsoft-powerpoint-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      926 2023-04-08 04:54:58.000000 afwf-0.3.2/afwf/icons/microsoft-word-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      688 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/minus-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      677 2023-04-08 09:08:18.000000 afwf-0.3.2/afwf/icons/password-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      734 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/pause-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      697 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/plus-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1146 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/question-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      609 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/redo-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      779 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/refresh-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      526 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/remove-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1014 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/reset-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1277 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/rocket-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)     1037 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/search-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      814 2023-04-08 04:48:18.000000 afwf-0.3.2/afwf/icons/star-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      772 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/start-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      850 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/stop-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      952 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/task-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      595 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/todo-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      381 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/trash-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      613 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/icons/undo-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-04-08 09:04:04.000000 afwf-0.3.2/afwf/icons/upload-96.png
--rw-r--r--   0 sanhehu    (501) staff       (20)    10476 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/item.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/path.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1170 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/query.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1385 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/script_filter.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1798 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/script_filter_object.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4936 2023-04-08 04:39:55.000000 afwf-0.3.2/afwf/workflow.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.441706 afwf-0.3.2/afwf.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5404 2023-04-08 05:19:20.000000 afwf-0.3.2/afwf.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2729 2023-04-08 05:19:20.000000 afwf-0.3.2/afwf.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-04-08 05:19:20.000000 afwf-0.3.2/afwf.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      203 2023-04-08 05:19:20.000000 afwf-0.3.2/afwf.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-04-08 05:19:20.000000 afwf-0.3.2/afwf.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     3405 2023-04-08 05:18:50.000000 afwf-0.3.2/preview-icons.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1877 2023-04-08 05:15:16.000000 afwf-0.3.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      305 2023-04-08 04:39:55.000000 afwf-0.3.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-08 04:39:55.000000 afwf-0.3.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-04-08 04:39:55.000000 afwf-0.3.2/requirements-ground-truth.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-04-08 04:39:55.000000 afwf-0.3.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-04-08 04:39:55.000000 afwf-0.3.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-04-08 05:19:20.456683 afwf-0.3.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7700 2023-04-08 04:39:55.000000 afwf-0.3.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-08 05:19:20.456131 afwf-0.3.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      608 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_enumeration.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      532 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1233 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_item.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      651 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_query.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      558 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_script_filter.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1941 2023-04-08 04:39:55.000000 afwf-0.3.2/tests/test_script_filter_object.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.162783 afwf-0.4.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-04-08 04:39:55.000000 afwf-0.4.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-04-08 04:39:55.000000 afwf-0.4.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-04-08 04:39:55.000000 afwf-0.4.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5404 2023-04-11 02:23:53.162647 afwf-0.4.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4220 2023-04-08 05:14:38.000000 afwf-0.4.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.144607 afwf-0.4.1/afwf/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      857 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.146426 afwf-0.4.1/afwf/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1037 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      220 2023-04-11 02:23:52.000000 afwf-0.4.1/afwf/__pycache__/_version.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2015 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/enumeration.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3966 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2762 2023-04-08 05:19:19.000000 afwf-0.4.1/afwf/__pycache__/icon.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10607 2023-04-11 02:23:52.000000 afwf-0.4.1/afwf/__pycache__/item.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/path.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1736 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/query.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1888 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/script_filter.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1809 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/script_filter_object.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4871 2023-04-08 04:41:08.000000 afwf-0.4.1/afwf/__pycache__/workflow.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      818 2023-04-08 05:17:16.000000 afwf-0.4.1/afwf/_icon.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-04-11 02:20:36.000000 afwf-0.4.1/afwf/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.146547 afwf-0.4.1/afwf/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1284 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/enumeration.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.146816 afwf-0.4.1/afwf/example_wf/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      132 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/example_wf/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.147160 afwf-0.4.1/afwf/example_wf/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      288 2023-04-10 23:57:29.000000 afwf-0.4.1/afwf/example_wf/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      392 2023-04-10 23:57:29.000000 afwf-0.4.1/afwf/example_wf/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      252 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/example_wf/cache.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.147520 afwf-0.4.1/afwf/example_wf/handlers/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/example_wf/handlers/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.147852 afwf-0.4.1/afwf/example_wf/handlers/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      172 2023-04-10 23:57:29.000000 afwf-0.4.1/afwf/example_wf/handlers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2304 2023-04-10 23:57:29.000000 afwf-0.4.1/afwf/example_wf/handlers/__pycache__/python_version.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2148 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/example_wf/handlers/python_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3496 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/handler.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3297 2023-04-08 05:17:18.000000 afwf-0.4.1/afwf/icon.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.157673 afwf-0.4.1/afwf/icons/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/android-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      648 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/archive-folder-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1617 2023-04-08 09:08:18.000000 afwf-0.4.1/afwf/icons/bash-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      401 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/bookmark-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      525 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/box-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      570 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/calendar-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1702 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/chat-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      342 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/check-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      422 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/close-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1127 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/code-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-04-08 04:55:02.000000 afwf-0.4.1/afwf/icons/console-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1886 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/debug-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      306 2023-04-08 04:55:03.000000 afwf-0.4.1/afwf/icons/desktop-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      860 2023-04-08 09:08:18.000000 afwf-0.4.1/afwf/icons/dictionary-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      464 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/download-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      901 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/error-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1390 2023-04-08 04:48:18.000000 afwf-0.4.1/afwf/icons/explosion-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-04-08 04:55:00.000000 afwf-0.4.1/afwf/icons/file-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1174 2023-04-08 04:46:09.000000 afwf-0.4.1/afwf/icons/fire-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1217 2023-04-08 04:55:03.000000 afwf-0.4.1/afwf/icons/flask-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-04-08 04:55:00.000000 afwf-0.4.1/afwf/icons/folder-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1370 2023-04-08 04:44:43.000000 afwf-0.4.1/afwf/icons/gear-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      724 2023-04-08 09:08:18.000000 afwf-0.4.1/afwf/icons/git-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2305 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/groupchat-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1025 2023-04-08 09:08:18.000000 afwf-0.4.1/afwf/icons/id-card-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1584 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/idea-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      438 2023-04-08 04:43:07.000000 afwf-0.4.1/afwf/icons/info-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2388 2023-04-08 04:55:01.000000 afwf-0.4.1/afwf/icons/internet-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      581 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/iphone-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      578 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/landline-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      400 2023-04-08 04:55:02.000000 afwf-0.4.1/afwf/icons/laptop-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      684 2023-04-08 04:54:57.000000 afwf-0.4.1/afwf/icons/mail-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1244 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/meeting-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      476 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/message-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      794 2023-04-08 04:54:59.000000 afwf-0.4.1/afwf/icons/microsoft-excel-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      718 2023-04-08 04:54:58.000000 afwf-0.4.1/afwf/icons/microsoft-powerpoint-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      926 2023-04-08 04:54:58.000000 afwf-0.4.1/afwf/icons/microsoft-word-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      688 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/minus-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      677 2023-04-08 09:08:18.000000 afwf-0.4.1/afwf/icons/password-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      734 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/pause-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      697 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/plus-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1146 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/question-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      609 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/redo-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      779 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/refresh-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      526 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/remove-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1014 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/reset-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1277 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/rocket-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1037 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/search-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      814 2023-04-08 04:48:18.000000 afwf-0.4.1/afwf/icons/star-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      772 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/start-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      850 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/stop-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      952 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/task-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      595 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/todo-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      381 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/trash-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      613 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/icons/undo-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-04-08 09:04:04.000000 afwf-0.4.1/afwf/icons/upload-96.png
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10776 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/item.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.157830 afwf-0.4.1/afwf/opt/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      111 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.158636 afwf-0.4.1/afwf/opt/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      245 2023-04-10 23:59:58.000000 afwf-0.4.1/afwf/opt/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.159057 afwf-0.4.1/afwf/opt/cache/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       63 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/cache/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.159513 afwf-0.4.1/afwf/opt/cache/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      208 2023-04-11 02:13:37.000000 afwf-0.4.1/afwf/opt/cache/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1208 2023-04-11 02:13:37.000000 afwf-0.4.1/afwf/opt/cache/__pycache__/impl.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      811 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/cache/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.159937 afwf-0.4.1/afwf/opt/fuzzy/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/fuzzy/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.160366 afwf-0.4.1/afwf/opt/fuzzy/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      196 2023-04-11 01:58:20.000000 afwf-0.4.1/afwf/opt/fuzzy/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3751 2023-04-11 02:04:53.000000 afwf-0.4.1/afwf/opt/fuzzy/__pycache__/impl.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3509 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/fuzzy/impl.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.160807 afwf-0.4.1/afwf/opt/fuzzy_item/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       59 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/fuzzy_item/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.161185 afwf-0.4.1/afwf/opt/fuzzy_item/__pycache__/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      220 2023-04-11 02:03:23.000000 afwf-0.4.1/afwf/opt/fuzzy_item/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1403 2023-04-11 02:03:23.000000 afwf-0.4.1/afwf/opt/fuzzy_item/__pycache__/impl.cpython-38.pyc
+-rw-r--r--   0 sanhehu    (501) staff       (20)      809 2023-04-11 02:20:21.000000 afwf-0.4.1/afwf/opt/fuzzy_item/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/path.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1170 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/query.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1385 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/script_filter.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1798 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/script_filter_object.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4936 2023-04-08 04:39:55.000000 afwf-0.4.1/afwf/workflow.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.145181 afwf-0.4.1/afwf.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5404 2023-04-11 02:23:53.000000 afwf-0.4.1/afwf.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3488 2023-04-11 02:23:53.000000 afwf-0.4.1/afwf.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-04-11 02:23:53.000000 afwf-0.4.1/afwf.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      224 2023-04-11 02:23:53.000000 afwf-0.4.1/afwf.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-04-11 02:23:53.000000 afwf-0.4.1/afwf.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3405 2023-04-08 05:18:50.000000 afwf-0.4.1/preview-icons.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2406 2023-04-11 02:23:06.000000 afwf-0.4.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      305 2023-04-08 04:39:55.000000 afwf-0.4.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-04-08 04:39:55.000000 afwf-0.4.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-04-08 04:39:55.000000 afwf-0.4.1/requirements-ground-truth.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      204 2023-04-11 02:20:21.000000 afwf-0.4.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       32 2023-04-08 04:39:55.000000 afwf-0.4.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-04-11 02:23:53.162822 afwf-0.4.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7700 2023-04-08 04:39:55.000000 afwf-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-04-11 02:23:53.162449 afwf-0.4.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      608 2023-04-08 04:39:55.000000 afwf-0.4.1/tests/test_enumeration.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      532 2023-04-08 04:39:55.000000 afwf-0.4.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1233 2023-04-08 04:39:55.000000 afwf-0.4.1/tests/test_item.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      651 2023-04-08 04:39:55.000000 afwf-0.4.1/tests/test_query.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      534 2023-04-11 02:20:21.000000 afwf-0.4.1/tests/test_script_filter.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1941 2023-04-08 04:39:55.000000 afwf-0.4.1/tests/test_script_filter_object.py
```

### Comparing `afwf-0.3.2/LICENSE.txt` & `afwf-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/PKG-INFO` & `afwf-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: afwf
-Version: 0.3.2
+Version: 0.4.1
 Summary: A powerful framework enables fast and elegant development of Alfred Workflows in Python.
 Home-page: https://github.com/MacHu-GWU/afwf-project
-Download-URL: https://pypi.python.org/pypi/afwf/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/afwf/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `afwf-0.3.2/README.rst` & `afwf-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__init__.py` & `afwf-0.4.1/afwf/__init__.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/__init__.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/enumeration.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/enumeration.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/handler.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/icon.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/icon.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/item.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/item.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Apr  8 04:39:55 2023 UTC, .py size: 10476 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1bf0 3064 ec28 0000  U.........0d.(..
+00000000: 550d 0d0a 0000 0000 e5c3 3464 182a 0000  U.........4d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6401 6403 6c06  m.Z.m.Z...d.d.l.
 00000050: 5a06 6401 6404 6c06 6d07 5a08 0100 6401  Z.d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6406 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6406 6408 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -57,30 +57,30 @@
 00000380: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
 00000390: 730a 0000 007c 007c 0164 018d 0153 0029  s....|.|.d...S.)
 000003a0: 027a 5a0a 2020 2020 2020 2020 4372 6561  .zZ.        Crea
 000003b0: 7465 2061 6e20 4963 6f6e 206f 626a 6563  te an Icon objec
 000003c0: 7420 7468 6174 2075 7369 6e67 2061 2066  t that using a f
 000003d0: 696c 6520 6f6e 206c 6f63 616c 2066 696c  ile on local fil
 000003e0: 6520 7379 7374 656d 2061 7320 616e 2069  e system as an i
-000003f0: 636f 6e2e 0a20 2020 2020 2020 20a9 0172  con..        ..r
+000003f0: 636f 6e2e 0a20 2020 2020 2020 2029 0172  con..        ).r
 00000400: 1400 0000 7211 0000 0029 02da 0363 6c73  ....r....)...cls
 00000410: 7214 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
 00000420: 1200 0000 da0f 6672 6f6d 5f69 6d61 6765  ......from_image
 00000430: 5f66 696c 6521 0000 0073 0200 0000 0005  _file!...s......
 00000440: 7a14 4963 6f6e 2e66 726f 6d5f 696d 6167  z.Icon.from_imag
 00000450: 655f 6669 6c65 2914 720e 0000 0072 0f00  e_file).r....r..
 00000460: 0000 7210 0000 00da 075f 5f64 6f63 5f5f  ..r......__doc__
 00000470: 7209 0000 0072 1300 0000 7207 0000 00da  r....r....r.....
 00000480: 0669 625f 7374 7272 1400 0000 da03 7374  .ib_strr......st
 00000490: 72da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  r..__annotations
 000004a0: 5f5f da04 6174 7472 da05 6669 656c 64da  __..attr..field.
 000004b0: 0276 73da 086f 7074 696f 6e61 6cda 0369  .vs..optional..i
 000004c0: 6e5f da09 746f 5f76 616c 7565 7372 1800  n_..to_valuesr..
 000004d0: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-000004e0: 1d00 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
+000004e0: 1c00 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
 000004f0: 0000 0072 1200 0000 720b 0000 0011 0000  ...r....r.......
 00000500: 0073 1200 0000 0a02 0404 1004 1001 0401  .s..............
 00000510: 1201 02fe 0e05 0201 720b 0000 0063 0000  ........r....c..
 00000520: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 00000530: 0000 4000 0000 7380 0000 0065 005a 0164  ..@...s....e.Z.d
 00000540: 005a 0264 015a 0364 025a 0464 035a 0564  .Z.d.Z.d.Z.d.Z.d
 00000550: 045a 0664 055a 0764 065a 0864 075a 0964  .Z.d.Z.d.Z.d.Z.d
@@ -125,82 +125,82 @@
 000007c0: 6669 6361 7469 6f6e da17 7365 6e64 5f6e  fication..send_n
 000007d0: 6f74 6966 6963 6174 696f 6e5f 7469 746c  otification_titl
 000007e0: 65da 1a73 656e 645f 6e6f 7469 6669 6361  e..send_notifica
 000007f0: 7469 6f6e 5f73 7562 7469 746c 65da 0e5f  tion_subtitle.._
 00000800: 6f70 656e 5f6c 6f67 5f66 696c 65da 135f  open_log_file.._
 00000810: 6f70 656e 5f6c 6f67 5f66 696c 655f 7061  open_log_file_pa
 00000820: 7468 4e29 2072 0e00 0000 720f 0000 0072  thN) r....r....r
-00000830: 1000 0000 721e 0000 0072 2a00 0000 722b  ....r....r*...r+
-00000840: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00000850: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00000860: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00000870: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00000880: 3800 0000 7239 0000 0072 3a00 0000 723b  8...r9...r:...r;
-00000890: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
-000008a0: 0000 723f 0000 0072 4000 0000 7241 0000  ..r?...r@...rA..
-000008b0: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
-000008c0: 7245 0000 0072 1100 0000 7211 0000 0072  rE...r....r....r
-000008d0: 1100 0000 7212 0000 0072 2900 0000 2900  ....r....r)...).
+00000830: 1000 0000 721d 0000 0072 2900 0000 722a  ....r....r)...r*
+00000840: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00000850: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
+00000860: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
+00000870: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+00000880: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
+00000890: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
+000008a0: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
+000008b0: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
+000008c0: 7244 0000 0072 1100 0000 7211 0000 0072  rD...r....r....r
+000008d0: 1100 0000 7212 0000 0072 2800 0000 2900  ....r....r(...).
 000008e0: 0000 733a 0000 0008 0104 0404 0104 0104  ..s:............
 000008f0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
 00000900: 0104 0104 0104 0104 0104 0104 0104 0104  ................
 00000910: 0104 0104 0104 0104 0104 0104 0104 0204  ................
-00000920: 0172 2900 0000 6300 0000 0000 0000 0000  .r)...c.........
+00000920: 0172 2800 0000 6300 0000 0000 0000 0000  .r(...c.........
 00000930: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
 00000940: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
 00000950: 6402 5a04 6403 5a05 6404 5300 2905 da0c  d.Z.d.Z.d.S.)...
 00000960: 5661 7256 616c 7565 456e 756d 7a3e 0a20  VarValueEnumz>. 
 00000970: 2020 204c 6973 7420 6f66 2061 7661 696c     List of avail
 00000980: 6162 6c65 2076 6172 6961 626c 6520 7661  able variable va
 00000990: 6c75 6573 2069 6e20 7468 6973 2066 7261  lues in this fra
 000009a0: 6d65 776f 726b 2e0a 2020 2020 da01 79da  mework..    ..y.
 000009b0: 016e 4e29 0672 0e00 0000 720f 0000 0072  .nN).r....r....r
-000009c0: 1000 0000 721e 0000 0072 4700 0000 7248  ....r....rG...rH
+000009c0: 1000 0000 721d 0000 0072 4600 0000 7247  ....r....rF...rG
 000009d0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-000009e0: 0000 7212 0000 0072 4600 0000 4d00 0000  ..r....rF...M...
-000009f0: 7306 0000 0008 0104 0404 0172 4600 0000  s..........rF...
+000009e0: 0000 7212 0000 0072 4500 0000 4d00 0000  ..r....rE...M...
+000009f0: 7306 0000 0008 0104 0404 0172 4500 0000  s..........rE...
 00000a00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000a10: 0003 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
 00000a20: 5a01 6400 5a02 5500 6401 5a03 6504 6a05  Z.d.Z.U.d.Z.e.j.
 00000a30: 6402 6403 8d01 5a06 6507 6508 6404 3c00  d.d...Z.e.e.d.<.
 00000a40: 6504 6a05 6402 6403 8d01 5a09 6507 6508  e.j.d.d...Z.e.e.
 00000a50: 6405 3c00 6402 5300 2906 da04 5465 7874  d.<.d.S.)...Text
 00000a60: 7a38 0a20 2020 2052 6570 7265 7365 6e74  z8.    Represent
 00000a70: 2061 2074 6578 7420 6f62 6a65 6374 2069   a text object i
 00000a80: 6e20 7363 7269 7074 2066 696c 7465 7220  n script filter 
 00000a90: 6974 656d 2e0a 2020 2020 4ea9 0172 1700  item..    N..r..
 00000aa0: 0000 da04 636f 7079 da09 6c61 7267 6574  ....copy..larget
 00000ab0: 7970 6529 0a72 0e00 0000 720f 0000 0072  ype).r....r....r
-00000ac0: 1000 0000 721e 0000 0072 0700 0000 721f  ....r....r....r.
-00000ad0: 0000 0072 4b00 0000 7220 0000 0072 2100  ...rK...r ...r!.
-00000ae0: 0000 724c 0000 0072 1100 0000 7211 0000  ..rL...r....r...
-00000af0: 0072 1100 0000 7212 0000 0072 4900 0000  .r....r....rI...
+00000ac0: 1000 0000 721d 0000 0072 0700 0000 721e  ....r....r....r.
+00000ad0: 0000 0072 4a00 0000 721f 0000 0072 2000  ...rJ...r....r .
+00000ae0: 0000 724b 0000 0072 1100 0000 7211 0000  ..rK...r....r...
+00000af0: 0072 1100 0000 7212 0000 0072 4800 0000  .r....r....rH...
 00000b00: 5600 0000 7306 0000 000a 0204 0414 0172  V...s..........r
-00000b10: 4900 0000 6300 0000 0000 0000 0000 0000  I...c...........
+00000b10: 4800 0000 6300 0000 0000 0000 0000 0000  H...c...........
 00000b20: 0000 0000 0001 0000 0040 0000 0073 2400  .........@...s$.
 00000b30: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
 00000b40: 5a04 6403 5a05 6404 5a06 6405 5a07 6406  Z.d.Z.d.Z.d.Z.d.
 00000b50: 5a08 6407 5300 2908 da07 4d6f 6445 6e75  Z.d.S.)...ModEnu
 00000b60: 6d7a 6e0a 2020 2020 4c69 7374 206f 6620  mzn.    List of 
 00000b70: 6176 6169 6c61 626c 6520 6d6f 6469 6669  available modifi
 00000b80: 6572 206b 6579 732e 2048 6974 2065 6e74  er keys. Hit ent
 00000b90: 6572 2077 6974 6820 7468 6520 6d6f 6469  er with the modi
 00000ba0: 6669 6572 206b 6579 2063 616e 206c 6561  fier key can lea
 00000bb0: 640a 2020 2020 746f 2064 6966 6665 7265  d.    to differe
 00000bc0: 6e74 2062 6568 6176 696f 722e 0a20 2020  nt behavior..   
 00000bd0: 20da 0363 6d64 da05 7368 6966 74da 0361   ..cmd..shift..a
 00000be0: 6c74 da04 6374 726c da02 666e 4e29 0972  lt..ctrl..fnN).r
-00000bf0: 0e00 0000 720f 0000 0072 1000 0000 721e  ....r....r....r.
-00000c00: 0000 0072 4e00 0000 724f 0000 0072 5000  ...rN...rO...rP.
-00000c10: 0000 7251 0000 0072 5200 0000 7211 0000  ..rQ...rR...r...
+00000bf0: 0e00 0000 720f 0000 0072 1000 0000 721d  ....r....r....r.
+00000c00: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
+00000c10: 0000 7250 0000 0072 5100 0000 7211 0000  ..rP...rQ...r...
 00000c20: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000c30: 724d 0000 0060 0000 0073 0c00 0000 0801  rM...`...s......
-00000c40: 0405 0401 0401 0401 0401 724d 0000 0063  ..........rM...c
+00000c30: 724c 0000 0060 0000 0073 0c00 0000 0801  rL...`...s......
+00000c40: 0405 0401 0401 0401 0401 724c 0000 0063  ..........rL...c
 00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c60: 0700 0000 4000 0000 7322 0200 0065 005a  ....@...s"...e.Z
+00000c60: 0700 0000 4000 0000 7336 0200 0065 005a  ....@...s6...e.Z
 00000c70: 0164 005a 0255 0064 015a 0347 0064 0264  .d.Z.U.d.Z.G.d.d
 00000c80: 0384 0064 0365 0483 035a 0565 06a0 07a1  ...d.e...Z.e....
 00000c90: 005a 0865 0965 0a64 043c 0065 066a 0764  .Z.e.e.d.<.e.j.d
 00000ca0: 0564 068d 015a 0b65 0965 0a64 073c 0065  .d...Z.e.e.d.<.e
 00000cb0: 066a 0764 0564 068d 015a 0c65 0965 0a64  .j.d.d...Z.e.e.d
 00000cc0: 083c 0065 066a 0764 0564 068d 015a 0d65  .<.e.j.d.d...Z.e
 00000cd0: 0965 0a64 093c 0065 0e6a 0f64 0564 068d  .e.d.<.e.j.d.d..
@@ -217,445 +217,447 @@
 00000d80: 0066 0319 0065 0a64 123c 0065 266a 0f64  .f...e.d.<.e&j.d
 00000d90: 0564 068d 015a 2765 2665 0a64 133c 0065  .d...Z'e&e.d.<.e
 00000da0: 066a 0764 0564 068d 015a 2865 0965 0a64  .j.d.d...Z(e.e.d
 00000db0: 143c 0065 066a 1d65 1f64 158d 015a 2965  .<.e.j.e.d...Z)e
 00000dc0: 1f65 0a64 163c 0065 0964 0064 179c 0264  .e.d.<.e.d.d...d
 00000dd0: 1864 1984 045a 2a65 2b6a 2c6a 2d64 0564  .d...Z*e+j,j-d.d
 00000de0: 0564 0b66 0465 0965 0b65 0965 1364 0064  .d.f.e.e.e.e.d.d
-00000df0: 1a9c 0564 1b64 1c84 055a 2e65 0964 1d9c  ...d.d...Z.e.d..
-00000e00: 0164 1e64 1f84 045a 2f65 0964 1d9c 0164  .d.d...Z/e.d...d
-00000e10: 2064 2184 045a 3065 0964 1d9c 0164 2264   d!..Z0e.d...d"d
-00000e20: 2384 045a 3165 0964 1d9c 0164 2464 2584  #..Z1e.d...d$d%.
-00000e30: 045a 3265 0964 1d9c 0164 2664 2784 045a  .Z2e.d...d&d'..Z
-00000e40: 3365 0964 1d9c 0164 2864 2984 045a 3465  3e.d...d(d)..Z4e
-00000e50: 0964 2a9c 0164 2b64 2c84 045a 3565 0964  .d*..d+d,..Z5e.d
-00000e60: 2d9c 0164 2e64 2f84 045a 3665 0964 2d9c  -..d.d/..Z6e.d-.
-00000e70: 0164 3064 3184 045a 3764 3665 0965 0964  .d0d1..Z7d6e.e.d
-00000e80: 339c 0264 3464 3584 055a 3864 0553 0029  3..d4d5..Z8d.S.)
-00000e90: 37da 0449 7465 6d61 0701 0000 0a20 2020  7..Itema.....   
-00000ea0: 2044 6174 6120 6d6f 6465 6c20 666f 7220   Data model for 
-00000eb0: 616c 6672 6564 2064 726f 7064 6f77 6e20  alfred dropdown 
-00000ec0: 6d65 6e75 2069 7465 6d73 2e0a 0a20 2020  menu items...   
-00000ed0: 202e 2e20 6e6f 7465 3a3a 0a0a 2020 2020   .. note::..    
-00000ee0: 2020 2020 506c 6561 7365 206d 616b 6520      Please make 
-00000ef0: 7375 7265 2074 6865 2061 7474 7269 6275  sure the attribu
-00000f00: 7465 206e 616d 6520 6973 2065 7861 6374  te name is exact
-00000f10: 6c79 2074 6865 2073 616d 6520 6173 2074  ly the same as t
-00000f20: 6865 2066 6965 6c64 206e 616d 650a 2020  he field name.  
-00000f30: 2020 2020 2020 696e 2074 6865 2066 6f6c        in the fol
-00000f40: 6c6f 7769 6e67 2064 6f63 756d 656e 742e  lowing document.
-00000f50: 0a0a 2020 2020 5265 663a 2068 7474 7073  ..    Ref: https
-00000f60: 3a2f 2f77 7777 2e61 6c66 7265 6461 7070  ://www.alfredapp
-00000f70: 2e63 6f6d 2f68 656c 702f 776f 726b 666c  .com/help/workfl
-00000f80: 6f77 732f 696e 7075 7473 2f73 6372 6970  ows/inputs/scrip
-00000f90: 742d 6669 6c74 6572 2f6a 736f 6e2f 0a20  t-filter/json/. 
-00000fa0: 2020 2063 0000 0000 0000 0000 0000 0000     c............
-00000fb0: 0000 0000 0100 0000 4000 0000 7314 0000  ........@...s...
-00000fc0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00000fd0: 0464 0353 0029 047a 0d49 7465 6d2e 5479  .d.S.).z.Item.Ty
-00000fe0: 7065 456e 756d da04 6669 6c65 7a0e 6669  peEnum..filez.fi
-00000ff0: 6c65 3a73 6b69 7063 6865 636b 4e29 0572  le:skipcheckN).r
-00001000: 0e00 0000 720f 0000 0072 1000 0000 7254  ....r....r....rT
-00001010: 0000 005a 0e66 696c 655f 736b 6970 6368  ...Z.file_skipch
-00001020: 6563 6b72 1100 0000 7211 0000 0072 1100  eckr....r....r..
-00001030: 0000 7212 0000 0072 1300 0000 7a00 0000  ..r....r....z...
-00001040: 7304 0000 0008 0104 0172 1300 0000 da05  s........r......
-00001050: 7469 746c 654e 724a 0000 00da 0873 7562  titleNrJ.....sub
-00001060: 7469 746c 65da 0361 7267 da0c 6175 746f  title..arg..auto
-00001070: 636f 6d70 6c65 7465 da04 6963 6f6e 54da  complete..iconT.
-00001080: 0576 616c 6964 da03 7569 64da 056d 6174  .valid..uid..mat
-00001090: 6368 7215 0000 0072 1800 0000 da04 6d6f  chr....r......mo
-000010a0: 6473 da06 6163 7469 6f6e da04 7465 7874  ds..action..text
-000010b0: da0c 7175 6963 6b6c 6f6f 6b75 726c 2901  ..quicklookurl).
-000010c0: da07 6661 6374 6f72 79da 0976 6172 6961  ..factory..varia
-000010d0: 626c 6573 7219 0000 0063 0200 0000 0000  blesr....c......
-000010e0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-000010f0: 0000 7310 0000 0074 00a0 017c 01a1 017c  ..s....t...|...|
-00001100: 005f 027c 0053 0029 017a 240a 2020 2020  ._.|.S.).z$.    
-00001110: 2020 2020 5365 7420 6963 6f6e 2066 6f72      Set icon for
-00001120: 2069 7465 6d2e 0a20 2020 2020 2020 2029   item..        )
-00001130: 0372 0b00 0000 721d 0000 0072 5900 0000  .r....r....rY...
-00001140: a902 da04 7365 6c66 7214 0000 0072 1100  ....selfr....r..
-00001150: 0000 7211 0000 0072 1200 0000 da08 7365  ..r....r......se
-00001160: 745f 6963 6f6e 9300 0000 7304 0000 0000  t_icon....s.....
-00001170: 040c 017a 0d49 7465 6d2e 7365 745f 6963  ...z.Item.set_ic
-00001180: 6f6e 2905 da03 6d6f 6472 5600 0000 7257  on)...modrV...rW
-00001190: 0000 0072 5a00 0000 721a 0000 0063 0500  ...rZ...r....c..
-000011a0: 0000 0000 0000 0000 0000 0600 0000 0600  ................
-000011b0: 0000 4300 0000 734c 0000 007c 0174 00a0  ..C...sL...|.t..
-000011c0: 01a1 006b 0772 1074 0282 0164 0164 0284  ...k.r.t...d.d..
-000011d0: 0074 037c 027c 037c 0464 038d 03a0 04a1  .t.|.|.|.d......
-000011e0: 0044 0083 017d 057c 006a 0564 046b 0872  .D...}.|.j.d.k.r
-000011f0: 3e74 0383 007c 005f 057c 057c 006a 057c  >t...|._.|.|.j.|
-00001200: 013c 007c 0053 0029 0561 8501 0000 0a20  .<.|.S.).a..... 
-00001210: 2020 2020 2020 2041 6464 206d 6f64 6966         Add modif
-00001220: 6965 7220 746f 2069 7465 6d2e 204d 6f64  ier to item. Mod
-00001230: 6966 6965 7220 616c 6c6f 7720 796f 7520  ifier allow you 
-00001240: 746f 2072 6574 7572 6e20 6469 6666 6572  to return differ
-00001250: 656e 7420 7469 746c 652c 0a20 2020 2020  ent title,.     
-00001260: 2020 2073 7562 7469 746c 6520 616e 6420     subtitle and 
-00001270: 6172 6775 6d65 6e74 2069 6e20 416c 6672  argument in Alfr
-00001280: 6564 2064 726f 7020 646f 776e 206d 656e  ed drop down men
-00001290: 7520 6974 656d 2077 6865 6e20 796f 7520  u item when you 
-000012a0: 6869 7420 610a 2020 2020 2020 2020 6d6f  hit a.        mo
-000012b0: 6469 6669 6572 206b 6579 2e0a 0a20 2020  difier key...   
-000012c0: 2020 2020 203a 7061 7261 6d20 6d6f 6465       :param mode
-000012d0: 3a20 7468 6520 6d6f 6469 6669 6572 206b  : the modifier k
-000012e0: 6579 0a20 2020 2020 2020 203a 7061 7261  ey.        :para
-000012f0: 6d20 7375 6274 6974 6c65 3a20 7468 6520  m subtitle: the 
-00001300: 7375 6274 6974 6c65 2079 6f75 2077 616e  subtitle you wan
-00001310: 7420 746f 2064 6973 706c 6179 0a20 2020  t to display.   
-00001320: 2020 2020 203a 7061 7261 6d20 6172 673a       :param arg:
-00001330: 2074 6865 2061 7267 756d 656e 7420 7061   the argument pa
-00001340: 7373 6564 2074 6f20 7375 6273 6571 7565  ssed to subseque
-00001350: 6e63 6520 6163 7469 6f6e 0a20 2020 2020  nce action.     
-00001360: 2020 203a 7061 7261 6d20 7661 6c69 643a     :param valid:
-00001370: 2077 6865 7468 6572 2074 6865 2069 7465   whether the ite
-00001380: 6d20 6973 2076 616c 6964 0a20 2020 2020  m is valid.     
-00001390: 2020 2063 0100 0000 0000 0000 0000 0000     c............
-000013a0: 0300 0000 0400 0000 5300 0000 731a 0000  ........S...s...
-000013b0: 0069 007c 005d 125c 027d 017d 027c 0272  .i.|.].\.}.}.|.r
-000013c0: 047c 017c 0293 0271 0453 0072 1100 0000  .|.|...q.S.r....
-000013d0: 7211 0000 0029 03da 022e 30da 016b da01  r....)....0..k..
-000013e0: 7672 1100 0000 7211 0000 0072 1200 0000  vr....r....r....
-000013f0: da0a 3c64 6963 7463 6f6d 703e ad00 0000  ..<dictcomp>....
-00001400: 7308 0000 0006 0206 0504 fa02 007a 2549  s............z%I
-00001410: 7465 6d2e 7365 745f 6d6f 6469 6669 6572  tem.set_modifier
-00001420: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00001430: 6f6d 703e 2903 7256 0000 0072 5700 0000  omp>).rV...rW...
-00001440: 725a 0000 004e 2906 724d 0000 0072 2700  rZ...N).rM...r'.
-00001450: 0000 da0a 5661 6c75 6545 7272 6f72 da04  ....ValueError..
-00001460: 6469 6374 da05 6974 656d 7372 5d00 0000  dict..itemsr]...
-00001470: 2906 7264 0000 0072 6600 0000 7256 0000  ).rd...rf...rV..
-00001480: 0072 5700 0000 725a 0000 00da 0364 6374  .rW...rZ.....dct
-00001490: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-000014a0: 0c73 6574 5f6d 6f64 6966 6965 729a 0000  .set_modifier...
-000014b0: 0073 1a00 0000 0011 0c01 0401 0602 0201  .s..............
-000014c0: 0201 0201 02fd 08fe 0609 0a01 0801 0a01  ................
-000014d0: 7a11 4974 656d 2e73 6574 5f6d 6f64 6966  z.Item.set_modif
-000014e0: 6965 7272 1b00 0000 6302 0000 0000 0000  ierr....c.......
-000014f0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001500: 0073 2400 0000 7400 6a01 6a02 7c00 6a03  .s$...t.j.j.|.j.
-00001510: 7404 6a05 6a02 3c00 7c01 7c00 6a03 7404  t.j.j.<.|.|.j.t.
-00001520: 6a06 6a02 3c00 6401 5300 2902 7aa2 0a20  j.j.<.d.S.).z.. 
-00001530: 2020 2020 2020 2054 6869 7320 6973 2061         This is a
-00001540: 2073 7065 6369 616c 2076 6172 6961 626c   special variabl
-00001550: 6520 7468 6174 2077 696c 6c20 6f70 656e  e that will open
-00001560: 2074 6865 206c 6173 7420 6572 726f 7220   the last error 
-00001570: 6669 6c65 2069 6e20 7468 6520 6564 6974  file in the edit
-00001580: 6f72 2e0a 2020 2020 2020 2020 4974 2069  or..        It i
-00001590: 7320 666f 7220 696e 7465 726e 616c 2069  s for internal i
-000015a0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f6e  mplementation on
-000015b0: 6c79 2c20 6e6f 7420 666f 7220 7075 626c  ly, not for publ
-000015c0: 6963 2041 5049 2e0a 2020 2020 2020 2020  ic API..        
-000015d0: 4e29 0772 4600 0000 7247 0000 00da 0576  N).rF...rG.....v
-000015e0: 616c 7565 7262 0000 0072 2900 0000 7244  aluerb...r)...rD
-000015f0: 0000 0072 4500 0000 7263 0000 0072 1100  ...rE...rc...r..
-00001600: 0000 7211 0000 0072 1200 0000 7244 0000  ..r....r....rD..
-00001610: 00be 0000 0073 0400 0000 0005 1201 7a13  .....s........z.
-00001620: 4974 656d 2e5f 6f70 656e 5f6c 6f67 5f66  Item._open_log_f
-00001630: 696c 6563 0200 0000 0000 0000 0000 0000  ilec............
-00001640: 0200 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-00001650: 0074 006a 016a 027c 006a 0374 046a 056a  .t.j.j.|.j.t.j.j
-00001660: 023c 007c 017c 006a 0374 046a 066a 023c  .<.|.|.j.t.j.j.<
-00001670: 0064 0153 0029 0261 1401 0000 0a20 2020  .d.S.).a.....   
-00001680: 2020 2020 2053 6574 2076 6172 6961 626c       Set variabl
-00001690: 6573 2074 6f20 7465 6c6c 2073 7562 7365  es to tell subse
-000016a0: 7175 656e 6365 2041 6c66 7265 6420 6163  quence Alfred ac
-000016b0: 7469 6f6e 2074 6f20 6f70 656e 2061 2066  tion to open a f
-000016c0: 696c 652e 0a0a 2020 2020 2020 2020 5573  ile...        Us
-000016d0: 6520 7468 6520 2255 7469 6c69 7469 6573  e the "Utilities
-000016e0: 202d 3e20 436f 6e64 6974 696f 6e61 6c22   -> Conditional"
-000016f0: 2077 6964 6765 7420 616e 6420 7365 743a   widget and set:
-00001700: 2069 6620 6060 7b76 6172 3a6f 7065 6e5f   if ``{var:open_
-00001710: 6669 6c65 7d60 600a 2020 2020 2020 2020  file}``.        
-00001720: 6973 2065 7175 616c 2074 6f20 2279 222e  is equal to "y".
-00001730: 0a0a 2020 2020 2020 2020 5573 6520 7468  ..        Use th
-00001740: 6520 2241 6374 696f 6e73 202d 3e20 4f70  e "Actions -> Op
-00001750: 656e 2046 696c 6522 2077 6964 6765 7420  en File" widget 
-00001760: 616e 6420 7365 743a 2046 696c 653a 2060  and set: File: `
-00001770: 607b 7661 723a 6f70 656e 5f66 696c 655f  `{var:open_file_
-00001780: 7061 7468 7d60 600a 2020 2020 2020 2020  path}``.        
-00001790: 4e29 0772 4600 0000 7247 0000 0072 7000  N).rF...rG...rp.
-000017a0: 0000 7262 0000 0072 2900 0000 722a 0000  ..rb...r)...r*..
-000017b0: 0072 2b00 0000 7263 0000 0072 1100 0000  .r+...rc...r....
-000017c0: 7211 0000 0072 1200 0000 722a 0000 00c6  r....r....r*....
-000017d0: 0000 0073 0400 0000 0009 1201 7a0e 4974  ...s........z.It
-000017e0: 656d 2e6f 7065 6e5f 6669 6c65 6302 0000  em.open_filec...
-000017f0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001800: 0043 0000 0073 2400 0000 7400 6a01 6a02  .C...s$...t.j.j.
-00001810: 7c00 6a03 7404 6a05 6a02 3c00 7c01 7c00  |.j.t.j.j.<.|.|.
-00001820: 6a03 7404 6a06 6a02 3c00 6401 5300 2902  j.t.j.j.<.d.S.).
-00001830: 610a 0100 000a 2020 2020 2020 2020 5365  a.....        Se
-00001840: 7420 7661 7269 6162 6c65 7320 746f 2074  t variables to t
-00001850: 656c 6c20 7375 6273 6571 7565 6e63 6520  ell subsequence 
-00001860: 416c 6672 6564 2061 6374 696f 6e20 746f  Alfred action to
-00001870: 206c 6175 6e63 6820 616e 2061 7070 206f   launch an app o
-00001880: 7220 6669 6c65 2e0a 0a20 2020 2020 2020  r file...       
-00001890: 2055 7365 2074 6865 2022 5574 696c 6974   Use the "Utilit
-000018a0: 6965 7320 2d3e 2043 6f6e 6469 7469 6f6e  ies -> Condition
-000018b0: 616c 2220 7769 6467 6574 2061 6e64 2073  al" widget and s
-000018c0: 6574 3a20 6966 2060 607b 7661 723a 6c61  et: if ``{var:la
-000018d0: 756e 6368 5f61 7070 5f6f 725f 6669 6c65  unch_app_or_file
-000018e0: 7d60 600a 2020 2020 2020 2020 6973 2065  }``.        is e
-000018f0: 7175 616c 2074 6f20 2279 222e 0a0a 2020  qual to "y"...  
-00001900: 2020 2020 2020 5573 6520 7468 6520 2241        Use the "A
-00001910: 6374 696f 6e73 202d 3e20 4c61 756e 6368  ctions -> Launch
-00001920: 2041 7070 7320 2f20 4669 6c65 7322 2077   Apps / Files" w
-00001930: 6964 6765 742e 0a20 2020 2020 2020 204e  idget..        N
-00001940: 2907 7246 0000 0072 4700 0000 7270 0000  ).rF...rG...rp..
-00001950: 0072 6200 0000 7229 0000 0072 2c00 0000  .rb...r)...r,...
-00001960: 722d 0000 0072 6300 0000 7211 0000 0072  r-...rc...r....r
-00001970: 1100 0000 7212 0000 0072 2c00 0000 d200  ....r....r,.....
-00001980: 0000 7304 0000 0000 0912 017a 1749 7465  ..s........z.Ite
-00001990: 6d2e 6c61 756e 6368 5f61 7070 5f6f 725f  m.launch_app_or_
-000019a0: 6669 6c65 6302 0000 0000 0000 0000 0000  filec...........
-000019b0: 0002 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
-000019c0: 0000 7400 6a01 6a02 7c00 6a03 7404 6a05  ..t.j.j.|.j.t.j.
-000019d0: 6a02 3c00 7c01 7c00 6a03 7404 6a06 6a02  j.<.|.|.j.t.j.j.
-000019e0: 3c00 6401 5300 2902 610f 0100 000a 2020  <.d.S.).a.....  
-000019f0: 2020 2020 2020 5365 7420 7661 7269 6162        Set variab
-00001a00: 6c65 7320 746f 2074 656c 6c20 7375 6273  les to tell subs
-00001a10: 6571 7565 6e63 6520 416c 6672 6564 2061  equence Alfred a
-00001a20: 6374 696f 6e20 746f 206c 6175 6e63 6820  ction to launch 
-00001a30: 616e 2061 7070 206f 7220 6669 6c65 2e0a  an app or file..
-00001a40: 0a20 2020 2020 2020 2055 7365 2074 6865  .        Use the
-00001a50: 2022 5574 696c 6974 6965 7320 2d3e 2043   "Utilities -> C
-00001a60: 6f6e 6469 7469 6f6e 616c 2220 7769 6467  onditional" widg
-00001a70: 6574 2061 6e64 2073 6574 3a20 6966 2060  et and set: if `
-00001a80: 607b 7661 723a 7265 7665 616c 5f66 696c  `{var:reveal_fil
-00001a90: 655f 696e 5f66 696e 6465 727d 6060 0a20  e_in_finder}``. 
-00001aa0: 2020 2020 2020 2069 7320 6571 7561 6c20         is equal 
-00001ab0: 746f 2022 7922 2e0a 0a20 2020 2020 2020  to "y"...       
-00001ac0: 2055 7365 2074 6865 2022 4163 7469 6f6e   Use the "Action
-00001ad0: 7320 2d3e 2052 6576 6561 6c20 4669 6c65  s -> Reveal File
-00001ae0: 2069 6e20 4669 6e64 6572 2220 7769 6467   in Finder" widg
-00001af0: 6574 2e0a 2020 2020 2020 2020 4e29 0772  et..        N).r
-00001b00: 4600 0000 7247 0000 0072 7000 0000 7262  F...rG...rp...rb
-00001b10: 0000 0072 2900 0000 722e 0000 0072 2f00  ...r)...r....r/.
-00001b20: 0000 7263 0000 0072 1100 0000 7211 0000  ..rc...r....r...
-00001b30: 0072 1200 0000 722e 0000 00de 0000 0073  .r....r........s
-00001b40: 0400 0000 0009 1201 7a1a 4974 656d 2e72  ........z.Item.r
-00001b50: 6576 6561 6c5f 6669 6c65 5f69 6e5f 6669  eveal_file_in_fi
-00001b60: 6e64 6572 6302 0000 0000 0000 0000 0000  nderc...........
-00001b70: 0002 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
-00001b80: 0000 7400 6a01 6a02 7c00 6a03 7404 6a05  ..t.j.j.|.j.t.j.
-00001b90: 6a02 3c00 7c01 7c00 6a03 7404 6a06 6a02  j.<.|.|.j.t.j.j.
-00001ba0: 3c00 6401 5300 2902 6106 0100 000a 2020  <.d.S.).a.....  
-00001bb0: 2020 2020 2020 5365 7420 7661 7269 6162        Set variab
-00001bc0: 6c65 7320 746f 2074 656c 6c20 7375 6273  les to tell subs
-00001bd0: 6571 7565 6e63 6520 416c 6672 6564 2061  equence Alfred a
-00001be0: 6374 696f 6e20 746f 2062 726f 7773 6520  ction to browse 
-00001bf0: 696e 2074 6572 6d69 6e61 6c2e 0a0a 2020  in terminal...  
-00001c00: 2020 2020 2020 5573 6520 7468 6520 2255        Use the "U
-00001c10: 7469 6c69 7469 6573 202d 3e20 436f 6e64  tilities -> Cond
-00001c20: 6974 696f 6e61 6c22 2077 6964 6765 7420  itional" widget 
-00001c30: 616e 6420 7365 743a 2069 6620 6060 7b76  and set: if ``{v
-00001c40: 6172 3a62 726f 7773 655f 696e 5f74 6572  ar:browse_in_ter
-00001c50: 6d69 6e61 6c7d 6060 0a20 2020 2020 2020  minal}``.       
-00001c60: 2069 7320 6571 7561 6c20 746f 2022 7922   is equal to "y"
-00001c70: 2e0a 0a20 2020 2020 2020 2055 7365 2074  ...        Use t
-00001c80: 6865 2022 4163 7469 6f6e 7320 2d3e 2042  he "Actions -> B
-00001c90: 726f 7773 6520 696e 2054 6572 6d69 6e61  rowse in Termina
-00001ca0: 6c22 2077 6964 6765 742e 0a20 2020 2020  l" widget..     
-00001cb0: 2020 204e 2907 7246 0000 0072 4700 0000     N).rF...rG...
-00001cc0: 7270 0000 0072 6200 0000 7229 0000 0072  rp...rb...r)...r
-00001cd0: 3000 0000 7231 0000 0072 6300 0000 7211  0...r1...rc...r.
-00001ce0: 0000 0072 1100 0000 7212 0000 0072 3000  ...r....r....r0.
-00001cf0: 0000 ea00 0000 7304 0000 0000 0912 017a  ......s........z
-00001d00: 1749 7465 6d2e 6272 6f77 7365 5f69 6e5f  .Item.browse_in_
-00001d10: 7465 726d 696e 616c 6302 0000 0000 0000  terminalc.......
-00001d20: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001d30: 0073 2400 0000 7400 6a01 6a02 7c00 6a03  .s$...t.j.j.|.j.
-00001d40: 7404 6a05 6a02 3c00 7c01 7c00 6a03 7404  t.j.j.<.|.|.j.t.
-00001d50: 6a06 6a02 3c00 6401 5300 2902 6100 0100  j.j.<.d.S.).a...
-00001d60: 000a 2020 2020 2020 2020 5365 7420 7661  ..        Set va
-00001d70: 7269 6162 6c65 7320 746f 2074 656c 6c20  riables to tell 
-00001d80: 7375 6273 6571 7565 6e63 6520 416c 6672  subsequence Alfr
-00001d90: 6564 2061 6374 696f 6e20 746f 2062 726f  ed action to bro
-00001da0: 7773 6520 696e 2041 6c66 7265 642e 0a0a  wse in Alfred...
-00001db0: 2020 2020 2020 2020 5573 6520 7468 6520          Use the 
-00001dc0: 2255 7469 6c69 7469 6573 202d 3e20 436f  "Utilities -> Co
-00001dd0: 6e64 6974 696f 6e61 6c22 2077 6964 6765  nditional" widge
-00001de0: 7420 616e 6420 7365 743a 2069 6620 6060  t and set: if ``
-00001df0: 7b76 6172 3a62 726f 7773 655f 696e 5f61  {var:browse_in_a
-00001e00: 6c66 7265 647d 6060 0a20 2020 2020 2020  lfred}``.       
-00001e10: 2069 7320 6571 7561 6c20 746f 2022 7922   is equal to "y"
-00001e20: 2e0a 0a20 2020 2020 2020 2055 7365 2074  ...        Use t
-00001e30: 6865 2022 4163 7469 6f6e 7320 2d3e 2042  he "Actions -> B
-00001e40: 726f 7773 6520 696e 2041 6c66 7265 6422  rowse in Alfred"
-00001e50: 2077 6964 6765 742e 0a20 2020 2020 2020   widget..       
-00001e60: 204e 2907 7246 0000 0072 4700 0000 7270   N).rF...rG...rp
-00001e70: 0000 0072 6200 0000 7229 0000 0072 3200  ...rb...r)...r2.
-00001e80: 0000 7233 0000 0072 6300 0000 7211 0000  ..r3...rc...r...
-00001e90: 0072 1100 0000 7212 0000 0072 3200 0000  .r....r....r2...
-00001ea0: f600 0000 7304 0000 0000 0912 017a 1549  ....s........z.I
-00001eb0: 7465 6d2e 6272 6f77 7365 5f69 6e5f 616c  tem.browse_in_al
-00001ec0: 6672 6564 2901 da03 7572 6c63 0200 0000  fred)...urlc....
-00001ed0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001ee0: 4300 0000 7324 0000 0074 006a 016a 027c  C...s$...t.j.j.|
-00001ef0: 006a 0374 046a 056a 023c 007c 017c 006a  .j.t.j.j.<.|.|.j
-00001f00: 0374 046a 066a 023c 0064 0153 0029 0261  .t.j.j.<.d.S.).a
-00001f10: 1901 0000 0a20 2020 2020 2020 2053 6574  .....        Set
-00001f20: 2076 6172 6961 626c 6573 2074 6f20 7465   variables to te
-00001f30: 6c6c 2073 7562 7365 7175 656e 6365 2041  ll subsequence A
-00001f40: 6c66 7265 6420 6163 7469 6f6e 2074 6f20  lfred action to 
-00001f50: 6f70 656e 2075 726c 2e0a 0a20 2020 2020  open url...     
-00001f60: 2020 2055 7365 2074 6865 2022 5574 696c     Use the "Util
-00001f70: 6974 6965 7320 2d3e 2043 6f6e 6469 7469  ities -> Conditi
-00001f80: 6f6e 616c 2220 7769 6467 6574 2061 6e64  onal" widget and
-00001f90: 2073 6574 3a20 6966 2060 607b 7661 723a   set: if ``{var:
-00001fa0: 6f70 656e 5f75 726c 7d60 600a 2020 2020  open_url}``.    
-00001fb0: 2020 2020 6973 2065 7175 616c 2074 6f20      is equal to 
-00001fc0: 2279 222e 0a0a 2020 2020 2020 2020 5573  "y"...        Us
-00001fd0: 6520 7468 6520 2241 6374 696f 6e73 202d  e the "Actions -
-00001fe0: 3e20 4f70 656e 2055 524c 2220 7769 6467  > Open URL" widg
-00001ff0: 6574 2061 6e64 2073 6574 3a0a 0a20 2020  et and set:..   
-00002000: 2020 2020 202d 2046 696c 6520 3d20 6060       - File = ``
-00002010: 7b76 6172 3a6f 7065 6e5f 7572 6c5f 6172  {var:open_url_ar
-00002020: 677d 6060 0a20 2020 2020 2020 204e 2907  g}``.        N).
-00002030: 7246 0000 0072 4700 0000 7270 0000 0072  rF...rG...rp...r
-00002040: 6200 0000 7229 0000 0072 3700 0000 7238  b...r)...r7...r8
-00002050: 0000 0029 0272 6400 0000 7271 0000 0072  ...).rd...rq...r
-00002060: 1100 0000 7211 0000 0072 1200 0000 7237  ....r....r....r7
-00002070: 0000 0002 0100 0073 0400 0000 000b 1201  .......s........
-00002080: 7a0d 4974 656d 2e6f 7065 6e5f 7572 6c29  z.Item.open_url)
-00002090: 0172 4e00 0000 6302 0000 0000 0000 0000  .rN...c.........
-000020a0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-000020b0: 2a00 0000 7400 6a01 6a02 7c00 6a03 7404  *...t.j.j.|.j.t.
-000020c0: 6a05 6a02 3c00 7c01 7c00 6a03 7404 6a06  j.j.<.|.|.j.t.j.
-000020d0: 6a02 3c00 7c01 7c00 5f07 6401 5300 2902  j.<.|.|._.d.S.).
-000020e0: 6188 0100 000a 2020 2020 2020 2020 5365  a.....        Se
-000020f0: 7420 7661 7269 6162 6c65 7320 746f 2074  t variables to t
-00002100: 656c 6c20 7375 6273 6571 7565 6e63 6520  ell subsequence 
-00002110: 416c 6672 6564 2061 6374 696f 6e20 746f  Alfred action to
-00002120: 2072 756e 2073 6372 6970 742e 0a0a 2020   run script...  
-00002130: 2020 2020 2020 5573 6520 7468 6520 2255        Use the "U
-00002140: 7469 6c69 7469 6573 202d 3e20 436f 6e64  tilities -> Cond
-00002150: 6974 696f 6e61 6c22 2077 6964 6765 7420  itional" widget 
-00002160: 616e 6420 7365 743a 2069 6620 6060 7b76  and set: if ``{v
-00002170: 6172 3a72 756e 5f73 6372 6970 747d 6060  ar:run_script}``
-00002180: 0a20 2020 2020 2020 2069 7320 6571 7561  .        is equa
-00002190: 6c20 746f 2022 7922 2e0a 0a20 2020 2020  l to "y"...     
-000021a0: 2020 2055 7365 2074 6865 2022 4163 7469     Use the "Acti
-000021b0: 6f6e 7320 2d3e 2052 756e 2053 6372 6970  ons -> Run Scrip
-000021c0: 7422 2077 6964 6765 7420 616e 6420 7365  t" widget and se
-000021d0: 743a 0a0a 2020 2020 2020 2020 2d20 4c61  t:..        - La
-000021e0: 6e67 7561 6765 203d 2060 602f 6269 6e2f  nguage = ``/bin/
-000021f0: 6261 7368 6060 0a20 2020 2020 2020 202d  bash``.        -
-00002200: 2022 7769 7468 2069 6e70 7574 2061 7320   "with input as 
-00002210: 7b71 7565 7279 7d22 0a20 2020 2020 2020  {query}".       
-00002220: 202d 2072 756e 6e69 6e67 2069 6e73 7461   - running insta
-00002230: 6e63 6573 203d 2022 5365 7175 656e 7469  nces = "Sequenti
-00002240: 616c 6c79 220a 2020 2020 2020 2020 2d20  ally".        - 
-00002250: 5363 7269 7074 203d 2060 607b 7175 6572  Script = ``{quer
-00002260: 797d 6060 0a20 2020 2020 2020 204e 2908  y}``.        N).
-00002270: 7246 0000 0072 4700 0000 7270 0000 0072  rF...rG...rp...r
-00002280: 6200 0000 7229 0000 0072 3b00 0000 723c  b...r)...r;...r<
-00002290: 0000 0072 5700 0000 a902 7264 0000 0072  ...rW.....rd...r
-000022a0: 4e00 0000 7211 0000 0072 1100 0000 7212  N...r....r....r.
-000022b0: 0000 0072 3b00 0000 1001 0000 7306 0000  ...r;.......s...
-000022c0: 0000 0e12 010e 017a 0f49 7465 6d2e 7275  .......z.Item.ru
-000022d0: 6e5f 7363 7269 7074 6302 0000 0000 0000  n_scriptc.......
-000022e0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-000022f0: 0073 2a00 0000 7400 6a01 6a02 7c00 6a03  .s*...t.j.j.|.j.
-00002300: 7404 6a05 6a02 3c00 7c01 7c00 6a03 7404  t.j.j.<.|.|.j.t.
-00002310: 6a06 6a02 3c00 7c01 7c00 5f07 6401 5300  j.j.<.|.|._.d.S.
-00002320: 2902 7adb 0a20 2020 2020 2020 2055 7365  ).z..        Use
-00002330: 2074 6865 2022 5574 696c 6974 6965 7320   the "Utilities 
-00002340: 2d3e 2043 6f6e 6469 7469 6f6e 616c 2220  -> Conditional" 
-00002350: 7769 6467 6574 2061 6e64 2073 6574 3a20  widget and set: 
-00002360: 6966 2060 607b 7661 723a 7465 726d 696e  if ``{var:termin
-00002370: 616c 5f63 6f6d 6d61 6e64 7d60 600a 2020  al_command}``.  
-00002380: 2020 2020 2020 6973 2065 7175 616c 2074        is equal t
-00002390: 6f20 2279 222e 0a0a 2020 2020 2020 2020  o "y"...        
-000023a0: 5573 6520 7468 6520 2241 6374 696f 6e73  Use the "Actions
-000023b0: 202d 3e20 5465 726d 696e 616c 2043 6f6d   -> Terminal Com
-000023c0: 6d61 6e64 2220 7769 6467 6574 2061 6e64  mand" widget and
-000023d0: 2073 6574 3a0a 0a20 2020 2020 2020 202d   set:..        -
-000023e0: 2043 6f6d 6d61 6e64 203d 2060 607b 7175   Command = ``{qu
-000023f0: 6572 797d 6060 0a20 2020 2020 2020 204e  ery}``.        N
-00002400: 2908 7246 0000 0072 4700 0000 7270 0000  ).rF...rG...rp..
-00002410: 0072 6200 0000 7229 0000 0072 3f00 0000  .rb...r)...r?...
-00002420: 7240 0000 0072 5700 0000 7272 0000 0072  r@...rW...rr...r
-00002430: 1100 0000 7211 0000 0072 1200 0000 723f  ....r....r....r?
-00002440: 0000 0022 0100 0073 0600 0000 0009 1201  ..."...s........
-00002450: 0e01 7a15 4974 656d 2e74 6572 6d69 6e61  ..z.Item.termina
-00002460: 6c5f 636f 6d6d 616e 64da 0029 0272 5500  l_command..).rU.
-00002470: 0000 7256 0000 0063 0300 0000 0000 0000  ..rV...c........
-00002480: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-00002490: 7332 0000 0074 006a 016a 027c 006a 0374  s2...t.j.j.|.j.t
-000024a0: 046a 056a 023c 007c 017c 006a 0374 046a  .j.j.<.|.|.j.t.j
-000024b0: 066a 023c 007c 027c 006a 0374 046a 076a  .j.<.|.|.j.t.j.j
-000024c0: 023c 0064 0153 0029 0261 7a01 0000 0a20  .<.d.S.).az.... 
-000024d0: 2020 2020 2020 2053 6574 2076 6172 6961         Set varia
-000024e0: 626c 6573 2074 6f20 7465 6c6c 2073 7562  bles to tell sub
-000024f0: 7365 7175 656e 6365 2041 6c66 7265 6420  sequence Alfred 
-00002500: 6163 7469 6f6e 2074 6f20 7365 6e64 206e  action to send n
-00002510: 6f74 6966 6963 6174 696f 6e2e 0a0a 2020  otification...  
-00002520: 2020 2020 2020 5573 6520 7468 6520 2255        Use the "U
-00002530: 7469 6c69 7469 6573 202d 3e20 436f 6e64  tilities -> Cond
-00002540: 6974 696f 6e61 6c22 2077 6964 6765 7420  itional" widget 
-00002550: 616e 6420 7365 743a 2069 6620 6060 7b76  and set: if ``{v
-00002560: 6172 3a73 656e 645f 6e6f 7469 6669 6361  ar:send_notifica
-00002570: 7469 6f6e 7d60 600a 2020 2020 2020 2020  tion}``.        
-00002580: 6973 2065 7175 616c 2074 6f20 2279 222e  is equal to "y".
-00002590: 0a0a 2020 2020 2020 2020 5573 6520 7468  ..        Use th
-000025a0: 6520 224f 7574 7075 7473 202d 3e20 506f  e "Outputs -> Po
-000025b0: 7374 204e 6f74 6966 6963 6174 696f 6e22  st Notification"
-000025c0: 2077 6964 6765 7420 616e 6420 7365 743a   widget and set:
-000025d0: 0a0a 2020 2020 2020 2020 2d20 5469 746c  ..        - Titl
-000025e0: 6520 3d20 6060 7b76 6172 3a73 656e 645f  e = ``{var:send_
-000025f0: 6e6f 7469 6669 6361 7469 6f6e 5f74 6974  notification_tit
-00002600: 6c65 7d60 600a 2020 2020 2020 2020 2d20  le}``.        - 
-00002610: 5375 6274 6974 6c65 203d 2060 607b 7661  Subtitle = ``{va
-00002620: 723a 7365 6e64 5f6e 6f74 6966 6963 6174  r:send_notificat
-00002630: 696f 6e5f 7375 6274 6974 6c65 7d60 600a  ion_subtitle}``.
-00002640: 2020 2020 2020 2020 4e29 0872 4600 0000          N).rF...
-00002650: 7247 0000 0072 7000 0000 7262 0000 0072  rG...rp...rb...r
-00002660: 2900 0000 7241 0000 0072 4200 0000 7243  )...rA...rB...rC
-00002670: 0000 0029 0372 6400 0000 7255 0000 0072  ...).rd...rU...r
-00002680: 5600 0000 7211 0000 0072 1100 0000 7212  V...r....r....r.
-00002690: 0000 0072 4100 0000 2f01 0000 7306 0000  ...rA.../...s...
-000026a0: 0000 0c12 010e 017a 1649 7465 6d2e 7365  .......z.Item.se
-000026b0: 6e64 5f6e 6f74 6966 6963 6174 696f 6e29  nd_notification)
-000026c0: 0172 7300 0000 2939 720e 0000 0072 0f00  .rs...)9r....r..
-000026d0: 0000 7210 0000 0072 1e00 0000 7209 0000  ..r....r....r...
-000026e0: 0072 1300 0000 7207 0000 0072 1f00 0000  .r....r....r....
-000026f0: 7255 0000 0072 2000 0000 7221 0000 0072  rU...r ...r!...r
-00002700: 5600 0000 7257 0000 0072 5800 0000 720b  V...rW...rX...r.
-00002710: 0000 005a 0969 625f 6e65 7374 6564 7259  ...Z.ib_nestedrY
-00002720: 0000 005a 0769 625f 626f 6f6c 725a 0000  ...Z.ib_boolrZ..
-00002730: 00da 0462 6f6f 6c72 5b00 0000 725c 0000  ...boolr[...r\..
-00002740: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
-00002750: 7225 0000 0072 2600 0000 7227 0000 0072  r%...r&...r'...r
-00002760: 1800 0000 5a07 6962 5f64 6963 7472 5d00  ....Z.ib_dictr].
-00002770: 0000 726c 0000 005a 0269 6272 5e00 0000  ..rl...Z.ibr^...
-00002780: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00002790: 0200 0000 7249 0000 0072 5f00 0000 7260  ....rI...r_...r`
-000027a0: 0000 0072 6200 0000 7265 0000 0072 4d00  ...rb...re...rM.
-000027b0: 0000 724e 0000 0072 7000 0000 726f 0000  ..rN...rp...ro..
-000027c0: 0072 4400 0000 722a 0000 0072 2c00 0000  .rD...r*...r,...
-000027d0: 722e 0000 0072 3000 0000 7232 0000 0072  r....r0...r2...r
-000027e0: 3700 0000 723b 0000 0072 3f00 0000 7241  7...r;...r?...rA
-000027f0: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00002800: 0000 7212 0000 0072 5300 0000 6d00 0000  ..r....rS...m...
-00002810: 7352 0000 000a 0204 0b10 0410 0114 0114  sR..............
-00002820: 0114 0114 0114 0114 0114 0104 0112 0102  ................
-00002830: fe0e 0414 012a 0114 0114 0114 0510 0906  .....*..........
-00002840: 0102 0102 0102 fb02 0202 0102 0102 0102  ................
-00002850: 0102 fa0c 240e 080e 0c0e 0c0e 0c0e 0c0e  ....$...........
-00002860: 0c0e 0e0e 120e 0d72 5300 0000 2916 721e  .......rS...).r.
-00002870: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
-00002880: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00002890: 2200 0000 7206 0000 0072 2400 0000 5a0a  "...r....r$...Z.
-000028a0: 6174 7472 735f 6d61 7465 7207 0000 00da  attrs_mater.....
-000028b0: 0b65 6e75 6d65 7261 7469 6f6e 7209 0000  .enumerationr...
-000028c0: 005a 1473 6372 6970 745f 6669 6c74 6572  .Z.script_filter
-000028d0: 5f6f 626a 6563 7472 0a00 0000 5a06 6465  _objectr....Z.de
-000028e0: 6669 6e65 720b 0000 0072 2900 0000 7246  finer....r)...rF
-000028f0: 0000 0072 4900 0000 724d 0000 0072 5300  ...rI...rM...rS.
-00002900: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00002910: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002920: 0300 0000 731e 0000 0004 0418 0208 010c  ....s...........
-00002930: 010c 020c 010c 0304 0112 1710 2410 0904  ............$...
-00002940: 0112 0910 0d04 01                        .......
+00000df0: 1a9c 0564 1b64 1c84 055a 2e65 0964 0064  ...d.d...Z.e.d.d
+00000e00: 179c 0264 1d64 1e84 045a 2f65 0964 0064  ...d.d...Z/e.d.d
+00000e10: 179c 0264 1f64 2084 045a 3065 0964 0064  ...d.d ..Z0e.d.d
+00000e20: 179c 0264 2164 2284 045a 3165 0964 0064  ...d!d"..Z1e.d.d
+00000e30: 179c 0264 2364 2484 045a 3265 0964 0064  ...d#d$..Z2e.d.d
+00000e40: 179c 0264 2564 2684 045a 3365 0964 0064  ...d%d&..Z3e.d.d
+00000e50: 179c 0264 2764 2884 045a 3465 0964 0064  ...d'd(..Z4e.d.d
+00000e60: 299c 0264 2a64 2b84 045a 3565 0964 0064  )..d*d+..Z5e.d.d
+00000e70: 2c9c 0264 2d64 2e84 045a 3665 0964 0064  ,..d-d...Z6e.d.d
+00000e80: 2c9c 0264 2f64 3084 045a 3764 3565 0965  ,..d/d0..Z7d5e.e
+00000e90: 0964 0064 329c 0364 3364 3484 055a 3864  .d.d2..d3d4..Z8d
+00000ea0: 0553 0029 36da 0449 7465 6d61 0701 0000  .S.)6..Itema....
+00000eb0: 0a20 2020 2044 6174 6120 6d6f 6465 6c20  .    Data model 
+00000ec0: 666f 7220 616c 6672 6564 2064 726f 7064  for alfred dropd
+00000ed0: 6f77 6e20 6d65 6e75 2069 7465 6d73 2e0a  own menu items..
+00000ee0: 0a20 2020 202e 2e20 6e6f 7465 3a3a 0a0a  .    .. note::..
+00000ef0: 2020 2020 2020 2020 506c 6561 7365 206d          Please m
+00000f00: 616b 6520 7375 7265 2074 6865 2061 7474  ake sure the att
+00000f10: 7269 6275 7465 206e 616d 6520 6973 2065  ribute name is e
+00000f20: 7861 6374 6c79 2074 6865 2073 616d 6520  xactly the same 
+00000f30: 6173 2074 6865 2066 6965 6c64 206e 616d  as the field nam
+00000f40: 650a 2020 2020 2020 2020 696e 2074 6865  e.        in the
+00000f50: 2066 6f6c 6c6f 7769 6e67 2064 6f63 756d   following docum
+00000f60: 656e 742e 0a0a 2020 2020 5265 663a 2068  ent...    Ref: h
+00000f70: 7474 7073 3a2f 2f77 7777 2e61 6c66 7265  ttps://www.alfre
+00000f80: 6461 7070 2e63 6f6d 2f68 656c 702f 776f  dapp.com/help/wo
+00000f90: 726b 666c 6f77 732f 696e 7075 7473 2f73  rkflows/inputs/s
+00000fa0: 6372 6970 742d 6669 6c74 6572 2f6a 736f  cript-filter/jso
+00000fb0: 6e2f 0a20 2020 2063 0000 0000 0000 0000  n/.    c........
+00000fc0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00000fd0: 7314 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00000fe0: 0364 025a 0464 0353 0029 047a 0d49 7465  .d.Z.d.S.).z.Ite
+00000ff0: 6d2e 5479 7065 456e 756d da04 6669 6c65  m.TypeEnum..file
+00001000: 7a0e 6669 6c65 3a73 6b69 7063 6865 636b  z.file:skipcheck
+00001010: 4e29 0572 0e00 0000 720f 0000 0072 1000  N).r....r....r..
+00001020: 0000 7253 0000 005a 0e66 696c 655f 736b  ..rS...Z.file_sk
+00001030: 6970 6368 6563 6b72 1100 0000 7211 0000  ipcheckr....r...
+00001040: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001050: 7a00 0000 7304 0000 0008 0104 0172 1300  z...s........r..
+00001060: 0000 da05 7469 746c 654e 7249 0000 00da  ....titleNrI....
+00001070: 0873 7562 7469 746c 65da 0361 7267 da0c  .subtitle..arg..
+00001080: 6175 746f 636f 6d70 6c65 7465 da04 6963  autocomplete..ic
+00001090: 6f6e 54da 0576 616c 6964 da03 7569 64da  onT..valid..uid.
+000010a0: 056d 6174 6368 7215 0000 0072 1800 0000  .matchr....r....
+000010b0: da04 6d6f 6473 da06 6163 7469 6f6e da04  ..mods..action..
+000010c0: 7465 7874 da0c 7175 6963 6b6c 6f6f 6b75  text..quicklooku
+000010d0: 726c 2901 da07 6661 6374 6f72 79da 0976  rl)...factory..v
+000010e0: 6172 6961 626c 6573 7219 0000 0063 0200  ariablesr....c..
+000010f0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001100: 0000 4300 0000 7310 0000 0074 00a0 017c  ..C...s....t...|
+00001110: 01a1 017c 005f 027c 0053 0029 017a 240a  ...|._.|.S.).z$.
+00001120: 2020 2020 2020 2020 5365 7420 6963 6f6e          Set icon
+00001130: 2066 6f72 2069 7465 6d2e 0a20 2020 2020   for item..     
+00001140: 2020 2029 0372 0b00 0000 721c 0000 0072     ).r....r....r
+00001150: 5800 0000 a902 da04 7365 6c66 7214 0000  X.......selfr...
+00001160: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00001170: da08 7365 745f 6963 6f6e 9300 0000 7304  ..set_icon....s.
+00001180: 0000 0000 040c 017a 0d49 7465 6d2e 7365  .......z.Item.se
+00001190: 745f 6963 6f6e 2905 da03 6d6f 6472 5500  t_icon)...modrU.
+000011a0: 0000 7256 0000 0072 5900 0000 721a 0000  ..rV...rY...r...
+000011b0: 0063 0500 0000 0000 0000 0000 0000 0600  .c..............
+000011c0: 0000 0600 0000 4300 0000 734c 0000 007c  ......C...sL...|
+000011d0: 0174 00a0 01a1 006b 0772 1074 0282 0164  .t.....k.r.t...d
+000011e0: 0164 0284 0074 037c 027c 037c 0464 038d  .d...t.|.|.|.d..
+000011f0: 03a0 04a1 0044 0083 017d 057c 006a 0564  .....D...}.|.j.d
+00001200: 046b 0872 3e74 0383 007c 005f 057c 057c  .k.r>t...|._.|.|
+00001210: 006a 057c 013c 007c 0053 0029 0561 8501  .j.|.<.|.S.).a..
+00001220: 0000 0a20 2020 2020 2020 2041 6464 206d  ...        Add m
+00001230: 6f64 6966 6965 7220 746f 2069 7465 6d2e  odifier to item.
+00001240: 204d 6f64 6966 6965 7220 616c 6c6f 7720   Modifier allow 
+00001250: 796f 7520 746f 2072 6574 7572 6e20 6469  you to return di
+00001260: 6666 6572 656e 7420 7469 746c 652c 0a20  fferent title,. 
+00001270: 2020 2020 2020 2073 7562 7469 746c 6520         subtitle 
+00001280: 616e 6420 6172 6775 6d65 6e74 2069 6e20  and argument in 
+00001290: 416c 6672 6564 2064 726f 7020 646f 776e  Alfred drop down
+000012a0: 206d 656e 7520 6974 656d 2077 6865 6e20   menu item when 
+000012b0: 796f 7520 6869 7420 610a 2020 2020 2020  you hit a.      
+000012c0: 2020 6d6f 6469 6669 6572 206b 6579 2e0a    modifier key..
+000012d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000012e0: 6d6f 6465 3a20 7468 6520 6d6f 6469 6669  mode: the modifi
+000012f0: 6572 206b 6579 0a20 2020 2020 2020 203a  er key.        :
+00001300: 7061 7261 6d20 7375 6274 6974 6c65 3a20  param subtitle: 
+00001310: 7468 6520 7375 6274 6974 6c65 2079 6f75  the subtitle you
+00001320: 2077 616e 7420 746f 2064 6973 706c 6179   want to display
+00001330: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001340: 6172 673a 2074 6865 2061 7267 756d 656e  arg: the argumen
+00001350: 7420 7061 7373 6564 2074 6f20 7375 6273  t passed to subs
+00001360: 6571 7565 6e63 6520 6163 7469 6f6e 0a20  equence action. 
+00001370: 2020 2020 2020 203a 7061 7261 6d20 7661         :param va
+00001380: 6c69 643a 2077 6865 7468 6572 2074 6865  lid: whether the
+00001390: 2069 7465 6d20 6973 2076 616c 6964 0a20   item is valid. 
+000013a0: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+000013b0: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+000013c0: 731a 0000 0069 007c 005d 125c 027d 017d  s....i.|.].\.}.}
+000013d0: 027c 0272 047c 017c 0293 0271 0453 0072  .|.r.|.|...q.S.r
+000013e0: 1100 0000 7211 0000 0029 03da 022e 30da  ....r....)....0.
+000013f0: 016b da01 7672 1100 0000 7211 0000 0072  .k..vr....r....r
+00001400: 1200 0000 da0a 3c64 6963 7463 6f6d 703e  ......<dictcomp>
+00001410: ad00 0000 7308 0000 0006 0206 0504 fa02  ....s...........
+00001420: 007a 2549 7465 6d2e 7365 745f 6d6f 6469  .z%Item.set_modi
+00001430: 6669 6572 2e3c 6c6f 6361 6c73 3e2e 3c64  fier.<locals>.<d
+00001440: 6963 7463 6f6d 703e 2903 7255 0000 0072  ictcomp>).rU...r
+00001450: 5600 0000 7259 0000 004e 2906 724c 0000  V...rY...N).rL..
+00001460: 0072 2600 0000 da0a 5661 6c75 6545 7272  .r&.....ValueErr
+00001470: 6f72 da04 6469 6374 da05 6974 656d 7372  or..dict..itemsr
+00001480: 5c00 0000 2906 7263 0000 0072 6500 0000  \...).rc...re...
+00001490: 7255 0000 0072 5600 0000 7259 0000 00da  rU...rV...rY....
+000014a0: 0364 6374 7211 0000 0072 1100 0000 7212  .dctr....r....r.
+000014b0: 0000 00da 0c73 6574 5f6d 6f64 6966 6965  .....set_modifie
+000014c0: 729a 0000 0073 1a00 0000 0011 0c01 0401  r....s..........
+000014d0: 0602 0201 0201 0201 02fd 08fe 0609 0a01  ................
+000014e0: 0801 0a01 7a11 4974 656d 2e73 6574 5f6d  ....z.Item.set_m
+000014f0: 6f64 6966 6965 7263 0200 0000 0000 0000  odifierc........
+00001500: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00001510: 7324 0000 0074 006a 016a 027c 006a 0374  s$...t.j.j.|.j.t
+00001520: 046a 056a 023c 007c 017c 006a 0374 046a  .j.j.<.|.|.j.t.j
+00001530: 066a 023c 007c 0053 0029 017a a20a 2020  .j.<.|.S.).z..  
+00001540: 2020 2020 2020 5468 6973 2069 7320 6120        This is a 
+00001550: 7370 6563 6961 6c20 7661 7269 6162 6c65  special variable
+00001560: 2074 6861 7420 7769 6c6c 206f 7065 6e20   that will open 
+00001570: 7468 6520 6c61 7374 2065 7272 6f72 2066  the last error f
+00001580: 696c 6520 696e 2074 6865 2065 6469 746f  ile in the edito
+00001590: 722e 0a20 2020 2020 2020 2049 7420 6973  r..        It is
+000015a0: 2066 6f72 2069 6e74 6572 6e61 6c20 696d   for internal im
+000015b0: 706c 656d 656e 7461 7469 6f6e 206f 6e6c  plementation onl
+000015c0: 792c 206e 6f74 2066 6f72 2070 7562 6c69  y, not for publi
+000015d0: 6320 4150 492e 0a20 2020 2020 2020 2029  c API..        )
+000015e0: 0772 4500 0000 7246 0000 00da 0576 616c  .rE...rF.....val
+000015f0: 7565 7261 0000 0072 2800 0000 7243 0000  uera...r(...rC..
+00001600: 0072 4400 0000 7262 0000 0072 1100 0000  .rD...rb...r....
+00001610: 7211 0000 0072 1200 0000 7243 0000 00be  r....r....rC....
+00001620: 0000 0073 0600 0000 0005 1201 0e01 7a13  ...s..........z.
+00001630: 4974 656d 2e5f 6f70 656e 5f6c 6f67 5f66  Item._open_log_f
+00001640: 696c 6563 0200 0000 0000 0000 0000 0000  ilec............
+00001650: 0200 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
+00001660: 0074 006a 016a 027c 006a 0374 046a 056a  .t.j.j.|.j.t.j.j
+00001670: 023c 007c 017c 006a 0374 046a 066a 023c  .<.|.|.j.t.j.j.<
+00001680: 007c 0053 0029 0161 1401 0000 0a20 2020  .|.S.).a.....   
+00001690: 2020 2020 2053 6574 2076 6172 6961 626c       Set variabl
+000016a0: 6573 2074 6f20 7465 6c6c 2073 7562 7365  es to tell subse
+000016b0: 7175 656e 6365 2041 6c66 7265 6420 6163  quence Alfred ac
+000016c0: 7469 6f6e 2074 6f20 6f70 656e 2061 2066  tion to open a f
+000016d0: 696c 652e 0a0a 2020 2020 2020 2020 5573  ile...        Us
+000016e0: 6520 7468 6520 2255 7469 6c69 7469 6573  e the "Utilities
+000016f0: 202d 3e20 436f 6e64 6974 696f 6e61 6c22   -> Conditional"
+00001700: 2077 6964 6765 7420 616e 6420 7365 743a   widget and set:
+00001710: 2069 6620 6060 7b76 6172 3a6f 7065 6e5f   if ``{var:open_
+00001720: 6669 6c65 7d60 600a 2020 2020 2020 2020  file}``.        
+00001730: 6973 2065 7175 616c 2074 6f20 2279 222e  is equal to "y".
+00001740: 0a0a 2020 2020 2020 2020 5573 6520 7468  ..        Use th
+00001750: 6520 2241 6374 696f 6e73 202d 3e20 4f70  e "Actions -> Op
+00001760: 656e 2046 696c 6522 2077 6964 6765 7420  en File" widget 
+00001770: 616e 6420 7365 743a 2046 696c 653a 2060  and set: File: `
+00001780: 607b 7661 723a 6f70 656e 5f66 696c 655f  `{var:open_file_
+00001790: 7061 7468 7d60 600a 2020 2020 2020 2020  path}``.        
+000017a0: 2907 7245 0000 0072 4600 0000 726f 0000  ).rE...rF...ro..
+000017b0: 0072 6100 0000 7228 0000 0072 2900 0000  .ra...r(...r)...
+000017c0: 722a 0000 0072 6200 0000 7211 0000 0072  r*...rb...r....r
+000017d0: 1100 0000 7212 0000 0072 2900 0000 c700  ....r....r).....
+000017e0: 0000 7306 0000 0000 0912 010e 017a 0e49  ..s..........z.I
+000017f0: 7465 6d2e 6f70 656e 5f66 696c 6563 0200  tem.open_filec..
+00001800: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001810: 0000 4300 0000 7324 0000 0074 006a 016a  ..C...s$...t.j.j
+00001820: 027c 006a 0374 046a 056a 023c 007c 017c  .|.j.t.j.j.<.|.|
+00001830: 006a 0374 046a 066a 023c 007c 0053 0029  .j.t.j.j.<.|.S.)
+00001840: 0161 0a01 0000 0a20 2020 2020 2020 2053  .a.....        S
+00001850: 6574 2076 6172 6961 626c 6573 2074 6f20  et variables to 
+00001860: 7465 6c6c 2073 7562 7365 7175 656e 6365  tell subsequence
+00001870: 2041 6c66 7265 6420 6163 7469 6f6e 2074   Alfred action t
+00001880: 6f20 6c61 756e 6368 2061 6e20 6170 7020  o launch an app 
+00001890: 6f72 2066 696c 652e 0a0a 2020 2020 2020  or file...      
+000018a0: 2020 5573 6520 7468 6520 2255 7469 6c69    Use the "Utili
+000018b0: 7469 6573 202d 3e20 436f 6e64 6974 696f  ties -> Conditio
+000018c0: 6e61 6c22 2077 6964 6765 7420 616e 6420  nal" widget and 
+000018d0: 7365 743a 2069 6620 6060 7b76 6172 3a6c  set: if ``{var:l
+000018e0: 6175 6e63 685f 6170 705f 6f72 5f66 696c  aunch_app_or_fil
+000018f0: 657d 6060 0a20 2020 2020 2020 2069 7320  e}``.        is 
+00001900: 6571 7561 6c20 746f 2022 7922 2e0a 0a20  equal to "y"... 
+00001910: 2020 2020 2020 2055 7365 2074 6865 2022         Use the "
+00001920: 4163 7469 6f6e 7320 2d3e 204c 6175 6e63  Actions -> Launc
+00001930: 6820 4170 7073 202f 2046 696c 6573 2220  h Apps / Files" 
+00001940: 7769 6467 6574 2e0a 2020 2020 2020 2020  widget..        
+00001950: 2907 7245 0000 0072 4600 0000 726f 0000  ).rE...rF...ro..
+00001960: 0072 6100 0000 7228 0000 0072 2b00 0000  .ra...r(...r+...
+00001970: 722c 0000 0072 6200 0000 7211 0000 0072  r,...rb...r....r
+00001980: 1100 0000 7212 0000 0072 2b00 0000 d400  ....r....r+.....
+00001990: 0000 7306 0000 0000 0912 010e 017a 1749  ..s..........z.I
+000019a0: 7465 6d2e 6c61 756e 6368 5f61 7070 5f6f  tem.launch_app_o
+000019b0: 725f 6669 6c65 6302 0000 0000 0000 0000  r_filec.........
+000019c0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000019d0: 2400 0000 7400 6a01 6a02 7c00 6a03 7404  $...t.j.j.|.j.t.
+000019e0: 6a05 6a02 3c00 7c01 7c00 6a03 7404 6a06  j.j.<.|.|.j.t.j.
+000019f0: 6a02 3c00 7c00 5300 2901 610f 0100 000a  j.<.|.S.).a.....
+00001a00: 2020 2020 2020 2020 5365 7420 7661 7269          Set vari
+00001a10: 6162 6c65 7320 746f 2074 656c 6c20 7375  ables to tell su
+00001a20: 6273 6571 7565 6e63 6520 416c 6672 6564  bsequence Alfred
+00001a30: 2061 6374 696f 6e20 746f 206c 6175 6e63   action to launc
+00001a40: 6820 616e 2061 7070 206f 7220 6669 6c65  h an app or file
+00001a50: 2e0a 0a20 2020 2020 2020 2055 7365 2074  ...        Use t
+00001a60: 6865 2022 5574 696c 6974 6965 7320 2d3e  he "Utilities ->
+00001a70: 2043 6f6e 6469 7469 6f6e 616c 2220 7769   Conditional" wi
+00001a80: 6467 6574 2061 6e64 2073 6574 3a20 6966  dget and set: if
+00001a90: 2060 607b 7661 723a 7265 7665 616c 5f66   ``{var:reveal_f
+00001aa0: 696c 655f 696e 5f66 696e 6465 727d 6060  ile_in_finder}``
+00001ab0: 0a20 2020 2020 2020 2069 7320 6571 7561  .        is equa
+00001ac0: 6c20 746f 2022 7922 2e0a 0a20 2020 2020  l to "y"...     
+00001ad0: 2020 2055 7365 2074 6865 2022 4163 7469     Use the "Acti
+00001ae0: 6f6e 7320 2d3e 2052 6576 6561 6c20 4669  ons -> Reveal Fi
+00001af0: 6c65 2069 6e20 4669 6e64 6572 2220 7769  le in Finder" wi
+00001b00: 6467 6574 2e0a 2020 2020 2020 2020 2907  dget..        ).
+00001b10: 7245 0000 0072 4600 0000 726f 0000 0072  rE...rF...ro...r
+00001b20: 6100 0000 7228 0000 0072 2d00 0000 722e  a...r(...r-...r.
+00001b30: 0000 0072 6200 0000 7211 0000 0072 1100  ...rb...r....r..
+00001b40: 0000 7212 0000 0072 2d00 0000 e100 0000  ..r....r-.......
+00001b50: 7306 0000 0000 0912 010e 017a 1a49 7465  s..........z.Ite
+00001b60: 6d2e 7265 7665 616c 5f66 696c 655f 696e  m.reveal_file_in
+00001b70: 5f66 696e 6465 7263 0200 0000 0000 0000  _finderc........
+00001b80: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00001b90: 7324 0000 0074 006a 016a 027c 006a 0374  s$...t.j.j.|.j.t
+00001ba0: 046a 056a 023c 007c 017c 006a 0374 046a  .j.j.<.|.|.j.t.j
+00001bb0: 066a 023c 007c 0053 0029 0161 0601 0000  .j.<.|.S.).a....
+00001bc0: 0a20 2020 2020 2020 2053 6574 2076 6172  .        Set var
+00001bd0: 6961 626c 6573 2074 6f20 7465 6c6c 2073  iables to tell s
+00001be0: 7562 7365 7175 656e 6365 2041 6c66 7265  ubsequence Alfre
+00001bf0: 6420 6163 7469 6f6e 2074 6f20 6272 6f77  d action to brow
+00001c00: 7365 2069 6e20 7465 726d 696e 616c 2e0a  se in terminal..
+00001c10: 0a20 2020 2020 2020 2055 7365 2074 6865  .        Use the
+00001c20: 2022 5574 696c 6974 6965 7320 2d3e 2043   "Utilities -> C
+00001c30: 6f6e 6469 7469 6f6e 616c 2220 7769 6467  onditional" widg
+00001c40: 6574 2061 6e64 2073 6574 3a20 6966 2060  et and set: if `
+00001c50: 607b 7661 723a 6272 6f77 7365 5f69 6e5f  `{var:browse_in_
+00001c60: 7465 726d 696e 616c 7d60 600a 2020 2020  terminal}``.    
+00001c70: 2020 2020 6973 2065 7175 616c 2074 6f20      is equal to 
+00001c80: 2279 222e 0a0a 2020 2020 2020 2020 5573  "y"...        Us
+00001c90: 6520 7468 6520 2241 6374 696f 6e73 202d  e the "Actions -
+00001ca0: 3e20 4272 6f77 7365 2069 6e20 5465 726d  > Browse in Term
+00001cb0: 696e 616c 2220 7769 6467 6574 2e0a 2020  inal" widget..  
+00001cc0: 2020 2020 2020 2907 7245 0000 0072 4600        ).rE...rF.
+00001cd0: 0000 726f 0000 0072 6100 0000 7228 0000  ..ro...ra...r(..
+00001ce0: 0072 2f00 0000 7230 0000 0072 6200 0000  .r/...r0...rb...
+00001cf0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00001d00: 2f00 0000 ee00 0000 7306 0000 0000 0912  /.......s.......
+00001d10: 010e 017a 1749 7465 6d2e 6272 6f77 7365  ...z.Item.browse
+00001d20: 5f69 6e5f 7465 726d 696e 616c 6302 0000  _in_terminalc...
+00001d30: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00001d40: 0043 0000 0073 2400 0000 7400 6a01 6a02  .C...s$...t.j.j.
+00001d50: 7c00 6a03 7404 6a05 6a02 3c00 7c01 7c00  |.j.t.j.j.<.|.|.
+00001d60: 6a03 7404 6a06 6a02 3c00 7c00 5300 2901  j.t.j.j.<.|.S.).
+00001d70: 6100 0100 000a 2020 2020 2020 2020 5365  a.....        Se
+00001d80: 7420 7661 7269 6162 6c65 7320 746f 2074  t variables to t
+00001d90: 656c 6c20 7375 6273 6571 7565 6e63 6520  ell subsequence 
+00001da0: 416c 6672 6564 2061 6374 696f 6e20 746f  Alfred action to
+00001db0: 2062 726f 7773 6520 696e 2041 6c66 7265   browse in Alfre
+00001dc0: 642e 0a0a 2020 2020 2020 2020 5573 6520  d...        Use 
+00001dd0: 7468 6520 2255 7469 6c69 7469 6573 202d  the "Utilities -
+00001de0: 3e20 436f 6e64 6974 696f 6e61 6c22 2077  > Conditional" w
+00001df0: 6964 6765 7420 616e 6420 7365 743a 2069  idget and set: i
+00001e00: 6620 6060 7b76 6172 3a62 726f 7773 655f  f ``{var:browse_
+00001e10: 696e 5f61 6c66 7265 647d 6060 0a20 2020  in_alfred}``.   
+00001e20: 2020 2020 2069 7320 6571 7561 6c20 746f       is equal to
+00001e30: 2022 7922 2e0a 0a20 2020 2020 2020 2055   "y"...        U
+00001e40: 7365 2074 6865 2022 4163 7469 6f6e 7320  se the "Actions 
+00001e50: 2d3e 2042 726f 7773 6520 696e 2041 6c66  -> Browse in Alf
+00001e60: 7265 6422 2077 6964 6765 742e 0a20 2020  red" widget..   
+00001e70: 2020 2020 2029 0772 4500 0000 7246 0000       ).rE...rF..
+00001e80: 0072 6f00 0000 7261 0000 0072 2800 0000  .ro...ra...r(...
+00001e90: 7231 0000 0072 3200 0000 7262 0000 0072  r1...r2...rb...r
+00001ea0: 1100 0000 7211 0000 0072 1200 0000 7231  ....r....r....r1
+00001eb0: 0000 00fb 0000 0073 0600 0000 0009 1201  .......s........
+00001ec0: 0e01 7a15 4974 656d 2e62 726f 7773 655f  ..z.Item.browse_
+00001ed0: 696e 5f61 6c66 7265 6429 02da 0375 726c  in_alfred)...url
+00001ee0: 721a 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00001ef0: 0000 0200 0000 0300 0000 4300 0000 7324  ..........C...s$
+00001f00: 0000 0074 006a 016a 027c 006a 0374 046a  ...t.j.j.|.j.t.j
+00001f10: 056a 023c 007c 017c 006a 0374 046a 066a  .j.<.|.|.j.t.j.j
+00001f20: 023c 007c 0053 0029 0161 1901 0000 0a20  .<.|.S.).a..... 
+00001f30: 2020 2020 2020 2053 6574 2076 6172 6961         Set varia
+00001f40: 626c 6573 2074 6f20 7465 6c6c 2073 7562  bles to tell sub
+00001f50: 7365 7175 656e 6365 2041 6c66 7265 6420  sequence Alfred 
+00001f60: 6163 7469 6f6e 2074 6f20 6f70 656e 2075  action to open u
+00001f70: 726c 2e0a 0a20 2020 2020 2020 2055 7365  rl...        Use
+00001f80: 2074 6865 2022 5574 696c 6974 6965 7320   the "Utilities 
+00001f90: 2d3e 2043 6f6e 6469 7469 6f6e 616c 2220  -> Conditional" 
+00001fa0: 7769 6467 6574 2061 6e64 2073 6574 3a20  widget and set: 
+00001fb0: 6966 2060 607b 7661 723a 6f70 656e 5f75  if ``{var:open_u
+00001fc0: 726c 7d60 600a 2020 2020 2020 2020 6973  rl}``.        is
+00001fd0: 2065 7175 616c 2074 6f20 2279 222e 0a0a   equal to "y"...
+00001fe0: 2020 2020 2020 2020 5573 6520 7468 6520          Use the 
+00001ff0: 2241 6374 696f 6e73 202d 3e20 4f70 656e  "Actions -> Open
+00002000: 2055 524c 2220 7769 6467 6574 2061 6e64   URL" widget and
+00002010: 2073 6574 3a0a 0a20 2020 2020 2020 202d   set:..        -
+00002020: 2046 696c 6520 3d20 6060 7b76 6172 3a6f   File = ``{var:o
+00002030: 7065 6e5f 7572 6c5f 6172 677d 6060 0a20  pen_url_arg}``. 
+00002040: 2020 2020 2020 2029 0772 4500 0000 7246         ).rE...rF
+00002050: 0000 0072 6f00 0000 7261 0000 0072 2800  ...ro...ra...r(.
+00002060: 0000 7236 0000 0072 3700 0000 2902 7263  ..r6...r7...).rc
+00002070: 0000 0072 7000 0000 7211 0000 0072 1100  ...rp...r....r..
+00002080: 0000 7212 0000 0072 3600 0000 0801 0000  ..r....r6.......
+00002090: 7306 0000 0000 0b12 010e 017a 0d49 7465  s..........z.Ite
+000020a0: 6d2e 6f70 656e 5f75 726c 2902 724d 0000  m.open_url).rM..
+000020b0: 0072 1a00 0000 6302 0000 0000 0000 0000  .r....c.........
+000020c0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000020d0: 2a00 0000 7400 6a01 6a02 7c00 6a03 7404  *...t.j.j.|.j.t.
+000020e0: 6a05 6a02 3c00 7c01 7c00 6a03 7404 6a06  j.j.<.|.|.j.t.j.
+000020f0: 6a02 3c00 7c01 7c00 5f07 7c00 5300 2901  j.<.|.|._.|.S.).
+00002100: 6188 0100 000a 2020 2020 2020 2020 5365  a.....        Se
+00002110: 7420 7661 7269 6162 6c65 7320 746f 2074  t variables to t
+00002120: 656c 6c20 7375 6273 6571 7565 6e63 6520  ell subsequence 
+00002130: 416c 6672 6564 2061 6374 696f 6e20 746f  Alfred action to
+00002140: 2072 756e 2073 6372 6970 742e 0a0a 2020   run script...  
+00002150: 2020 2020 2020 5573 6520 7468 6520 2255        Use the "U
+00002160: 7469 6c69 7469 6573 202d 3e20 436f 6e64  tilities -> Cond
+00002170: 6974 696f 6e61 6c22 2077 6964 6765 7420  itional" widget 
+00002180: 616e 6420 7365 743a 2069 6620 6060 7b76  and set: if ``{v
+00002190: 6172 3a72 756e 5f73 6372 6970 747d 6060  ar:run_script}``
+000021a0: 0a20 2020 2020 2020 2069 7320 6571 7561  .        is equa
+000021b0: 6c20 746f 2022 7922 2e0a 0a20 2020 2020  l to "y"...     
+000021c0: 2020 2055 7365 2074 6865 2022 4163 7469     Use the "Acti
+000021d0: 6f6e 7320 2d3e 2052 756e 2053 6372 6970  ons -> Run Scrip
+000021e0: 7422 2077 6964 6765 7420 616e 6420 7365  t" widget and se
+000021f0: 743a 0a0a 2020 2020 2020 2020 2d20 4c61  t:..        - La
+00002200: 6e67 7561 6765 203d 2060 602f 6269 6e2f  nguage = ``/bin/
+00002210: 6261 7368 6060 0a20 2020 2020 2020 202d  bash``.        -
+00002220: 2022 7769 7468 2069 6e70 7574 2061 7320   "with input as 
+00002230: 7b71 7565 7279 7d22 0a20 2020 2020 2020  {query}".       
+00002240: 202d 2072 756e 6e69 6e67 2069 6e73 7461   - running insta
+00002250: 6e63 6573 203d 2022 5365 7175 656e 7469  nces = "Sequenti
+00002260: 616c 6c79 220a 2020 2020 2020 2020 2d20  ally".        - 
+00002270: 5363 7269 7074 203d 2060 607b 7175 6572  Script = ``{quer
+00002280: 797d 6060 0a20 2020 2020 2020 2029 0872  y}``.        ).r
+00002290: 4500 0000 7246 0000 0072 6f00 0000 7261  E...rF...ro...ra
+000022a0: 0000 0072 2800 0000 723a 0000 0072 3b00  ...r(...r:...r;.
+000022b0: 0000 7256 0000 00a9 0272 6300 0000 724d  ..rV.....rc...rM
+000022c0: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+000022d0: 0000 723a 0000 0017 0100 0073 0800 0000  ..r:.......s....
+000022e0: 000e 1201 0e01 0601 7a0f 4974 656d 2e72  ........z.Item.r
+000022f0: 756e 5f73 6372 6970 7463 0200 0000 0000  un_scriptc......
+00002300: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00002310: 0000 732a 0000 0074 006a 016a 027c 006a  ..s*...t.j.j.|.j
+00002320: 0374 046a 056a 023c 007c 017c 006a 0374  .t.j.j.<.|.|.j.t
+00002330: 046a 066a 023c 007c 017c 005f 077c 0053  .j.j.<.|.|._.|.S
+00002340: 0029 017a db0a 2020 2020 2020 2020 5573  .).z..        Us
+00002350: 6520 7468 6520 2255 7469 6c69 7469 6573  e the "Utilities
+00002360: 202d 3e20 436f 6e64 6974 696f 6e61 6c22   -> Conditional"
+00002370: 2077 6964 6765 7420 616e 6420 7365 743a   widget and set:
+00002380: 2069 6620 6060 7b76 6172 3a74 6572 6d69   if ``{var:termi
+00002390: 6e61 6c5f 636f 6d6d 616e 647d 6060 0a20  nal_command}``. 
+000023a0: 2020 2020 2020 2069 7320 6571 7561 6c20         is equal 
+000023b0: 746f 2022 7922 2e0a 0a20 2020 2020 2020  to "y"...       
+000023c0: 2055 7365 2074 6865 2022 4163 7469 6f6e   Use the "Action
+000023d0: 7320 2d3e 2054 6572 6d69 6e61 6c20 436f  s -> Terminal Co
+000023e0: 6d6d 616e 6422 2077 6964 6765 7420 616e  mmand" widget an
+000023f0: 6420 7365 743a 0a0a 2020 2020 2020 2020  d set:..        
+00002400: 2d20 436f 6d6d 616e 6420 3d20 6060 7b71  - Command = ``{q
+00002410: 7565 7279 7d60 600a 2020 2020 2020 2020  uery}``.        
+00002420: 2908 7245 0000 0072 4600 0000 726f 0000  ).rE...rF...ro..
+00002430: 0072 6100 0000 7228 0000 0072 3e00 0000  .ra...r(...r>...
+00002440: 723f 0000 0072 5600 0000 7271 0000 0072  r?...rV...rq...r
+00002450: 1100 0000 7211 0000 0072 1200 0000 723e  ....r....r....r>
+00002460: 0000 002a 0100 0073 0800 0000 0009 1201  ...*...s........
+00002470: 0e01 0601 7a15 4974 656d 2e74 6572 6d69  ....z.Item.termi
+00002480: 6e61 6c5f 636f 6d6d 616e 64da 0029 0372  nal_command..).r
+00002490: 5400 0000 7255 0000 0072 1a00 0000 6303  T...rU...r....c.
+000024a0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000024b0: 0000 0043 0000 0073 3200 0000 7400 6a01  ...C...s2...t.j.
+000024c0: 6a02 7c00 6a03 7404 6a05 6a02 3c00 7c01  j.|.j.t.j.j.<.|.
+000024d0: 7c00 6a03 7404 6a06 6a02 3c00 7c02 7c00  |.j.t.j.j.<.|.|.
+000024e0: 6a03 7404 6a07 6a02 3c00 7c00 5300 2901  j.t.j.j.<.|.S.).
+000024f0: 617a 0100 000a 2020 2020 2020 2020 5365  az....        Se
+00002500: 7420 7661 7269 6162 6c65 7320 746f 2074  t variables to t
+00002510: 656c 6c20 7375 6273 6571 7565 6e63 6520  ell subsequence 
+00002520: 416c 6672 6564 2061 6374 696f 6e20 746f  Alfred action to
+00002530: 2073 656e 6420 6e6f 7469 6669 6361 7469   send notificati
+00002540: 6f6e 2e0a 0a20 2020 2020 2020 2055 7365  on...        Use
+00002550: 2074 6865 2022 5574 696c 6974 6965 7320   the "Utilities 
+00002560: 2d3e 2043 6f6e 6469 7469 6f6e 616c 2220  -> Conditional" 
+00002570: 7769 6467 6574 2061 6e64 2073 6574 3a20  widget and set: 
+00002580: 6966 2060 607b 7661 723a 7365 6e64 5f6e  if ``{var:send_n
+00002590: 6f74 6966 6963 6174 696f 6e7d 6060 0a20  otification}``. 
+000025a0: 2020 2020 2020 2069 7320 6571 7561 6c20         is equal 
+000025b0: 746f 2022 7922 2e0a 0a20 2020 2020 2020  to "y"...       
+000025c0: 2055 7365 2074 6865 2022 4f75 7470 7574   Use the "Output
+000025d0: 7320 2d3e 2050 6f73 7420 4e6f 7469 6669  s -> Post Notifi
+000025e0: 6361 7469 6f6e 2220 7769 6467 6574 2061  cation" widget a
+000025f0: 6e64 2073 6574 3a0a 0a20 2020 2020 2020  nd set:..       
+00002600: 202d 2054 6974 6c65 203d 2060 607b 7661   - Title = ``{va
+00002610: 723a 7365 6e64 5f6e 6f74 6966 6963 6174  r:send_notificat
+00002620: 696f 6e5f 7469 746c 657d 6060 0a20 2020  ion_title}``.   
+00002630: 2020 2020 202d 2053 7562 7469 746c 6520       - Subtitle 
+00002640: 3d20 6060 7b76 6172 3a73 656e 645f 6e6f  = ``{var:send_no
+00002650: 7469 6669 6361 7469 6f6e 5f73 7562 7469  tification_subti
+00002660: 746c 657d 6060 0a20 2020 2020 2020 2029  tle}``.        )
+00002670: 0872 4500 0000 7246 0000 0072 6f00 0000  .rE...rF...ro...
+00002680: 7261 0000 0072 2800 0000 7240 0000 0072  ra...r(...r@...r
+00002690: 4100 0000 7242 0000 0029 0372 6300 0000  A...rB...).rc...
+000026a0: 7254 0000 0072 5500 0000 7211 0000 0072  rT...rU...r....r
+000026b0: 1100 0000 7212 0000 0072 4000 0000 3801  ....r....r@...8.
+000026c0: 0000 7308 0000 0000 0c12 010e 010e 017a  ..s............z
+000026d0: 1649 7465 6d2e 7365 6e64 5f6e 6f74 6966  .Item.send_notif
+000026e0: 6963 6174 696f 6e29 0172 7200 0000 2939  ication).rr...)9
+000026f0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00002700: 1d00 0000 7209 0000 0072 1300 0000 7207  ....r....r....r.
+00002710: 0000 0072 1e00 0000 7254 0000 0072 1f00  ...r....rT...r..
+00002720: 0000 7220 0000 0072 5500 0000 7256 0000  ..r ...rU...rV..
+00002730: 0072 5700 0000 720b 0000 005a 0969 625f  .rW...r....Z.ib_
+00002740: 6e65 7374 6564 7258 0000 005a 0769 625f  nestedrX...Z.ib_
+00002750: 626f 6f6c 7259 0000 00da 0462 6f6f 6c72  boolrY.....boolr
+00002760: 5a00 0000 725b 0000 0072 2100 0000 7222  Z...r[...r!...r"
+00002770: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00002780: 0000 7226 0000 0072 1800 0000 5a07 6962  ..r&...r....Z.ib
+00002790: 5f64 6963 7472 5c00 0000 726b 0000 005a  _dictr\...rk...Z
+000027a0: 0269 6272 5d00 0000 7203 0000 0072 0400  .ibr]...r....r..
+000027b0: 0000 7205 0000 0072 0200 0000 7248 0000  ..r....r....rH..
+000027c0: 0072 5e00 0000 725f 0000 0072 6100 0000  .r^...r_...ra...
+000027d0: 7264 0000 0072 4c00 0000 724d 0000 0072  rd...rL...rM...r
+000027e0: 6f00 0000 726e 0000 0072 4300 0000 7229  o...rn...rC...r)
+000027f0: 0000 0072 2b00 0000 722d 0000 0072 2f00  ...r+...r-...r/.
+00002800: 0000 7231 0000 0072 3600 0000 723a 0000  ..r1...r6...r:..
+00002810: 0072 3e00 0000 7240 0000 0072 1100 0000  .r>...r@...r....
+00002820: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00002830: 5200 0000 6d00 0000 7352 0000 000a 0204  R...m...sR......
+00002840: 0b10 0410 0114 0114 0114 0114 0114 0114  ................
+00002850: 0114 0104 0112 0102 fe0e 0414 012a 0114  .............*..
+00002860: 0114 0114 0510 0906 0102 0102 0102 fb02  ................
+00002870: 0202 0102 0102 0102 0102 fa0c 2410 0910  ............$...
+00002880: 0d10 0d10 0d10 0d10 0d10 0f10 1310 0e72  ...............r
+00002890: 5200 0000 2916 721d 0000 00da 0674 7970  R...).r......typ
+000028a0: 696e 6772 0200 0000 7203 0000 0072 0400  ingr....r....r..
+000028b0: 0000 7205 0000 0072 2100 0000 7206 0000  ..r....r!...r...
+000028c0: 0072 2300 0000 5a0a 6174 7472 735f 6d61  .r#...Z.attrs_ma
+000028d0: 7465 7207 0000 00da 0b65 6e75 6d65 7261  ter......enumera
+000028e0: 7469 6f6e 7209 0000 005a 1473 6372 6970  tionr....Z.scrip
+000028f0: 745f 6669 6c74 6572 5f6f 626a 6563 7472  t_filter_objectr
+00002900: 0a00 0000 5a06 6465 6669 6e65 720b 0000  ....Z.definer...
+00002910: 0072 2800 0000 7245 0000 0072 4800 0000  .r(...rE...rH...
+00002920: 724c 0000 0072 5200 0000 7211 0000 0072  rL...rR...r....r
+00002930: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
+00002940: 3c6d 6f64 756c 653e 0300 0000 731e 0000  <module>....s...
+00002950: 0004 0418 0208 010c 010c 020c 010c 0304  ................
+00002960: 0112 1710 2410 0904 0112 0910 0d04 01    ....$..........
```

### Comparing `afwf-0.3.2/afwf/__pycache__/query.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/query.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/script_filter.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/script_filter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/script_filter_object.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/script_filter_object.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/__pycache__/workflow.cpython-38.pyc` & `afwf-0.4.1/afwf/__pycache__/workflow.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/_icon.py` & `afwf-0.4.1/afwf/_icon.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/enumeration.py` & `afwf-0.4.1/afwf/enumeration.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/example_wf/handlers/python_version.py` & `afwf-0.4.1/afwf/example_wf/handlers/python_version.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/handler.py` & `afwf-0.4.1/afwf/handler.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icon.py` & `afwf-0.4.1/afwf/icon.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/archive-folder-96.png` & `afwf-0.4.1/afwf/icons/archive-folder-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/bash-96.png` & `afwf-0.4.1/afwf/icons/bash-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/box-96.png` & `afwf-0.4.1/afwf/icons/box-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/calendar-96.png` & `afwf-0.4.1/afwf/icons/calendar-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/chat-96.png` & `afwf-0.4.1/afwf/icons/chat-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/code-96.png` & `afwf-0.4.1/afwf/icons/code-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/debug-96.png` & `afwf-0.4.1/afwf/icons/debug-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/dictionary-96.png` & `afwf-0.4.1/afwf/icons/dictionary-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/error-96.png` & `afwf-0.4.1/afwf/icons/error-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/explosion-96.png` & `afwf-0.4.1/afwf/icons/explosion-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/fire-96.png` & `afwf-0.4.1/afwf/icons/fire-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/flask-96.png` & `afwf-0.4.1/afwf/icons/flask-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/folder-96.png` & `afwf-0.4.1/afwf/icons/folder-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/gear-96.png` & `afwf-0.4.1/afwf/icons/gear-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/git-96.png` & `afwf-0.4.1/afwf/icons/git-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/groupchat-96.png` & `afwf-0.4.1/afwf/icons/groupchat-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/id-card-96.png` & `afwf-0.4.1/afwf/icons/id-card-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/idea-96.png` & `afwf-0.4.1/afwf/icons/idea-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/internet-96.png` & `afwf-0.4.1/afwf/icons/internet-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/iphone-96.png` & `afwf-0.4.1/afwf/icons/iphone-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/landline-96.png` & `afwf-0.4.1/afwf/icons/landline-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/mail-96.png` & `afwf-0.4.1/afwf/icons/mail-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/meeting-96.png` & `afwf-0.4.1/afwf/icons/meeting-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/microsoft-excel-96.png` & `afwf-0.4.1/afwf/icons/microsoft-excel-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/microsoft-powerpoint-96.png` & `afwf-0.4.1/afwf/icons/microsoft-powerpoint-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/microsoft-word-96.png` & `afwf-0.4.1/afwf/icons/microsoft-word-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/minus-96.png` & `afwf-0.4.1/afwf/icons/minus-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/password-96.png` & `afwf-0.4.1/afwf/icons/password-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/pause-96.png` & `afwf-0.4.1/afwf/icons/pause-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/plus-96.png` & `afwf-0.4.1/afwf/icons/plus-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/question-96.png` & `afwf-0.4.1/afwf/icons/question-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/redo-96.png` & `afwf-0.4.1/afwf/icons/redo-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/refresh-96.png` & `afwf-0.4.1/afwf/icons/refresh-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/remove-96.png` & `afwf-0.4.1/afwf/icons/remove-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/reset-96.png` & `afwf-0.4.1/afwf/icons/reset-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/rocket-96.png` & `afwf-0.4.1/afwf/icons/rocket-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/search-96.png` & `afwf-0.4.1/afwf/icons/search-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/star-96.png` & `afwf-0.4.1/afwf/icons/star-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/start-96.png` & `afwf-0.4.1/afwf/icons/start-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/stop-96.png` & `afwf-0.4.1/afwf/icons/stop-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/task-96.png` & `afwf-0.4.1/afwf/icons/task-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/todo-96.png` & `afwf-0.4.1/afwf/icons/todo-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/icons/undo-96.png` & `afwf-0.4.1/afwf/icons/undo-96.png`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/item.py` & `afwf-0.4.1/afwf/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,97 +183,104 @@
             self.mods = dict()
         self.mods[mod] = dct
         return self
 
     # --------------------------------------------------------------------------
     # Set variables
     # --------------------------------------------------------------------------
-    def _open_log_file(self, path: str):  # pragma: no cover
+    def _open_log_file(self, path: str) -> "Item":  # pragma: no cover
         """
         This is a special variable that will open the last error file in the editor.
         It is for internal implementation only, not for public API.
         """
         self.variables[VarKeyEnum._open_log_file.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum._open_log_file_path.value] = path
+        return self
 
-    def open_file(self, path: str):
+    def open_file(self, path: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to open a file.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:open_file}``
         is equal to "y".
 
         Use the "Actions -> Open File" widget and set: File: ``{var:open_file_path}``
         """
         self.variables[VarKeyEnum.open_file.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.open_file_path.value] = path
+        return self
 
-    def launch_app_or_file(self, path: str):
+    def launch_app_or_file(self, path: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to launch an app or file.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:launch_app_or_file}``
         is equal to "y".
 
         Use the "Actions -> Launch Apps / Files" widget.
         """
         self.variables[VarKeyEnum.launch_app_or_file.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.launch_app_or_file_path.value] = path
+        return self
 
-    def reveal_file_in_finder(self, path: str):
+    def reveal_file_in_finder(self, path: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to launch an app or file.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:reveal_file_in_finder}``
         is equal to "y".
 
         Use the "Actions -> Reveal File in Finder" widget.
         """
         self.variables[VarKeyEnum.reveal_file_in_finder.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.reveal_file_in_finder_path.value] = path
+        return self
 
-    def browse_in_terminal(self, path: str):
+    def browse_in_terminal(self, path: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to browse in terminal.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:browse_in_terminal}``
         is equal to "y".
 
         Use the "Actions -> Browse in Terminal" widget.
         """
         self.variables[VarKeyEnum.browse_in_terminal.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.browse_in_terminal_path.value] = path
+        return self
 
-    def browse_in_alfred(self, path: str):
+    def browse_in_alfred(self, path: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to browse in Alfred.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:browse_in_alfred}``
         is equal to "y".
 
         Use the "Actions -> Browse in Alfred" widget.
         """
         self.variables[VarKeyEnum.browse_in_alfred.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.browse_in_alfred_path.value] = path
+        return self
 
-    def open_url(self, url: str):
+    def open_url(self, url: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to open url.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:open_url}``
         is equal to "y".
 
         Use the "Actions -> Open URL" widget and set:
 
         - File = ``{var:open_url_arg}``
         """
         self.variables[VarKeyEnum.open_url.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.open_url_arg.value] = url
+        return self
 
-    def run_script(self, cmd: str):
+    def run_script(self, cmd: str) -> "Item":
         """
         Set variables to tell subsequence Alfred action to run script.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:run_script}``
         is equal to "y".
 
         Use the "Actions -> Run Script" widget and set:
@@ -282,36 +289,39 @@
         - "with input as {query}"
         - running instances = "Sequentially"
         - Script = ``{query}``
         """
         self.variables[VarKeyEnum.run_script.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.run_script_arg.value] = cmd
         self.arg = cmd
+        return self
 
-    def terminal_command(self, cmd: str):
+    def terminal_command(self, cmd: str) -> "Item":
         """
         Use the "Utilities -> Conditional" widget and set: if ``{var:terminal_command}``
         is equal to "y".
 
         Use the "Actions -> Terminal Command" widget and set:
 
         - Command = ``{query}``
         """
         self.variables[VarKeyEnum.terminal_command.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.terminal_command_arg.value] = cmd
         self.arg = cmd
+        return self
 
-    def send_notification(self, title: str, subtitle: str = ""):
+    def send_notification(self, title: str, subtitle: str = "") -> "Item":
         """
         Set variables to tell subsequence Alfred action to send notification.
 
         Use the "Utilities -> Conditional" widget and set: if ``{var:send_notification}``
         is equal to "y".
 
         Use the "Outputs -> Post Notification" widget and set:
 
         - Title = ``{var:send_notification_title}``
         - Subtitle = ``{var:send_notification_subtitle}``
         """
         self.variables[VarKeyEnum.send_notification.value] = VarValueEnum.y.value
         self.variables[VarKeyEnum.send_notification_title.value] = title
         self.variables[VarKeyEnum.send_notification_subtitle.value] = subtitle
+        return self
```

### Comparing `afwf-0.3.2/afwf/query.py` & `afwf-0.4.1/afwf/query.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/script_filter.py` & `afwf-0.4.1/afwf/script_filter.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/script_filter_object.py` & `afwf-0.4.1/afwf/script_filter_object.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf/workflow.py` & `afwf-0.4.1/afwf/workflow.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/afwf.egg-info/PKG-INFO` & `afwf-0.4.1/afwf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: afwf
-Version: 0.3.2
+Version: 0.4.1
 Summary: A powerful framework enables fast and elegant development of Alfred Workflows in Python.
 Home-page: https://github.com/MacHu-GWU/afwf-project
-Download-URL: https://pypi.python.org/pypi/afwf/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/afwf/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `afwf-0.3.2/preview-icons.rst` & `afwf-0.4.1/preview-icons.rst`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/requirements-doc.txt` & `afwf-0.4.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/setup.py` & `afwf-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/tests/test_enumeration.py` & `afwf-0.4.1/tests/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/tests/test_import.py` & `afwf-0.4.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/tests/test_item.py` & `afwf-0.4.1/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/tests/test_query.py` & `afwf-0.4.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `afwf-0.3.2/tests/test_script_filter.py` & `afwf-0.4.1/tests/test_script_filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 class TestScriptFilter:
     def test_to_script_filter(self):
         sf = ScriptFilter()
         assert sf.to_script_filter() == {"items": []}
 
         sf.items.append(Item(title="option1"))
-        assert sf.to_script_filter() == {
-            "items": [
-                {"title": "option1", "valid": True}
-            ]
-        }
+        assert sf.to_script_filter() == {"items": [{"title": "option1", "valid": True}]}
+
+        sf.send_feedback()
 
 
 if __name__ == "__main__":
     import os
 
     basename = os.path.basename(__file__)
     pytest.main([basename, "-s", "--tb=native"])
```

### Comparing `afwf-0.3.2/tests/test_script_filter_object.py` & `afwf-0.4.1/tests/test_script_filter_object.py`

 * *Files identical despite different names*

