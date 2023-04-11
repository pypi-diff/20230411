# Comparing `tmp/unicms_template_unical-1.1.9.tar.gz` & `tmp/unicms_template_unical-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicms_template_unical-1.1.9.tar", last modified: Wed Nov 16 08:34:52 2022, max compression
+gzip compressed data, was "unicms_template_unical-1.2.0.tar", last modified: Tue Apr 11 09:19:33 2023, max compression
```

## Comparing `unicms_template_unical-1.1.9.tar` & `unicms_template_unical-1.2.0.tar`

### file list

```diff
@@ -1,215 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.053993 unicms_template_unical-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.053993 unicms_template_unical-1.1.9/src/unicms_template_unical/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.053993 unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8511 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    22153 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.053993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/_old/
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/_old/unical-portale-v-original.scss
--rw-r--r--   0 runner    (1001) docker     (121)     4660 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/_old/unical-style.scss
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/colors/
--rw-r--r--   0 runner    (1001) docker     (121)     6473 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (121)     6637 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/colors/unicms_unical.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/scss/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/scss/colors/
--rw-r--r--   0 runner    (1001) docker     (121)     7665 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/scss/colors/unicms_exbriner.scss
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/scss/colors/unicms_unical.scss
--rw-r--r--   0 runner    (1001) docker     (121)    10410 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/scss/unicms_unical.scss
--rw-r--r--   0 runner    (1001) docker     (121)     9944 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/unicms_unical.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    43664 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.065993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/addressbook.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10243 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/agenda.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/alert-red.svg
--rw-r--r--   0 runner    (1001) docker     (121)   130694 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/banner_1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8720 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/chi.png
--rw-r--r--   0 runner    (1001) docker     (121)    17329 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12905 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/en.png
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/esp.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.065993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/favicon/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/favicon/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.065993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/ar.svg
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/en.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/es.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/eu.svg
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/fr.svg
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/it.svg
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/pt.svg
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/ru.svg
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/zh.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5936 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/ita.png
--rw-r--r--   0 runner    (1001) docker     (121)   312996 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/library1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    27664 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo1.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_back.svg
--rw-r--r--   0 runner    (1001) docker     (121)    32050 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_presta.svg
--rw-r--r--   0 runner    (1001) docker     (121)    42300 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_unical_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.069993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (121)     2612 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/HRS4R.svg
--rw-r--r--   0 runner    (1001) docker     (121)    24514 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/ctc.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25799 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/demacs.svg
--rw-r--r--   0 runner    (1001) docker     (121)    27889 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/desf.svg
--rw-r--r--   0 runner    (1001) docker     (121)    28678 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dfssn.svg
--rw-r--r--   0 runner    (1001) docker     (121)    23742 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/diam.svg
--rw-r--r--   0 runner    (1001) docker     (121)    27886 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dibest.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25693 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dices.svg
--rw-r--r--   0 runner    (1001) docker     (121)    28422 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dimeg.svg
--rw-r--r--   0 runner    (1001) docker     (121)    31883 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (121)    22720 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dinci.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25608 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/discag.svg
--rw-r--r--   0 runner    (1001) docker     (121)    25944 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dispes.svg
--rw-r--r--   0 runner    (1001) docker     (121)    23078 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/disu.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5331 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/exbriner.png
--rw-r--r--   0 runner    (1001) docker     (121)    20713 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/fis.svg
--rw-r--r--   0 runner    (1001) docker     (121)   473786 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/master_ges.png
--rw-r--r--   0 runner    (1001) docker     (121)   356948 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   441153 2022-11-16 08:34:41.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   422058 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news3.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   126770 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   508364 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_banner.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    23187 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.069993 unicms_template_unical-1.1.9/src/unicms_template_unical/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/js/external_link_new_tab.js
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/static/js/unicms_api_utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.069993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.069993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/base_v_original.html
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/error-page.html
--rw-r--r--   0 runner    (1001) docker     (121)     4443 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/unical_api_list.html
--rw-r--r--   0 runner    (1001) docker     (121)    33255 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/unicms_unical.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.077993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
--rw-r--r--   0 runner    (1001) docker     (121)     5974 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
--rw-r--r--   0 runner    (1001) docker     (121)     3804 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_contact.html
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
--rw-r--r--   0 runner    (1001) docker     (121)     5717 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
--rw-r--r--   0 runner    (1001) docker     (121)     1685 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
--rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_main.html
--rw-r--r--   0 runner    (1001) docker     (121)     3871 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_side.html
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_links.html
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_card.html
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
--rw-r--r--   0 runner    (1001) docker     (121)     8239 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)     9756 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.057993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.077993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_1/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.077993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_2/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.077993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_3/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.077993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/inits/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/inits/brython-init.html
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/loading-jumbo.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     8495 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department.html
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_ctc.html
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_demacs.html
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_desf.html
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dfssn.html
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_diam.html
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dibest.html
--rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dices.html
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dimeg.html
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dimes.html
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dinci.html
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_discag.html
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dispes.html
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_disu.html
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_fis.html
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/master_ges.html
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/multi_language.html
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/opendata.html
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_v_original.html
--rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/project_exbriner.html
--rw-r--r--   0 runner    (1001) docker     (121)    15513 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_list.html
--rw-r--r--   0 runner    (1001) docker     (121)    12280 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_view.html
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/unical.html
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/unical_right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/src/unicms_template_unical/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-11-16 08:34:42.000000 unicms_template_unical-1.1.9/src/unicms_template_unical/templatetags/unicms_template_unical.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 08:34:52.081993 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-16 08:34:52.000000 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11844 2022-11-16 08:34:52.000000 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 08:34:52.000000 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-16 08:34:52.000000 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-16 08:34:52.000000 unicms_template_unical-1.1.9/unicms_template_unical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_unical.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/unicms_unical.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.491947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/addressbook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/agenda.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/alert-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130694 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/banner_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/chi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/en.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/esp.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.491947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.495947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/en.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/es.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/eu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/it.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/pt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/zh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ita.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312996 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/library1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32050 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_presta.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_unical_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.495947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/HRS4R.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/ctc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/demacs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/desf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dfssn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/diam.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27886 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dibest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dices.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dinci.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/discag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dispes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/disu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106385 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/exbriner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/fis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   473786 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/master_ges.png
+-rw-r--r--   0 runner    (1001) docker     (123)   356948 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   441153 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   422058 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   126770 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   508364 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_banner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/external_link_new_tab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/unicms_api_utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/base_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/error-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unical_api_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32264 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unicms_unical.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/inits/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/inits/brython-init.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/loading-jumbo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_ctc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_demacs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_desf.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dfssn.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_diam.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dibest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dices.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimeg.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dinci.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_discag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dispes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_disu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_fis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/master_ges.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/multi_language.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/opendata.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/project_exbriner.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/unicms_template_unical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/top_level.txt
```

### Comparing `unicms_template_unical-1.1.9/LICENSE` & `unicms_template_unical-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/PKG-INFO` & `unicms_template_unical-1.2.0/unicms_template_unical.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: unicms_template_unical
-Version: 1.1.9
+Name: unicms-template-unical
+Version: 1.2.0
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `unicms_template_unical-1.1.9/setup.py` & `unicms_template_unical-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  twine upload dist/*
 
 SRC_FOLDER = 'src'
 PKG_NAME = 'unicms_template_unical'
 
 setup(
     name=PKG_NAME,
-    version='1.1.9',
+    version='1.2.0',
 
     packages=[PKG_NAME],
     package_dir={PKG_NAME: f"{SRC_FOLDER}/{PKG_NAME}"},
 
     package_data={PKG_NAME: [i.replace(f'{SRC_FOLDER}/{PKG_NAME}/', '')
                                    for i in glob(f'{SRC_FOLDER}/{PKG_NAME}/**',
                                                  recursive=True)]
@@ -35,14 +35,15 @@
     author='Giuseppe De Marco, Francesco Filicetti',
     author_email='giuseppe.demarco@unical.it, francesco.filicetti@unical.it',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 2.0',
         'Framework :: Django :: 3.0',
+        'Framework :: Django :: 4.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     install_requires=[
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo` & `unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po` & `unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/css/unicms_unical.css` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/unicms_unical.css`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/addressbook.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/addressbook.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/agenda.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/agenda.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/alert-red.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/alert-red.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/banner_1.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/banner_1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/chi.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/chi.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/dimes.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/en.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/en.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/esp.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/esp.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/ar.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ar.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/en.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/en.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/es.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/es.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/eu.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/eu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/flags/zh.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/zh.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/ita.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ita.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/library1.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/library1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo1.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_back.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_presta.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_presta.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_unical_white.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_unical_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logo_white.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/HRS4R.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/HRS4R.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/ctc.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/ctc.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/demacs.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/demacs.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/desf.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/desf.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dfssn.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dfssn.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/diam.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/diam.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dibest.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dibest.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dices.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dices.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dimeg.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimeg.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dimes.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dinci.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dinci.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/discag.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/discag.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/dispes.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dispes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/disu.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/disu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/exbriner.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/exbriner.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/fis.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/fis.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/logos/master_ges.png` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/master_ges.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news1.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news2.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news2.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/news3.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news3.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/ponte-bucci-1.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ponte-bucci-1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_banner.jpg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_logo.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg` & `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/404.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/404.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/base_v_original.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/base_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/error-page.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/error-page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/unical_api_list.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unical_api_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/bases/unicms_unical.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unicms_unical.html`

 * *Files 8% similar despite different names*

```diff
@@ -28,35 +28,21 @@
     <link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/colors/unicms_unical.css' %}" type="text/css">
     {% endblock custom_style %}
 
     {% block head_inits %}
         {{ block.super }}
     {% endblock head_inits %}
 
