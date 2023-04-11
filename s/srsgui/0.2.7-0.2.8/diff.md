# Comparing `tmp/srsgui-0.2.7.tar.gz` & `tmp/srsgui-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ryn3s73s\srsgui-0.2.7.tar", last modified: Mon Apr 10 18:10:58 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-7qun3s1f\srsgui-0.2.8.tar", last modified: Tue Apr 11 18:06:49 2023, max compression
```

## Comparing `srsgui-0.2.7.tar` & `srsgui-0.2.8.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.7/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3330 2023-04-10 18:10:58.659996 srsgui-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.590006 srsgui-0.2.7/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.600037 srsgui-0.2.7/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.609999 srsgui-0.2.7/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 18:10:58.659996 srsgui-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.609999 srsgui-0.2.7/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-04-10 18:09:46.000000 srsgui-0.2.7/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.7/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.584070 srsgui-0.2.7/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.629989 srsgui-0.2.7/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.7/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9583 2023-04-10 17:21:10.000000 srsgui-0.2.7/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.629989 srsgui-0.2.7/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.7/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.640009 srsgui-0.2.7/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.7/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.649978 srsgui-0.2.7/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3489 2023-04-10 16:08:39.000000 srsgui-0.2.7/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.7/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     7833 2023-04-10 17:30:59.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5161 2023-04-10 16:05:18.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     4071 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4803 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.7/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.7/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.7/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.7/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.8/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 18:06:49.463283 srsgui-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.373332 srsgui-0.2.8/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.393348 srsgui-0.2.8/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.403325 srsgui-0.2.8/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 18:06:49.463283 srsgui-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.403325 srsgui-0.2.8/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 18:05:11.000000 srsgui-0.2.8/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.8/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.363366 srsgui-0.2.8/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.423305 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.423305 srsgui-0.2.8/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.8/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.433300 srsgui-0.2.8/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.8/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.8/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.433300 srsgui-0.2.8/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.8/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.8/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.453288 srsgui-0.2.8/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.8/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     2931 2023-04-11 17:36:09.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.8/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.8/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.8/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.8/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.8/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.8/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.7/.gitignore` & `srsgui-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/LICENSE.txt` & `srsgui-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/PKG-INFO` & `srsgui-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.7
+Version: 0.2.8
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.7/README.md` & `srsgui-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/Makefile` & `srsgui-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/make.bat` & `srsgui-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.8/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.8/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.8/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.8/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.8/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.8/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.8/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.8/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.8/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.8/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/conf.py` & `srsgui-0.2.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/create-project.rst` & `srsgui-0.2.8/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/create-task.rst` & `srsgui-0.2.8/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/define-instrument.rst` & `srsgui-0.2.8/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/example.rst` & `srsgui-0.2.8/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/index.rst` & `srsgui-0.2.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/installation.rst` & `srsgui-0.2.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.8/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/srsgui.inst.rst` & `srsgui-0.2.8/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/srsgui.task.rst` & `srsgui-0.2.8/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.8/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/docs/source/srsgui.ui.rst` & `srsgui-0.2.8/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/pyproject.toml` & `srsgui-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/__init__.py` & `srsgui-0.2.8/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.7"  # Global version number
+__version__ = "0.2.8"  # Global version number
```

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/__init__.py` & `srsgui-0.2.8/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/commands.py` & `srsgui-0.2.8/srsgui/inst/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self._set_convert_function = None
 
         self._value = ''
         self.default_value = default_value
         if default_value:
             self._value = default_value
         self.fmt = ''  # format for string conversion
-                       # '.3f' , '10.3e', 's', 'd', 'x'
+                       # '.3f' , '10.3e', 'd', 'x'
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
```

