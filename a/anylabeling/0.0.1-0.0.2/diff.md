# Comparing `tmp/anylabeling-0.0.1.tar.gz` & `tmp/anylabeling-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.0.1.tar", last modified: Sat Apr  8 19:08:19 2023, max compression
+gzip compressed data, was "anylabeling-0.0.2.tar", last modified: Tue Apr 11 18:27:41 2023, max compression
```

## Comparing `anylabeling-0.0.1.tar` & `anylabeling-0.0.2.tar`

### file list

```diff
@@ -1,125 +1,81 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.652703 anylabeling-0.0.1/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.1/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.1/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1747 2023-04-08 19:08:19.652440 anylabeling-0.0.1/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)      963 2023-04-08 19:01:48.000000 anylabeling-0.0.1/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.628595 anylabeling-0.0.1/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1053 2023-04-08 18:53:13.000000 anylabeling-0.0.1/anylabeling/app.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.630048 anylabeling-0.0.1/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.630371 anylabeling-0.0.1/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.1/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2226 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.630753 anylabeling-0.0.1/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.631981 anylabeling-0.0.1/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/services/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)       73 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/storage.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.632453 anylabeling-0.0.1/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.633012 anylabeling-0.0.1/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.633383 anylabeling-0.0.1/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      616 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labeling_wrapper.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.635756 anylabeling-0.0.1/anylabeling/views/labeling/labelme/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5760 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-08 18:56:18.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.648764 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36694 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6350 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    82410 2023-04-08 19:03:22.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/labelme_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1812 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/testing.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2369 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/tracker.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.649831 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      510 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      669 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      769 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.652049 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      446 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    42162 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      302 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-08 18:50:31.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1113 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1261 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      697 2023-04-08 18:49:39.000000 anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      771 2023-04-08 18:54:53.000000 anylabeling-0.0.1/anylabeling/views/maintabs.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1451 2023-04-08 19:01:27.000000 anylabeling-0.0.1/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-08 19:08:19.629810 anylabeling-0.0.1/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1747 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5132 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      179 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-08 19:08:19.000000 anylabeling-0.0.1/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.1/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-08 19:08:19.652754 anylabeling-0.0.1/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2314 2023-04-08 19:02:38.000000 anylabeling-0.0.1/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.274711 anylabeling-0.0.2/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.0.2/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      120 2023-04-08 18:53:13.000000 anylabeling-0.0.2/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2039 2023-04-11 18:27:41.274552 anylabeling-0.0.2/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1153 2023-04-11 17:52:02.000000 anylabeling-0.0.2/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.262849 anylabeling-0.0.2/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       22 2023-04-11 18:19:13.000000 anylabeling-0.0.2/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1062 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/app.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264833 anylabeling-0.0.2/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264981 anylabeling-0.0.2/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.0.2/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      315 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1171 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.265213 anylabeling-0.0.2/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   423402 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.266562 anylabeling-0.0.2/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.267300 anylabeling-0.0.2/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2955 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5277 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9837 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1284 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5127 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.267918 anylabeling-0.0.2/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.268486 anylabeling-0.0.2/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9637 2023-04-08 18:49:39.000000 anylabeling-0.0.2/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.270836 anylabeling-0.0.2/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      343 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5758 2023-04-08 20:04:23.000000 anylabeling-0.0.2/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2717 2023-04-09 06:42:35.000000 anylabeling-0.0.2/anylabeling/views/labeling/config.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6405 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    88768 2023-04-11 18:18:40.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      606 2023-04-08 20:07:28.000000 anylabeling-0.0.2/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1811 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10541 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.271873 anylabeling-0.0.2/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.273915 anylabeling-0.0.2/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.274338 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6906 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46264 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8023 2023-04-08 19:49:25.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5778 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1390 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      768 2023-04-08 20:09:45.000000 anylabeling-0.0.2/anylabeling/views/maintabs.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      981 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/mainwindow.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1458 2023-04-11 17:52:02.000000 anylabeling-0.0.2/anylabeling/views/mainwindow_tabs.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-11 18:27:41.264124 anylabeling-0.0.2/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2039 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2620 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      235 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-11 18:27:41.000000 anylabeling-0.0.2/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      204 2023-04-08 18:53:13.000000 anylabeling-0.0.2/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-11 18:27:41.274754 anylabeling-0.0.2/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2503 2023-04-11 17:52:02.000000 anylabeling-0.0.2/setup.py
```

### Comparing `anylabeling-0.0.1/LICENSE` & `anylabeling-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/PKG-INFO` & `anylabeling-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.1
+Version: 0.0.2
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
-  <p align="center">Effortless data labeling with AI support<p>
-  <p align="center">With <b>Improved Labelme</b> and <b>Segment Anything</b><p>
+  <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
+  <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 
 ## I. Install and run
 
@@ -76,10 +78,9 @@
 
 ```
 python anylabeling/app.py
 ```
 
 ## III. References
 
-- labelme
-- gpu_util
+- Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

### Comparing `anylabeling-0.0.1/README.md` & `anylabeling-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
-  <p align="center">Effortless data labeling with AI support<p>
-  <p align="center">With <b>Improved Labelme</b> and <b>Segment Anything</b><p>
+  <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
+  <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 
 ## I. Install and run
 
@@ -55,10 +55,9 @@
 
 ```
 python anylabeling/app.py
 ```
 
 ## III. References
 
-- labelme
-- gpu_util
+- Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

### Comparing `anylabeling-0.0.1/anylabeling/app.py` & `anylabeling-0.0.2/anylabeling/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 
     QtCore.QCoreApplication.setAttribute(QtCore.Qt.AA_ShareOpenGLContexts)
     app = QApplication(sys.argv)
     app.processEvents()
 
     main_win = MainWindow(app)
 
-    main_win.show()
+    main_win.showMaximized()
     sys.exit(app.exec_())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `anylabeling-0.0.1/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.0.2/anylabeling/configs/anylabeling_config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -106,10 +106,8 @@
   add_point_to_edge: Ctrl+Shift+P
   edit_label: Ctrl+E
   toggle_keep_prev_mode: Ctrl+P
   remove_selected_point: Backspace
   group_selected_shapes: G
   ungroup_selected_shapes: U
 
-  tracking: T
-  load_ai_model: L
-  auto_label: I
+  auto_label: Ctrt+A
```

