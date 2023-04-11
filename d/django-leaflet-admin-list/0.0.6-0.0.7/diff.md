# Comparing `tmp/django-leaflet-admin-list-0.0.6.tar.gz` & `tmp/django-leaflet-admin-list-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-leaflet-admin-list-0.0.6.tar", last modified: Mon Feb 20 18:59:58 2023, max compression
+gzip compressed data, was "django-leaflet-admin-list-0.0.7.tar", last modified: Tue Apr 11 10:16:05 2023, max compression
```

## Comparing `django-leaflet-admin-list-0.0.6.tar` & `django-leaflet-admin-list-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/
--rw-rw-r--   0 seva      (1000) seva      (1000)     7652 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/LICENSE
--rw-rw-r--   0 seva      (1000) seva      (1000)       60 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/MANIFEST.in
--rw-rw-r--   0 seva      (1000) seva      (1000)     1218 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/PKG-INFO
--rw-rw-r--   0 seva      (1000) seva      (1000)      196 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/README.rst
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/
--rw-rw-r--   0 seva      (1000) seva      (1000)     1218 2023-02-20 18:59:58.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/PKG-INFO
--rw-rw-r--   0 seva      (1000) seva      (1000)      596 2023-02-20 18:59:58.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/SOURCES.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)        1 2023-02-20 18:59:58.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/dependency_links.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)        1 2022-04-01 09:20:29.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/not-zip-safe
--rw-rw-r--   0 seva      (1000) seva      (1000)       22 2023-02-20 18:59:58.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/requires.txt
--rw-rw-r--   0 seva      (1000) seva      (1000)       19 2023-02-20 18:59:58.000000 django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/top_level.txt
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/leaflet_admin_list/
--rw-rw-r--   0 seva      (1000) seva      (1000)       41 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/__init__.py
--rw-rw-r--   0 seva      (1000) seva      (1000)     7228 2022-04-01 13:45:11.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/admin.py
--rw-rw-r--   0 seva      (1000) seva      (1000)     1705 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/filters.py
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-02-20 18:59:58.723479 django-leaflet-admin-list-0.0.6/leaflet_admin_list/templates/
-drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/leaflet_admin_list/templates/leaflet_admin_list/
--rw-rw-r--   0 seva      (1000) seva      (1000)      472 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_filter.html
--rw-rw-r--   0 seva      (1000) seva      (1000)     7522 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_list.html
--rw-rw-r--   0 seva      (1000) seva      (1000)       22 2023-02-20 15:40:17.000000 django-leaflet-admin-list-0.0.6/leaflet_admin_list/version.py
--rw-rw-r--   0 seva      (1000) seva      (1000)       38 2023-02-20 18:59:58.727479 django-leaflet-admin-list-0.0.6/setup.cfg
--rw-rw-r--   0 seva      (1000) seva      (1000)     1609 2022-04-01 14:34:00.000000 django-leaflet-admin-list-0.0.6/setup.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/
+-rw-rw-r--   0 seva      (1000) seva      (1000)     7652 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/LICENSE
+-rw-rw-r--   0 seva      (1000) seva      (1000)       60 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/MANIFEST.in
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1218 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/PKG-INFO
+-rw-rw-r--   0 seva      (1000) seva      (1000)      196 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/README.rst
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1218 2023-04-11 10:16:05.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/PKG-INFO
+-rw-rw-r--   0 seva      (1000) seva      (1000)      596 2023-04-11 10:16:05.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/SOURCES.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)        1 2023-04-11 10:16:05.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/dependency_links.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)        1 2022-04-01 09:20:29.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/not-zip-safe
+-rw-rw-r--   0 seva      (1000) seva      (1000)       22 2023-04-11 10:16:05.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/requires.txt
+-rw-rw-r--   0 seva      (1000) seva      (1000)       19 2023-04-11 10:16:05.000000 django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/top_level.txt
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/leaflet_admin_list/
+-rw-rw-r--   0 seva      (1000) seva      (1000)       41 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/__init__.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)     7228 2022-04-01 13:45:11.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/admin.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1705 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/filters.py
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-04-11 10:16:05.236058 django-leaflet-admin-list-0.0.7/leaflet_admin_list/templates/
+drwxrwxr-x   0 seva      (1000) seva      (1000)        0 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/leaflet_admin_list/templates/leaflet_admin_list/
+-rw-rw-r--   0 seva      (1000) seva      (1000)      472 2022-04-01 09:06:51.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_filter.html
+-rw-rw-r--   0 seva      (1000) seva      (1000)     7682 2023-04-11 09:57:51.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_list.html
+-rw-rw-r--   0 seva      (1000) seva      (1000)       22 2023-04-11 09:57:51.000000 django-leaflet-admin-list-0.0.7/leaflet_admin_list/version.py
+-rw-rw-r--   0 seva      (1000) seva      (1000)       38 2023-04-11 10:16:05.240058 django-leaflet-admin-list-0.0.7/setup.cfg
+-rw-rw-r--   0 seva      (1000) seva      (1000)     1609 2022-04-01 14:34:00.000000 django-leaflet-admin-list-0.0.7/setup.py
```

### Comparing `django-leaflet-admin-list-0.0.6/LICENSE` & `django-leaflet-admin-list-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-leaflet-admin-list-0.0.6/PKG-INFO` & `django-leaflet-admin-list-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-leaflet-admin-list
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django Leaflet Admin List
 Home-page: https://github.com/nnseva/django-leaflet-admin-list
 Author: Vsevolod Novikov
 Author-email: nnseva@gmail.com
 License: LGPL
 Keywords: django admin leaflet map list view
 Classifier: Programming Language :: Python
