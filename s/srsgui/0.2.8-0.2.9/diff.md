# Comparing `tmp/srsgui-0.2.8.tar.gz` & `tmp/srsgui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-7qun3s1f\srsgui-0.2.8.tar", last modified: Tue Apr 11 18:06:49 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ps3u1u8m\srsgui-0.2.9.tar", last modified: Tue Apr 11 21:39:00 2023, max compression
```

## Comparing `srsgui-0.2.8.tar` & `srsgui-0.2.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.8/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3330 2023-04-11 18:06:49.463283 srsgui-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.373332 srsgui-0.2.8/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.393348 srsgui-0.2.8/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.403325 srsgui-0.2.8/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.8/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.8/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 18:06:49.463283 srsgui-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.403325 srsgui-0.2.8/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-04-11 18:05:11.000000 srsgui-0.2.8/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.8/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.363366 srsgui-0.2.8/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.423305 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.423305 srsgui-0.2.8/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.8/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.433300 srsgui-0.2.8/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.8/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.8/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.433300 srsgui-0.2.8/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.8/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.8/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.453288 srsgui-0.2.8/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.8/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     2931 2023-04-11 17:36:09.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.8/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.8/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.8/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.8/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.8/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.8/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.8/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.463283 srsgui-0.2.8/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.8/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.8/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.8/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.8/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.8/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:06:49.413310 srsgui-0.2.8/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3162 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 18:06:49.000000 srsgui-0.2.8/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.979862 srsgui-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.889910 srsgui-0.2.9/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.899904 srsgui-0.2.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:39:00.979862 srsgui-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 21:34:20.000000 srsgui-0.2.9/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.9/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.879943 srsgui-0.2.9/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.929916 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.9/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.9/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.9/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.9/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.949878 srsgui-0.2.9/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.9/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.959872 srsgui-0.2.9/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.969903 srsgui-0.2.9/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3127 2023-04-11 21:33:12.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.9/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.9/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.8/.gitignore` & `srsgui-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/LICENSE.txt` & `srsgui-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/PKG-INFO` & `srsgui-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.8
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.8/README.md` & `srsgui-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/Makefile` & `srsgui-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/make.bat` & `srsgui-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/conf.py` & `srsgui-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/create-project.rst` & `srsgui-0.2.9/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/create-task.rst` & `srsgui-0.2.9/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/define-instrument.rst` & `srsgui-0.2.9/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/example.rst` & `srsgui-0.2.9/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/index.rst` & `srsgui-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/installation.rst` & `srsgui-0.2.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/srsgui.inst.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/srsgui.task.rst` & `srsgui-0.2.9/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/docs/source/srsgui.ui.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/pyproject.toml` & `srsgui-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/__init__.py` & `srsgui-0.2.9/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.8"  # Global version number
+__version__ = "0.2.9"  # Global version number
```

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/__init__.py` & `srsgui-0.2.9/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/commands.py` & `srsgui-0.2.9/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/communications/interface.py` & `srsgui-0.2.9/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.9/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/component.py` & `srsgui-0.2.9/srsgui/inst/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
             if hasattr(instance, 'get_lists'):
                 return instance.get_lists()
 
     dir = DirCommand('dir')
     """ class instance of DirCommand"""
 
     exclude_capture = []
-    """exclude commands from query in capture_commands"""
+    """Exclude commands from query in capture_commands"""
+
+    allow_run_button = []
+    """Allow methods to have run buttons in a control panel"""
 
     def __init__(self, parent, name='unnamed'):
         self._name = name
         self._children = []
         if parent is None:
             self._parent = None
             self.comm = None
```

### Comparing `srsgui-0.2.8/srsgui/inst/exceptions.py` & `srsgui-0.2.9/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/indexcommands.py` & `srsgui-0.2.9/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/inst/instrument.py` & `srsgui-0.2.9/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/callbacks.py` & `srsgui-0.2.9/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/config.py` & `srsgui-0.2.9/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/inputs.py` & `srsgui-0.2.9/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/sessionhandler.py` & `srsgui-0.2.9/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/task.py` & `srsgui-0.2.9/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/task/taskresult.py` & `srsgui-0.2.9/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandhandler.py` & `srsgui-0.2.9/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandterminal.py` & `srsgui-0.2.9/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
 from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView, QPushButton
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 from .commandspinbox import RunButton
 
+
 class CommandTreeView(QTreeView):
     def __init__(self, parent=None):
         super(CommandTreeView, self).__init__(parent)
         
         self.query_only_included = False
         self.set_only_included = False
         self.excluded_included = False
@@ -42,24 +43,27 @@
             state = query_only or set_only or is_method or is_excluded
             self.setRowHidden(i, parent, state)
 
     def connect_methods_to_buttons(self, parent=QModelIndex()):
         for i in range(self.model().rowCount(parent)):
             index = self.model().index(i, 0, parent)
             self.connect_methods_to_buttons(index)
-
-            item = index.internalPointer()
-            if item.is_method:
-                widget_index = self.model().index(i, 1, parent)
-                if len(inspect.getfullargspec(item.comp).args) == 1:
-                    button = RunButton()
-                    func = getattr(item.parent().comp, item.name)
-                    if func is not None and parent.isValid():
-                        button.pressed.connect(func)
-                        self.setIndexWidget(widget_index, button)
+            try:
+                item = index.internalPointer()
+                if item.is_method:
+                    widget_index = self.model().index(i, 1, parent)
+                    if len(inspect.getfullargspec(item.comp).args) == 1:
+                        parent_comp = item.parent().comp
+                        meth = getattr(parent_comp, item.name)
+                        if meth and meth.__func__ in parent_comp.allow_run_button:
+                            button = RunButton()
+                            button.pressed.connect(meth)
+                            self.setIndexWidget(widget_index, button)
+            except Exception as e:
+                logging.error(e)
 
 
 if __name__ == "__main__":
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
     view = CommandTreeView()
```

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/connectdlg.py` & `srsgui-0.2.9/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.9/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/dockhandler.py` & `srsgui-0.2.9/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/inputpanel.py` & `srsgui-0.2.9/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.9/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.9/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/qt/__init__.py` & `srsgui-0.2.9/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/qtloghandler.py` & `srsgui-0.2.9/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/resource_rc.py` & `srsgui-0.2.9/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/signalhandler.py` & `srsgui-0.2.9/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/srslogo.jpg` & `srsgui-0.2.9/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/stdout.py` & `srsgui-0.2.9/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/taskmain.py` & `srsgui-0.2.9/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/taskmain.ui` & `srsgui-0.2.9/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.9/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.8/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.9/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.8
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.8/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.9/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

