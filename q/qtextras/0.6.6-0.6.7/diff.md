# Comparing `tmp/qtextras-0.6.6.tar.gz` & `tmp/qtextras-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtextras-0.6.6.tar", last modified: Fri Dec  9 07:09:37 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `qtextras-0.6.6.tar` & `qtextras-0.6.7.tar`

### file list

```diff
@@ -1,51 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.972112 qtextras-0.6.6/
--rw-rw-rw-   0        0        0      202 2022-09-20 22:42:55.000000 qtextras-0.6.6/.flake8
--rw-rw-rw-   0        0        0       61 2022-08-05 02:55:24.000000 qtextras-0.6.6/.git-blame-ignore-revs
--rw-rw-rw-   0        0        0       52 2022-08-05 02:55:24.000000 qtextras-0.6.6/.gitignore
--rw-rw-rw-   0        0        0     1321 2022-12-09 07:09:37.972112 qtextras-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      785 2022-09-02 04:05:07.000000 qtextras-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.860047 qtextras-0.6.6/doc/
--rw-rw-rw-   0        0        0      768 2022-09-18 15:34:17.000000 qtextras-0.6.6/doc/ptree.md
--rw-rw-rw-   0        0        0     1369 2022-11-22 04:22:37.000000 qtextras-0.6.6/pyproject.toml
--rw-rw-rw-   0        0        0      140 2022-08-05 02:55:24.000000 qtextras-0.6.6/pytest.ini
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.882392 qtextras-0.6.6/qtextras/
--rw-rw-rw-   0        0        0      412 2022-12-09 07:03:45.000000 qtextras-0.6.6/qtextras/__init__.py
--rw-rw-rw-   0        0        0     9537 2022-12-09 05:28:33.000000 qtextras-0.6.6/qtextras/_funcparse.py
--rw-rw-rw-   0        0        0      268 2022-09-17 15:52:03.000000 qtextras-0.6.6/qtextras/constants.py
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.901454 qtextras-0.6.6/qtextras/examples/
--rw-rw-rw-   0        0        0        0 2022-09-18 15:34:04.000000 qtextras-0.6.6/qtextras/examples/__init__.py
--rw-rw-rw-   0        0        0     2855 2022-09-20 22:42:55.000000 qtextras-0.6.6/qtextras/examples/parameditor.py
--rw-rw-rw-   0        0        0    31569 2022-11-25 03:45:28.000000 qtextras-0.6.6/qtextras/fns.py
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.921323 qtextras-0.6.6/qtextras/misc/
--rw-rw-rw-   0        0        0      192 2022-09-21 00:46:48.000000 qtextras-0.6.6/qtextras/misc/__init__.py
--rw-rw-rw-   0        0        0    17873 2022-09-21 00:09:35.000000 qtextras-0.6.6/qtextras/misc/actionstack.py
--rw-rw-rw-   0        0        0     2568 2022-09-20 22:42:55.000000 qtextras-0.6.6/qtextras/misc/composition.py
--rw-rw-rw-   0        0        0     3172 2022-09-21 00:15:18.000000 qtextras-0.6.6/qtextras/misc/logger.py
--rw-rw-rw-   0        0        0     7402 2022-10-21 21:16:34.000000 qtextras-0.6.6/qtextras/misc/models.py
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.944072 qtextras-0.6.6/qtextras/params/
--rw-rw-rw-   0        0        0      135 2022-09-21 00:05:20.000000 qtextras-0.6.6/qtextras/params/__init__.py
--rw-rw-rw-   0        0        0    37501 2022-12-09 05:28:33.000000 qtextras-0.6.6/qtextras/params/editor.py
--rw-rw-rw-   0        0        0     7022 2022-11-08 14:04:07.000000 qtextras-0.6.6/qtextras/params/optionsdict.py
--rw-rw-rw-   0        0        0    14455 2022-12-09 05:28:33.000000 qtextras-0.6.6/qtextras/params/pgregistered.py
--rw-rw-rw-   0        0        0      835 2022-12-09 05:28:33.000000 qtextras-0.6.6/qtextras/shims.py
--rw-rw-rw-   0        0        0      200 2022-10-27 19:24:02.000000 qtextras-0.6.6/qtextras/typeoverloads.py
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.963139 qtextras-0.6.6/qtextras/widgets/
--rw-rw-rw-   0        0        0      526 2022-09-21 00:26:02.000000 qtextras-0.6.6/qtextras/widgets/__init__.py
--rw-rw-rw-   0        0        0     7197 2022-11-08 14:04:07.000000 qtextras-0.6.6/qtextras/widgets/buttoncollection.py
--rw-rw-rw-   0        0        0     3856 2022-12-09 05:28:33.000000 qtextras-0.6.6/qtextras/widgets/console.py
--rw-rw-rw-   0        0        0     7013 2022-11-05 23:12:31.000000 qtextras-0.6.6/qtextras/widgets/easywidget.py
--rw-rw-rw-   0        0        0    26063 2022-12-01 14:11:57.000000 qtextras-0.6.6/qtextras/widgets/imageviewer.py
--rw-rw-rw-   0        0        0     5025 2022-12-01 14:11:57.000000 qtextras-0.6.6/qtextras/widgets/lineeditor.py
--rw-rw-rw-   0        0        0     9556 2022-11-10 22:30:03.000000 qtextras-0.6.6/qtextras/widgets/loghandlers.py
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.899449 qtextras-0.6.6/qtextras.egg-info/
--rw-rw-rw-   0        0        0     1321 2022-12-09 07:09:37.000000 qtextras-0.6.6/qtextras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2022-12-09 07:09:37.000000 qtextras-0.6.6/qtextras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-09 07:09:37.000000 qtextras-0.6.6/qtextras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-12-09 07:09:37.000000 qtextras-0.6.6/qtextras.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-09 07:09:37.000000 qtextras-0.6.6/qtextras.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-09 07:09:37.972112 qtextras-0.6.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-09 07:09:37.971110 qtextras-0.6.6/tests/
--rw-rw-rw-   0        0        0       39 2022-09-19 02:27:10.000000 qtextras-0.6.6/tests/conftest.py
--rw-rw-rw-   0        0        0     7383 2022-09-20 22:42:55.000000 qtextras-0.6.6/tests/test_actionstack.py
--rw-rw-rw-   0        0        0     1050 2022-11-16 22:24:21.000000 qtextras-0.6.6/tests/test_dockgroup.py
--rw-rw-rw-   0        0        0     2429 2022-11-11 02:28:23.000000 qtextras-0.6.6/tests/test_parameditor.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 qtextras-0.6.7/.flake8
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qtextras-0.6.7/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qtextras-0.6.7/pytest.ini
+-rw-r--r--   0        0        0    65144 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras-0.6.7-py3-none-any.whl
+-rw-r--r--   0        0        0    59816 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras-0.6.7.tar.gz
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 qtextras-0.6.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 qtextras-0.6.7/doc/ptree.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/__init__.py
+-rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/_funcparse.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/constants.py
+-rw-r--r--   0        0        0    31614 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/fns.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/shims.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/typeoverloads.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/examples/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/examples/parameditor.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/misc/__init__.py
+-rw-r--r--   0        0        0    17873 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/misc/actionstack.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/misc/composition.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/misc/logger.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/misc/models.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/params/__init__.py
+-rw-r--r--   0        0        0    38175 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/params/editor.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/params/optionsdict.py
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/params/pgregistered.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/__init__.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/buttoncollection.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/console.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/easywidget.py
+-rw-r--r--   0        0        0    26361 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/imageviewer.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/lineeditor.py
+-rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 qtextras-0.6.7/qtextras/widgets/loghandlers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 qtextras-0.6.7/tests/conftest.py
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 qtextras-0.6.7/tests/test_actionstack.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 qtextras-0.6.7/tests/test_dockgroup.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 qtextras-0.6.7/tests/test_parameditor.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 qtextras-0.6.7/.gitignore
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 qtextras-0.6.7/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 qtextras-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 qtextras-0.6.7/PKG-INFO
```

