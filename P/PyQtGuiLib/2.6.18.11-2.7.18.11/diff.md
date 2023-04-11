# Comparing `tmp/PyQtGuiLib-2.6.18.11.tar.gz` & `tmp/PyQtGuiLib-2.7.18.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtGuiLib-2.6.18.11.tar", last modified: Fri Apr  7 10:02:19 2023, max compression
+gzip compressed data, was "PyQtGuiLib-2.7.18.11.tar", last modified: Tue Apr 11 06:07:32 2023, max compression
```

## Comparing `PyQtGuiLib-2.6.18.11.tar` & `PyQtGuiLib-2.7.18.11.tar`

### file list

```diff
@@ -1,226 +1,239 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.168904 PyQtGuiLib-2.6.18.11/
--rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.6.18.11/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.920568 PyQtGuiLib-2.6.18.11/Log/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/Log/__init__.py
--rw-rw-rw-   0        0        0     9385 2023-04-07 09:59:18.000000 PyQtGuiLib-2.6.18.11/Log/developmentLog.py
--rw-rw-rw-   0        0        0    17825 2023-04-07 10:02:19.168904 PyQtGuiLib-2.6.18.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.922586 PyQtGuiLib-2.6.18.11/PyQtGuiLib/
--rw-rw-rw-   0        0        0      106 2023-04-03 06:49:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.936526 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/
--rw-rw-rw-   0        0        0      216 2023-03-17 10:17:57.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/__init__.py
--rw-rw-rw-   0        0        0    21262 2023-03-28 10:15:34.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animation.py
--rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationDrawType.py
--rw-rw-rw-   0        0        0    11607 2023-03-27 02:05:15.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationFactory.py
--rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationLayout.py
--rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/customAniTest.py
--rw-rw-rw-   0        0        0     3076 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/lmlmAni.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.949490 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/
--rw-rw-rw-   0        0        0      540 2023-03-13 03:28:34.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/__init__.py
--rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/bubbleWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.954476 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/
--rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/__init__.py
--rw-rw-rw-   0        0        0     4854 2023-02-13 10:30:41.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/combBox.py
--rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/comboBox.py
--rw-rw-rw-   0        0        0     4107 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/comboBox2.py
--rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/flowLayout.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.956471 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/lineedit/
--rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/lineedit/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py
--rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/listWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.962456 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/
--rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py
--rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py
--rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.964450 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/notice/
--rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/notice/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/notice/notice.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.967442 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/__init__.py
--rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/colorHsv.py
--rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/paletteFrame.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.974424 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/
--rw-rw-rw-   0        0        0      244 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/__init__.py
--rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/circularBar.py
--rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/gradientBar.py
--rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/loadBar.py
--rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/waterBar.py
--rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/pullOver.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.977416 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/resolver/
--rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/resolver/__init__.py
--rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/resolver/controls.py
--rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/rollWidget.py
--rw-rw-rw-   0        0        0     8684 2023-03-07 03:04:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.979410 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slider/
--rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slider/__init__.py
--rw-rw-rw-   0        0        0     8623 2023-03-06 01:03:54.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slider/slider.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.981405 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/switchButtons/
--rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/switchButtons/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/switchButtons/swButton.py
--rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/toolBox.py
--rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.990403 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/
--rw-rw-rw-   0        0        0    11338 2023-02-10 01:10:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/WidgetABC.py
--rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/__init__.py
--rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/statusBar.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.994388 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/tets/
--rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/tets/1.py
--rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/tets/2.py
--rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/tets/__init__.py
--rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/titleBar.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.001369 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.011349 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/__init__.py
--rw-rw-rw-   0        0        0     4997 2023-02-09 08:40:57.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qt.py
--rw-rw-rw-   0        0        0     2672 2023-02-18 03:01:28.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtCore.py
--rw-rw-rw-   0        0        0     3019 2023-02-18 05:34:36.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtGui.py
--rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtSip.py
--rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtUic.py
--rw-rw-rw-   0        0        0     6996 2023-02-18 02:58:53.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtWidgets.py
--rw-rw-rw-   0        0        0      632 2023-02-13 08:14:52.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/__init__.py
--rw-rw-rw-   0        0        0     6403 2023-02-14 05:59:02.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/customStyle.py
--rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/error.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.013320 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/py/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/py/__init__.py
--rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/py/common.py
--rw-rw-rw-   0        0        0     3516 2023-02-13 08:24:26.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/utility.py
--rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/versions.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.016336 PyQtGuiLib-2.6.18.11/PyQtGuiLib/layoutDeformation/
--rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/layoutDeformation/__init__.py
--rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/layoutDeformation/test.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.022297 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/
--rw-rw-rw-   0        0        0      302 2023-04-07 09:06:55.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.028280 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/
--rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
--rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
--rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
--rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.031274 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/buttons/
--rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/buttons/__init__.py
--rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.039276 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/
--rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/component.py
--rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/controlType.py
--rw-rw-rw-   0        0        0    11557 2023-02-23 09:01:24.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/styleLinker.py
--rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.042243 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.046232 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/drak/
--rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/drak/__init__.py
--rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/drak/config.py
--rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.050222 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/image/
--rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/image/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py
--rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/image/qssFile.py
--rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/qssFile.py
--rw-rw-rw-   0        0        0     6314 2023-03-30 09:24:42.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/test.py
--rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/skinABC.py
--rw-rw-rw-   0        0        0     8426 2023-04-06 03:40:05.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/styleAnalysis.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.053230 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter/
--rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter/__init__.py
--rw-rw-rw-   0        0        0    10866 2023-04-07 08:05:01.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter/superPainter.py
--rw-rw-rw-   0        0        0    17854 2023-03-10 06:22:00.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:18.927550 PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/
--rw-rw-rw-   0        0        0    17825 2023-04-07 10:02:18.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6182 2023-04-07 10:02:18.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 10:02:18.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-07 10:02:18.000000 PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.6.18.11/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.062215 PyQtGuiLib-2.6.18.11/abandonCase/
--rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.067176 PyQtGuiLib-2.6.18.11/abandonCase/acrylic/
--rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/acrylic/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/acrylic/acrylicWidget.py
--rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/acrylic/cstruct.py
--rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/acrylic/windowEffect.py
--rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/bubbleWidget.py
--rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/bubbleWidget_case.py
--rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/nodeBar.py
--rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/slideShow.py
--rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/slideShow2.py
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/spaceWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.078147 PyQtGuiLib-2.6.18.11/abandonCase/widgets/
--rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessFrame.py
--rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessMainWindow.py
--rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessStackedWidget.py
--rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessWidget.py
--rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessWidgetABC.py
--rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/statusBar.py
--rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/abandonCase/widgets/titleBar.py
--rw-rw-rw-   0        0        0       42 2023-04-07 10:02:19.168904 PyQtGuiLib-2.6.18.11/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-04-07 09:56:06.000000 PyQtGuiLib-2.6.18.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.117042 PyQtGuiLib-2.6.18.11/tests/
--rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.6.18.11/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.135994 PyQtGuiLib-2.6.18.11/tests/test_Animation/
--rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/1.py
--rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-03-24 08:50:00.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/eg1.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.137988 PyQtGuiLib-2.6.18.11/tests/test_Animation/test_ani/
--rw-rw-rw-   0        0        0     6145 2023-04-05 10:32:05.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/test_ani/1.py
--rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/test_ani/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-03-28 08:45:42.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_1.py
--rw-rw-rw-   0        0        0     1824 2023-03-28 08:48:45.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_10.py
--rw-rw-rw-   0        0        0     1305 2023-03-28 08:45:46.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_2.py
--rw-rw-rw-   0        0        0     2011 2023-03-28 08:45:51.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_3.py
--rw-rw-rw-   0        0        0     1276 2023-03-28 08:45:56.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_4.py
--rw-rw-rw-   0        0        0     1851 2023-03-28 08:46:24.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_5.py
--rw-rw-rw-   0        0        0     1759 2023-03-28 08:46:54.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_6.py
--rw-rw-rw-   0        0        0     2206 2023-03-28 08:47:16.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_7.py
--rw-rw-rw-   0        0        0     2000 2023-03-28 08:47:46.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_8.py
--rw-rw-rw-   0        0        0     1712 2023-03-28 08:48:15.000000 PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_9.py
--rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_BubbleWidget.py
--rw-rw-rw-   0        0        0     1592 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_Notice.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.150951 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg1.py
--rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg2.py
--rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg3.py
--rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg4.py
--rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg5.py
--rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg6.py
--rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg7.py
--rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/test.py
--rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis.py
--rw-rw-rw-   0        0        0     2278 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_SlideShow.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.154941 PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/
--rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/__init__.py
--rw-rw-rw-   0        0        0      949 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/eg1_QPushButton.py
--rw-rw-rw-   0        0        0      807 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/eg2_QLabel.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.161924 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/
--rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/__init__.py
--rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg1.py
--rw-rw-rw-   0        0        0     2125 2023-04-07 09:35:19.000000 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg2.py
--rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg3.py
--rw-rw-rw-   0        0        0     2372 2023-04-07 09:54:15.000000 PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg4.py
--rw-rw-rw-   0        0        0     2457 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_barset.py
--rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_circularBar.py
--rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_colorPalette.py
--rw-rw-rw-   0        0        0     1042 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_comboBox.py
--rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_dumpStructure.py
--rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_dynamicTLine.py
--rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_flowLayot.py
--rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_gradientBar.py
--rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_listWidget.py
--rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_loadbar.py
--rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_no_border.py
--rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_no_border_pullOver.py
--rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_pullOverWidget.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.164939 PyQtGuiLib-2.6.18.11/tests/test_qssFile/
--rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.6.18.11/tests/test_qssFile/__init__.py
--rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.6.18.11/tests/test_qssFile/test.py
--rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_rollWidget.py
--rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_slider.py
--rw-rw-rw-   0        0        0     1721 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_statusBar.py
--rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_styles.py
--rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_switchButton.py
--rw-rw-rw-   0        0        0     1138 2023-03-10 08:33:39.000000 PyQtGuiLib-2.6.18.11/tests/test_template.py
--rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.6.18.11/tests/test_toolList.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:02:19.166932 PyQtGuiLib-2.6.18.11/tests/test_uic/
--rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_uic/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_uic/test_uic.py
--rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.6.18.11/tests/test_waterBar.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.381422 PyQtGuiLib-2.7.18.11/
+-rw-rw-rw-   0        0        0     1091 2022-12-10 10:29:38.000000 PyQtGuiLib-2.7.18.11/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.134484 PyQtGuiLib-2.7.18.11/Log/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/Log/__init__.py
+-rw-rw-rw-   0        0        0     9452 2023-04-11 05:53:43.000000 PyQtGuiLib-2.7.18.11/Log/developmentLog.py
+-rw-rw-rw-   0        0        0    17825 2023-04-11 06:07:32.380418 PyQtGuiLib-2.7.18.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.135482 PyQtGuiLib-2.7.18.11/PyQtGuiLib/
+-rw-rw-rw-   0        0        0      106 2023-04-03 06:49:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.149443 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/
+-rw-rw-rw-   0        0        0      216 2023-03-17 10:17:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/__init__.py
+-rw-rw-rw-   0        0        0    21262 2023-03-28 10:15:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animation.py
+-rw-rw-rw-   0        0        0     2792 2023-03-28 09:06:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationDrawType.py
+-rw-rw-rw-   0        0        0    11607 2023-03-27 02:05:15.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationFactory.py
+-rw-rw-rw-   0        0        0     1636 2023-03-20 04:02:29.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationLayout.py
+-rw-rw-rw-   0        0        0     2292 2023-03-15 01:17:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/customAniTest.py
+-rw-rw-rw-   0        0        0     3076 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/lmlmAni.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.160414 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/
+-rw-rw-rw-   0        0        0      540 2023-03-13 03:28:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/__init__.py
+-rw-rw-rw-   0        0        0     5953 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/bubbleWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.165401 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/
+-rw-rw-rw-   0        0        0      218 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/__init__.py
+-rw-rw-rw-   0        0        0     4854 2023-02-13 10:30:41.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/combBox.py
+-rw-rw-rw-   0        0        0     8171 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox.py
+-rw-rw-rw-   0        0        0     4107 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox2.py
+-rw-rw-rw-   0        0        0     3886 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/flowLayout.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.167396 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/
+-rw-rw-rw-   0        0        0      170 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py
+-rw-rw-rw-   0        0        0     5090 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/listWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.173380 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/
+-rw-rw-rw-   0        0        0      107 2023-03-27 09:33:07.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-03-31 09:04:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py
+-rw-rw-rw-   0        0        0     5112 2023-04-03 02:45:06.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py
+-rw-rw-rw-   0        0        0      554 2023-03-31 09:29:33.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.176372 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/
+-rw-rw-rw-   0        0        0        0 2023-02-08 01:08:13.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-02-10 11:02:17.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/notice.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.179364 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/__init__.py
+-rw-rw-rw-   0        0        0     9818 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/colorHsv.py
+-rw-rw-rw-   0        0        0     6728 2023-02-18 01:06:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/paletteFrame.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.185352 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/
+-rw-rw-rw-   0        0        0      244 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/__init__.py
+-rw-rw-rw-   0        0        0     5602 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/circularBar.py
+-rw-rw-rw-   0        0        0     3943 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/gradientBar.py
+-rw-rw-rw-   0        0        0     4365 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/loadBar.py
+-rw-rw-rw-   0        0        0     6734 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/waterBar.py
+-rw-rw-rw-   0        0        0     5092 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/pullOver.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.188340 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/
+-rw-rw-rw-   0        0        0       59 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/__init__.py
+-rw-rw-rw-   0        0        0      674 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/controls.py
+-rw-rw-rw-   0        0        0     7628 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/rollWidget.py
+-rw-rw-rw-   0        0        0     8775 2023-04-11 04:20:04.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.191332 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/
+-rw-rw-rw-   0        0        0        0 2023-02-14 00:37:29.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/__init__.py
+-rw-rw-rw-   0        0        0     8623 2023-03-06 01:03:54.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/slider.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.193326 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/
+-rw-rw-rw-   0        0        0       63 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-02-23 01:29:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/swButton.py
+-rw-rw-rw-   0        0        0     2743 2023-03-06 05:54:08.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolBox.py
+-rw-rw-rw-   0        0        0     5588 2023-03-14 01:24:55.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.202302 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/
+-rw-rw-rw-   0        0        0    11338 2023-02-10 01:10:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/WidgetABC.py
+-rw-rw-rw-   0        0        0      260 2023-02-09 10:20:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3995 2023-02-10 07:29:38.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0      303 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0     4935 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/statusBar.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.206292 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/
+-rw-rw-rw-   0        0        0      375 2023-02-27 10:18:30.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/1.py
+-rw-rw-rw-   0        0        0     3504 2023-02-27 00:36:50.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/2.py
+-rw-rw-rw-   0        0        0        0 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/__init__.py
+-rw-rw-rw-   0        0        0    17840 2023-02-10 03:56:26.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/titleBar.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.212276 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.221252 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/__init__.py
+-rw-rw-rw-   0        0        0     4997 2023-02-09 08:40:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qt.py
+-rw-rw-rw-   0        0        0     2672 2023-02-18 03:01:28.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtCore.py
+-rw-rw-rw-   0        0        0     3019 2023-02-18 05:34:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtGui.py
+-rw-rw-rw-   0        0        0      509 2023-02-09 08:33:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtSip.py
+-rw-rw-rw-   0        0        0      505 2023-02-13 08:07:57.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtUic.py
+-rw-rw-rw-   0        0        0     6996 2023-02-18 02:58:53.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtWidgets.py
+-rw-rw-rw-   0        0        0      632 2023-02-13 08:14:52.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/__init__.py
+-rw-rw-rw-   0        0        0     6403 2023-02-14 05:59:02.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/customStyle.py
+-rw-rw-rw-   0        0        0      262 2023-02-10 01:34:45.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/error.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.224244 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/py/common.py
+-rw-rw-rw-   0        0        0     3516 2023-02-13 08:24:26.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/utility.py
+-rw-rw-rw-   0        0        0      396 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/versions.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.226239 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/
+-rw-rw-rw-   0        0        0      106 2023-03-04 03:38:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/__init__.py
+-rw-rw-rw-   0        0        0     4425 2023-03-07 08:03:39.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/test.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.231225 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/
+-rw-rw-rw-   0        0        0      302 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.236212 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/
+-rw-rw-rw-   0        0        0      105 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/__init__.py
+-rw-rw-rw-   0        0        0     7168 2023-02-24 00:57:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py
+-rw-rw-rw-   0        0        0     5062 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.239204 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-02-01 01:34:23.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.245838 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/
+-rw-rw-rw-   0        0        0      106 2023-02-20 02:36:19.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-02-23 01:15:37.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/component.py
+-rw-rw-rw-   0        0        0     8822 2023-03-13 01:50:58.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/controlType.py
+-rw-rw-rw-   0        0        0    11557 2023-02-23 09:01:24.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinker.py
+-rw-rw-rw-   0        0        0     1444 2023-02-22 03:17:40.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.248830 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.252820 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/
+-rw-rw-rw-   0        0        0      107 2023-03-29 02:48:22.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-03-29 08:26:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/config.py
+-rw-rw-rw-   0        0        0    11537 2023-03-30 09:13:08.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.256808 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/
+-rw-rw-rw-   0        0        0      107 2023-03-29 03:26:49.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-03-30 10:20:11.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py
+-rw-rw-rw-   0        0        0      300 2023-03-30 10:19:06.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/qssFile.py
+-rw-rw-rw-   0        0        0    20518 2023-03-30 10:20:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/qssFile.py
+-rw-rw-rw-   0        0        0     6314 2023-03-30 09:24:42.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/test.py
+-rw-rw-rw-   0        0        0    10615 2023-02-09 08:32:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/skinABC.py
+-rw-rw-rw-   0        0        0     8474 2023-04-11 01:23:59.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/styleAnalysis.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.258803 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/
+-rw-rw-rw-   0        0        0      107 2023-03-18 07:49:47.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/__init__.py
+-rw-rw-rw-   0        0        0    11549 2023-04-10 04:38:34.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/superPainter.py
+-rw-rw-rw-   0        0        0    17854 2023-03-10 06:22:00.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.259810 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.262792 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/
+-rw-rw-rw-   0        0        0      193 2023-04-11 03:59:36.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/__init__.py
+-rw-rw-rw-   0        0        0     4564 2023-04-11 05:44:28.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.264787 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/
+-rw-rw-rw-   0        0        0      107 2023-04-10 09:41:12.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/__init__.py
+-rw-rw-rw-   0        0        0     4891 2023-04-11 05:44:46.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
+-rw-rw-rw-   0        0        0      189 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib/templateWindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.140468 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/
+-rw-rw-rw-   0        0        0    17825 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6566 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-11 06:07:32.000000 PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17395 2023-03-27 01:38:52.000000 PyQtGuiLib-2.7.18.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.275758 PyQtGuiLib-2.7.18.11/abandonCase/
+-rw-rw-rw-   0        0        0      108 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.280744 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/
+-rw-rw-rw-   0        0        0       37 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/acrylicWidget.py
+-rw-rw-rw-   0        0        0     1550 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/cstruct.py
+-rw-rw-rw-   0        0        0     2183 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/acrylic/windowEffect.py
+-rw-rw-rw-   0        0        0     9981 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget.py
+-rw-rw-rw-   0        0        0     3620 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget_case.py
+-rw-rw-rw-   0        0        0     1411 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/nodeBar.py
+-rw-rw-rw-   0        0        0     9873 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/slideShow.py
+-rw-rw-rw-   0        0        0     7801 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/slideShow2.py
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/spaceWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.292712 PyQtGuiLib-2.7.18.11/abandonCase/widgets/
+-rw-rw-rw-   0        0        0      110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessFrame.py
+-rw-rw-rw-   0        0        0     1962 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessMainWindow.py
+-rw-rw-rw-   0        0        0     1441 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessStackedWidget.py
+-rw-rw-rw-   0        0        0     1402 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidget.py
+-rw-rw-rw-   0        0        0    10095 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidgetABC.py
+-rw-rw-rw-   0        0        0     5034 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/statusBar.py
+-rw-rw-rw-   0        0        0    17577 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/abandonCase/widgets/titleBar.py
+-rw-rw-rw-   0        0        0       42 2023-04-11 06:07:32.381422 PyQtGuiLib-2.7.18.11/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-04-11 05:55:32.000000 PyQtGuiLib-2.7.18.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.326562 PyQtGuiLib-2.7.18.11/tests/
+-rw-rw-rw-   0        0        0      107 2023-03-06 03:09:41.000000 PyQtGuiLib-2.7.18.11/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.342519 PyQtGuiLib-2.7.18.11/tests/test_Animation/
+-rw-rw-rw-   0        0        0     1994 2023-04-05 10:25:59.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/1.py
+-rw-rw-rw-   0        0        0      606 2023-03-15 09:52:36.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-03-24 08:50:00.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/eg1.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.345511 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/
+-rw-rw-rw-   0        0        0     6145 2023-04-05 10:32:05.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/1.py
+-rw-rw-rw-   0        0        0      107 2023-03-27 05:53:58.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-03-28 08:45:42.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_1.py
+-rw-rw-rw-   0        0        0     1824 2023-03-28 08:48:45.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_10.py
+-rw-rw-rw-   0        0        0     1305 2023-03-28 08:45:46.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_2.py
+-rw-rw-rw-   0        0        0     2011 2023-03-28 08:45:51.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_3.py
+-rw-rw-rw-   0        0        0     1276 2023-03-28 08:45:56.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_4.py
+-rw-rw-rw-   0        0        0     1851 2023-03-28 08:46:24.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_5.py
+-rw-rw-rw-   0        0        0     1759 2023-03-28 08:46:54.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_6.py
+-rw-rw-rw-   0        0        0     2206 2023-03-28 08:47:16.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_7.py
+-rw-rw-rw-   0        0        0     2000 2023-03-28 08:47:46.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_8.py
+-rw-rw-rw-   0        0        0     1712 2023-03-28 08:48:15.000000 PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_9.py
+-rw-rw-rw-   0        0        0     1541 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_BubbleWidget.py
+-rw-rw-rw-   0        0        0     1592 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_Notice.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.357510 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-04-06 02:24:28.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg1.py
+-rw-rw-rw-   0        0        0     2306 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg2.py
+-rw-rw-rw-   0        0        0     1891 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg3.py
+-rw-rw-rw-   0        0        0     2110 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg4.py
+-rw-rw-rw-   0        0        0     2519 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg5.py
+-rw-rw-rw-   0        0        0     1881 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg6.py
+-rw-rw-rw-   0        0        0     2617 2023-03-22 05:45:33.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg7.py
+-rw-rw-rw-   0        0        0     2042 2023-04-06 03:41:23.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/test.py
+-rw-rw-rw-   0        0        0     2275 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis.py
+-rw-rw-rw-   0        0        0     2278 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_SlideShow.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.361493 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/
+-rw-rw-rw-   0        0        0        0 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/__init__.py
+-rw-rw-rw-   0        0        0      949 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg1_QPushButton.py
+-rw-rw-rw-   0        0        0      807 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg2_QLabel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.371457 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/
+-rw-rw-rw-   0        0        0        0 2023-04-10 02:56:18.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/1.py
+-rw-rw-rw-   0        0        0      106 2023-04-07 09:06:55.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/__init__.py
+-rw-rw-rw-   0        0        0     1568 2023-04-07 09:19:44.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg1.py
+-rw-rw-rw-   0        0        0     2143 2023-04-10 00:27:52.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg2.py
+-rw-rw-rw-   0        0        0     1648 2023-04-07 09:39:03.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg3.py
+-rw-rw-rw-   0        0        0     2372 2023-04-07 09:54:15.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg4.py
+-rw-rw-rw-   0        0        0     2111 2023-04-10 03:46:57.000000 PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/test.py
+-rw-rw-rw-   0        0        0     2457 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_barset.py
+-rw-rw-rw-   0        0        0     1648 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_circularBar.py
+-rw-rw-rw-   0        0        0     1723 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_colorPalette.py
+-rw-rw-rw-   0        0        0     1042 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_comboBox.py
+-rw-rw-rw-   0        0        0      289 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_dumpStructure.py
+-rw-rw-rw-   0        0        0      830 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_dynamicTLine.py
+-rw-rw-rw-   0        0        0     1315 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_flowLayot.py
+-rw-rw-rw-   0        0        0     1788 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_gradientBar.py
+-rw-rw-rw-   0        0        0     1865 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_listWidget.py
+-rw-rw-rw-   0        0        0     1398 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_loadbar.py
+-rw-rw-rw-   0        0        0     2498 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_no_border.py
+-rw-rw-rw-   0        0        0     1365 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_no_border_pullOver.py
+-rw-rw-rw-   0        0        0     1022 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_pullOverWidget.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.374434 PyQtGuiLib-2.7.18.11/tests/test_qssFile/
+-rw-rw-rw-   0        0        0      107 2023-03-29 06:12:59.000000 PyQtGuiLib-2.7.18.11/tests/test_qssFile/__init__.py
+-rw-rw-rw-   0        0        0      584 2023-04-04 06:18:57.000000 PyQtGuiLib-2.7.18.11/tests/test_qssFile/test.py
+-rw-rw-rw-   0        0        0     1444 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_rollWidget.py
+-rw-rw-rw-   0        0        0     1666 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_slider.py
+-rw-rw-rw-   0        0        0     1721 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_statusBar.py
+-rw-rw-rw-   0        0        0     1014 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_styles.py
+-rw-rw-rw-   0        0        0     1122 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_switchButton.py
+-rw-rw-rw-   0        0        0     1138 2023-03-10 08:33:39.000000 PyQtGuiLib-2.7.18.11/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.377426 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/
+-rw-rw-rw-   0        0        0      107 2023-04-11 04:44:35.000000 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-04-11 05:48:48.000000 PyQtGuiLib-2.7.18.11/tests/test_templateWindow/test_listTemplateWindow.py
+-rw-rw-rw-   0        0        0     1356 2023-03-13 08:03:45.000000 PyQtGuiLib-2.7.18.11/tests/test_toolList.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:07:32.379420 PyQtGuiLib-2.7.18.11/tests/test_uic/
+-rw-rw-rw-   0        0        0      107 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_uic/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_uic/test_uic.py
+-rw-rw-rw-   0        0        0     1547 2023-03-06 00:27:58.000000 PyQtGuiLib-2.7.18.11/tests/test_waterBar.py
```

### Comparing `PyQtGuiLib-2.6.18.11/LICENSE.txt` & `PyQtGuiLib-2.7.18.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/Log/developmentLog.py` & `PyQtGuiLib-2.7.18.11/Log/developmentLog.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,16 @@
 
 2023.3.24 - 2023.4.7
     - Animation 动画框架 已经快接近完成,目前大部分功能已经可用
     - 修改QSS解析器的已知BUG,并且在多线程时,是安全的
     - 新增 SuperPainter 超级画师类
         - 导入方法 from PyQtGuiLib.styles import SuperPainter
         - 教学案例在test\test_SuperPainter 目录下