### Comparing `anylabeling-0.0.1/anylabeling/resources/resources.py` & `anylabeling-0.0.2/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/common/tableview.py` & `anylabeling-0.0.2/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/common/toaster.py` & `anylabeling-0.0.2/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labeling_wrapper.py` & `anylabeling-0.0.2/anylabeling/views/labeling/label_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module defines labelme wrapper and related functions"""
 
 from PyQt5.QtWidgets import QVBoxLayout, QWidget
 
-from .labelme.labelme_widget import LabelmeWidget
+from .label_widget import LabelmeWidget
 
 
 class LabelingWrapper(QWidget):
     """Wrapper widget for labelme module"""
 
     def __init__(self, parent):
         super().__init__()
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/__main__.py` & `anylabeling-0.0.2/anylabeling/views/labeling/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 import yaml
 from PyQt5 import QtCore, QtWidgets
 
 from . import __appname__, __version__
 from .config import get_config
-from .labelme_widget import MainWindow
+from .label_widget import MainWindow
 from .logger import logger
 from .utils import new_icon
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/config.py` & `anylabeling-0.0.2/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/label_file.py` & `anylabeling-0.0.2/anylabeling/views/labeling/label_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 
 class LabelFileError(Exception):
     pass
 
 
 class LabelFile:
-
     suffix = ".json"
 
     def __init__(self, filename=None):
         self.shapes = []
         self.image_path = None
         self.image_data = None
         if filename is not None:
@@ -83,17 +82,19 @@
                 logger.warning(
                     "Loading JSON file (%s) of unknown version", filename
                 )
             elif (
                 version.split(".")[0] != __version__.split(".", maxsplit=1)[0]
             ):
                 logger.warning(
-                    "This JSON file (%s) may be incompatible with "
-                    "current labelme. version in file: %s, "
-                    "current version: %s",
+                    (
+                        "This JSON file (%s) may be incompatible with "
+                        "current labelme. version in file: %s, "
+                        "current version: %s"
+                    ),
                     filename,
                     version,
                     __version__,
                 )
 
             if data["imageData"] is not None:
                 image_data = base64.b64decode(data["imageData"])
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/labelme_widget.py` & `anylabeling-0.0.2/anylabeling/views/labeling/label_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,43 @@
 import os.path as osp
 import re
 import webbrowser
 
 import imgviz
 import natsort
 from PyQt5 import QtCore, QtGui, QtWidgets
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import (QDockWidget, QHBoxLayout, QLabel, QMessageBox,
-                             QPlainTextEdit, QVBoxLayout, QWhatsThis)
+from PyQt5.QtCore import Qt, pyqtSlot
+from PyQt5.QtWidgets import (
+    QDockWidget,
+    QHBoxLayout,
+    QLabel,
+    QPlainTextEdit,
+    QVBoxLayout,
+    QWhatsThis,
+)
 
 from . import __appname__, utils
 from .config import get_config
 from .label_file import LabelFile, LabelFileError
 from .logger import logger
 from .shape import Shape
-from .tracker import Tracker
-from .widgets import (BrightnessContrastDialog, Canvas, FileDialogPreview,
-                      LabelDialog, LabelListWidget, LabelListWidgetItem,
-                      ToolBar, UniqueLabelQListWidget, ZoomWidget)
+from .widgets import (
+    BrightnessContrastDialog,
+    Canvas,
+    FileDialogPreview,
+    LabelDialog,
+    LabelListWidget,
+    LabelListWidgetItem,
+    ToolBar,
+    UniqueLabelQListWidget,
+    ZoomWidget,
+    AutoLabelingWidget,
+)
+
+from anylabeling.services.auto_labeling.types import AutoLabelingMode
 
 LABEL_COLORMAP = imgviz.label_colormap()
 
 # Green for the first label
 LABEL_COLORMAP[2] = LABEL_COLORMAP[1]
 LABEL_COLORMAP[1] = [0, 180, 33]
 
@@ -56,21 +72,15 @@
 
         self.filename = None
         self.image_path = None
         self.image_data = None
         self.label_file = None
         self.other_data = {}
 
-        # Tracker
-        self.tracker = Tracker()
-
-        # AI models for auto labeling
-        self.ai_model = None
-
-        # see configs/anylabeling_config.yaml for valid configuration
+        # see configs/labelme_config.yaml for valid configuration
         if config is None:
             config = get_config()
         self._config = config
 
         # set default shape colors
         Shape.line_color = QtGui.QColor(*self._config["shape"]["line_color"])
         Shape.fill_color = QtGui.QColor(*self._config["shape"]["fill_color"])
@@ -115,26 +125,42 @@
 
         self.flag_dock = self.flag_widget = None
         self.flag_dock = QtWidgets.QDockWidget(self.tr("Flags"), self)
         self.flag_dock.setObjectName("Flags")
         self.flag_widget = QtWidgets.QListWidget()
         if config["flags"]:
             self.load_flags({k: False for k in config["flags"]})
+        else:
+            self.flag_dock.hide()
         self.flag_dock.setWidget(self.flag_widget)
         self.flag_widget.itemChanged.connect(self.set_dirty)
+        self.flag_dock.setStyleSheet(
+            "QDockWidget::title {"
+            "text-align: center;"
+            "padding: 0px;"
+            "background-color: #f0f0f0;"
+            "}"
+        )
 
         self.label_list.item_selection_changed.connect(
             self.label_selection_changed
         )
         self.label_list.item_double_clicked.connect(self.edit_label)
         self.label_list.item_changed.connect(self.label_item_changed)
         self.label_list.item_dropped.connect(self.label_order_changed)
         self.shape_dock = QtWidgets.QDockWidget(self.tr("Objects"), self)
-        self.shape_dock.setObjectName("Labels")
+        self.shape_dock.setObjectName("Objects")
         self.shape_dock.setWidget(self.label_list)