### Comparing `qtextras-0.6.6/PKG-INFO` & `qtextras-0.6.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-Metadata-Version: 2.1
-Name: qtextras
-Version: 0.6.6
-Summary: High-level widgets and features for scientific Qt GUI development
-Author-email: Nathan Jessurun <ntjessu@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: full
-
-# Qt Extras
-## General Scientific Python Qt GUI Utilities
-
-A collection of Python Qt GUI builders and other functions I've found helpful as I develop
-python mockups.
-
-## Installation
-
-`qtextras` lives in pypi too, so the easiest way to install it is through `pip`:
-
-```bash
-pip install qtextras
-```
-
-Note that a version of Qt must be installed for it to work, such as PyQt5/6 or Pyside2/6.
-PySide6 will also be installed with `pip install qtextras[full]`
-
-Alternatively, you can do so through downloading the repository:
-
-```bash
-git clone https://gitlab.com/s3a/qtextras
-pip install -e ./qtextras # Or ./qtextras[full] as mentioned above
-```
-
-## Usage
-
-Usage will vary depending on the requested capabilities. Check out the `examples`
-folder for some usages
+Metadata-Version: 2.1
+Name: qtextras
+Version: 0.6.7
+Summary: High-level widgets and features for scientific Qt GUI development
+Author-email: Nathan Jessurun <ntjessu@gmail.com>
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.8
+Requires-Dist: numpy>=1.0
+Requires-Dist: pyqtgraph>=0.13.1
+Requires-Dist: ruamel-yaml>=0.17.0
+Provides-Extra: full
+Requires-Dist: pandas>=1.4.0; extra == 'full'
+Requires-Dist: pyside6>=6.2.0; extra == 'full'
+Description-Content-Type: text/markdown
+
+# Qt Extras
+## General Scientific Python Qt GUI Utilities
+
+A collection of Python Qt GUI builders and other functions I've found helpful as I develop
+python mockups.
+
+## Installation
+
+`qtextras` lives in pypi too, so the easiest way to install it is through `pip`:
+
+```bash
+pip install qtextras
+```
+
+Note that a version of Qt must be installed for it to work, such as PyQt5/6 or Pyside2/6.
+PySide6 will also be installed with `pip install qtextras[full]`
+
+Alternatively, you can do so through downloading the repository:
+
+```bash
+git clone https://gitlab.com/s3a/qtextras
+pip install -e ./qtextras # Or ./qtextras[full] as mentioned above
+```
+
+## Usage
+
+Usage will vary depending on the requested capabilities. Check out the `examples`
+folder for some usages
```

### Comparing `qtextras-0.6.6/README.md` & `qtextras-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/doc/ptree.md` & `qtextras-0.6.7/doc/ptree.md`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/pyproject.toml` & `qtextras-0.6.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "qtextras"
 description = "High-level widgets and features for scientific Qt GUI development"
 authors = [
     {name = "Nathan Jessurun", email = "ntjessu@gmail.com"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 dependencies = [
     "numpy            >= 1.0",
-    "pandas           >= 1.0",
-    # Avoid force-uninstalling already-git install versions
-    # Note: Until 0.13.2 release, need commit >= 553287a
-    "pyqtgraph",
+    "pyqtgraph        >= 0.13.1",
     "ruamel.yaml      >= 0.17.0",
 ]
 dynamic = ["version"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 
 [project.optional-dependencies]
 full = [
     "PySide6 >= 6.2.0",
+    "pandas  >= 1.4.0",
 ]
 
-[tool.setuptools.dynamic]
-version = { attr = "qtextras.__version__" }
+[tool.hatch.version]
+path = "qtextras/__init__.py"
 
 [tool.isort]
 profile = "black"
 reverse_relative = true
 combine_as_imports = true
 
 [tool.unimport]
```