+2023.4.7 - 2023.4.11
+    - 更新模板窗口 ListTemplateWindow
 '''
 
 
 # -------------------------------
 '''
     暂时搁浅的任务
 1.新无边框窗口主窗口,(还没有设计完成,暂时先放下 2023.1.31)
```

### Comparing `PyQtGuiLib-2.6.18.11/PKG-INFO` & `PyQtGuiLib-2.7.18.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.6.18.11
+Version: 2.7.18.11
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animation.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationDrawType.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationDrawType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationFactory.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationFactory.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/animationLayout.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/animationLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/customAniTest.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/customAniTest.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/animation/lmlmAni.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/animation/lmlmAni.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/__init__.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/bubbleWidget.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/combBox.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/combBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/comboBox.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/comboBox/comboBox2.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/comboBox/comboBox2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/flowLayout.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/flowLayout.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/lineedit/dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/listWidget.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/loadLogTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logBrowser.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/logBrowser/logSizeTh.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/notice/notice.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/notice/notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/colorHsv.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/colorHsv.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/palettes/paletteFrame.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/palettes/paletteFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/circularBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/gradientBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/loadBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/loadBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/progressBar/waterBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/progressBar/waterBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/pullOver.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/resolver/controls.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/resolver/controls.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/rollWidget.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slideShow.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slideShow.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # @software:PyCharm
 
 from PyQtGuiLib.header import (
     QWidget,
     QPushButton,
     QPoint,
     QPropertyAnimation,
-    Signal
+    Signal,
+    QSize
 )
 
 '''
     组件轮播 2023.3.7 当前控件的所有功能均处于稳定状态
     SlideShow 独立版本 3.0
 '''
 class SlideShow(QWidget):