+    {% block html_head %}
+        {{ block.super }}
+    {% endblock html_head %}
+
     {% block social_tags %}
-    <meta property="og:url" content="{{ request.build_absolute_uri }}" />
-    <meta property="og:type" content="article" />
-    <meta property="og:title" content="{{ page.title }}" />
-    <meta property="og:description" content="{{ page.description }}" />
-    <meta property="og:image" content="https://{{ request.get_host }}/static/images/logo.png">
-    <meta property="og:image:alt" content="{{ page.title }}" />
-    <meta property="og:image:width" content="330" />
-    <meta property="og:image:height" content="330" />
-
-    <meta name="twitter:card" content="summary_large_image">
-    <meta name="twitter:title" content="{{ page.title }}">
-    <meta name="twitter:description" content="{{ page.description }}">
-    <meta name="twitter:image" content="https://{{ request.get_host }}/static/images/logo.png">
-    <meta name="twitter:image:alt" content="{{ page.title }}">
+        {{ block.super }}
     {% endblock social_tags %}
-
-    {% block analytics_value %}
-        {% settings_value "ANALYTICS_CODE" as analytics_code %}
-        {{ analytics_code|safe }}
-    {% endblock analytics_value %}
 {% endblock extra_head %}
 
 <!-- Meta Description (for all pages if not overrided) -->
 {% block page_meta_description %}{% if webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans "Official University of Calabria website" %}{% endif %}{% endblock page_meta_description %}
 {% block page_meta_keywords %}{% if webpath.meta_keywords %}{{ webpath.meta_keywords }}{% else %}UniCal{% endif %}{% endblock page_meta_keywords %}
 
 {% block header_brand_wrapper %}
