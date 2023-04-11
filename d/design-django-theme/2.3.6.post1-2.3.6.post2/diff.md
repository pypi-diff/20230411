# Comparing `tmp/design-django-theme-2.3.6.post1.tar.gz` & `tmp/design-django-theme-2.3.6.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design-django-theme-2.3.6.post1.tar", last modified: Tue Apr 11 07:33:58 2023, max compression
+gzip compressed data, was "design-django-theme-2.3.6.post2.tar", last modified: Tue Apr 11 17:44:38 2023, max compression
```

## Comparing `design-django-theme-2.3.6.post1.tar` & `design-django-theme-2.3.6.post2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.775789 design-django-theme-2.3.6.post1/bootstrap_italia_template/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.771789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.775789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/assets/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2379 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/assets/upload-drag-drop-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.775789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   557772 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia-comuni.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   554420 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   141582 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.771789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.783789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4515 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/OFL.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    30422 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    79827 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    60972 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    30912 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    24832 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    32092 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    87104 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    65292 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    32484 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    26036 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    32479 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    86923 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    64692 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    33032 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    26240 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29889 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    79868 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    61104 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    30488 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    24456 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.787789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11560 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    18048 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    71199 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    31792 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    20292 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16124 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    19986 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    75791 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    34444 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    22448 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    19821 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    75835 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    34372 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    22292 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17776 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    18045 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    71187 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    31812 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    20168 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16116 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.799789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4523 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/OFL.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    22303 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    43644 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    51368 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    24912 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    18212 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    25086 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    48640 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    57652 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    20480 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21905 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    42807 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    50436 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    24568 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    18120 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    25381 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    48410 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    57952 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    28168 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    20568 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20871 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    42820 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    48712 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    23768 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17340 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    24386 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    48288 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    56392 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    27276 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    20196 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    25356 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    48457 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    58376 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    28280 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    20740 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    22122 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    43156 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    51152 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    24856 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    18136 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.803789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.803789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   349666 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/js/bootstrap-italia.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   210429 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/js/bootstrap-italia.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.819789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/accordion.js
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/accordion.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/alert.js
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/alert.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/backToTop.js
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/backToTop.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/button.js
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/button.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel-bi.js
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel-bi.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel.js
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/collapse.js
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/collapse.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/cookiebar.js
--rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/cookiebar.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dimmer.js
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dimmer.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dropdown.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/fonts-loader.js
--rw-r--r--   0 runner    (1001) docker     (123)    19751 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/fonts-loader.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/form-validate.js
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/form-validate.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/forward.js
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/forward.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/header-sticky.js
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/header-sticky.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/history-back.js
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/history-back.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/init.js
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/init.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-label.js
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-label.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-number.js
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-number.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-password.js
--rw-r--r--   0 runner    (1001) docker     (123)    24680 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-password.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-search-autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-search-autocomplete.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input.js
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/list.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/masonry.js
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/masonry.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/modal.js
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/modal.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navbar-collapsible.js
--rw-r--r--   0 runner    (1001) docker     (123)    18849 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navbar-collapsible.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navscroll.js
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navscroll.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/notification.js
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/notification.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/offcanvas.js
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/offcanvas.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/popover.js
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/popover.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/progress-donut.js
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/progress-donut.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/scrollspy.js
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/scrollspy.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/select-autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/select-autocomplete.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/sticky.js
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/sticky.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tab.js
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tab.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/toast.js
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/toast.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tooltip.js
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tooltip.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/track-focus.js
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/track-focus.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/transfer.js
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/transfer.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/upload-dragdrop.js
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/upload-dragdrop.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/device.js
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/device.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/dom.js
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/dom.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/observer.js
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/observer.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/on-document-scroll.js
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/on-document-scroll.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/pageScroll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/pageScroll.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/tween.js
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/tween.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/svg/
--rw-r--r--   0 runner    (1001) docker     (123)    76139 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/static/svg/sprites.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    38330 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/bootstrap-italia-base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/date.html
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/radio.html
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/bootstrap_italia_template/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/templatetags/django_bootstrap_italia.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/bootstrap_italia_template/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/design_django_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-11 07:33:58.000000 design-django-theme-2.3.6.post1/design_django_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-11 07:33:58.000000 design-django-theme-2.3.6.post1/design_django_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:33:58.000000 design-django-theme-2.3.6.post1/design_django_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 07:33:58.000000 design-django-theme-2.3.6.post1/design_django_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 07:33:58.000000 design-django-theme-2.3.6.post1/design_django_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:33:58.823789 design-django-theme-2.3.6.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-11 07:33:41.000000 design-django-theme-2.3.6.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.790610 design-django-theme-2.3.6.post2/bootstrap_italia_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.790610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.790610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2379 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/assets/upload-drag-drop-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.794610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   557772 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia-comuni.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   554420 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   141582 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.790610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.798610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4515 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/OFL.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30422 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79827 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60972 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30912 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24832 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32092 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87104 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65292 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32484 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26036 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32479 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    86923 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64692 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33032 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26240 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29889 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    79868 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61104 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30488 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24456 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.802610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11560 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18048 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71199 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31792 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20292 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16124 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19986 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75791 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34444 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22448 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19821 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75835 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34372 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22292 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17776 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18045 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71187 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31812 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20168 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16116 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.806610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4523 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/OFL.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22303 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43644 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51368 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24912 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18212 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25086 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48640 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57652 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20480 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21905 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42807 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50436 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24568 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18120 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25381 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48410 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57952 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28168 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20568 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20871 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42820 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48712 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23768 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17340 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24386 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48288 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56392 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27276 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20196 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25356 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48457 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58376 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28280 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20740 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22122 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43156 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51152 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24856 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18136 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.810610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.810610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   349666 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/js/bootstrap-italia.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   210429 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/js/bootstrap-italia.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.818610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/accordion.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/accordion.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/alert.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/backToTop.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/backToTop.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/button.js
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/button.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel-bi.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel-bi.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/collapse.js
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/collapse.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/cookiebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/cookiebar.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dimmer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dimmer.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dropdown.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/fonts-loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19751 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/fonts-loader.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/form-validate.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/form-validate.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/forward.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/forward.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/header-sticky.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/header-sticky.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/history-back.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/history-back.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/init.js
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/init.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-label.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-label.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-number.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-number.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-password.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24680 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-password.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-search-autocomplete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-search-autocomplete.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/list.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/masonry.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/masonry.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/modal.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navbar-collapsible.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18849 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navbar-collapsible.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navscroll.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navscroll.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/notification.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/notification.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/offcanvas.js
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/offcanvas.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/popover.js
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/popover.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/progress-donut.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/progress-donut.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/scrollspy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/scrollspy.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/select-autocomplete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/select-autocomplete.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/sticky.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/sticky.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tab.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tab.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/toast.js
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/toast.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tooltip.js
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tooltip.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/track-focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/track-focus.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/transfer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/transfer.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/upload-dragdrop.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/upload-dragdrop.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/device.js
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/device.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/dom.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/observer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/observer.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/on-document-scroll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/on-document-scroll.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/pageScroll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/pageScroll.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/tween.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/tween.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)    76139 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/static/svg/sprites.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38430 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/bootstrap-italia-base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/radio.html
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/bootstrap_italia_template/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/templatetags/django_bootstrap_italia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-11 17:44:29.000000 design-django-theme-2.3.6.post2/bootstrap_italia_template/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/design_django_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-11 17:44:38.000000 design-django-theme-2.3.6.post2/design_django_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14285 2023-04-11 17:44:38.000000 design-django-theme-2.3.6.post2/design_django_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:44:38.000000 design-django-theme-2.3.6.post2/design_django_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 17:44:38.000000 design-django-theme-2.3.6.post2/design_django_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 17:44:38.000000 design-django-theme-2.3.6.post2/design_django_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:44:38.822610 design-django-theme-2.3.6.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-11 17:44:30.000000 design-django-theme-2.3.6.post2/setup.py
```

### Comparing `design-django-theme-2.3.6.post1/LICENSE` & `design-django-theme-2.3.6.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/MANIFEST.in` & `design-django-theme-2.3.6.post2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/PKG-INFO` & `design-django-theme-2.3.6.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design-django-theme
-Version: 2.3.6.post1
+Version: 2.3.6.post2
 Summary: Bootstrap Italia template for Django
 Home-page: https://github.com/italia/design-django-theme
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `design-django-theme-2.3.6.post1/README.md` & `design-django-theme-2.3.6.post2/README.md`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/assets/upload-drag-drop-icon.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/assets/upload-drag-drop-icon.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia-comuni.min.css` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia-comuni.min.css`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia.min.css` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia.min.css`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/css/bootstrap-italia.min.css.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/css/bootstrap-italia.min.css.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/OFL.txt` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/OFL.txt`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Lora/lora-v20-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/LICENSE.txt` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Roboto_Mono/roboto-mono-v13-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/OFL.txt` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/OFL.txt`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.eot` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.eot`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.ttf` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff2` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/fonts/Titillium_Web/titillium-web-v10-latin-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon-16x16.png` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon-32x32.png` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/images/favicon.ico` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/js/bootstrap-italia.bundle.min.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/js/bootstrap-italia.bundle.min.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/js/bootstrap-italia.min.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/js/bootstrap-italia.min.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/accordion.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/accordion.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/accordion.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/accordion.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/backToTop.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/backToTop.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/backToTop.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/backToTop.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel-bi.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel-bi.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/carousel-bi.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/carousel-bi.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/cookiebar.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/cookiebar.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/cookiebar.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/cookiebar.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dimmer.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dimmer.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/dimmer.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/dimmer.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/fonts-loader.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/fonts-loader.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/fonts-loader.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/fonts-loader.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/form-validate.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/form-validate.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/form-validate.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/form-validate.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/forward.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/forward.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/forward.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/forward.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/header-sticky.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/header-sticky.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/header-sticky.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/header-sticky.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/history-back.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/history-back.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/history-back.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/history-back.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/init.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/init.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-label.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-label.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-label.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-label.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-number.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-number.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-number.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-number.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-password.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-password.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-password.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-password.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-search-autocomplete.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-search-autocomplete.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input-search-autocomplete.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input-search-autocomplete.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/input.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/input.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/list.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/list.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/list.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/list.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/masonry.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/masonry.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/masonry.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/masonry.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navbar-collapsible.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navbar-collapsible.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navbar-collapsible.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navbar-collapsible.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navscroll.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navscroll.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/navscroll.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/navscroll.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/notification.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/notification.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/notification.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/notification.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/progress-donut.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/progress-donut.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/progress-donut.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/progress-donut.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/select-autocomplete.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/select-autocomplete.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/select-autocomplete.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/select-autocomplete.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/sticky.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/sticky.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/sticky.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/sticky.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tab.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tab.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/tab.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/tab.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/track-focus.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/track-focus.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/track-focus.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/track-focus.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/transfer.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/transfer.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/transfer.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/transfer.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/upload-dragdrop.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/upload-dragdrop.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/upload-dragdrop.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/upload-dragdrop.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/dom.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/dom.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/dom.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/dom.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/observer.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/observer.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/observer.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/observer.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/on-document-scroll.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/on-document-scroll.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/on-document-scroll.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/on-document-scroll.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/pageScroll.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/pageScroll.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/pageScroll.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/pageScroll.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/tween.js` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/tween.js`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/plugins/util/tween.js.map` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/plugins/util/tween.js.map`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/static/svg/sprites.svg` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/static/svg/sprites.svg`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/bootstrap-italia-base.html` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/bootstrap-italia-base.html`

 * *Files 0% similar despite different names*