@@ -47,14 +48,17 @@
         # 指向两个当前窗口
         self.cursor_widget_p = None # type:QWidget
         self.cursor_widget_p2 = None # type:QWidget
 
         # 创建两侧按钮
         self.createButtons()
 
+    def setDuration(self,p_int):
+        self.animation_time = p_int
+
     # 设置自动轮播
     def setAutoSlideShow(self,b:bool,interval=1500,direction_:str="R"):
         if direction_ not in ["R","L"]:
             raise TypeError("Parameter error, Support only 'R' or 'L' !")
 
         if interval <= self.animation_time:
             raise ValueError("The interval between auto wheel casting must be longer than the animation time!")
@@ -134,25 +138,27 @@
             self.index -= 1
             if self.index < -self.count():
                 self.index = -1
 
         if not direction:
             return
 
+
         w_2 = self.widgets[self.index]
         self.cursor_widget_p = w_2 # 保存当前窗口
         self.cursor_widget_p2 = w_1
         self.changeWidget.emit(w_2)# 切换窗口时发送信号
         w_1.show()
         w_2.show()
 
         self.ani_(w_1, w_2, direction)
 
     def addWidget(self,widget:QWidget):
         widget.setParent(self)
+
         widget.resize(self.size())
         widget.lower()
         self.widgets.append(widget)
 
         if self.count() > 1:
             widget.hide()
         else:
@@ -217,14 +223,15 @@
         if not widget_show.parent():
             widget_show.setParent(self)
 
         wid1,wid2 = widget_out,widget_show
         wid1.resize(self.size())
         wid2.resize(self.size())
 
+
         ani_1 = QPropertyAnimation(wid1,b"pos",self)
         ani_2 = QPropertyAnimation(wid2,b"pos",self)
         ani_1.setDuration(self.animation_time)
         ani_2.setDuration(self.animation_time)
 
         if direction == SlideShow.Ani_Left:
             s_ani_1, e_ani_1 = QPoint(0, 0), QPoint(-self.width(), 0)
```

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/slider/slider.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/slider/slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/switchButtons/swButton.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/switchButtons/swButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/toolBox.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/toolList.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/WidgetABC.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/WidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/statusBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/tets/2.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/tets/2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/core/widgets/titleBar.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/core/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qt.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qt.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtCore.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtCore.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtGui.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtGui.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/Qt/qtWidgets.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/Qt/qtWidgets.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/__init__.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/customStyle.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/customStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/header/utility.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/header/utility.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/layoutDeformation/test.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/layoutDeformation/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesigner.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/builtStyleDesignerUI.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/builtStyleDesigner/controlConfig.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/buttons/buttonStyle.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/component.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/component.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/controlType.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/controlType.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/styleLinker.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinker.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/linker/styleLinkerUi.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/drak/qssDrak.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/image/image_rc.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/qssFile.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/qssFile.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/qssFile/test.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/skinABC.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/skinABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/styleAnalysis.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/styleAnalysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,23 +92,23 @@
         else:
            raise KeyError("Without this attribute,'%s'" % key)
 
     def updateAttr(self,key:str,value:str):
         self._qss_dict[self.header()][key]=value
         self._qss_str = dictTostr(self._qss_dict)
         self.Init()
-        if self.__parent:
+        if self.__parent is not None:
             self.__qs.updateStyleSheet()
 
     def removeAttr(self,key:str):
         if key in self._qss_dict[self.header()]:
             del self._qss_dict[self.header()][key]
             self._qss_str = dictTostr(self._qss_dict)
             self.Init()
-            if self.__parent:
+            if self.__parent is not None:
                 self.__qs.updateStyleSheet()
         else:
             raise TypeError("Without this attribute,'%s'"%key)
 
     def isAttr(self,key:str)->bool:
         if self._qss_dict[self.header()].get(key):
             return True
@@ -161,15 +161,15 @@
 
     def setQSS(self,qss:str):
         # Preprocessing qss
         self._qss = [Qss(qss,self,self.__parent) for qss in self.groupDecomposition(qss)]
         # Mapping coordinate
         self.__mappCoordinate(0,self.count())
 
-        if self.__parent:
+        if self.__parent is not None:
             self.__updateStyle(self.__parent)
 
     # Bidirectional mapping
     def __mappCoordinate(self,s,e):
         for i in range(s,e):
             self._map_qss[self.selectorIndex(i).header()] = i
             self._reverse_map_qss[str(i)] = self.selectorIndex(i).header()
@@ -195,15 +195,15 @@
 
         # del temp_hear
         old_count = self.count()
         self._qss.extend(new_qss)
 
         # remap
         self.__mappCoordinate(old_count,self.count())
-        if self.__parent:
+        if self.__parent is not None:
             self.__updateStyle(self.__parent)
 
     def appendQSSDict(self,qss_dict:dict):
         self.appendQSS(dictTostr(qss_dict))
 
     def selectorKey(self,key:str)->Qss:
         return self.selectorIndex(self._map_qss[key])
```

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter/superPainter.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter/superPainter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,155 @@
 # -*- coding:utf-8 -*-
 from PyQtGuiLib.header import (
-    QApplication,
-    PYQT_VERSIONS,
-    sys,
-    QWidget,
-    QObject,
-    QRect,
-    QSize,
     QPainter,
-    QPoint,
     QPen,
     QBrush,
     QFont,
     qt,
     Qt,
     QColor,
     QPaintEvent,
-    QPushButton
 )
 import typing
 