@@ -257,17 +243,14 @@
                 </a>
             </div>
         </div>
     </div>
 </div>
 {% endblock unical_header_languages %}
 
-{% load_blocks section='head' as head %}
-{{ head }}
-
 <div class="it-header-navbar-wrapper">
     <div class="container">
         <div class="row">
             <div class="col-12">
                 <nav class="navbar navbar-expand-lg has-megamenu" aria-label="{% trans 'Main menu' %}">
                     <button class="custom-navbar-toggler"
                             type="button"
@@ -345,15 +328,15 @@
             <a class="p-2" href="https://www.instagram.com/unical_official/" target="_blank" rel="noopener noreferrer" title="Instagram">
                 <svg class="icon icon-secondary align-top">
                     <use xlink:href="{% static 'svg/sprites.svg' %}#it-instagram"></use>
                 </svg><span class="visually-hidden">Instagram</span>
             </a>
         </li>
         <li class="list-inline-item">
-            <a class="p-2" href="https://www.youtube.com/channel/UCnd5Oen95TMO9aLfVRUAABQ" target="_blank" rel="noopener noreferrer" title="YouTube">
+            <a class="p-2" href="https://www.youtube.com/@campusunical" target="_blank" rel="noopener noreferrer" title="YouTube">
                 <svg class="icon icon-secondary align-top">
                     <use xlink:href="{% static 'svg/sprites.svg' %}#it-youtube"></use>
                 </svg><span class="visually-hidden">Youtube</span>
             </a>
         </li>
         <li class="list-inline-item">
             <a class="p-2" href="https://github.com/UniversitaDellaCalabria" target="_blank" rel="noopener noreferrer" title="Github">
