# Comparing `tmp/Subsearch-2.33.3.tar.gz` & `tmp/Subsearch-2.33.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.33.3.tar", last modified: Wed Mar 15 22:28:12 2023, max compression
+gzip compressed data, was "Subsearch-2.33.4.tar", last modified: Tue Apr 11 17:14:02 2023, max compression
```

## Comparing `Subsearch-2.33.3.tar` & `Subsearch-2.33.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.886014 Subsearch-2.33.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-15 22:27:53.000000 Subsearch-2.33.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-15 22:27:53.000000 Subsearch-2.33.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-03-15 22:28:12.886014 Subsearch-2.33.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-03-15 22:27:53.000000 Subsearch-2.33.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-15 22:27:53.000000 Subsearch-2.33.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 22:28:12.886014 Subsearch-2.33.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-15 22:27:53.000000 Subsearch-2.33.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.862013 Subsearch-2.33.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 22:28:12.000000 Subsearch-2.33.3/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/application_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/set_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.870014 Subsearch-2.33.3/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.874014 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.874014 Subsearch-2.33.3/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.878014 Subsearch-2.33.3/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.878014 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.882014 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.882014 Subsearch-2.33.3/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.882014 Subsearch-2.33.3/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 22:28:12.886014 Subsearch-2.33.3/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-15 22:27:53.000000 Subsearch-2.33.3/src/subsearch/utils/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 17:13:46.000000 Subsearch-2.33.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 17:13:46.000000 Subsearch-2.33.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-11 17:14:02.893850 Subsearch-2.33.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-11 17:13:46.000000 Subsearch-2.33.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-11 17:13:46.000000 Subsearch-2.33.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:14:02.893850 Subsearch-2.33.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-11 17:13:46.000000 Subsearch-2.33.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.881850 Subsearch-2.33.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/application_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/updates.py
```

### Comparing `Subsearch-2.33.3/LICENSE` & `Subsearch-2.33.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/PKG-INFO` & `Subsearch-2.33.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.3
+Version: 2.33.4
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.3/README.md` & `Subsearch-2.33.4/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/pyproject.toml` & `Subsearch-2.33.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 include = ["subsearch*"]
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
-optional = ["black==23.1.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.7", "mypy==1.1.1", "pipreqs==0.4.11"]
-dev = ["pytest==7.2.2", "pytest-cov==4.0.0", "tox==4.4.7"]
+optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.9", "mypy==1.2.0", "pipreqs==0.4.11"]
+dev = ["pytest==7.3.0", "pytest-cov==4.0.0", "tox==4.4.11"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
@@ -64,8 +64,9 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 mypy_path = "src"
 ignore_missing_imports = true
-warn_no_return = false 
+warn_no_return = false
+check_untyped_defs = true
```

### Comparing `Subsearch-2.33.3/setup.py` & `Subsearch-2.33.4/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.33.4/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.3
+Version: 2.33.4
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.3/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.33.4/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/__init__.py` & `Subsearch-2.33.4/src/subsearch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,20 +62,14 @@
 
     def provider_yifysubtitles(self) -> None:
         """
         Search for subtitles on yifysubtitles
         """
         self._provider_yifysubtitles()
 
-    def provider_yifysubtitles(self) -> None:
-        """
-        Search for subtitles on yifysubtitles
-        """
-        self._provider_yifysubtitles()
-
     def process_files(self) -> None:
         """
         Download zip files containing the .srt files, extract, rename and clean up tmp files
         """
         self._download_files()
         self._not_downloaded()
         self._extract_zip_files()
```

### Comparing `Subsearch-2.33.3/src/subsearch/core.py` & `Subsearch-2.33.4/src/subsearch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
             log.output_header("Renaming best match")
             file_manager.rename_best_match(f"{self.release_data.release}.srt", video_data.directory_path, ".srt")
             log.output_done_with_tasks(end_new_line=True)
 
         log.output_header("Cleaning up")
         file_manager.clean_up_files(video_data.subs_directory, "nfo")
         file_manager.del_directory(video_data.tmp_directory)
+        if file_manager.directory_is_empty(video_data.subs_directory):
+            file_manager.del_directory(video_data.subs_directory)
         log.output_done_with_tasks(end_new_line=True)
 
     def _pre_exit(self) -> None:
         elapsed = time.perf_counter() - self.start
         log.output(f"Finished in {elapsed} seconds")
 
         if self.app_config.show_terminal is False:
```

### Comparing `Subsearch-2.33.3/src/subsearch/data/application_config.json` & `Subsearch-2.33.4/src/subsearch/data/application_config.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/data/data_objects.py` & `Subsearch-2.33.4/src/subsearch/data/data_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name: str
     alpha_1: str
     alpha_2b: str
     incompatibility: list[str]
 
 
 @dataclass(order=True)
-class ProviderAlphaCodeType:
+class ProviderAlphaCodeData:
     provider: str
     alpha_code: str
 
 
 @dataclass(order=True)
 class AppPaths:
     """
```

### Comparing `Subsearch-2.33.3/src/subsearch/data/languages.json` & `Subsearch-2.33.4/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/data/set_data.py` & `Subsearch-2.33.4/src/subsearch/data/set_data.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/__init__.py` & `Subsearch-2.33.4/src/subsearch/gui/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def init(func):
     def wrapper(*args, **kwargs):
         global inited
         global root
 
         if not inited:
-            from tkinter import _default_root
+            from tkinter import _default_root  # type: ignore
 
             path = (Path(__file__).parent / "assets" / "ttk_style.tcl").resolve()
 
             try:
                 _default_root.tk.call("source", str(path))
             except AttributeError:
                 raise RuntimeError(
@@ -31,29 +31,29 @@
 
 
 @init
 def set_theme(theme):
     if theme not in {"dark"}:
         raise RuntimeError(f"not a valid theme name: {theme}")
 
-    root.tk.call("set_theme", theme)
+    root.tk.call("set_theme", theme)  # type: ignore
 
 
 @init
 def get_theme():
-    theme = root.tk.call("ttk::style", "theme", "use")
+    theme = root.tk.call("ttk::style", "theme", "use")  # type: ignore
 
     try:
         return {"ttk_style": "dark"}[theme]
     except KeyError:
         return theme
 
 
 @init
-def toggle_theme():
+def toggle_theme() -> None:
     if get_theme() == "dark":
         use_dark_theme()
     else:
         use_dark_theme()
 
 
 use_dark_theme = lambda: set_theme("dark")
```

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.33.4/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.33.4/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tab_manager.py` & `Subsearch-2.33.4/src/subsearch/gui/tab_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,10 +183,10 @@
     """
     if io_winreg.registry_key_exists() is False and io_json.get_json_key("context_menu"):
         io_json.set_default_json()
         io_winreg.add_context_menu()
     root = tk.Tk(className=f"Subsearch")
     root.configure(background=GUI_DATA.colors.dark_grey)
     root.iconbitmap(app_paths.icon)
-    root.geometry(tkinter_utils.WindowPosition.set(root))
+    root.geometry(tkinter_utils.WindowPosition.set(root))  # type: ignore
     root.resizable(False, False)
     return root
```

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.33.4/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.33.4/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.33.4/src/subsearch/gui/tabs/search_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         if value.get() is True:
             self.data["subtitle_type"][key] = False
         elif value.get() is False:
             self.data["subtitle_type"][key] = True
         io_json.set_config(self.data)
         self.sub_type_txt()
 
-    def sub_type_txt(self):
+    def sub_type_txt(self) -> None:
         hi_sub = self.data["subtitle_type"]["hearing_impaired"]
         nonhi_sub = self.data["subtitle_type"]["non_hearing_impaired"]
         if (hi_sub and nonhi_sub) or (hi_sub is False and nonhi_sub is False):
             self.string_var.set(f"Both")
         if hi_sub and nonhi_sub is False:
             self.string_var.set(f"Only HI")
         if hi_sub is False and nonhi_sub:
@@ -204,15 +204,15 @@
 
     def release_slider(self, event) -> None:
         btn = event.widget
         if btn == self.slider:
             self.slider.configure(command=self.set_value)
             self.update_config()
 
-    def update_config(self):
+    def update_config(self) -> None:
         update_svar = self.current_value.get()
         io_json.set_config_key_value("percentage_threshold", update_svar)
         tkinter_utils.VarColorPicker(self.string_var, self.clabel, True)
 
 
 class RenameBestMatch(tkinter_utils.ToggleableFrameButton):
     """
```

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.33.4/src/subsearch/gui/tabs/settings_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             self.data["file_extensions"][key] = False
         elif value.get() is False:
             self.data["file_extensions"][key] = True
         io_json.set_config(self.data)
 
         self.update_registry()
 
-    def update_registry(self):
+    def update_registry(self) -> None:
         from subsearch.utils import io_winreg
 
         io_winreg.write_all_valuex()
 
 
 class ShowContextMenu(tkinter_utils.ToggleableFrameButton):
     """
```

### Comparing `Subsearch-2.33.3/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.33.4/src/subsearch/gui/tkinter_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             and vertically (hs_value_offset). If other=True, it allows changing other dimensions not typically
             touched (eg. height of frame/window title bar)
 
     Returns:
        None
     """
 
-    def __init__(self, parent):
+    def __init__(self, parent) -> None:
         """
         Constructor Method for WindowPosition Class
 
         Args:
             parent: The parent widget.
         """
         tk.Frame.__init__(self, parent)
@@ -217,15 +217,15 @@
 
     def __init__(self, string_var: StringVar, clabel: Label, is_pct: bool = False):
         self.string_var = string_var
         self.clabel = clabel
         self.is_pct = is_pct
         self.pick()
 
-    def pick(self):  # string boolean
+    def pick(self) -> None:
         if self.string_var.get() == "True":
             self.clabel.configure(fg=GUI_DATA.colors.green)
         elif self.string_var.get() == "False":
             self.clabel.configure(fg=GUI_DATA.colors.red)
         elif self.string_var.get() == "Both":
             self.clabel.configure(fg=GUI_DATA.colors.blue)
         elif self.string_var.get().startswith("Only"):
@@ -259,15 +259,15 @@
 
     def __init__(self, parent, _widget, *_text, _background=GUI_DATA.colors.light_black):
         self.parent = parent
         self.widget = _widget
         self.text = _text
         self.background = _background
 
-    def show(self):
+    def show(self) -> None:
         tk.Toplevel.__init__(self, self.parent)
         self.configure(background=GUI_DATA.colors.light_black)
         # remove the standard window titlebar from the tooltip
         self.overrideredirect(True)
         # unpack *args and put each /n on a new line
         lines = "\n".join(self.text)
         frame = tk.Frame(self, background=GUI_DATA.colors.light_black)
@@ -294,15 +294,15 @@
         frame.place(x=1, y=1, anchor="nw")
         label.place(x=0, y=0, anchor="nw")
         root_x = center_tip_over_mouse  # offset the tooltip by extra 4px so it doesn't overlap the widget
         root_y = self.widget.winfo_rooty() - self.widget.winfo_height() - 4
         # set position of the tooltip, size and add 2px around the tooltip for a 1px border
         self.geometry(f"{x+2}x{y+2}+{root_x}+{root_y}")
 
-    def hide(self):
+    def hide(self) -> None:
         self.destroy()
 
 
 class ToggleableFrameButton(tk.Frame):
     """
     A button that toggles a configuration setting on or off.
```

### Comparing `Subsearch-2.33.3/src/subsearch/providers/generic.py` & `Subsearch-2.33.4/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.33.4/src/subsearch/providers/opensubtitles.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class OpenSubtitlesScraper:
-    def __init__(self):
+    def __init__(self) -> None:
         ...
 
     def opensubtitles_down(self, tree: Any):
         is_offline = tree.css_matches("pre")
         if is_offline is False:
             return False
         offline_text = tree.css_first("pre").text()
```

### Comparing `Subsearch-2.33.3/src/subsearch/providers/subscene.py` & `Subsearch-2.33.4/src/subsearch/providers/subscene.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from subsearch.data.data_objects import DownloadMetaData, FormattedMetadata
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class SubsceneScraper:
-    def __init__(self):
+    def __init__(self) -> None:
         ...
 
-    def find_title(self, url: str, current_language: str, definitive_match: list[str]):
+    def find_title(self, url: str, current_language: str, definitive_match: list[str]) -> str | None:
         tree = generic.get_html_parser(url)
         products = tree.css("div.title")
         for item in products:
             node = item.css_first("a")
             result_href = node.attributes["href"]
             result_title = str(node.child.html).lower()
             if result_title not in definitive_match:
```

### Comparing `Subsearch-2.33.3/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.33.4/src/subsearch/providers/yifysubtitles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from subsearch.providers import generic
 from subsearch.providers.generic import ProviderParameters
 from subsearch.utils import log, string_parser
 
 
 class YifySubtitlesScraper:
-    def __init__(self):
+    def __init__(self) -> None:
         ...
 
     def skip_item(self, item: Node, hi_sub: bool, regular_sub: bool, current_language: str) -> bool:
         subtitle_language = item.css_first("span.sub-lang").child.text_content
         hearing_impaired = item.css_matches("span.hi-subtitle")
         if subtitle_language.lower() != current_language.lower():
             return True
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/exceptions.py` & `Subsearch-2.33.4/src/subsearch/utils/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
     pass
 
 
 class CaptchaError(ProviderError):
     """Error raised when a captcha challenge is encountered."""
 
-    def __init__(self, message="Captcha challenge encountered"):
+    def __init__(self, message: str = "Captcha challenge encountered"):
         super().__init__(message)
 
 
 class ProviderNotImplemented(ProviderError):
     """Error raised when using an unsupported subtitle provider."""
 
-    def __init__(self, message="This provider is not implemented"):
+    def __init__(self, message: str = "This provider is not implemented"):
         super().__init__(message)
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/file_manager.py` & `Subsearch-2.33.4/src/subsearch/utils/file_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,21 @@
     """
     for file in os.listdir(directory):
         log.output(f"Removing: {file}")
     log.output(f"Removing: {directory}")
     shutil.rmtree(directory)
 
 
-def make_necessary_directories():
+def directory_is_empty(directory: Path) -> bool:
+    if len(os.listdir(directory)) == 0:
+        return True
+    return False
+
+
+def make_necessary_directories() -> None:
     """
     Make necessary directories using video object info.
     """
 
     if video_data is None:
         return None
     if not Path(video_data.tmp_directory).exists():
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.33.4/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/utils/io_json.py` & `Subsearch-2.33.4/src/subsearch/utils/io_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
 from typing import Any, Union
 
 from subsearch.data import app_paths
-from subsearch.data.data_objects import AppConfig, LanguageData, ProviderAlphaCodeType
+from subsearch.data.data_objects import AppConfig, LanguageData, ProviderAlphaCodeData
 from subsearch.utils.exceptions import ProviderNotImplemented
 
 APPLICATION_CONFIG_JSON = Path(app_paths.data) / "application_config.json"
 LANGUAGES_JSON = Path(app_paths.data) / "languages.json"
 
 
 def get_json_data(json_file: Path = APPLICATION_CONFIG_JSON) -> Any:
@@ -146,40 +146,41 @@
     return language_data
 
 
 def get_available_languages() -> dict:
     return get_json_data(LANGUAGES_JSON)
 
 
-def get_provider_alpha_code_type(provider: str) -> ProviderAlphaCodeType:
+def get_provider_alpha_code_type(provider: str) -> ProviderAlphaCodeData:
     """
     Generates ProviderAlphaCodeType object containing provider and its associated alpha code.
 
     Args:
         provider (str): a string specifying the name of the provider
 
     Returns:
         ProviderAlphaCodeType: an instance of ProviderAlphaCodeType with the given provider and its associated alpha code_
     """
     providers = {"subscene": "name", "opensubtitles": "alpha_2b", "yifisubtitles": "name"}
     if provider not in providers:
         raise ProviderNotImplemented
-    return ProviderAlphaCodeType(provider, providers[provider])
+    return ProviderAlphaCodeData(provider, providers[provider])
 
 
 def get_alpha_code(alpha_code_type: str) -> str:
     language_data = get_language_data()
     return getattr(language_data, alpha_code_type)
 
 
 def get_provider_alpha_code(provider: str) -> str:
-    code_type = get_provider_alpha_code_type(provider)
-    return get_alpha_code(code_type)
+    data = get_provider_alpha_code_type(provider)
+    return get_alpha_code(data.alpha_code)
 
 
 def check_language_compatibility(provider: str, language: str = _current_language) -> bool:
     data = get_language_data(language)
     if not data.incompatibility:
         return True
 
     elif provider in data.incompatibility:
         return False
+    return False
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/io_winreg.py` & `Subsearch-2.33.4/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.3/src/subsearch/utils/log.py` & `Subsearch-2.33.4/src/subsearch/utils/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,34 +62,34 @@
         else:
             print(f"{level.upper()} - {msg}")
 
     _to_log(msg, level)
     _to_terminal(msg, terminal, level)
 
 
-def warning_spaces_in_filename():
+def warning_spaces_in_filename() -> None:
     name_unresolved = f"{video_data.filename}{video_data.file_extension}"
     output(f"File: '{name_unresolved}' contains spaces", level="warning")
     output(f"Results may vary, use punctuation marks for a more accurate result", level="info")
     output("")
 
 
-def output_header(msg: str):
+def output_header(msg: str) -> None:
     output(f"--- [{msg}] ---")
 
 
-def output_skip_provider(provider: str, reason: str):
+def output_skip_provider(provider: str, reason: str) -> None:
     output("")
     output_header(f"Skipping {provider}")
     output(f"{reason}")
     output("Done with tasks")
     output("")
 
 
-def output_done_with_tasks(end_new_line: bool = False):
+def output_done_with_tasks(end_new_line: bool = False) -> None:
     output("Done with tasks")
     if end_new_line:
         output("")
 
 
 def output_parameters() -> None:
     output_header(f"User data")
@@ -121,30 +121,30 @@
     output(f"opensubtitles_site:               {provider_urls.opensubtitles}")
     output(f"opensubtitles_hash:               {provider_urls.opensubtitles_hash}")
     output(f"yifysubtitles_site:               {provider_urls.yifysubtitles}")
 
     output("")
 
 
-def output_match(provider: str, pct_result: int, key: str, to_log_: bool = False):
+def output_match(provider: str, pct_result: int, key: str, to_log_: bool = False) -> None:
     if pct_result >= app_config.percentage_threshold:
         output(f"> {provider:<14}{pct_result:>3}% {key}", to_log=to_log_)
     else:
         output(f"  {provider:<14}{pct_result:>3}% {key}", to_log=to_log_)
 
 
-def set_logger_data(**kwargs):
+def set_logger_data(**kwargs) -> None:
     global release_data, app_config, provider_urls, language_data
     release_data = kwargs["release_data"]
     app_config = kwargs["app_config"]
     provider_urls = kwargs["provider_urls"]
     language_data = kwargs["language_data"]
 
 
-def downlod_metadata(provider_: str, formatted_metadata_: list[FormattedMetadata], search_threashold: int):
+def downlod_metadata(provider_: str, formatted_metadata_: list[FormattedMetadata], search_threashold: int) -> None:
     output("")
     output(f"--- [Sorted List from {provider_}] ---", False)
     downloaded_printed = False
     not_downloaded_printed = False
     for data in formatted_metadata_:
         if data.pct_result >= search_threashold and not downloaded_printed:
             output(f"--- Has been downloaded ---\n", False)
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/string_parser.py` & `Subsearch-2.33.4/src/subsearch/utils/string_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -135,26 +135,26 @@
         title = find_title_by_show(filename)
     else:
         title = filename.rsplit("-", 1)[0]
     return title
 
 
 class CreateProviderUrls:
-    def __init__(self, file_hash: str, app_config: AppConfig, release_metadata: ReleaseData, language_data: LanguageData):
+    def __init__(self, file_hash: str, app_config: AppConfig, release_data: ReleaseData, language_data: LanguageData):
         """
         Initializes a new instance of the CreateProviderUrls class.
 
         Args:
             file_hash (str): The file hash.
             app_config (AppConfig): The application configuration
             release_metadata (ReleaseMetadata): The release metadata
         """
         self.file_hash = file_hash
         self.app_config = app_config
-        self.release_metadata = release_metadata
+        self.release_data = release_data
         self.language_data = language_data
 
     def retrieve_urls(self) -> ProviderUrls:
         """
         Get the provider urls to search for subtitles.
 
         Returns:
@@ -201,30 +201,30 @@
     def yifysubtitles(self) -> str:
         """
         Gets the Url for the YifySubtitles website to search for subtitles for movies.
 
         Returns:
             str: The url to search for subtitles on yifysubtitles.org
         """
-        if self.release_metadata.tvseries:
+        if self.release_data.tvseries:
             return "N/A"
         domain = "https://yifysubtitles.org"
-        tt_id = imdb_lookup.FindImdbID(self.release_metadata.title, self.release_metadata.year).id
+        tt_id = imdb_lookup.FindImdbID(self.release_data.title, self.release_data.year).id
         return f"{domain}/movie-imdb/{tt_id}" if tt_id is not None else "N/A"
 
     def _subscene_search_parameters(self) -> str:
         """
         Gets the search parameters for Subscene to search for the appropriate subtitles based on File name and season ordinal.
 
         Returns:
             str: The search parameter value for Subscene to search for the applicable subtitles.
         """
-        if self.release_metadata.tvseries:
-            return f"{self.release_metadata.title} - {self.release_metadata.season_ordinal} season"
-        return f"{self.release_metadata.title}"
+        if self.release_data.tvseries:
+            return f"{self.release_data.title} - {self.release_data.season_ordinal} season"
+        return f"{self.release_data.title}"
 
     def _opensubtitles_subtitle_type(self) -> str:
         """
         Gets the subtitle type and language settings for Opensubtitles based on Application configuration.
 
         Returns:
             str: The subtitle types and language configurations to search for subtitles in Opensubtitles.
@@ -236,17 +236,17 @@
     def _opensubtitles_search_parameters(self) -> str:
         """
         Gets the search parameters for Opensubtitles to search for the appropriate subtitles based on Movie title, year, season and episode number.
 
         Returns:
             str: The search parameter value for Opensubtitles to search for the applicable subtitles.
         """
-        if self.release_metadata.tvseries:
-            return f"searchonlytvseries-on/season-{self.release_metadata.season}/episode-{self.release_metadata.episode}/moviename-{self.release_metadata.title}"
-        return f"searchonlymovies-on/moviename-{self.release_metadata.title} ({self.release_metadata.year})"
+        if self.release_data.tvseries:
+            return f"searchonlytvseries-on/season-{self.release_data.season}/episode-{self.release_data.episode}/moviename-{self.release_data.title}"
+        return f"searchonlymovies-on/moviename-{self.release_data.title} ({self.release_data.year})"
 
 
 def get_release_metadata(filename: str, file_hash: str) -> ReleaseData:
     """
     Collects the necessary metadata from a filename.
 
     Args:
```

### Comparing `Subsearch-2.33.3/src/subsearch/utils/updates.py` & `Subsearch-2.33.4/src/subsearch/utils/updates.py`

 * *Files identical despite different names*