```diff
@@ -554,12 +554,15 @@
                 </div>
             </div>
             {% endblock footer_bottom %}
         </footer>
         {% endblock footer %}
 
         <script src="{% django_bootstrap_italia_static_path 'js/bootstrap-italia.bundle.min.js' %}"></script>
+        <script>
+            bootstrap.loadFonts('/bootstrap-italia/dist/fonts');
+        </script>
 
         {% block bottom_scripts %}{% endblock bottom_scripts %}
         {% block extra_scripts %}{% endblock extra_scripts %}
     </body>
 </html>
```

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/formset.html` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/formset.html`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/templates/widgets/radio.html` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/templates/widgets/radio.html`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/templatetags/django_bootstrap_italia.py` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/templatetags/django_bootstrap_italia.py`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/bootstrap_italia_template/widgets.py` & `design-django-theme-2.3.6.post2/bootstrap_italia_template/widgets.py`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/design_django_theme.egg-info/PKG-INFO` & `design-django-theme-2.3.6.post2/design_django_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design-django-theme
-Version: 2.3.6.post1
+Version: 2.3.6.post2
 Summary: Bootstrap Italia template for Django
 Home-page: https://github.com/italia/design-django-theme
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `design-django-theme-2.3.6.post1/design_django_theme.egg-info/SOURCES.txt` & `design-django-theme-2.3.6.post2/design_django_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `design-django-theme-2.3.6.post1/setup.py` & `design-django-theme-2.3.6.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 #  rm -R build/ dist/ *egg-info
 #  python3 setup.py sdist
 #  twine upload dist/*
 
 setup(
     name='design-django-theme',
-    version='v2.3.6-1',
+    version='v2.3.6-2',
     packages=['bootstrap_italia_template', ],
     package_data={'bootstrap_italia_template': ['bootstrap_italia_template/*']},
     include_package_data=True,
     license='Apache 2.0',
     description="Bootstrap Italia template for Django",
     long_description=README,
     long_description_content_type='text/markdown',
```