@@ -408,16 +391,16 @@
             <div class="link-list-wrapper">
                 <ul class="footer-list link-list clearfix">
                     <li><a class="list-item" href="/front-office/" title="{% trans 'Online front-office' %}">{% trans 'Online front-office' %}</a></li>
                     <li><a class="list-item" href="https://ticket.unical.it/" target="_blank" rel="noopener noreferrer" title="{% trans 'Online ticket' %}">{% trans 'Online ticket' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict" title="{% trans 'ITC Services' %}">{% trans 'ITC Services' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict/servizi-digitali-studenti/accesso-wifi-ateneo/" title="{% trans 'Wi-Fi Services' %}">{% trans 'Wi-Fi Services' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict/servizi-digitali-studenti/posta-elettronica-studenti/" title="{% trans 'Students webmail' %}">{% trans 'Students webmail' %}</a></li>
-                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-utente/posta-elettronica/" title="{% trans 'Employees webmail' %}">{% trans 'Employees webmail' %}</a></li>
-                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-utente/credenziali-di-ateneo/" title="{% trans 'SPID / UniCal ID' %}">{% trans 'SPID / UniCal ID' %}</a></li>
+                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-per-il-personale/posta-elettronica/" title="{% trans 'Employees webmail' %}">{% trans 'Employees webmail' %}</a></li>
+                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-studenti/credenziali-di-ateneo/" title="{% trans 'SPID / UniCal ID' %}">{% trans 'SPID / UniCal ID' %}</a></li>
                     <li><a class="list-item" href="/didattica/iscriversi-studiare-laurearsi/tasse-ed-esoneri/" title="{% trans 'Online Taxes / PagoPA' %}">{% trans 'Online Taxes / PagoPA' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict/servizi-digitali-studenti/esse3-web/" title="{% trans 'Exam reservations - ESSE3' %}">{% trans 'Exam reservations - ESSE3' %}</a></li>
                     <li><a class="list-item" href="https://www.unical.it/esse3pa" target="_blank" rel="noopener noreferrer" title="{% trans 'ESSE3PA' %}">{% trans 'ESSE3PA' %}</a></li>
                     <li><a class="list-item" href="https://24cfu.unical.it/elearning/" target="_blank" rel="noopener noreferrer" title="{% trans 'e-Learning platform' %}">{% trans 'e-Learning platform' %}</a></li>
                     <li><a class="list-item" href="/web-radio" title="{% trans 'Web Radio' %}">{% trans 'Web Radio' %}</a></li>
                     <li><a class="list-item" href="/unical-magazine/" title="{% trans 'Online Magazine' %}">{% trans 'Online Magazine' %}</a></li>
                 </ul>
```

#### html2text {}

```diff
@@ -2,32 +2,19 @@
 {% load unicms_carousels %} {% load unicms_contexts %} {% load unicms_menus %}
 {% load unicms_templates %} {% load unicms_pages %} {% load unicms_publications
 %} {% load unicms_template_unical %}  {% block extra_head %} {% block
 custom_style %}
 
 
  {% endblock custom_style %} {% block head_inits %} {{ block.super }} {%
-endblock head_inits %} {% block social_tags %}
-
-
-
-
-
-
-
-
-
-
-
-
- {% endblock social_tags %} {% block analytics_value %} {% settings_value
-"ANALYTICS_CODE" as analytics_code %} {{ analytics_code|safe }} {% endblock
-analytics_value %} {% endblock extra_head %}  {% block page_meta_description %}
-{% if webpath.meta_description %}{{ webpath.meta_description }}{% else %}{%
-trans "Official University of Calabria website" %}{% endif %}{% endblock
+endblock head_inits %} {% block html_head %} {{ block.super }} {% endblock
+html_head %} {% block social_tags %} {{ block.super }} {% endblock social_tags
+%} {% endblock extra_head %}  {% block page_meta_description %}{% if
+webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans
+"Official University of Calabria website" %}{% endif %}{% endblock
 page_meta_description %} {% block page_meta_keywords %}{% if
 webpath.meta_keywords %}{{ webpath.meta_keywords }}{% else %}UniCal{% endif %}
 {% endblock page_meta_keywords %} {% block header_brand_wrapper %}
 {{ block.super }}
 {% endblock header_brand_wrapper %}  {% block header_center_logo %}
 
 {% endblock header_center_logo %} {% block header_brand_text %} {% endblock
@@ -59,16 +46,15 @@
 {% endcomment %}
 {% endblock header_center_right_zone %}  {% block main_menu %} {% block
 unical_header_languages %}
 {% language_menu as language_urls %} {% for cod,params in language_urls.items
 %} {% load_lang_flag cod as flag_path %} [{{_params.0_}}] {% endfor %} [{%
 trans_'Chinese'_%}] [{%_trans_'French'_%}] [{%_trans_'Portuguese'_%}] [{%_trans
 'Espanol'_%}] [{%_trans_'Arabic'_%}] [{%_trans_'Russian'_%}]
-{% endblock unical_header_languages %} {% load_blocks section='head' as head %}
-{{ head }}
+{% endblock unical_header_languages %}
 
      {% trans "Close" %}
     * {% block menu_main %}  {% load_blocks section='menu-1' as main_menu %} {
       { main_menu }} {% endblock menu_main %}
 {% endblock main_menu %} {% block section_2_classes %} dark-grey-background py-
 5 {% endblock section_2_classes %} {% block footer_top_section %} {% endblock
 footer_top_section %} {% block footer_top %}
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_contact.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_contact_v2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_main.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_side.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_alert.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_alert.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         //itemsDesktop : false,
         //itemsDesktopSmall : false,
         //itemsTablet: false,
         //itemsMobile : false,
         dots: false,
         margin: 12,
         //dotsEach: false,
-        stagePadding: 1,
+        stagePadding: 0,
 
         responsive : {
             // breakpoint from 0 up
             0 : {
                 items: 1
             },
             // breakpoint from 480 up
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_card.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_card.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         //itemsDesktop : false,
         //itemsDesktopSmall : false,
         //itemsTablet: false,
         //itemsMobile : false,
         dots: false,
         margin: 12,
         //dotsEach: false,
-        stagePadding: 1,
+        stagePadding: 0,
 
         responsive : {
             // breakpoint from 0 up
             0 : {
                 items: 1
             },
             // breakpoint from 480 up
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/loading-jumbo.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/loading-jumbo.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_ctc.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_ctc.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_demacs.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_demacs.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_desf.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_desf.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dfssn.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dfssn.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_diam.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_diam.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dibest.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dibest.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dices.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dices.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dimeg.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimeg.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dimes.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dinci.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dinci.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 {% load unicms_menus %}
 {% load unicms_templates %}
 {% load unicms_pages %}
 {% load unicms_publications %}
 {% load unicms_template_unical %}
 
 
-{% block analytics_value %}
-    {% settings_value "ANALYTICS_CODE_DINCI" as analytics_code %}
-    {{ analytics_code|safe }}
-{% endblock analytics_value %}
-
 <!-- Logo in Header -->
 {% block header_center_logo_side %}
 <image src="{% unicms_template_unical_static_path 'images/logos/dinci.svg' %}" class="h-100" />
 {% endblock header_center_logo_side %}
 
 {% block header_slim_mobile_org_name_side %}
 <image src="{% unicms_template_unical_static_path 'images/logos/dinci.svg' %}" class="mw-100" />
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_discag.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_discag.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_dispes.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dispes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_disu.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_disu.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/department_fis.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_fis.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/master_ges.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/master_ges.html`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 {% load unicms_menus %}
 {% load unicms_templates %}
 {% load unicms_pages %}
 {% load unicms_publications %}
 {% load unicms_template_unical %}
 
 
-{% block analytics_value %}
-    {% settings_value "ANALYTICS_CODE_DINCI" as analytics_code %}
-    {{ analytics_code|safe }}
-{% endblock analytics_value %}
-
 {% block header_center_url %}
 /didattica/offerta-formativa/master-e-alta-formazione/master/manager-di-impianti-ed-eventi-sportivi-complessi/
 {% endblock header_center_url %}
 
 {% block header_mobile_center_url %}
 /didattica/offerta-formativa/master-e-alta-formazione/master/manager-di-impianti-ed-eventi-sportivi-complessi/
 {% endblock header_mobile_center_url %}
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/multi_language.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/multi_language.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/opendata.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/opendata.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/portale_home_v_original.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/project_exbriner.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/project_exbriner.html`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 {% load unicms_contexts %}
 {% load unicms_menus %}
 {% load unicms_templates %}
 {% load unicms_pages %}
 {% load unicms_publications %}
 {% load unicms_template_unical %}
 
+
+{% block analytics_value %}
+{% endblock analytics_value %}
+
 {% block custom_style %}
 <link rel="shortcut icon" href="{% unicms_template_unical_static_path 'images/favicon/favicon-32x32.png' %}">
 <link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/unicms_unical.css' %}" type="text/css">
 <link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/colors/unicms_exbriner.css' %}" type="text/css">
 {% endblock custom_style %}
 
 {% block page_meta_description %}{% if webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans "EXBRINER Project (Horizon Europe/Marie Skłodowska-Curie Actions/Doctoral Networks, call: HORIZON-MSCA-2021-DN-01)" %}{% endif %}{% endblock page_meta_description %}
@@ -24,82 +28,74 @@
 {% block header_slim_wrapper %}
 {% settings_value "MAIN_DOMAIN" as cms_main_domain %}
 <div class="it-header-slim-wrapper">
     <div class="container">
         <div class="row">
             <div class="col-12">
                 <div class="it-header-slim-wrapper-content">
-                    <a target="_blank" href="//{{ cms_main_domain }}" title="Exbriner" alt="exbriner.unical.it">
-                        <b>UniCal.it</b>
-                    </a>
+                    <small class="text-white">Call HORIZON – MSCA – 2021 – DN - Start Date 2022 | 10 | 01</small>
                     {% if request.user.is_staff %}
                     {% include "components/italia_editorialboard_frontend_menu.html" %}
                     {% endif %}
                 </div>
             </div>
         </div>
     </div>
 </div>
 <a href="/" aria-label="{% trans 'University of Calabria' %}">
     <div class="it-header-center-wrapper d-lg-none h-auto pt-4">
         {% block unical_mobile_logo %}
             {% block header_slim_mobile_org_name_side %}
+            <div class="col-5">
                 <image src="{% unicms_template_unical_static_path 'images/logos/exbriner.png' %}" class="mw-100" />
+            </div>
+            <div class="col-5 offset-2">
+                <image src="{% unicms_template_unical_static_path 'images/logos/eu_funded.svg' %}" class="mw-100" />
+            </div>
             {% endblock header_slim_mobile_org_name_side %}
         {% endblock unical_mobile_logo %}
     </div>
 </a>
 {% endblock header_slim_wrapper %}
 
 {% block header_center_right_zone %}
-
-{% settings_value "CMS_PATH_PREFIX" as cms_path_prefix %}
-
-<div class="it-right-zone col-12 col-lg-5 offset-lg-1">
+<div class="it-right-zone col-12 col-lg-4 d-none d-lg-block">
     <div class="row w-100">
         <div class="col-2 offset-10 offset-md-2 col-md-10">
-
-            {% settings_value "CMS_PATH_PREFIX" as cms_path_prefix %}
-            <a href='/{{ cms_path_prefix }}search/' aria-label="{% trans 'Search' %}">
-                <svg class="icon d-md-none icon-sm icon-light" aria-labelledby="search_mobile">
-                    <title id="search_mobile">
-                        {% trans 'Search' %}
-                    </title>
-                    <use xlink:href="{% static 'svg/sprites.svg' %}#it-search"></use>
-                </svg>
-            </a>
-            <div class="row d-none d-md-flex">
-                <div class="col-2 col-lg-3 text-end">
-                    <svg class="icon icon-md icon-light" aria-labelledby="search">
-                        <title id="search">
-                            {% trans 'Search' %}
-                        </title>
-                        <use xlink:href="{% static 'svg/sprites.svg' %}#it-search"></use>
-                    </svg>
-                </div>
-                <div class="col-9">
-                    <input id="search-engine-input" type="text" placeholder="{% trans 'Search' %}..." class="top-input" />
-                </div>
-            </div>
+            <image src="{% unicms_template_unical_static_path 'images/logos/eu_funded.svg' %}" class="mw-100" />
         </div>
     </div>
 </div>
 {% endblock header_center_right_zone %}
 
 <!-- Logo in Header -->
-{% block header_center_logo_side %}
-<image src="{% unicms_template_unical_static_path 'images/logos/exbriner.png' %}" class="h-100" />
-{% endblock header_center_logo_side %}
+{% block header_brand_wrapper %}
+<div class="it-brand-wrapper col-lg-4 col-12">
+    <a href="{% block header_center_url %}#{% endblock header_center_url %}">
+        {% block header_center_logo %}
+        <div class="d-none d-lg-flex col-lg-12 px-0 department_logo_lg">
+            {% block header_center_logo_side %}
+            <image src="{% unicms_template_unical_static_path 'images/logos/exbriner.png' %}" class="h-100" />
+            {% endblock header_center_logo_side %}
+        </div>
+        {% endblock header_center_logo %}
+
+        {% block header_brand_text %}
+        {% endblock header_brand_text %}
+    </a>
+</div>
+{% endblock header_brand_wrapper %}
 
 {% block unical_header_languages %}
-<div class="py-2 bordeaux-unical-bg">
-    <div class="container text-center">
+<div class="dark-grey-background py-2">
+    <div class="text-center px-3">
         <div class="row">
-            <div class="col white-unical-color">
-                Call HORIZON – MSCA – 2021 – DN - Start Date 2022 | 10 | 01
+            <div class="col">
+                <b>Next-generation membrane technologies for sustainable exploitation of
+    seawater brine resources: transition towards a circular blue industry</b>
             </div>
         </div>
     </div>
 </div>
 {% endblock unical_header_languages %}
 
 {% block department_contacts %}
@@ -125,55 +121,48 @@
 </div>
 {% endblock department_contacts %}
 
 {% block footer_top %}
 <div class="container text-center text-lg-start">
     <ul class="list-inline social py-4 mt-2 mb-0">
         <li class="list-inline-item">
-            <a class="p-2" href="#" target="_blank" rel="noopener noreferrer" title="Facebook">
+            <a class="p-2" href="https://www.facebook.com/profile.php?id=100088359406451" target="_blank" rel="noopener noreferrer" title="Facebook">
                 <svg class="icon icon-secondary align-top">
                     <use xlink:href="{% static 'svg/sprites.svg' %}#it-facebook-square"></use>
                 </svg><span class="visually-hidden">Facebook</span>
             </a>
         </li>
         <li class="list-inline-item">
-            <a class="p-2" href="#" target="_blank" rel="noopener noreferrer" title="Instagram">
+            <a class="p-2" href="https://www.instagram.com/exbriner_eu/" target="_blank" rel="noopener noreferrer" title="Instagram">
                 <svg class="icon icon-secondary align-top">
                     <use xlink:href="{% static 'svg/sprites.svg' %}#it-instagram"></use>
                 </svg><span class="visually-hidden">Instagram</span>
             </a>
         </li>
         <li class="list-inline-item">
-            <a class="p-2" href="#" target="_blank" rel="noopener noreferrer" title="Twitter">
+            <a class="p-2" href="https://twitter.com/exbriner" target="_blank" rel="noopener noreferrer" title="Twitter">
                 <svg class="icon icon-secondary align-top">
                     <use xlink:href="{% static 'svg/sprites.svg' %}#it-twitter"></use>
                 </svg><span class="visually-hidden">Twitter</span>
             </a>
         </li>
-        <li class="list-inline-item">
-            <a class="p-2" href="#" target="_blank" rel="noopener noreferrer" title="YouTube">
-                <svg class="icon icon-secondary align-top">
-                    <use xlink:href="{% static 'svg/sprites.svg' %}#it-youtube"></use>
-                </svg><span class="visually-hidden">Youtube</span>
-            </a>
-        </li>
     </ul>
 </div>
 {% endblock footer_top %}
 
 {% block footer_bottom %}
 <div class="it-footer-main clearfix py-4 border-white border-top unical-secondary-footer">
     <div class="container">
         <section>
             {% block footer_bottom_content %}
             <div class="row">
-                <div class="col-2 col-md-1">
-                    <img src="{% static 'images/flags/eu.svg' %}" alt="EU" height="40" />
+                <div class="col-12 col-lg-2">
+                    <img src="{% unicms_template_unical_static_path 'images/logos/eu_funded_white.svg' %}" alt="EU" height="40" />
                 </div>
-                <div class="col-10 col-md-11">
+                <div class="col-12 col-lg-10 mt-3 mt-lg-0">
                     The project EXBRINER — HORIZON-MSCA-DN-2021 has received funding
                     from the European Union’s Horizon Europe research and innovation programme
                     under the Marie Sklodowska-Curie grant agreement No 101072449.
                 </div>
             </div>
             {% endblock footer_bottom_content %}
         </section>
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
 {% extends "department.html" %} {% load i18n %} {% load static %}  {% load
 unicms_carousels %} {% load unicms_contexts %} {% load unicms_menus %} {% load
 unicms_templates %} {% load unicms_pages %} {% load unicms_publications %} {%
-load unicms_template_unical %} {% block custom_style %}
+load unicms_template_unical %} {% block analytics_value %} {% endblock
+analytics_value %} {% block custom_style %}
 
 
  {% endblock custom_style %} {% block page_meta_description %}{% if
 webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans
 "EXBRINER Project (Horizon Europe/Marie SkÅodowska-Curie Actions/Doctoral
 Networks, call: HORIZON-MSCA-2021-DN-01)" %}{% endif %}{% endblock
 page_meta_description %} {% block page_meta_keywords %}{% if
 webpath.meta_keywords %}{{ webpath.meta_keywords }}{% else %}ExBrineR{% endif
 %}{% endblock page_meta_keywords %} {% block header_slim_wrapper %} {%
 settings_value "MAIN_DOMAIN" as cms_main_domain %}
-UniCal.it {% if request.user.is_staff %} {% include "components/
+Call HORIZON â MSCA â 2021 â DN - Start Date 2022 | 10 | 01 {% if
+request.user.is_staff %} {% include "components/
 italia_editorialboard_frontend_menu.html" %} {% endif %}
-{%_block_unical_mobile_logo_%}_{%_block_header_slim_mobile_org_name_side_%}__{%
-endblock_header_slim_mobile_org_name_side_%}_{%_endblock_unical_mobile_logo_%}
- {% endblock header_slim_wrapper %} {% block header_center_right_zone %} {%
-settings_value "CMS_PATH_PREFIX" as cms_path_prefix %}
-{% settings_value "CMS_PATH_PREFIX" as cms_path_prefix %}
-
-
-[                    ]
-{% endblock header_center_right_zone %}  {% block header_center_logo_side %}
-{% endblock header_center_logo_side %} {% block unical_header_languages %}
-Call HORIZON â MSCA â 2021 â DN - Start Date 2022 | 10 | 01
+{%_block_unical_mobile_logo_%}_{%_block_header_slim_mobile_org_name_side_%}
+{%_endblock_header_slim_mobile_org_name_side_%}_{%_endblock_unical_mobile_logo
+%}
+ {% endblock header_slim_wrapper %} {% block header_center_right_zone %}
+{% endblock header_center_right_zone %}  {% block header_brand_wrapper %}
+{%_block_header_center_logo_%}
+{%_block_header_center_logo_side_%}__{%_endblock_header_center_logo_side_%}
+{%_endblock_header_center_logo_%}_{%_block_header_brand_text_%}_{%_endblock
+header_brand_text_%}
+{% endblock header_brand_wrapper %} {% block unical_header_languages %}
+Next-generation membrane technologies for sustainable exploitation of seawater
+brine resources: transition towards a circular blue industry
 {% endblock unical_header_languages %} {% block department_contacts %}
 Via P. Bucci
 87036 Arcavacata di Rende (CS)
 dipartimento.desf@pec.unical.it
 protocollo.desf@unical.it
 +39 0984 492434
 +39 0984 492422
 {% endblock department_contacts %} {% block footer_top %}
     * __Facebook
     * __Instagram
     * __Twitter
-    * __Youtube
 {% endblock footer_top %} {% block footer_bottom %}
  {% block footer_bottom_content %}
 [EU]
 The project EXBRINER â HORIZON-MSCA-DN-2021 has received funding from the
 European Unionâs Horizon Europe research and innovation programme under the
 Marie Sklodowska-Curie grant agreement No 101072449.
 {% endblock footer_bottom_content %}
```

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_list.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_view.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templates/pages/publication_view_hero_original.html` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view_hero_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/src/unicms_template_unical/templatetags/unicms_template_unical.py` & `unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/unicms_template_unical.py`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.1.9/unicms_template_unical.egg-info/SOURCES.txt` & `unicms_template_unical-1.2.0/unicms_template_unical.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 setup.py
 src/unicms_template_unical/__init__.py
 src/unicms_template_unical/apps.py
 src/unicms_template_unical/settings.py
 src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
 src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
 src/unicms_template_unical/static/css/unicms_unical.css
-src/unicms_template_unical/static/css/_old/unical-portale-v-original.scss
-src/unicms_template_unical/static/css/_old/unical-style.scss
 src/unicms_template_unical/static/css/colors/unicms_exbriner.css
 src/unicms_template_unical/static/css/colors/unicms_unical.css
-src/unicms_template_unical/static/css/scss/unicms_unical.scss
-src/unicms_template_unical/static/css/scss/colors/unicms_exbriner.scss
-src/unicms_template_unical/static/css/scss/colors/unicms_unical.scss
 src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
 src/unicms_template_unical/static/images/addressbook.svg
 src/unicms_template_unical/static/images/agenda.jpg
 src/unicms_template_unical/static/images/alert-red.svg
 src/unicms_template_unical/static/images/banner_1.jpg
 src/unicms_template_unical/static/images/chi.png
 src/unicms_template_unical/static/images/dimes.svg
@@ -61,14 +56,16 @@
 src/unicms_template_unical/static/images/logos/dices.svg
 src/unicms_template_unical/static/images/logos/dimeg.svg
 src/unicms_template_unical/static/images/logos/dimes.svg
 src/unicms_template_unical/static/images/logos/dinci.svg
 src/unicms_template_unical/static/images/logos/discag.svg
 src/unicms_template_unical/static/images/logos/dispes.svg
 src/unicms_template_unical/static/images/logos/disu.svg
+src/unicms_template_unical/static/images/logos/eu_funded.svg
+src/unicms_template_unical/static/images/logos/eu_funded_white.svg
 src/unicms_template_unical/static/images/logos/exbriner.png
 src/unicms_template_unical/static/images/logos/fis.svg
 src/unicms_template_unical/static/images/logos/master_ges.png
 src/unicms_template_unical/static/js/external_link_new_tab.js
 src/unicms_template_unical/static/js/unicms_api_utils.js
 src/unicms_template_unical/templates/404.html
 src/unicms_template_unical/templates/500.html
@@ -129,18 +126,22 @@
 src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
 src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
 src/unicms_template_unical/templates/blocks/unical_publications_card.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
+src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
+src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
 src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
+src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
+src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
 src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
 src/unicms_template_unical/templates/grid/section_1/right_spaced.html
 src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
 src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
 src/unicms_template_unical/templates/grid/section_2/right_spaced.html
 src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
 src/unicms_template_unical/templates/grid/section_3/right_spaced.html
```

