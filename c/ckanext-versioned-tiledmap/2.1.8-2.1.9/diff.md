# Comparing `tmp/ckanext-versioned-tiledmap-2.1.8.tar.gz` & `tmp/ckanext-versioned-tiledmap-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-versioned-tiledmap-2.1.8.tar", last modified: Tue Jan 31 13:52:53 2023, max compression
+gzip compressed data, was "ckanext-versioned-tiledmap-2.1.9.tar", last modified: Mon Feb 20 11:11:25 2023, max compression
```

## Comparing `ckanext-versioned-tiledmap-2.1.8.tar` & `ckanext-versioned-tiledmap-2.1.9.tar`

### file list

```diff
@@ -1,106 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/validators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/less/maps.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/map_view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/maptype_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/minimap_control.js
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.037971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/backbone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    59498 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.037971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)   248138 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js
--rw-r--r--   0 runner    (1001) docker     (123)    93869 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/
--rw-r--r--   0 runner    (1001) docker     (123)   215378 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)   125495 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.045971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/
--rw-r--r--   0 runner    (1001) docker     (123)    71140 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/terraformer/
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    39926 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.049971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/data/
--rw-r--r--   0 runner    (1001) docker     (123)   551530 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/data/countries.geojson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/toggle.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/map_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/map_view.html
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail.mustache
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail_hover.dwc.mustache
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail_hover.mustache
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 13:52:52.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 13:52:53.000000 ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.041971 ckanext-versioned-tiledmap-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 13:52:53.053971 ckanext-versioned-tiledmap-2.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-01-31 13:52:38.000000 ckanext-versioned-tiledmap-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/validators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/less/maps.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/map_view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/maptype_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/minimap_control.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/backbone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    59498 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.545980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   248138 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (123)    93869 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/
+-rw-r--r--   0 runner    (1001) docker     (123)   215378 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)   125495 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/
+-rw-r--r--   0 runner    (1001) docker     (123)    71140 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/terraformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39926 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.549980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   551530 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/data/countries.geojson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.minimap/toggle.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/map_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/map_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail_hover.dwc.mustache
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail_hover.mustache
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 11:11:25.000000 ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.541980 ckanext-versioned-tiledmap-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 11:11:25.553980 ckanext-versioned-tiledmap-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/tests/test_route_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-02-20 11:11:14.000000 ckanext-versioned-tiledmap-2.1.9/tests/test_validators.py
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/LICENSE` & `ckanext-versioned-tiledmap-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/PKG-INFO` & `ckanext-versioned-tiledmap-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-tiledmap
-Version: 2.1.8
+Version: 2.1.9
 Summary: A CKAN extension with a map view for versioned-datastore backed resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_tiledmap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/README.md` & `ckanext-versioned-tiledmap-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/config.py` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/lib/validators.py` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/lib/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/plugin.py` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/_helpers.py` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/routes/map.py` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/routes/map.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/less/maps.less` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/less/maps.less`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 body {
   margin: 0;
 }
 
 div.tiled-map {
   font-size: 13px;
-  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
+  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
   line-height: 18px;
   color: #333;
 
   & a {
     color: #363636;
     text-decoration: none;
 
@@ -26,29 +26,28 @@
       margin: 1px 0 0 1px;
       display: inline-block;
       font-size: 14px;
       line-height: 16px;
     }
 
     &.leaflet-draw-edit-remove:after {
-      content: "\f0e2";
+      content: '\f0e2';
     }
 
     &.leaflet-draw-draw-country:after {
-      content: "\f0ac" /* Puzzle piece - fa-puzzle-piece */
+      content: '\f0ac'; /* Puzzle piece - fa-puzzle-piece */
     }
 
     &.leaflet-draw-edit-remove,
     &.leaflet-draw-draw-country {
       background-image: none !important;
     }
   }
 }
 
-
 div.tiled-map-info {
   padding: 12px;
 }
 
 .info {
   color: #555;
   padding: 6px 8px;
@@ -68,15 +67,15 @@
   box-shadow: 0 0 15px rgba(0, 0, 0, 0.7);
   border-radius: 10px;
   width: 300px;
   min-height: 2em;
 }
 
 .leaflet-container {
-  background: #CBE6FE;
+  background: #cbe6fe;
 }
 
 .leaflet-bar a {
   &.active-selection {
     font-weight: bold;
     background: #f4f4f4;
   }
@@ -100,15 +99,15 @@
 }
 
 .panel.sidebar {
   float: right;
   width: 0px; /* Set to max-width when displayed */
   max-width: 230px;
   height: 500px; /* Set to 90% of screen height when displayed */
-  background: #EEE;
+  background: #eee;
   overflow-y: hidden; /* Set to 'auto' when displayed */
   overflow-x: hidden;
   position: relative;
 }
 
 div.tiled-map-point-detail,
 div.point-detail {
@@ -147,15 +146,16 @@
     }
 
     & td {
       word-wrap: break-word;
       overflow-wrap: break-word;
     }
 
-    & td, & th {
+    & td,
+    & th {
       text-align: left;
       vertical-align: top;
     }
   }
 
   & .point-detail-tree-label {
     color: #666;
@@ -177,15 +177,15 @@
   overflow-y: auto;
   height: 100%;
 }
 
 div.point-detail-info {
   font-size: 0.9em;
   color: #666;
-  background: #E4E4E4;
+  background: #e4e4e4;
   text-align: center;
   min-width: 210px;
   padding: 10px;
 
   & a:hover {
     text-decoration: underline;
   }
@@ -203,15 +203,15 @@
   right: 8px;
   color: #000000;
   cursor: pointer;
 }
 
 /* Map tooltips */
 div.map-hover-tooltip {
-  color: #FFF;
+  color: #fff;
   background: #000;
   font-size: 1em;
   padding: 3px 5px;
   border-radius: 2px;
   opacity: 0.7;
 }
 
@@ -223,15 +223,15 @@
 
   & div.tiled-map {
     width: 98%;
     margin-left: 1%;
   }
 
   & .fa-expand:before {
-    content: "\f066";
+    content: '\f066';
   }
 
   & .panel.sidebar {
     max-width: 400px;
   }
 
   & div.point-detail-info {
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/ckanfilterurl.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
             this.qs = {};
             if (parts.length > 1) {
                 var qs_idx = parts[1].split('&');
                 for (var i in qs_idx) {
                     var p = qs_idx[i].split('=');
                     p[0] = decodeURIComponent(p[0]);
                     p[1] = decodeURIComponent(p[1]);
-                    this.qs[p[0]] = p[1]
+                    this.qs[p[0]] = p[1];
                 }
                 if (typeof this.qs['filters'] !== 'undefined') {
                     this.set_filters(this.qs['filters']);
                 }
             }
 
             return this;
@@ -93,20 +93,20 @@
         this.set_filters = function(filters) {
             delete this.qs['filters'];
             if (typeof filters === 'string' && filters) {
                 var split = filters.split('|');
                 for (var i in split) {
                     var parts = split[i].split(':');
                     if (parts.length === 2) {
-                        this.set_filter(parts[0], parts[1])
+                        this.set_filter(parts[0], parts[1]);
                     }
                 }
             } else if (typeof filters === 'object') {
                 for (var i in filters) {
-                    this.set_filter(i, filters[i])
+                    this.set_filter(i, filters[i]);
                 }
             }
             return this;
         };
 
         /**
          * Returns the filter query string alone (not encoded)
@@ -117,15 +117,15 @@
             }
             var b_filter = [];
             for (var f in this.qs['filters']) {
                 for (var i = 0; i < this.qs['filters'][f].length; i++) {
                     b_filter.push(f + ':' + this.qs['filters'][f][i]);
                 }
             }
-            return b_filter.join('|')
+            return b_filter.join('|');
         };
 
         /**
          * Return the values (as an array) of a single filter in the filter query string
          */
         this.get_filter = function(name) {
             if (!this.qs['filters'] || !this.qs['filters'][name]) {
@@ -149,9 +149,9 @@
                 b_qs.push(encodeURIComponent(i) + '=' + encodeURIComponent(val));
             }
 
             return this.base + '?' + b_qs.join('&');
         };
 
         this.initialize();
-    }
+    };
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/drawshape_control.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
             $.ajax('/data/countries.geojson', {
                 dataType: 'json',
                 error: function(xhr, status, error) {
                     console.log('failed to load countries');
                 },
                 success: $.proxy(function(data, status, xhr) {
                     this.countries = data;
-                }, this)
+                }, this),
             });
         },
 
         /**
          * Plugin hook called when adding layers to a map.
          */
         layers: function() {
@@ -80,54 +80,54 @@
                     return {
                         stroke: true,
                         color: '#000',
                         opacity: 1,
                         weight: 1,
                         fill: true,
                         fillColor: '#FFF',
-                        fillOpacity: 0.25
+                        fillOpacity: 0.25,
                     };
                 },
                 onEachFeature: function(feature, layer) {
                     layer.on({
                         mouseover: function(e) {
                             layer.setStyle({
                                 stroke: true,
                                 color: '#000',
                                 opacity: 1,
                                 weight: 1,
                                 fill: true,
                                 fillColor: '#54F',
-                                fillOpacity: 0.75
+                                fillOpacity: 0.75,
                             });
                         },
                         mouseout: function(e) {
                             layer.setStyle({
                                 stroke: true,
                                 color: '#000',
                                 opacity: 1,
                                 weight: 1,
                                 fill: true,
                                 fillColor: '#FFF',
-                                fillOpacity: 0.25
+                                fillOpacity: 0.25,
                             });
                         },
                         click: function(e) {
                             self.view.map.fire('draw:created', {
                                 layer: layer,
-                                layerType: 'country'
+                                layerType: 'country',
                             });
                             self._disactivate();
-                        }
-                    })
-                }
+                        },
+                    });
+                },
             });
             return [{
-                'name': 'countries',
-                'layer': l
+                name: 'countries',
+                layer: l
             }];
         },
 
         _activate: function() {
             // Add the layer
             var l = this.layers();
             this.view._addLayer('countries', l[0].layer, true);
@@ -135,15 +135,15 @@
             var action_inner = $('<a>')
                 .attr('href', '#')
                 .html('Cancel')
                 .click($.proxy(this, 'onCountrySelectionClick'));
             this.action = $('<li>').append(action_inner);
             $('ul.leaflet-draw-actions').empty().append(this.action).css({
                 display: 'block',
-                top: '52px'
+                top: '52px',
             });
             // Ensure plugins can react to this
             this.view.map.fireEvent('draw:drawstart', {
                 layerType: 'country'
             });
         },
 
@@ -151,23 +151,23 @@
             // Remove layer
             this.view._removeLayer('countries', true);
             // Hide actions
             this.action.remove();
             $('ul.leaflet-draw-actions').css('display', 'none');
             // Ensure plugins can react to this
             this.view.map.fireEvent('draw:drawstop', {
-                'layerType': 'country'
+                layerType: 'country'
             });
         },
 
         onCountrySelectionClick: function(e) {
             this.active = !this.active;
             if (this.active) {
                 this._activate();
             } else {
                 this._disactivate();
             }
             e.stopPropagation();
             return false;
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/fullscreen_control.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -56,19 +56,24 @@
                 return false;
             }, this);
         },
 
         onAdd: function(map) {
             var body = jQuery('body').get(0);
             this.$bar = $('<div>').addClass('leaflet-bar');
-            if (body.requestFullscreen ||
-                body.mozRequestFullScreen || body.webkitRequestFullscreen) {
-                $('<a></a>').attr('href', '#').attr('title', 'full screen')
-                    .html('<i class="fa fa-expand"></i>').appendTo(this.$bar)
+            if (
+                body.requestFullscreen ||
+                body.mozRequestFullScreen ||
+                body.webkitRequestFullscreen
+            ) {
+                $('<a></a>')
+                    .attr('href', '#')
+                    .attr('title', 'full screen')
+                    .html('<i class="fa fa-expand"></i>')
+                    .appendTo(this.$bar)
                     .click($.proxy(this, '_onClick'));
             }
 
             return L.DomUtil.get(this.$bar.get(0));
-
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/map_view.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/map_view.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -41,34 +41,37 @@
             var out = Mustache.render(this.template);
             this.el.html(out);
             this.$map = this.el.find('.panel.map');
             // Add close button handler
             this.el.find('.close').click(this.closeSidebar);
             $('.panel.sidebar', this.el).append(this.sidebar_view.el);
             this.map_ready = false;
-            this._fetchMapInfo($.proxy(function(info) {
-                this.map_info = info;
-                this.map_info.draw = true;
-                this.map_ready = true;
-                this._setupMap();
-                this.redraw();
-                if (this.visible) {
-                    this.show()
-                }
-            }, this), $.proxy(function(message) {
-                this.map_info = {
-                    draw: false,
-                    error: message
-                };
-                // The map _is_ ready, even if all it displays is an error message.
-                this.map_ready = true;
-                if (this.visible) {
-                    this.show();
-                }
-            }, this));
+            this._fetchMapInfo(
+                $.proxy(function(info) {
+                    this.map_info = info;
+                    this.map_info.draw = true;
+                    this.map_ready = true;
+                    this._setupMap();
+                    this.redraw();
+                    if (this.visible) {
+                        this.show();
+                    }
+                }, this),
+                $.proxy(function(message) {
+                    this.map_info = {
+                        draw: false,
+                        error: message,
+                    };
+                    // The map _is_ ready, even if all it displays is an error message.
+                    this.map_ready = true;
+                    if (this.visible) {
+                        this.show();
+                    }
+                }, this),
+            );
         },
 
         /**
          * Show the map
          *
          * Called when the map visulisation is selected.
          */
@@ -102,54 +105,66 @@
          */
         updateRecordCounter: function() {
             var $rri = $('.tiled-map-info', this.el);
             var template = [
                 'Displaying <span class="doc-count">{{geoRecordCount}}</span>',
                 ' of ',
                 '</span><span class="doc-count">{{recordCount}}</span>',
-                'records'
+                'records',
             ].join(' ');
-            $rri.html(Mustache.render(template, {
-                recordCount: this.map_info.total_count ? this.map_info.total_count.toString() : '0',
-                geoRecordCount: this.map_info.geom_count ? this.map_info.geom_count.toString() : '0'
-            }));
+            $rri.html(
+                Mustache.render(template, {
+                    recordCount: this.map_info.total_count ?
+                        this.map_info.total_count.toString() :
+                        '0',
+                    geoRecordCount: this.map_info.geom_count ?
+                        this.map_info.geom_count.toString() :
+                        '0',
+                }),
+            );
         },
 
         /**
          * Hide the map.
          *
          * This is called when the grid or graph views are selected.
          */
         hide: function() {
             this.el.css('display', 'none');
-            this.visible = false
+            this.visible = false;
         },
 
         /**
          * Called when the window is resized to set the map size
          */
         _resize: function() {
             if (this.controls && this.controls['fullScreen'].is_full_screen) {
-                $('div.panel.map, div.panel.sidebar', this.el).height($(window.parent).height() * 0.90);
+                $('div.panel.map, div.panel.sidebar', this.el).height(
+                    $(window.parent).height() * 0.9,
+                );
             } else {
-                $('div.panel.map, div.panel.sidebar', this.el).height($(window.parent).height() * 0.75);
+                $('div.panel.map, div.panel.sidebar', this.el).height(
+                    $(window.parent).height() * 0.75,
+                );
             }
             if (this.map) {
                 this.map.invalidateSize();
             }
         },
 
         /**
          * Called when on popstate. Restore the previous __geo__ filter.
          */
         _popstate: function(e) {
             if (e.originalEvent.state && e.originalEvent.state.geom) {
                 this.setGeom(e.originalEvent.state.geom, true);
             } else {
-                var geom_t = new my.CkanFilterUrl(window.parent.location.href).get_filter('__geo__');
+                var geom_t = new my.CkanFilterUrl(
+                    window.parent.location.href,
+                ).get_filter('__geo__');
                 var geom = null;
                 if (geom_t.length > 0) {
                     // TODO: We don't support multi-value filters.
                     geom = JSON.parse(geom_t[0]);
                 }
                 this.setGeom(geom, true);
             }
@@ -167,51 +182,76 @@
             if (typeof this.map !== 'undefined') {
                 bounds = this.map.getBounds();
                 this.disablePlugins();
                 this.map.remove();
             }
             /* Fix map jump issue, see: https://github.com/Leaflet/Leaflet/issues/1228 */
             L.Map.addInitHook(function() {
-                return L.DomEvent.off(this._container, "mousedown", this.keyboard._onMouseDown);
+                return L.DomEvent.off(
+                    this._container,
+                    'mousedown',
+                    this.keyboard._onMouseDown,
+                );
             });
             this.map = new L.Map(this.$map.get(0), {
                 worldCopyJump: true,
                 trackResize: false,
                 minZoom: this.map_info.zoom_bounds.min,
-                maxZoom: this.map_info.zoom_bounds.max
+                maxZoom: this.map_info.zoom_bounds.max,
             });
             if (this.map_info.geom_count > 0 || !bounds) {
                 bounds = this.map_info.bounds;
             }
             this.map.fitBounds(this.map_info.bounds, {
                 animate: false,
-                maxZoom: this.map_info.initial_zoom.max
+                maxZoom: this.map_info.initial_zoom.max,
             });
             if (this.map.getZoom() < this.map_info.initial_zoom.min) {
                 var center = this.map.getCenter();
-                this.map.setView(center, this.map_info.initial_zoom.min)
+                this.map.setView(center, this.map_info.initial_zoom.min);
             }
             L.tileLayer(this.map_info.tile_layer.url, {
                 opacity: this.map_info.tile_layer.opacity,
-                noWrap: !this.map_info.repeat_map
+                noWrap: !this.map_info.repeat_map,
             }).addTo(this.map);
 
             // Set up the controls available to the map. These are assigned during redraw.
             this.controls = {
-                'drawShape': new my.DrawShapeControl(this, this.map_info.control_options['drawShape']),
-                'mapType': new my.MapTypeControl(this, this.map_info.control_options['mapType']),
-                'fullScreen': new my.FullScreenControl(this, this.map_info.control_options['fullScreen']),
-                'miniMap': new my.MiniMapControl(this, this.map_info.control_options['miniMap'])
+                drawShape: new my.DrawShapeControl(
+                    this,
+                    this.map_info.control_options['drawShape'],
+                ),
+                mapType: new my.MapTypeControl(
+                    this,
+                    this.map_info.control_options['mapType'],
+                ),
+                fullScreen: new my.FullScreenControl(
+                    this,
+                    this.map_info.control_options['fullScreen'],
+                ),
+                miniMap: new my.MiniMapControl(
+                    this,
+                    this.map_info.control_options['miniMap'],
+                ),
             };
 
             // Set up the plugins available to the map. These are assigned during redraw.
             this.plugins = {
-                'tooltipInfo': new my.TooltipPlugin(this, this.map_info.plugin_options['tooltipInfo']),
-                'tooltipCount': new my.TooltipPlugin(this, this.map_info.plugin_options['tooltipCount']),
-                'pointInfo': new my.PointInfoPlugin(this, this.map_info.plugin_options['pointInfo'])
+                tooltipInfo: new my.TooltipPlugin(
+                    this,
+                    this.map_info.plugin_options['tooltipInfo'],
+                ),
+                tooltipCount: new my.TooltipPlugin(
+                    this,
+                    this.map_info.plugin_options['tooltipCount'],
+                ),
+                pointInfo: new my.PointInfoPlugin(
+                    this,
+                    this.map_info.plugin_options['pointInfo'],
+                ),
             };
 
             // Setup handling of draw events to ensure plugins work nicely together
             this.map.on('draw:created', function(e) {
                 self.setGeom(e.layer.toGeoJSON().geometry);
             });
             this.map.on('draw:drawstart', function(e) {
@@ -233,20 +273,20 @@
          */
         _fetchMapInfo: function(callback, error_cb) {
             this.fetch_count++;
 
             var params = {
                 resource_id: this.resource_id,
                 view_id: this.view_id,
-                fetch_id: this.fetch_count
+                fetch_id: this.fetch_count,
             };
 
             var filters = new my.CkanFilterUrl().set_filters(this.filters.fields);
             if (this.filters.geom) {
-                filters.set_filter('__geo__', JSON.stringify(this.filters.geom))
+                filters.set_filter('__geo__', JSON.stringify(this.filters.geom));
             }
             params['filters'] = filters.get_filters();
 
             if (this.filters.q) {
                 params['q'] = this.filters.q;
             }
 
@@ -261,46 +301,49 @@
                 success: $.proxy(function(data, status, jqXHR) {
                     this.jqxhr = null;
                     // Ensure this is the result we want, not a previous query!
                     if (data.fetch_id === this.fetch_count) {
                         if (typeof data.geospatial !== 'undefined' && data.geospatial) {
                             callback(data);
                         } else {
-                            error_cb("This data does not have geospatial information");
+                            error_cb('This data does not have geospatial information');
                         }
                     }
                 }, this),
                 error: function(jqXHR, status, error) {
                     if (status !== 'abort') {
-                        error_cb("Error while loading the map");
+                        error_cb('Error while loading the map');
                     }
-                }
+                },
             });
         },
 
         /**
          * Reload the number of records. Called when filters change without a page reload.
          */
         _refreshInfo: function() {
             var $rri = $('.tiled-map-info', this.el);
             $rri.html('Loading...');
-            this._fetchMapInfo($.proxy(function(info) {
-                // cache the currently selected map style
-                var currentMapStyle = this.map_info.map_style;
-                // update the map_info property with the new data
-                this.map_info = info;
-                // and then write the current selection back into the object
-                this.map_info.map_style = currentMapStyle;
-                this.map_info.draw = true;
-                this.updateRecordCounter();
-                // and redraw the map
-                this.redraw();
-            }, this), function() {
-                /* NO OP */
-            });
+            this._fetchMapInfo(
+                $.proxy(function(info) {
+                    // cache the currently selected map style
+                    var currentMapStyle = this.map_info.map_style;
+                    // update the map_info property with the new data
+                    this.map_info = info;
+                    // and then write the current selection back into the object
+                    this.map_info.map_style = currentMapStyle;
+                    this.map_info.draw = true;
+                    this.updateRecordCounter();
+                    // and redraw the map
+                    this.redraw();
+                }, this),
+                function() {
+                    /* NO OP */
+                },
+            );
         },
 
         /**
          * Set the geom filter. This will cause the map to be redrawn and links to views to be
          * updated. If leave_window_url if false or undefined, this will also update the browser url
          * (or reload the page in older browsers).
          */
@@ -311,21 +354,28 @@
             }
             this.filters.geom = geom;
             // Inject the geom search term in links to all other views.
             var param = null;
             if (this.filters.geom) {
                 param = JSON.stringify(this.filters.geom);
             }
-            $('section.module ul.view-list li.resource-view-item a', window.parent.document).each(function() {
-                var href = new my.CkanFilterUrl($(this).attr('href')).set_filter('__geo__', param).get_url();
+            $(
+                'section.module ul.view-list li.resource-view-item a',
+                window.parent.document,
+            ).each(function() {
+                var href = new my.CkanFilterUrl($(this).attr('href'))
+                    .set_filter('__geo__', param)
+                    .get_url();
                 $(this).attr('href', href);
             });
             // Inject the geom search in the browser URL.
             if (!leave_window_url) {
-                var href = new my.CkanFilterUrl(window.parent.location.href).set_filter('__geo__', param).get_url();
+                var href = new my.CkanFilterUrl(window.parent.location.href)
+                    .set_filter('__geo__', param)
+                    .get_url();
                 if (window.parent.history.pushState) {
                     window.parent.history.pushState({
                         geom: geom
                     }, '', href);
                 } else {
                     window.parent.location = href;
                 }
@@ -362,31 +412,37 @@
             for (var i in this.layers) {
                 this.map.removeLayer(this.layers[i]);
             }
             this._removeAllLayers();
             if (this.filters.geom) {
                 this._addLayer('selection', L.geoJson(this.filters.geom));
             }
-            this._addLayer('plot', L.tileLayer(tile_url, {
-                noWrap: !this.map_info.repeat_map
-            }));
+            this._addLayer(
+                'plot',
+                L.tileLayer(tile_url, {
+                    noWrap: !this.map_info.repeat_map,
+                }),
+            );
 
             if (style.has_grid) {
                 var grid_params = $.extend({}, params);
                 if (style.grid_source.params) {
                     grid_params = $.extend(grid_params, style.grid_source.params);
                 }
                 var grid_url = style.grid_source.url + '?' + $.param(grid_params);
 
-                this._addLayer('grid', new L.UtfGrid(grid_url, {
-                    resolution: style.grid_resolution,
-                    useJsonP: false,
-                    maxRequests: 4,
-                    pointerCursor: false
-                }));
+                this._addLayer(
+                    'grid',
+                    new L.UtfGrid(grid_url, {
+                        resolution: style.grid_resolution,
+                        useJsonP: false,
+                        maxRequests: 4,
+                        pointerCursor: false,
+                    }),
+                );
             }
             // Ensure that click events on the selection get passed to the map.
             if (typeof this.layers['selection'] !== 'undefined') {
                 this.layers['selection'].on('click', function(e) {
                     self.map.fire('click', e);
                 });
             }
@@ -408,51 +464,51 @@
          */
         openSidebar: function(x, y) {
             var $sb = $('.panel.sidebar', this.el);
             var width = $sb.css('max-width');
             var base_duration = 200;
             if ($sb.width() < parseInt(width)) {
                 var distance = this.el.width() - x;
-                if (distance < (parseInt(width) + 50)) {
+                if (distance < parseInt(width) + 50) {
                     var diff = parseInt(width) + 50 - distance;
-                    var pan_duration = (base_duration * diff / parseInt(width)) / 1000.0;
+                    var pan_duration = (base_duration * diff) / parseInt(width) / 1000.0;
                     this.map.panBy([diff, 0], {
                         duration: pan_duration,
-                        easeLinearity: 1.0
+                        easeLinearity: 1.0,
                     });
                 }
             }
             $sb.stop().animate({
-                width: width
+                width: width,
             }, {
                 duration: base_duration,
-                easing: 'linear'
-            });
+                easing: 'linear',
+            }, );
         },
 
         /**
          * Close the sidebar
          */
         closeSidebar: function() {
             var $sb = $('.panel.sidebar', this.el);
             $sb.stop().animate({
-                width: 0
+                width: 0,
             }, {
                 complete: function() {
                     $sb.css('overflow-y', 'hidden');
-                }
-            });
+                },
+            }, );
         },
 
         /**
          * This function adds a new layer to the map
          */
         _addLayer: function(name, layer) {
             if (typeof this.layers[name] !== 'undefined') {
-                this.map.removeLayer(this.layers[name])
+                this.map.removeLayer(this.layers[name]);
             }
             this.layers[name] = layer;
             this.map.addLayer(layer);
         },
 
         /**
          * This function removes a layer from the map
@@ -474,30 +530,38 @@
             this.layers = {};
         },
 
         /**
          * Updates the controls used on the map for the current style
          */
         updateControls: function() {
-            this._updateAddons('controls', $.proxy(function(control) {
-                this.map.addControl(this.controls[control]);
-            }, this), $.proxy(function(control) {
-                this.map.removeControl(this.controls[control]);
-            }, this));
+            this._updateAddons(
+                'controls',
+                $.proxy(function(control) {
+                    this.map.addControl(this.controls[control]);
+                }, this),
+                $.proxy(function(control) {
+                    this.map.removeControl(this.controls[control]);
+                }, this),
+            );
         },
 
         /**
          * Updates the plugins used on this map
          */
         updatePlugins: function() {
-            this._updateAddons('plugins', $.proxy(function(plugin) {
-                this.plugins[plugin].enable();
-            }, this), $.proxy(function(plugin) {
-                this.plugins[plugin].disable();
-            }, this));
+            this._updateAddons(
+                'plugins',
+                $.proxy(function(plugin) {
+                    this.plugins[plugin].enable();
+                }, this),
+                $.proxy(function(plugin) {
+                    this.plugins[plugin].disable();
+                }, this),
+            );
         },
 
         /**
          * Disable all plugins
          */
         disablePlugins: function() {
             if (typeof this._current_addons === 'undefined') {
@@ -518,15 +582,15 @@
          */
         invoke: function(hook, args) {
             var ret = [];
             for (var p in this._current_addons) {
                 for (var i in this._current_addons[p]) {
                     var addon = this[p][this._current_addons[p][i]];
                     if (typeof addon[hook] == 'function') {
-                        var lr = addon[hook](args)
+                        var lr = addon[hook](args);
                         if ($.isArray(lr)) {
                             ret = ret.concat(lr);
                         } else if (typeof lr !== 'undefined') {
                             ret.push(lr);
                         }
                     }
                 }
@@ -560,10 +624,10 @@
             for (var i in this._current_addons[type]) {
                 var addon = this._current_addons[type][i];
                 if (remove_cb && $.inArray(addon, new_addons) === -1) {
                     remove_cb(addon);
                 }
             }
             this._current_addons[type] = new_addons;
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/maptype_control.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/maptype_control.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -34,14 +34,14 @@
                     .attr('href', '#')
                     .attr('title', title)
                     .html(icon)
                     .attr('stylecontrol', style)
                     .appendTo(this.$bar)
                     .click(this.getItemClickHandler(style));
                 if (style === this.view.map_info.map_style) {
-                    $elem.addClass('active-selection')
+                    $elem.addClass('active-selection');
                 }
             }
             return L.DomUtil.get(this.$bar.get(0));
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/minimap_control.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/minimap_control.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -14,23 +14,30 @@
             };
             options.shadowRectOptions = {
                 stroke: false,
                 fill: false
             };
             self._viewport_type = 'none';
             self._tile_layer = L.tileLayer(options.tile_layer.url);
-            L.Control.MiniMap.prototype.initialize.call(self, self._tile_layer, options);
+            L.Control.MiniMap.prototype.initialize.call(
+                self,
+                self._tile_layer,
+                options,
+            );
         },
 
         onAdd: function(map) {
             var pret = L.Control.MiniMap.prototype.onAdd.call(self, map);
             self._map = map;
             self._viewports = {
-                'rect': L.rectangle(self._map.getBounds(), self.options.viewport.rect),
-                'marker': new L.CircleMarker(self._map.getCenter(), self.options.viewport.marker)
+                rect: L.rectangle(self._map.getBounds(), self.options.viewport.rect),
+                marker: new L.CircleMarker(
+                    self._map.getCenter(),
+                    self.options.viewport.marker,
+                ),
             };
             self._miniMap.whenReady(function() {
                 self.updateViewport();
                 self._miniMap.on('move', self.updateViewport);
                 self._map.on('move', self.updateViewport);
                 self._setDisplay(self._decideMinimized());
             });
@@ -46,26 +53,26 @@
                     viewport_type = 'marker';
                 } else {
                     viewport_type = 'rect';
                 }
             }
             // Add the viewport to the minimap if needed
             if (viewport_type !== self._viewport_type) {
-                if (typeof(self._viewports[self._viewport_type]) !== 'undefined') {
+                if (typeof self._viewports[self._viewport_type] !== 'undefined') {
                     self._miniMap.removeLayer(self._viewports[self._viewport_type]);
                 }
-                if (typeof(self._viewports[viewport_type]) !== 'undefined') {
+                if (typeof self._viewports[viewport_type] !== 'undefined') {
                     self._viewports[viewport_type].addTo(self._miniMap);
                 }
                 self._viewport_type = viewport_type;
             }
             // Update bounds/position of viewport
             if (self._viewport_type === 'rect') {
                 self._viewports['rect'].setBounds(self._map.getBounds());
                 self._viewports['rect'].redraw();
             } else if (self._viewport_type === 'marker') {
                 self._viewports['marker'].setLatLng(self._map.getCenter());
                 self._viewports['marker'].redraw();
             }
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/pointinfo_plugin.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -30,27 +30,27 @@
         };
 
         /**
          * Remove event handlers
          */
         this._disable_event_handlers = function() {
             if (this.grid) {
-                this.grid.off('click', $.proxy(this, "_on_click"));
+                this.grid.off('click', $.proxy(this, '_on_click'));
             }
         };
 
         /**
          * redraw hanlder
          */
         this.redraw = function(layers) {
             // todo: handle click events
             this._disable_event_handlers();
             this.layers = layers;
             this.grid = layers['grid'];
-            this.grid.on('click', $.proxy(this, "_on_click"));
+            this.grid.on('click', $.proxy(this, '_on_click'));
 
             // todo: should we handle clicks outside the map, and remove the marker?
             // todo: should we handler the escape key and remove the marker ?
         };
 
         /**
          * click handler
@@ -65,15 +65,20 @@
                 }
                 $(this.animation).stop();
             }
             if (this.layers['_point_info_plugin']) {
                 view.map.removeLayer(this.layers['_point_info_plugin']);
                 view.map.removeLayer(this.layers['_point_info_plugin_1']);
             }
-            if (props && props.data && (view.map_info.repeat_map || (props.latlng.lng >= -180 && props.latlng.lng <= 180))) {
+            if (
+                props &&
+                props.data &&
+                (view.map_info.repeat_map ||
+                    (props.latlng.lng >= -180 && props.latlng.lng <= 180))
+            ) {
                 // Find coordinates. The values in props.latlng is the mouse position, not the point position -
                 // however it helps us know if we have clicked on a point that is wrapped around the world.
                 var lat = props.data.record_latitude;
                 var lng = props.data.record_longitude;
                 if (props.latlng.lng > 180) {
                     // Tricky because the clicking might not be within the same 360 block at the center of the marker. We must
                     // test for this eventuality.
@@ -85,49 +90,55 @@
                     lng = lng - Math.floor((lng - props.latlng.lng) / 360) * 360;
                     if (lng - props.latlng.lng > 180) {
                         lng = lng - 360;
                     }
                 }
                 // Highlight the point
                 this.layers['_point_info_plugin'] = L.circleMarker([lat, lng], {
-                    radius: 4,
-                    /* Ideally the same as the cartoCSS version */
+                    radius: 4 /* Ideally the same as the cartoCSS version */ ,
                     stroke: true,
                     color: '#FFF',
                     weight: 1,
                     fill: true,
                     fillColor: '#00F',
                     opacity: 1,
                     fillOpacity: 1,
-                    clickable: false
+                    clickable: false,
                 });
                 // Create pulse layer
                 this.layers['_point_info_plugin_1'] = L.circleMarker([lat, lng], {
                     radius: 1,
                     stroke: true,
                     weight: 4,
                     color: '#88F',
                     fill: false,
                     fillColor: '#FFF',
                     fillOpacity: 1,
-                    clickable: false
+                    clickable: false,
                 });
                 this._animate(this.layers['_point_info_plugin_1']);
                 // Add the layers in order
                 view.map.addLayer(this.layers['_point_info_plugin_1']);
                 view.map.addLayer(this.layers['_point_info_plugin']);
                 // Add the info in the sidebar
                 props.data._resource_url = window.parent.location.pathname;
-                props.data._multiple = options.count_field && props.data[options.count_field] > 1;
-                if (window.parent.ckan && window.parent.ckan.views.filters && props.data.geo_filter) {
+                props.data._multiple =
+                    options.count_field && props.data[options.count_field] > 1;
+                if (
+                    window.parent.ckan &&
+                    window.parent.ckan.views.filters &&
+                    props.data.geo_filter
+                ) {
                     var filters = window.parent.ckan.views.filters.get();
                     var furl = new my.CkanFilterUrl().set_filters(filters);
                     furl.remove_filter('__geo__');
                     furl.add_filter('__geo__', JSON.stringify(props.data.geo_filter));
-                    props.data._overlapping_records_filters = encodeURIComponent(furl.get_filters());
+                    props.data._overlapping_records_filters = encodeURIComponent(
+                        furl.get_filters(),
+                    );
                 }
                 view.sidebar_view.render(props.data, options['template']);
                 var ensure_point = view.map.latLngToContainerPoint([lat, lng]);
                 view.openSidebar(ensure_point.x, ensure_point.y);
             } else {
                 delete this.layers['_point_info_plugin'];
                 delete this.layers['_point_info_plugin_1'];
@@ -139,15 +150,15 @@
         /**
          * Animate
          */
         this._animate = function(layer) {
             var plugin = this;
             this.$animation = $('<div></div>').css('opacity', 0);
             this.$animation.animate({
-                opacity: 1
+                opacity: 1,
             }, {
                 duration: 750,
                 easing: 'swing',
                 step: function(value, fx) {
                     layer.setRadius(1 + value * 19);
                     layer.setStyle({
                         fillOpacity: 1 - value
@@ -157,12 +168,12 @@
                     });
                 },
                 complete: function() {
                     plugin.animation_restart = setTimeout(function() {
                         plugin.animation_restart = false;
                         $.proxy(plugin, '_animate')(layer);
                     }, 1000);
-                }
-            });
-        }
+                },
+            }, );
+        };
     };
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/sidebar_view.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -15,38 +15,38 @@
         render: function(data, template) {
             var self = this;
             var out = '';
             if (!data) {
                 out = Mustache.render(this.template);
             } else if (data && !template) {
                 for (var i in data) {
-                    out = i.toString() + ": " + data.toString() + "<br/>";
+                    out = i.toString() + ': ' + data.toString() + '<br/>';
                 }
             } else {
                 out = Mustache.render(template, data);
             }
             if (this.has_content) {
                 this.el.stop().animate({
-                    opacity: 0
+                    opacity: 0,
                 }, {
                     duration: 200,
                     complete: function() {
                         self.el.html(out);
                         self.el.animate({
                             opacity: 1
                         }, {
                             duration: 200
                         });
-                    }
-                });
+                    },
+                }, );
             } else {
                 self.el.html(out);
                 this.el.stop().animate({
                     opacity: 1
                 }, {
                     duration: 200
                 });
             }
             this.has_content = !!data;
-        }
+        },
     });
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/tiledmap_module.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -27,16 +27,20 @@
          * Sometimes this module loads before those properties are defined and therefore this module
          * fails due to the race condition. This only happens/is far more likely to happen when used in
          * an iframe where window.parent actually points to the parent rather than window.
          *
          * @param attempts the number of attempts at checking for the properties that we've done
          */
         waitForViews: function(attempts) {
-            if ((window.parent.ckan && window.parent.ckan.views && window.parent.ckan.views.filters) ||
-                attempts >= 100) {
+            if (
+                (window.parent.ckan &&
+                    window.parent.ckan.views &&
+                    window.parent.ckan.views.filters) ||
+                attempts >= 100
+            ) {
                 // the properties exist or we've waited for 2 seconds, let's go!
                 this.loadView();
             } else {
                 // the properties aren't there yet, wait 50ms and try again
                 setTimeout(this.waitForViews.bind(this, attempts + 1), 50);
             }
         },
@@ -58,16 +62,16 @@
             }
             this.view = new tiledmap.NHMMap({
                 resource_id: this.options.resource.id,
                 view_id: this.options.resource_view.id,
                 filters: {
                     fields: fields,
                     geom: geom,
-                    q: q
-                }
+                    q: q,
+                },
             });
             this.view.render();
             $(this.el).append(this.view.el);
             this.view.show();
-        }
+        },
     };
 });
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/scripts/tooltip_plugin.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -7,21 +7,24 @@
     my.TooltipPlugin = function(view, options) {
         /**
          * enable this plugin
          */
         this.enable = function() {
             this.grid = null;
             this.isactive = true;
-            this.$el = $('<div>').addClass('map-hover-tooltip').css({
-                display: 'none',
-                position: 'absolute',
-                top: 0,
-                left: 0,
-                zIndex: 100
-            }).appendTo(view.map.getContainer());
+            this.$el = $('<div>')
+                .addClass('map-hover-tooltip')
+                .css({
+                    display: 'none',
+                    position: 'absolute',
+                    top: 0,
+                    left: 0,
+                    zIndex: 100,
+                })
+                .appendTo(view.map.getContainer());
             this.hover = false;
         };
 
         /**
          * Disable this plugin
          */
         this.disable = function() {
@@ -31,17 +34,17 @@
         };
 
         /**
          * Remove event handlers
          */
         this._disable_event_handlers = function() {
             if (this.grid) {
-                this.grid.off('mouseover', $.proxy(this, "_mouseover"));
-                this.grid.off('mouseout', $.proxy(this, "_mouseout"));
-                view.map.off('mouseout', $.proxy(this, "_mouseout"));
+                this.grid.off('mouseover', $.proxy(this, '_mouseover'));
+                this.grid.off('mouseout', $.proxy(this, '_mouseout'));
+                view.map.off('mouseout', $.proxy(this, '_mouseout'));
                 this.grid = null;
             }
         };
 
         /**
          * Activate/disactive this plugin
          * (Used for temporary pause)
@@ -53,18 +56,26 @@
         /**
          * Mouseover handler
          */
         this._mouseover = function(props) {
             if (!this.isactive) {
                 return;
             }
-            if (props && props.data && !view.map_info.repeat_map && (props.latlng.lng < -180 || props.latlng.lng > 180)) {
+            if (
+                props &&
+                props.data &&
+                !view.map_info.repeat_map &&
+                (props.latlng.lng < -180 || props.latlng.lng > 180)
+            ) {
                 return;
             }
-            var count = options.count_field && props.data[options.count_field] ? props.data[options.count_field] : 1;
+            var count =
+                options.count_field && props.data[options.count_field] ?
+                props.data[options.count_field] :
+                1;
             var label = false;
             if (options.template && count === 1) {
                 props._multiple = count > 1;
                 props._resource_url = window.parent.location.pathname;
                 label = Mustache.render(options.template, props.data.data);
             } else {
                 label = count + ' record' + (count === 1 ? '' : 's');
@@ -72,76 +83,82 @@
             if (label) {
                 this.$el.stop().html(label);
                 // Place the element with visibility 'hidden' so we can get it's actual height/width.
                 this.$el.css({
                     top: 0,
                     left: 0,
                     visibility: 'hidden',
-                    display: 'block'
+                    display: 'block',
                 });
                 if (typeof this.initial_opacity === 'undefined') {
                     this.initial_opacity = this.$el.css('opacity'); // Store CSS value
                     this.$el.css('opacity', 0);
                 }
                 // Tooltip placement algorithm.
                 var point = view.map.latLngToContainerPoint(props.latlng);
                 var width = this.$el.width();
                 var height = this.$el.height();
                 var map_size = view.map.getSize();
                 var top, left;
-                if (point.x > map_size.x * 4 / 5 || point.x + width + 16 > map_size.x) {
+                if (
+                    point.x > (map_size.x * 4) / 5 ||
+                    point.x + width + 16 > map_size.x
+                ) {
                     left = point.x - width - 16;
                 } else {
                     left = point.x + 16;
                 }
                 if (point.y < map_size.y / 5) {
                     top = point.y + height * 0.5 + 8;
                 } else {
                     top = point.y - height * 1.5 - 8;
                 }
                 this.hover = true;
-                this.$el.css({
-                    top: top,
-                    left: left,
-                    visibility: 'visible'
-                }).stop().animate({
-                    opacity: this.initial_opacity
-                }, {
-                    duration: 100
-                });
+                this.$el
+                    .css({
+                        top: top,
+                        left: left,
+                        visibility: 'visible',
+                    })
+                    .stop()
+                    .animate({
+                        opacity: this.initial_opacity,
+                    }, {
+                        duration: 100,
+                    }, );
             }
             // Set the mouse cursor.
             $('div.panel.map').css('cursor', 'pointer');
         };
 
         /**
          * Mouseout handler
          */
         this._mouseout = function() {
             if (this.hover && this.$el) {
                 this.hover = false;
                 this.$el.stop().animate({
-                    'opacity': 0
+                    opacity: 0,
                 }, {
                     duration: 100,
                     complete: function() {
                         $(this).html('');
                         $(this).css('display', 'none');
-                    }
-                });
+                    },
+                }, );
                 // Remove the mouse cursor
                 $('div.panel.map').css('cursor', '');
             }
         };
 
         /**
          * redraw handler
          */
         this.redraw = function(layers) {
             this._disable_event_handlers();
             this.grid = layers['grid'];
-            this.grid.on('mouseover', $.proxy(this, "_mouseover"));
-            this.grid.on('mouseout', $.proxy(this, "_mouseout"));
-            view.map.on('mouseout', $.proxy(this, "_mouseout")); // UtfGrid doesn't trigger mouseout when you leave the map
-        }
-    }
+            this.grid.on('mouseover', $.proxy(this, '_mouseover'));
+            this.grid.on('mouseout', $.proxy(this, '_mouseout'));
+            view.map.on('mouseout', $.proxy(this, '_mouseout')); // UtfGrid doesn't trigger mouseout when you leave the map
+        };
+    };
 })(this.tiledmap, jQuery);
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/backbone/1.0.0/backbone.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/jquery/1.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw-src.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.draw/leaflet.draw.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.minimap/readme.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/leaflet.utfgrid/leaflet.utfgrid.queue.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/mustache/0.5.0-dev/mustache.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer-wkt-parser.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/terraformer/terraformer.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/vendor/underscore/1.4.2/underscore.min.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/assets/webassets.yml` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/assets/webassets.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/data/countries.geojson` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/data/countries.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/layers.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-icon.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet-2x.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/public/vendor/leaflet/leaflet.draw/spritesheet.png`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/map_form.html` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/map_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail.dwc.mustache`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext/tiledmap/theme/templates/point_detail.mustache` & `ckanext-versioned-tiledmap-2.1.9/ckanext/tiledmap/theme/templates/point_detail.mustache`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/PKG-INFO` & `ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-tiledmap
-Version: 2.1.8
+Version: 2.1.9
 Summary: A CKAN extension with a map view for versioned-datastore backed resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-tiledmap/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_tiledmap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/ckanext_versioned_tiledmap.egg-info/SOURCES.txt` & `ckanext-versioned-tiledmap-2.1.9/ckanext_versioned_tiledmap.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -63,8 +63,12 @@
 ckanext_versioned_tiledmap.egg-info/PKG-INFO
 ckanext_versioned_tiledmap.egg-info/SOURCES.txt
 ckanext_versioned_tiledmap.egg-info/dependency_links.txt
 ckanext_versioned_tiledmap.egg-info/entry_points.txt
 ckanext_versioned_tiledmap.egg-info/not-zip-safe
 ckanext_versioned_tiledmap.egg-info/requires.txt
 ckanext_versioned_tiledmap.egg-info/top_level.txt
-docs/_scripts/gen_api_pages.py
+docs/_scripts/gen_api_pages.py
+tests/test_helpers.py
+tests/test_route_helpers.py
+tests/test_utils.py
+tests/test_validators.py
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/docs/_scripts/gen_api_pages.py` & `ckanext-versioned-tiledmap-2.1.9/docs/_scripts/gen_api_pages.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 nav = mkdocs_gen_files.Nav()
 
 root = 'ckanext'
 
 py_files = sorted(Path(root).rglob('*.py'))
 
 for path in py_files:
+    try:
+        path.relative_to('ckanext/versioned_tiledmap/migration')
+        continue
+    except ValueError:
+        pass
+
     module_path = path.relative_to(root).with_suffix('')
     doc_path = path.relative_to(root).with_suffix('.md')
     full_doc_path = Path('API', doc_path)
 
     parts = tuple(module_path.parts)
 
     if parts[-1] == '__init__':
@@ -31,15 +37,15 @@
         doc_path = doc_path.with_name('index.md')
         full_doc_path = full_doc_path.with_name('index.md')
     elif parts[-1] == '__main__':
         continue
 
     nav[parts] = doc_path.as_posix()
 
-    with mkdocs_gen_files.open(full_doc_path, "w") as fd:
+    with mkdocs_gen_files.open(full_doc_path, 'w') as fd:
         ident = '.'.join(parts)
         fd.write(f'::: ckanext.{ident}')
 
     mkdocs_gen_files.set_edit_path(full_doc_path, path)
 
 with mkdocs_gen_files.open('API/index.md', 'w') as nav_file:
     nav_file.writelines(nav.build_literate_nav())
```

### Comparing `ckanext-versioned-tiledmap-2.1.8/pyproject.toml` & `ckanext-versioned-tiledmap-2.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-versioned-tiledmap"
-version = "2.1.8"
+version = "2.1.9"
 description = "A CKAN extension with a map view for versioned-datastore backed resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,15 +52,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.tiledmap.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.1.8"
+version = "2.1.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

