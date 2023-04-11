# Comparing `tmp/alphaz-0.7.3.7.tar.gz` & `tmp/alphaz-0.7.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.3.7.tar", last modified: Tue Apr 11 13:37:14 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.3.8.tar", last modified: Tue Apr 11 14:15:59 2023, max compression
```

## Comparing `alphaz-0.7.3.7.tar` & `alphaz-0.7.3.8.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.698631 alphaz-0.7.3.7/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8469 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 13:37:14.698631 alphaz-0.7.3.7/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.3.7/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.646631 alphaz-0.7.3.7/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      320 2023-03-23 07:52:23.000000 alphaz-0.7.3.7/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      662 2021-09-15 19:20:13.000000 alphaz-0.7.3.7/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.3.7/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.646631 alphaz-0.7.3.7/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.3.7/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.646631 alphaz-0.7.3.7/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2902 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.3.7/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.3.7/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.3.7/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.3.7/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.3.7/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.3.7/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.3.7/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.3.7/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.3.7/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.3.7/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.3.7/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.3.7/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.3.7/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.3.7/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8923 2022-08-31 08:56:44.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_api.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1284 2022-07-19 09:10:48.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5602 2022-07-19 09:10:48.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2215 2022-05-18 14:56:19.000000 alphaz-0.7.3.7/alphaz/documentations/docs/alpha_setup.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.3.7/alphaz/documentations/docs/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.3.7/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3505 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      440 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9286 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10320 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    47925 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_api/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.650631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18127 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    43708 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17969 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20160 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.626631 alphaz-0.7.3.7/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.654631 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24568 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13157 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25592 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.658631 alphaz-0.7.3.7/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    52508 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1081 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      200 2023-04-11 13:37:12.000000 alphaz-0.7.3.7/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.3.7/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.662631 alphaz-0.7.3.7/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5786 2023-03-24 12:18:56.000000 alphaz-0.7.3.7/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13997 2023-03-24 12:18:56.000000 alphaz-0.7.3.7/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.3.7/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9014 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.3.7/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5713 2023-04-08 19:15:15.000000 alphaz-0.7.3.7/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.662631 alphaz-0.7.3.7/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.3.7/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1096 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6170 2023-02-01 13:59:24.000000 alphaz-0.7.3.7/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.3.7/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.3.7/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.3.7/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.3.7/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6386 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.3.7/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.3.7/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.3.7/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.3.7/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.662631 alphaz-0.7.3.7/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.3.7/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.3.7/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.3.7/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.3.7/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.3.7/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.666631 alphaz-0.7.3.7/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.666631 alphaz-0.7.3.7/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.3.7/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.3.7/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.3.7/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.3.7/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.670631 alphaz-0.7.3.7/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.3.7/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.670631 alphaz-0.7.3.7/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.3.7/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      710 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.3.7/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.3.7/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.3.7/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18565 2023-03-29 19:05:00.000000 alphaz-0.7.3.7/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.3.7/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.3.7/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.3.7/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.670631 alphaz-0.7.3.7/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.3.7/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.3.7/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.670631 alphaz-0.7.3.7/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.3.7/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.3.7/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.3.7/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.3.7/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.3.7/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    53758 2023-03-16 19:44:05.000000 alphaz-0.7.3.7/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.3.7/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.3.7/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.3.7/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.3.7/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.670631 alphaz-0.7.3.7/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.3.7/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.3.7/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.3.7/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.3.7/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.3.7/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.3.7/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.3.7/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26166 2023-04-07 09:47:18.000000 alphaz-0.7.3.7/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.3.7/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.3.7/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.3.7/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.3.7/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4125 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13011 2023-03-24 12:18:56.000000 alphaz-0.7.3.7/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6334 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.3.7/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.3.7/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2022-05-14 15:57:01.000000 alphaz-0.7.3.7/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.3.7/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.3.7/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.674631 alphaz-0.7.3.7/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.678631 alphaz-0.7.3.7/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.678631 alphaz-0.7.3.7/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.678631 alphaz-0.7.3.7/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.686631 alphaz-0.7.3.7/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.626631 alphaz-0.7.3.7/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.3.7/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.7/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.3.7/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.3.7/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.3.7/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.3.7/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.694631 alphaz-0.7.3.7/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.3.7/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.3.7/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.3.7/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.698631 alphaz-0.7.3.7/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.3.7/alphaz/utils/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.3.7/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.3.7/alphaz/utils/configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.3.7/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.3.7/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.3.7/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.3.7/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.3.7/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.3.7/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.3.7/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 13:37:14.646631 alphaz-0.7.3.7/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9706 2023-04-11 13:37:14.000000 alphaz-0.7.3.7/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      447 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-11 13:37:13.000000 alphaz-0.7.3.7/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-11 13:37:14.698631 alphaz-0.7.3.7/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3075 2023-04-11 13:36:15.000000 alphaz-0.7.3.7/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8469 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.3.8/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.877067 alphaz-0.7.3.8/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      320 2023-03-23 07:52:23.000000 alphaz-0.7.3.8/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      662 2021-09-15 19:20:13.000000 alphaz-0.7.3.8/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.3.8/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2902 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.3.8/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.3.8/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.3.8/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.3.8/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.3.8/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8923 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_api.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1284 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5602 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2215 2022-05-18 14:56:19.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_setup.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/documentations/docs/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.3.8/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3505 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      440 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9286 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10320 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    47925 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18127 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    43708 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17969 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20160 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.873067 alphaz-0.7.3.8/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.889067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.889067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24568 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13157 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25592 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    52508 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1081 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      200 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.3.8/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5786 2023-03-24 12:18:56.000000 alphaz-0.7.3.8/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13997 2023-03-24 12:18:56.000000 alphaz-0.7.3.8/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.3.8/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9014 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.3.8/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6222 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.3.8/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1096 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.3.8/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.3.8/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6386 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.3.8/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.3.8/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.3.8/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.3.8/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.3.8/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.3.8/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.3.8/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.3.8/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      710 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.3.8/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.3.8/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.3.8/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18565 2023-03-29 19:05:00.000000 alphaz-0.7.3.8/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.3.8/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.3.8/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.3.8/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.3.8/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.3.8/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.3.8/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.3.8/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    53758 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.3.8/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.3.8/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.3.8/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.3.8/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.3.8/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.3.8/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    26166 2023-04-07 09:47:18.000000 alphaz-0.7.3.8/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.3.8/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.3.8/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.3.8/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13445 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6927 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.3.8/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.3.8/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.921067 alphaz-0.7.3.8/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.873067 alphaz-0.7.3.8/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.3.8/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.3.8/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.3.8/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.3.8/alphaz/utils/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.3.8/alphaz/utils/configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.3.8/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.3.8/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.877067 alphaz-0.7.3.8/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9706 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      447 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3075 2023-04-11 14:15:53.000000 alphaz-0.7.3.8/setup.py
```

### Comparing `alphaz-0.7.3.7/MANIFEST.in` & `alphaz-0.7.3.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/PKG-INFO` & `alphaz-0.7.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.7
+Version: 0.7.3.8
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.7.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.8.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.7/README.md` & `alphaz-0.7.3.8/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/api.json` & `alphaz-0.7.3.8/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/api.py` & `alphaz-0.7.3.8/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/mails.py` & `alphaz-0.7.3.8/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/admin.py` & `alphaz-0.7.3.8/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/api.py` & `alphaz-0.7.3.8/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.3.8/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/database.py` & `alphaz-0.7.3.8/alphaz/apis/routes/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/logs.py` & `alphaz-0.7.3.8/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/mails.py` & `alphaz-0.7.3.8/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/main.py` & `alphaz-0.7.3.8/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/tests.py` & `alphaz-0.7.3.8/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.3.8/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.3.8/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.3.8/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.3.8/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/routes/users.py` & `alphaz-0.7.3.8/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/tests.py` & `alphaz-0.7.3.8/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/users/ldap.py` & `alphaz-0.7.3.8/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/apis/users/users.py` & `alphaz-0.7.3.8/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config/config.css` & `alphaz-0.7.3.8/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config/config.html` & `alphaz-0.7.3.8/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config/main_configuration.py` & `alphaz-0.7.3.8/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config/page.py` & `alphaz-0.7.3.8/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config/source.html` & `alphaz-0.7.3.8/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/config.json` & `alphaz-0.7.3.8/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/alpha_api.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_api.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/alpha_database.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/docs/index.md` & `alphaz-0.7.3.8/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/404.html` & `alphaz-0.7.3.8/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_api/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_database/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/index.html` & `alphaz-0.7.3.8/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.3.8/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/index.html` & `alphaz-0.7.3.8/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/api_lib.py` & `alphaz-0.7.3.8/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/barcode_lib.py` & `alphaz-0.7.3.8/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/config_lib.py` & `alphaz-0.7.3.8/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/converter_lib.py` & `alphaz-0.7.3.8/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/database_lib.py` & `alphaz-0.7.3.8/alphaz/libs/database_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/date_lib.py` & `alphaz-0.7.3.8/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/dict_lib.py` & `alphaz-0.7.3.8/alphaz/libs/dict_lib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Iterable, List
+import dictdiffer
+from typing import Iterable, List, Union
 
 
 def sort_dict(x, value=False, reverse=False):
     sorted_x = {
         x: y
         for x, y in sorted(
             x.items(), key=lambda kv: kv[1 if value else 0], reverse=reverse
@@ -194,7 +195,28 @@
 def get_nested_dictionary_keys(d: dict) -> List[str]:
     keys = []
     for k, v in d.items():
         keys.append(k)
         if isinstance(v, dict):
             keys.extend(get_nested_dictionary_keys(v))
     return set(keys)
+
+
+def dict_diff(dict_1: dict, dict2: dict) -> List[any]:
+    return [diff for diff in list(dictdiffer.diff(dict_1, dict2))]
+
+
+def get_dicts_diff(dict_1: Union[dict, List[dict]], dict_2: Union[dict, List[dict]]):
+
+    if isinstance(dict_1, dict):
+        dict_1 = [dict_1]
+
+    if isinstance(dict_2, dict):
+        dict_2 = [dict_2]
+
+    return [
+        {
+            "item": i,
+            "diff": dict_diff(dict_1[i], dict_2[i]),
+        }
+        for i in range(len(dict_2))
+    ]
```

### Comparing `alphaz-0.7.3.7/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.3.8/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/events.py` & `alphaz-0.7.3.8/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/files_lib.py` & `alphaz-0.7.3.8/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/flask_lib.py` & `alphaz-0.7.3.8/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/img_lib.py` & `alphaz-0.7.3.8/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/io_lib.py` & `alphaz-0.7.3.8/alphaz/libs/io_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     with open(filename, "w", encoding="utf-8") as f:
         f.write(json_content)
         # json.dump(data, f)
 
 
 def read_json(file_path, log=None):
     data = {}
-    with open(file_path, encoding="utf-8") as json_data_file:
-        data = json.load(json_data_file)
+    if os.path.exists(file_path):
+        with open(file_path, encoding="utf-8") as json_data_file:
+            data = json.load(json_data_file)
     return data
 
     original = {}
 
     with open(file_path, "r", encoding="utf-8") as f:
         original = f.read()
     # save state
```

### Comparing `alphaz-0.7.3.7/alphaz/libs/json_lib.py` & `alphaz-0.7.3.8/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/logs_lib.py` & `alphaz-0.7.3.8/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/mail_lib.py` & `alphaz-0.7.3.8/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/notifications_lib.py` & `alphaz-0.7.3.8/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/number_lib.py` & `alphaz-0.7.3.8/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/process_lib.py` & `alphaz-0.7.3.8/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/py_lib.py` & `alphaz-0.7.3.8/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/scp_lib.py` & `alphaz-0.7.3.8/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/search_lib.py` & `alphaz-0.7.3.8/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/secure_lib.py` & `alphaz-0.7.3.8/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/soap_lib.py` & `alphaz-0.7.3.8/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/ssh_lib.py` & `alphaz-0.7.3.8/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/string_lib.py` & `alphaz-0.7.3.8/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/test_lib.py` & `alphaz-0.7.3.8/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/time_lib.py` & `alphaz-0.7.3.8/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/transactions_lib.py` & `alphaz-0.7.3.8/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/user_lib.py` & `alphaz-0.7.3.8/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.3.8/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.3.8/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.3.8/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.3.8/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Images/Background.png` & `alphaz-0.7.3.8/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.3.8/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.3.8/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.3.8/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Mail.png` & `alphaz-0.7.3.8/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/Webmail.html` & `alphaz-0.7.3.8/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/debug.html` & `alphaz-0.7.3.8/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/mail.html` & `alphaz-0.7.3.8/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/password_reset.html` & `alphaz-0.7.3.8/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.3.8/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_answer.py` & `alphaz-0.7.3.8/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_colorations.py` & `alphaz-0.7.3.8/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_parameter.py` & `alphaz-0.7.3.8/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_requests.py` & `alphaz-0.7.3.8/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_route.py` & `alphaz-0.7.3.8/alphaz/models/api/_route.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_structures.py` & `alphaz-0.7.3.8/alphaz/models/api/_structures.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/api/_utils.py` & `alphaz-0.7.3.8/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/config/_config.py` & `alphaz-0.7.3.8/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/config/_utils.py` & `alphaz-0.7.3.8/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/main_definitions.py` & `alphaz-0.7.3.8/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/models.py` & `alphaz-0.7.3.8/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/operators.py` & `alphaz-0.7.3.8/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/requests.py` & `alphaz-0.7.3.8/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/row.py` & `alphaz-0.7.3.8/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/structure.py` & `alphaz-0.7.3.8/alphaz/models/database/structure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/tests.py` & `alphaz-0.7.3.8/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/users_definitions.py` & `alphaz-0.7.3.8/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/utils.py` & `alphaz-0.7.3.8/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/database/views.py` & `alphaz-0.7.3.8/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/excel.py` & `alphaz-0.7.3.8/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/ftp.py` & `alphaz-0.7.3.8/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/json/_converters.py` & `alphaz-0.7.3.8/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/logger/_colorations.py` & `alphaz-0.7.3.8/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/logger/_logger.py` & `alphaz-0.7.3.8/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/logger/_utils.py` & `alphaz-0.7.3.8/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/logs/main.log` & `alphaz-0.7.3.8/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/main/_base.py` & `alphaz-0.7.3.8/alphaz/models/main/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/main/_core/_core.py` & `alphaz-0.7.3.8/alphaz/models/main/_core/_core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/main/_exception.py` & `alphaz-0.7.3.8/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/main/_request.py` & `alphaz-0.7.3.8/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/main/_singleton.py` & `alphaz-0.7.3.8/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/request.py` & `alphaz-0.7.3.8/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_category.py` & `alphaz-0.7.3.8/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_group.py` & `alphaz-0.7.3.8/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_method.py` & `alphaz-0.7.3.8/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_save.py` & `alphaz-0.7.3.8/alphaz/models/tests/_save.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # MODULES
 import os
-from typing import Any
+import json
+from pathlib import Path
+from typing import Any, Callable
+
+# MODELS
+from ...models.main import dataclass
 
 # LIBS
-from ...libs.io_lib import archive_object, unarchive_object
+from ...libs.io_lib import archive_object, unarchive_object, read_json, save_as_json
 
 # CORE
 from core import core
 
 
 def get_default_save_root() -> str:
     """
@@ -24,33 +29,38 @@
         default_root = (
             core.config.get("directories/tmp", "tmp")
             + os.sep
             + "tests"
             + os.sep
             + "saves"
         )
-    return default_root
+    return Path(default_root)
 
 
 class AlphaSave:
     """
     Utility class for saving and loading objects to/from files.
     """
 
-    def __init__(self, root: str = None, ext: str = ".ast"):
+    def __init__(self, root: Path = None, ext: str = ".ast"):
         """
         Initializes a new AlphaSave object with the specified root directory and file extension.
 
         Args:
             root: The root directory to save files to.
             ext: The file extension to use for saved files.
         """
+
         self.root = root or self.get_default_save_root()
         self.ext = ext
 
+    @property
+    def is_ext_json(self):
+        return self.ext == ".json"
+
     def get_default_save_root(self) -> str:
         """
         Get the default root directory for saving test files.
 
         If the "directories/tests/saves" configuration value is set, it will be used as the default root directory.
         Otherwise, the "directories/tmp" configuration value is used with "tests/saves" appended to the end.
 
@@ -62,15 +72,15 @@
             default_root = (
                 core.config.get("directories/tmp", "tmp")
                 + os.sep
                 + "tests"
                 + os.sep
                 + "saves"
             )
-        return default_root
+        return Path(default_root)
 
     def set_root(self, root: str):
         """
         Set the root directory for saving files.
 
         Args:
             root: The new root directory to use for saving files.
@@ -99,19 +109,24 @@
 
         Args:
             object_to_save: The object to save.
             filename: The name of the file to save the object to.
             class_name: The name of the class to save the object under.
         """
         file_path = self.get_file_path(filename, class_name)
+        if os.path.exists(file_path):
+            return None
+
         directory = os.path.dirname(file_path)
         os.makedirs(directory, exist_ok=True)
-        archive_object(object_to_save, file_path)
+        if self.is_ext_json:
+            return save_as_json(filename=file_path, data=object_to_save)
+
+        return archive_object(object_to_save, file_path)
 
-    @staticmethod
     def load(
         self,
         filename: str,
         class_name: str,
     ) -> Any:
         """
         Load an object from a file.
@@ -122,8 +137,12 @@
             filename: A string representing the name of the file to load.
             class_name: A string representing the name of the class to which the object belongs.
 
         Returns:
             The object loaded from the file.
         """
         file_path = self.get_file_path(filename, class_name)
+
+        if self.is_ext_json:
+            return read_json(file_path=file_path)
+
         return unarchive_object(file_path)
```

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_test.py` & `alphaz-0.7.3.8/alphaz/models/tests/_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -270,23 +270,37 @@
         self,
         a,
         b,
         ignore: list | dict = None,
         conditions: List[bool] = [],
         msg: str = "",
     ) -> bool:
-        if type(a) == dict and type(b) == dict:
+        if (
+            isinstance(a, list)
+            and isinstance(b, list)
+            and all(isinstance(item, dict) for item in a)
+            and all(isinstance(item, dict) for item in b)
+        ):
+            return [
+                self.assert_equal(
+                    a=item, b=b[index], ignore=ignore, conditions=conditions, msg=msg
+                )
+                for index, item in enumerate(a)
+            ]
+
+        elif type(a) == dict and type(b) == dict:
             diff = dict_lib.compare_dicts(a, b, ignore=ignore)
 
             status = diff is None
             if not status:
                 LOG.info(
                     f"{self.current_test_name} {msg} - Assert: dict are not equals\n"
                 )
                 print("\n", dict_lib.show_dict(diff))
+
         else:
             status = a == b
             if not status:
                 LOG.info(
                     f"{self.current_test_name} {msg} - Assert: {a} and {b} are not equals"
                 )
         return self._assert(status, conditions)
```

### Comparing `alphaz-0.7.3.7/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.3.8/alphaz/models/tests/_wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # MODULES
 from typing import List, Dict, Callable, Any
+from pathlib import Path
 
 # LOCALS
 from ...apis.users.users import try_su_login, logout_su
 from ..main import AlphaException
+from ...models.tests import AlphaTest
+from ...libs import dict_lib
 
 from ._levels import Levels
 from ._save import AlphaSave
 
 TEST_METHOD_NAME = "test_alpha_in"
 
 
@@ -37,16 +40,20 @@
         # Otherwise, call the function directly.
         return fct(*args, **kwargs)
 
 
 def test(
     mandatory: bool = False,
     save: bool = False,
+    save_ext: str = ".ast",
+    save_path: Path = None,
     begin: Callable = None,
     end: Callable = None,
+    save_post_process: Callable = None,
+    return_diff: bool = False,
     begin_args: list = None,
     begin_kwargs: Dict[str, Any] = None,
     end_args: list = None,
     end_kwargs: Dict[str, Any] = None,
     description: str = None,
     stop: bool = True,
     disable: bool = False,
@@ -78,44 +85,58 @@
 
     Returns:
         A wrapper function which performs pre- and post-processing before and after running the test function.
     """
 
     def test_alpha_in(func: Callable) -> Callable:
         def test_wrapper(*args, **kwargs):
-            TestClass = args[0]
+            TestClass: AlphaTest = args[0]
             TestClass.output = None
 
             logged_output = None
             if admin_user_id is not None or admin_user_name is not None:
                 logged_output = try_su_login(
                     admin_user_id if admin_user_id is not None else admin_user_name
                 )
                 if logged_output is None:
                     raise AlphaException("Unable to auth as an admin")
 
-            alpha_save = AlphaSave()
             if begin:
-                __call_fct(begin, TestClass, begin_args, begin_kwargs)
+                call_function(begin, TestClass, begin_args, begin_kwargs)
+
+            output = func(*args, **kwargs)
+
             if save:
+                alpha_save = AlphaSave(root=save_path, ext=save_ext)
                 return_save = alpha_save.load(
-                    func.__name__,
-                    TestClass.__class__.__name__,
+                    filename=func.__name__,
+                    class_name=TestClass.__class__.__name__,
                 )
-            output = func(*args, **kwargs)
-            if save and return_save is None:
-                alpha_save.save(output, func.__name__, TestClass.__class__.__name__)
-                output = True
-            elif save and return_save != output:
-                raise AlphaException(
-                    f"Saved test output and actual output are not similar:\n{output}\n\nVS{return_save}"
+
+                alpha_save.save(
+                    object_to_save=output,
+                    filename=func.__name__,
+                    class_name=TestClass.__class__.__name__,
+                )
+
+                return_save = (
+                    save_post_process(output, return_save)
+                    if save_post_process is not None
+                    else return_save
                 )
 
+                if return_diff:
+                    TestClass.outputs["dicts_diff"] = dict_lib.get_dicts_diff(
+                        dict_1=output, dict_2=return_save
+                    )
+                    
+                TestClass.assert_equal(return_save, output)
+
             if end:
-                __call_fct(end, TestClass, end_args, end_kwargs)
+                call_function(end, TestClass, end_args, end_kwargs)
 
             if logged_output is not None:
                 logout_su()
 
             if TestClass.output is not None:
                 # When using assertions
                 TestClass.outputs[func.__name__] = TestClass.output
```

### Comparing `alphaz-0.7.3.7/alphaz/models/user.py` & `alphaz-0.7.3.8/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/models/watcher.py` & `alphaz-0.7.3.8/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/pocs/main.py` & `alphaz-0.7.3.8/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/run.py` & `alphaz-0.7.3.8/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/src/alpha.png` & `alphaz-0.7.3.8/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/src/configs/loggers.json` & `alphaz-0.7.3.8/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/stitch/Core.py` & `alphaz-0.7.3.8/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/stitch/stitch.py` & `alphaz-0.7.3.8/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.3.8/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.3.8/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/css/home.css` & `alphaz-0.7.3.8/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.3.8/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.3.8/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.3.8/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.3.8/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.3.8/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/home.html` & `alphaz-0.7.3.8/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/templates/logs.html` & `alphaz-0.7.3.8/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/test.py` & `alphaz-0.7.3.8/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/tests/api.py` & `alphaz-0.7.3.8/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/tests/basic_test.py` & `alphaz-0.7.3.8/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/tests/configurations.py` & `alphaz-0.7.3.8/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/tests/database.py` & `alphaz-0.7.3.8/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/tests/utils.py` & `alphaz-0.7.3.8/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/api.py` & `alphaz-0.7.3.8/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/configuration.py` & `alphaz-0.7.3.8/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.3.8/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/decorators.py` & `alphaz-0.7.3.8/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/ensure.py` & `alphaz-0.7.3.8/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/mep.py` & `alphaz-0.7.3.8/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/screens.py` & `alphaz-0.7.3.8/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/selectionMenu.py` & `alphaz-0.7.3.8/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/tasks.py` & `alphaz-0.7.3.8/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/tests.py` & `alphaz-0.7.3.8/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/time.py` & `alphaz-0.7.3.8/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz/utils/transactions.py` & `alphaz-0.7.3.8/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.3.8/alphaz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.7
+Version: 0.7.3.8
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.7.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.8.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.7/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.3.8/alphaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.7/setup.py` & `alphaz-0.7.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.3.7"
+version = "0.7.3.8"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

