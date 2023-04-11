# Comparing `tmp/BBFinance-1.4.6.tar.gz` & `tmp/BBFinance-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.6.tar", last modified: Tue Apr 11 14:19:59 2023, max compression
+gzip compressed data, was "BBFinance-1.4.7.tar", last modified: Tue Apr 11 15:10:21 2023, max compression
```

## Comparing `BBFinance-1.4.6.tar` & `BBFinance-1.4.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:22.147733 BBFinance-1.4.6/
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:15.830237 BBFinance-1.4.6/BBFdocs/
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:15.924007 BBFinance-1.4.6/BBFdocs/docs/
--rw-rw-rw-   0        0        0     4250 2023-04-10 19:30:32.000000 BBFinance-1.4.6/BBFdocs/docs/index.md
--rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.4.6/BBFdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:16.205257 BBFinance-1.4.6/BBFdocs/site/
--rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/404.html
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:16.830260 BBFinance-1.4.6/BBFdocs/site/css/
--rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/base.css
--rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/base.min.css
--rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/bootstrap-custom.css
--rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/bootstrap-custom.min.css
--rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/cinder.css
--rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/cinder.min.css
--rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/highlight.css
--rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/css/highlight.min.css
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:17.377185 BBFinance-1.4.6/BBFdocs/site/fonts/
--rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.woff
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:19.458372 BBFinance-1.4.6/BBFdocs/site/img/
--rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/img/favicon.ico
--rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/img/grid1.png
--rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.4.6/BBFdocs/site/img/grid10.png
--rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid11.png
--rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid12.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid13.png
--rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid14.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid15.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid16.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid17.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid18.png
--rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid19.png
--rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid2.png
--rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid20.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid3.png
--rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid4.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid5.png
--rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid6.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid7.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid8.png
--rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/img/grid9.png
--rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/index.html
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:19.770875 BBFinance-1.4.6/BBFdocs/site/js/
--rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/js/base.js
--rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/js/bootstrap-3.0.3.min.js
--rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/js/highlight.pack.js
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:20.442766 BBFinance-1.4.6/BBFdocs/site/search/
--rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/search/lunr.js
--rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/search/main.js
--rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/search/search_index.json
--rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/search/worker.js
--rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/sitemap.xml
--rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.4.6/BBFdocs/site/sitemap.xml.gz
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:20.724028 BBFinance-1.4.6/BBFinance/
--rw-rw-rw-   0        0        0    38842 2023-04-10 19:06:27.000000 BBFinance-1.4.6/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      312 2023-04-10 15:30:26.000000 BBFinance-1.4.6/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:21.584448 BBFinance-1.4.6/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.6/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    23312 2023-04-10 17:41:27.000000 BBFinance-1.4.6/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.6/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      422 2023-04-10 17:41:27.000000 BBFinance-1.4.6/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:21.303188 BBFinance-1.4.6/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-04-11 14:23:06.000000 BBFinance-1.4.6/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1918 2023-04-11 14:23:14.000000 BBFinance-1.4.6/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:23:06.000000 BBFinance-1.4.6/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      326 2023-04-11 14:23:06.000000 BBFinance-1.4.6/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 14:23:06.000000 BBFinance-1.4.6/BBFinance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:21.834462 BBFinance-1.4.6/Data/
--rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.6/Data/AtivosIbov.xlsx
--rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2023 2023-04-11 14:23:22.132108 BBFinance-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 14:23:22.038353 BBFinance-1.4.6/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.6/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.6/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     1204 2023-04-10 17:22:53.000000 BBFinance-1.4.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 14:23:22.163356 BBFinance-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-04-11 14:22:22.000000 BBFinance-1.4.6/setup.py
--rw-rw-rw-   0        0        0       59 2023-04-10 17:42:02.000000 BBFinance-1.4.6/teste.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.959608 BBFinance-1.4.7/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.004850 BBFinance-1.4.7/BBFdocs/
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.239243 BBFinance-1.4.7/BBFdocs/docs/
+-rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.4.7/BBFdocs/docs/index.md
+-rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.4.7/BBFdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.364258 BBFinance-1.4.7/BBFdocs/site/
+-rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/404.html
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:38.801819 BBFinance-1.4.7/BBFdocs/site/css/
+-rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/base.css
+-rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/base.min.css
+-rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.css
+-rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.min.css
+-rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/cinder.css
+-rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/cinder.min.css
+-rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/highlight.css
+-rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/css/highlight.min.css
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:41.286723 BBFinance-1.4.7/BBFdocs/site/fonts/
+-rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.woff
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.286930 BBFinance-1.4.7/BBFdocs/site/img/
+-rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/favicon.ico
+-rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/grid1.png
+-rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.4.7/BBFdocs/site/img/grid10.png
+-rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid11.png
+-rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid12.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid13.png
+-rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid14.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid15.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid16.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid17.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid18.png
+-rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid19.png
+-rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid2.png
+-rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid20.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid3.png
+-rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid4.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid5.png
+-rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid6.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid7.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid8.png
+-rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/img/grid9.png
+-rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/index.html
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.536957 BBFinance-1.4.7/BBFdocs/site/js/
+-rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/base.js
+-rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/bootstrap-3.0.3.min.js
+-rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/js/highlight.pack.js
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:43.880753 BBFinance-1.4.7/BBFdocs/site/search/
+-rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/lunr.js
+-rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/main.js
+-rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/search_index.json
+-rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/search/worker.js
+-rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/sitemap.xml
+-rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.4.7/BBFdocs/site/sitemap.xml.gz
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.005764 BBFinance-1.4.7/BBFinance/
+-rw-rw-rw-   0        0        0    38842 2023-04-10 19:06:27.000000 BBFinance-1.4.7/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      312 2023-04-10 15:30:26.000000 BBFinance-1.4.7/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.412650 BBFinance-1.4.7/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23312 2023-04-10 17:41:27.000000 BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.7/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      422 2023-04-10 17:41:27.000000 BBFinance-1.4.7/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.334516 BBFinance-1.4.7/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1918 2023-04-11 15:13:35.000000 BBFinance-1.4.7/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 15:13:27.000000 BBFinance-1.4.7/BBFinance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.709559 BBFinance-1.4.7/Data/
+-rw-rw-rw-   0        0        0    14286 2023-04-10 14:00:41.000000 BBFinance-1.4.7/Data/AtivosIbov.xlsx
+-rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2023 2023-04-11 15:13:44.975215 BBFinance-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-04-06 20:03:42.000000 BBFinance-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 15:13:44.865867 BBFinance-1.4.7/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.7/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.7/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1354 2023-04-11 15:11:55.000000 BBFinance-1.4.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 15:13:45.006488 BBFinance-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-04-11 15:12:33.000000 BBFinance-1.4.7/setup.py
+-rw-rw-rw-   0        0        0       59 2023-04-10 17:42:02.000000 BBFinance-1.4.7/teste.py
```

### Comparing `BBFinance-1.4.6/BBFdocs/docs/index.md` & `BBFinance-1.4.7/BBFdocs/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Bem vindo a documentação do BBFinance!
 
 A BBFinance é uma biblioteca com o objetivo de apresentar informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado de investimentos.
 
 Para instalar a biblioteca utilize o comando `pip install BBFinance`.
 