+'''
+        drawRect 有(x,y)
+        drawRoundedRect  有(x,y)
+        drawLine 有(x,y)
+        drawLines  
+        drawArc  有(x,y)
+        drawEllipse  有(x,y)
+        drawPoint  有(x,y)
+        drawPoints 
+        drawText 有(x,y)
+        drawStaticText 
+        drawPolygon 
+        drawPie 有(x,y)
+        drawPicture 有(x,y)
+        drawChord 有(x,y)
+        drawRects 
+        drawPolyline 
+        drawPath 
+        drawConvexPolygon 
+        drawGlyphRun 
+        drawPixmap 有(x,y)
+        drawImage 有(x,y)
+        drawPixmapFragments 
+        drawTiledPixmap 有(x,y)
+'''
+RECT_TYPES = ["drawRect","drawRoundedRect","drawLine","drawArc","drawEllipse","drawPoint",
+                "drawText","drawPie","drawPicture","drawChord","drawPixmap","drawImage","drawTiledPixmap"]
+
+
+# 图形分类函数
+def patternClassification(name:str):
+    '''
+        返回参数含义:
+            Rect 表示前两个参数是x,y,可以直接进行移动操作
+
+    :param name:
+    :return:
+    '''
+    if name in RECT_TYPES:
+        return "Rect"
+
 
