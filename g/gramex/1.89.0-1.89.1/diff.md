# Comparing `tmp/gramex-1.89.0.tar.gz` & `tmp/gramex-1.89.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.89.0.tar", last modified: Mon Apr 10 11:35:33 2023, max compression
+gzip compressed data, was "gramex-1.89.1.tar", last modified: Mon Apr 10 12:42:28 2023, max compression
```

## Comparing `gramex-1.89.0.tar` & `gramex-1.89.1.tar`

### file list

```diff
@@ -1,409 +1,409 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.906995 gramex-1.89.0/
--rw-rw-rw-   0        0        0     1900 2023-04-10 11:33:47.000000 gramex-1.89.0/.gitignore
--rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.89.0/LICENSE
--rw-rw-rw-   0        0        0      620 2022-11-23 04:49:14.000000 gramex-1.89.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2956 2023-04-10 11:35:33.907982 gramex-1.89.0/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.89.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.799382 gramex-1.89.0/gramex/
--rw-rw-rw-   0        0        0    15368 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.89.0/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.859141 gramex-1.89.0/gramex/apps/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.89.0/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.864148 gramex-1.89.0/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.89.0/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-01-03 16:10:30.000000 gramex-1.89.0/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.895164 gramex-1.89.0/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      269 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/admin2/.eslintrc.js
--rw-rw-rw-   0        0        0      226 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/admin2/.snyk
--rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.89.0/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12257 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0    12293 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/admin2/package-lock.json
--rw-rw-rw-   0        0        0      132 2022-02-19 10:03:02.000000 gramex-1.89.0/gramex/apps/admin2/package.json
--rw-rw-rw-   0        0        0      231 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/admin2/rollup.config.js
--rw-rw-rw-   0        0        0     4919 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/admin2/schedule.js
--rw-rw-rw-   0        0        0     2505 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/admin2/schedule.src.js
--rw-rw-rw-   0        0        0     3037 2022-02-19 10:03:02.000000 gramex-1.89.0/gramex/apps/admin2/schedule.template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.911701 gramex-1.89.0/gramex/apps/capture/
--rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12034 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0   141593 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-02-08 17:06:15.000000 gramex-1.89.0/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.937709 gramex-1.89.0/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.89.0/gramex/apps/filemanager/.snyk
--rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.89.0/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.89.0/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.89.0/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.89.0/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.692010 gramex-1.89.0/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.972745 gramex-1.89.0/gramex/apps/init/default/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:38.000000 gramex-1.89.0/gramex/apps/init/default/$appname.py
--rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      592 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.89.0/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1144 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/.stylelintrc.js
--rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.89.0/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.975748 gramex-1.89.0/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/assets/README.template.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.987771 gramex-1.89.0/gramex/apps/init/default/error/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/error/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/error/401.html
--rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/error/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/error/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/error/500.html
--rw-rw-rw-   0        0        0    12057 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/init/default/favicon.ico
--rw-rw-rw-   0        0        0     2992 2022-10-02 08:02:34.000000 gramex-1.89.0/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0     2602 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.990764 gramex-1.89.0/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2604 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      304 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       77 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     2614 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.998291 gramex-1.89.0/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      377 2023-02-08 17:06:15.000000 gramex-1.89.0/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      199 2023-02-08 17:06:15.000000 gramex-1.89.0/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-02-08 17:06:15.000000 gramex-1.89.0/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.003301 gramex-1.89.0/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      199 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.010298 gramex-1.89.0/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.89.0/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.048684 gramex-1.89.0/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.89.0/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.89.0/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.89.0/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.89.0/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.89.0/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.89.0/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.89.0/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.89.0/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.89.0/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      775 2023-04-10 08:59:10.000000 gramex-1.89.0/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.89.0/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.055684 gramex-1.89.0/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.89.0/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.89.0/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.057680 gramex-1.89.0/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.89.0/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.069679 gramex-1.89.0/gramex/apps/pynode/
--rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/pynode/.snyk
--rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.89.0/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     2953 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.89.0/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.073676 gramex-1.89.0/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.89.0/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.89.0/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.094694 gramex-1.89.0/gramex/apps/ui/
--rw-rw-rw-   0        0        0     1019 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    12878 2022-12-20 15:16:57.000000 gramex-1.89.0/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2022-02-19 09:58:43.000000 gramex-1.89.0/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.89.0/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0   622531 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      341 2023-04-10 10:53:09.000000 gramex-1.89.0/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.89.0/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.107612 gramex-1.89.0/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.220064 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.89.0/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.89.0/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.361148 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.89.0/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.441225 gramex-1.89.0/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.89.0/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.444165 gramex-1.89.0/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.447173 gramex-1.89.0/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.89.0/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.457906 gramex-1.89.0/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.89.0/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.89.0/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.89.0/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.89.0/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.482342 gramex-1.89.0/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.498735 gramex-1.89.0/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     5540 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.504094 gramex-1.89.0/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.507096 gramex-1.89.0/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.509617 gramex-1.89.0/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.513607 gramex-1.89.0/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.516611 gramex-1.89.0/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.519629 gramex-1.89.0/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.522608 gramex-1.89.0/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.525627 gramex-1.89.0/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.528610 gramex-1.89.0/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.531626 gramex-1.89.0/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.534611 gramex-1.89.0/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.538677 gramex-1.89.0/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2023-01-07 08:41:00.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.541941 gramex-1.89.0/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.544957 gramex-1.89.0/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1766 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.89.0/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.564949 gramex-1.89.0/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.89.0/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.89.0/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.89.0/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      391 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/apps.yaml
--rw-rw-rw-   0        0        0    56930 2023-01-03 16:10:30.000000 gramex-1.89.0/gramex/cache.py
--rw-rw-rw-   0        0        0    34362 2023-02-09 09:15:32.000000 gramex-1.89.0/gramex/config.py
--rw-rw-rw-   0        0        0    93430 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/data.py
--rw-rw-rw-   0        0        0     6353 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.89.0/gramex/favicon.ico
--rw-rw-rw-   0        0        0    16330 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.717744 gramex-1.89.0/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     2499 2022-11-23 03:19:44.000000 gramex-1.89.0/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0    12772 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17394 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    61031 2023-04-03 08:25:14.000000 gramex-1.89.0/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    15648 2022-12-20 15:16:57.000000 gramex-1.89.0/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     1477 2022-11-06 08:24:25.000000 gramex-1.89.0/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0     8922 2022-11-06 08:24:26.000000 gramex-1.89.0/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14849 2023-02-24 08:15:32.000000 gramex-1.89.0/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.89.0/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-01-03 16:10:30.000000 gramex-1.89.0/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13238 2023-01-03 16:10:30.000000 gramex-1.89.0/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6622 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0    16154 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7193 2022-12-20 15:16:57.000000 gramex-1.89.0/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     6216 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7715 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.89.0/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11443 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9415 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.89.0/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/http.py
--rw-rw-rw-   0        0        0    34944 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.89.0/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-02-08 17:06:16.000000 gramex-1.89.0/gramex/migrate.py
--rw-rw-rw-   0        0        0    18498 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.740021 gramex-1.89.0/gramex/pptgen/
--rw-rw-rw-   0        0        0     9976 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18876 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.89.0/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.89.0/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.89.0/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26306 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.749532 gramex-1.89.0/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23501 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34484 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4208 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/pynode.py
--rw-rw-rw-   0        0        0     2985 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.773070 gramex-1.89.0/gramex/services/
--rw-rw-rw-   0        0        0    39415 2023-02-08 17:06:16.000000 gramex-1.89.0/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    10911 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3615 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-02-08 17:06:16.000000 gramex-1.89.0/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3668 2022-11-06 08:24:30.000000 gramex-1.89.0/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4529 2022-11-06 08:24:30.000000 gramex-1.89.0/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5762 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.787098 gramex-1.89.0/gramex/transforms/
--rw-rw-rw-   0        0        0      777 2022-11-23 04:49:14.000000 gramex-1.89.0/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.89.0/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.89.0/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32281 2023-04-10 11:33:47.000000 gramex-1.89.0/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10122 2022-11-06 08:24:30.000000 gramex-1.89.0/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.89.0/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:32.856179 gramex-1.89.0/gramex.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-04-10 11:35:29.000000 gramex-1.89.0/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12378 2023-04-10 11:35:32.000000 gramex-1.89.0/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 11:35:29.000000 gramex-1.89.0/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-04-10 11:35:29.000000 gramex-1.89.0/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      945 2023-04-10 11:35:29.000000 gramex-1.89.0/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 11:35:29.000000 gramex-1.89.0/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5972 2023-04-10 11:33:47.000000 gramex-1.89.0/pyproject.toml
--rw-rw-rw-   0        0        0      540 2023-04-10 11:35:33.922991 gramex-1.89.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 11:35:33.904984 gramex-1.89.0/tests/
--rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.89.0/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.89.0/tests/test_args.py
--rw-rw-rw-   0        0        0    38922 2023-04-10 11:33:47.000000 gramex-1.89.0/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.89.0/tests/test_cache.py
--rw-rw-rw-   0        0        0    15062 2022-11-23 04:49:14.000000 gramex-1.89.0/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.89.0/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.89.0/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.89.0/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2022-11-24 04:51:52.000000 gramex-1.89.0/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-01-03 16:10:30.000000 gramex-1.89.0/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.89.0/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.89.0/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    15699 2022-11-23 04:49:14.000000 gramex-1.89.0/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2022-11-23 04:49:14.000000 gramex-1.89.0/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.89.0/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.89.0/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.89.0/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2022-12-20 15:16:57.000000 gramex-1.89.0/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.89.0/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.89.0/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.89.0/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.89.0/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.89.0/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.89.0/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.89.0/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.89.0/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.89.0/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.89.0/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.89.0/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:28.145201 gramex-1.89.1/
+-rw-rw-rw-   0        0        0     1900 2023-04-10 11:33:47.000000 gramex-1.89.1/.gitignore
+-rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.89.1/LICENSE
+-rw-rw-rw-   0        0        0      620 2022-11-23 04:49:14.000000 gramex-1.89.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2956 2023-04-10 12:42:28.145201 gramex-1.89.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.89.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.099750 gramex-1.89.1/gramex/
+-rw-rw-rw-   0        0        0    15368 2023-04-10 12:40:48.000000 gramex-1.89.1/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.89.1/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.209204 gramex-1.89.1/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.89.1/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.217886 gramex-1.89.1/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.89.1/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-01-03 16:10:30.000000 gramex-1.89.1/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.264390 gramex-1.89.1/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      269 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/admin2/.eslintrc.js
+-rw-rw-rw-   0        0        0      226 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/apps/admin2/.snyk
+-rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.89.1/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12257 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0    12293 2023-04-10 12:35:57.000000 gramex-1.89.1/gramex/apps/admin2/package-lock.json
+-rw-rw-rw-   0        0        0      132 2022-02-19 10:03:02.000000 gramex-1.89.1/gramex/apps/admin2/package.json
+-rw-rw-rw-   0        0        0      231 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/admin2/rollup.config.js
+-rw-rw-rw-   0        0        0     4919 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/admin2/schedule.js
+-rw-rw-rw-   0        0        0     2505 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/admin2/schedule.src.js
+-rw-rw-rw-   0        0        0     3037 2022-02-19 10:03:02.000000 gramex-1.89.1/gramex/apps/admin2/schedule.template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.299046 gramex-1.89.1/gramex/apps/capture/
+-rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12034 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0   141593 2023-04-10 12:36:18.000000 gramex-1.89.1/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-02-08 17:06:15.000000 gramex-1.89.1/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.336322 gramex-1.89.1/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.89.1/gramex/apps/filemanager/.snyk
+-rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.89.1/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.89.1/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.89.1/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.89.1/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:24.936872 gramex-1.89.1/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.402017 gramex-1.89.1/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:38.000000 gramex-1.89.1/gramex/apps/init/default/$appname.py
+-rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/.flake8
+-rw-rw-rw-   0        0        0      592 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.89.1/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1144 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/.stylelintrc.js
+-rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.89.1/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.406853 gramex-1.89.1/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/assets/README.template.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.431897 gramex-1.89.1/gramex/apps/init/default/error/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/error/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/error/401.html
+-rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/error/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/error/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/error/500.html
+-rw-rw-rw-   0        0        0    12057 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/init/default/favicon.ico
+-rw-rw-rw-   0        0        0     2992 2022-10-02 08:02:34.000000 gramex-1.89.1/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0     2602 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.439928 gramex-1.89.1/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2604 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      304 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       77 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     2614 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.470052 gramex-1.89.1/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      377 2023-02-08 17:06:15.000000 gramex-1.89.1/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      199 2023-02-08 17:06:15.000000 gramex-1.89.1/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-02-08 17:06:15.000000 gramex-1.89.1/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.476861 gramex-1.89.1/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      199 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.491983 gramex-1.89.1/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.89.1/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.581259 gramex-1.89.1/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.89.1/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.89.1/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13287 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.89.1/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.89.1/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.89.1/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.89.1/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.89.1/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.89.1/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.89.1/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      775 2023-04-10 12:36:23.000000 gramex-1.89.1/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.89.1/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.604169 gramex-1.89.1/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.89.1/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.89.1/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.608254 gramex-1.89.1/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.89.1/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.678331 gramex-1.89.1/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/pynode/.snyk
+-rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.89.1/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     2953 2023-04-10 12:36:28.000000 gramex-1.89.1/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.89.1/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.687878 gramex-1.89.1/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.89.1/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.89.1/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.729244 gramex-1.89.1/gramex/apps/ui/
+-rw-rw-rw-   0        0        0     1019 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    12878 2022-12-20 15:16:57.000000 gramex-1.89.1/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2022-02-19 09:58:43.000000 gramex-1.89.1/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.89.1/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0   622531 2023-04-10 12:37:17.000000 gramex-1.89.1/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      341 2023-04-10 10:53:09.000000 gramex-1.89.1/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.89.1/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.762977 gramex-1.89.1/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.170487 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.89.1/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.89.1/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.550672 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.89.1/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.906237 gramex-1.89.1/gramex/apps/uifactory/
+-rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.89.1/gramex/apps/uifactory/.eslintrc.js
+-rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/.gitattributes
+-rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.912557 gramex-1.89.1/gramex/apps/uifactory/assets/
+-rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/assets/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.915975 gramex-1.89.1/gramex/apps/uifactory/assets/data/
+-rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.89.1/gramex/apps/uifactory/assets/data/input.json
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.946259 gramex-1.89.1/gramex/apps/uifactory/assets/img/
+-rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.89.1/gramex/apps/uifactory/assets/img/arrows-move.svg
+-rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.89.1/gramex/apps/uifactory/assets/img/clipboard.svg
+-rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
+-rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.89.1/gramex/apps/uifactory/assets/img/trash.svg
+-rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/create.html
+-rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/edit.html
+-rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/field-actions.html
+-rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.89.1/gramex/apps/uifactory/form_builder.py
+-rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/gramex.yaml
+-rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/index.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:26.983408 gramex-1.89.1/gramex/apps/uifactory/js/
+-rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/README.md
+-rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/embed.js
+-rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/fields.js
+-rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/fork-form.js
+-rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/index.js
+-rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/script.js
+-rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/utils.js
+-rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/js/viewform.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.050967 gramex-1.89.1/gramex/apps/uifactory/modals/
+-rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/modals/add-field.html
+-rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/modals/embed.html
+-rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/modals/remove.html
+-rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/modals/rename.html
+-rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/modals/themes.html
+-rw-rw-rw-   0        0        0     5540 2023-04-10 12:37:27.000000 gramex-1.89.1/gramex/apps/uifactory/package-lock.json
+-rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/uifactory/package.json
+-rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/popover-form.html
+-rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/sample.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.057493 gramex-1.89.1/gramex/apps/uifactory/snippets/
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.060503 gramex-1.89.1/gramex/apps/uifactory/snippets/button/
+-rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/button/bs4-button.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.063747 gramex-1.89.1/gramex/apps/uifactory/snippets/checkbox/
+-rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.066990 gramex-1.89.1/gramex/apps/uifactory/snippets/email/
+-rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/email/bs4-email.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.069990 gramex-1.89.1/gramex/apps/uifactory/snippets/hidden/
+-rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.071508 gramex-1.89.1/gramex/apps/uifactory/snippets/html/
+-rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/html/bs4-html.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.076329 gramex-1.89.1/gramex/apps/uifactory/snippets/multiselect/
+-rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.119703 gramex-1.89.1/gramex/apps/uifactory/snippets/number/
+-rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/number/bs4-number.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.123234 gramex-1.89.1/gramex/apps/uifactory/snippets/password/
+-rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/password/bs4-password.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.126764 gramex-1.89.1/gramex/apps/uifactory/snippets/radio/
+-rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.149198 gramex-1.89.1/gramex/apps/uifactory/snippets/range/
+-rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/range/bs4-range.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.165156 gramex-1.89.1/gramex/apps/uifactory/snippets/select/
+-rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/select/bs4-select.js
+-rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/setup.js
+-rw-rw-rw-   0        0        0        3 2023-01-07 08:41:00.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/snippets.json
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.170028 gramex-1.89.1/gramex/apps/uifactory/snippets/text/
+-rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/text/bs4-text.js
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.173397 gramex-1.89.1/gramex/apps/uifactory/snippets/textarea/
+-rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
+-rw-rw-rw-   0        0        0     1766 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/uifactory/style.scss
+-rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/template-navbar-view-form.html
+-rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/template-navbar.html
+-rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/toast.html
+-rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.89.1/gramex/apps/uifactory/viewform.html
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.189031 gramex-1.89.1/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.89.1/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.89.1/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.89.1/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      391 2023-04-10 12:40:48.000000 gramex-1.89.1/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    56930 2023-01-03 16:10:30.000000 gramex-1.89.1/gramex/cache.py
+-rw-rw-rw-   0        0        0    34362 2023-02-09 09:15:32.000000 gramex-1.89.1/gramex/config.py
+-rw-rw-rw-   0        0        0    93430 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/data.py
+-rw-rw-rw-   0        0        0     6353 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.89.1/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    16330 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.470743 gramex-1.89.1/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     2499 2022-11-23 03:19:44.000000 gramex-1.89.1/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0    12772 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17394 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    61031 2023-04-03 08:25:14.000000 gramex-1.89.1/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    15648 2022-12-20 15:16:57.000000 gramex-1.89.1/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     1477 2022-11-06 08:24:25.000000 gramex-1.89.1/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0     8922 2022-11-06 08:24:26.000000 gramex-1.89.1/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14849 2023-02-24 08:15:32.000000 gramex-1.89.1/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.89.1/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-01-03 16:10:30.000000 gramex-1.89.1/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13238 2023-01-03 16:10:30.000000 gramex-1.89.1/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6622 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0    16154 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7193 2022-12-20 15:16:57.000000 gramex-1.89.1/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     6216 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7715 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.89.1/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11443 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9415 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.89.1/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/http.py
+-rw-rw-rw-   0        0        0    34944 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.89.1/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-02-08 17:06:16.000000 gramex-1.89.1/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18498 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.520792 gramex-1.89.1/gramex/pptgen/
+-rw-rw-rw-   0        0        0     9976 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18876 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.89.1/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.89.1/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.89.1/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26306 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.533658 gramex-1.89.1/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23501 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34484 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4208 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2985 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.582886 gramex-1.89.1/gramex/services/
+-rw-rw-rw-   0        0        0    39415 2023-02-08 17:06:16.000000 gramex-1.89.1/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    10911 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3615 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-02-08 17:06:16.000000 gramex-1.89.1/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3668 2022-11-06 08:24:30.000000 gramex-1.89.1/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4529 2022-11-06 08:24:30.000000 gramex-1.89.1/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5762 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:27.601747 gramex-1.89.1/gramex/transforms/
+-rw-rw-rw-   0        0        0      777 2022-11-23 04:49:14.000000 gramex-1.89.1/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.89.1/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.89.1/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32281 2023-04-10 11:33:47.000000 gramex-1.89.1/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10122 2022-11-06 08:24:30.000000 gramex-1.89.1/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.89.1/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:25.203067 gramex-1.89.1/gramex.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-04-10 12:42:16.000000 gramex-1.89.1/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12378 2023-04-10 12:42:24.000000 gramex-1.89.1/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 12:42:16.000000 gramex-1.89.1/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-04-10 12:42:16.000000 gramex-1.89.1/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      945 2023-04-10 12:42:16.000000 gramex-1.89.1/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 12:42:16.000000 gramex-1.89.1/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5972 2023-04-10 12:40:48.000000 gramex-1.89.1/pyproject.toml
+-rw-rw-rw-   0        0        0      540 2023-04-10 12:42:28.161186 gramex-1.89.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 12:42:28.142194 gramex-1.89.1/tests/
+-rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.89.1/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.89.1/tests/test_args.py
+-rw-rw-rw-   0        0        0    38922 2023-04-10 11:33:47.000000 gramex-1.89.1/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.89.1/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15062 2022-11-23 04:49:14.000000 gramex-1.89.1/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.89.1/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.89.1/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.89.1/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2022-11-24 04:51:52.000000 gramex-1.89.1/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-01-03 16:10:30.000000 gramex-1.89.1/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.89.1/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.89.1/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    15699 2022-11-23 04:49:14.000000 gramex-1.89.1/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2022-11-23 04:49:14.000000 gramex-1.89.1/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.89.1/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.89.1/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.89.1/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2022-12-20 15:16:57.000000 gramex-1.89.1/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.89.1/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.89.1/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.89.1/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.89.1/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.89.1/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.89.1/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.89.1/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.89.1/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.89.1/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.89.1/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.89.1/tests/test_websockethandler.py
```

### Comparing `gramex-1.89.0/.gitignore` & `gramex-1.89.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/LICENSE` & `gramex-1.89.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/MANIFEST.in` & `gramex-1.89.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/PKG-INFO` & `gramex-1.89.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.89.0
+Version: 1.89.1
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.89.0/README.md` & `gramex-1.89.1/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/__init__.py` & `gramex-1.89.1/gramex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
 gramex complexity             Calculate cyclomatic complexity of the project
 '''
 
-__version__ = '1.89.0'
+__version__ = '1.89.1'
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
 paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
```

### Comparing `gramex-1.89.0/gramex/apps/admin2/gramex.yaml` & `gramex-1.89.1/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/gramexadmin.py` & `gramex-1.89.1/gramex/apps/admin2/gramexadmin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/index.html` & `gramex-1.89.1/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/package-lock.json` & `gramex-1.89.1/gramex/apps/admin2/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/schedule.js` & `gramex-1.89.1/gramex/apps/admin2/schedule.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/schedule.src.js` & `gramex-1.89.1/gramex/apps/admin2/schedule.src.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/admin2/schedule.template.html` & `gramex-1.89.1/gramex/apps/admin2/schedule.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/README.md` & `gramex-1.89.1/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/capture.js` & `gramex-1.89.1/gramex/apps/capture/capture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/chromecapture.js` & `gramex-1.89.1/gramex/apps/capture/chromecapture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/index.html` & `gramex-1.89.1/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/package-lock.json` & `gramex-1.89.1/gramex/apps/capture/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/capture/package.json` & `gramex-1.89.1/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/README.html` & `gramex-1.89.1/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.89.1/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.89.1/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/filemanager.html` & `gramex-1.89.1/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/filemanager.js` & `gramex-1.89.1/gramex/apps/filemanager/filemanager.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/filemanager.py` & `gramex-1.89.1/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/gramex.yaml` & `gramex-1.89.1/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/index.html` & `gramex-1.89.1/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/filemanager/navbar.html` & `gramex-1.89.1/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/.gitlab-ci.yml` & `gramex-1.89.1/gramex/apps/init/default/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/.stylelintrc.js` & `gramex-1.89.1/gramex/apps/init/default/.stylelintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/.template.gitignore` & `gramex-1.89.1/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/assets/README.template.md` & `gramex-1.89.1/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/error/400.html` & `gramex-1.89.1/gramex/apps/init/default/error/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/error/401.html` & `gramex-1.89.1/gramex/apps/init/default/error/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/error/403.html` & `gramex-1.89.1/gramex/apps/init/default/error/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/error/404.html` & `gramex-1.89.1/gramex/apps/init/default/error/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/error/500.html` & `gramex-1.89.1/gramex/apps/init/default/error/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/favicon.ico` & `gramex-1.89.1/gramex/apps/init/default/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.89.1/gramex/apps/init/default/gramex.template.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/index.template.html` & `gramex-1.89.1/gramex/apps/init/default/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/js/README.template.md` & `gramex-1.89.1/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/login.template.html` & `gramex-1.89.1/gramex/apps/init/default/login.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.89.1/gramex/apps/init/default/template-navbar.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/ide/index.template.html` & `gramex-1.89.1/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/init/minimal/index.template.html` & `gramex-1.89.1/gramex/apps/init/minimal/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/languagetool/README.md` & `gramex-1.89.1/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/languagetool/gramex.yaml` & `gramex-1.89.1/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/config.yaml` & `gramex-1.89.1/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/gramex.yaml` & `gramex-1.89.1/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/index.html` & `gramex-1.89.1/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/logviewer.py` & `gramex-1.89.1/gramex/apps/logviewer/logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.89.1/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/package-lock.json` & `gramex-1.89.1/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/render.js` & `gramex-1.89.1/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/logviewer/script.js` & `gramex-1.89.1/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/mail/index.html` & `gramex-1.89.1/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/mlhandler/template.html` & `gramex-1.89.1/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/pynode/index.js` & `gramex-1.89.1/gramex/apps/pynode/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/pynode/package-lock.json` & `gramex-1.89.1/gramex/apps/pynode/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/.snyk` & `gramex-1.89.1/gramex/apps/ui/.snyk`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/__init__.py` & `gramex-1.89.1/gramex/apps/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.89.1/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/config.yaml` & `gramex-1.89.1/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/gramex.yaml` & `gramex-1.89.1/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/gramexui.scss` & `gramex-1.89.1/gramex/apps/ui/gramexui.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/package-lock.json` & `gramex-1.89.1/gramex/apps/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/setup.js` & `gramex-1.89.1/gramex/apps/ui/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.89.1/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.89.1/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/default.png` & `gramex-1.89.1/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/index.html` & `gramex-1.89.1/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/sample.html` & `gramex-1.89.1/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.89.1/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/ui/theme/themes.json` & `gramex-1.89.1/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/.eslintrc.js` & `gramex-1.89.1/gramex/apps/uifactory/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/assets/data/input.json` & `gramex-1.89.1/gramex/apps/uifactory/assets/data/input.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/assets/img/arrows-move.svg` & `gramex-1.89.1/gramex/apps/uifactory/assets/img/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png` & `gramex-1.89.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/assets/img/trash.svg` & `gramex-1.89.1/gramex/apps/uifactory/assets/img/trash.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/create.html` & `gramex-1.89.1/gramex/apps/uifactory/create.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/edit.html` & `gramex-1.89.1/gramex/apps/uifactory/edit.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/field-actions.html` & `gramex-1.89.1/gramex/apps/uifactory/field-actions.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/form_builder.py` & `gramex-1.89.1/gramex/apps/uifactory/form_builder.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/gramex.yaml` & `gramex-1.89.1/gramex/apps/uifactory/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/index.html` & `gramex-1.89.1/gramex/apps/uifactory/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/README.md` & `gramex-1.89.1/gramex/apps/uifactory/js/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/fields.js` & `gramex-1.89.1/gramex/apps/uifactory/js/fields.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/fork-form.js` & `gramex-1.89.1/gramex/apps/uifactory/js/fork-form.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/index.js` & `gramex-1.89.1/gramex/apps/uifactory/js/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/script.js` & `gramex-1.89.1/gramex/apps/uifactory/js/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/utils.js` & `gramex-1.89.1/gramex/apps/uifactory/js/utils.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/js/viewform.js` & `gramex-1.89.1/gramex/apps/uifactory/js/viewform.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/modals/add-field.html` & `gramex-1.89.1/gramex/apps/uifactory/modals/add-field.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/modals/embed.html` & `gramex-1.89.1/gramex/apps/uifactory/modals/embed.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/modals/remove.html` & `gramex-1.89.1/gramex/apps/uifactory/modals/remove.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/modals/rename.html` & `gramex-1.89.1/gramex/apps/uifactory/modals/rename.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/modals/themes.html` & `gramex-1.89.1/gramex/apps/uifactory/modals/themes.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/package-lock.json` & `gramex-1.89.1/gramex/apps/uifactory/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/popover-form.html` & `gramex-1.89.1/gramex/apps/uifactory/popover-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/sample.html` & `gramex-1.89.1/gramex/apps/uifactory/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/button/bs4-button.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/button/bs4-button.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/email/bs4-email.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/email/bs4-email.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/number/bs4-number.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/number/bs4-number.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/range/bs4-range.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/range/bs4-range.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/select/bs4-select.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/select/bs4-select.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/setup.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/text/bs4-text.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/text/bs4-text.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js` & `gramex-1.89.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/style.scss` & `gramex-1.89.1/gramex/apps/uifactory/style.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/template-navbar-view-form.html` & `gramex-1.89.1/gramex/apps/uifactory/template-navbar-view-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/template-navbar.html` & `gramex-1.89.1/gramex/apps/uifactory/template-navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/uifactory/viewform.html` & `gramex-1.89.1/gramex/apps/uifactory/viewform.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/update/README.md` & `gramex-1.89.1/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/update/gramex.yaml` & `gramex-1.89.1/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/update/gramexupdate.py` & `gramex-1.89.1/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/apps/update/index.html` & `gramex-1.89.1/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/cache.py` & `gramex-1.89.1/gramex/cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/config.py` & `gramex-1.89.1/gramex/config.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/data.py` & `gramex-1.89.1/gramex/data.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/debug.py` & `gramex-1.89.1/gramex/debug.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/deploy.yaml` & `gramex-1.89.1/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/download.vega.js` & `gramex-1.89.1/gramex/download.vega.js`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/favicon.ico` & `gramex-1.89.1/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/gramex.yaml` & `gramex-1.89.1/gramex/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/400.html` & `gramex-1.89.1/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/401.html` & `gramex-1.89.1/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/403.html` & `gramex-1.89.1/gramex/handlers/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/404.html` & `gramex-1.89.1/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/500.html` & `gramex-1.89.1/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/__init__.py` & `gramex-1.89.1/gramex/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.89.1/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/auth.template.html` & `gramex-1.89.1/gramex/handlers/auth.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/authhandler.py` & `gramex-1.89.1/gramex/handlers/authhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/basehandler.py` & `gramex-1.89.1/gramex/handlers/basehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/capturehandler.py` & `gramex-1.89.1/gramex/handlers/capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/comichandler.py` & `gramex-1.89.1/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/drivehandler.py` & `gramex-1.89.1/gramex/handlers/drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/filehandler.py` & `gramex-1.89.1/gramex/handlers/filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/filehandler.template.html` & `gramex-1.89.1/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/formhandler.py` & `gramex-1.89.1/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/functionhandler.py` & `gramex-1.89.1/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/jsonhandler.py` & `gramex-1.89.1/gramex/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/mlhandler.py` & `gramex-1.89.1/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/modelhandler.py` & `gramex-1.89.1/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/openapiconfig.yaml` & `gramex-1.89.1/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/openapihandler.py` & `gramex-1.89.1/gramex/handlers/openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/pptxhandler.py` & `gramex-1.89.1/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/processhandler.py` & `gramex-1.89.1/gramex/handlers/processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/proxyhandler.py` & `gramex-1.89.1/gramex/handlers/proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/queryhandler.template.html` & `gramex-1.89.1/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/socialhandler.py` & `gramex-1.89.1/gramex/handlers/socialhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/uploadhandler.py` & `gramex-1.89.1/gramex/handlers/uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/handlers/websockethandler.py` & `gramex-1.89.1/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/http.py` & `gramex-1.89.1/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/install.py` & `gramex-1.89.1/gramex/install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/license.py` & `gramex-1.89.1/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/migrate.py` & `gramex-1.89.1/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/ml.py` & `gramex-1.89.1/gramex/ml.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/ml_api.py` & `gramex-1.89.1/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/__init__.py` & `gramex-1.89.1/gramex/pptgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/color.py` & `gramex-1.89.1/gramex/pptgen/color.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/colors.json` & `gramex-1.89.1/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/commands.py` & `gramex-1.89.1/gramex/pptgen/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/fonts.json` & `gramex-1.89.1/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/fontwidth.py` & `gramex-1.89.1/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen/utils.py` & `gramex-1.89.1/gramex/pptgen/utils.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen2/__init__.py` & `gramex-1.89.1/gramex/pptgen2/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen2/commands.py` & `gramex-1.89.1/gramex/pptgen2/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pptgen2/config.yaml` & `gramex-1.89.1/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/pynode.py` & `gramex-1.89.1/gramex/pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/scale.py` & `gramex-1.89.1/gramex/scale.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/secrets.py` & `gramex-1.89.1/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/servicenow.yaml` & `gramex-1.89.1/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/__init__.py` & `gramex-1.89.1/gramex/services/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/emailer.py` & `gramex-1.89.1/gramex/services/emailer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/rediscache.py` & `gramex-1.89.1/gramex/services/rediscache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/scheduler.py` & `gramex-1.89.1/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/sms.py` & `gramex-1.89.1/gramex/services/sms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/ttlcache.py` & `gramex-1.89.1/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/urlcache.py` & `gramex-1.89.1/gramex/services/urlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/services/watcher.py` & `gramex-1.89.1/gramex/services/watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/sm_api.py` & `gramex-1.89.1/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/topcause.py` & `gramex-1.89.1/gramex/topcause.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transformers.py` & `gramex-1.89.1/gramex/transformers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transforms/__init__.py` & `gramex-1.89.1/gramex/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transforms/auth.py` & `gramex-1.89.1/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transforms/template.py` & `gramex-1.89.1/gramex/transforms/template.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transforms/transforms.py` & `gramex-1.89.1/gramex/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/transforms/twitterstream.py` & `gramex-1.89.1/gramex/transforms/twitterstream.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex/winservice.py` & `gramex-1.89.1/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex.egg-info/PKG-INFO` & `gramex-1.89.1/gramex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.89.0
+Version: 1.89.1
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.89.0/gramex.egg-info/SOURCES.txt` & `gramex-1.89.1/gramex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/gramex.egg-info/requires.txt` & `gramex-1.89.1/gramex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/pyproject.toml` & `gramex-1.89.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.89.0"
+version = "1.89.1"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
```

### Comparing `gramex-1.89.0/setup.cfg` & `gramex-1.89.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_admin.py` & `gramex-1.89.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_alerts.py` & `gramex-1.89.1/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_args.py` & `gramex-1.89.1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_auth.py` & `gramex-1.89.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_cache.py` & `gramex-1.89.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_capturehandler.py` & `gramex-1.89.1/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_comichandler.py` & `gramex-1.89.1/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_drivehandler.py` & `gramex-1.89.1/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_filehandler.py` & `gramex-1.89.1/tests/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_filterhandler.py` & `gramex-1.89.1/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_formhandler.py` & `gramex-1.89.1/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_functionhandler.py` & `gramex-1.89.1/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_gramexlog.py` & `gramex-1.89.1/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_handlers.py` & `gramex-1.89.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_init.py` & `gramex-1.89.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_install.py` & `gramex-1.89.1/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_jsonhandler.py` & `gramex-1.89.1/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_ldapauth.py` & `gramex-1.89.1/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_logviewer.py` & `gramex-1.89.1/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_mlhandler.py` & `gramex-1.89.1/tests/test_mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_modelhandler.py` & `gramex-1.89.1/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_openapihandler.py` & `gramex-1.89.1/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_pptxhandler.py` & `gramex-1.89.1/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_processhandler.py` & `gramex-1.89.1/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_proxyhandler.py` & `gramex-1.89.1/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_pynode.py` & `gramex-1.89.1/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_schedule.py` & `gramex-1.89.1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_secrets.py` & `gramex-1.89.1/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_subprocess.py` & `gramex-1.89.1/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_translater.py` & `gramex-1.89.1/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_twitterresthandler.py` & `gramex-1.89.1/tests/test_twitterresthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_ui.py` & `gramex-1.89.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_update.py` & `gramex-1.89.1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_uploadhandler.py` & `gramex-1.89.1/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_watcher.py` & `gramex-1.89.1/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.89.0/tests/test_websockethandler.py` & `gramex-1.89.1/tests/test_websockethandler.py`

 * *Files identical despite different names*