+        self.shape_dock.setStyleSheet(
+            "QDockWidget::title {"
+            "text-align: center;"
+            "padding: 0px;"
+            "background-color: #f0f0f0;"
+            "}"
+        )
 
         self.unique_label_list = UniqueLabelQListWidget()
         self.unique_label_list.setToolTip(
             self.tr(
                 "Select label to start annotating for it. "
                 "Press 'Esc' to deselect."
             )
@@ -144,37 +170,52 @@
                 item = self.unique_label_list.create_item_from_label(label)
                 self.unique_label_list.addItem(item)
                 rgb = self._get_rgb_by_label(label)
                 self.unique_label_list.set_item_label(item, label, rgb)
         self.label_dock = QtWidgets.QDockWidget(self.tr("Labels"), self)
         self.label_dock.setObjectName("Labels")
         self.label_dock.setWidget(self.unique_label_list)
+        self.label_dock.setStyleSheet(
+            "QDockWidget::title {"
+            "text-align: center;"
+            "padding: 0px;"
+            "background-color: #f0f0f0;"
+            "}"
+        )
 
         self.file_search = QtWidgets.QLineEdit()
         self.file_search.setPlaceholderText(self.tr("Search Filename"))
         self.file_search.textChanged.connect(self.file_search_changed)
         self.file_list_widget = QtWidgets.QListWidget()
         self.file_list_widget.itemSelectionChanged.connect(
             self.file_selection_changed
         )
         file_list_layout = QtWidgets.QVBoxLayout()
         file_list_layout.setContentsMargins(0, 0, 0, 0)
         file_list_layout.setSpacing(0)
         file_list_layout.addWidget(self.file_search)
         file_list_layout.addWidget(self.file_list_widget)
-        self.file_dock = QtWidgets.QDockWidget(self.tr("File List"), self)
+        self.file_dock = QtWidgets.QDockWidget(self.tr("Files"), self)
         self.file_dock.setObjectName("Files")
         file_list_widget = QtWidgets.QWidget()
         file_list_widget.setLayout(file_list_layout)
         self.file_dock.setWidget(file_list_widget)
+        self.file_dock.setStyleSheet(
+            "QDockWidget::title {"
+            "text-align: center;"
+            "padding: 0px;"
+            "background-color: #f0f0f0;"
+            "}"
+        )
 
         self.zoom_widget = ZoomWidget()
         self.setAcceptDrops(True)
 
         self.canvas = self.label_list.canvas = Canvas(
+            parent=self,
             epsilon=self._config["epsilon"],
             double_click=self._config["canvas"]["double_click"],
             num_backups=self._config["canvas"]["num_backups"],
         )
         self.canvas.zoom_request.connect(self.zoom_request)
 
         scroll_area = QtWidgets.QScrollArea()
@@ -599,34 +640,20 @@
             self.tr("Fill polygon while drawing"),
             checkable=True,
             enabled=True,
         )
         fill_drawing.trigger()
 
         # AI Actions