### Comparing `srsgui-0.2.7/srsgui/inst/communications/interface.py` & `srsgui-0.2.8/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.8/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.8/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.8/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/component.py` & `srsgui-0.2.8/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/exceptions.py` & `srsgui-0.2.8/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/inst/indexcommands.py` & `srsgui-0.2.8/srsgui/inst/indexcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,16 @@
 
 class DictIndexCommand(IndexCommand):
     """
     Descriptor for a remote command to
     **set** and **query** using a conversion dictionary
     """
 
-    def __init__(self, remote_command_name, set_dict, index_max, index_min=0, index_dict=None, get_dict=None, unit=''):
+    def __init__(self, remote_command_name, set_dict, index_max, index_min=0,
+                 index_dict=None, get_dict=None, unit=''):
         super().__init__(remote_command_name, index_max, index_min, index_dict)
         self.set_dict = set_dict
         if get_dict is None:
             self.get_dict = self.set_dict
         self.key_type = type(list(set_dict.keys())[0])
         self.value_type = type(list(set_dict.values())[0])
```

### Comparing `srsgui-0.2.7/srsgui/inst/instrument.py` & `srsgui-0.2.8/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/task/callbacks.py` & `srsgui-0.2.8/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/task/config.py` & `srsgui-0.2.8/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/task/inputs.py` & `srsgui-0.2.8/srsgui/task/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,16 @@
                 li.append(str(num))
             except:
                 raise ValueError(msg.format(octet, self.value))
         return '.'.join(li)
 
 
 class CommandInput(IntegerInput):
-    def __init__(self, cmd_name, cmd_instance):
-        super().__init__(0)
+    def __init__(self, cmd_name, cmd_instance, default_value=None):
+        super().__init__(default_value)
 
         self.inst_name = ''
         self.cmd_name = cmd_name
         self.cmd_instance = cmd_instance
         self.cmd = ''
 
     def set_inst_name(self, inst_name):
```

### Comparing `srsgui-0.2.7/srsgui/task/sessionhandler.py` & `srsgui-0.2.8/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/task/task.py` & `srsgui-0.2.8/srsgui/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Image file for parent to display instead of the default logo image when the task is selected.
     """
 
     def __init__(self, parent=None):
         super().__init__()
         self.parent = parent
 
-        self._keep_running = False
+        self._keep_running = False  # flag to tell if the task instance is running
         self._aborted = False
         self._error_raised = False
         self._task_passed = True
         self._log_error_detail = False  # Enables logging traceback information
 
         self.name = 'Base Task'
         self.logger_prefix = ''  # used for logger name for multi-threaded tasks
@@ -271,14 +271,23 @@
         frequently. Stop if it returns False.
         """
 
         if self._keep_running:
             self._aborted = True
             self._keep_running = False
 
+    def delay(self, seconds):
+        """
+        Check if the task is stopped and wait for the given seconds.
+        """
+        if not self._keep_running:
+            raise KeyboardInterrupt('Task is stopped')
+        else:
+            time.sleep(seconds)
+
     def set_session_handler(self, session_handler):
         """
         Parent should set a session handler for Task to use file output.
         """
         self.session_handler = session_handler
 
     def set_callback_handler(self, callback_handler: Callbacks):
```

### Comparing `srsgui-0.2.7/srsgui/task/taskresult.py` & `srsgui-0.2.8/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandhandler.py` & `srsgui-0.2.8/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandterminal.py` & `srsgui-0.2.8/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 
 import sys
 import math
-from srsgui.ui.qt.QtWidgets import QApplication, QWidget, QSpinBox, QDoubleSpinBox, QLabel, QFormLayout
-from srsgui.ui.qt.QtCore import Qt
+
+from srsgui.ui.qt.QtCore import Qt, Signal
+from srsgui.ui.qt.QtWidgets import QApplication, QWidget, QSpinBox, QDoubleSpinBox, \
+                                   QLabel, QFormLayout, QWidget, QPushButton, \
+                                   QHBoxLayout, QSpacerItem, QSizePolicy
 
 
 class IntegerSpinBox(QSpinBox):
     """
     Adjust step size depending on the cursor postion
     """