-Para maiores informações acesse a pagina do Pypi. [Instalação](https://pypi.org/project/BBFinance/)
+Para maiores informações acesse a pagina do Pypi. [Instalação](https://github.com/beb0pp/BBFinance)
 
 A BBFinance possui diversos recursos, como:
 
 * Analise de preços e informações de ações e fundos de investimentos.
 * Apuração de tendências de preços e cálculos mais avançados como RSI e Alocação de Markowitz dos ativos.
 * Simuladores de posições, analisa as melhores ações para investir.
 * Comparadores de fundos e ativos.
```

### Comparing `BBFinance-1.4.6/BBFdocs/site/404.html` & `BBFinance-1.4.7/BBFdocs/site/404.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/base.css` & `BBFinance-1.4.7/BBFdocs/site/css/base.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/base.min.css` & `BBFinance-1.4.7/BBFdocs/site/css/base.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/bootstrap-custom.css` & `BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/bootstrap-custom.min.css` & `BBFinance-1.4.7/BBFdocs/site/css/bootstrap-custom.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/cinder.css` & `BBFinance-1.4.7/BBFdocs/site/css/cinder.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/cinder.min.css` & `BBFinance-1.4.7/BBFdocs/site/css/cinder.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/highlight.css` & `BBFinance-1.4.7/BBFdocs/site/css/highlight.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/css/highlight.min.css` & `BBFinance-1.4.7/BBFdocs/site/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.eot` & `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.svg` & `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.ttf` & `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/fonts/fontawesome-webfont.woff` & `BBFinance-1.4.7/BBFdocs/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/img/favicon.ico` & `BBFinance-1.4.7/BBFdocs/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/index.html` & `BBFinance-1.4.7/BBFdocs/site/index.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/js/base.js` & `BBFinance-1.4.7/BBFdocs/site/js/base.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/js/bootstrap-3.0.3.min.js` & `BBFinance-1.4.7/BBFdocs/site/js/bootstrap-3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/js/highlight.pack.js` & `BBFinance-1.4.7/BBFdocs/site/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/search/lunr.js` & `BBFinance-1.4.7/BBFdocs/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/search/main.js` & `BBFinance-1.4.7/BBFdocs/site/search/main.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/search/search_index.json` & `BBFinance-1.4.7/BBFdocs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFdocs/site/search/worker.js` & `BBFinance-1.4.7/BBFdocs/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFinance/BBFinance.py` & `BBFinance-1.4.7/BBFinance/BBFinance.py`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.4.7/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.4.7/BBFinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.6
+Version: 1.4.7
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.6/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.4.7/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/Data/AtivosIbov.xlsx` & `BBFinance-1.4.7/Data/AtivosIbov.xlsx`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/LICENSE.txt` & `BBFinance-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/PKG-INFO` & `BBFinance-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.6
+Version: 1.4.7
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.6/README.md` & `BBFinance-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/__pycache__/main.cpython-39.pyc` & `BBFinance-1.4.7/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.6/requirements.txt` & `BBFinance-1.4.7/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-﻿yfinance                      0.2.12
+﻿yfinance                      0.2.14
 scipy                         1.9.3
 selenium                      3.141.0
 pandas                        1.5.3
 pandas-datareader             0.10.0
 json5                         0.9.6
 numpy                         1.23.4
 uvicorn                       0.21.1
 fastapi                       0.95.0
 scipy                         1.10.1
 requests                      2.28.2
 bs4                           0.0.1
 beautifulsoup4                4.11.2
 pydantic                      1.10.7
 Unicode                       1.3.6
-typing_extensions             4.5.0
+typing_extensions             4.5.0
+scikit-image                  0.19.3
+scikit-learn                  1.2.2
```

### Comparing `BBFinance-1.4.6/setup.py` & `BBFinance-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4.6',
+    version='1.4.7',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='MIT',
     packages=['BBFinance'],
     long_description= long_description,
@@ -26,16 +26,15 @@
         'requests>=2.28.2',
         'bs4>=0.0.1',
         'beautifulsoup4>=4.11.2',
         'pydantic>=1.10.7',
         'Unicode>=1.3.6',
         'typing_extensions>=4.5.0',
         'scikit-image>=0.19.3',
-        'scikit-learn>=1.2.2',
-        'scikit-learn-intelex==2021.20221004.171935',
+        'scikit-learn>=1.2.2'
         
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9',
```

