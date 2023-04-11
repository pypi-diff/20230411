# Comparing `tmp/ckanext-gallery-2.2.6.tar.gz` & `tmp/ckanext-gallery-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-gallery-2.2.6.tar", last modified: Mon Feb 20 10:48:05 2023, max compression
+gzip compressed data, was "ckanext-gallery-2.2.7.tar", last modified: Tue Apr 11 08:18:59 2023, max compression
```

## Comparing `ckanext-gallery-2.2.6.tar` & `ckanext-gallery-2.2.7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/gallery/
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/lib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/logic/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/logic/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/plugins/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/plugins/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/gallery/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/js/gallery.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/less/gallery.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.618216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    31748 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/blueimp-gallery.jquery.json
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.622216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-indicator.css
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-video.css
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.css
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/demo.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.622216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.png
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.622216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-indicator.js
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-video.js
--rw-r--r--   0 runner    (1001) docker     (123)    50419 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.js
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-helper.js
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/demo.js
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.js
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.626216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.626216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)   293430 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    35997 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   520715 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    30748 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   253670 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    17342 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/package.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/snippets/gallery.html
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/snippets/lightbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 10:48:05.000000 ckanext-gallery-2.2.6/ckanext_gallery.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.614215 ckanext-gallery-2.2.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 10:48:05.630216 ckanext-gallery-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-20 10:47:51.000000 ckanext-gallery-2.2.6/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/lib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/logic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/logic/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/plugins/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/plugins/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/js/gallery.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/less/gallery.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.575665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.583665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    31748 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/blueimp-gallery.jquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.583665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-indicator.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-video.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/demo.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.583665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.583665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-indicator.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-video.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50419 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-helper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/demo.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.587665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.587665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)   293430 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35997 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   520715 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30748 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   253670 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18705 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17342 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/package.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/snippets/gallery.html
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/snippets/lightbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:18:59.000000 ckanext-gallery-2.2.7/ckanext_gallery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.579665 ckanext-gallery-2.2.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:18:59.591665 ckanext-gallery-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-11 08:18:45.000000 ckanext-gallery-2.2.7/tests/test_validators.py
```

### Comparing `ckanext-gallery-2.2.6/LICENSE` & `ckanext-gallery-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/PKG-INFO` & `ckanext-gallery-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-gallery
-Version: 2.2.6
+Version: 2.2.7
 Summary: A CKAN extension for a dataset gallery view.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-gallery
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-gallery/blob/main/CHANGELOG.md
 Keywords: CKAN,data,gallery
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-gallery-2.2.6/README.md` & `ckanext-gallery-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/lib/helpers.py` & `ckanext-gallery-2.2.7/ckanext/gallery/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/logic/validators.py` & `ckanext-gallery-2.2.7/ckanext/gallery/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/plugins/gallery.py` & `ckanext-gallery-2.2.7/ckanext/gallery/plugins/gallery.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/plugins/image.py` & `ckanext-gallery-2.2.7/ckanext/gallery/plugins/image.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/plugins/interfaces.py` & `ckanext-gallery-2.2.7/ckanext/gallery/plugins/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/js/gallery.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/js/gallery.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/less/gallery.less` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/less/gallery.less`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/Makefile` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/Makefile`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/README.md` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/blueimp-gallery.jquery.json` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/blueimp-gallery.jquery.json`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/bower.json` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/bower.json`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-indicator.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-indicator.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-video.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery-video.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.min.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/blueimp-gallery.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/demo.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/css/demo.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/error.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/loading.gif` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/loading.gif`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/play-pause.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/img/video-play.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/index.html` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-fullscreen.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-fullscreen.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-indicator.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-indicator.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-video.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery-video.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.min.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-gallery.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-helper.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/blueimp-helper.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/demo.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/demo.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.min.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/js/jquery.blueimp-gallery.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/blueimp-gallery/package.json` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/blueimp-gallery/package.json`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/AUTHORS.txt` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/LICENSE.txt` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/index.html` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/package.json` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/vendor/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/assets/webassets.yml` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/form.html` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/form.html`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/snippets/gallery.html` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/snippets/gallery.html`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext/gallery/theme/templates/gallery/snippets/lightbox.html` & `ckanext-gallery-2.2.7/ckanext/gallery/theme/templates/gallery/snippets/lightbox.html`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/ckanext_gallery.egg-info/PKG-INFO` & `ckanext-gallery-2.2.7/ckanext_gallery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-gallery
-Version: 2.2.6
+Version: 2.2.7
 Summary: A CKAN extension for a dataset gallery view.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-gallery
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-gallery/blob/main/CHANGELOG.md
 Keywords: CKAN,data,gallery
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-gallery-2.2.6/ckanext_gallery.egg-info/SOURCES.txt` & `ckanext-gallery-2.2.7/ckanext_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/docs/_scripts/gen_api_pages.py` & `ckanext-gallery-2.2.7/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/pyproject.toml` & `ckanext-gallery-2.2.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-gallery"
-version = "2.2.6"
+version = "2.2.7"
 description = "A CKAN extension for a dataset gallery view."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.gallery.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.6"
+version = "2.2.7"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-gallery-2.2.6/tests/test_helpers.py` & `ckanext-gallery-2.2.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-gallery-2.2.6/tests/test_validators.py` & `ckanext-gallery-2.2.7/tests/test_validators.py`

 * *Files identical despite different names*