-# 虚拟图形对象类
 class VirtualObject:
-    def __init__(self):
-        # 虚拟对象字典
-        self.__virtualObjects = dict()  # type:typing.Dict[str:typing.List]
+    def __init__(self,vobj_name:str,**kwargs):
+        self.__vobj_name = vobj_name
+        self.__vir_attr = kwargs # 虚拟属性
 
-    def isVirtualObject(self, vobj_name: str)->bool:
-        return True if self.__virtualObjects.get(vobj_name,None) else False
+    def type(self)->str:
+        return self.getVirtualFunc().__name__
 
-    def appendVirtualObject(self, vobj_name: str, **kwargs):
-        if not self.isVirtualObject(vobj_name):
-            self.__virtualObjects[vobj_name] = kwargs
+    def virName(self) -> str:
+        return self.__vobj_name
 
-    def getVirtualObjectAttr(self,vobj_name: str):
-        if self.isVirtualObject(vobj_name):
-            return self.__virtualObjects[vobj_name]
+    def getVirtualObjectAttr(self) -> dict:
+        return self.__vir_attr
 
-    def getVirtualObjectAttrValue(self,vobj_name: str,key:str):
-        if self.isVirtualObject(vobj_name):
-            return self.__virtualObjects[vobj_name][key]
+    def getVirtualObjectAttrValue(self, key: str):
+        return self.getVirtualObjectAttr()[key]
 
-    def getVirtualFunc(self,vobj_name:str)->typing.Callable:
-        return self.__virtualObjects[vobj_name]["func"]
+    def getVirtualFunc(self) -> typing.Callable:
+        return self.getVirtualObjectAttr()["func"]
 
-    def getVirtualArgs(self,vobj_name:str)->tuple:
-        return self.__virtualObjects[vobj_name]["args"]
+    def getVirtualArgs(self) -> tuple:
+        return self.getVirtualObjectAttr()["args"]
 
-    def getVirtualOpenAttr(self,vobj_name:str)->dict:
-        return self.__virtualObjects[vobj_name]["openAttr"]
+    def getVirtualOpenAttr(self) -> dict:
+        return self.getVirtualObjectAttr()["openAttr"]
 
-    def getVirtualBrushAttr(self,vobj_name:str)->dict:
-        return self.__virtualObjects[vobj_name]["brushAttr"]
+    def getVirtualBrushAttr(self)->dict:
+        return self.getVirtualObjectAttr()["brushAttr"]
 
-    def updateArgs(self,vobj_name:str,*args):
+    def updateArgs(self,*args):
         if args:
-            self.__virtualObjects[vobj_name]["args"] = args
+            self.getVirtualObjectAttr()["args"] = args
 
-    def updateOpenAttr(self,vobj_name:str,openAttr:dict):
+    def updateOpenAttr(self,openAttr:dict):
         if openAttr:
-            self.__virtualObjects[vobj_name]["openAttr"] = openAttr
+            self.getVirtualObjectAttr()["openAttr"] = openAttr
 
-    def updateBrushAttr(self,vobj_name:str,brushAttr:dict):
+    def updateBrushAttr(self,brushAttr:dict):
         if brushAttr:
-            self.__virtualObjects[vobj_name]["brushAttr"] = brushAttr
+            self.getVirtualObjectAttr()["brushAttr"] = brushAttr
 
-    def updateDraw(self,vobj_name:str,*args,**kwargs):
-        self.updateArgs(vobj_name,*args)
+    def updateDraw(self,*args,**kwargs):
+        self.updateArgs(self.virtualObjName(),*args)
         openAttr = kwargs.get("openAttr", None)
         brushAttr = kwargs.get("brushAttr", None)
