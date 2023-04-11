# Comparing `tmp/pybi-next-0.3.9.tar.gz` & `tmp/pybi-next-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybi-next-0.3.9.tar", last modified: Sun Mar 12 07:36:43 2023, max compression
+gzip compressed data, was "pybi-next-0.4.0.tar", last modified: Tue Apr 11 11:15:51 2023, max compression
```

## Comparing `pybi-next-0.3.9.tar` & `pybi-next-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.284083 pybi-next-0.3.9/
--rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      477 2023-03-12 07:36:43.283085 pybi-next-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     2037 2023-02-15 15:12:57.000000 pybi-next-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.198713 pybi-next-0.3.9/pybi/
--rw-rw-rw-   0        0        0     1138 2023-03-12 07:30:16.000000 pybi-next-0.3.9/pybi/__index.py
--rw-rw-rw-   0        0        0       49 2023-03-12 07:36:23.000000 pybi-next-0.3.9/pybi/__init__.py
--rw-rw-rw-   0        0        0    12235 2023-03-12 07:34:33.000000 pybi-next-0.3.9/pybi/app.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.203675 pybi-next-0.3.9/pybi/core/
--rw-rw-rw-   0        0        0       81 2023-03-09 16:59:45.000000 pybi-next-0.3.9/pybi/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.213649 pybi-next-0.3.9/pybi/core/components/
--rw-rw-rw-   0        0        0      453 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/core/components/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-03-11 14:40:12.000000 pybi-next-0.3.9/pybi/core/components/component.py
--rw-rw-rw-   0        0        0      349 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/core/components/componentTag.py
--rw-rw-rw-   0        0        0     6108 2023-03-11 14:40:17.000000 pybi-next-0.3.9/pybi/core/components/containerComponent.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.223622 pybi-next-0.3.9/pybi/core/components/reactiveComponent/
--rw-rw-rw-   0        0        0      116 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-03-09 16:59:45.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/base.py
--rw-rw-rw-   0        0        0     6133 2023-03-12 07:32:49.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/echarts.py
--rw-rw-rw-   0        0        0      628 2023-03-09 16:59:45.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/slicer.py
--rw-rw-rw-   0        0        0     1224 2023-03-11 14:40:12.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/table.py
--rw-rw-rw-   0        0        0      428 2023-03-09 16:59:45.000000 pybi-next-0.3.9/pybi/core/components/reactiveComponent/textValue.py
--rw-rw-rw-   0        0        0      374 2023-02-19 18:03:53.000000 pybi-next-0.3.9/pybi/core/components/staticComponent.py
--rw-rw-rw-   0        0        0     6135 2023-03-09 16:59:45.000000 pybi-next-0.3.9/pybi/core/dataSource.py
--rw-rw-rw-   0        0        0     4565 2023-03-12 07:32:35.000000 pybi-next-0.3.9/pybi/core/sql.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.229606 pybi-next-0.3.9/pybi/core/styles/
--rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/core/styles/__init__.py
--rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.3.9/pybi/core/styles/styles.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.237584 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/
--rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/boxShadow.py
--rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textAlign.py
--rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textColor.py
--rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textSize.py
--rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.3.9/pybi/core/styles/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.251351 pybi-next-0.3.9/pybi/easyEcharts/
--rw-rw-rw-   0        0        0     1820 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/easyEcharts/__init__.py
--rw-rw-rw-   0        0        0     3074 2023-03-11 14:40:12.000000 pybi-next-0.3.9/pybi/easyEcharts/bar.py
--rw-rw-rw-   0        0        0     3027 2023-03-11 14:40:12.000000 pybi-next-0.3.9/pybi/easyEcharts/base.py
--rw-rw-rw-   0        0        0     3288 2023-03-11 14:40:17.000000 pybi-next-0.3.9/pybi/easyEcharts/line.py
--rw-rw-rw-   0        0        0     2527 2023-03-11 14:40:12.000000 pybi-next-0.3.9/pybi/easyEcharts/pie.py
--rw-rw-rw-   0        0        0     2057 2023-03-11 14:40:17.000000 pybi-next-0.3.9/pybi/easyEcharts/scatter.py
--rw-rw-rw-   0        0        0     1498 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/easyEcharts/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.253150 pybi-next-0.3.9/pybi/template/
--rw-rw-rw-   0        0        0  2646997 2023-03-12 07:29:03.000000 pybi-next-0.3.9/pybi/template/index.html
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.270145 pybi-next-0.3.9/pybi/utils/
--rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.3.9/pybi/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.3.9/pybi/utils/dataSourceUtils.py
--rw-rw-rw-   0        0        0     2299 2023-02-15 14:58:33.000000 pybi-next-0.3.9/pybi/utils/data_gen.py
--rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.3.9/pybi/utils/dictUtils.py
--rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.3.9/pybi/utils/helper.py
--rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.3.9/pybi/utils/markdown2.py
--rw-rw-rw-   0        0        0     1398 2023-03-07 07:07:09.000000 pybi-next-0.3.9/pybi/utils/sql.py
-drwxrwxrwx   0        0        0        0 2023-03-12 07:36:43.281092 pybi-next-0.3.9/pybi_next.egg-info/
--rw-rw-rw-   0        0        0      477 2023-03-12 07:36:42.000000 pybi-next-0.3.9/pybi_next.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-03-12 07:36:42.000000 pybi-next-0.3.9/pybi_next.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 07:36:42.000000 pybi-next-0.3.9/pybi_next.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.3.9/pybi_next.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-03-12 07:36:42.000000 pybi-next-0.3.9/pybi_next.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-12 07:36:42.000000 pybi-next-0.3.9/pybi_next.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 07:36:43.284083 pybi-next-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1335 2023-03-07 07:07:09.000000 pybi-next-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.260890 pybi-next-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      477 2023-04-11 11:15:51.259921 pybi-next-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.125437 pybi-next-0.4.0/pybi/
+-rw-rw-rw-   0        0        0     1653 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/__index.py
+-rw-rw-rw-   0        0        0       49 2023-04-11 11:13:39.000000 pybi-next-0.4.0/pybi/__init__.py
+-rw-rw-rw-   0        0        0    18405 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/app.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.134387 pybi-next-0.4.0/pybi/core/
+-rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.145745 pybi-next-0.4.0/pybi/core/components/
+-rw-rw-rw-   0        0        0      631 2023-03-30 15:24:18.000000 pybi-next-0.4.0/pybi/core/components/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-03-29 14:36:39.000000 pybi-next-0.4.0/pybi/core/components/component.py
+-rw-rw-rw-   0        0        0      532 2023-03-30 15:24:18.000000 pybi-next-0.4.0/pybi/core/components/componentTag.py
+-rw-rw-rw-   0        0        0     7854 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/containerComponent.py
+-rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.0/pybi/core/components/mermaid.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.163697 pybi-next-0.4.0/pybi/core/components/reactiveComponent/
+-rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/base.py
+-rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/echarts.py
+-rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/input.py
+-rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/markdown.py
+-rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/numberSlider.py
+-rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/slicer.py
+-rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/table.py
+-rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/textValue.py
+-rw-rw-rw-   0        0        0     1008 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/staticComponent.py
+-rw-rw-rw-   0        0        0     6135 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/dataSource.py
+-rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.169712 pybi-next-0.4.0/pybi/core/styles/
+-rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/__init__.py
+-rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.0/pybi/core/styles/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.178657 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/
+-rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/boxShadow.py
+-rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textAlign.py
+-rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textColor.py
+-rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textSize.py
+-rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.0/pybi/core/styles/utils.py
+-rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/uiResource.py
+-rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/webResources.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.193617 pybi-next-0.4.0/pybi/easyEcharts/
+-rw-rw-rw-   0        0        0     1944 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/easyEcharts/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-04-11 11:03:46.000000 pybi-next-0.4.0/pybi/easyEcharts/bar.py
+-rw-rw-rw-   0        0        0     3592 2023-04-11 11:04:22.000000 pybi-next-0.4.0/pybi/easyEcharts/base.py
+-rw-rw-rw-   0        0        0     3334 2023-04-11 11:04:42.000000 pybi-next-0.4.0/pybi/easyEcharts/line.py
+-rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/easyEcharts/map.py
+-rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.0/pybi/easyEcharts/pie.py
+-rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.0/pybi/easyEcharts/scatter.py
+-rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.0/pybi/easyEcharts/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.199603 pybi-next-0.4.0/pybi/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/iconManager.py
+-rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/material_icons.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.230519 pybi-next-0.4.0/pybi/static/
+-rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.0/pybi/static/echarts.min.js
+-rw-rw-rw-   0        0        0      468 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/echartsCps-style.css
+-rw-rw-rw-   0        0        0    27467 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/echartsCps.iife.js
+-rw-rw-rw-   0        0        0   119709 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/elementCps-style.css
+-rw-rw-rw-   0        0        0   349813 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/elementCps.iife.js
+-rw-rw-rw-   0        0        0  2778154 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/mermaidCps.iife.js
+-rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.0/pybi/static/province_map_full.json
+-rw-rw-rw-   0        0        0     2000 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/sysApp-style.css
+-rw-rw-rw-   0        0        0  1012054 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/sysApp.iife.js
+-rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.0/pybi/static/vue.global.prod.min.js
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.232513 pybi-next-0.4.0/pybi/template/
+-rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/template/index.html
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.248470 pybi-next-0.4.0/pybi/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.0/pybi/utils/dataSourceUtils.py
+-rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.0/pybi/utils/data_gen.py
+-rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.0/pybi/utils/dictUtils.py
+-rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.0/pybi/utils/echarts_opts_utils.py
+-rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/helper.py
+-rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/markdown2.py
+-rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/utils/pyecharts_utils.py
+-rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/utils/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.258893 pybi-next-0.4.0/pybi_next.egg-info/
+-rw-rw-rw-   0        0        0      477 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2201 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.0/pybi_next.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 11:15:51.260890 pybi-next-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.0/setup.py
```

### Comparing `pybi-next-0.3.9/LICENSE` & `pybi-next-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/README.md` & `pybi-next-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # pybi
 
 pybi 是一个使用 Python 直观简洁声明语句的BI可视化报告库。使用 pybi，你可以创建灵活强大的 BI 式交互报告。生成的报告只有一个 html 文件，用户只需要使用浏览器打开就能看到所有的交互效果，无须 Python 环境。
 
 