### Comparing `qtextras-0.6.6/qtextras/_funcparse.py` & `qtextras-0.6.7/qtextras/_funcparse.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/examples/parameditor.py` & `qtextras-0.6.7/qtextras/examples/parameditor.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/fns.py` & `qtextras-0.6.7/qtextras/fns.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import re
 import typing as t
 from argparse import Namespace
 from contextlib import contextmanager
 from pathlib import Path
 from warnings import warn
 
-import pandas as pd
 import pyqtgraph as pg
 from pyqtgraph.parametertree import InteractiveFunction, Parameter, ParameterTree
 from pyqtgraph.Qt import QT_LIB, QtCore, QtGui, QtWidgets
 
 # -----
 # For ruamel yaml
 # -----
 # Needed for external modules to catch a YamlError
 from ruamel.yaml import YAML, YAMLError  # noqa
 
+from qtextras.shims import pd, requires_pandas
 from qtextras.typeoverloads import FilePath
 
 # -----
 # For Pyyaml
 # -----
 # import yaml
 # from yaml import YAMLError
@@ -185,14 +185,15 @@
         if embed:
             obj.__docObjs__ = kwargs
         return obj
 
     return wrapper
 
 
+@requires_pandas
 def seriesAsFrame(ser: pd.Series):
     return ser.to_frame().T
 
 
 def createAndAddMenuAct(
     mainWin: QtWidgets.QWidget, parentMenu: QtWidgets.QMenu, title: str, asMenu=False
 ) -> t.Union[QtWidgets.QMenu, QtGui.QAction]:
```

### Comparing `qtextras-0.6.6/qtextras/misc/actionstack.py` & `qtextras-0.6.7/qtextras/misc/actionstack.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/misc/composition.py` & `qtextras-0.6.7/qtextras/misc/composition.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/misc/logger.py` & `qtextras-0.6.7/qtextras/misc/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import signal
 import sys
 import typing as t
 import warnings
 
 from pyqtgraph import QtCore, QtWidgets
 
-from qtextras.constants import PrjEnums
+from qtextras.constants import LibraryNamespace
 from qtextras.widgets.loghandlers import DialogHandler
 
 
 class AppLogger(logging.Logger):
     nonCriticalErrors = ()
 
     old_showwarning = None