-        track = action(
-            self.tr("&Tracking"),
-            self.track,
-            shortcuts["tracking"],
-            "app",
-            self.tr("Track object"),
-        )
-        ai_load_model = action(
-            self.tr("&Load AI Model"),
-            self.ai_load_model,
-            shortcuts["load_ai_model"],
-            "upload_brain",
-            self.tr("Load AI Model"),
-        )
-        ai_predict = action(
-            self.tr("&Predict Shapes"),
-            self.ai_predict,
+        toggle_auto_labeling_widget = action(
+            self.tr("&Auto Labeling"),
+            self.toggle_auto_labeling_widget,
             shortcuts["auto_label"],
             "brain",
-            self.tr("Predict shapes"),
+            self.tr("Auto Labeling"),
         )
 
         # Lavel list context menu.
         label_menu = QtWidgets.QMenu()
         utils.add_actions(label_menu, (edit, delete))
         self.label_list.setContextMenuPolicy(Qt.CustomContextMenu)
         self.label_list.customContextMenuRequested.connect(
@@ -809,54 +836,83 @@
             create_mode,
             self.actions.create_rectangle_mode,
             self.actions.create_cirle_mode,
             self.actions.create_line_mode,
             self.actions.create_point_mode,
             self.actions.create_line_strip_mode,
             edit_mode,
-            duplicate,
-            copy,
-            paste,
+            # duplicate,
+            # copy,
+            # paste,
             delete,
             undo,
-            brightness_contrast,
+            # brightness_contrast,
             None,
             zoom,
             fit_width,
-            track,
-            ai_load_model,
-            ai_predict,
+            toggle_auto_labeling_widget,
         )
 
         layout = QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
 
         layout.addWidget(self.tools)
         central_layout = QVBoxLayout()
         central_layout.setContentsMargins(0, 0, 0, 0)
-        label_instruction = QLabel(
-            "<b>Shortcuts:</b> Previous: <b>A</b>, Next: <b>D</b>, Rectangle:"
-            " <b>R</b>, Polygon: <b>P</b>"
+        self.label_instruction = QLabel(self.get_labeling_instruction())
+        self.label_instruction.setContentsMargins(0, 0, 0, 0)
+        self.auto_labeling_widget = AutoLabelingWidget(self)
+        self.auto_labeling_widget.auto_segmentation_requested.connect(
+            self.on_auto_segmentation_requested
+        )
+        self.auto_labeling_widget.auto_segmentation_disabled.connect(
+            self.on_auto_segmentation_disabled
+        )
+        self.canvas.auto_labeling_marks_updated.connect(
+            self.auto_labeling_widget.on_new_marks
+        )
+        self.auto_labeling_widget.auto_labeling_mode_changed.connect(
+            self.canvas.set_auto_labeling_mode
         )
-        label_instruction.setContentsMargins(0, 10, 0, 10)
-        central_layout.addWidget(label_instruction)
+        self.auto_labeling_widget.clear_auto_labeling_action_requested.connect(
+            self.clear_auto_labeling_marks
+        )
+        self.auto_labeling_widget.finish_auto_labeling_object_action_requested.connect(
+            self.finish_auto_labeling_object
+        )
+        self.canvas.auto_labeling_mode_changed.connect(
+            lambda mode: self.auto_labeling_widget.update_button_colors(mode)
+        )
+        self.auto_labeling_widget.hide()  # Hide by default
+        central_layout.addWidget(self.label_instruction)
+        central_layout.addWidget(self.auto_labeling_widget)
         central_layout.addWidget(scroll_area)
         layout.addItem(central_layout)
 
         # Save central area for resize
         self._central_widget = scroll_area
 
         # Stretch central area (image view)
         layout.setStretch(1, 1)
 
         right_sidebar_layout = QVBoxLayout()
         right_sidebar_layout.setContentsMargins(0, 0, 0, 0)
-        self.shape_text_label = QLabel("Shape Text")
+        self.shape_text_label = QLabel("Object Text")
+        self.shape_text_label.setStyleSheet(
+            "QLabel {"
+            "text-align: center;"
+            "padding: 0px;"
+            "font-size: 11px;"
+            "margin-bottom: 5px;"
+            "}"
+        )
         self.shape_text_edit = QPlainTextEdit()
-        right_sidebar_layout.addWidget(self.shape_text_label)
+        right_sidebar_layout.addWidget(
+            self.shape_text_label, 0, Qt.AlignCenter
+        )
         right_sidebar_layout.addWidget(self.shape_text_edit)
         right_sidebar_layout.addWidget(self.flag_dock)
         right_sidebar_layout.addWidget(self.label_dock)
         right_sidebar_layout.addWidget(self.shape_dock)
         right_sidebar_layout.addWidget(self.file_dock)
         self.file_dock.setFeatures(QDockWidget.DockWidgetFloatable)
         dock_features = (
@@ -941,16 +997,33 @@
 
         self.populate_mode_actions()
 
         self.first_start = True
         if self.first_start:
             QWhatsThis.enterWhatsThisMode()
 
+    def get_labeling_instruction(self):
+        return (
+            f"<b>Mode:</b> {self.canvas.get_mode()} - <b>Shortcuts:</b>"
+            " Previous: <b>A</b>, Next: <b>D</b>, Rectangle: <b>R</b>,"
+            " Polygon: <b>P</b>"
+        )
+
+    @pyqtSlot()
+    def on_auto_segmentation_requested(self):
+        self.canvas.set_auto_labeling(True)
+        self.label_instruction.setText(self.get_labeling_instruction())
+
+    @pyqtSlot()
+    def on_auto_segmentation_disabled(self):
+        self.canvas.set_auto_labeling(False)
+        self.label_instruction.setText(self.get_labeling_instruction())
+
     def menu(self, title, actions=None):
-        menu = self.parent.parent.parent.menuBar().addMenu(title)
+        menu = self.parent.parent.menuBar().addMenu(title)
         if actions:
             utils.add_actions(menu, actions)
         return menu
 
     def central_widget(self):
         return self._central_widget
 
@@ -962,15 +1035,15 @@
         toolbar.setIconSize(QtCore.QSize(20, 20))
         toolbar.setMaximumWidth(40)
         if actions:
             utils.add_actions(toolbar, actions)
         return toolbar
 
     def statusBar(self):
-        return self.parent.parent.parent.statusBar()
+        return self.parent.parent.statusBar()
 
     def no_shape(self):
         return len(self.label_list) == 0
 
     def populate_mode_actions(self):
         tool = self.actions.tool
         menu = self.actions.menu
@@ -1205,28 +1278,36 @@
                 ),
             )
             return
         shape.label = text
         shape.flags = flags
         shape.group_id = group_id
 
+        # Update unique label list
+        if not self.unique_label_list.find_items_by_label(shape.label):
+            unique_label_item = self.unique_label_list.create_item_from_label(
+                shape.label
+            )
+            self.unique_label_list.addItem(unique_label_item)
+            rgb = self._get_rgb_by_label(shape.label)
+            self.unique_label_list.set_item_label(
+                unique_label_item, shape.label, rgb
+            )
+
         self._update_shape_color(shape)
         if shape.group_id is None:
+            color = shape.fill_color.getRgb()[:3]
             item.setText(
                 '{} <font color="#{:02x}{:02x}{:02x}">●</font>'.format(
-                    html.escape(shape.label), *shape.fill_color.getRgb()[:3]
+                    html.escape(shape.label), *color
                 )
             )
         else:
             item.setText(f"{shape.label} ({shape.group_id})")
         self.set_dirty()
-        if not self.unique_label_list.find_items_by_label(shape.label):
-            item = QtWidgets.QListWidgetItem()
-            item.setData(Qt.UserRole, shape.label)
-            self.unique_label_list.addItem(item)
 
     def file_search_changed(self):
         self.import_image_folder(
             self.last_open_dir,
             pattern=self.file_search.text(),
             load=False,
         )
@@ -1261,15 +1342,15 @@
         self._no_selection_slot = False
         n_selected = len(selected_shapes)
         self.actions.delete.setEnabled(n_selected)
         self.actions.duplicate.setEnabled(n_selected)
         self.actions.copy.setEnabled(n_selected)
         self.actions.edit.setEnabled(n_selected == 1)
         if len(selected_shapes) == 1:
-            self.shape_text_label.setText("Shape Text")
+            self.shape_text_label.setText("Object Text")
             self.shape_text_edit.textChanged.disconnect()
             self.shape_text_edit.setPlainText(selected_shapes[0].text)
             self.shape_text_edit.textChanged.connect(self.shape_text_changed)
         else:
             self.shape_text_label.setText("Image Text")
             self.shape_text_edit.textChanged.disconnect()
             self.shape_text_edit.setPlainText(
@@ -1317,14 +1398,17 @@
         shape.hvertex_fill_color = QtGui.QColor(255, 255, 255)
         shape.fill_color = QtGui.QColor(r, g, b, 128)
         shape.select_line_color = QtGui.QColor(255, 255, 255)
         shape.select_fill_color = QtGui.QColor(r, g, b, 155)
 
     def _get_rgb_by_label(self, label):
         if self._config["shape_color"] == "auto":
+            if not self.unique_label_list.find_items_by_label(label):
+                item = self.unique_label_list.create_item_from_label(label)
+                self.unique_label_list.addItem(item)
             item = self.unique_label_list.find_items_by_label(label)[0]
             label_id = self.unique_label_list.indexFromItem(item).row() + 1
             label_id += self._config["shift_auto_shape_color"]
             return LABEL_COLORMAP[label_id % len(LABEL_COLORMAP)]
         if (
             self._config["shape_color"] == "manual"
             and self._config["label_colors"]
@@ -1376,15 +1460,16 @@
             default_flags = {}
             if self._config["label_flags"]:
                 for pattern, keys in self._config["label_flags"].items():
                     if re.match(pattern, label):
                         for key in keys:
                             default_flags[key] = False
             shape.flags = default_flags
-            shape.flags.update(flags)
+            if flags:
+                shape.flags.update(flags)
             shape.other_data = other_data
 
             s.append(shape)
         self.load_shapes(s)
 
     def load_flags(self, flags):
         self.flag_widget.clear()
@@ -1496,15 +1581,21 @@
         """
         items = self.unique_label_list.selectedItems()
         text = None
         if items:
             text = items[0].data(Qt.UserRole)
         flags = {}
         group_id = None
-        if self._config["display_label_popup"] or not text:
+
+        if self.canvas.shapes[-1].label in [
+            AutoLabelingMode.ADD,
+            AutoLabelingMode.REMOVE,
+        ]:
+            text = self.canvas.shapes[-1].label
+        elif self._config["display_label_popup"] or not text:
             previous_text = self.label_dialog.edit.text()
             text, flags, group_id = self.label_dialog.pop_up(text)
             if not text:
                 self.label_dialog.edit.setText(previous_text)
 
         if text and not self.validate_label(text):
             self.error_message(
@@ -1633,17 +1724,14 @@
     def toggle_polygons(self, value):
         for item in self.label_list:
             item.setCheckState(Qt.Checked if value else Qt.Unchecked)
 
     def load_file(self, filename=None):
         """Load the specified file, or the last opened file if None."""
 
-        # Update tracker
-        self.tracker.update(self.canvas.shapes, self.image)
-
         # Changing file_list_widget loads file
         if filename in self.image_list and (
             self.file_list_widget.currentRow()
             != self.image_list.index(filename)
         ):
             self.file_list_widget.setCurrentRow(
                 self.image_list.index(filename)
@@ -1827,17 +1915,15 @@
         if not self.may_continue():
             event.ignore()
         self.settings.setValue(
             "filename", self.filename if self.filename else ""
         )
         self.settings.setValue("window/size", self.size())
         self.settings.setValue("window/position", self.pos())
-        self.settings.setValue(
-            "window/state", self.parent.parent.parent.saveState()
-        )
+        self.settings.setValue("window/state", self.parent.parent.saveState())
         self.settings.setValue("recent_files", self.recent_files)
         # ask the use for where to save the labels
         # self.settings.setValue('window/geometry', self.saveGeometry())
 
     # QT Overload
     def dragEnterEvent(self, event):
         extensions = [
@@ -2256,45 +2342,132 @@
             for file in files:
                 if file.lower().endswith(tuple(extensions)):
                     relative_path = osp.join(root, file)
                     images.append(relative_path)
         images = natsort.os_sorted(images)
         return images
 
-    def track(self):
-        QMessageBox.warning(self, "Warning", "Tracking is not supported now.")
-        # predicted_shapes = self.tracker.get(self.image)
-        # self.load_shapes(predicted_shapes, replace=True)
-        # self.set_dirty()
-
-    def ai_load_model(self):
-        """Load AI model from disk."""
-        file_path = QtWidgets.QFileDialog.getOpenFileName(
-            self, "Select AI Model Config", ".", "Model config file (*.yaml)"
-        )
-        if not file_path[0]:
+    def toggle_auto_labeling_widget(self):
+        """Toggle auto labeling widget visibility."""
+        if self.auto_labeling_widget.isVisible():
+            self.auto_labeling_widget.hide()
+        else:
+            self.auto_labeling_widget.show()
+
+    @pyqtSlot()
+    def new_shapes_from_auto_labeling(self, auto_labeling_result):
+        """Apply auto labeling results to the current image."""
+        if not self.image or not self.image_path:
+            return
+        # Clear existing shapes
+        if auto_labeling_result.replace:
+            self.load_shapes([], replace=True)
+            self.label_list.clear()
+            self.load_shapes(auto_labeling_result.shapes, replace=True)
+        else:  # Just update existing shapes
+            # Remove shapes with label "AUTOLABEL_OBJECT"
+            for shape in self.canvas.shapes:
+                if shape.label == "AUTOLABEL_OBJECT":
+                    item = self.label_list.find_item_by_shape(shape)
+                    self.label_list.remove_item(item)
+            self.load_shapes(auto_labeling_result.shapes, replace=False)
+
+        self.set_dirty()
+
+    def clear_auto_labeling_marks(self):
+        """Clear auto labeling marks."""
+        for shape in self.canvas.shapes:
+            if shape.label in [
+                AutoLabelingMode.OBJECT,
+                AutoLabelingMode.ADD,
+                AutoLabelingMode.REMOVE,
+            ]:
+                item = self.label_list.find_item_by_shape(shape)
+                self.label_list.remove_item(item)
+        self.canvas.update()
+
+    def finish_auto_labeling_object(self):
+        """Finish auto labeling object."""
+        has_object = False
+        for shape in self.canvas.shapes:
+            if shape.label == AutoLabelingMode.OBJECT:
+                has_object = True
+                break
+
+        # If there is no object, do nothing
+        if not has_object:
             return
-        file_path = file_path[0]
-        try:
-            # TODO: Load AI model
-            self.ai_model = None
-        except Exception as e:
-            QMessageBox.warning(self, "Error", f"Failed to load AI model: {e}")
-            return
-        self.statusBar().showMessage(f"AI Model loaded from {file_path}", 5000)
-
-    def ai_predict(self):
-        """Predict shapes using AI model"""
-        if self.image_path is None:
-            QMessageBox.warning(self, "Warning", "Please load images first.")
+
+        # Ask a label for the object
+        text, flags, group_id = self.label_dialog.pop_up(
+            text="",
+            flags={},
+            group_id=None,
+        )
+        if text is None:
             return
-        if self.ai_model is None:
-            QMessageBox.warning(
-                self,
-                "Warning",
-                "No AI model is loaded. Please load a model first.",
+        if not self.validate_label(text):
+            self.error_message(
+                self.tr("Invalid label"),
+                self.tr("Invalid label '{}' with validation type '{}'").format(
+                    text, self._config["validate_label"]
+                ),
             )
             return
 
-        shapes = self.ai_model.predict_shapes(self.image)
-        self.load_shapes(shapes, replace=True)
-        self.set_dirty()
+        # Update label for the object
+        updated_shapes = False
+        for shape in self.canvas.shapes:
+            if shape.label == AutoLabelingMode.OBJECT:
+                updated_shapes = True
+                shape.label = text
+                shape.flags = flags
+                shape.group_id = group_id
+                # Update unique label list
+                if not self.unique_label_list.find_items_by_label(shape.label):
+                    unique_label_item = self.unique_label_list.create_item_from_label(
+                        shape.label
+                    )
+                    self.unique_label_list.addItem(unique_label_item)
+                    rgb = self._get_rgb_by_label(shape.label)
+                    self.unique_label_list.set_item_label(
+                        unique_label_item, shape.label, rgb
+                    )
+
+                # Update label list
+                item = self.label_list.find_item_by_shape(shape)
+                if shape.group_id is None:
+                    color = shape.fill_color.getRgb()[:3]
+                    item.setText(
+                        '{} <font color="#{:02x}{:02x}{:02x}">●</font>'.format(
+                            html.escape(shape.label), *color
+                        )
+                    )
+                else:
+                    item.setText(f"{shape.label} ({shape.group_id})")
+
+        # Remove all ADD and REMOVE marks
+        for shape in self.canvas.shapes:
+            if shape.label in [AutoLabelingMode.ADD, AutoLabelingMode.REMOVE]:
+                item = self.label_list.find_item_by_shape(shape)
+                self.label_list.remove_item(item)
+
+        # Remove all auto labeling marks from unique label list
+        for item in self.unique_label_list.find_items_by_label(
+            AutoLabelingMode.OBJECT
+        ):
+            self.unique_label_list.takeItem(self.unique_label_list.row(item))
+        for item in self.unique_label_list.find_items_by_label(
+            AutoLabelingMode.ADD
+        ):
+            self.unique_label_list.takeItem(self.unique_label_list.row(item))
+        for item in self.unique_label_list.find_items_by_label(
+            AutoLabelingMode.REMOVE
+        ):
+            self.unique_label_list.takeItem(self.unique_label_list.row(item))
+
+        # Update shape colors
+        for shape in self.canvas.shapes:
+            self._update_shape_color(shape)
+
+        if updated_shapes:
+            self.set_dirty()
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/logger.py` & `anylabeling-0.0.2/anylabeling/views/labeling/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             record.module2 = termcolor.colored(record.module, color="cyan")
             record.funcName2 = termcolor.colored(record.funcName, color="cyan")
             record.lineno2 = termcolor.colored(record.lineno, color="cyan")
         return logging.Formatter.format(self, record)
 
 
 class ColoredLogger(logging.Logger):
-
     FORMAT = (
         "[%(levelname2)s] %(module2)s:%(funcName2)s:%(lineno2)s - %(message2)s"
     )
 
     def __init__(self, name):
         logging.Logger.__init__(self, name, logging.INFO)
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/shape.py` & `anylabeling-0.0.2/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/testing.py` & `anylabeling-0.0.2/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/_io.py` & `anylabeling-0.0.2/anylabeling/views/labeling/utils/_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import imgviz
 import numpy as np
 import PIL.Image
 
 
 def lblsave(filename, lbl):
-
     if osp.splitext(filename)[1] != ".png":
         filename += ".png"
     # Assume label ranses [-1, 254] for int32,
     # and [0, 255] for uint8 as VOC.
     if lbl.min() >= -1 and lbl.max() < 255:
         lbl_pil = PIL.Image.fromarray(lbl.astype(np.uint8), mode="P")
         colormap = imgviz.label_colormap()
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/image.py` & `anylabeling-0.0.2/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/qt.py` & `anylabeling-0.0.2/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/utils/shape.py` & `anylabeling-0.0.2/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/brightness_contrast_dialog.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/canvas.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QWheelEvent
 
 from .. import utils
 from ..shape import Shape
 
+from anylabeling.services.auto_labeling.types import AutoLabelingMode
+
 CURSOR_DEFAULT = QtCore.Qt.ArrowCursor
 CURSOR_POINT = QtCore.Qt.PointingHandCursor
 CURSOR_DRAW = QtCore.Qt.CrossCursor
 CURSOR_MOVE = QtCore.Qt.ClosedHandCursor
 CURSOR_GRAB = QtCore.Qt.OpenHandCursor
 
 MOVE_SPEED = 5.0
@@ -26,34 +28,38 @@
     zoom_request = QtCore.pyqtSignal(int, QtCore.QPoint)
     scroll_request = QtCore.pyqtSignal(int, int)
     new_shape = QtCore.pyqtSignal()
     selection_changed = QtCore.pyqtSignal(list)
     shape_moved = QtCore.pyqtSignal()
     drawing_polygon = QtCore.pyqtSignal(bool)
     vertex_selected = QtCore.pyqtSignal(bool)
+    auto_labeling_marks_updated = QtCore.pyqtSignal(list)
+    auto_labeling_mode_changed = QtCore.pyqtSignal(AutoLabelingMode)
 
     CREATE, EDIT = 0, 1
-    CREATE, EDIT = 0, 1
 
     # polygon, rectangle, line, or point
     _create_mode = "polygon"
 
     _fill_drawing = False
 
     def __init__(self, *args, **kwargs):
         self.epsilon = kwargs.pop("epsilon", 10.0)
         self.double_click = kwargs.pop("double_click", "close")
         if self.double_click not in [None, "close"]:
             raise ValueError(
                 f"Unexpected value for double_click event: {self.double_click}"
             )
         self.num_backups = kwargs.pop("num_backups", 10)
+        self.parent = kwargs.pop("parent")
         super().__init__(*args, **kwargs)
         # Initialise local state.
         self.mode = self.EDIT
+        self.is_auto_labeling = False
+        self.auto_labeling_mode: AutoLabelingMode = None
         self.shapes = []
         self.shapes_backups = []
         self.current = None
         self.selected_shapes = []  # save the selected shapes here
         self.selected_shapes_copy = []
         # self.line represents:
         #   - create_mode == 'polygon': edge from last point to current
@@ -87,14 +93,22 @@
         # Set widget options.
         self.setMouseTracking(True)
         self.setFocusPolicy(QtCore.Qt.WheelFocus)
         self.show_cross_line = True
         self.show_shape_groups = True
         self.show_texts = True
 
+    def set_auto_labeling_mode(self, mode: AutoLabelingMode):
+        """Set auto labeling mode"""
+        self.is_auto_labeling = True
+        self.auto_labeling_mode = mode
+        self.create_mode = mode.shape_type
+        self.parent.toggle_draw_mode(False, mode.shape_type)
+        self.auto_labeling_mode_changed.emit(mode)
+
     def fill_drawing(self):
         """Get option to fill shapes by color"""
         return self._fill_drawing
 
     def set_fill_drawing(self, value):
         """Set shape filling option"""
         self._fill_drawing = value
@@ -176,14 +190,38 @@
         """Check if user is drawing (mode==CREATE)"""
         return self.mode == self.CREATE
 
     def editing(self):
         """Check if user is editing (mode==EDIT)"""
         return self.mode == self.EDIT
 
+    def set_auto_labeling(self, value=True):
+        """Set auto labeling mode"""
+        self.is_auto_labeling = value
+        if self.auto_labeling_mode is None:
+            self.auto_labeling_mode = AutoLabelingMode.get_default_mode()
+            self.parent.toggle_draw_mode(
+                False, self.auto_labeling_mode.shape_type
+            )
+        if not self.auto_labeling_mode:
+            self.auto_labeling_mode_changed.emit(None)
+        else:
+            self.auto_labeling_mode_changed.emit(self.auto_labeling_mode)
+
+    def get_mode(self):
+        """Get current mode"""
+        if self.is_auto_labeling:
+            return "Auto Labeling"
+        if self.mode == self.CREATE:
+            return "Drawing"
+        elif self.mode == self.EDIT:
+            return "Editing"
+        else:
+            return "Unknown"
+
     def set_editing(self, value=True):
         """Set editing mode. Editing is set to False, user is drawing"""
         self.mode = self.EDIT if value else self.CREATE
         if not value:  # Create
             self.un_highlight()
             self.deselect_shape()
 
@@ -824,21 +862,82 @@
             return True
         w, h = self.pixmap.width(), self.pixmap.height()
         return not (0 <= p.x() <= w - 1 and 0 <= p.y() <= h - 1)
 
     def finalise(self):
         """Finish drawing for a shape"""
         assert self.current
+        if self.is_auto_labeling:
+            self.current.label = self.auto_labeling_mode.edit_mode
         self.current.close()
         self.shapes.append(self.current)
         self.store_shapes()
         self.current = None
         self.set_hiding(False)
         self.new_shape.emit()
         self.update()
+        if self.is_auto_labeling:
+            self.update_auto_labeling_marks()
+
+    def update_auto_labeling_marks(self):
+        """Update the auto labeling marks"""
+        marks = []
+        for shape in self.shapes:
+            if shape.label == AutoLabelingMode.ADD:
+                if shape.shape_type == AutoLabelingMode.POINT:
+                    marks.append(
+                        {
+                            "type": "point",
+                            "data": [
+                                int(shape.points[0].x()),
+                                int(shape.points[0].y()),
+                            ],
+                            "label": 1,
+                        }
+                    )
+                elif shape.shape_type == AutoLabelingMode.RECTANGLE:
+                    marks.append(
+                        {
+                            "type": "rectangle",
+                            "data": [
+                                int(shape.points[0].x()),
+                                int(shape.points[0].y()),
+                                int(shape.points[1].x()),
+                                int(shape.points[1].y()),
+                            ],
+                            "label": 1,
+                        }
+                    )
+            elif shape.label == AutoLabelingMode.REMOVE:
+                if shape.shape_type == AutoLabelingMode.POINT:
+                    marks.append(
+                        {
+                            "type": "point",
+                            "data": [
+                                int(shape.points[0].x()),
+                                int(shape.points[0].y()),
+                            ],
+                            "label": 0,
+                        }
+                    )
+                elif shape.shape_type == AutoLabelingMode.RECTANGLE:
+                    marks.append(
+                        {
+                            "type": "rectangle",
+                            "data": [
+                                int(shape.points[0].x()),
+                                int(shape.points[0].y()),
+                                int(shape.points[1].x()),
+                                int(shape.points[1].y()),
+                            ],
+                            "label": 0,
+                        }
+                    )
+
+        self.auto_labeling_marks_updated.emit(marks)
 
     def close_enough(self, p1, p2):
         """Check if 2 points are close enough (by an threshold epsilon)"""
         # d = distance(p1 - p2)
         # m = (p1-p2).manhattanLength()
         # print "d %.2f, m %d, %.2f" % (d, m, d - m)
         # divide by scale to allow more precision when zoomed in
@@ -979,15 +1078,18 @@
                     self.shape_moved.emit()
 
                 self.moving_shape = False
 
     def set_last_label(self, text, flags):
         """Set label and flags for last shape"""
         assert text
-        self.shapes[-1].label = text
+        if self.is_auto_labeling:
+            self.shapes[-1].label = self.auto_labeling_mode.edit_mode
+        else:
+            self.shapes[-1].label = text
         self.shapes[-1].flags = flags
         self.shapes_backups.pop()
         self.store_shapes()
         return self.shapes[-1]
 
     def undo_last_line(self):
         """Undo last line"""
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/color_dialog.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/file_dialog_preview.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/label_dialog.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/label_list_widget.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,26 +91,24 @@
         return id(self)
 
     def __repr__(self):
         return f'{self.__class__.__name__}("{self.text()}")'
 
 
 class StandardItemModel(QtGui.QStandardItemModel):
-
     itemDropped = QtCore.pyqtSignal()
 
     # QT Overload
     def removeRows(self, *args, **kwargs):
         ret = super().removeRows(*args, **kwargs)
         self.itemDropped.emit()
         return ret
 
 
 class LabelListWidget(QtWidgets.QListView):
-
     item_double_clicked = QtCore.pyqtSignal(LabelListWidgetItem)
     item_selection_changed = QtCore.pyqtSignal(list, list)
 
     def __init__(self):
         super().__init__()
         self._selected_items = []
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/unique_label_qlist_widget.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import Qt
 
 from .escapable_qlist_widget import EscapableQListWidget
 
 
 class UniqueLabelQListWidget(EscapableQListWidget):
-
     # QT Overload
     def mousePressEvent(self, event):
         super().mousePressEvent(event)
         if not self.indexAt(event.pos()).isValid():
             self.clearSelection()
 
     def find_items_by_label(self, label):
```

### Comparing `anylabeling-0.0.1/anylabeling/views/labeling/labelme/widgets/zoom_widget.py` & `anylabeling-0.0.2/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 
 class ZoomWidget(QtWidgets.QSpinBox):
     def __init__(self, value=100):
         super().__init__()
         self.setButtonSymbols(QtWidgets.QAbstractSpinBox.NoButtons)
         self.setRange(1, 1000)
-        self.setSuffix(" %")
+        self.setSuffix("%")
         self.setValue(value)
         self.setToolTip("Zoom Level")
         self.setStatusTip(self.toolTip())
         self.setAlignment(QtCore.Qt.AlignCenter)
+        font = self.font()
+        font.setPointSize(9)
+        self.setFont(font)
 
     # QT Overload
     def minimumSizeHint(self):
         height = super().minimumSizeHint().height()
         font_metric = QtGui.QFontMetrics(self.font())
         width = font_metric.horizontalAdvance(str(self.maximum()))
         return QtCore.QSize(width, height)
```

### Comparing `anylabeling-0.0.1/anylabeling/views/maintabs.py` & `anylabeling-0.0.2/anylabeling/views/maintabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main tab widget for anylabeling app"""
 
 from PyQt5.QtWidgets import QTabWidget
 
-from .labeling.labeling_wrapper import LabelingWrapper
+from .labeling.label_wrapper import LabelingWrapper
 
 
 class MainTabsWidget(QTabWidget):
     """Main tab widget for anylabeling app"""
 
     def __init__(self, parent):
         super().__init__()
```

### Comparing `anylabeling-0.0.1/anylabeling/views/mainwindow.py` & `anylabeling-0.0.2/anylabeling/views/mainwindow_tabs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """This module defines the main application window"""
 
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QHBoxLayout, QLabel, QMainWindow, QStatusBar,
-                             QVBoxLayout, QWidget)
+from PyQt5.QtWidgets import (
+    QHBoxLayout,
+    QLabel,
+    QMainWindow,
+    QStatusBar,
+    QVBoxLayout,
+    QWidget,
+)
 
 from .maintabs import MainTabsWidget
 
 
 class MainWindow(QMainWindow):
     """Main application window"""
 
@@ -17,19 +23,19 @@
         self.setContentsMargins(0, 0, 0, 0)
         self.setWindowTitle("AnyLabeling")
 
         header_widget = QWidget(self)
         header_layout = QHBoxLayout(header_widget)
         program_title = QLabel("AnyLabeling - Effortless Labeling Tool")
         program_title.setStyleSheet(
-            "QLabel {background-color: #333; color: #fff; font: bold;}"
+            "QLabel {background-color: #ffffff; color: #333333; font: bold;}"
         )
         program_title.setFont(QFont("Arial", 16))
         header_layout.addWidget(program_title)
-        header_widget.setStyleSheet("background-color: #333;")
+        header_widget.setStyleSheet("background-color: #ffffff;")
 
         self.maintabs_widget = MainTabsWidget(self)
 
         main_layout = QVBoxLayout()
         main_layout.setContentsMargins(0, 0, 0, 0)
         main_layout.addWidget(header_widget)
         main_layout.addWidget(self.maintabs_widget)
```

### Comparing `anylabeling-0.0.1/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.0.2/anylabeling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.0.1
+Version: 0.0.2
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <h1 align="center">🌟 AnyLabeling 🌟</h1>
-  <p align="center">Effortless data labeling with AI support<p>
-  <p align="center">With <b>Improved Labelme</b> and <b>Segment Anything</b><p>
+  <p align="center">Effortless data labeling with AI support from <b>YOLO</b> and <b>Segment Anything</b>!<p>
+  <p align="center"><b>AnyLabeling = LabelImg + Labelme + Improved UI + Auto-labeling</b><p>
 </p>
 
 ![](https://i.imgur.com/waxVImv.png)
 
 
 ## I. Install and run
 
@@ -76,10 +78,9 @@
 
 ```
 python anylabeling/app.py
 ```
 
 ## III. References
 
-- labelme
-- gpu_util
+- Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

### Comparing `anylabeling-0.0.1/setup.py` & `anylabeling-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         "termcolor",
         "pyqtgraph",
         "pandas",
         "psutil",
         "opencv-python-headless",
         "imutils",
         'PyQt5>=5.15.7; platform_system != "Darwin"',
+        "onnx==1.13.1",
+        "onnxruntime==1.14.1",
+        "qimage2ndarray==1.10.0",
     ]
 
     if os.name == "nt":  # Windows
         install_requires.append("colorama")
 
     return install_requires
 
@@ -66,14 +69,16 @@
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "anylabeling=anylabeling.app:main",
         ],
```