```

### Comparing `django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/PKG-INFO` & `django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-leaflet-admin-list
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django Leaflet Admin List
 Home-page: https://github.com/nnseva/django-leaflet-admin-list
 Author: Vsevolod Novikov
 Author-email: nnseva@gmail.com
 License: LGPL
 Keywords: django admin leaflet map list view
 Classifier: Programming Language :: Python
```

### Comparing `django-leaflet-admin-list-0.0.6/django_leaflet_admin_list.egg-info/SOURCES.txt` & `django-leaflet-admin-list-0.0.7/django_leaflet_admin_list.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-leaflet-admin-list-0.0.6/leaflet_admin_list/admin.py` & `django-leaflet-admin-list-0.0.7/leaflet_admin_list/admin.py`

 * *Files identical despite different names*

### Comparing `django-leaflet-admin-list-0.0.6/leaflet_admin_list/filters.py` & `django-leaflet-admin-list-0.0.7/leaflet_admin_list/filters.py`

 * *Files identical despite different names*

### Comparing `django-leaflet-admin-list-0.0.6/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_list.html` & `django-leaflet-admin-list-0.0.7/leaflet_admin_list/templates/leaflet_admin_list/leaflet_admin_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,14 @@
     function loadmap() {
         map = L.map('leaflet_admin_list_map', {
             maxZoom: 19,
             maxBounds: [[-90, -180], [90, 180]],
             zoomControl: false,
             attributionControl: false,
         });
-        var hash = document.URL.split('#')[1];
-        if( !hash ) {
-            map.setView([0, 0], 1);
-        }
 
         var colors = [
             '#ff0000', '#800000', '#191970', '#ffa500', '#0000cd', '#7cfc00', '#00fa9a', '#00ffff', '#ff00ff', '#1e90ff', '#ffff54', '#dda0dd', '#ff1493', '#ffdab9', '#2f4f4f', '#6b8e23',
         ]
 
         var osm = L.tileLayer('//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
             attribution: '<a title="{% trans 'Open Street Map Tiles' %}" href="https://www.openstreetmap.org/">OSM</a>',
@@ -50,14 +46,23 @@
                     var tooltip = feature.properties.tooltip;
                     if( tooltip[0] == '<' ) // >
                         tooltip = django.jQuery(feature.properties.tooltip)[0];
                     layer.bindTooltip(tooltip);
                 }
             }
         }).addTo(map);
+        var hash = document.URL.split('#')[1];
+        if( !hash ) {
+            var bounds = geojson.getBounds();
+            if (bounds.isValid()) {
+                map.fitBounds(bounds);
+            } else {
+                map.setView([0, 0], 1);
+            }
+        }
 
         L.control.attribution({
             prefix:
                 '<a title="A JS Library for interactive maps" href="https://leafletjs.com/" target="_blank">Leaflet v.'+L.version+'</a>' + ' | ' +
                 '<a title="{% blocktrans %}Django Leaflet Admin List Version {{ version }}{% endblocktrans %}" href="https://github.com/nnseva/django-leaflet-admin-list">' +
                 '{% blocktrans %}DLAList v.{{ version }}{% endblocktrans %}</a>'
         }).addTo(map).setPosition('bottomright');
```

### Comparing `django-leaflet-admin-list-0.0.6/setup.py` & `django-leaflet-admin-list-0.0.7/setup.py`

 * *Files identical despite different names*