@@ -22,15 +22,15 @@
         # Define local function to avoid uncollected garbage on pyside2
         def doLog():
             self.log(msg, *args, **kwargs)
 
         QtCore.QTimer.singleShot(0, doLog)
 
     def attention(self, msg, *args, **kwargs):
-        return self.log(PrjEnums.LOG_LVL_ATTN, msg, *args, **kwargs)
+        return self.log(LibraryNamespace.LOG_LEVEL_ATTENTION, msg, *args, **kwargs)
 
     def registerExceptions(
         self,
         win: QtWidgets.QMainWindow = None,
         nonCriticalErrors: t.Sequence[t.Type[Exception] | t.Type[Warning]] = (),
     ):
         self.old_sys_excepthook = sys.excepthook
@@ -67,15 +67,15 @@
         app = QtWidgets.QApplication.instance()
         if etype in [KeyboardInterrupt, SystemExit]:
             app.exit(1)
             app.processEvents()
             raise
 
         if issubclass(etype, self.nonCriticalErrors):
-            level = PrjEnums.LOG_LVL_ATTN
+            level = LibraryNamespace.LOG_LEVEL_ATTENTION
         else:
             level = logging.CRITICAL
         self.log(level, "", exc_info=(etype, evalue, tb))
 
     @classmethod
     def getAppLogger(cls, name=""):
         """
```

### Comparing `qtextras-0.6.6/qtextras/misc/models.py` & `qtextras-0.6.7/qtextras/misc/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import typing as t
 
 import numpy as np
-import pandas as pd
 from pyqtgraph import QtCore
 
-from qtextras.constants import PrjEnums
+from qtextras.constants import LibraryNamespace
+from qtextras.shims import pd, requires_pandas
 
 
+@requires_pandas
 class PandasTableModel(QtCore.QAbstractTableModel):
     """
     Class to populate a table view with a pandas dataframe
     """
 
     sigDataChanged = QtCore.Signal(object)
     defaultEmitDict = {
@@ -75,18 +76,21 @@
         ):
             return self.dataframe.columns[section]
 
     def flags(self, index: QtCore.QModelIndex) -> QtCore.Qt.ItemFlags:
         return QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
 
     def addDfRows(
-        self, rowData: pd.DataFrame, addType=PrjEnums.ADD_TYPE_NEW, emitChange=True
+        self,
+        rowData: pd.DataFrame,
+        addType=LibraryNamespace.ADD_TYPE_NEW,
+        emitChange=True,
     ):
         toEmit = self.defaultEmitDict.copy()
-        if addType == PrjEnums.ADD_TYPE_NEW:
+        if addType == LibraryNamespace.ADD_TYPE_NEW:
             # Treat all components as new -> set their IDs to guaranteed new values
             newIds = np.arange(
                 self._nextRowId, self._nextRowId + len(rowData), dtype=int
             )
             rowData.set_index(newIds, inplace=True, verify_integrity=False)
             # For new data without all columns, add missing values to ensure they're
             # correctly filled
```

### Comparing `qtextras-0.6.6/qtextras/params/editor.py` & `qtextras-0.6.7/qtextras/params/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
     deleted = Signal(list)
     loadRequested = Signal(str)
 
 
 class FileStateManager:
     DEFAULT_STATE_NAME = "Default"
 
+    allowBrowseForLoad = True
+
     def __init__(
         self,
         directory: FilePath | None = None,
         suffix: str = ".param",
     ):
         self.signals = ParameterStateSignals()
         self.directory: Path | None = None
@@ -284,14 +286,20 @@
             self.addSavedStatesToMenu(parentMenu)
 
         for name in dirGlob:
             # glob returns entire filepath, so keep only filename as layout name
             curAction = parentMenu.addAction(name)
             curAction.triggered.connect(functools.partial(loaderFunc, name))
 
+        if self.allowBrowseForLoad:
+            parentMenu.addSeparator()
+            parentMenu.addAction("Browse...").triggered.connect(
+                functools.partial(self.signals.loadRequested.emit, "")
+            )
+
         if keepUpdated:
             self.signals.created.connect(populateFunc)
             self.signals.deleted.connect(populateFunc)
 
 
 class ParameterEditor(QtWidgets.QWidget):
     sigStateCreated = Signal(str)
@@ -549,14 +557,24 @@
         self.stateName = self.stateManager.formatFileName(stateName).stem
 
         return self.getParameterValues()
 
     def onLoadRequested(self, stateName):
         # First check for extra keys, will be the case if 'children' is one of the
         # keys. Can't do value-loading in that case, must do state-loading instead
+        if not stateName:
+            # No state name given, get from the user
+            stateName, _ = QtWidgets.QFileDialog.getOpenFileName(
+                self,
+                "Load State",
+                str(self.directory),
+                f"State files (*{self.stateManager.suffix});; All files (*)",
+            )
+            if not stateName:
+                return
         stateDict = self.stateManager.loadState(stateName)
         if not stateDict:
             # File didn't exist or there was a problem during loading
             return
         if "children" in stateDict:
             # Bug in pyqtgraph restore state doesn't play nice when parameters have
             # connected functions outside the parameter item, so re-implement without
@@ -666,18 +684,18 @@
             Template for the run action. See ``Interactor.runActionTemplate`` for
             more details.
         parametersNeedRunKwargs
             Passed to ``InteractiveFunction.parametersNeedRunKwargs``. If ``None``,
             the function's original attribute value is unchanged.
         container
             The container in which to put child parameters from the registered function.
-            This has a similar effect to calling `registerProps` on each of the
+            This has a similar effect to calling `registerParameterList` on each of the
             function arguments with this container. *Note*: while the former will
-            register props according to the `parameter` OptionsDict, this will register
-            to the container using the raw parameter name. A KeyError is raised when
+            register according to the `parameter` OptionsDict, this function will register
+            to the container using the string parameter name. A KeyError is raised when
             a new parameter name clashes with something already in the container.
         **kwargs
             All additional kwargs are passed to InteractiveFunction when wrapping the
             function. If an InteractiveFunction is passed in, ``kwargs`` are passed to
             the interactor.
         """
         if interactor is None:
@@ -930,21 +948,22 @@
         return [
             self.treeButtonsWidget,
             self.tree,
             [self.saveAsButton, self.loadButton],
         ]
 
     def _createLoadButton(self):
-        self.loadButton = QtWidgets.QToolButton()
+        self.loadButton = QtWidgets.QToolButton(self)
         self.loadButton.setText("Load...")
         pol = QtWidgets.QSizePolicy.Policy
         self.loadButton.setSizePolicy(pol.MinimumExpanding, pol.Fixed)
-        self.loadButton.setMenu(QtWidgets.QMenu(self.loadButton))
+        menu = QtWidgets.QMenu(self.loadButton)
+        self.loadButton.setMenu(menu)
         self.loadButton.setPopupMode(QtWidgets.QToolButton.InstantPopup)
-        self.stateManager.addSavedStatesToMenu(self.loadButton.menu())
+        self.stateManager.addSavedStatesToMenu(menu)
         return self.loadButton
 
     def __repr__(self):
         selfCls = type(self)
         oldName: str = super().__repr__()
         # Remove module name for brevity
         oldName = oldName.replace(
```

### Comparing `qtextras-0.6.6/qtextras/params/optionsdict.py` & `qtextras-0.6.7/qtextras/params/optionsdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import builtins
 from typing import Optional, Sequence
 
 import numpy as np
-import pandas as pd
+
+from qtextras.shims import pd, requires_pandas
 
 
 def _rescale(data, min_, max_):
     # Handle nan values
     rng = max_ - min_
     if rng == 0:
         return np.ones_like(data)
@@ -88,14 +89,15 @@
     def __hash__(self):
         # Since every parameter within a group will have a unique name, just the name is
         # sufficient to form a proper hash
         return hash(
             self.comparator(self),
         )
 
+    @requires_pandas
     def toNumeric(self, data: Sequence, rescale=False, returnMapping=False):
         """
         Useful for converting string-like or list-like parameters to integer
         representations.
 
         If self's `value` is non-numeric data (e.g. strings):
            - First, the parameter is searched for a 'limits' property. This will
```

### Comparing `qtextras-0.6.6/qtextras/params/pgregistered.py` & `qtextras-0.6.7/qtextras/params/pgregistered.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,15 @@
         interactor: Interactor = None,
         stageInputOptions: dict = None,
         **metaOptions,
     ):
         if isinstance(stage, ChainedActionGroupParameter):
             # Child pipelines should only be activatable by the parents
             stage.setButtonOpts(visible=False)
+            stage.setOpts(**metaOptions)
             return self.addChild(stage)
         elif callable(stage) and not isinstance(stage, InteractiveFunction):
             stage = InteractiveFunction(stage)
         elif not isinstance(stage, InteractiveFunction):
             raise TypeError("Stage must be callable")
 
         stage: InteractiveFunction
```

### Comparing `qtextras-0.6.6/qtextras/widgets/__init__.py` & `qtextras-0.6.7/qtextras/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/widgets/buttoncollection.py` & `qtextras-0.6.7/qtextras/widgets/buttoncollection.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/widgets/console.py` & `qtextras-0.6.7/qtextras/widgets/console.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/widgets/easywidget.py` & `qtextras-0.6.7/qtextras/widgets/easywidget.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/widgets/imageviewer.py` & `qtextras-0.6.7/qtextras/widgets/imageviewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import typing as t
 
 import numpy as np
-import pandas as pd
 import pyqtgraph as pg
 from _warnings import warn
 from pyqtgraph import QtCore, QtGui, QtWidgets
 from pyqtgraph.graphicsItems.LegendItem import ItemSample
 from pyqtgraph.graphicsItems.ScatterPlotItem import drawSymbol
 from pyqtgraph.graphicsItems.ViewBox.ViewBoxMenu import ViewBoxMenu
 
 from qtextras import fns
 from qtextras._funcparse import bindInteractorOptions as bind
 from qtextras.misc import CompositionMixin
 from qtextras.params import ParameterEditor, RunOptions
+from qtextras.shims import pd, requires_pandas
 from qtextras.typeoverloads import FilePath
 from qtextras.widgets.easywidget import EasyWidget
 
 
 class ImageViewer(CompositionMixin, pg.PlotWidget):
     sigMouseMoved = QtCore.Signal(object)  # ndarray(int, int) xy pos rel. to image
 
@@ -30,16 +30,16 @@
         under the mouse
         """
         self.toolsEditor = ParameterEditor(name="Region Tools")
         vb = self.getViewBox()
         self.menu: QtWidgets.QMenu = vb.menu
         self.oldVbMenu: ViewBoxMenu = vb.menu
         # Disable default menus
-        self.plotItem.ctrlMenu = None
-        self.sceneObj.contextMenu = None
+        # self.plotItem.ctrlMenu = None
+        # self.sceneObj.contextMenu = None
 
         self.setAspectLocked(True)
         vb.invertY()
 
         # -----
         # IMAGE
         # -----
@@ -176,86 +176,84 @@
     def paint(self, p: QtGui.QPainter, *args):
         br = self.boundingRect()
         p.setPen(self.opts["pen"])
         p.setBrush(self.opts["brush"])
         p.drawRoundedRect(br, 5, 5)
 
 
+@requires_pandas
 class MaskCompositor(ImageViewer):
     _cachedCmapLimits = None
 
-    def __init__(self, img: np.ndarray = None):
+    def __init__(self, img: np.ndarray = None, registerDefaultFunctions=False):
         super().__init__()
         # -----
         # Create properties
         # -----
         self.masksParameter = fns.getParameterChild(
             self.toolsEditor.rootParameter, "Overlays"
         )
         if self._cachedCmapLimits is None:
             # Set at class level to cache for new instances too
             type(self)._cachedCmapLimits = fns.listAllPgColormaps()
 
         self.legend = CompositorLegend(
             offset=(5, 5), horSpacing=5, brush="#ccce", pen="k"
         )
-        self.recordDf = pd.DataFrame(
-            columns=["name", "item", "opacity", "isMask"]
-        ).set_index("name")
+        self.recordDf = (
+            pd.DataFrame(columns=["name", "item", "opacity", "isMask"])
+            .set_index("name")
+            .astype(dict(isMask="bool"))
+        )
         # Initialized in clearOverlays and updateLabelMap. Given here to avoid
         # intellisense warnings
         self.inUseLabelValues = (
             self.scatterSer
-        ) = self.backgroundValues = self.labelToNameMapping = None
+        ) = self.backgroundValues = self.labelNameMap = None
         self.updateLabelMap()
         self.legendFontArgs = {"size": "11pt", "color": "k", "bold": True}
         self.curZ = 2
 
         # -----
         # Configure relationships
         # -----
         self.legend.setParentItem(self.plotItem)