-    
-    def stepBy(self, steps):        
+
+    def stepBy(self, steps):
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
         sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
-        
+
         exponent = sep_pos - cur_pos
-            
-        single_step = 10 ** exponent        
+
+        single_step = 10 ** exponent
         self.setSingleStep(single_step)
-        
+
         super().stepBy(steps)
 
         self.lineEdit().deselect()
-        
+
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
-        
+
         text = self.lineEdit().text()
         new_sep_pos = len(text)
-        
-        new_cur_pos = cur_pos + new_sep_pos - sep_pos        
+
+        new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
 class FloatSpinBox(QDoubleSpinBox):
     """
@@ -94,79 +97,60 @@
                 prec = self.decimals
         except Exception as e:
             print(e)
         self.precision = prec
         format_string = '{:.' + str(prec) + 'f}'
         text = format_string.format(value)
         return text
-    
-    def stepBy(self, steps):        
+
+    def stepBy(self, steps):
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
         sep_pos = text.find('.')
         if sep_pos < 0:
             sep_pos = len(text)
-            
+
         if cur_pos < min_pos:
             return
-        
+
         exponent = sep_pos - cur_pos
         if exponent == -1:
             cur_pos += 1
-            
+
         if exponent < -1:
             exponent += 1
-            
-        single_step = 10 ** exponent        
+
+        single_step = 10 ** exponent
         self.setSingleStep(single_step)
-        
+
         super().stepBy(steps)
 
         self.lineEdit().deselect()
-        
+
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
-        
+
         text = self.lineEdit().text()
         new_sep_pos = text.find('.')
         if new_sep_pos < 0:
             new_sep_pos = len(text)
-        
-        new_cur_pos = cur_pos + new_sep_pos - sep_pos        
+
+        new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
-class MainWindow(QWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.setWindowTitle('PyQt QSpinBox')
-        self.setMinimumWidth(300)
-
-        # create a grid layout
-        layout = QFormLayout()
-        self.setLayout(layout)
-
-        amount = FloatSpinBox(minimum=-100, maximum=1000, value=20, prefix='$')
-
-        amount.valueChanged.connect(self.update)
-
-        self.result_label = QLabel('', self)
-
-        layout.addRow('Amount:', amount)
-        layout.addRow(self.result_label)
-
-        # show the window
-        self.show()
-
-    def update(self, value):
-        self.result_label.setText(f'Current Value: {value:.3f}')
-
+class RunButton(QWidget):
+    pressed = Signal()
 
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-    window = MainWindow()
-    sys.exit(app.exec_())
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        layout = QHBoxLayout(self)
+        layout.setContentsMargins(1, 1, -1, 1)
+        self.button = QPushButton('Run', self)
+        spacer = QSpacerItem(100, 10, QSizePolicy.Expanding, QSizePolicy.Minimum)
+        layout.addWidget(self.button)
+        layout.addItem(spacer)
+        self.button.pressed.connect(self.pressed)
```

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.8/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
 from srsgui.ui.qt.QtWidgets import QWidget
 
-from .ui_commandcapturewidget import Ui_CommandCaptureWidget
-
+from .ui_commandtreewidget import Ui_CommandTreeWidget
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 
 logger = logging.getLogger(__name__)
 
 
-class CommandTreeWidget(QWidget, Ui_CommandCaptureWidget):
+class CommandTreeWidget(QWidget, Ui_CommandTreeWidget):
     def __init__(self, parent=None):
         super(CommandTreeWidget, self).__init__(parent)
         self.parent = parent
         self.setupUi(self)
 
         self.inst = None
         self.name = None
@@ -43,67 +42,74 @@
         self.collapse_button.clicked.connect(self.on_collapse_clicked)
 
     def set_inst(self, name, inst):
         self.inst = inst
         self.name = name
 
     def on_query_only_changed(self, state):
-        self.query_only_included = state
-        self.update_item_display()
-
-    def update_item_display(self, parent=QModelIndex()):
-        for i in range(self.model.rowCount(parent)):
-            index = self.model.index(i, 0, parent)
-            self.update_item_display(index)
-
-            item = index.internalPointer()
-            query_only = set_only = is_method = is_excluded = False
-            if not self.query_only_included:
-                if not item.set_enable and item.get_enable:
-                    query_only = True
-            if not self.set_only_included:
-                if item.set_enable and not item.get_enable:
-                    set_only = True
-            if not self.method_included:
-                if item.is_method:
-                    is_method = True
-            if not self.excluded_included:
-                if item.excluded:
-                    is_excluded = True
-            state = query_only or set_only or is_method or is_excluded
-            self.tree_view.setRowHidden(i, parent, state)
+        self.tree_view.query_only_included = state
+        self.tree_view.update_item_display()
 
     def on_set_only_changed(self, state):
-        self.set_only_included = state
-        self.update_item_display()
+        self.tree_view.set_only_included = state
+        self.tree_view.update_item_display()
 
     def on_excluded_changed(self, state):
-        self.excluded_included = state
-        self.update_item_display()
+        self.tree_view.excluded_included = state
+        self.tree_view.update_item_display()
 
     def on_method_changed(self, state):
-        self.method_included = state
-        self.update_item_display()
+        self.tree_view.method_included = state
+        self.tree_view.update_item_display()
 
     def on_raw_command_changed(self, state):
-        self.show_raw_command = state
-        self.model.show_raw_remote_command = self.show_raw_command
+        self.tree_view.show_raw_command = state
+        self.model.show_raw_remote_command = self.tree_view.show_raw_command
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
                 self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
-                self.update_item_display()
+                self.tree_view.update_item_display()
+                self.tree_view.connect_methods_to_buttons()
+
             except Exception as e:
                 logger.error(f'Failed to load command tree from {self.name}: {e}')
         else:
             logger.warning(f' {self.name} is NOT connected.')
 
     def on_expand_clicked(self):
         self.tree_view.expandAll()
 
     def on_collapse_clicked(self):
         self.tree_view.collapseAll()
+
+
+if __name__ == '__main__':
+    import sys
+    from srsgui.ui.qt.QtWidgets import QApplication, QHeaderView
+    from srsinst.sr860 import SR860
+
+    app = QApplication(sys.argv)
+
+    widget = CommandTreeWidget()
+
+    inst = SR860('tcpip', '172.25.70.129')
+    inst.query_text(' ')
+
+    widget.set_inst('lockin', inst)
+
+    # print(inst.check_id())
+    # inst.comm.set_callbacks(print, print)
+
+    # widget.model.load(inst)
+
+    widget.show()
+
+    widget.tree_view.header().setSectionResizeMode(0, QHeaderView.Stretch)
+    widget.resize(600, 400)
+
+    app.exec_()
```

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.8/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.8/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/connectdlg.py` & `srsgui-0.2.8/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.8/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/dockhandler.py` & `srsgui-0.2.8/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/inputpanel.py` & `srsgui-0.2.8/srsgui/ui/inputpanel.py`

 * *Files 14% similar despite different names*

```diff
@@ -112,14 +112,16 @@
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, DictCommand) or \
                          issubclass(p.cmd_instance.__class__, DictIndexCommand):
                         widget = QComboBox()
                         item_list = map(str, p.cmd_instance.set_dict.keys())
                         widget.addItems(item_list)
+                        if p.value is None:
+                            p.value = 0
                         widget.setCurrentIndex(p.value)
                         p.text = widget.currentText()
 
                     else:
                         widget = QLineEdit()
 
                     self.command_dict[p.cmd] = widget
@@ -193,23 +195,49 @@
             logger.debug("{} updated".format(self.__class__.__name__))
         except Exception as e:
             logger.error(e)
 
     def on_default(self):
         try:
             params = self.task_class.input_parameters
-            for i in params.keys():
-                params[i].value = params[i].default_value
-                widget = getattr(self, i, None)
-                if type(widget) == QLineEdit:
-                    widget.setText(params[i].default_value)
-                elif type(widget) == QComboBox:
-                    widget.setCurrentIndex(params[i].default_value)
+            for name in params.keys():
+                if params[name].default_value is None:
+                    continue
+                widget = getattr(self, name, None)
+                cmd = None
+                if type(widget) == QLineEdit and type(params[name].default_value) == str:
+                    params[name].value = params[name].default_value
+                    widget.setText(params[name].default_value)
+                    if type(params[name]) == CommandInput:
+                        cmd = '{} = "{}"'.format(params[name].cmd, params[name].default_value)
+                elif type(widget) == QComboBox and type(params[name].default_value) == int:
+                    params[name].value = params[name].default_value
+                    widget.setCurrentIndex(params[name].default_value)
+                    params[name].text = widget.currentText()
+                    if type(params[name]) == CommandInput:
+                        if hasattr(params[name].cmd_instance, 'key_type') and \
+                           getattr(params[name].cmd_instance, 'key_type') == 'int':
+                            cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
+                        else:
+                            cmd = '{} = "{}"'.format(params[name].cmd, params[name].text)
+                elif type(widget) == QSpinBox and type(params[name].default_value) == int:
+                    params[name].value = params[name].default_value
+                    widget.setValue(params[name].default_value)
+                    if type(params[name]) == CommandInput:
+                        cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
+                elif type(widget) == QDoubleSpinBox and type(params[name].default_value) == float:
+                    params[name].value = params[name].default_value
+                    widget.setValue(params[name].default_value)
+                    if type(params[name]) == CommandInput:
+                        cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
                 else:
-                    widget.setValue(params[i].default_value)
+                    logger.error('error to reset "{}" to default, {}'.
+                                 format(name, params[name].default_value))
+                if cmd:
+                    self.command_handler.process_command(cmd, '')
             logger.debug("{} reset to default".format(self.__class__.__name__))
         except Exception as e:
             logger.error(e)
 
     def on_apply(self):
         try:
             params = self.task_class.input_parameters
```

### Comparing `srsgui-0.2.7/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.8/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.8/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.8/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/qt/__init__.py` & `srsgui-0.2.8/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/qtloghandler.py` & `srsgui-0.2.8/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/resource_rc.py` & `srsgui-0.2.8/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/signalhandler.py` & `srsgui-0.2.8/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/srslogo.jpg` & `srsgui-0.2.8/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/stdout.py` & `srsgui-0.2.8/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/taskmain.py` & `srsgui-0.2.8/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/taskmain.ui` & `srsgui-0.2.8/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.8/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.7/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.8/srsgui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.7
+Version: 0.2.8
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.7/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.8/srsgui.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 srsgui/ui/ui_taskmain.py
 srsgui/ui/commandtree/commandcapturewidget.py
 srsgui/ui/commandtree/commandcapturewidget.ui
 srsgui/ui/commandtree/commanddelegate.py
 srsgui/ui/commandtree/commanditem.py
 srsgui/ui/commandtree/commandmodel.py
 srsgui/ui/commandtree/commandspinbox.py
+srsgui/ui/commandtree/commandtreeview.py
 srsgui/ui/commandtree/commandtreewidget.py
 srsgui/ui/commandtree/jsonmodel.py
 srsgui/ui/commandtree/ui_commandcapturewidget.py
+srsgui/ui/commandtree/ui_commandtreewidget.py
 srsgui/ui/qt/QtCore.py
 srsgui/ui/qt/QtGui.py
 srsgui/ui/qt/QtWidgets.py
 srsgui/ui/qt/__init__.py
```