-        self.updateOpenAttr(vobj_name,openAttr)
-        self.updateBrushAttr(vobj_name,brushAttr)
+        self.updateOpenAttr(self.virtualObjName(),openAttr)
+        self.updateBrushAttr(self.virtualObjName(),brushAttr)
+
+    def move(self,x,y):
+        if patternClassification(self.type()) == "Rect":
+            args = self.getVirtualArgs()[2:]
+            self.updateArgs(x,y,*args)
+
+    def scale(self,proportion:float):
+        if patternClassification(self.type()) == "Rect":
+            xy = self.getVirtualArgs()[:2]
+            wh = self.getVirtualArgs()[2:4]
+            w,h = int(wh[0]*proportion),int(wh[1]*proportion)
+            self.updateArgs(*xy,w,h)
+
+
+# 虚拟图形对象管理类
+class VirtualObjectManagement:
+    def __init__(self):
+        # 虚拟对象字典
+        self.__virtualObjects = dict()  # type:typing.Dict[str:typing.List]
+
+    def virtualObjName(self,vobj_name:str)->str:
+        if self.isVirtualObject(vobj_name):
+            return self.__virtualObjects[vobj_name]
+        else:
+            raise Exception("[{}] The virtual object does not exist!".format(vobj_name))
+
+    def isVirtualObject(self,vobj_name:str)->bool:
+        return True if self.__virtualObjects.get(vobj_name,None) else False
+
+    def appendVirtualObject(self, vobj_name: str, **kwargs):
+        if not self.isVirtualObject(vobj_name):
+            self.__virtualObjects[vobj_name] = VirtualObject(vobj_name,**kwargs)
+
 
 
 class SuperPainterAttr(QPainter):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
 
         self.__op = QPen(QColor(0,0,0))  # type:QPen
         self.__brush = QBrush(QColor(0,0,0)) # type: QBrush
         self.__font = None  # type: QFont
-        self.__virtualObject = VirtualObject()
+        self.__virtualObject = VirtualObjectManagement() # 虚拟对象
 
-    def virtualObj(self)->VirtualObject:
-        return self.__virtualObject
+    def virtualObj(self,vobj_name:str)->VirtualObject:
+        return self.__virtualObject.virtualObjName(vobj_name)
 
     def setPen(self, op:QPen):
         if not isinstance(op,QPen):
             op = QPen(op)
         self.__op = op
         super().setPen(op)
 
@@ -191,15 +252,14 @@
 
         if brushAttr:
             self.setBrush(brush)
 
     def __restorePrivateAttr(self, op:QPen, brush:QBrush):
         if op:
             self.setPen(op)
-
         if brush:
             self.setBrush(brush)
 
     def decorator_to_all_draw_methods(self):
         def decorator(func):
             def wrapper(*args, **kwargs):
                 op = self.open_()
@@ -207,20 +267,27 @@
 
                 openAttr = kwargs.get("openAttr", None)
                 brushAttr = kwargs.get("brushAttr", None)
                 virtual_object_name = kwargs.get("virtualObjectName",None) or kwargs.get("vobj",None)
                 if virtual_object_name:
                     self.__virtualObject.appendVirtualObject(virtual_object_name,func=func,args=args,kwargs=kwargs,
                                                              openAttr=openAttr,brushAttr=brushAttr)
+                    vir_obj = self.virtualObj(virtual_object_name)
+                    args = vir_obj.getVirtualArgs()
+                    vir_openAttr = vir_obj.getVirtualOpenAttr()
+                    vir_brushAttr = vir_obj.getVirtualBrushAttr()
+                    if openAttr:openAttr = vir_openAttr
+                    elif vir_openAttr:
+                        openAttr = vir_openAttr
+                        kwargs["openAttr"] = openAttr
+                    if brushAttr:brushAttr = vir_brushAttr
+                    elif vir_brushAttr:
+                        brushAttr = vir_brushAttr
+                        kwargs["brushAttr"] = brushAttr
 
-                    args = self.virtualObj().getVirtualArgs(virtual_object_name)
-                    if openAttr:
-                        openAttr = self.virtualObj().getVirtualOpenAttr(virtual_object_name)
-                    if brushAttr:
-                        brushAttr = self.virtualObj().getVirtualBrushAttr(virtual_object_name)
                 self.__privateAttr(openAttr, brushAttr)
                 if openAttr:del kwargs["openAttr"]
                 if brushAttr:del kwargs["brushAttr"]
                 if virtual_object_name: del kwargs["virtualObjectName"]
                 value = func(*args,**kwargs)
                 self.__restorePrivateAttr(op,brush)
                 return value
@@ -252,49 +319,7 @@
 
 
 class SuperPainter(SuperPainterAttr):
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
         self.decorator_to_all_draw_methods()
 
-
-class Test(QWidget):
-    def __init__(self,*args,**kwargs):
-        super().__init__(*args,**kwargs)
-        self.resize(600,600)
-        self.painter = SuperPainter()
-        self.btn = QPushButton("更新图像",self)
-        self.btn.move(300,50)
-        self.btn.clicked.connect(lambda :self.test_update())
-
-    def test_update(self):
-        print(self.painter.virtualObj().getVirtualObjectAttr("rect_tt"))
-        self.painter.virtualObj().updateDraw("rect_tt",20,20,70,70,openAttr={"color":"blue"},brushAttr={"color":"yellow"})
-        self.update()
-        print(self.painter.virtualObj().getVirtualObjectAttr("rect_tt"))
-
-    def paintEvent(self, e:QPaintEvent) -> None:
-        self.painter.begin(self)
-        self.painter.setRenderHints(qt.Antialiasing | qt.SmoothPixmapTransform | qt.TextAntialiasing)
-
-        self.painter.setPen(QColor(52,44,120))
-
-        self.painter.drawRect(20, 20, 50, 50, openAttr={"color": "red", "brush": "#9bff7d"},brushAttr={"color":"green"},
-                              virtualObjectName="rect_tt")
-
-        self.painter.drawLine(70, 70, 200, 200)
-        self.painter.drawRect(200, 200, 50, 50,openAttr={"color":"yellow"},brushAttr={"color":"#9bff7d"})
-
-        self.painter.end()
-
-
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-
-    win = Test()
-
-    win.show()
-
-    if PYQT_VERSIONS in ["PyQt6","PySide6"]:
-        sys.exit(app.exec())
-    else:
-        sys.exit(app.exec_())
```

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib/styles/superPainter.py` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib/styles/superPainter.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/PKG-INFO` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtGuiLib
-Version: 2.6.18.11
+Version: 2.7.18.11
 Summary: Python version of the qt component library.
 Home-page: https://github.com/LX-sys/PyQtGuiLib
 Author: LX
 Author-email: lx984608061@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyQtGuiLib-2.6.18.11/PyQtGuiLib.egg-info/SOURCES.txt` & `PyQtGuiLib-2.7.18.11/PyQtGuiLib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -97,14 +97,19 @@
 PyQtGuiLib/styles/qssFile/drak/config.py
 PyQtGuiLib/styles/qssFile/drak/qssDrak.py
 PyQtGuiLib/styles/qssFile/image/__init__.py
 PyQtGuiLib/styles/qssFile/image/image_rc.py
 PyQtGuiLib/styles/qssFile/image/qssFile.py
 PyQtGuiLib/styles/superPainter/__init__.py
 PyQtGuiLib/styles/superPainter/superPainter.py
+PyQtGuiLib/templateWindow/__init__.py
+PyQtGuiLib/templateWindow/UI/__init__.py
+PyQtGuiLib/templateWindow/UI/listTemplateWindowUI.py
+PyQtGuiLib/templateWindow/Window/__init__.py
+PyQtGuiLib/templateWindow/Window/listTemplateWindow.py
 abandonCase/__init__.py
 abandonCase/bubbleWidget.py
 abandonCase/bubbleWidget_case.py
 abandonCase/nodeBar.py
 abandonCase/slideShow.py
 abandonCase/slideShow2.py
 abandonCase/spaceWidget.py
@@ -169,16 +174,20 @@
 tests/test_QssStyleAnalysis/eg5.py
 tests/test_QssStyleAnalysis/eg6.py
 tests/test_QssStyleAnalysis/eg7.py
 tests/test_QssStyleAnalysis/test.py
 tests/test_StyleLinker/__init__.py
 tests/test_StyleLinker/eg1_QPushButton.py
 tests/test_StyleLinker/eg2_QLabel.py
+tests/test_SuperPainter/1.py
 tests/test_SuperPainter/__init__.py
 tests/test_SuperPainter/eg1.py
 tests/test_SuperPainter/eg2.py
 tests/test_SuperPainter/eg3.py
 tests/test_SuperPainter/eg4.py
+tests/test_SuperPainter/test.py
 tests/test_qssFile/__init__.py
 tests/test_qssFile/test.py
+tests/test_templateWindow/__init__.py
+tests/test_templateWindow/test_listTemplateWindow.py
 tests/test_uic/__init__.py
 tests/test_uic/test_uic.py
```