+        self.legend.hide()
         self.viewbox: pg.ViewBox = self.getViewBox()
 
+        self.compositorMenu = self.menu.addMenu("Compositor Options")
+        for func in self.toggleLegendVisible, self.toggleImageVisible:
+            self.compositorMenu.addAction(fns.nameFormatter(func.__name__), func)
+
         self.allVisible = True
         # for ax in 'left', 'bottom', 'right', 'top':
         #   self.mainImage.plotItem.hideAxis(ax)
         # self.mainImage.setContentsMargins(0, 0, 0, 0)
+        self.propertiesProc = self.toolsEditor.registerFunction(
+            self.setOverlayProperties,
+            name=fns.nameFormatter("overlayProperties"),
+            runOptions=RunOptions.ON_CHANGED,
+            colormap=dict(limits=self._cachedCmapLimits),
+            fullLabelMapColors=dict(ignore=True),
+        )
+
+        if registerDefaultFunctions:
+            self.registerDefaultFunctions()
 
-        def newFmt(name):
-            if name.startswith("set"):
-                name = name.replace("set", "")
-            name = fns.pascalCaseToTitle(name)
-            return name
-
-        with fns.nameFormatter.set(newFmt):
-            self.propertiesProc = self.toolsEditor.registerFunction(
-                self.setOverlayProperties,
-                runOptions=RunOptions.ON_CHANGED,
-                colormap=dict(limits=self._cachedCmapLimits),
-                fullLabelMapColors=dict(ignore=True),
-            )
-            self.toolsEditor.registerFunction(self.save)
-            self.toolsEditor.registerFunction(
-                lambda: self.imageItem.setVisible(not self.imageItem.isVisible()),
-                name="Toggle Image Visible",
-            )
-            self.toolsEditor.registerFunction(
-                lambda: self.legend.setVisible(not self.legend.isVisible()),
-                name="Toggle Legend Visible",
-            )
-            self.toolsEditor.registerFunction(
-                self.toggleAllVisible, parent=("Overlays",)
-            )
         if img is not None:
             self.setImage(img)
         self.clearOverlays()
 