+[点击这里，在线执行](https://carson_add.gitee.io/test_page/)
+
+
 [点击这里看效果](https://gitee.com/carson_add/pybi-gallery/blob/master/src/BIExamples/Superstore.gif)
 
 
 ## 例子
 
 示例请移步至 [pybi-gallery](https://gitee.com/carson_add/pybi-gallery)
```

### Comparing `pybi-next-0.3.9/pybi/app.py` & `pybi-next-0.4.0/pybi/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,41 +13,54 @@
     ComponentTag,
     BoxComponent,
     FlowBoxComponent,
     TextComponent,
     UploadComponent,
     GridBoxComponent,
     TabsComponent,
+    Markdown,
+    IconComponent,
+    SvgIconComponent,
+    AffixComponent,
+    Mermaid,
+    Input,
+    NumberSlider,
 )
 from pybi.core.components.reactiveComponent import EChart, Slicer, Table, TextValue
 from pybi.core.dataSource import (
     DataSourceField,
     DataSourceTable,
     DataView,
     DataViewBase,
     PivotDataView,
 )
 from pybi.utils.dataSourceUtils import ds2sqlite_file_base64, ds2sqlite
 from pybi.utils.data_gen import (
-    json_dumps_fn,
+    JsonUtils,
     random_ds_name,
     random_dv_name,
     get_project_root,
 )
+from pybi.utils.markdown2 import markdown
+from pybi.core.uiResource import ResourceManager
 
 from pybi.core.sql import SqlInfo, SqlWrapper
 import pybi.utils.sql as sqlUtils
 from pybi.easyEcharts.base import BaseChart, ChartCollector
 from pybi.easyEcharts import easy_echarts
 from pybi.core.components.reactiveComponent.echarts import (
     EChartInfo,
     EChartDatasetInfo,
     EChartJscode,
     OptionsExtractor,
 )
+import pybi.utils.pyecharts_utils as pyecharts_utils
+from pybi.icons.iconManager import get_singleton as get_iconManager
+from pybi.core.webResources import WebResourceManager
+import pybi as pbi
 
 if TYPE_CHECKING:
     pass
     # from pybi.core.components import ReactiveComponent
 
 
 class AppMeta:
@@ -82,14 +95,20 @@
         self.__dataSetNames = set()
         self._with_temp_host_stack: List[ContainerComponent] = []
         self._clear_data = False
         self.dbLocalStorage = False
         self.echartsRenderer = "canvas"
         self._doc_title = None
         self.__meta = AppMeta(self)
+        self.__json_utils = JsonUtils()
+        self.__resourceManager = ResourceManager()
+        self._iconManager = get_iconManager()
+
+        self.__webResourceManager = WebResourceManager()
+        self.webResources = []
 
     def __record_and_check_dataset_name(self, name: str):
         if name in self.__dataSetNames:
             raise Exception(f"dataset name '{name}' is duplicate")
         self.__dataSetNames.add(name)
 
     @property
@@ -159,20 +178,20 @@
         return SqlWrapper(sql)
 
     def add_upload(
         self,
         *,
         host: Optional[ContainerComponent] = None,
     ):
-
         cp = UploadComponent()
 
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
+        self.__resourceManager.register_element_cps()
         return cp
 
     def add_text(
         self,
         text: Union[str, SqlWrapper],
         *,
         host: Optional[ContainerComponent] = None,
@@ -211,77 +230,90 @@
         cp = Slicer(SqlInfo(sql))
         cp.title = field.name
         cp.add_updateInfo(field.source_name, field._get_sql_field_name())
 
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
+        self.__resourceManager.register_element_cps()
         return cp
 
     def add_table(
         self,
         dataSourceTable: DataSourceTable,
         *,
         host: Optional[ContainerComponent] = None,
     ):
-
         sql = ""
         if dataSourceTable._user_specified_field:
             sql = dataSourceTable._to_sql()
         else:
             sql = f"select * from {dataSourceTable.source_name}"
         cp = Table(SqlInfo(sql))
 
         host = host or self._get_temp_host() or self
         host._add_children(cp)
 
+        self.__resourceManager.register_element_cps()
         return cp
 
     def add_echart(
         self,
         options: Union[Dict, BaseChart, ChartCollector],
         *,
         host: Optional[ContainerComponent] = None,
     ):
         cp = None
 
+        if not isinstance(options, (BaseChart, ChartCollector, dict)):
+            from pyecharts.charts.base import Base
+
+            if isinstance(options, Base):
+                options = options.get_options()
+                assert isinstance(options, dict)
+                pyecharts_utils.replace_jscode(options)
+                #
+                self.__json_utils.mark_pyecharts()
+
         if isinstance(options, (BaseChart, ChartCollector)):
+            opts = options
 
-            if isinstance(options, BaseChart):
-                options = ChartCollector().append(options)
+            if isinstance(opts, BaseChart):
+                opts = ChartCollector().append(opts)
 
             cp = EChart(option_type="dict")
 
             if (
-                len(options._collector) > 1
+                len(opts._collector) > 1
                 and easy_echarts._settings.drill_down_default_set_click_filter
             ):
-                for chart in options._collector:
+                for chart in opts._collector:
                     chart._create_default_click_filter()
 
-            for chart in options._collector:
-                options, updateInfos = chart.get_options_infos()
+            for chart in opts._collector:
+                opts, updateInfos, mapIds = chart.get_options_infos()
 
                 ds_infos = []
                 jscodes = []
 
-                OptionsExtractor.extract_and_remove_from_dict(
-                    options, ds_infos, jscodes
-                )
+                OptionsExtractor.extract_and_remove_from_dict(opts, ds_infos, jscodes)
 
                 ds_infos = [
                     EChartDatasetInfo({}, path, sql._sql_info) for path, sql in ds_infos
                 ]
 
                 jscodes = [EChartJscode(path, jscode) for path, jscode in jscodes]
 
-                info = EChartInfo(options, ds_infos, updateInfos, jscodes)
+                for map_name in mapIds:
+                    self.__webResourceManager.mark_echarts_map(map_name)
+
+                info = EChartInfo(opts, ds_infos, updateInfos, jscodes, mapIds)
                 cp._add_chart_info(info)
 
-        else:
+        elif isinstance(options, dict):
             cp = EChart(option_type="dict")
 
             ds_infos = []
             jscodes = []
 
             OptionsExtractor.extract_and_remove_from_dict(options, ds_infos, jscodes)
 
@@ -291,16 +323,19 @@
 
             jscodes = [EChartJscode(path, jscode) for path, jscode in jscodes]
 
             info = EChartInfo(options, ds_infos, [], jscodes)
             cp._add_chart_info(info)
 
         host = host or self._get_temp_host() or self
+
+        assert cp is not None
         host._add_children(cp)
 
+        self.__resourceManager.register_echarts()
         return cp
 
     def flowBox(
         self,
         *,
         host: Optional[ContainerComponent] = None,
     ):
@@ -349,77 +384,255 @@
         host = host or self._get_temp_host() or self
         host._add_children(cp)
         return cp
 
     def add_tabs(
         self,
         names: List[str],
-        mode="narrowing",
         *,
         host: Optional[ContainerComponent] = None,
     ):
-        """
-        mode: 'fullWidth' | 'narrowing'
-            fullWidth:全宽度;页签栏会横向撑满屏幕宽度
-            narrowing(默认值):收窄;页签栏向左靠拢
-        """
-        cp = TabsComponent(names, mode, appHost=self)
+        """ """
+        cp = TabsComponent(names, appHost=self)
         host = host or self._get_temp_host() or self
         host._add_children(cp)
+
+        self.__resourceManager.register_element_cps()
         return cp
 
     def save_zip_db(self, path: str):
         with open(path, mode="w", encoding="utf8") as f:
             f.write(ds2sqlite_file_base64(self.dataSources))
 
     def save_db(self, path: str):
         if Path(path).exists():
             os.remove(path)
         ds2sqlite(path, self.dataSources)
 
     def _to_json_dict(self):
+        self.webResources.append(
+            {
+                "id": "DbFile",
+                "type": "DbFile",
+                "input": ds2sqlite_file_base64(
+                    self.dataSources, clear_data=self._clear_data
+                ),
+                "actionPipe": [],
+            }
+        )
+
+        # self.webResources.append(
+        #     {
+        #         "id": "maps1",
+        #         "type": "echarts-map",
+        #         "input": ds2sqlite_file_base64(
+        #             self.dataSources, clear_data=self._clear_data
+        #         ),
+        #         "actionPipe": [],
+        #     }
+        # )
+
+        # self.webResources.append(
+        #     {
+        #         "id": "maps1",
+        #         "type": "echarts-map",
+        #         "input": None,
+        #         "actionPipe": [
+        #             {
+        #                 "name": "fetch",
+        #                 "args": {
+        #                     "url": "https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json",
+        #                     "options": {},
+        #                 },
+        #             }
+        #         ],
+        #     }
+        # )
+
+        wrs = self.__webResourceManager.create_webResources()
+        self.webResources.extend(wrs)
+
         data = super()._to_json_dict()
 
-        data["dbFile"] = ds2sqlite_file_base64(
-            self.dataSources, clear_data=self._clear_data
-        )
         if self._doc_title:
             data["docTitle"] = self._doc_title
+
+        data["version"] = pbi.__version__
         return data
 
     def __reset_data(self):
         """support for run on ipython env"""
         self.children = []
         self.dataSources = []
         self.dataViews = []
 
-    def to_json(self):
-        return json_dumps_fn(self, indent=2, ensure_ascii=False)
+    def to_json(self, *args, **kws):
+        return self.__json_utils.dumps(self, *args, **kws)
+        # return json_dumps_fn(self, indent=2, ensure_ascii=False)
 
     def to_raw_html(self):
         try:
             symbol = '"__{{__config_data__}}___"'
 
-            config = json_dumps_fn(self, ensure_ascii=False)
+            config = self.__json_utils.dumps(self)
 
             with open(
                 get_project_root() / "template/index.html", mode="r", encoding="utf8"
             ) as html:
                 res = html.read().replace(symbol, config)
                 return res
         except Exception as e:
             raise e
         else:
             self.__reset_data()
 
     def to_html(self, file, display_output_path=False):
         try:
-            file = Path(file)
-            raw = self.to_raw_html()
+            # file = Path(file)
+            # raw = self.to_raw_html()
+
+            raw = self.__resourceManager.build_html(
+                self.to_json(), svg_infos=get_iconManager().get_infos()
+            )
             Path(file).write_text(raw, "utf8")
 
             if display_output_path:
                 print(f"to html:{file.absolute()}")
         except Exception as e:
             raise e
         else:
             self.__reset_data()
+
+    def add_markdown(
+        self,
+        md: str,
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        # if isinstance(md, SqlWrapper):
+        #     md = str(md)
+        md = SqlInfo.around_backticks(md)
+
+        html = markdown(
+            md,
+            extras=[
+                "fenced-code-blocks",
+                "target-blank-links",
+                "task_list",
+                "code-color",
+                "tag-friendly",
+            ],
+        )
+
+        contents = list(SqlInfo.extract_sql_from_text(html))
+
+        cp = Markdown(contents)
+
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        return cp
+
+    def add_icon(
+        self,
+        icon_svg: str,
+        size="2em",
+        color="currentColor",
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        icon_id = get_iconManager().make_icon(icon_svg)
+        cp = IconComponent(icon_id, size, color)
+
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        return cp
+
+    def add_svg_icon(
+        self,
+        svg: str,
+        size="2em",
+        color="currentColor",
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        cp = SvgIconComponent(svg, size, color)
+
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        return cp
+
+    def affix(
+        self,
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        cp = AffixComponent(self)
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        self.__resourceManager.register_element_cps()
+        return cp
+
+    def add_mermaid(
+        self,
+        graph: str,
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        """
+        [mermaid文档](https://github.com/mermaid-js/mermaid/blob/develop/README.zh-CN.md)
+        ---
+        >>> graph = '''
+        flowchart LR
+        A[Hard] -->|Text| B(Round)
+        B --> C{Decision}
+        C -->|One| D[Result 1]
+        C -->|Two| E[Result 2]
+        '''
+        >>> add_mermaid(graph)
+        """
+        cp = Mermaid(graph)
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        self.__resourceManager.register_mermaid_cps()
+        return cp
+
+    def add_input(
+        self,
+        data: DataSourceTable,
+        field: str,
+        where_expr="like '%${}%'",
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        """ """
+        cp = Input(where_expr).add_updateInfo(data.source_name, field)
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        self.__resourceManager.register_element_cps()
+        return cp
+
+    def add_numberSlider(
+        self,
+        data: DataSourceTable,
+        field: str,
+        where_expr=" between ${0} and ${1}",
+        range=True,
+        *,
+        host: Optional[ContainerComponent] = None,
+    ):
+        """ """
+        cp = (
+            NumberSlider(where_expr)
+            .add_updateInfo(data.source_name, field)
+            .set_props({"range": range})
+        )
+        host = host or self._get_temp_host() or self
+        host._add_children(cp)
+
+        self.__resourceManager.register_element_cps()
+        return cp
```

### Comparing `pybi-next-0.3.9/pybi/core/components/component.py` & `pybi-next-0.4.0/pybi/core/components/reactiveComponent/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional, Dict, Set, Any, Union
 
+from pybi.utils.data_gen import Jsonable
+
+from pybi.core.components import ComponentTag
+from pybi.core.components.component import Component
+from pybi.core.sql import SqlInfo
+
+from pybi.core.dataSource import DataSourceView, DataSourceTable
+import re
 
-from pybi.utils.data_gen import Jsonable, get_global_id
-from .componentTag import ComponentTag
 
 if TYPE_CHECKING:
-    from pybi.core.styles.styles import Style
-    from pybi.core.sql import SqlWrapper
+    from pybi.core.dataSource import DataSourceTable
 
 
-class Component(Jsonable):
-    def __init__(self, tag: ComponentTag) -> None:
-        self.id = get_global_id()
-        self.tag = tag
-        self._debugTag: Optional[str] = None
-        self._styles: List[Style] = []
-        self.visible: Union[bool, SqlWrapper] = True
-        self.__gridArea: str = ""
+class UpdateInfo(Jsonable):
+    def __init__(self, table: str, field: str) -> None:
+        super().__init__()
+        self.table = table
+        self.field = field
 
-    def set_debugTag(self, tag: str):
-        self._debugTag = tag
-        return self
 
-    def set_gridArea(self, area_name: str):
-        self.__gridArea = area_name
+class ReactiveComponent(Component):
+    def __init__(self, tag: ComponentTag) -> None:
+        super().__init__(tag)
+        self._updateInfos: List[UpdateInfo] = []
+
+    def add_updateInfo(self, table: str, field: str):
+        self._updateInfos.append(UpdateInfo(table, field))
         return self
 
     def _to_json_dict(self):
         data = super()._to_json_dict()
-        styles_dict = {}
-        for style in self._styles:
-            styles_dict.update(style._get_styles_dict())
-        data["styles"] = styles_dict
-
-        if isinstance(self.visible, bool) and self.visible == True:
-            del data["visible"]
-
-        if self.__gridArea:
-            data["gridArea"] = self.__gridArea
-
-        data["debugTag"] = self._debugTag
+        data["updateInfos"] = self._updateInfos
 
         return data
 
-    def __add__(self, other: Style):
-        self._styles.append(other)
-        return self
-
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __eq__(self, __o: object) -> bool:
-        if isinstance(__o, self.__class__):
-            return hash(__o.id) == hash(self.id)
 
-        return False
+class SingleReactiveComponent(ReactiveComponent):
+    def __init__(self, tag: ComponentTag, sql: SqlInfo) -> None:
+        super().__init__(tag)
+        self.sqlInfo = sql
+
+    # def sql(self, sql: str):
+    #     self._sql = sql
+    #     return self
```

### Comparing `pybi-next-0.3.9/pybi/core/components/containerComponent.py` & `pybi-next-0.4.0/pybi/core/components/containerComponent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union, List, Optional
+from typing import TYPE_CHECKING, Dict, Union, List, Optional
 
 from .componentTag import ComponentTag
 from .component import Component
+from pybi.icons.iconManager import get_singleton as get_iconManager
 
 if TYPE_CHECKING:
     from pybi.app import App
 
 
 class ContainerComponent(Component):
     def __init__(self, tag: ComponentTag, appHost: Optional[App] = None) -> None:
@@ -164,25 +165,27 @@
         assert self._appHost is not None, "self._appHost must be app instance"
 
     def __getitem__(self, idx: int):
         return self.children[idx]
 
 
 class TabsComponent(ContainerComponent):
-    def __init__(
-        self, names: List[str], mode="narrowing", appHost: Optional[App] = None
-    ) -> None:
+    def __init__(self, names: List[str], appHost: Optional[App] = None) -> None:
         """
         mode: 'fullWidth' | 'narrowing'
         """
         super().__init__(ComponentTag.Tabs, appHost)
         if len(names) > len(set(names)):
             raise Exception("names cannot be duplicated")
         self.names = names
-        self.mode = mode
+        self.__icons = []
+        self.tabsProps = {}
+        self.panelsProps = {}
+        self.tabsClasses: List[str] = []
+        self.panelsClasses: List[str] = []
 
         self.__name2idx = {name: idx for idx, name in enumerate(self.names)}
 
         for _ in range(len(self.names)):
             self._add_children(BoxComponent(appHost))
 
     def __getitem__(self, idx: Union[int, str]):
@@ -190,7 +193,59 @@
             if idx not in self.__name2idx:
                 raise Exception(f"tab name[{idx}] not found")
             idx = self.__name2idx[idx]
 
         res = self.children[idx]
         assert isinstance(res, ContainerComponent)
         return res
+
+    def set_icons(self, icons: List[str]):
+        self.__icons = icons
+
+        self.set_tabsProps({"inline-label": len(icons) > 0})
+        return self
+
+    def set_tabsProps(self, props: Dict):
+        self.tabsProps.update(props)
+        return self
+
+    def set_panelsProps(self, props: Dict):
+        self.panelsProps.update(props)
+        return self
+
+    def set_tabsClasses(self, value: str):
+        """
+        set_tabsClasses('text-primary bg-positive')
+        """
+        values = (v for v in value.split(" ") if v)
+        self.tabsClasses.extend(values)
+        return self
+
+    def set_panelsClasses(self, value: str):
+        """
+        set_panelsClasses('text-primary bg-positive')
+        """
+        values = (v for v in value.split(" ") if v)
+        self.panelsClasses.extend(values)
+        return self
+
+    def set_props(self, props: Dict):
+        return self.set_tabsProps(props)
+
+    def _to_json_dict(self):
+        data = super()._to_json_dict()
+        data["tabsClasses"] = list(dict.fromkeys(data["tabsClasses"]).keys())
+        data["panelsClasses"] = list(dict.fromkeys(data["panelsClasses"]).keys())
+
+        icon_ids = []
+        for icon in self.__icons:
+            icon_id = get_iconManager().make_icon(icon)
+            icon_ids.append(icon_id)
+
+        data["iconIds"] = icon_ids
+
+        return data
+
+
+class AffixComponent(ContainerComponent):
+    def __init__(self, appHost: Optional[App] = None) -> None:
+        super().__init__(ComponentTag.Affix, appHost)
```

### Comparing `pybi-next-0.3.9/pybi/core/components/reactiveComponent/base.py` & `pybi-next-0.4.0/pybi/core/components/reactiveComponent/slicer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,33 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, List, Optional, Dict, Set, Any, Union
+from typing import TYPE_CHECKING, List, Dict
 
-from pybi.utils.data_gen import Jsonable
 
 from pybi.core.components import ComponentTag
-from pybi.core.components.component import Component
-from pybi.core.sql import SqlInfo
-
-from pybi.core.dataSource import DataSourceView, DataSourceTable
-import re
+from .base import SingleReactiveComponent
 
 
 if TYPE_CHECKING:
-    from pybi.core.dataSource import DataSourceTable
-
+    from pybi.core.sql import SqlInfo
 
-class UpdateInfo(Jsonable):
-    def __init__(self, table: str, field: str) -> None:
-        super().__init__()
-        self.table = table
-        self.field = field
 
+class Slicer(SingleReactiveComponent):
+    def __init__(self, sql: SqlInfo) -> None:
+        super().__init__(ComponentTag.Slicer, sql)
+        self.title = ""
+        self.multiple = True
 
-class ReactiveComponent(Component):
-    def __init__(self, tag: ComponentTag) -> None:
-        super().__init__(tag)
-        self._updateInfos: List[UpdateInfo] = []
-
-    def add_updateInfo(self, table: str, field: str):
-        self._updateInfos.append(UpdateInfo(table, field))
+    def set_title(self, title: str):
+        self.title = title
         return self
 
-    def _to_json_dict(self):
-        data = super()._to_json_dict()
-        data["updateInfos"] = self._updateInfos
-
-        return data
-
-
-class SingleReactiveComponent(ReactiveComponent):
-    def __init__(self, tag: ComponentTag, sql: SqlInfo) -> None:
-        super().__init__(tag)
-        self.sqlInfo = sql
+    def set_multiple(self, multiple: bool):
+        self.multiple = multiple
+        return self
 
-    # def sql(self, sql: str):
-    #     self._sql = sql
-    #     return self
+    def set_props(self, props: Dict):
+        """
+        [slicer props](https://element-plus.gitee.io/zh-CN/component/select.html#select-attributes)
+        e.g
+        >>> .add_slicer(...).set_props({'placeholder':'my define placeholder'})
+        """
+        return super().set_props(props)
```

### Comparing `pybi-next-0.3.9/pybi/core/components/reactiveComponent/echarts.py` & `pybi-next-0.4.0/pybi/core/components/reactiveComponent/echarts.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, List, Optional, Dict, Set, Any, Union
 from pybi.core.sql import SqlWrapper
 
 from pybi.utils.data_gen import Jsonable
 from pybi.core.components import ComponentTag
 from .base import ReactiveComponent
 from pybi.core.dataSource import DataSourceTable
-
+import pybi.utils.echarts_opts_utils as echarts_opts_utils
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
     from pybi.core.sql import SqlInfo
 
 
 class EChartSqlInfo(Jsonable):
@@ -75,29 +75,15 @@
 class OptionsExtractor:
     @staticmethod
     def extract_and_remove_from_dict(
         data: Dict,
         out_datasets: List[tuple[str, SqlWrapper]],
         out_jscodes: List[tuple[str, str]],
     ):
-        stack = [(data, "")]
-
-        while len(stack) > 0:
-            target, path = stack.pop()
-
-            if isinstance(target, dict):
-                inputs = ((value, f"{path}.{key}") for key, value in target.items())
-                stack.extend(inputs)
-                continue
-
-            if isinstance(target, list):
-                inputs = ((value, f"{path}[{idx}]") for idx, value in enumerate(target))
-                stack.extend(inputs)
-                continue
-
+        for target, path in echarts_opts_utils.iter_each_items(data):
             if isinstance(target, SqlWrapper):
                 rpath = path[1:]
                 out_datasets.append((rpath, target))
                 OptionsExtractor.set_none_prop(data, rpath)
 
             if isinstance(target, EChartJsCode):
                 rpath = path[1:]
@@ -119,56 +105,35 @@
                 OptionsExtractor.set_none_prop(data, rpath)
 
     @staticmethod
     def set_none_prop(options: Dict, path: str):
         """
         path: 'sreies[0].data[0].item.value'
         """
-        paths = path.split(".")
-        target = options
-        for path in paths[:-1]:
-            if path[-1] == "]":
-                # e.g sreies[0]
-                start_idx = path.index("[")
-                key = path[:start_idx]
-                path_idx = int(path[start_idx + 1 : -1])
-                target = target[key][path_idx]
-            else:
-                # e.g .item
-                target = target[path]
-
-        path = paths[-1]
-        if path[-1] == "]":
-            # e.g sreies[0]
-            start_idx = path.index("[")
-            key = path[:start_idx]
-            path_idx = int(path[start_idx + 1 : -1])
-            target[key][path_idx] = None
-        else:
-            # e.g .item
-            target[path] = None
+        echarts_opts_utils.set_prop_by_path(options, path, None)
 
 
 class EChartInfo(Jsonable):
     def __init__(
         self,
         options: Dict,
         datasetInfos: List[EChartDatasetInfo],
         updateInfos: List[EChartUpdateInfo],
         jscodes: List[EChartJscode],
+        mapIds: Optional[List[str]] = None,
     ):
         self.options = options
         self.datasetInfos = datasetInfos
         self.updateInfos = updateInfos
         self.jsCodes = jscodes
+        self.mapIds = mapIds or []
 
 
 class EChart(ReactiveComponent):
     def __init__(self, *, option_type="dict") -> None:
-
         super().__init__(ComponentTag.EChart)
         self._chart_mappings = {}
         self._chartInfos: List[EChartInfo] = []
         self.optionType = option_type
         self.height = "100%"
 
     def set_height(self, value: str):
```

### Comparing `pybi-next-0.3.9/pybi/core/components/reactiveComponent/table.py` & `pybi-next-0.4.0/pybi/core/components/reactiveComponent/table.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/dataSource.py` & `pybi-next-0.4.0/pybi/core/dataSource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/sql.py` & `pybi-next-0.4.0/pybi/core/sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,22 +38,43 @@
             `rows` e.g `[{name:'x1',age:20,value:100},{name:'x2',age:30,value:200},...]`
             `fields` e.g `['name','age','value']`
         """
         self._sql_info.jsMap = code
         self._sql_info.set_udf_type()
         return self
 
-    def toflatlist(self):
+    def toflatlist(self, with_header=False):
+        """
+        >>> query = pbi.sql('select name,value from {data}')
+        >>> query.toflatlist()
+        >>> [
+                ['name a',100],
+                ['name b',200],
+                ...
+            ]
+
+        >>> query.toflatlist(True)
+        >>> [
+                ['name','value'],
+                ['name a',100],
+                ['name b',200],
+                ...
+            ]
+        """
+
+        cols_define = "const cols=[fields]" if with_header else "const cols=[]"
+
         self.js_map(
-            """
-if (fields.length>1){
-    return rows.map(data=> fields.map(f=> data[f]))
-}else {
-     return rows.map(data=>data[fields[0]])
-}"""
+            f"""
+{cols_define}
+if (fields.length>1){{
+    return [...cols,...rows.map(data=> fields.map(f=> data[f]))] 
+}}else {{
+    return [...cols,...rows.map(data=>data[fields[0]])]
+}}"""
         )
         return self
 
     def __str__(self) -> str:
         return str(self._sql_info)
 
     def _to_json_dict(self):
@@ -102,17 +123,24 @@
             yield SqlInfo(
                 match.group(1), match.group(2), None if len(js_map) == 0 else js_map
             )
             start_idx = span[1]
 
         end_idx = len(text) - 1
 
-        if start_idx < end_idx:
+        if start_idx <= end_idx:
             yield text[start_idx : len(text)]
 
+    @staticmethod
+    def around_backticks(text: str):
+        def add_backtick(match: re.Match):
+            return f"`{match.group()}`"
+
+        return m_sql_from_text_pat.sub(add_backtick, text)
+
 
 # class SqlExtractor:
 #     js_code_flag = "--x_x--0_0--"
 
 #     @staticmethod
 #     def extract_from_dict(
 #         data: Dict,
```

### Comparing `pybi-next-0.3.9/pybi/core/styles/__init__.py` & `pybi-next-0.4.0/pybi/core/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/styles/styles.py` & `pybi-next-0.4.0/pybi/core/styles/styles.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/styles/tailwindStyles/boxShadow.py` & `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/boxShadow.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textAlign.py` & `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textAlign.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textColor.py` & `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textColor.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/core/styles/tailwindStyles/textSize.py` & `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textSize.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/__init__.py` & `pybi-next-0.4.0/pybi/easyEcharts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 from .line import LineChart
 from .bar import BarChart
 from .pie import PieChart
 from .scatter import ScatterChart
+from .map import MapChart
 from typing import TYPE_CHECKING, Optional
+import pybi as pbi
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
 
 
 __all__ = ["easy_echarts"]
 
@@ -66,9 +68,12 @@
         x: str,
         y: str,
         color: Optional[str] = None,
         agg="round(avg(${}),2)",
     ):
         return ScatterChart(data, x, y, color, agg)
 
+    def make_map(self, level="province"):
+        return MapChart(level)
+
 
 easy_echarts = EasyEChartsMeta()
```

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/bar.py` & `pybi-next-0.4.0/pybi/easyEcharts/bar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import annotations
 
-from pybi.core.sql import SqlInfo
 
 from .base import BaseChart
 import pybi as pbi
 import pybi.utils.sql as sqlUtils
 
 
 from typing import TYPE_CHECKING, Optional
-from pybi.core.components.reactiveComponent import EChartDatasetInfo
-from .utils import merge_user_options
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
 
 
 class BarChart(BaseChart):
     def __init__(
@@ -47,15 +44,15 @@
     def get_options_infos(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": [
                 {
                     "type": "",
-                    "data": [],
+                    # "data": [],
                 }
             ],
             "yAxis": [{"type": ""}],
             "series": [],
         }
         base_opt.update(opts)
 
@@ -65,21 +62,25 @@
             sql = f"select {self.x},{agg_field},{self.color} from {self.data} group by {self.color},{self.x}"
         else:
             sql = f"select {self.x},{agg_field} from {self.data} group by {self.x}"
 
         dv = pbi.set_dataView(sql)
 
         if self.color:
+            row_map_x, row_map_y = "r[fields[0]]", "r[fields[1]]"
+            if self._reverse_axis:
+                row_map_x, row_map_y = row_map_y, row_map_x
+
             base_opt["series"] = pbi.sql(
-                f"select {self.y},{self.color} from {dv}"
+                f"select {self.x},{self.y},{self.color} from {dv}"
             ).split_group(
                 self.color,
-                """
-                const data = rows.map(r=> r[fields[0]])
-                return {id:key,data,type:'bar',name:key,universalTransition: {enabled: true, divideShape: 'clone'}}""",
+                f"""
+                const data = rows.map(r=> [{row_map_x},{row_map_y}])
+                return {{id:key,data,type:'bar',name:key,universalTransition: {{enabled: true, divideShape: 'clone'}}}}""",
             )
         else:
             base_opt["series"].append(
                 {
                     "name": self.x,
                     "type": "bar",
                     "id": self.x,
@@ -92,12 +93,16 @@
 
         catAxis = base_opt["xAxis"][0]
         valueAxis = base_opt["yAxis"][0]
 
         if self._reverse_axis:
             catAxis, valueAxis = valueAxis, catAxis
 
-        catAxis["data"] = pbi.sql(f"select distinct {self.x} from {dv}").toflatlist()
+        catAxis["data"] = pbi.sql(
+            f"select distinct {self.x} from {dv} order by {self.x}"
+        ).toflatlist()
         catAxis["type"] = "category"
         valueAxis["type"] = "value"
 
-        return base_opt, self._updateInfos
+        base_opt = self._post_options(base_opt)
+
+        return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/base.py` & `pybi-next-0.4.0/pybi/easyEcharts/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Dict, Tuple, List, Sequence, Union
+from typing import TYPE_CHECKING, Dict, Tuple, List, Any, Union
 
 from pybi.core.components.reactiveComponent.echarts import EChartUpdateInfo
 from pybi.core.dataSource import DataSourceTable
+import pybi.utils.echarts_opts_utils as echarts_opts_utils
+import copy
+from .utils import merge_user_options
+
 
 if TYPE_CHECKING:
-    from pybi.core.components.reactiveComponent import EChartDatasetInfo
+    pass
 
 m_merge_keys = set(["legend", "title", "grid", "series"])
 
 
 class BaseChart:
     def __init__(self) -> None:
         self.__base_opt = {
             "tooltip": {},
             "legend": {},
             "series": [],
             "title": {},
             "grid": {"containLabel": True},
         }
-        self.__merge_opt = {}
+        self._merge_opt = {}
         self._updateInfos: List[EChartUpdateInfo] = []
+        self._prop_by_paths: List[Tuple[str, Any]] = []
 
     def __add__(self, other: BaseChart):
         return ChartCollector().append(self).append(other)
 
     def merge(self, options: Dict):
-        self.__merge_opt = options
+        self._merge_opt = options
         return self
 
     def get_options(self):
-        return {
-            **self.__base_opt,
-            **{k: v for k, v in self.__merge_opt.items() if k in m_merge_keys},
-        }
+        return copy.deepcopy(self.__base_opt)
 
     def set_title(self, text: str):
         opt_title: Dict = self.__base_opt["title"]
         opt_title["text"] = text
 
         return self
 
@@ -63,14 +65,19 @@
         if isinstance(table, DataSourceTable):
             table = table.source_name
 
         self._updateInfos.append(EChartUpdateInfo("click", value_type, table, field))
 
         return self
 
+    def _post_options(self, opts: Dict):
+        opts = merge_user_options(opts, self._merge_opt)
+        self._update_props_by_path(opts)
+        return opts
+
     def _remove_filters(self, actionType: str):
         """
         actionType : 'click' | 'hover'
         """
         self._updateInfos = [
             info for info in self._updateInfos if info.actionType != actionType
         ]
@@ -80,17 +87,28 @@
         return self._remove_filters("click")
 
     def _create_default_click_filter(self):
         pass
 
     def get_options_infos(
         self,
-    ) -> Tuple[Dict, List[EChartUpdateInfo]]:
+    ) -> Tuple[Dict, List[EChartUpdateInfo], List[str]]:
         raise NotImplementedError
 
+    def set_prop_by_path(self, path: str, value):
+        """
+        >>> .set_prop_by_path('xAxis[0].axisLabel.interval',1)
+        """
+        self._prop_by_paths.append((path, value))
+        return self
+
+    def _update_props_by_path(self, opts: Dict):
+        for path, value in self._prop_by_paths:
+            echarts_opts_utils.set_prop_by_path(opts, path, value)
+
 
 class ChartCollector:
     def __init__(self) -> None:
         self._collector: List[BaseChart] = []
 
     def append(self, other: BaseChart):
         self._collector.append(other)
```

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/line.py` & `pybi-next-0.4.0/pybi/easyEcharts/line.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 from .base import BaseChart
 import pybi as pbi
 import pybi.utils.sql as sqlUtils
 
 from typing import TYPE_CHECKING, Optional
-from pybi.core.components.reactiveComponent import EChartDatasetInfo
-from .utils import merge_user_options
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
 
 
 class LineChart(BaseChart):
     def __init__(
@@ -69,20 +67,20 @@
         else:
             sql = f"select {self.x},{agg_field} from {self.data} group by {self.x}"
 
         dv = pbi.set_dataView(sql)
 
         if self.color:
             base_opt["series"] = pbi.sql(
-                f"select {self.y},{self.color} from {dv}"
+                f"select {self.x},{self.y},{self.color} from {dv}"
             ).split_group(
                 self.color,
                 """
-                const data = rows.map(r=> r[fields[0]])
-                return {id:key,data,type:'line',name:key}""",
+                const data = rows.map(r=> [r[fields[0]],r[fields[1]]])
+                return {id:key,data,type:'line',name:key,universalTransition: {enabled: true}}""",
             )
         else:
             base_opt["series"].append(
                 {
                     "name": self.x,
                     "id": self.x,
                     "universalTransition": {"enabled": True, "divideShape": "clone"},
@@ -92,19 +90,23 @@
                     ),
                 }
             )
 
         catAxis = base_opt["xAxis"][0]
         valueAxis = base_opt["yAxis"][0]
 
-        catAxis["data"] = pbi.sql(f"select distinct {self.x} from {dv}").toflatlist()
+        catAxis["data"] = pbi.sql(
+            f"select distinct {self.x} from {dv} order by {self.x}"
+        ).toflatlist()
         catAxis.update(self._xAxis)
         # catAxis["axisLabel"] = {"formatter": "{value}月"}
         catAxis["boundaryGap"] = False
         valueAxis["type"] = "value"
 
         opts["tooltip"] = {
             "trigger": "axis",
             "axisPointer": {"type": "cross", "label": {"backgroundColor": "#6a7985"}},
         }
 
-        return base_opt, self._updateInfos
+        self._update_props_by_path(base_opt)
+
+        return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/pie.py` & `pybi-next-0.4.0/pybi/easyEcharts/pie.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 from .base import BaseChart
 import pybi as pbi
 import pybi.utils.sql as sqlUtils
 
 from typing import TYPE_CHECKING, Optional
-from pybi.core.components.reactiveComponent import EChartDatasetInfo
-from .utils import merge_user_options
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
 
 
 class PieChart(BaseChart):
     def __init__(
@@ -76,8 +74,9 @@
 
         series_config["data"] = sql
 
         base_opt["series"].append(series_config)
 
         opts["tooltip"] = {"trigger": "item"}
 
-        return base_opt, self._updateInfos
+        self._update_props_by_path(base_opt)
+        return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.3.9/pybi/easyEcharts/scatter.py` & `pybi-next-0.4.0/pybi/easyEcharts/scatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 from .base import BaseChart
 import pybi as pbi
 
 from typing import TYPE_CHECKING, Optional
-from pybi.core.components.reactiveComponent import EChartDatasetInfo
-from .utils import merge_user_options
-import pybi.utils.sql as sqlUtils
+
 
 if TYPE_CHECKING:
     from pybi.core.dataSource import DataSourceTable
 
 
 class ScatterChart(BaseChart):
     def __init__(
@@ -63,8 +61,9 @@
         else:
             sql = pbi.sql(f"select {self.x},{self.y} from {self.data}").toflatlist()
             series = {"type": "scatter", "symbolSize": 15, "data": sql}
             base_opt["series"].append(series)
 
         opts["tooltip"] = {"trigger": "item"}
 
-        return base_opt, self._updateInfos
+        self._update_props_by_path(base_opt)
+        return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.3.9/pybi/utils/dataSourceUtils.py` & `pybi-next-0.4.0/pybi/utils/dataSourceUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/utils/data_gen.py` & `pybi-next-0.4.0/pybi/utils/data_gen.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import base64
-from datetime import datetime
+import datetime
 from enum import Enum
 from pathlib import Path
-from json import JSONEncoder, dumps
+import simplejson as json
 from functools import partial
-from typing import Callable
+from typing import Callable, Sequence, List, Dict
 import numpy as np
 import pandas as pd
 import inspect
 
 from abc import abstractmethod
-
+import pybi.utils.echarts_opts_utils as echarts_opts_utils
+import pybi.utils.pyecharts_utils as pybi_pyecharts_utils
 
 _global_id = 0
 
 
 class Jsonable:
     @abstractmethod
     def _to_json_dict(self):
@@ -44,56 +45,76 @@
 _m_project_root = Path(__file__).absolute().parent.parent
 
 
 def get_project_root():
     return _m_project_root
 
 
-def _nan2None(obj):
-    if isinstance(obj, dict):
-        return {k: _nan2None(v) for k, v in obj.items()}
-    elif isinstance(obj, list):
-        return [_nan2None(v) for v in obj]
-    elif isinstance(obj, float) and pd.isna(obj):
+def pybi_json_default(obj):
+    if isinstance(obj, float) and pd.isna(obj):
         return None
-    elif isinstance(obj, np.ndarray):
+    if isinstance(obj, np.ndarray):
         return obj.tolist()
-    elif isinstance(obj, datetime):
-        return str(obj)
-    elif isinstance(obj, Enum):
+    if isinstance(obj, (datetime.date, datetime.datetime)):
+        return obj.isoformat()
+    if isinstance(obj, Enum):
         return obj.value
-    elif isinstance(obj, Jsonable):
-        return _nan2None(obj._to_json_dict())
-
-    return obj
-
-
-class _NanConverter(JSONEncoder):
-    def default(self, obj):
-        # possible other customizations here
-        pass
+    if isinstance(obj, Jsonable):
+        return obj._to_json_dict()
 
-    def encode(self, obj, *args, **kwargs):
-        obj = _nan2None(obj)
-        return super().encode(obj, *args, **kwargs)
 
-    def iterencode(self, obj, *args, **kwargs):
-        obj = _nan2None(obj)
-        return super().iterencode(obj, *args, **kwargs)
+class JsonUtils:
+    def __init__(self) -> None:
+        self.json_defalut_fns: List[Callable] = [pybi_json_default]
+
+    def mark_pyecharts(self):
+        if len(self.json_defalut_fns) >= 2:
+            return
+
+        from pyecharts.options.series_options import BasicOpts
+        from pyecharts.commons import utils as pyecharts_utils
+
+        self.json_defalut_fns.append(
+            partial(
+                pybi_pyecharts_utils.pyecharts_json_default,
+                utils=pyecharts_utils,
+                basicOptsType=BasicOpts,
+            )
+        )
+
+    def dumps(self, obj, *args, **kws):
+        def json_default(obj):
+            for fn in self.json_defalut_fns:
+                res = fn(obj)
+                if res is not None:
+                    return res
+
+        return json.dumps(
+            obj, *args, **kws, ignore_nan=True, default=json_default, ensure_ascii=False
+        )
 
 
-json_dumps_fn = partial(dumps, cls=_NanConverter)
+# json_dumps_fn = partial(json.dumps, ignore_nan=True, default=json_default)
 
 
 def data2html_img_src(data: bytes):
     b64 = base64.b64encode(data).decode("utf8")
     value = f"data:image/png;base64,{b64}"
     return value
 
 
+def file2html_base64_src(file: str, format: str):
+
+    with open(file, mode="rb") as f:
+        b64 = base64.b64encode(f.read())
+        b64 = str(b64, "utf8")
+        value = f"data:{format};base64,{b64}"
+        return value
+
+
 class StrEnum(str, Enum):
     def __new__(cls, value, *args, **kwargs):
         return super().__new__(cls, value, *args, **kwargs)
 
     def __str__(self):
         return str(self.value)
```

### Comparing `pybi-next-0.3.9/pybi/utils/dictUtils.py` & `pybi-next-0.4.0/pybi/utils/dictUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/utils/helper.py` & `pybi-next-0.4.0/pybi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/utils/markdown2.py` & `pybi-next-0.4.0/pybi/utils/markdown2.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/pybi/utils/sql.py` & `pybi-next-0.4.0/pybi/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.3.9/setup.py` & `pybi-next-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 #!/usr/bin/env python
 """The setup script."""
 
 from setuptools import setup, find_packages
 import pybi as pbi
+from pathlib import Path
+
+
+def all_static_files():
+    files = [str(p) for p in Path("pybi/static").glob("*.*")]
+    return files
+
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
-requirements = ["pandas"]
+requirements = ["pandas", "simplejson", "jinja2"]
 
-test_requirements = ["pytest>=3", "playwright"]
+test_requirements = ["pytest>=3", "playwright", "pyecharts"]
 
 setup(
     author="carson_jia",
     author_email="568166495@qq.com",
     python_requires=">=3.7",
     classifiers=[
         "Intended Audience :: Developers",
@@ -37,15 +44,19 @@
     packages=find_packages(include=["pybi", "pybi.*"]),
     data_files=[
         (
             "template",
             [
                 "pybi/template/index.html",
             ],
-        )
+        ),
+        (
+            "static",
+            all_static_files(),
+        ),
     ],
     test_suite="__tests",
     tests_require=test_requirements,
     url="",
     version=pbi.__version__,
     zip_safe=False,
 )
```