### Comparing `PyQtGuiLib-2.6.18.11/README.md` & `PyQtGuiLib-2.7.18.11/README.md`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/acrylic/acrylicWidget.py` & `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/acrylicWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/acrylic/cstruct.py` & `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/cstruct.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/acrylic/windowEffect.py` & `PyQtGuiLib-2.7.18.11/abandonCase/acrylic/windowEffect.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/bubbleWidget.py` & `PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/bubbleWidget_case.py` & `PyQtGuiLib-2.7.18.11/abandonCase/bubbleWidget_case.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/nodeBar.py` & `PyQtGuiLib-2.7.18.11/abandonCase/nodeBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/slideShow.py` & `PyQtGuiLib-2.7.18.11/abandonCase/slideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/slideShow2.py` & `PyQtGuiLib-2.7.18.11/abandonCase/slideShow2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessFrame.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessFrame.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessMainWindow.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessMainWindow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessStackedWidget.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessStackedWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessWidget.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/borderlessWidgetABC.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/borderlessWidgetABC.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/statusBar.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/abandonCase/widgets/titleBar.py` & `PyQtGuiLib-2.7.18.11/abandonCase/widgets/titleBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/setup.py` & `PyQtGuiLib-2.7.18.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name="PyQtGuiLib",
     packages =find_packages(),
-    version="2.6.18.11",
+    version="2.7.18.11",
     author="LX",
     author_email = "lx984608061@163.com",
     description = "Python version of the qt component library.",
     long_description=open('README.md', 'r',encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url = "https://github.com/LX-sys/PyQtGuiLib",
     classifiers = [
```

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/1.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/__init__.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/eg1.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/test_ani/1.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/test_ani/1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_1.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_10.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_10.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_2.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_3.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_4.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_5.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_6.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_7.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_8.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_8.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Animation/tutorial_9.py` & `PyQtGuiLib-2.7.18.11/tests/test_Animation/tutorial_9.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_BubbleWidget.py` & `PyQtGuiLib-2.7.18.11/tests/test_BubbleWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_Notice.py` & `PyQtGuiLib-2.7.18.11/tests/test_Notice.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/__init__.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg1.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg2.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg2.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg3.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg4.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg5.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg5.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg6.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg6.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/eg7.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/eg7.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis/test.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_QssStyleAnalysis.py` & `PyQtGuiLib-2.7.18.11/tests/test_QssStyleAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_SlideShow.py` & `PyQtGuiLib-2.7.18.11/tests/test_SlideShow.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/eg1_QPushButton.py` & `PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg1_QPushButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_StyleLinker/eg2_QLabel.py` & `PyQtGuiLib-2.7.18.11/tests/test_StyleLinker/eg2_QLabel.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg1.py` & `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg1.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg2.py` & `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg2.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # @file:eg2.py
 # @software:PyCharm
 from PyQtGuiLib.header import (
     PYQT_VERSIONS,
     QApplication,
     sys,
     QWidget,
-    QColor
+    QColor,
+    Qt,
+    qt
 )
 from PyQtGuiLib.styles import SuperPainter
 
 
 
 class Test(QWidget):
     def __init__(self):
```

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg3.py` & `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg3.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_SuperPainter/eg4.py` & `PyQtGuiLib-2.7.18.11/tests/test_SuperPainter/eg4.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_barset.py` & `PyQtGuiLib-2.7.18.11/tests/test_barset.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_circularBar.py` & `PyQtGuiLib-2.7.18.11/tests/test_circularBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_colorPalette.py` & `PyQtGuiLib-2.7.18.11/tests/test_colorPalette.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_comboBox.py` & `PyQtGuiLib-2.7.18.11/tests/test_comboBox.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_dynamicTLine.py` & `PyQtGuiLib-2.7.18.11/tests/test_dynamicTLine.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_flowLayot.py` & `PyQtGuiLib-2.7.18.11/tests/test_flowLayot.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_gradientBar.py` & `PyQtGuiLib-2.7.18.11/tests/test_gradientBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_listWidget.py` & `PyQtGuiLib-2.7.18.11/tests/test_listWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_loadbar.py` & `PyQtGuiLib-2.7.18.11/tests/test_loadbar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_no_border.py` & `PyQtGuiLib-2.7.18.11/tests/test_no_border.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_no_border_pullOver.py` & `PyQtGuiLib-2.7.18.11/tests/test_no_border_pullOver.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_pullOverWidget.py` & `PyQtGuiLib-2.7.18.11/tests/test_pullOverWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_qssFile/test.py` & `PyQtGuiLib-2.7.18.11/tests/test_qssFile/test.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_rollWidget.py` & `PyQtGuiLib-2.7.18.11/tests/test_rollWidget.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_slider.py` & `PyQtGuiLib-2.7.18.11/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_statusBar.py` & `PyQtGuiLib-2.7.18.11/tests/test_statusBar.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_styles.py` & `PyQtGuiLib-2.7.18.11/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_switchButton.py` & `PyQtGuiLib-2.7.18.11/tests/test_switchButton.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_template.py` & `PyQtGuiLib-2.7.18.11/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_toolList.py` & `PyQtGuiLib-2.7.18.11/tests/test_toolList.py`

 * *Files identical despite different names*

### Comparing `PyQtGuiLib-2.6.18.11/tests/test_waterBar.py` & `PyQtGuiLib-2.7.18.11/tests/test_waterBar.py`

 * *Files identical despite different names*