+    def registerDefaultFunctions(self):
+        self.toolsEditor.registerFunction(self.save)
+        self.toolsEditor.registerFunction(self.toggleImageVisible)
+        self.toolsEditor.registerFunction(self.toggleAllVisible, parent=("Overlays",))
+
     @staticmethod
-    def _createLabelToNameMapping(data=None):
+    def _createLabelNameMap(data=None):
         """
         Helper method to ensure proper dtypes when making a legend series. Helps avoid
         pitfalls with empty data, etc.
         """
         if data is None:
             data = []
         ser = pd.Series(data, dtype=str)
@@ -285,15 +283,18 @@
             self.clearOverlays()
 
     def setImage(self, *args, **kwargs):
         super().setImage(*args, **kwargs)
         self._updateLegendPos()
 
     def _addRecord(self, rec: pd.Series, update=True):
+        # Fix futurewarning from pandas 1.5 regarding bool assignment. It's a false positive,
+        # But the FutureWarnings can crowd the terminal
         self.recordDf.loc[rec.name] = rec
+        self.recordDf = self.recordDf.astype(dict(isMask="bool"))
         self.curZ += 1
 
         self._addItemCtrls(rec)
 
         if update:
             self._updateGraphics()
 
@@ -302,15 +303,15 @@
         name = self._getUniqueName(kwargs.pop("name", None))
         update = kwargs.pop("update", True)
         kwargs.setdefault("isMask", False)
         newRecord = dict(item=item, **kwargs)
         item.setZValue(self.curZ + 1)
         self.viewbox.addItem(item)
 
-        rec = pd.Series(newRecord, name=name)
+        rec = pd.Series(newRecord, name=name, dtype=object)
         self._addRecord(rec, update)
 
     def _getUniqueName(self, baseName: str = None):
         if baseName is None:
             baseName = "[No Name]"
         ii = 2
         name = baseName
@@ -403,19 +404,19 @@
         useFullLabelMap
             If *True*, guarantees that every entry in the label->name mapping will be
             present in the legend.
         updateOverlays
             If *True*, the image overlay properties will be refereshed
         """
         if useFullLabelMap:
-            labels = np.union1d(self.inUseLabelValues, self.labelToNameMapping.index)
+            labels = np.union1d(self.inUseLabelValues, self.labelNameMap.index)
         else:
             labels = self.inUseLabelValues
         labels = np.setdiff1d(labels, self.backgroundValues)
-        names = self.labelToNameMapping.reindex(labels)
+        names = self.labelNameMap.reindex(labels)
         needsEntry = names.isna()
         names[needsEntry] = names.index[needsEntry].map(str)
         self.legend.clear()
         self.scatterSer = pd.Series(
             [None] * len(names), index=names.index, dtype=object
         )
         # Make sure alpha is not carried over
@@ -448,15 +449,15 @@
             *False* if several updates will happen in sequence.
         """
         if labelMap is None:
             labelMap = {}
         if np.isscalar(backgroundValues):
             backgroundValues = [backgroundValues]
         self.backgroundValues = np.array(backgroundValues)
-        self.labelToNameMapping = self._createLabelToNameMapping(labelMap)
+        self.labelNameMap = self._createLabelNameMap(labelMap)
         if updateOverlays:
             self._updateGraphics()
 
     @bind(opacity=dict(limits=[0, 1], step=0.1), colormap=dict(type="popuplineeditor"))
     def setOverlayProperties(
         self, colormap="magma", opacity=0.6, fullLabelMapColors=False
     ):
@@ -468,52 +469,49 @@
         colormap
             Colormap to use for the overlay. Should be a string that names a pyqtgraph
             colormap
         opacity
             Opacity of the overlay, from 0 (transparent) to 1 (opaque)
         fullLabelMapColors
             If *True*, enough colors will be generated for all labels in
-            ``self.labelToNameMapping``. If *False*, only enough colors will be
+            ``self.labelNameMap``. If *False*, only enough colors will be
             generated for the labels in the added masks.
         """
         maskIdxs = self.recordDf["isMask"].to_numpy(bool)
         cmap = fns.getAnyPgColormap(colormap)
         labelValues = self.scatterSer.index.values
         if fullLabelMapColors:
-            labelValues = np.union1d(labelValues, self.labelToNameMapping.index.values)
+            labelValues = np.union1d(labelValues, self.labelNameMap.index.values)
         if not len(labelValues):
             pass  # return
         if cmap is None:
             raise ValueError(f"Invalid colormap: {colormap}")
         colors = cmap.getLookupTable(nPts=len(labelValues), alpha=True)
         colors[:, -1] = opacity * 255
         # If a labelmap has entries, try to scale the colormap to contain all
         # possibilities
-        numEntries = (
-            max(
-                np.max(labelValues, initial=-1),
-                np.max(self.labelToNameMapping.index.values, initial=-1),
-            )
-            + 1
+        numEntries = max(
+            np.max(labelValues, initial=1),
+            np.max(self.labelNameMap.index.to_numpy(), initial=1),
         )
-        lut = np.zeros((numEntries, 4), dtype="uint8")
+        lut = np.zeros((numEntries + 1, 4), dtype="uint8")
         lut[labelValues] = colors
         bgValsInLut = self.backgroundValues[self.backgroundValues < len(lut)]
         lut[bgValsInLut] = 0
         for idx, scat in self.scatterSer.items():
             # Make sure alpha is not carried over
             color = lut[idx, :-1]
             brush, pen = pg.mkBrush(color), pg.mkPen(color)
             scat.setData(symbol="s", brush=brush, pen=pen, width=5)
         for _, maskRec in self.recordDf[maskIdxs].iterrows():
             itemOpacity = maskRec["opacity"]
             if itemOpacity < 0:
                 itemOpacity = opacity
             maskRec["item"].setOpts(
-                lut=lut, opacity=itemOpacity, levels=[0, numEntries - 1]
+                lut=lut, opacity=itemOpacity, levels=[0, numEntries]
             )
         # Handle non-mask items who still want controlled opacity
         for _, rec in self.recordDf[
             (~maskIdxs) & self.recordDf["opacity"] < 0
         ].iterrows():
             rec["item"].setOpts(opacity=opacity)
         self.setLegendFontStyle(**self.legendFontArgs)
@@ -642,14 +640,20 @@
             exportScene.render(painter)
             self.legend.setScale(1 / oldScale)
             painter.restore()
         finally:
             self.legend.setParentItem(self.plotItem)
             self.legend.autoAnchor(oldPos, relative=False)
 
+    def toggleLegendVisible(self):
+        self.legend.setVisible(not self.legend.isVisible())
+
+    def toggleImageVisible(self):
+        self.imageItem.setVisible(not self.imageItem.isVisible())
+
     def __getstate__(self):
         ret = dict(
             image=self.imageItem.image,
             legendVisible=self.legend.isVisible(),
         )
         if len(self.recordDf):
             ret["recordDf"] = self.recordDf
```

### Comparing `qtextras-0.6.6/qtextras/widgets/lineeditor.py` & `qtextras-0.6.7/qtextras/widgets/lineeditor.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/qtextras/widgets/loghandlers.py` & `qtextras-0.6.7/qtextras/widgets/loghandlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         # For some reason, width doesn't set properly here
         fadeMsg.setFixedWidth(fadeMsg.sizeHint().width())
         fadeMsg.setAlignment(QtCore.Qt.AlignCenter)
         fadeMsg.setAttribute(QtCore.Qt.WidgetAttribute.WA_TransparentForMouseEvents)
         parent: QtWidgets.QMainWindow = self.getWindow()
         if parent is not None:
             metrics = fadeMsg.fontMetrics()
-            padding = (parent.width() - metrics.width(msg)) // 2
+            padding = (parent.width() - metrics.boundingRect(msg).width()) // 2
             msgX = padding
             # Make sure multiple messages don't overlap
             msgY = int(0.05 * parent.height())
             msgY += self.getUniqueLblOffset(msgY)
             fadeMsg.move(msgX, msgY)
         anim = self.makeAnimation(fadeMsg, timeout_ms)
         # 10 fps
```

### Comparing `qtextras-0.6.6/tests/test_actionstack.py` & `qtextras-0.6.7/tests/test_actionstack.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/tests/test_dockgroup.py` & `qtextras-0.6.7/tests/test_dockgroup.py`

 * *Files identical despite different names*

### Comparing `qtextras-0.6.6/tests/test_parameditor.py` & `qtextras-0.6.7/tests/test_parameditor.py`

 * *Files identical despite different names*

